# Comparing `tmp/seealgo-0.1.1.tar.gz` & `tmp/seealgo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seealgo-0.1.1.tar", last modified: Thu Mar 23 23:38:52 2023, max compression
+gzip compressed data, was "seealgo-0.2.0.tar", last modified: Fri May  5 16:16:07 2023, max compression
```

## Comparing `seealgo-0.1.1.tar` & `seealgo-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,177 @@
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.690510 seealgo-0.1.1/
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.664704 seealgo-0.1.1/.github/
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.667166 seealgo-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 sarahtang   (501) staff       (20)      834 2023-03-23 03:50:25.000000 seealgo-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 sarahtang   (501) staff       (20)      595 2023-03-23 03:50:25.000000 seealgo-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 sarahtang   (501) staff       (20)      125 2023-03-23 03:50:25.000000 seealgo-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.669035 seealgo-0.1.1/.github/workflows/
--rw-r--r--   0 sarahtang   (501) staff       (20)     1189 2023-03-23 03:50:25.000000 seealgo-0.1.1/.github/workflows/main.yml
--rw-r--r--   0 sarahtang   (501) staff       (20)     1799 2023-03-23 03:50:25.000000 seealgo-0.1.1/.gitignore
--rw-r--r--   0 sarahtang   (501) staff       (20)     1011 2023-03-23 04:40:49.000000 seealgo-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 sarahtang   (501) staff       (20)    11357 2023-03-23 03:50:25.000000 seealgo-0.1.1/LICENSE
--rw-r--r--   0 sarahtang   (501) staff       (20)      133 2023-03-23 06:27:31.000000 seealgo-0.1.1/MANIFEST.in
--rw-r--r--   0 sarahtang   (501) staff       (20)     2223 2023-03-23 04:40:49.000000 seealgo-0.1.1/Makefile
--rw-r--r--   0 sarahtang   (501) staff       (20)     1735 2023-03-23 23:38:52.689730 seealgo-0.1.1/PKG-INFO
--rw-r--r--   0 sarahtang   (501) staff       (20)     1455 2023-03-23 05:53:43.000000 seealgo-0.1.1/README.md
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.681908 seealgo-0.1.1/outputFiles/
--rw-r--r--   0 sarahtang   (501) staff       (20)      193 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/appendListOutput1.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      243 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/appendListOutput2.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      193 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/deleteListOutput1.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      150 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/deleteListOutput2.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)    37390 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/eg_appendlist_after.png
--rw-r--r--   0 sarahtang   (501) staff       (20)    29368 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/eg_appendlist_before.png
--rw-r--r--   0 sarahtang   (501) staff       (20)      325 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/initListOutput.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      246 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/insertListOutput1.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      298 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/insertListOutput2.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      326 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/mixListOutput1.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      283 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/mixListOutput2.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      335 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/mixListOutput3.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      378 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/mixListOutput4.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      380 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/mixListOutput5.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      199 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/setListOutput1.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      206 2023-03-23 03:50:25.000000 seealgo-0.1.1/outputFiles/setListOutput2.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)      485 2023-03-23 06:11:47.000000 seealgo-0.1.1/pyproject.toml
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.683297 seealgo-0.1.1/seealgo/
--rw-r--r--   0 sarahtang   (501) staff       (20)      110 2023-03-23 05:53:43.000000 seealgo-0.1.1/seealgo/__init__.py
--rw-r--r--   0 sarahtang   (501) staff       (20)     2194 2023-03-23 03:50:25.000000 seealgo-0.1.1/seealgo/see_list_algo.py
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.688891 seealgo-0.1.1/seealgo/tests/
--rw-r--r--   0 sarahtang   (501) staff       (20)       49 2023-03-23 05:53:43.000000 seealgo-0.1.1/seealgo/tests/__init__.py
--rw-r--r--   0 sarahtang   (501) staff       (20)     5467 2023-03-23 05:53:43.000000 seealgo-0.1.1/seealgo/tests/test_list.py
-drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-03-23 23:38:52.687205 seealgo-0.1.1/seealgo.egg-info/
--rw-r--r--   0 sarahtang   (501) staff       (20)     1735 2023-03-23 23:38:52.000000 seealgo-0.1.1/seealgo.egg-info/PKG-INFO
--rw-r--r--   0 sarahtang   (501) staff       (20)      995 2023-03-23 23:38:52.000000 seealgo-0.1.1/seealgo.egg-info/SOURCES.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)        1 2023-03-23 23:38:52.000000 seealgo-0.1.1/seealgo.egg-info/dependency_links.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)        9 2023-03-23 23:38:52.000000 seealgo-0.1.1/seealgo.egg-info/requires.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)        8 2023-03-23 23:38:52.000000 seealgo-0.1.1/seealgo.egg-info/top_level.txt
--rw-r--r--   0 sarahtang   (501) staff       (20)       38 2023-03-23 23:38:52.690885 seealgo-0.1.1/setup.cfg
--rw-r--r--   0 sarahtang   (501) staff       (20)      411 2023-03-23 06:11:47.000000 seealgo-0.1.1/setup.py
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.974427 seealgo-0.2.0/
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.743469 seealgo-0.2.0/.github/
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.747288 seealgo-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 sarahtang   (501) staff       (20)      834 2023-03-23 03:50:25.000000 seealgo-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 sarahtang   (501) staff       (20)      595 2023-03-23 03:50:25.000000 seealgo-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 sarahtang   (501) staff       (20)      125 2023-03-23 03:50:25.000000 seealgo-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.748422 seealgo-0.2.0/.github/workflows/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     1195 2023-04-08 06:07:05.000000 seealgo-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0 sarahtang   (501) staff       (20)     1799 2023-03-23 03:50:25.000000 seealgo-0.2.0/.gitignore
+-rw-r--r--   0 sarahtang   (501) staff       (20)     1011 2023-03-23 04:40:49.000000 seealgo-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 sarahtang   (501) staff       (20)    11357 2023-03-23 03:50:25.000000 seealgo-0.2.0/LICENSE
+-rw-r--r--   0 sarahtang   (501) staff       (20)      133 2023-03-23 06:27:31.000000 seealgo-0.2.0/MANIFEST.in
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2531 2023-04-08 06:45:50.000000 seealgo-0.2.0/Makefile
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3104 2023-05-05 16:16:07.973794 seealgo-0.2.0/PKG-INFO
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2824 2023-05-05 14:50:40.000000 seealgo-0.2.0/README.md
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.755336 seealgo-0.2.0/docs/
+-rw-r--r--   0 sarahtang   (501) staff       (20)      633 2023-05-05 15:39:18.000000 seealgo-0.2.0/docs/Makefile
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.650697 seealgo-0.2.0/docs/build/
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.764788 seealgo-0.2.0/docs/build/doctrees/
+-rw-r--r--   0 sarahtang   (501) staff       (20)    30139 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 sarahtang   (501) staff       (20)     6895 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/index.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)    23050 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/list.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2651 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/modules.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)    73659 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/seealgo.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4102 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/seealgo.tests.doctree
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.768146 seealgo-0.2.0/docs/build/doctrees/source/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2689 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/source/modules.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)    73673 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/source/seealgo.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4102 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/source/seealgo.tests.doctree
+-rw-r--r--   0 sarahtang   (501) staff       (20)    45109 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/doctrees/tree.doctree
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.789817 seealgo-0.2.0/docs/build/html/
+-rw-r--r--   0 sarahtang   (501) staff       (20)      230 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/.buildinfo
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.792438 seealgo-0.2.0/docs/build/html/.doctrees/
+-rw-r--r--   0 sarahtang   (501) staff       (20)    11120 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/.doctrees/environment.pickle
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4925 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/.doctrees/index.doctree
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.794291 seealgo-0.2.0/docs/build/html/_images/
+-rw-r--r--   0 sarahtang   (501) staff       (20)    37390 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_images/eg_appendlist_after.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)    29368 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_images/eg_appendlist_before.png
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.805558 seealgo-0.2.0/docs/build/html/_sources/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     1562 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)       77 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/list.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)       58 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      552 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/seealgo.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      505 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/seealgo.tests.rst.txt
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.813885 seealgo-0.2.0/docs/build/html/_sources/source/
+-rw-r--r--   0 sarahtang   (501) staff       (20)       58 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/source/modules.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      552 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/source/seealgo.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      505 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/source/seealgo.tests.rst.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)       78 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_sources/tree.rst.txt
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.845353 seealgo-0.2.0/docs/build/html/_static/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4418 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)    11185 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/alabaster.css
+-rw-r--r--   0 sarahtang   (501) staff       (20)    15228 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/basic.css
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.848419 seealgo-0.2.0/docs/build/html/_static/css/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3229 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/badge_only.css
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.904084 seealgo-0.2.0/docs/build/html/_static/css/fonts/
+-rw-r--r--   0 sarahtang   (501) staff       (20)    87624 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)    67312 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)    86288 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)    66444 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)   165742 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 sarahtang   (501) staff       (20)   444379 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 sarahtang   (501) staff       (20)   165548 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 sarahtang   (501) staff       (20)    98024 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)    77160 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)   323344 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)   193308 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)   309728 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)   184912 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)   328412 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)   195704 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)   309192 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 sarahtang   (501) staff       (20)   182708 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 sarahtang   (501) staff       (20)   135235 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0 sarahtang   (501) staff       (20)       42 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/custom.css
+-rw-r--r--   0 sarahtang   (501) staff       (20)     8171 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)      421 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)      286 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/file.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)   288580 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)    89501 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/jquery.js
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.913997 seealgo-0.2.0/docs/build/html/_static/js/
+-rw-r--r--   0 sarahtang   (501) staff       (20)      934 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4370 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2734 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)     5023 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4758 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)       90 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/minus.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)       90 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/plus.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4819 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0 sarahtang   (501) staff       (20)    17088 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)    68420 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)    19530 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/_static/underscore.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)    12534 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/genindex.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     7237 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/index.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)    10895 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/list.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3762 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/modules.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)      610 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/objects.inv
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4694 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/py-modindex.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3866 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/search.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     5665 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/searchindex.js
+-rw-r--r--   0 sarahtang   (501) staff       (20)    27082 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/seealgo.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4820 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/seealgo.tests.html
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.916743 seealgo-0.2.0/docs/build/html/source/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     5214 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/source/modules.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)    26836 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/source/seealgo.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4617 2023-04-08 19:33:07.000000 seealgo-0.2.0/docs/build/html/source/seealgo.tests.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)    17488 2023-05-05 00:40:27.000000 seealgo-0.2.0/docs/build/html/tree.html
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2058 2023-05-05 15:55:55.000000 seealgo-0.2.0/docs/conf.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     1562 2023-05-05 15:39:18.000000 seealgo-0.2.0/docs/index.rst
+-rw-r--r--   0 sarahtang   (501) staff       (20)       77 2023-04-08 18:30:20.000000 seealgo-0.2.0/docs/list.rst
+-rw-r--r--   0 sarahtang   (501) staff       (20)      804 2023-04-08 06:07:05.000000 seealgo-0.2.0/docs/make.bat
+-rw-r--r--   0 sarahtang   (501) staff       (20)       58 2023-04-08 18:30:20.000000 seealgo-0.2.0/docs/modules.rst
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.924701 seealgo-0.2.0/docs/source/
+-rw-r--r--   0 sarahtang   (501) staff       (20)       58 2023-04-08 06:07:05.000000 seealgo-0.2.0/docs/source/modules.rst
+-rw-r--r--   0 sarahtang   (501) staff       (20)      552 2023-04-08 18:30:20.000000 seealgo-0.2.0/docs/source/seealgo.rst
+-rw-r--r--   0 sarahtang   (501) staff       (20)      505 2023-04-08 06:07:05.000000 seealgo-0.2.0/docs/source/seealgo.tests.rst
+-rw-r--r--   0 sarahtang   (501) staff       (20)       78 2023-04-08 18:30:20.000000 seealgo-0.2.0/docs/tree.rst
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.959371 seealgo-0.2.0/outputFiles/
+-rw-r--r--   0 sarahtang   (501) staff       (20)      182 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/addSetOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      225 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/addSetOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      297 2023-04-08 00:49:26.000000 seealgo-0.2.0/outputFiles/addTreeOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      360 2023-04-08 00:49:26.000000 seealgo-0.2.0/outputFiles/addTreeOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      221 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/appendListOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      278 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/appendListOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      180 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/clearSetOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      134 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/clearSetOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      221 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/deleteListOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      171 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/deleteListOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      298 2023-04-08 00:49:26.000000 seealgo-0.2.0/outputFiles/deleteTreeOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      234 2023-04-08 00:49:26.000000 seealgo-0.2.0/outputFiles/deleteTreeOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)    13854 2023-05-05 01:11:42.000000 seealgo-0.2.0/outputFiles/eg_appendlist_after.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)     9872 2023-05-05 01:11:42.000000 seealgo-0.2.0/outputFiles/eg_appendlist_before.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)    16565 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/eg_appendtree_after.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)    13049 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/eg_appendtree_before.png
+-rw-r--r--   0 sarahtang   (501) staff       (20)      224 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/initDictOutput.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      374 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/initListOutput.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      232 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/initSetOutput.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      548 2023-04-08 00:49:26.000000 seealgo-0.2.0/outputFiles/initTreeOutput.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      281 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/insertListOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      340 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/insertListOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      375 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/mixListOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      325 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/mixListOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      384 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/mixListOutput3.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      434 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/mixListOutput4.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      436 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/mixListOutput5.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      385 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/nestedDictOutput.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      271 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/popDictOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      235 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/popDictOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      204 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/removeSetOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      190 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/removeSetOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      227 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/setListOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      234 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/setListOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      220 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/updateDictOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      355 2023-05-05 14:50:40.000000 seealgo-0.2.0/outputFiles/updateDictOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      218 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/updateSetOutput1.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      260 2023-04-15 04:07:32.000000 seealgo-0.2.0/outputFiles/updateSetOutput2.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)      485 2023-05-05 15:56:17.000000 seealgo-0.2.0/pyproject.toml
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.964714 seealgo-0.2.0/seealgo/
+-rw-r--r--   0 sarahtang   (501) staff       (20)      293 2023-05-05 14:50:40.000000 seealgo-0.2.0/seealgo/__init__.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4203 2023-05-05 14:50:40.000000 seealgo-0.2.0/seealgo/see_dict_algo.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     4342 2023-05-05 14:50:40.000000 seealgo-0.2.0/seealgo/see_list_algo.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3200 2023-04-15 04:07:32.000000 seealgo-0.2.0/seealgo/see_set_algo.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     8522 2023-04-08 06:07:05.000000 seealgo-0.2.0/seealgo/see_tree_algo.py
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.972831 seealgo-0.2.0/seealgo/tests/
+-rw-r--r--   0 sarahtang   (501) staff       (20)       49 2023-03-23 05:53:43.000000 seealgo-0.2.0/seealgo/tests/__init__.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2948 2023-05-05 14:50:40.000000 seealgo-0.2.0/seealgo/tests/test_dict.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     5467 2023-03-23 05:53:43.000000 seealgo-0.2.0/seealgo/tests/test_list.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3712 2023-04-15 04:07:32.000000 seealgo-0.2.0/seealgo/tests/test_set.py
+-rw-r--r--   0 sarahtang   (501) staff       (20)     2767 2023-04-08 03:03:20.000000 seealgo-0.2.0/seealgo/tests/test_tree.py
+drwxr-xr-x   0 sarahtang   (501) staff       (20)        0 2023-05-05 16:16:07.967820 seealgo-0.2.0/seealgo.egg-info/
+-rw-r--r--   0 sarahtang   (501) staff       (20)     3104 2023-05-05 16:16:07.000000 seealgo-0.2.0/seealgo.egg-info/PKG-INFO
+-rw-r--r--   0 sarahtang   (501) staff       (20)     5312 2023-05-05 16:16:07.000000 seealgo-0.2.0/seealgo.egg-info/SOURCES.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)        1 2023-05-05 16:16:07.000000 seealgo-0.2.0/seealgo.egg-info/dependency_links.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)        9 2023-05-05 16:16:07.000000 seealgo-0.2.0/seealgo.egg-info/requires.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)        8 2023-05-05 16:16:07.000000 seealgo-0.2.0/seealgo.egg-info/top_level.txt
+-rw-r--r--   0 sarahtang   (501) staff       (20)       38 2023-05-05 16:16:07.974704 seealgo-0.2.0/setup.cfg
+-rw-r--r--   0 sarahtang   (501) staff       (20)      411 2023-05-05 15:56:25.000000 seealgo-0.2.0/setup.py
```

### Comparing `seealgo-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `seealgo-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `seealgo-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/.github/workflows/main.yml` & `seealgo-0.2.0/.github/workflows/main.yml`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
         
     - name: Format code with Black
       run: black .
       
     - name: Analysing the code with pylint
       run: |
-        pylint $(git ls-files '*.py')
+        pylint $(find seealgo -name '*.py')
       
     - name: Test
       run: |
         pytest --cov=./ --cov-report=xml
         
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
```

