# Comparing `tmp/splotify-0.1.0.tar.gz` & `tmp/Splotify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splotify-0.1.0.tar", last modified: Sun Mar 26 15:55:28 2023, max compression
+gzip compressed data, was "dist/Splotify-0.1.1.tar", last modified: Fri May  5 04:04:55 2023, max compression
```

## Comparing `splotify-0.1.0.tar` & `Splotify-0.1.1.tar`

### file list

```diff
@@ -1,79 +1,73 @@
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.087050 splotify-0.1.0/
--rw-r--r--   0 liachen    (501) staff       (20)      297 2023-03-26 15:27:50.000000 splotify-0.1.0/.bumpversion.cfg
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.015963 splotify-0.1.0/.github/
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.023111 splotify-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 liachen    (501) staff       (20)      834 2023-03-26 03:19:47.000000 splotify-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 liachen    (501) staff       (20)      595 2023-03-26 03:19:47.000000 splotify-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 liachen    (501) staff       (20)      118 2023-03-26 03:19:47.000000 splotify-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.029420 splotify-0.1.0/.github/workflows/
--rw-r--r--   0 liachen    (501) staff       (20)     1272 2023-03-26 03:19:47.000000 splotify-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 liachen    (501) staff       (20)     1808 2023-03-26 03:19:47.000000 splotify-0.1.0/.gitignore
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.033473 splotify-0.1.0/.vscode/
--rw-r--r--   0 liachen    (501) staff       (20)      172 2023-03-26 03:19:47.000000 splotify-0.1.0/.vscode/settings.json
--rw-r--r--   0 liachen    (501) staff       (20)      749 2023-03-26 15:20:37.000000 splotify-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 liachen    (501) staff       (20)    11357 2023-03-26 03:19:47.000000 splotify-0.1.0/LICENSE
--rw-r--r--   0 liachen    (501) staff       (20)      169 2023-03-26 15:51:18.000000 splotify-0.1.0/MANIFEST.in
--rw-r--r--   0 liachen    (501) staff       (20)      564 2023-03-26 15:27:50.000000 splotify-0.1.0/Makefile
--rw-r--r--   0 liachen    (501) staff       (20)    16295 2023-03-26 15:55:28.086730 splotify-0.1.0/PKG-INFO
--rw-r--r--   0 liachen    (501) staff       (20)     2470 2023-03-26 15:20:37.000000 splotify-0.1.0/README.md
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.037017 splotify-0.1.0/examples/
--rw-r--r--   0 liachen    (501) staff       (20)   112044 2023-03-26 15:20:37.000000 splotify-0.1.0/examples/radiohead_box_plot.png
--rw-r--r--   0 liachen    (501) staff       (20)    91188 2023-03-26 15:20:37.000000 splotify-0.1.0/examples/radiohead_pie_chart.png
--rw-r--r--   0 liachen    (501) staff       (20)    74775 2023-03-26 15:20:37.000000 splotify-0.1.0/examples/radiohead_scatter_plot.png
--rw-r--r--   0 liachen    (501) staff       (20)     1454 2023-03-26 15:49:57.000000 splotify-0.1.0/pyproject.toml
--rw-r--r--   0 liachen    (501) staff       (20)      172 2023-03-26 15:20:37.000000 splotify-0.1.0/requirements.txt
--rw-r--r--   0 liachen    (501) staff       (20)       38 2023-03-26 15:55:28.087154 splotify-0.1.0/setup.cfg
--rw-r--r--   0 liachen    (501) staff       (20)       38 2023-03-26 03:19:47.000000 splotify-0.1.0/setup.py
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.042242 splotify-0.1.0/splotify/
--rw-r--r--   0 liachen    (501) staff       (20)       22 2023-03-26 15:27:50.000000 splotify-0.1.0/splotify/__init__.py
--rw-r--r--   0 liachen    (501) staff       (20)     1713 2023-03-26 15:20:37.000000 splotify-0.1.0/splotify/data.py
--rw-r--r--   0 liachen    (501) staff       (20)     2042 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/helpers.py
--rw-r--r--   0 liachen    (501) staff       (20)        0 2023-03-26 04:59:47.000000 splotify-0.1.0/splotify/main.py
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.050826 splotify-0.1.0/splotify/plots/
--rw-r--r--   0 liachen    (501) staff       (20)        0 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/plots/___init__.py
--rw-r--r--   0 liachen    (501) staff       (20)        0 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/plots/audioanalysis.py
--rw-r--r--   0 liachen    (501) staff       (20)     4394 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/plots/audiofeatures.py
--rw-r--r--   0 liachen    (501) staff       (20)      747 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/plots/category.py
--rw-r--r--   0 liachen    (501) staff       (20)        0 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/plots/timeline.py
--rw-r--r--   0 liachen    (501) staff       (20)     1349 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/spotifyapi.py
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.057972 splotify-0.1.0/splotify/tests/
--rw-r--r--   0 liachen    (501) staff       (20)      153 2023-03-26 03:35:13.000000 splotify-0.1.0/splotify/tests/__init__.py
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:27.997826 splotify-0.1.0/splotify/tests/cassettes/
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.066268 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_box_plot.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_histogram.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d_average.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d_average.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_select_features.yaml
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.071861 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/
--rw-r--r--   0 liachen    (501) staff       (20)   113096 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/test_add_albums.yaml
--rw-r--r--   0 liachen    (501) staff       (20)   440329 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/test_add_playlists.yaml
--rw-r--r--   0 liachen    (501) staff       (20)   100792 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/test_add_tracks.yaml
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.074268 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_helpers/
--rw-r--r--   0 liachen    (501) staff       (20)    17003 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_helpers/test_my_id.yaml
--rw-r--r--   0 liachen    (501) staff       (20)    25309 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_helpers/test_search_id.yaml
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.075824 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_integration/
--rw-r--r--   0 liachen    (501) staff       (20)   171216 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_integration/test_integration.yaml
--rw-r--r--   0 liachen    (501) staff       (20)     3761 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/conftest.py
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.085415 splotify-0.1.0/splotify/tests/expected_plot_outputs/
--rw-r--r--   0 liachen    (501) staff       (20)    22294 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_bar_chart.png
--rw-r--r--   0 liachen    (501) staff       (20)    37166 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_box_plot.png
--rw-r--r--   0 liachen    (501) staff       (20)    29434 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_histogram.png
--rw-r--r--   0 liachen    (501) staff       (20)    33495 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_pie_chart.png
--rw-r--r--   0 liachen    (501) staff       (20)    38658 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_and_integration.png
--rw-r--r--   0 liachen    (501) staff       (20)    34973 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_average.png
--rw-r--r--   0 liachen    (501) staff       (20)    93897 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_3d.png
--rw-r--r--   0 liachen    (501) staff       (20)    81566 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_3d_average.png
--rw-r--r--   0 liachen    (501) staff       (20)     1451 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/test_audiofeatures.py
--rw-r--r--   0 liachen    (501) staff       (20)      314 2023-03-26 03:19:47.000000 splotify-0.1.0/splotify/tests/test_category.py
--rw-r--r--   0 liachen    (501) staff       (20)     2442 2023-03-26 15:20:37.000000 splotify-0.1.0/splotify/tests/test_data.py
--rw-r--r--   0 liachen    (501) staff       (20)     1647 2023-03-26 15:16:11.000000 splotify-0.1.0/splotify/tests/test_helpers.py
--rw-r--r--   0 liachen    (501) staff       (20)      694 2023-03-26 15:20:37.000000 splotify-0.1.0/splotify/tests/test_integration.py
-drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-03-26 15:55:28.045719 splotify-0.1.0/splotify.egg-info/
--rw-r--r--   0 liachen    (501) staff       (20)    16295 2023-03-26 15:55:27.000000 splotify-0.1.0/splotify.egg-info/PKG-INFO
--rw-r--r--   0 liachen    (501) staff       (20)     2534 2023-03-26 15:55:27.000000 splotify-0.1.0/splotify.egg-info/SOURCES.txt
--rw-r--r--   0 liachen    (501) staff       (20)        1 2023-03-26 15:55:27.000000 splotify-0.1.0/splotify.egg-info/dependency_links.txt
--rw-r--r--   0 liachen    (501) staff       (20)      247 2023-03-26 15:55:27.000000 splotify-0.1.0/splotify.egg-info/requires.txt
--rw-r--r--   0 liachen    (501) staff       (20)        9 2023-03-26 15:55:27.000000 splotify-0.1.0/splotify.egg-info/top_level.txt
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.069754 Splotify-0.1.1/
+-rw-r--r--   0 liachen    (501) staff       (20)      297 2023-05-05 04:00:35.000000 Splotify-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 liachen    (501) staff       (20)      749 2023-05-05 03:58:30.000000 Splotify-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 liachen    (501) staff       (20)    11357 2023-05-05 03:58:30.000000 Splotify-0.1.1/LICENSE
+-rw-r--r--   0 liachen    (501) staff       (20)      169 2023-05-05 03:58:30.000000 Splotify-0.1.1/MANIFEST.in
+-rw-r--r--   0 liachen    (501) staff       (20)      926 2023-05-05 03:58:30.000000 Splotify-0.1.1/Makefile
+-rw-r--r--   0 liachen    (501) staff       (20)    16934 2023-05-05 04:04:55.069236 Splotify-0.1.1/PKG-INFO
+-rw-r--r--   0 liachen    (501) staff       (20)     3109 2023-05-05 03:58:30.000000 Splotify-0.1.1/README.md
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.022722 Splotify-0.1.1/Splotify.egg-info/
+-rw-r--r--   0 liachen    (501) staff       (20)    16934 2023-05-05 04:04:54.000000 Splotify-0.1.1/Splotify.egg-info/PKG-INFO
+-rw-r--r--   0 liachen    (501) staff       (20)     2645 2023-05-05 04:04:54.000000 Splotify-0.1.1/Splotify.egg-info/SOURCES.txt
+-rw-r--r--   0 liachen    (501) staff       (20)        1 2023-05-05 04:04:54.000000 Splotify-0.1.1/Splotify.egg-info/dependency_links.txt
+-rw-r--r--   0 liachen    (501) staff       (20)      247 2023-05-05 04:04:54.000000 Splotify-0.1.1/Splotify.egg-info/requires.txt
+-rw-r--r--   0 liachen    (501) staff       (20)        9 2023-05-05 04:04:54.000000 Splotify-0.1.1/Splotify.egg-info/top_level.txt
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.025883 Splotify-0.1.1/examples/
+-rw-r--r--   0 liachen    (501) staff       (20)   112044 2023-05-05 03:58:30.000000 Splotify-0.1.1/examples/radiohead_box_plot.png
+-rw-r--r--   0 liachen    (501) staff       (20)    91188 2023-05-05 03:58:30.000000 Splotify-0.1.1/examples/radiohead_pie_chart.png
+-rw-r--r--   0 liachen    (501) staff       (20)    74775 2023-05-05 03:58:30.000000 Splotify-0.1.1/examples/radiohead_scatter_plot.png
+-rw-r--r--   0 liachen    (501) staff       (20)     1512 2023-05-05 04:00:35.000000 Splotify-0.1.1/pyproject.toml
+-rw-r--r--   0 liachen    (501) staff       (20)      172 2023-05-05 03:58:30.000000 Splotify-0.1.1/requirements.txt
+-rw-r--r--   0 liachen    (501) staff       (20)       38 2023-05-05 04:04:55.069925 Splotify-0.1.1/setup.cfg
+-rw-r--r--   0 liachen    (501) staff       (20)       38 2023-05-05 03:58:30.000000 Splotify-0.1.1/setup.py
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.028410 Splotify-0.1.1/splotify/
+-rw-r--r--   0 liachen    (501) staff       (20)       22 2023-05-05 04:00:35.000000 Splotify-0.1.1/splotify/__init__.py
+-rw-r--r--   0 liachen    (501) staff       (20)     3919 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/data.py
+-rw-r--r--   0 liachen    (501) staff       (20)     3332 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/helpers.py
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.030207 Splotify-0.1.1/splotify/plots/
+-rw-r--r--   0 liachen    (501) staff       (20)        0 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/plots/__init__.py
+-rw-r--r--   0 liachen    (501) staff       (20)     8230 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/plots/audiofeatures.py
+-rw-r--r--   0 liachen    (501) staff       (20)     1878 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/plots/category.py
+-rw-r--r--   0 liachen    (501) staff       (20)     1972 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/plots/popularity.py
+-rw-r--r--   0 liachen    (501) staff       (20)     2155 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/spotifyapi.py
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.037414 Splotify-0.1.1/splotify/tests/
+-rw-r--r--   0 liachen    (501) staff       (20)      153 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/__init__.py
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.014263 Splotify-0.1.1/splotify/tests/cassettes/
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.047702 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_box_plot.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_histogram.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d_average.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d_average.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    54880 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_select_features.yaml
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.052406 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/
+-rw-r--r--   0 liachen    (501) staff       (20)   113096 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/test_add_albums.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)   440329 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/test_add_playlists.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)   100792 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/test_add_tracks.yaml
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.054529 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_helpers/
+-rw-r--r--   0 liachen    (501) staff       (20)    17003 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_helpers/test_my_id.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)    25309 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_helpers/test_search_id.yaml
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.055124 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_integration/
+-rw-r--r--   0 liachen    (501) staff       (20)   171216 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_integration/test_integration.yaml
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.057532 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_popularity/
+-rw-r--r--   0 liachen    (501) staff       (20)   254997 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_popularity/test_album_bar_chart.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)   100727 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_popularity/test_track_bar_chart.yaml
+-rw-r--r--   0 liachen    (501) staff       (20)     3761 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/conftest.py
+drwxr-xr-x   0 liachen    (501) staff       (20)        0 2023-05-05 04:04:55.067771 Splotify-0.1.1/splotify/tests/expected_plot_outputs/
+-rw-r--r--   0 liachen    (501) staff       (20)    41212 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_album_bar_chart.png
+-rw-r--r--   0 liachen    (501) staff       (20)    22294 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_bar_chart.png
+-rw-r--r--   0 liachen    (501) staff       (20)    37166 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_box_plot.png
+-rw-r--r--   0 liachen    (501) staff       (20)    29434 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_histogram.png
+-rw-r--r--   0 liachen    (501) staff       (20)    33495 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_pie_chart.png
+-rw-r--r--   0 liachen    (501) staff       (20)    38658 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_and_integration.png
+-rw-r--r--   0 liachen    (501) staff       (20)    34973 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_average.png
+-rw-r--r--   0 liachen    (501) staff       (20)    93897 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_3d.png
+-rw-r--r--   0 liachen    (501) staff       (20)    81566 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_3d_average.png
+-rw-r--r--   0 liachen    (501) staff       (20)   102696 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_track_bar_chart.png
+-rw-r--r--   0 liachen    (501) staff       (20)     1627 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/test_audiofeatures.py
+-rw-r--r--   0 liachen    (501) staff       (20)      505 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/test_category.py
+-rw-r--r--   0 liachen    (501) staff       (20)     2442 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/test_data.py
+-rw-r--r--   0 liachen    (501) staff       (20)     1647 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/test_helpers.py
+-rw-r--r--   0 liachen    (501) staff       (20)      669 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/test_integration.py
+-rw-r--r--   0 liachen    (501) staff       (20)      713 2023-05-05 03:58:30.000000 Splotify-0.1.1/splotify/tests/test_popularity.py
```

### Comparing `splotify-0.1.0/CONTRIBUTING.md` & `Splotify-0.1.1/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Thank you for your interest in contributing to splotify!!
+Thank you for your interest in contributing to Splotify!!
 
 ## Prerequisites
 
 1. Fork the repository.
 2. Clone the forked repository to your local machine.
 3. Install python.
 4. Install the development dependencies by running `make develop`.
