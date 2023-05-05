# Comparing `tmp/pretext-1.5.3.dev20230504.tar.gz` & `tmp/pretext-1.5.3.dev20230505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.3.dev20230504.tar", max compression
+gzip compressed data, was "pretext-1.5.3.dev20230505.tar", max compression
```

## Comparing `pretext-1.5.3.dev20230504.tar` & `pretext-1.5.3.dev20230505.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2023-05-04 06:18:25.287603 pretext-1.5.3.dev20230504/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-04 06:18:25.287603 pretext-1.5.3.dev20230504/README.md
--rw-r--r--   0        0        0     1440 2023-05-04 06:19:14.204128 pretext-1.5.3.dev20230504/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/core/__init__.py
--rw-r--r--   0        0        0   173946 2023-05-04 06:19:19.480521 pretext-1.5.3.dev20230504/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/core/resources.py
--rw-r--r--   0        0        0  1053177 2023-05-04 06:19:19.480521 pretext-1.5.3.dev20230504/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160171 2023-05-04 06:19:19.540525 pretext-1.5.3.dev20230504/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7677 2023-05-04 06:19:19.564527 pretext-1.5.3.dev20230504/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173370 2023-05-04 06:19:19.560527 pretext-1.5.3.dev20230504/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     1236 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4718 2023-05-04 06:19:19.568527 pretext-1.5.3.dev20230504/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8453 2023-05-04 06:19:19.572528 pretext-1.5.3.dev20230504/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-04 06:18:25.291603 pretext-1.5.3.dev20230504/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-04 06:19:14.204128 pretext-1.5.3.dev20230504/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230504/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/README.md
+-rw-r--r--   0        0        0     1440 2023-05-05 20:46:30.750810 pretext-1.5.3.dev20230505/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-05 20:45:45.982438 pretext-1.5.3.dev20230505/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/core/__init__.py
+-rw-r--r--   0        0        0   173946 2023-05-05 20:46:32.998828 pretext-1.5.3.dev20230505/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/core/resources.py
+-rw-r--r--   0        0        0  1053273 2023-05-05 20:46:32.994828 pretext-1.5.3.dev20230505/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160171 2023-05-05 20:46:33.070829 pretext-1.5.3.dev20230505/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7677 2023-05-05 20:46:33.098829 pretext-1.5.3.dev20230505/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173370 2023-05-05 20:46:33.090829 pretext-1.5.3.dev20230505/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     1236 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4718 2023-05-05 20:46:33.102829 pretext-1.5.3.dev20230505/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      630 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/postCreateCommand.sh
+-rw-r--r--   0        0        0     1710 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8453 2023-05-05 20:46:33.106829 pretext-1.5.3.dev20230505/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-05 20:45:45.986438 pretext-1.5.3.dev20230505/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-05 20:46:30.750810 pretext-1.5.3.dev20230505/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.3.dev20230505/PKG-INFO
```

### Comparing `pretext-1.5.3.dev20230504/LICENSE` & `pretext-1.5.3.dev20230505/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/README.md` & `pretext-1.5.3.dev20230505/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/__init__.py` & `pretext-1.5.3.dev20230505/pretext/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = 'f509db302370e65a3da303230e4ce7cd03c3fb8d'
+CORE_COMMIT = '49b6569fc697733cea093afd581c8cc7c26cf7dd'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.3.dev20230504/pretext/build.py` & `pretext-1.5.3.dev20230505/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/cli.py` & `pretext-1.5.3.dev20230505/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/codechat.py` & `pretext-1.5.3.dev20230505/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/config/xml_overlay.py` & `pretext-1.5.3.dev20230505/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/core/pretext.py` & `pretext-1.5.3.dev20230505/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/core/resources.py` & `pretext-1.5.3.dev20230505/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/core/resources.zip` & `pretext-1.5.3.dev20230505/pretext/core/resources.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 1053177 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/utilities/
--rw-r--r--  2.0 unx    11766 b- defN 23-May-04 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx   262590 b- defN 23-May-04 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-04 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-04 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-04 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-04 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-04 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-May-04 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-04 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-04 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-04 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    69315 b- defN 23-May-04 06:19 xsl/pretext-braille.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-04 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx   544147 b- defN 23-May-04 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    64782 b- defN 23-May-04 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-04 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-04 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-04 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-04 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-04 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-04 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139661 b- defN 23-May-04 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-04 06:19 xsl/README.md
--rw-r--r--  2.0 unx     2740 b- defN 23-May-04 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx   608699 b- defN 23-May-04 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-May-04 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx     2846 b- defN 23-May-04 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-04 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-04 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-04 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   541182 b- defN 23-May-04 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-04 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-04 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    39922 b- defN 23-May-04 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-04 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-04 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-04 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-04 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-04 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-04 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1810 b- defN 23-May-04 06:19 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 23-May-04 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-04 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-May-04 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-04 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    17285 b- defN 23-May-04 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-04 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-May-04 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-04 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-04 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-04 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-04 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-04 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-04 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-04 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx     2227 b- defN 23-May-04 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-04 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-04 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-04 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-May-04 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-04 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-04 06:19 xsl/localizations/pt-PT.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx     5800 b- defN 23-May-04 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-04 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-04 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-May-04 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-May-04 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx      486 b- defN 23-May-04 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5241 b- defN 23-May-04 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-May-04 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-May-04 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-May-04 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx     3024 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-04 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx   133917 b- defN 23-May-04 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx   124561 b- defN 23-May-04 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-May-04 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx      326 b- defN 23-May-04 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    57960 b- defN 23-May-04 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-May-04 06:19 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 23-May-04 06:19 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-May-04 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    25290 b- defN 23-May-04 06:19 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-May-04 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   101402 b- defN 23-May-04 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx     2446 b- defN 23-May-04 06:19 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-04 06:19 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-04 06:19 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-04 06:19 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     1280 b- defN 23-May-04 06:19 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-04 06:19 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-04 06:19 css/style_oscarlevin.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-04 06:19 css/setcolors.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-04 06:19 css/README.md
--rw-r--r--  2.0 unx     4021 b- defN 23-May-04 06:19 css/update_css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-04 06:19 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-04 06:19 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-04 06:19 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-04 06:19 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-04 06:19 css/style_default.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-04 06:19 css/epub.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-04 06:19 css/colors_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-04 06:19 css/style_soundwriting.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-04 06:19 css/mathbook-3.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-04 06:19 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-04 06:19 css/kindle.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-04 06:19 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1276 b- defN 23-May-04 06:19 css/colors_maroon_grey.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 script/braille/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-04 06:19 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-04 06:19 script/mbx
--rw-r--r--  2.0 unx     2573 b- defN 23-May-04 06:19 script/braille/pretext-symbol.dis
--rw-r--r--  2.0 unx     8913 b- defN 23-May-04 06:19 script/braille/pretext.sem
--rw-r--r--  2.0 unx      735 b- defN 23-May-04 06:19 script/braille/README.md
--rw-r--r--  2.0 unx     6616 b- defN 23-May-04 06:19 script/braille/pretext-liblouis.cfg
--rw-r--r--  2.0 unx     1011 b- defN 23-May-04 06:19 script/braille/pretext-liblouis-emboss.cfg
--rw-r--r--  2.0 unx      490 b- defN 23-May-04 06:19 script/braille/pretext-liblouis-electronic.cfg
--rw-r--r--  2.0 unx      481 b- defN 23-May-04 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-May-04 06:19 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      116 b- defN 23-May-04 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx     2566 b- defN 23-May-04 06:19 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1367 b- defN 23-May-04 06:19 pretext/README.md
--rw-r--r--  2.0 unx   173946 b- defN 23-May-04 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx    34807 b- defN 23-May-04 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-04 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx    31361 b- defN 23-May-04 06:19 pretext/pretext
-148 files, 4883208 bytes uncompressed, 1034753 bytes compressed:  78.8%
+Zip file size: 1053273 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/utilities/
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-05 20:46 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx   262590 b- defN 23-May-05 20:46 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-05 20:46 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-05 20:46 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-05 20:46 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-05 20:46 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-05 20:46 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-05 20:46 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-05 20:46 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-05 20:46 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-05 20:46 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    69315 b- defN 23-May-05 20:46 xsl/pretext-braille.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-05 20:46 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx   544147 b- defN 23-May-05 20:46 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    65459 b- defN 23-May-05 20:46 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-05 20:46 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-05 20:46 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-05 20:46 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-05 20:46 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-05 20:46 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-05 20:46 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139661 b- defN 23-May-05 20:46 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-05 20:46 xsl/README.md
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-05 20:46 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx   608699 b- defN 23-May-05 20:46 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-05 20:46 xsl/entities.ent
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-05 20:46 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-05 20:46 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-05 20:46 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-05 20:46 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   541182 b- defN 23-May-05 20:46 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-05 20:46 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-05 20:46 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    39922 b- defN 23-May-05 20:46 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-05 20:46 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   103788 b- defN 23-May-05 20:46 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-05 20:46 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-05 20:46 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-05 20:46 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-05 20:46 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-05 20:46 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 23-May-05 20:46 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-05 20:46 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-05 20:46 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-05 20:46 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-05 20:46 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-05 20:46 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-05 20:46 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-05 20:46 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-05 20:46 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-05 20:46 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-05 20:46 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-05 20:46 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-05 20:46 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-05 20:46 xsl/localizations/README.md
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-05 20:46 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-05 20:46 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-05 20:46 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-05 20:46 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-05 20:46 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-05 20:46 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-05 20:46 xsl/localizations/pt-PT.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-05 20:46 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-05 20:46 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-05 20:46 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-05 20:46 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-May-05 20:46 xsl/support/README.md
+-rw-r--r--  2.0 unx      486 b- defN 23-May-05 20:46 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-05 20:46 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-May-05 20:46 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-05 20:46 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-05 20:46 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-05 20:46 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx   133917 b- defN 23-May-05 20:46 schema/pretext.xml
+-rw-r--r--  2.0 unx   124561 b- defN 23-May-05 20:46 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-05 20:46 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx      326 b- defN 23-May-05 20:46 schema/xml.xsd
+-rw-r--r--  2.0 unx    57960 b- defN 23-May-05 20:46 schema/pretext.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-05 20:46 schema/README.md
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-05 20:46 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-05 20:46 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-05 20:46 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-05 20:46 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   101402 b- defN 23-May-05 20:46 schema/pretext.rng
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-05 20:46 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-05 20:46 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-05 20:46 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-05 20:46 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-05 20:46 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-05 20:46 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-05 20:46 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-05 20:46 css/setcolors.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-05 20:46 css/README.md
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-05 20:46 css/update_css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-05 20:46 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-05 20:46 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-05 20:46 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-05 20:46 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-05 20:46 css/style_default.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-05 20:46 css/epub.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-05 20:46 css/colors_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-05 20:46 css/style_soundwriting.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-05 20:46 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-05 20:46 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-05 20:46 css/kindle.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-05 20:46 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-05 20:46 css/colors_maroon_grey.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 script/braille/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-05 20:46 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-05 20:46 script/mbx
+-rw-r--r--  2.0 unx     2573 b- defN 23-May-05 20:46 script/braille/pretext-symbol.dis
+-rw-r--r--  2.0 unx     8913 b- defN 23-May-05 20:46 script/braille/pretext.sem
+-rw-r--r--  2.0 unx      735 b- defN 23-May-05 20:46 script/braille/README.md
+-rw-r--r--  2.0 unx     6616 b- defN 23-May-05 20:46 script/braille/pretext-liblouis.cfg
+-rw-r--r--  2.0 unx     1011 b- defN 23-May-05 20:46 script/braille/pretext-liblouis-emboss.cfg
+-rw-r--r--  2.0 unx      490 b- defN 23-May-05 20:46 script/braille/pretext-liblouis-electronic.cfg
+-rw-r--r--  2.0 unx      481 b- defN 23-May-05 20:46 script/mjsre/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 20:46 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-05 20:46 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      116 b- defN 23-May-05 20:46 script/mjsre/package.json
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-05 20:46 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-05 20:46 pretext/README.md
+-rw-r--r--  2.0 unx   173946 b- defN 23-May-05 20:46 pretext/pretext.py
+-rw-r--r--  2.0 unx    35057 b- defN 23-May-05 20:46 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 20:46 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-05 20:46 pretext/module-test.py
+-rw-r--r--  2.0 unx    31361 b- defN 23-May-05 20:46 pretext/pretext
+148 files, 4884135 bytes uncompressed, 1034849 bytes compressed:  78.8%
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -528,15 +528,15 @@
   <!-- that will require changes in the Python lxml which assumes otherwise -->
   <xsl:template match="||">
     <xsl:apply-templates select="." mode="block-title"/>
     <xsl:apply-templates select="*[not(self::title)]"/>
   </xsl:template>
   <!-- A "case" is a further division of a PROOF-LIKE -->
   <xsl:template match="case">
