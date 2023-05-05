# Comparing `tmp/vvvvid_downloader-1.3.2.tar.gz` & `tmp/vvvvid_downloader-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvvvid_downloader-1.3.2.tar", last modified: Thu Apr 27 15:39:53 2023, max compression
+gzip compressed data, was "vvvvid_downloader-1.3.3.tar", last modified: Fri May  5 08:11:52 2023, max compression
```

## Comparing `vvvvid_downloader-1.3.2.tar` & `vvvvid_downloader-1.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      147 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/.editorconfig
--rw-r--r--   0        0        0       73 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/.gitattributes
--rw-r--r--   0        0        0     2064 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/.gitignore
--rw-r--r--   0        0        0     1198 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      243 2023-04-27 14:44:52.806456 vvvvid_downloader-1.3.2/Pipfile
--rw-r--r--   0        0        0    26600 2023-04-27 14:45:26.766698 vvvvid_downloader-1.3.2/Pipfile.lock
--rw-r--r--   0        0        0      978 2023-04-27 14:44:09.270044 vvvvid_downloader-1.3.2/README.md
--rw-r--r--   0        0        0     1211 2023-04-27 14:44:09.270044 vvvvid_downloader-1.3.2/UNLICENSE
--rw-r--r--   0        0        0      663 2023-04-27 15:37:54.210365 vvvvid_downloader-1.3.2/pyproject.toml
--rw-r--r--   0        0        0       77 2023-04-27 15:36:29.529395 vvvvid_downloader-1.3.2/vvvvid_downloader/__init__.py
--rw-r--r--   0        0        0     4180 2023-04-27 14:53:50.208970 vvvvid_downloader-1.3.2/vvvvid_downloader/__main__.py
--rw-r--r--   0        0        0     1852 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.2/vvvvid_downloader/api.py
--rw-r--r--   0        0        0        0 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.2/vvvvid_downloader/py.typed
--rw-r--r--   0        0        0     9663 2023-04-27 15:09:03.413557 vvvvid_downloader-1.3.2/vvvvid_downloader/responses.py
--rw-r--r--   0        0        0     1308 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.2/vvvvid_downloader/vvvvid.py
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 vvvvid_downloader-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      147 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.3/.editorconfig
+-rw-r--r--   0        0        0       73 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.3/.gitattributes
+-rw-r--r--   0        0        0     2064 2023-04-27 14:44:09.269045 vvvvid_downloader-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1367 2023-05-05 08:09:48.034215 vvvvid_downloader-1.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0      243 2023-04-27 14:44:52.806456 vvvvid_downloader-1.3.3/Pipfile
+-rw-r--r--   0        0        0    26600 2023-04-27 14:45:26.766698 vvvvid_downloader-1.3.3/Pipfile.lock
+-rw-r--r--   0        0        0      978 2023-04-27 14:44:09.270044 vvvvid_downloader-1.3.3/README.md
+-rw-r--r--   0        0        0     1211 2023-04-27 14:44:09.270044 vvvvid_downloader-1.3.3/UNLICENSE
+-rw-r--r--   0        0        0      663 2023-04-27 15:37:54.210365 vvvvid_downloader-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-05 08:09:52.951216 vvvvid_downloader-1.3.3/vvvvid_downloader/__init__.py
+-rw-r--r--   0        0        0     4172 2023-05-05 08:09:33.091996 vvvvid_downloader-1.3.3/vvvvid_downloader/__main__.py
+-rw-r--r--   0        0        0     1852 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.3/vvvvid_downloader/api.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.3/vvvvid_downloader/py.typed
+-rw-r--r--   0        0        0     9663 2023-04-27 15:09:03.413557 vvvvid_downloader-1.3.3/vvvvid_downloader/responses.py
+-rw-r--r--   0        0        0     1308 2023-04-27 14:44:09.271044 vvvvid_downloader-1.3.3/vvvvid_downloader/vvvvid.py
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 vvvvid_downloader-1.3.3/PKG-INFO
```

### Comparing `vvvvid_downloader-1.3.2/.gitignore` & `vvvvid_downloader-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/CHANGELOG.md` & `vvvvid_downloader-1.3.3/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.3.3] - 2023-05-05
+
+- fix: download the right episodes when downloading the whole season
+
+## [1.3.2] - 2023-04-27
+
+- feat: Aggiunto supporto per video/dash format
+
 ## [1.3.1] - 2022-01-04
 
 - (Fix) Aggiornate le dipendenze necessarie per far funzionare correttamente lo script.
 
 ## [1.3.0] - 2022-01-03
 
 - Rimosso il file di configurazione persistente.
```

### Comparing `vvvvid_downloader-1.3.2/Pipfile.lock` & `vvvvid_downloader-1.3.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/README.md` & `vvvvid_downloader-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/UNLICENSE` & `vvvvid_downloader-1.3.3/UNLICENSE`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/pyproject.toml` & `vvvvid_downloader-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/vvvvid_downloader/__main__.py` & `vvvvid_downloader-1.3.3/vvvvid_downloader/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             season = [i for index, i in enumerate(season, 1) if index in answer]
 
     i: SeasonObject
     for i in track(season, "Scarico..."):
         show_title = i.show_title
         episode_number = i.number
 
-        embed_code = getattr(season[0], quality_code, "")
+        embed_code = getattr(i, quality_code, "")
         output_dir = Path().joinpath("vvvvid", show_title)
         output_name = re_sub(r"\s", "_", f"{show_title}_Ep_{episode_number}_{quality}")
 
         log.info(f"Scarico episodio #{episode_number}...")
 
         response = i.download(embed_code, output_dir, output_name)
```

### Comparing `vvvvid_downloader-1.3.2/vvvvid_downloader/api.py` & `vvvvid_downloader-1.3.3/vvvvid_downloader/api.py`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/vvvvid_downloader/responses.py` & `vvvvid_downloader-1.3.3/vvvvid_downloader/responses.py`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/vvvvid_downloader/vvvvid.py` & `vvvvid_downloader-1.3.3/vvvvid_downloader/vvvvid.py`

 * *Files identical despite different names*

### Comparing `vvvvid_downloader-1.3.2/PKG-INFO` & `vvvvid_downloader-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vvvvid_downloader
-Version: 1.3.2
+Version: 1.3.3
 Summary: Uno script in Python per scaricare da VVVVID. 
 Home-page: https://github.com/nearata/vvvvid-downloader
 Author: Nearata
 Author-email: nearata@protonmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

