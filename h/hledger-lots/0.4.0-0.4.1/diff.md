# Comparing `tmp/hledger_lots-0.4.0.tar.gz` & `tmp/hledger_lots-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.4.0.tar", last modified: Fri May  5 17:38:54 2023, max compression
+gzip compressed data, was "hledger_lots-0.4.1.tar", last modified: Fri May  5 17:46:41 2023, max compression
```

## Comparing `hledger_lots-0.4.0.tar` & `hledger_lots-0.4.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.982166 hledger_lots-0.4.0/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5711 2023-05-05 17:38:54.982166 hledger_lots-0.4.0/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.971166 hledger_lots-0.4.0/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5371 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.975165 hledger_lots-0.4.0/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       95 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2882 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7839 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1589 2023-05-03 16:08:12.000000 hledger_lots-0.4.0/hledger_lots/commodity_tag.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3423 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1707 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4267 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3231 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/lib.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/hledger_lots/options.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4404 2023-05-05 17:38:44.000000 hledger_lots-0.4.0/hledger_lots/prices_yahoo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7421 2023-05-05 17:38:45.000000 hledger_lots-0.4.0/hledger_lots/prompt.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/hledger_lots/prompt_buy.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/hledger_lots/prompt_sell.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.976166 hledger_lots-0.4.0/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5711 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1135 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-05-05 17:38:54.000000 hledger_lots-0.4.0/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-05-05 17:37:51.000000 hledger_lots-0.4.0/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-05 17:38:54.982166 hledger_lots-0.4.0/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.978165 hledger_lots-0.4.0/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.4.0/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.4.0/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3080 2023-05-05 16:33:52.000000 hledger_lots-0.4.0/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.4.0/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.971166 hledger_lots-0.4.0/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:38:54.981166 hledger_lots-0.4.0/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.4.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.516516 hledger_lots-0.4.1/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5711 2023-05-05 17:46:41.516516 hledger_lots-0.4.1/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.507516 hledger_lots-0.4.1/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5371 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.511515 hledger_lots-0.4.1/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       95 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.4.1/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2882 2023-05-05 17:43:35.000000 hledger_lots-0.4.1/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7839 2023-05-05 17:43:35.000000 hledger_lots-0.4.1/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1589 2023-05-03 16:08:12.000000 hledger_lots-0.4.1/hledger_lots/commodity_tag.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.4.1/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3423 2023-05-05 17:43:35.000000 hledger_lots-0.4.1/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1707 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4267 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3231 2023-05-05 17:43:35.000000 hledger_lots-0.4.1/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/hledger_lots/options.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4404 2023-05-05 17:43:35.000000 hledger_lots-0.4.1/hledger_lots/prices_yahoo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7421 2023-05-05 17:43:35.000000 hledger_lots-0.4.1/hledger_lots/prompt.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.4.1/hledger_lots/prompt_buy.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.4.1/hledger_lots/prompt_sell.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.512515 hledger_lots-0.4.1/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5711 2023-05-05 17:46:41.000000 hledger_lots-0.4.1/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1135 2023-05-05 17:46:41.000000 hledger_lots-0.4.1/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-05 17:46:41.000000 hledger_lots-0.4.1/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-05 17:46:41.000000 hledger_lots-0.4.1/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-05-05 17:46:41.000000 hledger_lots-0.4.1/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-05-05 17:46:41.000000 hledger_lots-0.4.1/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-05-05 17:45:45.000000 hledger_lots-0.4.1/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-05 17:46:41.516516 hledger_lots-0.4.1/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.514515 hledger_lots-0.4.1/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.4.1/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.4.1/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.4.1/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.4.1/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3080 2023-05-05 16:33:52.000000 hledger_lots-0.4.1/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.4.1/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.507516 hledger_lots-0.4.1/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-05 17:46:41.516516 hledger_lots-0.4.1/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.4.1/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.4.0/PKG-INFO` & `hledger_lots-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_lots
-Version: 0.4.0
+Version: 0.4.1
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hledger_lots-0.4.0/docs/README.md` & `hledger_lots-0.4.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/avg.py` & `hledger_lots-0.4.1/hledger_lots/avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/avg_info.py` & `hledger_lots-0.4.1/hledger_lots/avg_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/checks.py` & `hledger_lots-0.4.1/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/cli.py` & `hledger_lots-0.4.1/hledger_lots/cli.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/commodity_tag.py` & `hledger_lots-0.4.1/hledger_lots/commodity_tag.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/fifo.py` & `hledger_lots-0.4.1/hledger_lots/fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/fifo_info.py` & `hledger_lots-0.4.1/hledger_lots/fifo_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/hl.py` & `hledger_lots-0.4.1/hledger_lots/hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/info.py` & `hledger_lots-0.4.1/hledger_lots/info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/lib.py` & `hledger_lots-0.4.1/hledger_lots/lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/options.py` & `hledger_lots-0.4.1/hledger_lots/options.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/prices_yahoo.py` & `hledger_lots-0.4.1/hledger_lots/prices_yahoo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/prompt.py` & `hledger_lots-0.4.1/hledger_lots/prompt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/prompt_buy.py` & `hledger_lots-0.4.1/hledger_lots/prompt_buy.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots/prompt_sell.py` & `hledger_lots-0.4.1/hledger_lots/prompt_sell.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/hledger_lots.egg-info/PKG-INFO` & `hledger_lots-0.4.1/hledger_lots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-lots
-Version: 0.4.0
+Version: 0.4.1
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hledger_lots-0.4.0/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.4.1/hledger_lots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/pyproject.toml` & `hledger_lots-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.4.0"
+version = "0.4.1"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
```

### Comparing `hledger_lots-0.4.0/tests/lots_data.py` & `hledger_lots-0.4.1/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/tests/test_avg.py` & `hledger_lots-0.4.1/tests/test_avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/tests/test_checks.py` & `hledger_lots-0.4.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/tests/test_fifo.py` & `hledger_lots-0.4.1/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/tests/test_hl.py` & `hledger_lots-0.4.1/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/tests/test_info.py` & `hledger_lots-0.4.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/tests/test_lib.py` & `hledger_lots-0.4.1/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2html.py` & `hledger_lots-0.4.1/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2html4.py` & `hledger_lots-0.4.1/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2html5.py` & `hledger_lots-0.4.1/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2latex.py` & `hledger_lots-0.4.1/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2man.py` & `hledger_lots-0.4.1/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2odt.py` & `hledger_lots-0.4.1/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.4.1/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.4.1/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2s5.py` & `hledger_lots-0.4.1/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2xetex.py` & `hledger_lots-0.4.1/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rst2xml.py` & `hledger_lots-0.4.1/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.4.0/venv/bin/rstpep2html.py` & `hledger_lots-0.4.1/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