-    <runin indentation="2" separator="  ">
+    <runin indentation="2" separator=" ">
       <xsl:apply-templates select="." mode="title-full"/>
     </runin>
     <xsl:apply-templates select="*"/>
   </xsl:template>
   <!-- Titles of blocks can be an entire "segment" if they finish with a  -->
   <!-- newline.  Other titles are "runin" and are consolidated in a final -->
   <!-- post-processing step.                                              -->
@@ -562,43 +562,43 @@
   </xsl:template>
   <!-- Should be run-in with automatic space afterward -->
   <!-- There may be multiple proofs, but we do not number them at birth, -->
   <!-- the number only gets used in a cross-reference.  Maybe standalone -->
   <!-- is different??                                                    -->
   <!-- TENTATIVE: DISCUSSION-LIKE may be identical                       -->
   <xsl:template match="|" mode="block-title">
-    <runin indentation="0" lines-before="1" separator="  ">
+    <runin indentation="0" lines-before="1" separator=" ">
       <!--  -->
       <xsl:apply-templates select="." mode="type-name"/>
       <xsl:text>.</xsl:text>
       <!--  -->
       <xsl:if test="title">
         <xsl:text/>
         <xsl:apply-templates select="." mode="title-full"/>
       </xsl:if>
       <!--  -->
     </runin>
   </xsl:template>
   <!-- Should be run-in with automatic space afterward -->
   <xsl:template match="exercise[not()]" mode="block-title">
