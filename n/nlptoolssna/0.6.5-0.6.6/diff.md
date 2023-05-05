# Comparing `tmp/nlptoolssna-0.6.5.tar.gz` & `tmp/nlptoolssna-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.6.5.tar", last modified: Fri May  5 21:24:38 2023, max compression
+gzip compressed data, was "nlptoolssna-0.6.6.tar", last modified: Fri May  5 21:29:15 2023, max compression
```

## Comparing `nlptoolssna-0.6.5.tar` & `nlptoolssna-0.6.6.tar`

### file list

```diff
@@ -1,81 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.297800 nlptoolssna-0.6.5/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-05 21:24:38.298818 nlptoolssna-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.174868 nlptoolssna-0.6.5/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.6.5/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.133615 nlptoolssna-0.6.5/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.135566 nlptoolssna-0.6.5/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.177077 nlptoolssna-0.6.5/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.5/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.186974 nlptoolssna-0.6.5/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.5/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.6.5/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.5/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.5/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.6.5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.202589 nlptoolssna-0.6.5/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.204541 nlptoolssna-0.6.5/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.5/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.213333 nlptoolssna-0.6.5/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.215374 nlptoolssna-0.6.5/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.6.5/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.6.5/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.218234 nlptoolssna-0.6.5/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.6.5/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.6.5/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.225058 nlptoolssna-0.6.5/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.6.5/docs/source/api/utils/implication.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.227992 nlptoolssna-0.6.5/docs/source/api/utils/jaccard/
--rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.6.5/docs/source/api/utils/jaccard/jaccardFunction.rst
--rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.6.5/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.6.5/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.6.5/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.6.5/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.6.5/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.6.5/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.6.5/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.6.5/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.235793 nlptoolssna-0.6.5/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.239697 nlptoolssna-0.6.5/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.6.5/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.6.5/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.255396 nlptoolssna-0.6.5/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.6.5/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.6.5/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.6.5/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.6.5/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.6.5/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.6.5/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.258266 nlptoolssna-0.6.5/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.6.5/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.270430 nlptoolssna-0.6.5/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.6.5/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.6.5/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     7950 2023-05-04 20:21:37.000000 nlptoolssna-0.6.5/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.6.5/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.6.5/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.274730 nlptoolssna-0.6.5/nlptools/tools/
--rw-rw-rw-   0        0        0        0 2023-05-05 21:18:08.000000 nlptoolssna-0.6.5/nlptools/tools/__init__.py
--rw-rw-rw-   0        0        0     9326 2023-05-05 21:18:44.000000 nlptoolssna-0.6.5/nlptools/tools/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.291947 nlptoolssna-0.6.5/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-05 21:24:37.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1642 2023-05-05 21:24:38.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 21:24:37.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-05 21:24:37.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-05 21:24:37.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 21:24:37.000000 nlptoolssna-0.6.5/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-05 21:24:38.300776 nlptoolssna-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 21:24:38.296826 nlptoolssna-0.6.5/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.6.5/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.470716 nlptoolssna-0.6.6/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-05 21:29:15.470716 nlptoolssna-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.357340 nlptoolssna-0.6.6/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.6.6/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.311746 nlptoolssna-0.6.6/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.313664 nlptoolssna-0.6.6/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.359365 nlptoolssna-0.6.6/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.6/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.367142 nlptoolssna-0.6.6/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.6/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.6.6/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.6/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.6.6/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.6.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.378861 nlptoolssna-0.6.6/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.380811 nlptoolssna-0.6.6/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.6.6/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.387649 nlptoolssna-0.6.6/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.389664 nlptoolssna-0.6.6/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.6.6/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.6.6/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.391555 nlptoolssna-0.6.6/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.6.6/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.6.6/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.397456 nlptoolssna-0.6.6/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.6.6/docs/source/api/utils/implication.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.399369 nlptoolssna-0.6.6/docs/source/api/utils/jaccard/
+-rw-rw-rw-   0        0        0      150 2023-05-04 19:29:01.000000 nlptoolssna-0.6.6/docs/source/api/utils/jaccard/jaccardFunction.rst
+-rw-rw-rw-   0        0        0      235 2023-05-04 19:55:02.000000 nlptoolssna-0.6.6/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.6.6/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      240 2023-05-04 19:54:12.000000 nlptoolssna-0.6.6/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      180 2023-05-04 19:55:43.000000 nlptoolssna-0.6.6/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.6.6/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.6.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-04 19:59:32.000000 nlptoolssna-0.6.6/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.6.6/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.405224 nlptoolssna-0.6.6/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.409220 nlptoolssna-0.6.6/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.6.6/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4027 2023-05-02 17:30:35.000000 nlptoolssna-0.6.6/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.421849 nlptoolssna-0.6.6/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.6.6/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.6.6/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.6.6/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.6.6/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.6.6/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.6.6/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.423786 nlptoolssna-0.6.6/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.6.6/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.433544 nlptoolssna-0.6.6/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.6.6/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.6.6/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     5305 2023-05-05 21:28:54.000000 nlptoolssna-0.6.6/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.6.6/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-02 13:53:43.000000 nlptoolssna-0.6.6/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.440393 nlptoolssna-0.6.6/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.6.6/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0    20588 2023-05-04 20:28:19.000000 nlptoolssna-0.6.6/nlptools/parse/implication.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.445260 nlptoolssna-0.6.6/nlptools/parse/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.6.6/nlptools/parse/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-05-05 21:27:38.000000 nlptoolssna-0.6.6/nlptools/parse/jaccard/jaccardFunction.py
+-rw-rw-rw-   0        0        0     9326 2023-05-04 19:41:34.000000 nlptoolssna-0.6.6/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.449012 nlptoolssna-0.6.6/nlptools/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-05 21:18:08.000000 nlptoolssna-0.6.6/nlptools/tools/__init__.py
+-rw-rw-rw-   0        0        0     9326 2023-05-05 21:18:44.000000 nlptoolssna-0.6.6/nlptools/tools/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.464677 nlptoolssna-0.6.6/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1801 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 21:29:15.000000 nlptoolssna-0.6.6/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-05 21:29:15.472749 nlptoolssna-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     2097 2023-05-04 15:44:31.000000 nlptoolssna-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:29:15.469754 nlptoolssna-0.6.6/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.6.6/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.6.5/CONTRIBUTING.rst` & `nlptoolssna-0.6.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/LICENSE` & `nlptoolssna-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/PKG-INFO` & `nlptoolssna-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.6.5/README.rst` & `nlptoolssna-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/Makefile` & `nlptoolssna-0.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/build/html/_images/download.png` & `nlptoolssna-0.6.6/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/build/html/_static/download.png` & `nlptoolssna-0.6.6/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/make.bat` & `nlptoolssna-0.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/source/_static/download.png` & `nlptoolssna-0.6.6/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/source/conf.py` & `nlptoolssna-0.6.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/docs/source/installation.rst` & `nlptoolssna-0.6.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.6.6/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/arabiner/data.py` & `nlptoolssna-0.6.6/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/arabiner/datasets.py` & `nlptoolssna-0.6.6/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/arabiner/helpers.py` & `nlptoolssna-0.6.6/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/arabiner/infer.py` & `nlptoolssna-0.6.6/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/arabiner/transforms.py` & `nlptoolssna-0.6.6/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/data/my_data.pickle` & `nlptoolssna-0.6.6/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/morphology/charsets.py` & `nlptoolssna-0.6.6/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.6.6/nlptools/morphology/morph_analyzer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-import pickle
+
 from nlptools.morphology import settings 
 import re
 from nlptools.morphology.tokenizers_words import simple_word_tokenize
