# Comparing `tmp/qtconsole-5.4.2.tar.gz` & `tmp/qtconsole-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtconsole-5.4.2.tar", last modified: Sun Apr  2 21:18:07 2023, max compression
+gzip compressed data, was "qtconsole-5.4.3.tar", last modified: Fri May  5 17:41:21 2023, max compression
```

## Comparing `qtconsole-5.4.2.tar` & `qtconsole-5.4.3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.629845 qtconsole-5.4.2/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       44 2020-10-24 15:40:21.000000 qtconsole-5.4.2/.coveragerc
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.609845 qtconsole-5.4.2/.github/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.613845 qtconsole-5.4.2/.github/workflows/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2620 2023-03-07 00:10:49.000000 qtconsole-5.4.2/.github/workflows/linux-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1346 2023-03-07 00:10:49.000000 qtconsole-5.4.2/.github/workflows/macos-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1360 2023-03-07 00:10:49.000000 qtconsole-5.4.2/.github/workflows/windows-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      342 2020-10-24 15:40:21.000000 qtconsole-5.4.2/.gitignore
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10807 2015-12-20 14:40:14.000000 qtconsole-5.4.2/.mailmap
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      624 2022-03-27 18:25:58.000000 qtconsole-5.4.2/CONTRIBUTING.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1528 2020-10-24 15:40:21.000000 qtconsole-5.4.2/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      371 2020-10-24 15:40:21.000000 qtconsole-5.4.2/MANIFEST.in
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4610 2023-04-02 21:18:07.629845 qtconsole-5.4.2/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3665 2021-03-17 01:07:09.000000 qtconsole-5.4.2/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      678 2020-10-24 15:40:21.000000 qtconsole-5.4.2/RELEASE.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.613845 qtconsole-5.4.2/docs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7886 2015-12-20 14:40:14.000000 qtconsole-5.4.2/docs/Makefile
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1007 2020-10-24 15:40:21.000000 qtconsole-5.4.2/docs/autogen_config.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      161 2022-03-27 18:25:58.000000 qtconsole-5.4.2/docs/environment.yml
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4166 2021-03-17 01:07:09.000000 qtconsole-5.4.2/docs/gh-pages.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.613845 qtconsole-5.4.2/docs/source/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.613845 qtconsole-5.4.2/docs/source/_images/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   153249 2015-12-20 14:40:14.000000 qtconsole-5.4.2/docs/source/_images/qtconsole.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11348 2023-04-02 21:15:37.000000 qtconsole-5.4.2/docs/source/changelog.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10284 2021-03-17 01:07:09.000000 qtconsole-5.4.2/docs/source/conf.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.617845 qtconsole-5.4.2/docs/source/figs/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    53726 2015-12-20 14:40:14.000000 qtconsole-5.4.2/docs/source/figs/besselj.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    61184 2015-12-20 14:40:14.000000 qtconsole-5.4.2/docs/source/figs/colors_dark.png
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    44935 2015-12-20 14:40:14.000000 qtconsole-5.4.2/docs/source/figs/jn.html
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    29224 2015-12-20 14:40:14.000000 qtconsole-5.4.2/docs/source/figs/jn.xhtml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    18580 2020-10-24 15:40:21.000000 qtconsole-5.4.2/docs/source/index.rst
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1630 2020-10-24 15:40:21.000000 qtconsole-5.4.2/docs/source/installation.rst
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.617845 qtconsole-5.4.2/examples/
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1580 2020-10-24 15:40:21.000000 qtconsole-5.4.2/examples/embed_qtconsole.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1057 2020-10-24 15:40:21.000000 qtconsole-5.4.2/examples/inprocess_qtconsole.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      421 2020-10-24 15:40:21.000000 qtconsole-5.4.2/examples/jupyter-qtconsole.desktop
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.625845 qtconsole-5.4.2/qtconsole/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       48 2015-12-20 14:40:14.000000 qtconsole-5.4.2/qtconsole/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       82 2015-12-20 14:40:14.000000 qtconsole-5.4.2/qtconsole/__main__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       72 2023-04-02 21:17:22.000000 qtconsole-5.4.2/qtconsole/_version.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14185 2021-11-14 18:48:23.000000 qtconsole-5.4.2/qtconsole/ansi_code_processor.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     6295 2021-11-14 18:48:23.000000 qtconsole-5.4.2/qtconsole/base_frontend_mixin.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3733 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/bracket_matcher.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10683 2022-03-27 18:25:58.000000 qtconsole-5.4.2/qtconsole/call_tip_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1971 2023-03-30 15:34:17.000000 qtconsole-5.4.2/qtconsole/client.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8888 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/comms.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    12957 2022-10-29 16:58:15.000000 qtconsole-5.4.2/qtconsole/completion_html.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2247 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/completion_plain.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8151 2022-10-29 16:58:15.000000 qtconsole-5.4.2/qtconsole/completion_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   105444 2022-11-02 00:49:56.000000 qtconsole-5.4.2/qtconsole/console_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    34897 2023-03-30 15:34:17.000000 qtconsole-5.4.2/qtconsole/frontend_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9947 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/history_console_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2753 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/inprocess.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      169 2020-10-24 15:40:21.000000 qtconsole-5.4.2/qtconsole/ipython_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    24994 2023-03-28 21:52:03.000000 qtconsole-5.4.2/qtconsole/jupyter_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1813 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/kernel_mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3793 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/kill_ring.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    38402 2022-05-29 16:43:26.000000 qtconsole-5.4.2/qtconsole/mainwindow.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2602 2023-03-28 21:52:03.000000 qtconsole-5.4.2/qtconsole/manager.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9119 2021-05-02 17:44:56.000000 qtconsole-5.4.2/qtconsole/pygments_highlighter.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      540 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/qstringhelpers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    17229 2023-03-11 20:35:38.000000 qtconsole-5.4.2/qtconsole/qtconsoleapp.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.609845 qtconsole-5.4.2/qtconsole/resources/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.625845 qtconsole-5.4.2/qtconsole/resources/icon/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    26397 2015-12-20 14:40:14.000000 qtconsole-5.4.2/qtconsole/resources/icon/JupyterConsole.svg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      184 2020-10-24 15:40:21.000000 qtconsole-5.4.2/qtconsole/rich_ipython_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    17956 2023-03-07 00:10:49.000000 qtconsole-5.4.2/qtconsole/rich_jupyter_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8638 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/rich_text.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3801 2020-10-24 15:40:21.000000 qtconsole-5.4.2/qtconsole/styles.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2394 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/svg.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.629845 qtconsole-5.4.2/qtconsole/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      132 2020-10-24 15:40:22.000000 qtconsole-5.4.2/qtconsole/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    26302 2023-03-28 21:52:03.000000 qtconsole-5.4.2/qtconsole/tests/test_00_console_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7430 2021-11-14 18:48:23.000000 qtconsole-5.4.2/qtconsole/tests/test_ansi_code_processor.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1003 2020-10-24 15:40:22.000000 qtconsole-5.4.2/qtconsole/tests/test_app.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5400 2021-05-02 17:44:56.000000 qtconsole-5.4.2/qtconsole/tests/test_comms.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3343 2021-03-17 01:07:09.000000 qtconsole-5.4.2/qtconsole/tests/test_completion_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2020-10-24 15:40:22.000000 qtconsole-5.4.2/qtconsole/tests/test_frontend_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4976 2023-03-07 00:10:49.000000 qtconsole-5.4.2/qtconsole/tests/test_jupyter_widget.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2278 2020-10-24 15:40:22.000000 qtconsole-5.4.2/qtconsole/tests/test_kill_ring.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      519 2020-10-24 15:40:22.000000 qtconsole-5.4.2/qtconsole/tests/test_styles.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     8349 2020-10-24 15:40:22.000000 qtconsole-5.4.2/qtconsole/usage.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3976 2021-04-07 19:47:19.000000 qtconsole-5.4.2/qtconsole/util.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.625845 qtconsole-5.4.2/qtconsole.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4610 2023-04-02 21:18:07.000000 qtconsole-5.4.2/qtconsole.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2099 2023-04-02 21:18:07.000000 qtconsole-5.4.2/qtconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-04-02 21:18:07.000000 qtconsole-5.4.2/qtconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       62 2023-04-02 21:18:07.000000 qtconsole-5.4.2/qtconsole.egg-info/entry_points.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      183 2023-04-02 21:18:07.000000 qtconsole-5.4.2/qtconsole.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-04-02 21:18:07.000000 qtconsole-5.4.2/qtconsole.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       88 2020-10-24 15:40:22.000000 qtconsole-5.4.2/readthedocs.yml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 21:18:07.629845 qtconsole-5.4.2/requirements/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      252 2022-03-27 18:25:58.000000 qtconsole-5.4.2/requirements/environment.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-04-02 21:18:07.629845 qtconsole-5.4.2/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3314 2023-03-11 20:35:38.000000 qtconsole-5.4.2/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.943406 qtconsole-5.4.3/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       44 2020-10-24 15:40:21.000000 qtconsole-5.4.3/.coveragerc
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.923405 qtconsole-5.4.3/.github/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.923405 qtconsole-5.4.3/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2620 2023-03-07 00:10:49.000000 qtconsole-5.4.3/.github/workflows/linux-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1346 2023-03-07 00:10:49.000000 qtconsole-5.4.3/.github/workflows/macos-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1360 2023-03-07 00:10:49.000000 qtconsole-5.4.3/.github/workflows/windows-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      350 2023-05-05 17:34:26.000000 qtconsole-5.4.3/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10807 2015-12-20 14:40:14.000000 qtconsole-5.4.3/.mailmap
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      624 2022-03-27 18:25:58.000000 qtconsole-5.4.3/CONTRIBUTING.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1528 2020-10-24 15:40:21.000000 qtconsole-5.4.3/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      371 2020-10-24 15:40:21.000000 qtconsole-5.4.3/MANIFEST.in
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4610 2023-05-05 17:41:21.943406 qtconsole-5.4.3/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3665 2021-03-17 01:07:09.000000 qtconsole-5.4.3/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      678 2020-10-24 15:40:21.000000 qtconsole-5.4.3/RELEASE.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.927405 qtconsole-5.4.3/docs/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7886 2015-12-20 14:40:14.000000 qtconsole-5.4.3/docs/Makefile
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1007 2020-10-24 15:40:21.000000 qtconsole-5.4.3/docs/autogen_config.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      161 2022-03-27 18:25:58.000000 qtconsole-5.4.3/docs/environment.yml
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4166 2021-03-17 01:07:09.000000 qtconsole-5.4.3/docs/gh-pages.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.927405 qtconsole-5.4.3/docs/source/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.927405 qtconsole-5.4.3/docs/source/_images/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   153249 2015-12-20 14:40:14.000000 qtconsole-5.4.3/docs/source/_images/qtconsole.png
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11490 2023-05-05 17:37:08.000000 qtconsole-5.4.3/docs/source/changelog.rst
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10284 2021-03-17 01:07:09.000000 qtconsole-5.4.3/docs/source/conf.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.931405 qtconsole-5.4.3/docs/source/figs/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    53726 2015-12-20 14:40:14.000000 qtconsole-5.4.3/docs/source/figs/besselj.png
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    61184 2015-12-20 14:40:14.000000 qtconsole-5.4.3/docs/source/figs/colors_dark.png
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    44935 2015-12-20 14:40:14.000000 qtconsole-5.4.3/docs/source/figs/jn.html
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    29224 2015-12-20 14:40:14.000000 qtconsole-5.4.3/docs/source/figs/jn.xhtml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    18580 2020-10-24 15:40:21.000000 qtconsole-5.4.3/docs/source/index.rst
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1630 2020-10-24 15:40:21.000000 qtconsole-5.4.3/docs/source/installation.rst
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.931405 qtconsole-5.4.3/examples/
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     1580 2020-10-24 15:40:21.000000 qtconsole-5.4.3/examples/embed_qtconsole.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1057 2020-10-24 15:40:21.000000 qtconsole-5.4.3/examples/inprocess_qtconsole.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      421 2020-10-24 15:40:21.000000 qtconsole-5.4.3/examples/jupyter-qtconsole.desktop
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.939406 qtconsole-5.4.3/qtconsole/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       48 2015-12-20 14:40:14.000000 qtconsole-5.4.3/qtconsole/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       82 2015-12-20 14:40:14.000000 qtconsole-5.4.3/qtconsole/__main__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       72 2023-05-05 17:38:42.000000 qtconsole-5.4.3/qtconsole/_version.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    14185 2021-11-14 18:48:23.000000 qtconsole-5.4.3/qtconsole/ansi_code_processor.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     6295 2021-11-14 18:48:23.000000 qtconsole-5.4.3/qtconsole/base_frontend_mixin.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3733 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/bracket_matcher.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10683 2022-03-27 18:25:58.000000 qtconsole-5.4.3/qtconsole/call_tip_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1971 2023-03-30 15:34:17.000000 qtconsole-5.4.3/qtconsole/client.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8888 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/comms.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12957 2022-10-29 16:58:15.000000 qtconsole-5.4.3/qtconsole/completion_html.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2247 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/completion_plain.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8151 2022-10-29 16:58:15.000000 qtconsole-5.4.3/qtconsole/completion_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   105444 2022-11-02 00:49:56.000000 qtconsole-5.4.3/qtconsole/console_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    34897 2023-03-30 15:34:17.000000 qtconsole-5.4.3/qtconsole/frontend_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9947 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/history_console_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2874 2023-05-05 17:34:26.000000 qtconsole-5.4.3/qtconsole/inprocess.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      169 2020-10-24 15:40:21.000000 qtconsole-5.4.3/qtconsole/ipython_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    24994 2023-03-28 21:52:03.000000 qtconsole-5.4.3/qtconsole/jupyter_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1813 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/kernel_mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3793 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/kill_ring.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    38402 2022-05-29 16:43:26.000000 qtconsole-5.4.3/qtconsole/mainwindow.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2602 2023-03-28 21:52:03.000000 qtconsole-5.4.3/qtconsole/manager.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9119 2021-05-02 17:44:56.000000 qtconsole-5.4.3/qtconsole/pygments_highlighter.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      540 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/qstringhelpers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17229 2023-03-11 20:35:38.000000 qtconsole-5.4.3/qtconsole/qtconsoleapp.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.923405 qtconsole-5.4.3/qtconsole/resources/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.943406 qtconsole-5.4.3/qtconsole/resources/icon/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    26397 2015-12-20 14:40:14.000000 qtconsole-5.4.3/qtconsole/resources/icon/JupyterConsole.svg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      184 2020-10-24 15:40:21.000000 qtconsole-5.4.3/qtconsole/rich_ipython_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17956 2023-03-07 00:10:49.000000 qtconsole-5.4.3/qtconsole/rich_jupyter_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8638 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/rich_text.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3801 2020-10-24 15:40:21.000000 qtconsole-5.4.3/qtconsole/styles.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2394 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/svg.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.943406 qtconsole-5.4.3/qtconsole/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      132 2020-10-24 15:40:22.000000 qtconsole-5.4.3/qtconsole/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    26302 2023-03-28 21:52:03.000000 qtconsole-5.4.3/qtconsole/tests/test_00_console_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7430 2021-11-14 18:48:23.000000 qtconsole-5.4.3/qtconsole/tests/test_ansi_code_processor.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1003 2020-10-24 15:40:22.000000 qtconsole-5.4.3/qtconsole/tests/test_app.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5400 2021-05-02 17:44:56.000000 qtconsole-5.4.3/qtconsole/tests/test_comms.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3343 2021-03-17 01:07:09.000000 qtconsole-5.4.3/qtconsole/tests/test_completion_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3219 2020-10-24 15:40:22.000000 qtconsole-5.4.3/qtconsole/tests/test_frontend_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      976 2023-05-05 17:34:26.000000 qtconsole-5.4.3/qtconsole/tests/test_inprocess_kernel.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4976 2023-03-07 00:10:49.000000 qtconsole-5.4.3/qtconsole/tests/test_jupyter_widget.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2278 2020-10-24 15:40:22.000000 qtconsole-5.4.3/qtconsole/tests/test_kill_ring.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      519 2020-10-24 15:40:22.000000 qtconsole-5.4.3/qtconsole/tests/test_styles.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     8349 2020-10-24 15:40:22.000000 qtconsole-5.4.3/qtconsole/usage.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3976 2021-04-07 19:47:19.000000 qtconsole-5.4.3/qtconsole/util.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.943406 qtconsole-5.4.3/qtconsole.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4610 2023-05-05 17:41:21.000000 qtconsole-5.4.3/qtconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2140 2023-05-05 17:41:21.000000 qtconsole-5.4.3/qtconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-05 17:41:21.000000 qtconsole-5.4.3/qtconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       62 2023-05-05 17:41:21.000000 qtconsole-5.4.3/qtconsole.egg-info/entry_points.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      183 2023-05-05 17:41:21.000000 qtconsole-5.4.3/qtconsole.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-05 17:41:21.000000 qtconsole-5.4.3/qtconsole.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       88 2020-10-24 15:40:22.000000 qtconsole-5.4.3/readthedocs.yml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-05 17:41:21.943406 qtconsole-5.4.3/requirements/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      252 2022-03-27 18:25:58.000000 qtconsole-5.4.3/requirements/environment.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-05 17:41:21.943406 qtconsole-5.4.3/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3314 2023-03-11 20:35:38.000000 qtconsole-5.4.3/setup.py
```

### Comparing `qtconsole-5.4.2/.github/workflows/linux-tests.yml` & `qtconsole-5.4.3/.github/workflows/linux-tests.yml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/.github/workflows/macos-tests.yml` & `qtconsole-5.4.3/.github/workflows/macos-tests.yml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/.github/workflows/windows-tests.yml` & `qtconsole-5.4.3/.github/workflows/windows-tests.yml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/.mailmap` & `qtconsole-5.4.3/.mailmap`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/CONTRIBUTING.md` & `qtconsole-5.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/LICENSE` & `qtconsole-5.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/PKG-INFO` & `qtconsole-5.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtconsole
-Version: 5.4.2
+Version: 5.4.3
 Summary: Jupyter Qt console
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 Maintainer: Spyder Development Team
 License: BSD
 Keywords: Interactive,Interpreter,Shell
```