-    <runin indentation="0" lines-before="1" separator="  ">
+    <runin indentation="0" lines-before="1" separator=" ">
       <xsl:apply-templates select="." mode="serial-number"/>
       <xsl:text>.</xsl:text>
       <!--  -->
       <xsl:if test="title">
         <xsl:text>(</xsl:text>
         <xsl:apply-templates select="." mode="title-full"/>
         <xsl:text>)</xsl:text>
       </xsl:if>
       <!--  -->
     </runin>
   </xsl:template>
   <!-- Should be run-in with automatic space afterward -->
   <xsl:template match="" mode="block-title">
-    <runin indentation="0" lines-before="1" separator="  ">
+    <runin indentation="0" lines-before="1" separator=" ">
       <!--  -->
       <xsl:apply-templates select="." mode="type-name"/>
       <!--  -->
       <xsl:variable name="the-number">
         <xsl:apply-templates select="." mode="non-singleton-number"/>
       </xsl:variable>
       <xsl:if test="not($the-number = '')">
@@ -615,37 +615,45 @@
       <!--  -->
     </runin>
   </xsl:template>
   <!-- TODO: GOAL-LIKE -->
   <!-- ########### -->
   <!-- FIGURE-LIKE -->
   <!-- ########### -->
+  <!-- [BANA, 2016] 6.2.2 -->
+  <!-- 7-5 margins for captions of "Illustrative Materials" -->
+  <!-- We generalize to titles of "table" and "list" blocks -->
   <!-- [BANA, 2016] 6.2.2(e) -->
   <!-- When both a print caption and a transcriber-generated description    -->
   <!-- are needed, begin the description (enclosed in transcriber's note    -->
   <!-- indicators) on the line following the caption.                       -->
   <!-- Figures are treated different for the case where their contents are  -->
   <!-- images (thus requiring a tactile graphic page to follow the figure). -->
   <xsl:template match="figure[image]">