### Comparing `seealgo-0.1.1/.gitignore` & `seealgo-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/CONTRIBUTING.md` & `seealgo-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/LICENSE` & `seealgo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/Makefile` & `seealgo-0.2.0/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 install:  ## install library
 	python -m pip install .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with black
-	python -m black --check seealgo setup.py
-	python -m flake8 seealgo setup.py
+	python -m black --check seealgo
+	python -m flake8 seealgo
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
 	python -m black seealgo/ setup.py
 
@@ -59,14 +59,30 @@
 
 minor:
 	bump2version minor
 
 major:
 	bump2version major
 
+## DOCS
+docs:
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages:
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/sarahtang7/seealgo.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	touch .nojekyll;\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
 ########
 # DIST #
 ########
 dist-build:  # Build python dist
 	python setup.py sdist bdist_wheel
 
 dist-check:
```

### Comparing `seealgo-0.1.1/outputFiles/eg_appendlist_after.png` & `seealgo-0.2.0/docs/build/html/_images/eg_appendlist_after.png`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/outputFiles/eg_appendlist_before.png` & `seealgo-0.2.0/docs/build/html/_images/eg_appendlist_before.png`

 * *Files identical despite different names*

### Comparing `seealgo-0.1.1/seealgo/tests/test_list.py` & `seealgo-0.2.0/seealgo/tests/test_list.py`

 * *Files identical despite different names*