-from nlptools.utils.parser import arStrip
-import os.path
+from nlptools.parse.parser import arStrip
 from nlptools.DataDownload import downloader
 from nlptools.morphology.charsets import AR_CHARSET, AR_DIAC_CHARSET
 import copy
-# def load_ALMA_dic():
-#    # Open the Pickle file in binary mode
-#     filename = 'ALMA27012000.pickle'
-#     path =downloader.get_appdatadir()
-#     file_path = os.path.join(path, filename)
-    
 
-#     with open(file_path, 'rb') as f:
-#        #Load the serialized data from the file
-#        ALMA_dic = pickle.load(f)
-#        #print(ALMA_dic)
-#        return ALMA_dic
 _IS_AR_RE = re.compile(u'^[' + re.escape(u''.join(AR_CHARSET)) + u']+$')
 def find_solution(token, language, task):
     """
     Given a token, this method finds the morphological solution lemma and/or pos based on a spesific language and task.
           
     Args:
         - token (:obj:`str`): The Arabic token to be morphologcaly analyzed.
@@ -128,102 +116,27 @@
     elif task == 'pos':
         return remove_items_by_index(lst, [1])
     else: 
         return lst
 
 
 def remove_items_by_index(lst, index_list):
-    out_put_list= copy.deepcopy(lst)
-    for inner_list in out_put_list:
+
+    for inner_list in index_list:
         for index in sorted(index_list, reverse=True):
             if len(inner_list) > index:
                 inner_list.pop(index)
-    return out_put_list
+    return index_list
 
 
 def _is_ar(word):
     return _IS_AR_RE.match(word) is not None       
         
-# def tagger(text: str, task = 'full', language = 'MSA'):
-
-#     """
-#     This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
-#     There is no limit for the text size, but one should be resonable based on the available resources (computational power).
-    
-#         Args:
-#             - text (:obj:`str`): The input Arabic text to be morphologically analyzed and tagged.
-#             - task (:obj:`str`): The type of morphological analysis and tagging to be performed (the default is `full`).
-#             - language (:obj:`str`): The language of the input text (the default is 'MSA' (Modern Standard Arabic)).
-        
-#     Returns:
-#            - output_list list(:obj:`list`): A list of lists, where each sublist contains information about a token in the input text, including the original token, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
-
-#     **Example:**
-
-#     .. highlight:: python
-#     .. code-block:: python
-
-#          from nlptools.morph import morph_tagger
-      
-#          # Return the morpological solution for each token in this text
-#          morph_tagger.tagger('ذهب الولد الى المدرسة')
-
-#          # the output
-#             [['ذهب', 'فعل', 349890, 'MSA', 'lemmatizer'],
-#             ['الولد', 'اسم', 320244, 'MSA', 'lemmatizer'],
-#             ['الى', 'كلمة وظيفية', 20215999, 'MSA', 'lemmatizer'],
-#             ['المدرسة', 'اسم', 561184, 'MSA', 'lemmatizer']]
-#     """
-    
-#     # Check if the ALMA dictionary has been loaded
-#     if settings.flag == True:
-#         settings.flag = False
-#         settings.div_dic = load_ALMA_dic()
-   
-    
-#     # Perform morphological tagging for the input text
-#     output_list = morph_tagger(text,language, task)
-    
-#     # Return a list of morphological solution for each token in the input text
-#     return output_list
 
   
   
   
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-  
-
```

### Comparing `nlptoolssna-0.6.5/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.6.6/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptools/tools/parser.py` & `nlptoolssna-0.6.6/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.6.6/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.6.5/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.6.6/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 nlptools/arabiner/transforms.py
 nlptools/data/my_data.pickle
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
+nlptools/parse/__init__.py
+nlptools/parse/implication.py
+nlptools/parse/parser.py
+nlptools/parse/jaccard/__init__.py
+nlptools/parse/jaccard/jaccardFunction.py
 nlptools/tools/__init__.py
 nlptools/tools/parser.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
```

### Comparing `nlptoolssna-0.6.5/setup.cfg` & `nlptoolssna-0.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.6.5/setup.py` & `nlptoolssna-0.6.6/setup.py`

 * *Files identical despite different names*