-    <block breakable="no" box="standard">
-      <segment>
+    <block breakable="no" box="standard" lines-before="1" lines-after="1">
+      <segment indentation="6" runover="4">
         <xsl:apply-templates select="." mode="block-title"/>
       </segment>
       <xsl:apply-templates select="*[not(self::image)]"/>
       <xsl:apply-templates select="image" mode="braille-representation"/>
     </block>
     <!-- Form a page to be replaced by tactile version -->
-    <segment ownpage="yes">
-      <xsl:apply-templates select="." mode="block-title"/>
-    </segment>
+    <block ownpage="yes">
+      <xsl:apply-templates select="." mode="transcriber-note">
+        <xsl:with-param name="message">
+          <xsl:text>Replace this page with</xsl:text>
+          <xsl:apply-templates select="." mode="block-title"/>
+        </xsl:with-param>
+      </xsl:apply-templates>
+    </block>
   </xsl:template>
   <!-- Other FIGURE-LIKE can be handled together -->
   <xsl:template match="figure|listing|table|list">
-    <block breakable="no" box="standard">
-      <segment>
+    <block breakable="no" box="standard" lines-before="1" lines-after="1">
+      <segment indentation="6" runover="4">
         <xsl:apply-templates select="." mode="block-title"/>
       </segment>
       <xsl:apply-templates/>
     </block>
   </xsl:template>
   <!-- Caption/title, with label, number, etc.  "caption" and -->
   <!-- "title" elements are metadata, killed in -common,      -->
