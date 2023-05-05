# Comparing `tmp/nvm-0.0.4.tar.gz` & `tmp/nvm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-0.0.4.tar", last modified: Thu May  4 02:36:01 2023, max compression
+gzip compressed data, was "nvm-0.1.0.tar", last modified: Fri May  5 21:34:42 2023, max compression
```

## Comparing `nvm-0.0.4.tar` & `nvm-0.1.0.tar`

### file list

```diff
@@ -1,85 +1,94 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.0.4/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.0.4/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/.github/
--rw-------   0 jiko      (1000) jiko      (1000)      314 2023-05-03 18:32:02.000000 nvm-0.0.4/.github/ISSUE_TEMPLATE.md
--rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-0.0.4/.gitignore
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.0.4/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.0.4/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.0.4/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.0.4/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.0.4/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-0.0.4/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-04 02:36:01.126451 nvm-0.0.4/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)      748 2023-05-03 18:44:59.000000 nvm-0.0.4/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/bin/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.4/bin/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.0.4/bin/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.4/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.0.4/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.0.4/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.118451 nvm-0.0.4/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.118451 nvm-0.0.4/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-03 15:23:48.000000 nvm-0.0.4/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-03 15:23:48.000000 nvm-0.0.4/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-03 15:23:49.000000 nvm-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-03 15:23:35.000000 nvm-0.0.4/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.4/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-03 15:23:35.000000 nvm-0.0.4/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      526 2023-05-03 19:24:06.000000 nvm-0.0.4/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.122451 nvm-0.0.4/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-0.0.4/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-04 01:17:49.000000 nvm-0.0.4/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-0.0.4/docs/source/nvm.aux_log.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-0.0.4/docs/source/nvm.aux_str.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-0.0.4/docs/source/nvm.aux_sys.rst
--rw-------   0 jiko      (1000) jiko      (1000)      366 2023-05-04 01:17:49.000000 nvm-0.0.4/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.0.4/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      455 2023-05-04 02:13:00.000000 nvm-0.0.4/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/_version.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_log/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-0.0.4/nvm/aux_log/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-0.0.4/nvm/aux_log/aux_log.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_pandas/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-0.0.4/nvm/aux_pandas/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1588 2023-05-04 02:26:33.000000 nvm-0.0.4/nvm/aux_pandas/aux_pandas.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_str/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      146 2023-05-03 21:40:50.000000 nvm-0.0.4/nvm/aux_str/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5218 2023-05-03 23:59:43.000000 nvm-0.0.4/nvm/aux_str/aux_str.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm/aux_sys/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-0.0.4/nvm/aux_sys/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1341 2023-05-04 00:31:05.000000 nvm-0.0.4/nvm/aux_sys/aux_sys.py
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.0.4/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     1715 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1411 2023-05-04 02:36:01.000000 nvm-0.0.4/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-04 02:36:00.000000 nvm-0.0.4/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.0.4/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      414 2023-05-03 18:32:02.000000 nvm-0.0.4/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-04 02:36:01.126451 nvm-0.0.4/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.0.4/setup.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-04 02:36:01.126451 nvm-0.0.4/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.0.4/tests/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-03 18:32:02.000000 nvm-0.0.4/tests/test_nvm.py
--rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.0.4/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.0.4/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-0.1.0/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-0.1.0/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-0.1.0/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-0.1.0/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-0.1.0/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-0.1.0/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-0.1.0/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       89 2023-05-03 18:32:02.000000 nvm-0.1.0/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-0.1.0/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-0.1.0/MANIFEST.in
+-rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-0.1.0/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2048 2023-05-05 21:34:42.970808 nvm-0.1.0/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1081 2023-05-05 21:31:52.000000 nvm-0.1.0/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/bin/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.1.0/bin/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-0.1.0/bin/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.1.0/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-0.1.0/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-0.1.0/data/emacs-logo/emacs.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.962808 nvm-0.1.0/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.962808 nvm-0.1.0/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-0.1.0/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-0.1.0/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.962808 nvm-0.1.0/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-0.1.0/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-0.1.0/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-0.1.0/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-0.1.0/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.966808 nvm-0.1.0/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-0.1.0/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-05 19:03:25.000000 nvm-0.1.0/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-0.1.0/docs/source/nvm.aux_log.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-05 13:07:38.000000 nvm-0.1.0/docs/source/nvm.aux_pandas.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-0.1.0/docs/source/nvm.aux_str.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-0.1.0/docs/source/nvm.aux_sys.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      384 2023-05-05 19:03:25.000000 nvm-0.1.0/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-0.1.0/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 19:45:20.000000 nvm-0.1.0/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/_version.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_log/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-0.1.0/nvm/aux_log/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-0.1.0/nvm/aux_log/aux_log.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_pandas/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-0.1.0/nvm/aux_pandas/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1590 2023-05-05 18:55:20.000000 nvm-0.1.0/nvm/aux_pandas/aux_pandas.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_str/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      179 2023-05-05 15:19:07.000000 nvm-0.1.0/nvm/aux_str/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     3135 2023-05-05 21:16:37.000000 nvm-0.1.0/nvm/aux_str/aux_str.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1790 2023-05-05 15:15:18.000000 nvm-0.1.0/nvm/aux_str/clean_str_mappings.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm/aux_sys/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-0.1.0/nvm/aux_sys/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1342 2023-05-05 19:03:51.000000 nvm-0.1.0/nvm/aux_sys/aux_sys.py
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-0.1.0/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2048 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1635 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-05 21:34:42.000000 nvm-0.1.0/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-0.1.0/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-0.1.0/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-05 21:34:42.970808 nvm-0.1.0/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2578 2023-05-03 18:32:02.000000 nvm-0.1.0/setup.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 21:34:42.970808 nvm-0.1.0/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-0.1.0/tests/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1563 2023-05-05 15:01:56.000000 nvm-0.1.0/tests/test_aux_str.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-0.1.0/tests/test_nvm.py
+-rw-------   0 jiko      (1000) jiko      (1000)      533 2023-05-03 18:32:02.000000 nvm-0.1.0/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-0.1.0/versioneer.py
```

### Comparing `nvm-0.0.4/.gitignore` & `nvm-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/CONTRIBUTING.rst` & `nvm-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/LICENSE` & `nvm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/Makefile` & `nvm-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/PKG-INFO` & `nvm-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.0.4
+Version: 0.1.0
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,35 +25,42 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===
 NVM
 ===
 
