# Comparing `tmp/nlptoolssna-0.6.0.tar.gz` & `tmp/nlptoolssna-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.6.0.tar", last modified: Thu May  4 20:22:50 2023, max compression
+gzip compressed data, was "nlptoolssna-0.6.1.tar", last modified: Fri May  5 21:06:16 2023, max compression
```

## Comparing `nlptoolssna-0.6.0.tar` & `nlptoolssna-0.6.1.tar`

### file list

```diff
@@ -1,85 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.877013 nlptoolssna-0.6.0/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-04 20:22:50.877013 nlptoolssna-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.789021 nlptoolssna-0.6.0/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.6.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.753902 nlptoolssna-0.6.0/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.755503 nlptoolssna-0.6.0/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.789997 nlptoolssna-0.6.0/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.0/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.796842 nlptoolssna-0.6.0/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.0/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.6.0/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.0/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.0/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.6.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.809690 nlptoolssna-0.6.0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.811622 nlptoolssna-0.6.0/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.0/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.817780 nlptoolssna-0.6.0/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.818756 nlptoolssna-0.6.0/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.6.0/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.6.0/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.820712 nlptoolssna-0.6.0/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.6.0/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.6.0/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.824615 nlptoolssna-0.6.0/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.6.0/docs/source/api/utils/implication.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.826617 nlptoolssna-0.6.0/docs/source/api/utils/jaccard/
--rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.6.0/docs/source/api/utils/jaccard/jaccardFunction.rst
--rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.6.0/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.6.0/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.6.0/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.6.0/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.6.0/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.6.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.6.0/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.6.0/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.831502 nlptoolssna-0.6.0/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.833980 nlptoolssna-0.6.0/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.6.0/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.6.0/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.842326 nlptoolssna-0.6.0/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.6.0/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.6.0/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.6.0/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.6.0/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.6.0/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.6.0/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.844267 nlptoolssna-0.6.0/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.6.0/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.852604 nlptoolssna-0.6.0/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.6.0/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.6.0/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     7950 2023-05-04 20:21:37.000000 nlptoolssna-0.6.0/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.6.0/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.6.0/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.856505 nlptoolssna-0.6.0/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.6.0/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    20611 2023-05-04 16:11:55.000000 nlptoolssna-0.6.0/nlptools/utils/implication.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.860410 nlptoolssna-0.6.0/nlptools/utils/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.6.0/nlptools/utils/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-05-04 20:21:33.000000 nlptoolssna-0.6.0/nlptools/utils/jaccard/jaccardFunction.py
--rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.6.0/nlptools/utils/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.872128 nlptoolssna-0.6.0/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-04 20:22:50.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1749 2023-05-04 20:22:50.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:22:50.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-04 20:22:50.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-04 20:22:50.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 20:22:50.000000 nlptoolssna-0.6.0/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-04 20:22:50.877990 nlptoolssna-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:22:50.874079 nlptoolssna-0.6.0/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.6.0/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.821108 nlptoolssna-0.6.1/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-05 21:06:16.821108 nlptoolssna-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.698488 nlptoolssna-0.6.1/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.6.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.648806 nlptoolssna-0.6.1/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.650763 nlptoolssna-0.6.1/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.701389 nlptoolssna-0.6.1/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.1/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.711170 nlptoolssna-0.6.1/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.1/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.6.1/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.1/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.1/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.6.1/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.726201 nlptoolssna-0.6.1/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.728175 nlptoolssna-0.6.1/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.1/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.734990 nlptoolssna-0.6.1/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.737978 nlptoolssna-0.6.1/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.6.1/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.6.1/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.739868 nlptoolssna-0.6.1/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.6.1/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.6.1/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.747679 nlptoolssna-0.6.1/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.6.1/docs/source/api/utils/implication.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.749635 nlptoolssna-0.6.1/docs/source/api/utils/jaccard/
+-rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.6.1/docs/source/api/utils/jaccard/jaccardFunction.rst
+-rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.6.1/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.6.1/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.6.1/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.6.1/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.6.1/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.6.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.6.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.6.1/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.756471 nlptoolssna-0.6.1/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.760399 nlptoolssna-0.6.1/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.6.1/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.6.1/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.775026 nlptoolssna-0.6.1/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.6.1/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.6.1/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.6.1/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.6.1/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.6.1/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.6.1/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.778009 nlptoolssna-0.6.1/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.6.1/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.790805 nlptoolssna-0.6.1/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.6.1/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.6.1/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     7950 2023-05-04 20:21:37.000000 nlptoolssna-0.6.1/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.6.1/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.6.1/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.795741 nlptoolssna-0.6.1/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-05 21:03:30.000000 nlptoolssna-0.6.1/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0     9326 2023-05-05 21:03:18.000000 nlptoolssna-0.6.1/nlptools/utils/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.814235 nlptoolssna-0.6.1/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-05 21:06:16.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1642 2023-05-05 21:06:16.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 21:06:16.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-05 21:06:16.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-05 21:06:16.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 21:06:16.000000 nlptoolssna-0.6.1/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-05 21:06:16.822047 nlptoolssna-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:06:16.818142 nlptoolssna-0.6.1/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.6.1/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.6.0/CONTRIBUTING.rst` & `nlptoolssna-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/LICENSE` & `nlptoolssna-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/PKG-INFO` & `nlptoolssna-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.6.0/README.rst` & `nlptoolssna-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/Makefile` & `nlptoolssna-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/build/html/_images/download.png` & `nlptoolssna-0.6.1/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/build/html/_static/download.png` & `nlptoolssna-0.6.1/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/make.bat` & `nlptoolssna-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/source/_static/download.png` & `nlptoolssna-0.6.1/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/source/conf.py` & `nlptoolssna-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/docs/source/installation.rst` & `nlptoolssna-0.6.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.6.1/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/arabiner/data.py` & `nlptoolssna-0.6.1/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/arabiner/datasets.py` & `nlptoolssna-0.6.1/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/arabiner/helpers.py` & `nlptoolssna-0.6.1/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/arabiner/infer.py` & `nlptoolssna-0.6.1/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/arabiner/transforms.py` & `nlptoolssna-0.6.1/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/data/my_data.pickle` & `nlptoolssna-0.6.1/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/morphology/charsets.py` & `nlptoolssna-0.6.1/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.6.1/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.6.1/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptools/utils/parser.py` & `nlptoolssna-0.6.1/nlptools/utils/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.6.1/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.6.0/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.6.1/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -43,18 +43,15 @@
 nlptools/data/my_data.pickle
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
 nlptools/utils/__init__.py
-nlptools/utils/implication.py
 nlptools/utils/parser.py
-nlptools/utils/jaccard/__init__.py
-nlptools/utils/jaccard/jaccardFunction.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
 nlptoolssna.egg-info/requires.txt
 nlptoolssna.egg-info/top_level.txt
```

### Comparing `nlptoolssna-0.6.0/setup.cfg` & `nlptoolssna-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.0/setup.py` & `nlptoolssna-0.6.1/setup.py`

 * *Files identical despite different names*