@@ -682,17 +690,22 @@
       <xsl:with-param name="message">
         <xsl:apply-templates select="." mode="block-title"/>
         <xsl:text/>
         <xsl:apply-templates select="description"/>
       </xsl:with-param>
     </xsl:apply-templates>
     <!-- Form a page to be replaced by tactile version -->
-    <segment ownpage="yes">
-      <xsl:apply-templates select="." mode="block-title"/>
-    </segment>
+    <block ownpage="yes">
+      <xsl:apply-templates select="." mode="transcriber-note">
+        <xsl:with-param name="message">
+          <xsl:text>Replace this page with</xsl:text>
+          <xsl:apply-templates select="." mode="block-title"/>
+        </xsl:with-param>
+      </xsl:apply-templates>
+    </block>
   </xsl:template>
   <!-- A transcriber note replacing an image when included -->
   <!-- in some other (identifying) structure.              -->
   <xsl:template match="image" mode="braille-representation">
     <!-- A "segment" with the author's "description" -->
     <xsl:apply-templates select="." mode="transcriber-note">
       <xsl:with-param name="message">
@@ -782,15 +795,15 @@
   <!-- 2023-04-06: very prelimnary, e.g. no runover       -->
   <xsl:template match="ul|ol|dl">
     <!-- <segment>LIST</segment> -->
     <xsl:apply-templates select="li"/>
   </xsl:template>
   <xsl:template match="li">
     <!-- Marker as a "runin" element -->
-    <runin indentation="0" separator="  ">
+    <runin indentation="0" separator=" ">
       <xsl:choose>
         <xsl:when test="parent::ol">
           <xsl:apply-templates select="." mode="item-number"/>
           <xsl:text>.</xsl:text>
         </xsl:when>
         <xsl:when test="parent::ul">
           <xsl:apply-templates select="." mode="unicode-list-marker"/>
@@ -841,15 +854,15 @@
   <!-- ########## -->
   <!-- Bibliography [BANA-2016, 22.2.1]                           -->
   <!-- Bibliographic items in a "references" division have a      -->
   <!-- bracketed number leading each new entry, then two spaces   -->
   <!-- of indentation for the remainder .                         -->
   <!-- TODO: expand to accomodate annotations ("note"), BANA 22.3 -->
   <xsl:template match="biblio[@type='raw']">
