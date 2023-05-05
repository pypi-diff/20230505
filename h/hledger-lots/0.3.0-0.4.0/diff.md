# Comparing `tmp/hledger_lots-0.3.0.tar.gz` & `tmp/hledger_lots-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.3.0.tar", last modified: Wed May  3 17:00:37 2023, max compression
+gzip compressed data, was "hledger_lots-0.4.0.tar", last modified: Fri May  5 17:38:54 2023, max compression
```

## Comparing `hledger_lots-0.3.0.tar` & `hledger_lots-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5683 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.403625 hledger_lots-0.3.0/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5343 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.406625 hledger_lots-0.3.0/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2719 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13625 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1589 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/commodity_tag.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3245 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      913 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4277 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2758 2023-04-24 18:30:26.000000 hledger_lots-0.3.0/hledger_lots/lib.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4161 2023-05-03 16:08:12.000000 hledger_lots-0.3.0/hledger_lots/prices_yahoo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7340 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/prompt.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/prompt_buy.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/hledger_lots/prompt_sell.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.407625 hledger_lots-0.3.0/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5683 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1111 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-05-03 17:00:37.000000 hledger_lots-0.3.0/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-05-03 16:56:13.000000 hledger_lots-0.3.0/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.409625 hledger_lots-0.3.0/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.3.0/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.3.0/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.3.0/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.402625 hledger_lots-0.3.0/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-03 17:00:37.412625 hledger_lots-0.3.0/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.3.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.982166 hledger_lots-0.4.0/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5711 2023-05-05 17:38:54.982166 hledger_lots-0.4.0/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.971166 hledger_lots-0.4.0/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5371 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.975165 hledger_lots-0.4.0/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       95 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2882 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7839 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1589 2023-05-03 16:08:12.000000 hledger_lots-0.4.0/hledger_lots/commodity_tag.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3423 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1707 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4267 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3231 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/options.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4404 2023-05-05 17:38:44.000000 hledger_lots-0.4.0/hledger_lots/prices_yahoo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7421 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/prompt.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/hledger_lots/prompt_buy.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/hledger_lots/prompt_sell.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.976166 hledger_lots-0.4.0/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5711 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1135 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-05-05 17:37:51.000000 hledger_lots-0.4.0/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-05 17:38:54.982166 hledger_lots-0.4.0/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.978165 hledger_lots-0.4.0/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3080 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.971166 hledger_lots-0.4.0/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.981166 hledger_lots-0.4.0/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.3.0/PKG-INFO` & `hledger_lots-0.4.0/docs/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: hledger_lots
-Version: 0.3.0
-License: MIT License
-Project-URL: homepage, https://github.com/edkedk99/hledger-lots
-Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
-Project-URL: repository, https://github.com/edkedk99/hledger-lots
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Hledger-lots
 
 ![automatic lots](img/meme.jpg)
 
 This package helps [hledger](https://hledger.org/) users to add and manage transactions involving buying and selling commodities like stock, currency, etc.
 
 ## Features
@@ -52,36 +42,39 @@
 The indicators provided by these command are explained [here](#indicators).
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
 
-## Installation
+## Setup
 
 ### Requirements
 
 - [python](https://www.python.org/)
 - [hledger](https://hledger.org/1.29/hledger.html#p-directive)
 
-### Command
+### Install
 
 ```python
 pip install --upgrade hledger-lots
 ```
 
-## Workflow
+### Config
 
-1. Add purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
-2. Download market price history as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
-3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
-4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
+Instead of using command options, which is hard to remember and makes the command long, environment variables, which demands tweaking the .bashrc file or a configuration file, this app add configuration options directly in the journal using a custom directives specification explained [here](config)
 
-> By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
+> You can still use **LEDGER_FILE** environment variable by adding `export LEDGER_FILE=your_data.journal` or prepend to the command: `LEDGER_FILE=your_data.journal hledger-lots ...`
 
+## Workflow
+
+1. Add a commodity purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See some examples [here](examples/data.journal)
+2. Download market price history from [Yahoo Finance](https://finance.yahoo.com/) as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
+3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list).
+4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
@@ -102,15 +95,13 @@
 
 The sale transaction gives you the calculated **xirr** as tag, which is the internal rate of return of an investment based on a specified series of irregularly spaced cash flows. This value is annual percentage rate following the 30/360US day count convention. It is a good metric to compare the investment return with a benchmark like the S&P or the T-Bill, for example.
 
 > Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
 
 ## Checks
 
-It is recommended to use the option *--check* to ensure you past selling transaction has the correct cost according to the choosen cost method. It can be enabled by setting the environment variable **HLEDGER_LOTS_CHECK** to "true". It can be disabled with the option *--no-check* or setting the environment variable **HLEDGER_LOTS_CHECK** to "false".
-
-> At the moment the default is set to "false", but expect it to be turned to "true" in future releases.
+It is recommended to set the option *check* to true to ensure you past selling transaction has the correct cost according to the choosen cost method. See how to set it up [here](config)
 
 ## Limitations
 
 - No _short-selling_
 - Each commodity can have only one base currency. For example, it is not possible to buy AAPL with USD and later with EUR.
```

### Comparing `hledger_lots-0.3.0/docs/README.md` & `hledger_lots-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: hledger_lots
+Version: 0.4.0
+License: MIT License
+Project-URL: homepage, https://github.com/edkedk99/hledger-lots
+Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
+Project-URL: repository, https://github.com/edkedk99/hledger-lots
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # Hledger-lots
 
 ![automatic lots](img/meme.jpg)
 
 This package helps [hledger](https://hledger.org/) users to add and manage transactions involving buying and selling commodities like stock, currency, etc.
 
 ## Features
@@ -42,36 +52,39 @@
 The indicators provided by these command are explained [here](#indicators).
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
 
-## Installation
+## Setup
 
 ### Requirements
 
 - [python](https://www.python.org/)
 - [hledger](https://hledger.org/1.29/hledger.html#p-directive)
 
-### Command
+### Install
 
 ```python
 pip install --upgrade hledger-lots
 ```
 
-## Workflow
+### Config
 
-1. Add purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
-2. Download market price history as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
-3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
-4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
+Instead of using command options, which is hard to remember and makes the command long, environment variables, which demands tweaking the .bashrc file or a configuration file, this app add configuration options directly in the journal using a custom directives specification explained [here](config)
 
-> By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
+> You can still use **LEDGER_FILE** environment variable by adding `export LEDGER_FILE=your_data.journal` or prepend to the command: `LEDGER_FILE=your_data.journal hledger-lots ...`
 
+## Workflow
+
+1. Add a commodity purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See some examples [here](examples/data.journal)
+2. Download market price history from [Yahoo Finance](https://finance.yahoo.com/) as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
+3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list).
+4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
@@ -92,15 +105,13 @@
 
 The sale transaction gives you the calculated **xirr** as tag, which is the internal rate of return of an investment based on a specified series of irregularly spaced cash flows. This value is annual percentage rate following the 30/360US day count convention. It is a good metric to compare the investment return with a benchmark like the S&P or the T-Bill, for example.
 
 > Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
 
 ## Checks
 
-It is recommended to use the option *--check* to ensure you past selling transaction has the correct cost according to the choosen cost method. It can be enabled by setting the environment variable **HLEDGER_LOTS_CHECK** to "true". It can be disabled with the option *--no-check* or setting the environment variable **HLEDGER_LOTS_CHECK** to "false".
-
-> At the moment the default is set to "false", but expect it to be turned to "true" in future releases.
+It is recommended to set the option *check* to true to ensure you past selling transaction has the correct cost according to the choosen cost method. See how to set it up [here](config)
 
 ## Limitations
 
 - No _short-selling_
 - Each commodity can have only one base currency. For example, it is not possible to buy AAPL with USD and later with EUR.
```

### Comparing `hledger_lots-0.3.0/hledger_lots/avg.py` & `hledger_lots-0.4.0/hledger_lots/avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/hledger_lots/avg_info.py` & `hledger_lots-0.4.0/hledger_lots/avg_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     def __init__(
         self,
         journals: Tuple[str, ...],
         commodity: str,
         check: bool,
         no_desc: Optional[str] = None,
     ):
-        super().__init__(journals, commodity)
+        super().__init__(journals, commodity, no_desc)
         self.check = check
         self.avg_lots = get_avg_cost(self.txns, self.check)
         self.table = dt_list2table(self.avg_lots)
 
-    @property
-    def info(self):
+    def get_info(self):
+        if len(self.txns) == 0:
+            return
+
         commodity = self.commodity
         cur = self.txns[0].base_cur
         qtty = self.avg_lots[-1].total_qtty
         amount = self.avg_lots[-1].total_amount
         avg_cost = self.avg_lots[-1].avg_cost
         last_buy_date = datetime.strptime(self.avg_lots[-1].date, "%Y-%m-%d").date()
         xirr = self.get_lots_xirr(last_buy_date)
@@ -55,28 +57,32 @@
             mkt_profit=market_profit_str,
             mkt_date=market_date,
             xirr=xirr_str,
         )
 
     @property
     def info_txt(self):
-        return self.get_info_txt(self.info)
+        info = self.get_info()
+        if not info:
+            return f"No transaction for {self.commodity}"
+
+        return self.get_info_txt(info)
 
 
 class AllAvgInfo(AllInfo):
     def __init__(self, journals: Tuple[str, ...], no_desc: str, check: bool):
         super().__init__(journals, no_desc)
         self.check = check
 
     def get_info(self, commodity: str):
         avg_obj = AvgInfo(self.journals, commodity, self.check)
         if len(avg_obj.txns) == 0:
             return
         else:
-            return avg_obj.info
+            return avg_obj.get_info()
 
     @property
     def infos(self):
         infos = [self.get_info(com) for com in self.commodities]
         infos = [info for info in infos if info]
         return infos
```

### Comparing `hledger_lots-0.3.0/hledger_lots/checks.py` & `hledger_lots-0.4.0/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/hledger_lots/commodity_tag.py` & `hledger_lots-0.4.0/hledger_lots/commodity_tag.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/hledger_lots/fifo.py` & `hledger_lots-0.4.0/hledger_lots/fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/hledger_lots/fifo_info.py` & `hledger_lots-0.4.0/hledger_lots/fifo_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,25 +12,27 @@
     def __init__(
         self,
         journals: Tuple[str, ...],
         commodity: str,
         check: bool,
         no_desc: Optional[str] = None,
     ):
-        super().__init__(journals, commodity)
+        super().__init__(journals, commodity, no_desc)
         self.check = check
 
         self.lots = get_lots(self.txns, check)
         self.last_buy_date = self.lots[-1].date if len(self.lots) > 0 else None
 
         self.buy_lots = get_lots(self.txns, check)
         self.table = dt_list2table(self.buy_lots)
 
-    @property
-    def info(self):
+    def get_info(self):
+        if len(self.txns) == 0:
+            return None
+
         commodity = self.commodity
 
         cur = self.lots[0].base_cur
         qtty = sum(lot.qtty for lot in self.lots)
         amount = sum(lot.price * lot.qtty for lot in self.lots)
         avg_cost = get_avg_fifo(self.lots) if qtty > 0 else 0
 
@@ -68,15 +70,18 @@
             mkt_profit=market_profit_str,
             mkt_date=market_date,
             xirr=xirr_str,
         )
 
     @property
     def info_txt(self):
-        return self.get_info_txt(self.info)
+        info = self.get_info()
+        if not info:
+            return f"No transactions available for {self.commodity}"
+        return self.get_info_txt(info)
 
 
 class AllFifoInfo(AllInfo):
     def __init__(self, journals: Tuple[str, ...], no_desc: str, check: bool):
         super().__init__(journals, no_desc)
         self.check = check
 
@@ -84,15 +89,15 @@
         txns = hledger2txn(self.journals, commodity, self.no_desc)
         try:
             lots = get_lots(txns, self.check)
         except MultipleBaseCurrencies:
             return None
 
         if len(lots) > 0:
-            lot_info = FifoInfo(self.journals, commodity, self.check).info
+            lot_info = FifoInfo(self.journals, commodity, self.check).get_info()
             return lot_info
 
     @property
     def infos(self):
         infos = [self.get_info(com) for com in self.commodities]
         infos = [info for info in infos if info is not None]
         return infos
```

### Comparing `hledger_lots-0.3.0/hledger_lots/hl.py` & `hledger_lots-0.4.0/hledger_lots/hl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import subprocess
 import sys
 from typing import List, Optional, Tuple
 
-from .files import get_files_comm
-from .lib import AdjustedTxn, Txn, get_avg_fifo, get_xirr
+from .lib import AdjustedTxn, Txn, get_avg_fifo, get_files_comm, get_xirr
 
 
 def adjust_txn(txn: Txn) -> AdjustedTxn:
     price = txn.price if txn.type == "UnitPrice" else txn.price / txn.qtty
 
     result = AdjustedTxn(txn.date, price, txn.base_cur, txn.qtty, txn.acct)
     return result
@@ -40,12 +39,12 @@
     txns_list = json.loads(hl_data)
 
     txns = [
         prices_items2txn(txn["tdate"], prices_items, posting_items["paccount"])
         for txn in txns_list
         for posting_items in txn["tpostings"]
         for prices_items in posting_items["pamount"]
-        if prices_items["acommodity"] == cur and prices_items["aprice"]
+        if prices_items["acommodity"].upper() == cur.upper() and prices_items["aprice"]
     ]
 
     adjusted_txns = [adjust_txn(txn) for txn in txns]
     return adjusted_txns
```

### Comparing `hledger_lots-0.3.0/hledger_lots/info.py` & `hledger_lots-0.4.0/hledger_lots/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from io import StringIO
 from typing import List, Optional, Tuple, TypedDict
 
 from tabulate import tabulate
 
-from .files import get_files_comm
 from .hl import hledger2txn
-from .lib import adjust_commodity, get_xirr
+from .lib import adjust_commodity, get_files_comm, get_xirr
 
 
 class LotsInfo(TypedDict):
     comm: str
     cur: str
     qtty: str
     amount: str
@@ -75,15 +74,15 @@
 
 class Info:
     def __init__(
         self, journals: Tuple[str, ...], commodity: str, no_desc: Optional[str] = None
     ) -> None:
         self.journals = journals
         self.files_comm = get_files_comm(journals)
-        self.commodity = commodity
+        self.commodity = commodity.upper()
         self.txns = hledger2txn(journals, commodity, no_desc)
 
         self.has_txn = len(self.txns) > 0
         self.last_price = get_last_price(self.files_comm, commodity)
 
         self.market_date, self.market_price = self.last_price
```

### Comparing `hledger_lots-0.3.0/hledger_lots/lib.py` & `hledger_lots-0.4.0/hledger_lots/lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import re
 import shlex
+import sys
+import tempfile
 from dataclasses import asdict, dataclass
 from datetime import date
-from typing import List, Optional
+from pathlib import Path
+from typing import List, Optional, Tuple
 
-import click
 from pyxirr import DayCount, xirr
 from tabulate import tabulate
 
 
 @dataclass
 class AdjustedTxn:
     date: str
@@ -26,14 +28,42 @@
 
 class CostMethodError(Exception):
     def __init__(self, sell: AdjustedTxn, price: float, base_cur: str) -> None:
         self.message = f"Error in sale {sell}. Correct price should be {price} in currency {base_cur}"
         super().__init__(self.message)
 
 
+def get_file_from_stdin():
+    tmp_file = tempfile.NamedTemporaryFile(suffix=".journal", delete=False)
+    name = tmp_file.name
+
+    with open(tmp_file.name, "w") as f:
+        for line in sys.stdin:
+            f.write(line)
+
+    return name
+
+
+def get_default_file():
+    ledger_file = os.getenv("LEDGER_FILE")
+    if ledger_file:
+        return (ledger_file,)
+
+    default_path = Path.home() / ".hledger.journal"
+    if default_path.exists():
+        return (str(default_path),)
+
+
+def get_files_comm(file_path: Tuple[str, ...]) -> List[str]:
+    files = []
+    for file in file_path:
+        files = [*files, "-f", file]
+    return files
+
+
 def get_avg_fifo(txns: List[AdjustedTxn]):
     total_qtty = sum(txn.qtty for txn in txns)
     if total_qtty == 0:
         return 0
     mult = [txn.qtty * txn.price for txn in txns]
     total_mult = sum(mult)
     avg = total_mult / total_qtty
@@ -71,24 +101,14 @@
 
 def adjust_commodity(comm: str):
     has_non_word = re.search(r"\W", comm)
     adjusted = f'"{comm}"' if has_non_word else comm
     return adjusted
 
 
-def default_fn_bool(env_name: str, default: bool):
-    env = os.environ.get(env_name, None)
-    if env == "true":
-        return True
-    elif env == "False":
-        return False
-    else:
-        return default
-
-
 def get_sell_comm(
     commodity: str,
     no_desc: str,
     commodity_account: str,
     cash_account: str,
     revenue_account: str,
     date: str,
```

### Comparing `hledger_lots-0.3.0/hledger_lots/prices_yahoo.py` & `hledger_lots-0.4.0/hledger_lots/prices_yahoo.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Dict, List, Tuple
 
 import yfinance as yf
 from requests.exceptions import HTTPError
 from requests_cache import CachedSession
 
 from .commodity_tag import CommodityDirective, CommodityTag
-from .files import get_files_comm
 from .hl import hledger2txn
 from .info import get_last_price
+from .lib import get_files_comm
 
 
 @dataclass
 class Price:
     name: str
     date: date
     price: float
@@ -36,28 +36,37 @@
         self.yesterday_str = yesterday.strftime("%Y-%m-%d")
 
         commodity_directive = CommodityDirective(self.files)
         self.commodities = commodity_directive.get_commodity_tag(self.TAG)
 
     def get_start_date(self, commodity: CommodityTag):
         txns = hledger2txn(self.files, commodity["commodity"])
+        qtty = sum(txn.qtty for txn in txns)
+        if qtty == 0:
+            print(
+                f"; stderr: No transaction for {commodity['commodity']}. Not downloading ",
+                file=sys.stderr,
+            )
+            return
+
         first_date_str = txns[0].date
         first_date = datetime.strptime(first_date_str, "%Y-%m-%d").date()
         last_market_date = get_last_price(self.files_comm, commodity["commodity"])[0]
 
         if not last_market_date:
             last_date = first_date
         elif last_market_date < first_date:
             last_date = first_date
         else:
             last_date = last_market_date
 
         start_date = last_date + timedelta(days=1)
         past = date.today() - start_date
         if past.days < 1:
+            print(f"; stderr: No new data for {commodity}", file=sys.stderr)
             return
 
         return start_date
 
     def prices2hledger(self, prices: List[Price]):
         prices_list = [
             f"P {price.date.strftime('%Y-%m-%d')} \"{price.name}\" {price.price} {price.cur}"
@@ -95,15 +104,14 @@
             for row in df.iterrows()
         ]
         return prices
 
     def get_commodity_prices(self, commodity: CommodityTag):
         start_date = self.get_start_date(commodity)
         if not start_date:
-            print(f"; stderr: No new data for {commodity}", file=sys.stderr)
             return
 
         start_date_str = start_date.strftime("%Y-%m-%d")
         try:
             prices = [
                 price for price in self.get_prices(commodity, start_date_str) if price
             ]
```

### Comparing `hledger_lots-0.3.0/hledger_lots/prompt.py` & `hledger_lots-0.4.0/hledger_lots/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import List, Optional, Tuple
 
 import questionary
 from prompt_toolkit.shortcuts import CompleteStyle
 
 from .avg_info import AllAvgInfo
 from .fifo_info import AllFifoInfo
-from .files import get_files_comm
 from .info import LotsInfo
+from .lib import get_files_comm
 
 
 class PromptError(BaseException):
     def __init__(self, message: str) -> None:
         self.message = message
         super().__init__(self.message)
 
@@ -133,15 +133,19 @@
         self.avg_cost = avg_cost
 
         self.files_comm = get_files_comm(file)
         self.infos = self.get_infos()
         self.commodities = [info["comm"] for info in self.get_infos()]
 
     def run_hledger(self, *comm: str):
-        command = ["hledger", *self.files_comm, *comm, f"not:desc:{self.no_desc}"]
+        command = ["hledger", *self.files_comm, *comm]
+
+        if self.no_desc and self.no_desc != "":
+            command = [*command, f"not:desc:{self.no_desc}"]
+
         proc = subprocess.run(command, capture_output=True)
         if proc.returncode != 0:
             raise subprocess.SubprocessError(proc.stderr.decode("utf8"))
 
         result = proc.stdout.decode("utf8")
         return result
```

### Comparing `hledger_lots-0.3.0/hledger_lots/prompt_buy.py` & `hledger_lots-0.4.0/hledger_lots/prompt_buy.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/hledger_lots/prompt_sell.py` & `hledger_lots-0.4.0/hledger_lots/prompt_sell.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/hledger_lots.egg-info/PKG-INFO` & `hledger_lots-0.4.0/hledger_lots.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-lots
-Version: 0.3.0
+Version: 0.4.0
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -52,36 +52,39 @@
 The indicators provided by these command are explained [here](#indicators).
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
 
-## Installation
+## Setup
 
 ### Requirements
 
 - [python](https://www.python.org/)
 - [hledger](https://hledger.org/1.29/hledger.html#p-directive)
 
-### Command
+### Install
 
 ```python
 pip install --upgrade hledger-lots
 ```
 
-## Workflow
+### Config
 
-1. Add purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
-2. Download market price history as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
-3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
-4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
+Instead of using command options, which is hard to remember and makes the command long, environment variables, which demands tweaking the .bashrc file or a configuration file, this app add configuration options directly in the journal using a custom directives specification explained [here](config)
+
+> You can still use **LEDGER_FILE** environment variable by adding `export LEDGER_FILE=your_data.journal` or prepend to the command: `LEDGER_FILE=your_data.journal hledger-lots ...`
 
-> By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
+## Workflow
 
+1. Add a commodity purchase using the command [buy](usage/#hledger-lots-buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See some examples [here](examples/data.journal)
+2. Download market price history from [Yahoo Finance](https://finance.yahoo.com/) as [price directive](https://hledger.org/1.29/hledger.html#p-directive) using the command [prices](usage/#hledger-lots-prices)
+3. View financial indicators for a specific commodity using [view](usage/#hledger-lots-view) or a summary of all commodities using [list](usage/$list).
+4. When you sell, use the command [sell](usage/#hledger-lots-sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
@@ -102,15 +105,13 @@
 
 The sale transaction gives you the calculated **xirr** as tag, which is the internal rate of return of an investment based on a specified series of irregularly spaced cash flows. This value is annual percentage rate following the 30/360US day count convention. It is a good metric to compare the investment return with a benchmark like the S&P or the T-Bill, for example.
 
 > Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
 
 ## Checks
 
-It is recommended to use the option *--check* to ensure you past selling transaction has the correct cost according to the choosen cost method. It can be enabled by setting the environment variable **HLEDGER_LOTS_CHECK** to "true". It can be disabled with the option *--no-check* or setting the environment variable **HLEDGER_LOTS_CHECK** to "false".
-
-> At the moment the default is set to "false", but expect it to be turned to "true" in future releases.
+It is recommended to set the option *check* to true to ensure you past selling transaction has the correct cost according to the choosen cost method. See how to set it up [here](config)
 
 ## Limitations
 
 - No _short-selling_
 - Each commodity can have only one base currency. For example, it is not possible to buy AAPL with USD and later with EUR.
```

### Comparing `hledger_lots-0.3.0/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.4.0/hledger_lots.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 hledger_lots/commodity_tag.py
 hledger_lots/fifo.py
 hledger_lots/fifo_info.py
 hledger_lots/files.py
 hledger_lots/hl.py
 hledger_lots/info.py
 hledger_lots/lib.py
+hledger_lots/options.py
 hledger_lots/prices_yahoo.py
 hledger_lots/prompt.py
 hledger_lots/prompt_buy.py
 hledger_lots/prompt_sell.py
 hledger_lots.egg-info/PKG-INFO
 hledger_lots.egg-info/SOURCES.txt
 hledger_lots.egg-info/dependency_links.txt
```

### Comparing `hledger_lots-0.3.0/pyproject.toml` & `hledger_lots-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.3.0"
+version = "0.4.0"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
```

### Comparing `hledger_lots-0.3.0/tests/lots_data.py` & `hledger_lots-0.4.0/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/tests/test_avg.py` & `hledger_lots-0.4.0/tests/test_avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/tests/test_checks.py` & `hledger_lots-0.4.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/tests/test_fifo.py` & `hledger_lots-0.4.0/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/tests/test_hl.py` & `hledger_lots-0.4.0/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/tests/test_info.py` & `hledger_lots-0.4.0/tests/test_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,13 +105,13 @@
             "mkt_price": "6.0000",
             "mkt_amount": "36.00",
             "mkt_profit": "4.80",
             "mkt_date": "2023-02-01",
             "xirr": "6.2529%",
         }
     def test_fifo_info(self, fifo_info: FifoInfo):
-        assert fifo_info.info == self.expected
+        assert fifo_info.get_info() == self.expected
 
     def test_avg_info(self, avg_info: AvgInfo):
-        assert avg_info.info == self.expected
+        assert avg_info.get_info() == self.expected
```

### Comparing `hledger_lots-0.3.0/tests/test_lib.py` & `hledger_lots-0.4.0/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2html.py` & `hledger_lots-0.4.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2html4.py` & `hledger_lots-0.4.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2html5.py` & `hledger_lots-0.4.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2latex.py` & `hledger_lots-0.4.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2man.py` & `hledger_lots-0.4.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2odt.py` & `hledger_lots-0.4.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.4.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.4.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2s5.py` & `hledger_lots-0.4.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2xetex.py` & `hledger_lots-0.4.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rst2xml.py` & `hledger_lots-0.4.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.3.0/venv/bin/rstpep2html.py` & `hledger_lots-0.4.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

