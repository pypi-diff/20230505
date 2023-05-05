# Comparing `tmp/linkedinpdfextractor-1.1.1.tar.gz` & `tmp/linkedinpdfextractor-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedinpdfextractor-1.1.1.tar", last modified: Mon Apr 24 07:59:53 2023, max compression
+gzip compressed data, was "linkedinpdfextractor-1.1.7.tar", last modified: Fri May  5 09:50:35 2023, max compression
```

## Comparing `linkedinpdfextractor-1.1.1.tar` & `linkedinpdfextractor-1.1.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.947129 linkedinpdfextractor-1.1.1/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.1.1/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1809 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.1.1/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.1.1/AUTHORS.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/CHANGELOG.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.1.1/LICENSE.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2374 2023-04-24 07:59:53.947317 linkedinpdfextractor-1.1.1/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1865 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/README.rst
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.920647 linkedinpdfextractor-1.1.1/docs/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/Makefile
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.920912 linkedinpdfextractor-1.1.1/docs/_static/
--rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/_static/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/authors.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/changelog.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/conf.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/contributing.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/index.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/license.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/readme.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/docs/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/pyproject.toml
--rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.1.1/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1249 2023-04-24 07:59:53.948259 linkedinpdfextractor-1.1.1/setup.cfg
--rw-r--r--   0 seshivitakula   (501) staff       (20)      719 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/setup.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.921174 linkedinpdfextractor-1.1.1/src/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.1.1/src/.DS_Store
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.922767 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5537 2023-04-24 07:41:41.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/extractor.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.924172 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/__init__.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.925578 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.926979 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.927801 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/model/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/model/document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/model/style.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/source.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/skeleton.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.929405 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2374 2023-04-24 07:59:53.000000 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2518 2023-04-24 07:59:53.000000 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/SOURCES.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-24 07:59:53.000000 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/dependency_links.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/not-zip-safe
--rw-r--r--   0 seshivitakula   (501) staff       (20)      101 2023-04-24 07:59:53.000000 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/requires.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-04-24 07:59:53.000000 linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/top_level.txt
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.934179 linkedinpdfextractor-1.1.1/tests/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 17:09:48.000000 linkedinpdfextractor-1.1.1/tests/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/tests/conftest.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/helper.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.944197 linkedinpdfextractor-1.1.1/tests/resources/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/5648.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/SameSize_BoldTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/SameSize_EnumeratedTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/SameStyleOnly.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/interview_cheatsheet-excerpt.png
--rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/interview_cheatsheet.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/lorem.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/paper.pdf
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 07:59:53.946748 linkedinpdfextractor-1.1.1/tests/resources/parsed/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/parsed/interview_cheatsheet.json
--rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/parsed/interview_cheatsheet_pretty.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.1.1/tests/resources/profile.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.1/tests/resources/samplepptx.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_custom_use_cases.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_hierarchy.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/tests/test_skeleton.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_style_analyser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_traversal.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.1/tests/test_utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.1/tox.ini
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.359652 linkedinpdfextractor-1.1.7/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.1.7/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1809 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.1.7/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.1.7/AUTHORS.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/CHANGELOG.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/CONTRIBUTING.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.1.7/LICENSE.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2917 2023-05-05 09:50:35.359830 linkedinpdfextractor-1.1.7/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2408 2023-05-04 13:07:58.000000 linkedinpdfextractor-1.1.7/README.rst
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.326505 linkedinpdfextractor-1.1.7/docs/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/Makefile
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.326777 linkedinpdfextractor-1.1.7/docs/_static/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/_static/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/authors.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/changelog.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/conf.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/contributing.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/index.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/license.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/readme.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/docs/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/pyproject.toml
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.1.7/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1249 2023-05-05 09:50:35.360787 linkedinpdfextractor-1.1.7/setup.cfg
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      720 2023-05-05 09:47:02.000000 linkedinpdfextractor-1.1.7/setup.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.327046 linkedinpdfextractor-1.1.7/src/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.1.7/src/.DS_Store
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.328658 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5950 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/extractor.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.330127 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/__init__.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.335524 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.342767 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.343685 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/model/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/model/document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/model/style.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/source.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/skeleton.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.346896 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2917 2023-05-05 09:50:35.000000 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2518 2023-05-05 09:50:35.000000 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-05-05 09:50:35.000000 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/not-zip-safe
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      101 2023-05-05 09:50:35.000000 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/requires.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-05-05 09:50:35.000000 linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/top_level.txt
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.350732 linkedinpdfextractor-1.1.7/tests/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.1.7/tests/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/tests/conftest.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/helper.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.357735 linkedinpdfextractor-1.1.7/tests/resources/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/5648.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/SameSize_BoldTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/SameSize_EnumeratedTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/SameStyleOnly.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/interview_cheatsheet-excerpt.png
+-rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/interview_cheatsheet.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/lorem.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/paper.pdf
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-05 09:50:35.359384 linkedinpdfextractor-1.1.7/tests/resources/parsed/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/parsed/interview_cheatsheet.json
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/parsed/interview_cheatsheet_pretty.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.1.7/tests/resources/profile.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.1.7/tests/resources/samplepptx.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_custom_use_cases.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_hierarchy.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/tests/test_skeleton.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_style_analyser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_traversal.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.1.7/tests/test_utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.1.7/tox.ini
```

### Comparing `linkedinpdfextractor-1.1.1/.DS_Store` & `linkedinpdfextractor-1.1.7/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -308,20 +308,20 @@
 00001330: 0000 0000 0000 008b 0000 0003 0073 0072  .............s.r
 00001340: 0063 7653 726e 6c6f 6e67 0000 0001 0000  .cvSrnlong......
 00001350: 0005 0074 0065 0073 0074 0073 496c 6f63  ...t.e.s.t.sIloc
 00001360: 626c 6f62 0000 0010 0000 00af 0000 009e  blob............
 00001370: ffff ffff ffff 0000 0000 0005 0074 0065  .............t.e
 00001380: 0073 0074 0073 6277 7370 626c 6f62 0000  .s.t.sbwspblob..
 00001390: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