-    <runin indentation="0" separator="  ">
+    <runin indentation="0" separator=" ">
       <xsl:text>[</xsl:text>
       <xsl:apply-templates select="." mode="serial-number"/>
       <xsl:text>]</xsl:text>
     </runin>
     <segment indentation="0" runover="2">
       <xsl:apply-templates/>
     </segment>
@@ -1336,16 +1349,16 @@
   <!--                                                                   -->
   <!-- Template could be context-free for literal messages, but the      -->
   <!-- $message will sometimes come from the context of an element       -->
   <!-- (e.g. the "description" of an "image")                            -->
   <xsl:template match="*" mode="transcriber-note">
     <xsl:param name="message"/>
     <segment indentation="7" runover="5">
-      <!-- dot 4, dot 46, dot 126, spacee -->
-      <xsl:text>⠈⠨⠣⠀</xsl:text>
+      <!-- dot 4, dot 46, dot 126 -->
+      <xsl:text>⠈⠨⠣</xsl:text>
       <!-- *Copy* literal markup, or result of applying templates -->
       <xsl:copy-of select="$message"/>
-      <!-- space, dot 4, dot 46, dot 345 -->
-      <xsl:text>⠀⠈⠨⠜</xsl:text>
+      <!-- dot 4, dot 46, dot 345 -->
+      <xsl:text>⠈⠨⠜</xsl:text>
     </segment>
   </xsl:template>
 </xsl:stylesheet>
```

#### pretext/braille_format.py

```diff
@@ -745,14 +745,17 @@
         # characters and we assume punctuation does the same.
         # If not, we could map a few punctuation marks to Unicode.
         # Or perhaps set argument to do uncontracted braille.
         return louis.translateString(["en-ueb-g2.ctb"], aline, None, 0)
 
     def process_block(self, blk):
 
+        if blk.ownpage and self.cursor.embossing():
+            self.advance_page()
+
         # Lines before (but not if at the start of a page)
         if not(self.cursor.at_page_start()):
             for i in range(blk.lines_before):
                 self.blank_line()
 
         if blk.box == "standard":
             top_line = "7" * self.line_buffer.text_width
@@ -789,14 +792,19 @@
             self.advance_one_line()
 
         # Lines after
         for i in range(blk.lines_after):
             self.blank_line()
             self.flush()
 
+        # Dedicated page, so off we go (reqires something was written on page)
+        if blk.ownpage and self.cursor.embossing():
+            self.advance_page()
+
+
     # The next two "write" routines simply check if a page advance
     # is necessary/desirable for the block or segment in question,
     # and then call the "process" versions, where the real action
     # happens.  Then a flush.
 
     def write_segment(self, seg):
         # See if a page advance will improve awkward page breaks
```

### Comparing `pretext-1.5.3.dev20230504/pretext/generate.py` & `pretext-1.5.3.dev20230505/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/project.py` & `pretext-1.5.3.dev20230505/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/__init__.py` & `pretext-1.5.3.dev20230505/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/.gitignore` & `pretext-1.5.3.dev20230505/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/article.zip` & `pretext-1.5.3.dev20230505/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 160171 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-04 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-04 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-04 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-May-04 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      449 b- defN 23-May-04 06:18 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-04 06:18 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-04 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-May-05 20:45 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-05 20:46 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-05 20:45 publication/publication.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-05 20:45 assets/frog.jpg
+-rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      449 b- defN 23-May-05 20:45 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-05 20:45 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-05 20:45 source/main.ptx
 15 files, 164515 bytes uncompressed, 158505 bytes compressed:  3.7%
```

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/book.zip` & `pretext-1.5.3.dev20230505/pretext/templates/resources/book.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 7677 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-04 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-04 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
--rw-r--r--  2.0 unx     6114 b- defN 23-May-04 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     1767 b- defN 23-May-04 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-05 20:45 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-05 20:46 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-05 20:45 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-05 20:45 source/main.ptx
 11 files, 15483 bytes uncompressed, 6439 bytes compressed:  58.4%
```

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/demo.zip` & `pretext-1.5.3.dev20230505/pretext/templates/resources/demo.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,37 @@
 Zip file size: 173370 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-May-04 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-04 06:19 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