-
-.. image:: https://img.shields.io/pypi/v/nvm.svg
-        :target: https://pypi.python.org/pypi/nvm
+.. image:: https://img.shields.io/pypi/v/nvm
+   :target: https://pypi.python.org/pypi/nvm
+   :alt: PyPI Version
 
 .. image:: https://readthedocs.org/projects/nvm/badge/?version=latest
-        :target: https://nvm.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
+   :target: https://nvm.readthedocs.io/en/latest
+   :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/l/nvm?color=blue
+   :target: https://github.com/cogsys-io/nvm/blob/master/LICENSE
+   :alt: License
+
+.. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/nvm/build-main.yml
+   :alt: GitHub Workflow (Build Main) Status
+   :target: https://github.com/cogsys-io/nvm
 
 
 Plenty little helpers.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://nvm.readthedocs.io.
 
 
 Features
 --------
 
+* Plenty little helpers.
 * TODO
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `cogsys-io/cogsys-io-cookiecutter-pypackage`_ project template.
```

### Comparing `nvm-0.0.4/README.rst` & `nvm-0.1.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 ===
 NVM
 ===
 
-
-.. image:: https://img.shields.io/pypi/v/nvm.svg
-        :target: https://pypi.python.org/pypi/nvm
+.. image:: https://img.shields.io/pypi/v/nvm
+   :target: https://pypi.python.org/pypi/nvm
+   :alt: PyPI Version
 
 .. image:: https://readthedocs.org/projects/nvm/badge/?version=latest
-        :target: https://nvm.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
+   :target: https://nvm.readthedocs.io/en/latest
+   :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/l/nvm?color=blue
+   :target: https://github.com/cogsys-io/nvm/blob/master/LICENSE
+   :alt: License
+
+.. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/nvm/build-main.yml
+   :alt: GitHub Workflow (Build Main) Status
+   :target: https://github.com/cogsys-io/nvm
 
 
 Plenty little helpers.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://nvm.readthedocs.io.
 
 
 Features
 --------
 
+* Plenty little helpers.
 * TODO
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `cogsys-io/cogsys-io-cookiecutter-pypackage`_ project template.
```

### Comparing `nvm-0.0.4/data/emacs-logo/emacs-128x128.png` & `nvm-0.1.0/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/data/emacs-logo/emacs.svg` & `nvm-0.1.0/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/docs/Makefile` & `nvm-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-0.1.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/docs/source/conf.py` & `nvm-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/docs/source/installation.rst` & `nvm-0.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/nvm/aux_log/aux_log.py` & `nvm-0.1.0/nvm/aux_log/aux_log.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/nvm/aux_pandas/aux_pandas.py` & `nvm-0.1.0/nvm/aux_pandas/aux_pandas.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     df0.columns = df0.columns.map(lambda x: x.replace(".", "_"))
     if lowercase:
         df0.columns = df0.columns.map(str.lower)
 
     return df0
 
 