```

### Comparing `splotify-0.1.0/LICENSE` & `Splotify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/PKG-INFO` & `Splotify-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: splotify
-Version: 0.1.0
+Name: Splotify
+Version: 0.1.1
 Summary: A python library for easily graphing and visualizing your Spotify data.
 Author-email: Cordelia Chen <liachen2002@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,56 +216,67 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# splotify
+# Splotify
 
 A python library for easily graphing and visualizing your Spotify data.
 
 [![Build Status](https://github.com/cordeliachen/splotify/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/cordeliachen/splotify/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/cordeliachen/splotify/branch/main/graph/badge.svg)](https://codecov.io/gh/cordeliachen/splotify)
 ![](https://img.shields.io/badge/license-Apache--2.0-blue)
 ![](https://img.shields.io/github/issues/cordeliachen/splotify)
+[![PyPI](https://img.shields.io/pypi/v/splotify)](https://pypi.org/project/splotify/)
+
+## Documentation
+
+Github Pages: [![Docs](https://img.shields.io/badge/Github-Pages-brightgreen)](https://cordeliachen.github.io/splotify/)
+Read the Docs: [![Read the Docs](https://img.shields.io/readthedocs/splotify)](https://splotify.readthedocs.io/en/latest/)
+
+## Tutorial
+
+View the Jupyter Notebook tutorial with interactive Plotly plots [here](https://colab.research.google.com/drive/14jXAa_LertvDA4oHT148vWpNIDBiYZ5O?usp=sharing).
 
 ## Installation
 
 Install the library by running:
 
 `pip install splotify`
 
 ## Usage
 
 1. First, you need to get your `SPOTIPY_CLIENT_ID`, `SPOTIPY_CLIENT_SECRET`, and redirect uri. [Here](https://www.youtube.com/watch?v=3RGm4jALukM) is a video created by Spotipy that explains how to do so.
+![](https://github.com/cordeliachen/splotify/blob/docs/examples/splotifydemo.gif)
 
 2. Declare a `SpotifyAPI` object that allows you to access data from Spotify.
 
 3. Declare a `Data` object to store all the songs which you want to plot. You can add individual or multiple tracks, albums, or playlists at a time.
 
 4. Determine the kind of data you want to plot:
 
    - Category plots (bar charts, pie charts) allow you to plot songs by groups (i.e. artists or albums).
    - Audio Feature Plots allow you to plot songs by their audio features.
 
 5. If you need to look up the Spotify ids of tracks, albums, artists, or playlists, you can use the `search_id` (for general searches) or `my_id` (for user-specific playlists) functions.
 
 Here is an example analyzing Spotify's "This is Radiohead" playlist:
 
-```
-import spotifyapi
-import data
-import plots.audiofeatures as af
-import plots.category as c
+```python
+import splotify.spotifyapi as spotifyapi
+import splotify.data as data
+import splotify.plots.audiofeatures as af
+import splotify.plots.category as c
 
 sp = spotifyapi.SpotifyApi(
-    "234645624be5451eb959f0af3d9e00ac",
-    "a1425a973e8d4574a0dfbd3c9e20438f",
-    "https://localhost:8888/callback",
+    "YOUR SPOTIPY_CLIENT_ID",
+    "YOUR SPOTIPY_CLIENT_SECRET",
+    "YOUR REDIRECT URI",
 )
 
 d = data.Data(sp)
 
 # add tracks from the "This is Radiohead" playlist
 d.add_playlist("37i9dQZF1DZ06evO2VxlyE")
```

### Comparing `splotify-0.1.0/README.md` & `Splotify-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,60 @@
-# splotify
+# Splotify
 
 A python library for easily graphing and visualizing your Spotify data.
 
 [![Build Status](https://github.com/cordeliachen/splotify/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/cordeliachen/splotify/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/cordeliachen/splotify/branch/main/graph/badge.svg)](https://codecov.io/gh/cordeliachen/splotify)
 ![](https://img.shields.io/badge/license-Apache--2.0-blue)
 ![](https://img.shields.io/github/issues/cordeliachen/splotify)
+[![PyPI](https://img.shields.io/pypi/v/splotify)](https://pypi.org/project/splotify/)
+
+## Documentation
+
+Github Pages: [![Docs](https://img.shields.io/badge/Github-Pages-brightgreen)](https://cordeliachen.github.io/splotify/)
+Read the Docs: [![Read the Docs](https://img.shields.io/readthedocs/splotify)](https://splotify.readthedocs.io/en/latest/)
+
+## Tutorial
+
+View the Jupyter Notebook tutorial with interactive Plotly plots [here](https://colab.research.google.com/drive/14jXAa_LertvDA4oHT148vWpNIDBiYZ5O?usp=sharing).
 
 ## Installation
 
 Install the library by running:
 
 `pip install splotify`
 
 ## Usage
 
 1. First, you need to get your `SPOTIPY_CLIENT_ID`, `SPOTIPY_CLIENT_SECRET`, and redirect uri. [Here](https://www.youtube.com/watch?v=3RGm4jALukM) is a video created by Spotipy that explains how to do so.
+![](https://github.com/cordeliachen/splotify/blob/docs/examples/splotifydemo.gif)
 
 2. Declare a `SpotifyAPI` object that allows you to access data from Spotify.
 
 3. Declare a `Data` object to store all the songs which you want to plot. You can add individual or multiple tracks, albums, or playlists at a time.
 
 4. Determine the kind of data you want to plot:
 
    - Category plots (bar charts, pie charts) allow you to plot songs by groups (i.e. artists or albums).
    - Audio Feature Plots allow you to plot songs by their audio features.
 
 5. If you need to look up the Spotify ids of tracks, albums, artists, or playlists, you can use the `search_id` (for general searches) or `my_id` (for user-specific playlists) functions.
 
 Here is an example analyzing Spotify's "This is Radiohead" playlist:
 
-```
-import spotifyapi
-import data
-import plots.audiofeatures as af
-import plots.category as c
+```python
+import splotify.spotifyapi as spotifyapi
+import splotify.data as data
+import splotify.plots.audiofeatures as af
+import splotify.plots.category as c
 
 sp = spotifyapi.SpotifyApi(
-    "234645624be5451eb959f0af3d9e00ac",
-    "a1425a973e8d4574a0dfbd3c9e20438f",
-    "https://localhost:8888/callback",
+    "YOUR SPOTIPY_CLIENT_ID",
+    "YOUR SPOTIPY_CLIENT_SECRET",
+    "YOUR REDIRECT URI",
 )
 
 d = data.Data(sp)
 
 # add tracks from the "This is Radiohead" playlist
 d.add_playlist("37i9dQZF1DZ06evO2VxlyE")
```

### Comparing `splotify-0.1.0/examples/radiohead_box_plot.png` & `Splotify-0.1.1/examples/radiohead_box_plot.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/examples/radiohead_pie_chart.png` & `Splotify-0.1.1/examples/radiohead_pie_chart.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/examples/radiohead_scatter_plot.png` & `Splotify-0.1.1/examples/radiohead_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/pyproject.toml` & `Splotify-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     "setuptools",
     "setuptools-scm",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
-name = "splotify"
+name = "Splotify"
 authors = [{name = "Cordelia Chen", email = "liachen2002@gmail.com"}]
 description="A python library for easily graphing and visualizing your Spotify data."
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = [
     'pandas>=1.2.4',
     'plotly>=5.13.1',
-    'spotipy>=2.22.1',
+    'spotipy>=2.23.0',
     'tabulate>=0.9.0',
     'tqdm>=4.64.0',
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -57,8 +57,11 @@
 ]
 
 [tool.flake8]
 ignore = ['E203']
 max-line-length=88
 exclude=[
     'splotify/tests/conftest.py'
-]
+]
+
+[tool.check-manifest]
+ignore = [".vscode/settings.json"]
```

### Comparing `splotify-0.1.0/splotify/helpers.py` & `Splotify-0.1.1/splotify/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,37 @@
-from tabulate import tabulate
+"""URI search functions.
+
+This module contains functions to help get the Spotify URIs of tracks, albums,
+artists, and playlists.
 
-# for getting the uris of public spotify data
-# i.e. tracks, albums, artists, and public playlists
+"""
+
+from tabulate import tabulate
 
 
 def search_id(sp, query, limit=10, type="track"):
+    """Returns and prints the URIs of public Spotify data.
+
+    Returns and prints the URIs of Spotify data that is not user-specific such
+    as tracks, albums, artists, and public playlists.
+
+    Args:
+        sp (splotify.spotifyapi.SpotifyApi): A `SpotifyApi` instance.
+        query (str): The query you want to search for.
+        limit (:obj:`int`, optional): The number of results you want to view.
+            Defaults to 10.
+        type (:obj:`str`, optional): The type of URI you want to search up.
+            Currently only supports 'track', 'album', 'artist', and 'playlist'.
+            Defaults to 'track'.
+
+    Returns:
+        A nested list. The first list is the names of the columns, and the
+        remaining lists are the search results.
+
+    """
     results = sp.search(query, limit, type)
     if type == "track":
         table = [["Name", "Album", "Artists", "URI"]]
         for i in range(limit):
             song = results["tracks"]["items"][i]
             table.append(
                 [
@@ -37,21 +60,34 @@
         table = [["Name", "Owner", "URI"]]
         for i in range(limit):
             playlist = results["playlists"]["items"][i]
             table.append(
                 [playlist["name"], playlist["owner"]["display_name"], playlist["uri"]]
             )
         print(tabulate(table, headers="firstrow"))
+    # else:
+
     return table
 
 
-# for getting the uris of personal spotify data i.e. playlists you own
+def my_id(sp, limit=10, type="playlist"):
+    """Returns and prints the URIs of your personal Spotify playlists.
 
+    Args:
+        sp (splotify.spotifyapi.SpotifyApi): A `SpotifyApi` instance.
+        limit (:obj:`int`, optional): The number of results you want to view.
+            Defaults to 10.
+        type (str, optional): The type of URI you want to search up. Defaults
+            to 'playlist'. Currently only supports 'playlist'.
+
+    Returns:
+        A nested list. The first list is the names of the columns, and the
+        remaining lists are the search results.
 
-def my_id(sp, limit=10, type="playlist"):
+    """
     if type == "playlist":
         results = sp.current_user_playlists()
         table = [["Name", "URI"]]
         for i in range(limit):
             playlist = results["items"][i]
             table.append([playlist["name"], playlist["uri"]])
         print(tabulate(table, headers="firstrow"))
```

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_box_plot.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_box_plot.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_histogram.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_histogram.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d_average.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d_average.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d_average.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d_average.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_select_features.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_select_features.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/test_add_albums.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/test_add_albums.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/test_add_playlists.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/test_add_playlists.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_data/test_add_tracks.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_data/test_add_tracks.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_helpers/test_my_id.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_helpers/test_my_id.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_helpers/test_search_id.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_helpers/test_search_id.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/cassettes/splotify.tests.test_integration/test_integration.yaml` & `Splotify-0.1.1/splotify/tests/cassettes/splotify.tests.test_integration/test_integration.yaml`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/conftest.py` & `Splotify-0.1.1/splotify/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_bar_chart.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_bar_chart.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_box_plot.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_box_plot.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_histogram.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_histogram.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_pie_chart.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_pie_chart.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_and_integration.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_and_integration.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_average.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_2d_average.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_3d.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_3d.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/expected_plot_outputs/test_scatter_plot_3d_average.png` & `Splotify-0.1.1/splotify/tests/expected_plot_outputs/test_scatter_plot_3d_average.png`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/test_audiofeatures.py` & `Splotify-0.1.1/splotify/tests/test_audiofeatures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from splotify.plots import audiofeatures
 from splotify.tests import sp
+from splotify.data import Data
+import unittest.mock as mock
 import pytest
 import os
 
 
 @pytest.fixture(scope="module")
 def vcr_cassette_dir(request):
     return os.path.join("splotify/tests/cassettes", request.module.__name__)
 
 
 @pytest.fixture
 def afp(track_data):
-    return audiofeatures.AudioFeaturesPlot(
-        sp, track_data, ["loudness", "danceability", "energy"]
-    )
+    with mock.patch("splotify.data.Data.get_data") as get_data:
+        get_data.return_value = track_data
+        yield audiofeatures.AudioFeaturesPlot(
+            sp, Data(sp), ["loudness", "danceability", "energy"]
+        )
 
 
 @pytest.mark.vcr()
 def test_select_features(afp):
     assert afp.get_features() == ["loudness", "danceability", "energy"]
 
     afp.select_features(["speechiness", "tempo", "key"])
```

### Comparing `splotify-0.1.0/splotify/tests/test_data.py` & `Splotify-0.1.1/splotify/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/test_helpers.py` & `Splotify-0.1.1/splotify/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `splotify-0.1.0/splotify/tests/test_integration.py` & `Splotify-0.1.1/splotify/tests/test_integration.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,14 +16,12 @@
     d = data.Data(sp)
 
     id1 = "spotify:album:7iLuHJkrb9KHPkMgddYigh"
     id2 = helpers.search_id(sp, "OK Computer", limit=1, type="album")[1][2]
 
     d.add_albums([id1, id2])
 
-    afp = audiofeatures.AudioFeaturesPlot(
-        sp, d.get_data(), ["loudness", "danceability"]
-    )
+    afp = audiofeatures.AudioFeaturesPlot(sp, d, ["loudness", "danceability"])
 
     fig = afp.scatter_plot_2d(color="album")
 
     assert fig is not None
```

### Comparing `splotify-0.1.0/splotify.egg-info/PKG-INFO` & `Splotify-0.1.1/Splotify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: splotify
-Version: 0.1.0
+Name: Splotify
+Version: 0.1.1
 Summary: A python library for easily graphing and visualizing your Spotify data.
 Author-email: Cordelia Chen <liachen2002@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,56 +216,67 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
-# splotify
+# Splotify
 
 A python library for easily graphing and visualizing your Spotify data.
 
 [![Build Status](https://github.com/cordeliachen/splotify/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/cordeliachen/splotify/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/cordeliachen/splotify/branch/main/graph/badge.svg)](https://codecov.io/gh/cordeliachen/splotify)
 ![](https://img.shields.io/badge/license-Apache--2.0-blue)
 ![](https://img.shields.io/github/issues/cordeliachen/splotify)
+[![PyPI](https://img.shields.io/pypi/v/splotify)](https://pypi.org/project/splotify/)
+
+## Documentation
+
+Github Pages: [![Docs](https://img.shields.io/badge/Github-Pages-brightgreen)](https://cordeliachen.github.io/splotify/)
+Read the Docs: [![Read the Docs](https://img.shields.io/readthedocs/splotify)](https://splotify.readthedocs.io/en/latest/)
+
+## Tutorial
+
+View the Jupyter Notebook tutorial with interactive Plotly plots [here](https://colab.research.google.com/drive/14jXAa_LertvDA4oHT148vWpNIDBiYZ5O?usp=sharing).
 
 ## Installation
 
 Install the library by running:
 
 `pip install splotify`
 
 ## Usage
 
 1. First, you need to get your `SPOTIPY_CLIENT_ID`, `SPOTIPY_CLIENT_SECRET`, and redirect uri. [Here](https://www.youtube.com/watch?v=3RGm4jALukM) is a video created by Spotipy that explains how to do so.
+![](https://github.com/cordeliachen/splotify/blob/docs/examples/splotifydemo.gif)
 
 2. Declare a `SpotifyAPI` object that allows you to access data from Spotify.
 
 3. Declare a `Data` object to store all the songs which you want to plot. You can add individual or multiple tracks, albums, or playlists at a time.
 
 4. Determine the kind of data you want to plot:
 
    - Category plots (bar charts, pie charts) allow you to plot songs by groups (i.e. artists or albums).
    - Audio Feature Plots allow you to plot songs by their audio features.
 
 5. If you need to look up the Spotify ids of tracks, albums, artists, or playlists, you can use the `search_id` (for general searches) or `my_id` (for user-specific playlists) functions.
 
 Here is an example analyzing Spotify's "This is Radiohead" playlist:
 
-```
-import spotifyapi
-import data
-import plots.audiofeatures as af
-import plots.category as c
+```python
+import splotify.spotifyapi as spotifyapi
+import splotify.data as data
+import splotify.plots.audiofeatures as af
+import splotify.plots.category as c
 
 sp = spotifyapi.SpotifyApi(
-    "234645624be5451eb959f0af3d9e00ac",
-    "a1425a973e8d4574a0dfbd3c9e20438f",
-    "https://localhost:8888/callback",
+    "YOUR SPOTIPY_CLIENT_ID",
+    "YOUR SPOTIPY_CLIENT_SECRET",
+    "YOUR REDIRECT URI",
 )
 
 d = data.Data(sp)
 
 # add tracks from the "This is Radiohead" playlist
 d.add_playlist("37i9dQZF1DZ06evO2VxlyE")
```

### Comparing `splotify-0.1.0/splotify.egg-info/SOURCES.txt` & `Splotify-0.1.1/Splotify.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 .bumpversion.cfg
-.gitignore
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.py
-.github/dependabot.yml
-.github/ISSUE_TEMPLATE/bug_report.md
-.github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/build.yml
-.vscode/settings.json
+Splotify.egg-info/PKG-INFO
+Splotify.egg-info/SOURCES.txt
+Splotify.egg-info/dependency_links.txt
+Splotify.egg-info/requires.txt
+Splotify.egg-info/top_level.txt
 examples/radiohead_box_plot.png
 examples/radiohead_pie_chart.png
 examples/radiohead_scatter_plot.png
 splotify/__init__.py
 splotify/data.py
 splotify/helpers.py
-splotify/main.py
 splotify/spotifyapi.py
-splotify.egg-info/PKG-INFO
-splotify.egg-info/SOURCES.txt
-splotify.egg-info/dependency_links.txt
-splotify.egg-info/requires.txt
-splotify.egg-info/top_level.txt
-splotify/plots/___init__.py
-splotify/plots/audioanalysis.py
+splotify/plots/__init__.py
 splotify/plots/audiofeatures.py
 splotify/plots/category.py
-splotify/plots/timeline.py
+splotify/plots/popularity.py
 splotify/tests/__init__.py
 splotify/tests/conftest.py
 splotify/tests/test_audiofeatures.py
 splotify/tests/test_category.py
 splotify/tests/test_data.py
 splotify/tests/test_helpers.py
 splotify/tests/test_integration.py
+splotify/tests/test_popularity.py
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_box_plot.yaml
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_histogram.yaml
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d.yaml
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_2d_average.yaml
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d.yaml
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_scatter_plot_3d_average.yaml
 splotify/tests/cassettes/splotify.tests.test_audiofeatures/test_select_features.yaml
 splotify/tests/cassettes/splotify.tests.test_data/test_add_albums.yaml
 splotify/tests/cassettes/splotify.tests.test_data/test_add_playlists.yaml
 splotify/tests/cassettes/splotify.tests.test_data/test_add_tracks.yaml
 splotify/tests/cassettes/splotify.tests.test_helpers/test_my_id.yaml
 splotify/tests/cassettes/splotify.tests.test_helpers/test_search_id.yaml
 splotify/tests/cassettes/splotify.tests.test_integration/test_integration.yaml
+splotify/tests/cassettes/splotify.tests.test_popularity/test_album_bar_chart.yaml
+splotify/tests/cassettes/splotify.tests.test_popularity/test_track_bar_chart.yaml
+splotify/tests/expected_plot_outputs/test_album_bar_chart.png
 splotify/tests/expected_plot_outputs/test_bar_chart.png
 splotify/tests/expected_plot_outputs/test_box_plot.png
 splotify/tests/expected_plot_outputs/test_histogram.png
 splotify/tests/expected_plot_outputs/test_pie_chart.png
 splotify/tests/expected_plot_outputs/test_scatter_plot_2d_and_integration.png
 splotify/tests/expected_plot_outputs/test_scatter_plot_2d_average.png
 splotify/tests/expected_plot_outputs/test_scatter_plot_3d.png
-splotify/tests/expected_plot_outputs/test_scatter_plot_3d_average.png
+splotify/tests/expected_plot_outputs/test_scatter_plot_3d_average.png
+splotify/tests/expected_plot_outputs/test_track_bar_chart.png
```