--rw-r--r--  2.0 unx     6092 b- defN 23-May-04 06:18 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-04 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-04 06:18 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-May-04 06:18 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-04 06:18 source/ch-generate.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-04 06:18 source/frontmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-04 06:18 source/sec-features.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-May-04 06:18 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-04 06:18 source/ch-empty.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-04 06:18 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-04 06:18 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-04 06:18 source/docinfo.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-04 06:18 source/ex-first.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-04 06:18 source/backmatter.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-04 06:18 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-04 06:18 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-04 06:18 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-04 06:18 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-04 06:18 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-May-04 06:18 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-04 06:18 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-04 06:18 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 23-May-04 06:18 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-May-05 20:45 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-05 20:46 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-05 20:45 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-05 20:45 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-05 20:45 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-May-05 20:45 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-05 20:45 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-05 20:45 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-05 20:45 source/sec-features.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-May-05 20:45 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-05 20:45 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-05 20:45 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-05 20:45 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-05 20:45 source/docinfo.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-05 20:45 source/ex-first.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-05 20:45 source/backmatter.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-05 20:45 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-05 20:45 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-05 20:45 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-05 20:45 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-05 20:45 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-May-05 20:45 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-05 20:45 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-05 20:45 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx       10 b- defN 23-May-05 20:45 source/images/sageplot2d.sage
 35 files, 189778 bytes uncompressed, 169270 bytes compressed:  10.8%
```

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/devcontainer.json` & `pretext-1.5.3.dev20230505/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/hello.zip` & `pretext-1.5.3.dev20230505/pretext/templates/resources/hello.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4718 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-May-04 06:18 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-04 06:18 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
--rw-r--r--  2.0 unx      242 b- defN 23-May-04 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      156 b- defN 23-May-04 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-May-05 20:45 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-05 20:45 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
+-rw-r--r--  2.0 unx      242 b- defN 23-May-05 20:45 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      156 b- defN 23-May-05 20:45 source/main.ptx
 11 files, 7494 bytes uncompressed, 3480 bytes compressed:  53.6%
```

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/postCreateCommand.sh` & `pretext-1.5.3.dev20230505/pretext/templates/resources/postCreateCommand.sh`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/project.ptx` & `pretext-1.5.3.dev20230505/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pretext/templates/resources/slideshow.zip` & `pretext-1.5.3.dev20230505/pretext/templates/resources/slideshow.zip`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 8453 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 06:18 xsl/
--rw-r--r--  2.0 unx     2268 b- defN 23-May-04 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-May-04 06:18 project.ptx
--rw-r--r--  2.0 unx     1676 b- defN 23-May-04 06:19 .gitignore
--rw-r--r--  2.0 unx      190 b- defN 23-May-04 06:18 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-04 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      630 b- defN 23-May-04 06:19 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     1236 b- defN 23-May-04 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx    11200 b- defN 23-May-04 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:46 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 20:45 xsl/
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-05 20:46 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-May-05 20:45 project.ptx
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-05 20:46 .gitignore
+-rw-r--r--  2.0 unx      190 b- defN 23-May-05 20:45 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-05 20:45 publication/publication.ptx
+-rw-r--r--  2.0 unx      630 b- defN 23-May-05 20:46 .devcontainer/postCreateCommand.sh
+-rw-r--r--  2.0 unx     1236 b- defN 23-May-05 20:46 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-05 20:45 source/main.ptx
 12 files, 20081 bytes uncompressed, 7121 bytes compressed:  64.5%
```

### Comparing `pretext-1.5.3.dev20230504/pretext/utils.py` & `pretext-1.5.3.dev20230505/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.3.dev20230504/pyproject.toml` & `pretext-1.5.3.dev20230505/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.3.dev20230504"
+version = "1.5.3.dev20230505"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.3.dev20230504/PKG-INFO` & `pretext-1.5.3.dev20230505/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.3.dev20230504
+Version: 1.5.3.dev20230505
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