### Comparing `qtconsole-5.4.2/README.md` & `qtconsole-5.4.3/README.md`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/RELEASE.md` & `qtconsole-5.4.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/Makefile` & `qtconsole-5.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/autogen_config.py` & `qtconsole-5.4.3/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/gh-pages.py` & `qtconsole-5.4.3/docs/gh-pages.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/_images/qtconsole.png` & `qtconsole-5.4.3/docs/source/_images/qtconsole.png`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/changelog.rst` & `qtconsole-5.4.3/docs/source/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 =============================
 
 .. _5.4:
 
 5.4
 ~~~
 
+5.4.3
+-----
+
+`5.4.3 on GitHub <https://github.com/jupyter/qtconsole/milestones/5.4.3>`__
+
+* Add missing closed method to QtInProcessChannel.
+
 5.4.2
 -----
 
 `5.4.2 on GitHub <https://github.com/jupyter/qtconsole/milestones/5.4.2>`__
 
 * Check if the iopub channel is not closed before flushing it.
 * Fix kernel autorestart after it's killed for Jupyter-client 8+.
```

### Comparing `qtconsole-5.4.2/docs/source/conf.py` & `qtconsole-5.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/figs/besselj.png` & `qtconsole-5.4.3/docs/source/figs/besselj.png`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/figs/colors_dark.png` & `qtconsole-5.4.3/docs/source/figs/colors_dark.png`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/figs/jn.html` & `qtconsole-5.4.3/docs/source/figs/jn.html`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/figs/jn.xhtml` & `qtconsole-5.4.3/docs/source/figs/jn.xhtml`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/index.rst` & `qtconsole-5.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/docs/source/installation.rst` & `qtconsole-5.4.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/examples/embed_qtconsole.py` & `qtconsole-5.4.3/examples/embed_qtconsole.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/examples/inprocess_qtconsole.py` & `qtconsole-5.4.3/examples/inprocess_qtconsole.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/ansi_code_processor.py` & `qtconsole-5.4.3/qtconsole/ansi_code_processor.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/base_frontend_mixin.py` & `qtconsole-5.4.3/qtconsole/base_frontend_mixin.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/bracket_matcher.py` & `qtconsole-5.4.3/qtconsole/bracket_matcher.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/call_tip_widget.py` & `qtconsole-5.4.3/qtconsole/call_tip_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/client.py` & `qtconsole-5.4.3/qtconsole/client.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/comms.py` & `qtconsole-5.4.3/qtconsole/comms.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/completion_html.py` & `qtconsole-5.4.3/qtconsole/completion_html.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/completion_plain.py` & `qtconsole-5.4.3/qtconsole/completion_plain.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/completion_widget.py` & `qtconsole-5.4.3/qtconsole/completion_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/console_widget.py` & `qtconsole-5.4.3/qtconsole/console_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/frontend_widget.py` & `qtconsole-5.4.3/qtconsole/frontend_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/history_console_widget.py` & `qtconsole-5.4.3/qtconsole/history_console_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/inprocess.py` & `qtconsole-5.4.3/qtconsole/inprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 
     def flush(self, timeout=1.0):
         """ Reimplemented to ensure that signals are dispatched immediately.
         """
         super().flush()
         self.process_events()
 