-def context_pandas(
+def _context_pandas(
     max_columns=222,
     max_colwidth=44,
     width=2222,
     max_rows=44,
     min_rows=33,
 ):
     """Apply custom context to dataframe representation (ExitStack)."""
@@ -52,9 +52,9 @@
     >>> import pandas as pd
     >>> from nvm import disp_df
     >>> from nvm.aux_pandas import wine_df
     >>> disp_df(df0)
 
     """
     with ExitStack() as stack:
-        _ = [stack.enter_context(cont) for cont in context_pandas(**opt)]
+        _ = [stack.enter_context(cont) for cont in _context_pandas(**opt)]
         display(df0)
```

### Comparing `nvm-0.0.4/nvm/aux_sys/aux_sys.py` & `nvm-0.1.0/nvm/aux_sys/aux_sys.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,35 @@
 )
 
 
 def chdir(
     locations: Dict[str, Dict[str, str]],
     log0: Optional[logging.Logger] = logging.getLogger("dummy"),
 ) -> str:
-    """
-    Change current directory according to hostname and username.
+    """Change current directory according to hostname and username.
 
     Target directory path is relative to user's ``${HOME}`` directory.
 
     Parameters
     ----------
     locations : Dict[str, Dict[str, str]]
         Dictionary containing locations, usernames and paths.
     log0 : Optional[logging.Logger]
         Logger.
 
     Examples
     --------
     >>> import srsly
     >>> import nvm
-    >>> locations = '''
+    >>> locations = \'\'\'
     >>> stardust7:
     >>>   jiko: cc/dev/
     >>> buka2:
     >>>   jiko: cc/cfg/
-    >>> '''
+    >>> \'\'\'
     >>> locations = srsly.yaml_loads(locations)
     >>> print(nvm.chdir(locations))
 
     """
     hostname = str(socket.gethostname())
     username = str(pwd.getpwuid(os.getuid()).pw_name)
     log0.debug(f"{hostname = }")
```

### Comparing `nvm-0.0.4/nvm.egg-info/PKG-INFO` & `nvm-0.1.0/nvm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 0.0.4
+Version: 0.1.0
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,35 +25,42 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===
 NVM
 ===
 
-
-.. image:: https://img.shields.io/pypi/v/nvm.svg
-        :target: https://pypi.python.org/pypi/nvm
+.. image:: https://img.shields.io/pypi/v/nvm
+   :target: https://pypi.python.org/pypi/nvm
+   :alt: PyPI Version
 
 .. image:: https://readthedocs.org/projects/nvm/badge/?version=latest
-        :target: https://nvm.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
+   :target: https://nvm.readthedocs.io/en/latest
+   :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/l/nvm?color=blue
+   :target: https://github.com/cogsys-io/nvm/blob/master/LICENSE
+   :alt: License
+
+.. image:: https://img.shields.io/github/actions/workflow/status/cogsys-io/nvm/build-main.yml
+   :alt: GitHub Workflow (Build Main) Status
+   :target: https://github.com/cogsys-io/nvm
 
 
 Plenty little helpers.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://nvm.readthedocs.io.
 
 
 Features
 --------
 
+* Plenty little helpers.
 * TODO
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `cogsys-io/cogsys-io-cookiecutter-pypackage`_ project template.
```

### Comparing `nvm-0.0.4/nvm.egg-info/SOURCES.txt` & `nvm-0.1.0/nvm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 .editorconfig
 .gitattributes
 .gitignore
+.readthedocs.yaml
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 pyproject.toml
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 versioneer.py
-.github/ISSUE_TEMPLATE.md
+.github/PULL_REQUEST_TEMPLATE.md
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/build-main.yml
 bin/.gitkeep
 bin/nvm.py
 data/.gitkeep
 data/emacs-logo/emacs-128x128.png
 data/emacs-logo/emacs.svg
 docs/Makefile
 docs/requirements.txt
@@ -32,14 +36,15 @@
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/history.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/modules.rst
 docs/source/nvm.aux_log.rst
+docs/source/nvm.aux_pandas.rst
 docs/source/nvm.aux_str.rst
 docs/source/nvm.aux_sys.rst
 docs/source/nvm.rst
 docs/source/readme.rst
 docs/source/usage.rst
 docs/source/_static/.gitkeep
 nvm/__init__.py
@@ -54,11 +59,13 @@
 nvm.egg-info/top_level.txt
 nvm/aux_log/__init__.py
 nvm/aux_log/aux_log.py
 nvm/aux_pandas/__init__.py
 nvm/aux_pandas/aux_pandas.py
 nvm/aux_str/__init__.py
 nvm/aux_str/aux_str.py
+nvm/aux_str/clean_str_mappings.py
 nvm/aux_sys/__init__.py
 nvm/aux_sys/aux_sys.py
 tests/__init__.py
+tests/test_aux_str.py
 tests/test_nvm.py
```

### Comparing `nvm-0.0.4/nvm.egg-info/requires.txt` & `nvm-0.1.0/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/pyproject.toml` & `nvm-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/setup.cfg` & `nvm-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/setup.py` & `nvm-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/tests/test_nvm.py` & `nvm-0.1.0/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/tox.ini` & `nvm-0.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `nvm-0.0.4/versioneer.py` & `nvm-0.1.0/versioneer.py`

 * *Files identical despite different names*