-000013a0: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
+000013a0: 0607 0808 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 000013b0: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 000013c0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 000013d0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 000013e0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-000013f0: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
+000013f0: 735b 5368 6f77 5369 6465 6261 7208 0909  s[ShowSidebar...
 00001400: 095f 1018 7b7b 3338 302c 2034 3632 7d2c  ._..{{380, 462},
 00001410: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
 00001420: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
 00001430: 0101 0000 0000 0000 000d 0000 0000 0000  ................
 00001440: 0000 0000 0000 0000 008b 0000 0005 0074  ...............t
 00001450: 0065 0073 0074 0073 7653 726e 6c6f 6e67  .e.s.t.svSrnlong
 00001460: 0000 0001 0000 0007 0074 006f 0078 002e  .........t.o.x..
```

### Comparing `linkedinpdfextractor-1.1.1/.gitignore` & `linkedinpdfextractor-1.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/CONTRIBUTING.rst` & `linkedinpdfextractor-1.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/LICENSE.txt` & `linkedinpdfextractor-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/PKG-INFO` & `linkedinpdfextractor-1.1.7/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: linkedinpdfextractor
-Version: 1.1.1
-Summary: Add a short description here!
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: Ketan Prabhu
-Author-email: ketan.prabhu@gigvistas.com
-License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/linkedin_pdf_extractor.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/linkedin_pdf_extractor
     .. image:: https://readthedocs.org/projects/linkedin_pdf_extractor/badge/?version=latest
@@ -60,7 +43,28 @@
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.3.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+Steps to upload it to pypi:
+1. Delete the old tag 
+command to delete the tag on local repo : git tag -d <tagname>
+
+2. Push the changes to remote:
+command:    git push origin --delete <tagname>
+
+3. create a new tag 
+Command: to create a new tag : git tag -a tagname -m "my version 1.4"
+
+4. push that tag
+Command:    git push origin tagname
+
+5. Build the package distribution
+Command:  tox -e build  # to build your package distribution
+
+6. Publish the package 
+Command: tox -e publish -- --repository pypi  # to release your package to PyPI
+
+
```

### Comparing `linkedinpdfextractor-1.1.1/docs/Makefile` & `linkedinpdfextractor-1.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/docs/conf.py` & `linkedinpdfextractor-1.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/docs/index.rst` & `linkedinpdfextractor-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/setup.cfg` & `linkedinpdfextractor-1.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/setup.py` & `linkedinpdfextractor-1.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
     This file was generated with PyScaffold 4.3.1.
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 from setuptools import setup
 
+from setuptools import setup
+
 if __name__ == "__main__":
     try:
-        setup(use_scm_version={"version_scheme": "no-guess-dev"})
-    except:  # noqa
+        setup(use_scm_version=True)
+    except Exception as e:
+        print("\n\nAn error occurred while building the project:", e)
         print(
-            "\n\nAn error occurred while building the project, "
-            "please ensure you have the most updated version of setuptools, "
-            "setuptools_scm and wheel with:\n"
+            "\n\nPlease ensure you have the most updated version of setuptools, setuptools_scm, and wheel with:\n"
             "   pip install -U setuptools setuptools_scm wheel\n\n"
         )
-        raise
+        raise
```

### Comparing `linkedinpdfextractor-1.1.1/src/.DS_Store` & `linkedinpdfextractor-1.1.7/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/.DS_Store` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/__init__.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/extractor.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/extractor.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 class Experience:
     def __init__(self):
         self.id = 0
         self.companyName = ""
         self.position = ""
         self.date = ""
         self.description = ""
+        self.location = ""
     def toJSON(self):
         return json.dumps(self, default=lambda o: o.__dict__, 
             sort_keys=True, indent=2)
 
 class Education:
     def __init__(self):
         self.course = ""
@@ -76,14 +77,15 @@
 
     a = document.elements
     #print(a[0])
     #print(a[0].children[1])
 
     traverse(document.elements, document.elements[0].level)
     df = pd.DataFrame(Data)
+    print(df)
     dtoData = createData(df)
     print("The variable, name : ", dtoData.name)
     print("The variable, mobile : ", dtoData.contact.mobile)
     print("The variable, email : ", dtoData.contact.email)
     print("The variable, title : ", dtoData.title)
     print("The variable, summary : ", dtoData.summary)
     jsonStr = dtoData.toJSON()
@@ -118,38 +120,52 @@
             user.title = row["text"]
         elif (row['level'] == 2 and row["mean_size"] == 12.0 and row["max_size"] == 12.0 and row["type"] == "Summary"):
             summary.description.append(row["text"])
         elif (row['level'] == 3 and row["mean_size"] == 10.5 and row["max_size"] == 10.5 and row["type"] == "Contact"):
             contact.description = row["text"]
         elif (row['level'] == 3 and row["mean_size"] == 10.5 and row["max_size"] == 10.5 and row["type"] == "Top Skills"):
             user.skills.append(row["text"])
-        # elif (row['level'] == 2 and row["type"] == "Experience"):
-        #     if (row["max_size"] == 12.0):
-        #         if(experience.companyName is not None):
-        #             user.experience.append(experience)
-        #         experience=Experience
-        #         # experience.id = i
-        #         experience.companyName = row['text'].split('\n')[0]
-        #         experience.position = row['text'].split('\n')[1]
-        #         experience.date = row['text'].split('\n')[2]
-        #         i = i + 1
-        #     elif (row["mean_size"] == 10.5 and row["max_size"] == 10.5):
-        #         experience.description.append(row["text"])
-        elif (row['level'] == 2 and row["mean_size"] == 12.0 and row["max_size"] == 12.0 and row["type"] == "Education"):
-            education.description.append(row["text"])
+        elif(row['level'] == 2 and row["type"] == "Experience"):
+            parseExperience(row, user)
+        # elif (row["type"] == "Education"):
+        #     education.description.append(row["text"])
 
     user.summary = ' '.join(map(str, summary.description))
 
-    mobile_pattern = r'\+(\d{1,2})?\s*\d{9,10}\s*\((Mobile)\)'
-    email_pattern = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
-    match = re.search(mobile_pattern, contact.description)
-    if match:
-        contact.mobile = match.group(0)
-        contact.email = re.search(
-            email_pattern, contact.description[match.end():]).group(0)
-    else:
-        contact.email = re.search(email_pattern, contact.description).group(0)
-    user.contact = contact
+    # mobile_pattern = r'\+(\d{1,2})?\s*\d{9,10}\s*\((Mobile)\)'
+    # email_pattern = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
+    # match = re.search(mobile_pattern, contact.description)
+    # if match:
+    #     contact.mobile = match.group(0)
+    #     contact.email = re.search(
+    #         email_pattern, contact.description[match.end():]).group(0)
+    # else:
+    #     contact.email = re.search(email_pattern, contact.description).group(0)
+    # user.contact = contact
 
     return user
 
-#pdf_to_json("/Users/rishav/code/github/gigvistas/linkedin-pdf-parser/tests/resources/profile.pdf")
+def parseExperience(row, user):
+    expLength = len(user.experience)
+    exp = Experience() if expLength == 0 else user.experience[expLength-1]
+    
+    if (row["max_size"] == 12.0):
+        exp = Experience()
+        expElements = row['text'].split('\n')
+        if(len(expElements) == 2):
+            exp.companyName = expElements[0]
+            exp.date = expElements[1].replace('\xa0','')
+        elif(len(expElements) == 3):
+            exp.companyName = expElements[0]
+            exp.position = expElements[1]
+            exp.date = expElements[2].replace('\xa0','')
+        elif(len(expElements) == 4 ):
+            exp.companyName = expElements[0]
+            exp.position = expElements[1]
+            exp.date = expElements[2].replace('\xa0','')
+            exp.location = expElements[3]
+        user.experience.append(exp)
+    elif(row["max_size"] > 9.0):
+        user.experience[expLength-1].description += row["text"]
+
+#pdf_to_json("/Users/rishav/code/github/gigvistas/linkedin-pdf-parser/tests/resources/profile.pdf")
+#pdf_to_json("/Users/rishav/Downloads/rishav_linkedin.pdf")
```

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/model/document.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/model/document.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/model/style.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/model/style.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/printer.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/printer.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/source.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/source.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/pdfstructure/utils.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/pdfstructure/utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedin_pdf_extractor/skeleton.py` & `linkedinpdfextractor-1.1.7/src/linkedin_pdf_extractor/skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/PKG-INFO` & `linkedinpdfextractor-1.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.1.1
+Version: 1.1.7
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -60,7 +60,28 @@
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.3.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
+
+Steps to upload it to pypi:
+1. Delete the old tag 
+command to delete the tag on local repo : git tag -d <tagname>
+
+2. Push the changes to remote:
+command:    git push origin --delete <tagname>
+
+3. create a new tag 
+Command: to create a new tag : git tag -a tagname -m "my version 1.4"
+
+4. push that tag
+Command:    git push origin tagname
+
+5. Build the package distribution
+Command:  tox -e build  # to build your package distribution
+
+6. Publish the package 
+Command: tox -e publish -- --repository pypi  # to release your package to PyPI
+
+
```

### Comparing `linkedinpdfextractor-1.1.1/src/linkedinpdfextractor.egg-info/SOURCES.txt` & `linkedinpdfextractor-1.1.7/src/linkedinpdfextractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/helper.py` & `linkedinpdfextractor-1.1.7/tests/helper.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/5648.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/5648.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/SameSize_BoldTitle.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/SameSize_BoldTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/SameSize_EnumeratedTitle.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/SameSize_EnumeratedTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/SameStyleOnly.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/SameStyleOnly.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/interview_cheatsheet-excerpt.png` & `linkedinpdfextractor-1.1.7/tests/resources/interview_cheatsheet-excerpt.png`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/interview_cheatsheet.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/interview_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/lorem.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/lorem.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/paper.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/paper.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/parsed/interview_cheatsheet.json` & `linkedinpdfextractor-1.1.7/tests/resources/parsed/interview_cheatsheet.json`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/parsed/interview_cheatsheet_pretty.txt` & `linkedinpdfextractor-1.1.7/tests/resources/parsed/interview_cheatsheet_pretty.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/profile.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/profile.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/resources/samplepptx.pdf` & `linkedinpdfextractor-1.1.7/tests/resources/samplepptx.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_custom_use_cases.py` & `linkedinpdfextractor-1.1.7/tests/test_custom_use_cases.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_document.py` & `linkedinpdfextractor-1.1.7/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_headercompare.py` & `linkedinpdfextractor-1.1.7/tests/test_headercompare.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_hierarchy.py` & `linkedinpdfextractor-1.1.7/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_printer.py` & `linkedinpdfextractor-1.1.7/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_skeleton.py` & `linkedinpdfextractor-1.1.7/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_style_analyser.py` & `linkedinpdfextractor-1.1.7/tests/test_style_analyser.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_traversal.py` & `linkedinpdfextractor-1.1.7/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tests/test_utils.py` & `linkedinpdfextractor-1.1.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.1.1/tox.ini` & `linkedinpdfextractor-1.1.7/tox.ini`

 * *Files identical despite different names*