+    def closed(self):
+        """ Function to ensure compatibility with the QtZMQSocketChannel."""
+        return False
+
 
 class QtInProcessHBChannel(SuperQObject, InProcessHBChannel):
     # This signal will never be fired, but it needs to exist
     kernel_died = QtCore.Signal()
 
 
 class QtInProcessKernelClient(QtKernelClientMixin, InProcessKernelClient):
```

### Comparing `qtconsole-5.4.2/qtconsole/jupyter_widget.py` & `qtconsole-5.4.3/qtconsole/jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/kernel_mixins.py` & `qtconsole-5.4.3/qtconsole/kernel_mixins.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/kill_ring.py` & `qtconsole-5.4.3/qtconsole/kill_ring.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/mainwindow.py` & `qtconsole-5.4.3/qtconsole/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/manager.py` & `qtconsole-5.4.3/qtconsole/manager.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/pygments_highlighter.py` & `qtconsole-5.4.3/qtconsole/pygments_highlighter.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/qstringhelpers.py` & `qtconsole-5.4.3/qtconsole/qstringhelpers.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/qtconsoleapp.py` & `qtconsole-5.4.3/qtconsole/qtconsoleapp.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/resources/icon/JupyterConsole.svg` & `qtconsole-5.4.3/qtconsole/resources/icon/JupyterConsole.svg`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/rich_jupyter_widget.py` & `qtconsole-5.4.3/qtconsole/rich_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/rich_text.py` & `qtconsole-5.4.3/qtconsole/rich_text.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/styles.py` & `qtconsole-5.4.3/qtconsole/styles.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/svg.py` & `qtconsole-5.4.3/qtconsole/svg.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_00_console_widget.py` & `qtconsole-5.4.3/qtconsole/tests/test_00_console_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_ansi_code_processor.py` & `qtconsole-5.4.3/qtconsole/tests/test_ansi_code_processor.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_app.py` & `qtconsole-5.4.3/qtconsole/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_comms.py` & `qtconsole-5.4.3/qtconsole/tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_completion_widget.py` & `qtconsole-5.4.3/qtconsole/tests/test_completion_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_frontend_widget.py` & `qtconsole-5.4.3/qtconsole/tests/test_frontend_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_jupyter_widget.py` & `qtconsole-5.4.3/qtconsole/tests/test_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_kill_ring.py` & `qtconsole-5.4.3/qtconsole/tests/test_kill_ring.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/tests/test_styles.py` & `qtconsole-5.4.3/qtconsole/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/usage.py` & `qtconsole-5.4.3/qtconsole/usage.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole/util.py` & `qtconsole-5.4.3/qtconsole/util.py`

 * *Files identical despite different names*

### Comparing `qtconsole-5.4.2/qtconsole.egg-info/PKG-INFO` & `qtconsole-5.4.3/qtconsole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtconsole
-Version: 5.4.2
+Version: 5.4.3
 Summary: Jupyter Qt console
 Home-page: http://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 Maintainer: Spyder Development Team
 License: BSD
 Keywords: Interactive,Interpreter,Shell
```

### Comparing `qtconsole-5.4.2/qtconsole.egg-info/SOURCES.txt` & `qtconsole-5.4.3/qtconsole.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,11 +69,12 @@
 qtconsole/tests/__init__.py
 qtconsole/tests/test_00_console_widget.py
 qtconsole/tests/test_ansi_code_processor.py
 qtconsole/tests/test_app.py
 qtconsole/tests/test_comms.py
 qtconsole/tests/test_completion_widget.py
 qtconsole/tests/test_frontend_widget.py
+qtconsole/tests/test_inprocess_kernel.py
 qtconsole/tests/test_jupyter_widget.py
 qtconsole/tests/test_kill_ring.py
 qtconsole/tests/test_styles.py
 requirements/environment.yml
```

### Comparing `qtconsole-5.4.2/setup.py` & `qtconsole-5.4.3/setup.py`

 * *Files identical despite different names*

