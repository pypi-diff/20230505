# Comparing `tmp/orange-widget-base-4.8.1.tar.gz` & `tmp/orange-widget-base-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orange-widget-base-4.8.1.tar", last modified: Mon Sep 14 07:25:58 2020, max compression
+gzip compressed data, was "dist/orange-widget-base-4.9.0.tar", last modified: Thu Oct  8 08:29:24 2020, max compression
```

## Comparing `orange-widget-base-4.8.1.tar` & `orange-widget-base-4.9.0.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.606225 orange-widget-base-4.8.1/
--rw-r--r--   0 primoz     (501) staff       (20)      162 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/.coveragerc
--rw-r--r--   0 primoz     (501) staff       (20)      329 2019-10-04 12:37:48.000000 orange-widget-base-4.8.1/.gitattributes
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.438200 orange-widget-base-4.8.1/.github/
--rw-r--r--   0 primoz     (501) staff       (20)      701 2019-10-04 12:37:48.000000 orange-widget-base-4.8.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 primoz     (501) staff       (20)      226 2019-10-04 12:37:48.000000 orange-widget-base-4.8.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 primoz     (501) staff       (20)      332 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/.gitignore
--rw-r--r--   0 primoz     (501) staff       (20)      157 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/.readthedocs.yml
--rw-r--r--   0 primoz     (501) staff       (20)     1130 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/.travis.yml
--rw-r--r--   0 primoz     (501) staff       (20)       97 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/CHANGELOG.md
--rw-r--r--   0 primoz     (501) staff       (20)     4966 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/CONTRIBUTING.md
--rw-r--r--   0 primoz     (501) staff       (20)      378 2019-10-04 12:37:48.000000 orange-widget-base-4.8.1/LICENSE
--rw-r--r--   0 primoz     (501) staff       (20)      183 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/MANIFEST.in
--rw-r--r--   0 primoz     (501) staff       (20)     1452 2020-09-14 07:25:58.605953 orange-widget-base-4.8.1/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)      947 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/README.md
--rw-r--r--   0 primoz     (501) staff       (20)     1559 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/appveyor.yml
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.445745 orange-widget-base-4.8.1/doc/
--rw-r--r--   0 primoz     (501) staff       (20)     7462 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/Makefile
--rw-r--r--   0 primoz     (501) staff       (20)     7012 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/make.bat
--rw-r--r--   0 primoz     (501) staff       (20)       45 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/requirements-rtd.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.461837 orange-widget-base-4.8.1/doc/source/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.469825 orange-widget-base-4.8.1/doc/source/code/
--rw-r--r--   0 primoz     (501) staff       (20)     1268 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/code/owMultiplier.py
--rw-r--r--   0 primoz     (501) staff       (20)      831 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/code/owNumber.py
--rw-r--r--   0 primoz     (501) staff       (20)     1210 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/code/owProduct.py
--rw-r--r--   0 primoz     (501) staff       (20)      562 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/code/widgetTemplate.py
--rw-r--r--   0 primoz     (501) staff       (20)     1256 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/concurrent.rst
--rw-r--r--   0 primoz     (501) staff       (20)    11882 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/conf.py
--rw-r--r--   0 primoz     (501) staff       (20)     4856 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/gui.rst
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.495374 orange-widget-base-4.8.1/doc/source/images/
--rw-r--r--   0 primoz     (501) staff       (20)    33026 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/dataSamplerBWidget.png
--rw-r--r--   0 primoz     (501) staff       (20)    36203 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/datasampler-channelquerry.png
--rw-r--r--   0 primoz     (501) staff       (20)    20550 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/datasampler-totable.png
--rw-r--r--   0 primoz     (501) staff       (20)    20230 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/datasamplerAempty.png
--rw-r--r--   0 primoz     (501) staff       (20)    71797 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/datasamplerAupdated.png
--rw-r--r--   0 primoz     (501) staff       (20)    16744 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/file-to-learningcurveb.png
--rw-r--r--   0 primoz     (501) staff       (20)     4834 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/io-summary-empty.png
--rw-r--r--   0 primoz     (501) staff       (20)    18430 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/io-summary-popup.png
--rw-r--r--   0 primoz     (501) staff       (20)    11222 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/io-summary.png
--rw-r--r--   0 primoz     (501) staff       (20)    88330 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/learningcurve-output.png
--rw-r--r--   0 primoz     (501) staff       (20)    51967 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/learningcurve.png
--rw-r--r--   0 primoz     (501) staff       (20)    12621 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/owScatterplot.png
--rw-r--r--   0 primoz     (501) staff       (20)    35260 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/progressbar-title.png
--rw-r--r--   0 primoz     (501) staff       (20)    14424 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/progressbar.png
--rw-r--r--   0 primoz     (501) staff       (20)    41488 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/samplewidgetontoolbox.png
--rw-r--r--   0 primoz     (501) staff       (20)    23557 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/schemawithdatasamplerB.png
--rw-r--r--   0 primoz     (501) staff       (20)    24791 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/schemawithdatatable.png
--rw-r--r--   0 primoz     (501) staff       (20)    36373 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/usertips.png
--rw-r--r--   0 primoz     (501) staff       (20)    32173 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/warningmessage.png
--rw-r--r--   0 primoz     (501) staff       (20)    38387 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/images/widgettoolbox.png
--rw-r--r--   0 primoz     (501) staff       (20)      282 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/index.rst
--rw-r--r--   0 primoz     (501) staff       (20)      464 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/messagewidget.rst
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.496608 orange-widget-base-4.8.1/doc/source/orange-demo/
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.504665 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/
--rw-r--r--   0 primoz     (501) staff       (20)     1643 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWDataSamplerA.py
--rw-r--r--   0 primoz     (501) staff       (20)     2764 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWDataSamplerB.py
--rw-r--r--   0 primoz     (501) staff       (20)     2981 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWDataSamplerC.py
--rw-r--r--   0 primoz     (501) staff       (20)    10039 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWLearningCurveA.py
--rw-r--r--   0 primoz     (501) staff       (20)    13552 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWLearningCurveB.py
--rw-r--r--   0 primoz     (501) staff       (20)    19243 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWLearningCurveC.py
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.506212 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/
--rw-r--r--   0 primoz     (501) staff       (20)     2422 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/DataSamplerA.svg
--rw-r--r--   0 primoz     (501) staff       (20)     2425 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/DataSamplerB.svg
--rw-r--r--   0 primoz     (501) staff       (20)     2425 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/DataSamplerC.svg
--rw-r--r--   0 primoz     (501) staff       (20)     5625 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/LearningCurve.svg
--rw-r--r--   0 primoz     (501) staff       (20)      320 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/orange-demo/setup.py
--rw-r--r--   0 primoz     (501) staff       (20)     2884 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/testing.rst
--rw-r--r--   0 primoz     (501) staff       (20)     7912 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/tutorial-channels.rst
--rw-r--r--   0 primoz     (501) staff       (20)     5934 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/tutorial-cont.rst
--rw-r--r--   0 primoz     (501) staff       (20)     5071 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/tutorial-responsive-gui.rst
--rw-r--r--   0 primoz     (501) staff       (20)    14895 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/tutorial-settings.rst
--rw-r--r--   0 primoz     (501) staff       (20)     6661 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/tutorial-utilities.rst
--rw-r--r--   0 primoz     (501) staff       (20)     7055 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/tutorial.rst
--rw-r--r--   0 primoz     (501) staff       (20)     6214 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/doc/source/widget.rst
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.508597 orange-widget-base-4.8.1/orange_widget_base.egg-info/
--rw-r--r--   0 primoz     (501) staff       (20)     1452 2020-09-14 07:25:57.000000 orange-widget-base-4.8.1/orange_widget_base.egg-info/PKG-INFO
--rw-r--r--   0 primoz     (501) staff       (20)     6107 2020-09-14 07:25:57.000000 orange-widget-base-4.8.1/orange_widget_base.egg-info/SOURCES.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2020-09-14 07:25:57.000000 orange-widget-base-4.8.1/orange_widget_base.egg-info/dependency_links.txt
--rw-r--r--   0 primoz     (501) staff       (20)        1 2020-07-03 09:27:24.000000 orange-widget-base-4.8.1/orange_widget_base.egg-info/not-zip-safe
--rw-r--r--   0 primoz     (501) staff       (20)       97 2020-09-14 07:25:57.000000 orange-widget-base-4.8.1/orange_widget_base.egg-info/requires.txt
--rw-r--r--   0 primoz     (501) staff       (20)       13 2020-09-14 07:25:57.000000 orange-widget-base-4.8.1/orange_widget_base.egg-info/top_level.txt
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.512993 orange-widget-base-4.8.1/orangewidget/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    99473 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/gui.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.539199 orange-widget-base-4.8.1/orangewidget/icons/
--rw-r--r--   0 primoz     (501) staff       (20)      352 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_arrow.png
--rw-r--r--   0 primoz     (501) staff       (20)      261 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_clear.png
--rw-r--r--   0 primoz     (501) staff       (20)      584 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_down3.png
--rw-r--r--   0 primoz     (501) staff       (20)      144 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_enter.png
--rw-r--r--   0 primoz     (501) staff       (20)      586 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_pan_hand.png
--rw-r--r--   0 primoz     (501) staff       (20)      345 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_redo.png
--rw-r--r--   0 primoz     (501) staff       (20)      291 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_send.png
--rw-r--r--   0 primoz     (501) staff       (20)      322 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_sort.png
--rw-r--r--   0 primoz     (501) staff       (20)      236 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_undo.png
--rw-r--r--   0 primoz     (501) staff       (20)      555 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_up3.png
--rw-r--r--   0 primoz     (501) staff       (20)      390 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_zoom.png
--rw-r--r--   0 primoz     (501) staff       (20)      348 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_zoom_reset.png
--rw-r--r--   0 primoz     (501) staff       (20)      392 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Dlg_zoom_selection.png
--rw-r--r--   0 primoz     (501) staff       (20)      229 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/Unknown.png
--rw-r--r--   0 primoz     (501) staff       (20)      923 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/chart-hover.svg
--rw-r--r--   0 primoz     (501) staff       (20)      836 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/chart.svg
--rw-r--r--   0 primoz     (501) staff       (20)      924 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/downgreenarrow.png
--rw-r--r--   0 primoz     (501) staff       (20)      659 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/error.png
--rw-r--r--   0 primoz     (501) staff       (20)     1581 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/help-hover.svg
--rw-r--r--   0 primoz     (501) staff       (20)     1084 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/help.svg
--rw-r--r--   0 primoz     (501) staff       (20)      691 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/information.png
--rw-r--r--   0 primoz     (501) staff       (20)      582 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/input-empty.svg
--rw-r--r--   0 primoz     (501) staff       (20)      393 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/input-partial.svg
--rw-r--r--   0 primoz     (501) staff       (20)      265 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/input.svg
--rw-r--r--   0 primoz     (501) staff       (20)      554 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/output-empty.svg
--rw-r--r--   0 primoz     (501) staff       (20)      400 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/output-partial.svg
--rw-r--r--   0 primoz     (501) staff       (20)      273 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/output.svg
--rw-r--r--   0 primoz     (501) staff       (20)      988 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/report-hover.svg
--rw-r--r--   0 primoz     (501) staff       (20)      899 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/report.svg
--rw-r--r--   0 primoz     (501) staff       (20)     2542 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/reset-hover.svg
--rw-r--r--   0 primoz     (501) staff       (20)     2551 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/reset.svg
--rw-r--r--   0 primoz     (501) staff       (20)      926 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/upgreenarrow.png
--rw-r--r--   0 primoz     (501) staff       (20)     2938 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/visual-settings-hover.svg
--rw-r--r--   0 primoz     (501) staff       (20)     2938 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/visual-settings.svg
--rw-r--r--   0 primoz     (501) staff       (20)      664 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/icons/warning.png
--rw-r--r--   0 primoz     (501) staff       (20)    10364 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/io.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.541625 orange-widget-base-4.8.1/orangewidget/report/
--rw-r--r--   0 primoz     (501) staff       (20)      122 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/report/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.542611 orange-widget-base-4.8.1/orangewidget/report/icons/
--rw-r--r--   0 primoz     (501) staff       (20)     4276 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/report/icons/delete.svg
--rw-r--r--   0 primoz     (501) staff       (20)     8825 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/report/icons/scheme.svg
--rw-r--r--   0 primoz     (501) staff       (20)     2764 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/report/index.html
--rw-r--r--   0 primoz     (501) staff       (20)    17097 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/report/owreport.py
--rw-r--r--   0 primoz     (501) staff       (20)    24219 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/report/report.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.543704 orange-widget-base-4.8.1/orangewidget/report/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/report/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)     6922 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/report/tests/test_report.py
--rw-r--r--   0 primoz     (501) staff       (20)    35957 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/settings.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.555125 orange-widget-base-4.8.1/orangewidget/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    24031 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/tests/base.py
--rw-r--r--   0 primoz     (501) staff       (20)    11798 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_context_handler.py
--rw-r--r--   0 primoz     (501) staff       (20)     1023 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_control_getter.py
--rw-r--r--   0 primoz     (501) staff       (20)     7283 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_gui.py
--rw-r--r--   0 primoz     (501) staff       (20)     3981 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_io.py
--rw-r--r--   0 primoz     (501) staff       (20)      662 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_matplotlib_export.py
--rw-r--r--   0 primoz     (501) staff       (20)    10840 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_setting_provider.py
--rw-r--r--   0 primoz     (501) staff       (20)    13752 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_settings_handler.py
--rw-r--r--   0 primoz     (501) staff       (20)    16538 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/tests/test_widget.py
--rw-r--r--   0 primoz     (501) staff       (20)     9485 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/tests/utils.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.580783 orange-widget-base-4.8.1/orangewidget/utils/
--rw-r--r--   0 primoz     (501) staff       (20)     1921 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/PDFExporter.py
--rw-r--r--   0 primoz     (501) staff       (20)    17426 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/SVGExporter.py
--rw-r--r--   0 primoz     (501) staff       (20)     1866 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/__init__.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.581763 orange-widget-base-4.8.1/orangewidget/utils/_webview/
--rw-r--r--   0 primoz     (501) staff       (20)     1758 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/_webview/helpers.js
--rw-r--r--   0 primoz     (501) staff       (20)     1277 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/_webview/init-webengine-webchannel.js
--rw-r--r--   0 primoz     (501) staff       (20)     4327 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/buttons.py
--rw-r--r--   0 primoz     (501) staff       (20)    18499 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/utils/combobox.py
--rw-r--r--   0 primoz     (501) staff       (20)    16697 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/concurrent.py
--rw-r--r--   0 primoz     (501) staff       (20)    15727 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/filedialogs.py
--rw-r--r--   0 primoz     (501) staff       (20)    29470 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/utils/itemmodels.py
--rw-r--r--   0 primoz     (501) staff       (20)     5618 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/utils/listview.py
--rw-r--r--   0 primoz     (501) staff       (20)     6900 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/matplotlib_export.py
--rw-r--r--   0 primoz     (501) staff       (20)    14943 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/messages.py
--rw-r--r--   0 primoz     (501) staff       (20)    25010 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/messagewidget.py
--rw-r--r--   0 primoz     (501) staff       (20)    17760 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/overlay.py
--rw-r--r--   0 primoz     (501) staff       (20)     3362 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/progressbar.py
--rw-r--r--   0 primoz     (501) staff       (20)     1632 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/saveplot.py
--rw-r--r--   0 primoz     (501) staff       (20)     9278 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/signals.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.596143 orange-widget-base-4.8.1/orangewidget/utils/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)     1079 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_buttons.py
--rw-r--r--   0 primoz     (501) staff       (20)     4741 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_combobox.py
--rw-r--r--   0 primoz     (501) staff       (20)    10186 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_concurrent.py
--rw-r--r--   0 primoz     (501) staff       (20)     1321 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_filedialogs.py
--rw-r--r--   0 primoz     (501) staff       (20)    18628 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_itemmodels.py
--rw-r--r--   0 primoz     (501) staff       (20)     2164 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_listview.py
--rw-r--r--   0 primoz     (501) staff       (20)     2108 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_messagewidget.py
--rw-r--r--   0 primoz     (501) staff       (20)     3179 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_overlay.py
--rw-r--r--   0 primoz     (501) staff       (20)     1073 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_save_plot.py
--rw-r--r--   0 primoz     (501) staff       (20)     7737 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_signals.py
--rw-r--r--   0 primoz     (501) staff       (20)     3904 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_visual_settings_dlg.py
--rw-r--r--   0 primoz     (501) staff       (20)     2640 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_webview.py
--rw-r--r--   0 primoz     (501) staff       (20)     6496 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/tests/test_widgetpreview.py
--rw-r--r--   0 primoz     (501) staff       (20)     9889 2020-09-14 07:24:34.000000 orange-widget-base-4.8.1/orangewidget/utils/visual_settings_dlg.py
--rw-r--r--   0 primoz     (501) staff       (20)    22481 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/webview.py
--rw-r--r--   0 primoz     (501) staff       (20)     4863 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/utils/widgetpreview.py
--rw-r--r--   0 primoz     (501) staff       (20)      268 2020-09-14 07:25:57.000000 orange-widget-base-4.8.1/orangewidget/version.py
--rw-r--r--   0 primoz     (501) staff       (20)    64104 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/widget.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.602260 orange-widget-base-4.8.1/orangewidget/workflow/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)     5631 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/config.py
--rw-r--r--   0 primoz     (501) staff       (20)     2221 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/discovery.py
--rw-r--r--   0 primoz     (501) staff       (20)    10150 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/errorreporting.py
--rw-r--r--   0 primoz     (501) staff       (20)     7372 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/mainwindow.py
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.604049 orange-widget-base-4.8.1/orangewidget/workflow/tests/
--rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/tests/__init__.py
--rw-r--r--   0 primoz     (501) staff       (20)    10709 2020-09-11 16:02:36.000000 orange-widget-base-4.8.1/orangewidget/workflow/tests/test_widgetsscheme.py
--rw-r--r--   0 primoz     (501) staff       (20)    29350 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/orangewidget/workflow/widgetsscheme.py
--rw-r--r--   0 primoz     (501) staff       (20)    12683 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/pylintrc
-drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-09-14 07:25:58.605276 orange-widget-base-4.8.1/scripts/
--rwxr-xr-x   0 primoz     (501) staff       (20)      737 2019-10-04 12:37:48.000000 orange-widget-base-4.8.1/scripts/create_changelog.sh
--rw-r--r--   0 primoz     (501) staff       (20)     5026 2020-09-11 08:23:59.000000 orange-widget-base-4.8.1/scripts/create_widget_catalog.py
--rw-r--r--   0 primoz     (501) staff       (20)       38 2020-09-14 07:25:58.606303 orange-widget-base-4.8.1/setup.cfg
--rwxr-xr-x   0 primoz     (501) staff       (20)     4746 2020-09-14 07:25:48.000000 orange-widget-base-4.8.1/setup.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.135061 orange-widget-base-4.9.0/
+-rw-r--r--   0 primoz     (501) staff       (20)      162 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/.coveragerc
+-rw-r--r--   0 primoz     (501) staff       (20)      329 2019-10-04 12:37:48.000000 orange-widget-base-4.9.0/.gitattributes
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.824401 orange-widget-base-4.9.0/.github/
+-rw-r--r--   0 primoz     (501) staff       (20)      701 2019-10-04 12:37:48.000000 orange-widget-base-4.9.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 primoz     (501) staff       (20)      226 2019-10-04 12:37:48.000000 orange-widget-base-4.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 primoz     (501) staff       (20)      332 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/.gitignore
+-rw-r--r--   0 primoz     (501) staff       (20)      157 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/.readthedocs.yml
+-rw-r--r--   0 primoz     (501) staff       (20)     1130 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/.travis.yml
+-rw-r--r--   0 primoz     (501) staff       (20)       97 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/CHANGELOG.md
+-rw-r--r--   0 primoz     (501) staff       (20)     4966 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/CONTRIBUTING.md
+-rw-r--r--   0 primoz     (501) staff       (20)      378 2019-10-04 12:37:48.000000 orange-widget-base-4.9.0/LICENSE
+-rw-r--r--   0 primoz     (501) staff       (20)      183 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/MANIFEST.in
+-rw-r--r--   0 primoz     (501) staff       (20)     1452 2020-10-08 08:29:24.134506 orange-widget-base-4.9.0/PKG-INFO
+-rw-r--r--   0 primoz     (501) staff       (20)      947 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/README.md
+-rw-r--r--   0 primoz     (501) staff       (20)     1559 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/appveyor.yml
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.828426 orange-widget-base-4.9.0/doc/
+-rw-r--r--   0 primoz     (501) staff       (20)     7462 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/Makefile
+-rw-r--r--   0 primoz     (501) staff       (20)     7012 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/make.bat
+-rw-r--r--   0 primoz     (501) staff       (20)       45 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/requirements-rtd.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.838274 orange-widget-base-4.9.0/doc/source/
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.840321 orange-widget-base-4.9.0/doc/source/code/
+-rw-r--r--   0 primoz     (501) staff       (20)     1268 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/code/owMultiplier.py
+-rw-r--r--   0 primoz     (501) staff       (20)      831 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/code/owNumber.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1210 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/code/owProduct.py
+-rw-r--r--   0 primoz     (501) staff       (20)      562 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/code/widgetTemplate.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1256 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/concurrent.rst
+-rw-r--r--   0 primoz     (501) staff       (20)    11882 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/conf.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4856 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/gui.rst
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.865385 orange-widget-base-4.9.0/doc/source/images/
+-rw-r--r--   0 primoz     (501) staff       (20)    33026 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/dataSamplerBWidget.png
+-rw-r--r--   0 primoz     (501) staff       (20)    36203 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/datasampler-channelquerry.png
+-rw-r--r--   0 primoz     (501) staff       (20)    20550 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/datasampler-totable.png
+-rw-r--r--   0 primoz     (501) staff       (20)    20230 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/datasamplerAempty.png
+-rw-r--r--   0 primoz     (501) staff       (20)    71797 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/datasamplerAupdated.png
+-rw-r--r--   0 primoz     (501) staff       (20)    16744 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/file-to-learningcurveb.png
+-rw-r--r--   0 primoz     (501) staff       (20)     4834 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/io-summary-empty.png
+-rw-r--r--   0 primoz     (501) staff       (20)    18430 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/io-summary-popup.png
+-rw-r--r--   0 primoz     (501) staff       (20)    11222 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/io-summary.png
+-rw-r--r--   0 primoz     (501) staff       (20)    88330 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/learningcurve-output.png
+-rw-r--r--   0 primoz     (501) staff       (20)    51967 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/learningcurve.png
+-rw-r--r--   0 primoz     (501) staff       (20)    12621 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/owScatterplot.png
+-rw-r--r--   0 primoz     (501) staff       (20)    35260 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/progressbar-title.png
+-rw-r--r--   0 primoz     (501) staff       (20)    14424 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/progressbar.png
+-rw-r--r--   0 primoz     (501) staff       (20)    41488 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/samplewidgetontoolbox.png
+-rw-r--r--   0 primoz     (501) staff       (20)    23557 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/schemawithdatasamplerB.png
+-rw-r--r--   0 primoz     (501) staff       (20)    24791 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/schemawithdatatable.png
+-rw-r--r--   0 primoz     (501) staff       (20)    36373 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/usertips.png
+-rw-r--r--   0 primoz     (501) staff       (20)    32173 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/warningmessage.png
+-rw-r--r--   0 primoz     (501) staff       (20)    38387 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/images/widgettoolbox.png
+-rw-r--r--   0 primoz     (501) staff       (20)      282 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/index.rst
+-rw-r--r--   0 primoz     (501) staff       (20)      464 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/messagewidget.rst
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.866395 orange-widget-base-4.9.0/doc/source/orange-demo/
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.876690 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/
+-rw-r--r--   0 primoz     (501) staff       (20)     1643 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWDataSamplerA.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2764 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWDataSamplerB.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2981 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWDataSamplerC.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10039 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWLearningCurveA.py
+-rw-r--r--   0 primoz     (501) staff       (20)    13552 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWLearningCurveB.py
+-rw-r--r--   0 primoz     (501) staff       (20)    19243 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWLearningCurveC.py
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.878967 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/
+-rw-r--r--   0 primoz     (501) staff       (20)     2422 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/DataSamplerA.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     2425 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/DataSamplerB.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     2425 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/DataSamplerC.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     5625 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/LearningCurve.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      320 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/orange-demo/setup.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2884 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/testing.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     7912 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/tutorial-channels.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     5934 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/tutorial-cont.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     5071 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/tutorial-responsive-gui.rst
+-rw-r--r--   0 primoz     (501) staff       (20)    14895 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/tutorial-settings.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     6661 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/tutorial-utilities.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     7055 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/tutorial.rst
+-rw-r--r--   0 primoz     (501) staff       (20)     6214 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/doc/source/widget.rst
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.882746 orange-widget-base-4.9.0/orange_widget_base.egg-info/
+-rw-r--r--   0 primoz     (501) staff       (20)     1452 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orange_widget_base.egg-info/PKG-INFO
+-rw-r--r--   0 primoz     (501) staff       (20)     6107 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orange_widget_base.egg-info/SOURCES.txt
+-rw-r--r--   0 primoz     (501) staff       (20)        1 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orange_widget_base.egg-info/dependency_links.txt
+-rw-r--r--   0 primoz     (501) staff       (20)        1 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orange_widget_base.egg-info/not-zip-safe
+-rw-r--r--   0 primoz     (501) staff       (20)       97 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orange_widget_base.egg-info/requires.txt
+-rw-r--r--   0 primoz     (501) staff       (20)       13 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orange_widget_base.egg-info/top_level.txt
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.889321 orange-widget-base-4.9.0/orangewidget/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    99966 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/gui.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.916975 orange-widget-base-4.9.0/orangewidget/icons/
+-rw-r--r--   0 primoz     (501) staff       (20)      352 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_arrow.png
+-rw-r--r--   0 primoz     (501) staff       (20)      261 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_clear.png
+-rw-r--r--   0 primoz     (501) staff       (20)      584 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_down3.png
+-rw-r--r--   0 primoz     (501) staff       (20)      144 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_enter.png
+-rw-r--r--   0 primoz     (501) staff       (20)      586 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_pan_hand.png
+-rw-r--r--   0 primoz     (501) staff       (20)      345 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_redo.png
+-rw-r--r--   0 primoz     (501) staff       (20)      291 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_send.png
+-rw-r--r--   0 primoz     (501) staff       (20)      322 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_sort.png
+-rw-r--r--   0 primoz     (501) staff       (20)      236 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_undo.png
+-rw-r--r--   0 primoz     (501) staff       (20)      555 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_up3.png
+-rw-r--r--   0 primoz     (501) staff       (20)      390 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_zoom.png
+-rw-r--r--   0 primoz     (501) staff       (20)      348 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_zoom_reset.png
+-rw-r--r--   0 primoz     (501) staff       (20)      392 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Dlg_zoom_selection.png
+-rw-r--r--   0 primoz     (501) staff       (20)      229 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/Unknown.png
+-rw-r--r--   0 primoz     (501) staff       (20)      923 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/chart-hover.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      836 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/chart.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      924 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/downgreenarrow.png
+-rw-r--r--   0 primoz     (501) staff       (20)      659 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/error.png
+-rw-r--r--   0 primoz     (501) staff       (20)     1581 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/help-hover.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     1084 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/help.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      691 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/information.png
+-rw-r--r--   0 primoz     (501) staff       (20)      582 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/input-empty.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      393 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/input-partial.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      265 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/input.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      554 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/output-empty.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      400 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/output-partial.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      273 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/output.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      988 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/report-hover.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      899 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/report.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     2542 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/reset-hover.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     2551 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/reset.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      926 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/upgreenarrow.png
+-rw-r--r--   0 primoz     (501) staff       (20)     2938 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/visual-settings-hover.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     2938 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/visual-settings.svg
+-rw-r--r--   0 primoz     (501) staff       (20)      664 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/icons/warning.png
+-rw-r--r--   0 primoz     (501) staff       (20)    10364 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/io.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.920540 orange-widget-base-4.9.0/orangewidget/report/
+-rw-r--r--   0 primoz     (501) staff       (20)      122 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/report/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.922239 orange-widget-base-4.9.0/orangewidget/report/icons/
+-rw-r--r--   0 primoz     (501) staff       (20)     4276 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/report/icons/delete.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     8825 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/report/icons/scheme.svg
+-rw-r--r--   0 primoz     (501) staff       (20)     2764 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/report/index.html
+-rw-r--r--   0 primoz     (501) staff       (20)    17097 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/report/owreport.py
+-rw-r--r--   0 primoz     (501) staff       (20)    24219 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/report/report.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.923116 orange-widget-base-4.9.0/orangewidget/report/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/report/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)     6922 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/report/tests/test_report.py
+-rw-r--r--   0 primoz     (501) staff       (20)    35957 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/settings.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:23.932757 orange-widget-base-4.9.0/orangewidget/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    25361 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/tests/base.py
+-rw-r--r--   0 primoz     (501) staff       (20)    11798 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/tests/test_context_handler.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1023 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/tests/test_control_getter.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7283 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/tests/test_gui.py
+-rw-r--r--   0 primoz     (501) staff       (20)     3981 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/tests/test_io.py
+-rw-r--r--   0 primoz     (501) staff       (20)      662 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/tests/test_matplotlib_export.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10840 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/tests/test_setting_provider.py
+-rw-r--r--   0 primoz     (501) staff       (20)    13752 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/tests/test_settings_handler.py
+-rw-r--r--   0 primoz     (501) staff       (20)    16538 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/tests/test_widget.py
+-rw-r--r--   0 primoz     (501) staff       (20)     9485 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/tests/utils.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.051402 orange-widget-base-4.9.0/orangewidget/utils/
+-rw-r--r--   0 primoz     (501) staff       (20)     1921 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/PDFExporter.py
+-rw-r--r--   0 primoz     (501) staff       (20)    17426 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/SVGExporter.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1866 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/__init__.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.084469 orange-widget-base-4.9.0/orangewidget/utils/_webview/
+-rw-r--r--   0 primoz     (501) staff       (20)     1758 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/_webview/helpers.js
+-rw-r--r--   0 primoz     (501) staff       (20)     1277 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/_webview/init-webengine-webchannel.js
+-rw-r--r--   0 primoz     (501) staff       (20)     4327 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/buttons.py
+-rw-r--r--   0 primoz     (501) staff       (20)    18499 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/utils/combobox.py
+-rw-r--r--   0 primoz     (501) staff       (20)    16697 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/concurrent.py
+-rw-r--r--   0 primoz     (501) staff       (20)    15727 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/utils/filedialogs.py
+-rw-r--r--   0 primoz     (501) staff       (20)    29470 2020-10-07 06:16:11.000000 orange-widget-base-4.9.0/orangewidget/utils/itemmodels.py
+-rw-r--r--   0 primoz     (501) staff       (20)     5618 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/utils/listview.py
+-rw-r--r--   0 primoz     (501) staff       (20)     6900 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/matplotlib_export.py
+-rw-r--r--   0 primoz     (501) staff       (20)    14943 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/messages.py
+-rw-r--r--   0 primoz     (501) staff       (20)    25010 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/messagewidget.py
+-rw-r--r--   0 primoz     (501) staff       (20)    17760 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/overlay.py
+-rw-r--r--   0 primoz     (501) staff       (20)     3362 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/progressbar.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1632 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/saveplot.py
+-rw-r--r--   0 primoz     (501) staff       (20)     9278 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/signals.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.117758 orange-widget-base-4.9.0/orangewidget/utils/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1079 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_buttons.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4741 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_combobox.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10186 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_concurrent.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1321 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_filedialogs.py
+-rw-r--r--   0 primoz     (501) staff       (20)    18628 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_itemmodels.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2164 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_listview.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2108 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_messagewidget.py
+-rw-r--r--   0 primoz     (501) staff       (20)     3179 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_overlay.py
+-rw-r--r--   0 primoz     (501) staff       (20)     1073 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_save_plot.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7737 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_signals.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4608 2020-10-06 14:21:39.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_visual_settings_dlg.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2640 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_webview.py
+-rw-r--r--   0 primoz     (501) staff       (20)     6496 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/tests/test_widgetpreview.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10000 2020-10-06 14:21:39.000000 orange-widget-base-4.9.0/orangewidget/utils/visual_settings_dlg.py
+-rw-r--r--   0 primoz     (501) staff       (20)    22481 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/webview.py
+-rw-r--r--   0 primoz     (501) staff       (20)     4863 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/utils/widgetpreview.py
+-rw-r--r--   0 primoz     (501) staff       (20)      268 2020-10-08 08:29:22.000000 orange-widget-base-4.9.0/orangewidget/version.py
+-rw-r--r--   0 primoz     (501) staff       (20)    64104 2020-10-06 14:27:36.000000 orange-widget-base-4.9.0/orangewidget/widget.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.123528 orange-widget-base-4.9.0/orangewidget/workflow/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)     5631 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/config.py
+-rw-r--r--   0 primoz     (501) staff       (20)     2221 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/discovery.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10150 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/errorreporting.py
+-rw-r--r--   0 primoz     (501) staff       (20)     7372 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/mainwindow.py
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.127605 orange-widget-base-4.9.0/orangewidget/workflow/tests/
+-rw-r--r--   0 primoz     (501) staff       (20)        0 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/tests/__init__.py
+-rw-r--r--   0 primoz     (501) staff       (20)    10709 2020-09-11 16:02:36.000000 orange-widget-base-4.9.0/orangewidget/workflow/tests/test_widgetsscheme.py
+-rw-r--r--   0 primoz     (501) staff       (20)    29350 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/orangewidget/workflow/widgetsscheme.py
+-rw-r--r--   0 primoz     (501) staff       (20)    12683 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/pylintrc
+drwxr-xr-x   0 primoz     (501) staff       (20)        0 2020-10-08 08:29:24.130878 orange-widget-base-4.9.0/scripts/
+-rwxr-xr-x   0 primoz     (501) staff       (20)      737 2019-10-04 12:37:48.000000 orange-widget-base-4.9.0/scripts/create_changelog.sh
+-rw-r--r--   0 primoz     (501) staff       (20)     5026 2020-09-11 08:23:59.000000 orange-widget-base-4.9.0/scripts/create_widget_catalog.py
+-rw-r--r--   0 primoz     (501) staff       (20)       38 2020-10-08 08:29:24.135480 orange-widget-base-4.9.0/setup.cfg
+-rwxr-xr-x   0 primoz     (501) staff       (20)     4746 2020-10-08 08:28:15.000000 orange-widget-base-4.9.0/setup.py
```

### Comparing `orange-widget-base-4.8.1/.github/ISSUE_TEMPLATE.md` & `orange-widget-base-4.9.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/.travis.yml` & `orange-widget-base-4.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/CONTRIBUTING.md` & `orange-widget-base-4.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/PKG-INFO` & `orange-widget-base-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-widget-base
-Version: 4.8.1
+Version: 4.9.0
 Summary: Base Widget for Orange Canvas
 Home-page: http://orange.biolab.si/
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 License: GPLv3+
 Description: 
         This project implements the base OWBaseWidget class and utilities for use in
```

### Comparing `orange-widget-base-4.8.1/README.md` & `orange-widget-base-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/appveyor.yml` & `orange-widget-base-4.9.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/Makefile` & `orange-widget-base-4.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/make.bat` & `orange-widget-base-4.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/code/owMultiplier.py` & `orange-widget-base-4.9.0/doc/source/code/owMultiplier.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/code/owNumber.py` & `orange-widget-base-4.9.0/doc/source/code/owNumber.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/code/owProduct.py` & `orange-widget-base-4.9.0/doc/source/code/owProduct.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/code/widgetTemplate.py` & `orange-widget-base-4.9.0/doc/source/code/widgetTemplate.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/concurrent.rst` & `orange-widget-base-4.9.0/doc/source/concurrent.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/conf.py` & `orange-widget-base-4.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/gui.rst` & `orange-widget-base-4.9.0/doc/source/gui.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/dataSamplerBWidget.png` & `orange-widget-base-4.9.0/doc/source/images/dataSamplerBWidget.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/datasampler-channelquerry.png` & `orange-widget-base-4.9.0/doc/source/images/datasampler-channelquerry.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/datasampler-totable.png` & `orange-widget-base-4.9.0/doc/source/images/datasampler-totable.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/datasamplerAempty.png` & `orange-widget-base-4.9.0/doc/source/images/datasamplerAempty.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/datasamplerAupdated.png` & `orange-widget-base-4.9.0/doc/source/images/datasamplerAupdated.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/file-to-learningcurveb.png` & `orange-widget-base-4.9.0/doc/source/images/file-to-learningcurveb.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/io-summary-empty.png` & `orange-widget-base-4.9.0/doc/source/images/io-summary-empty.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/io-summary-popup.png` & `orange-widget-base-4.9.0/doc/source/images/io-summary-popup.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/io-summary.png` & `orange-widget-base-4.9.0/doc/source/images/io-summary.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/learningcurve-output.png` & `orange-widget-base-4.9.0/doc/source/images/learningcurve-output.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/learningcurve.png` & `orange-widget-base-4.9.0/doc/source/images/learningcurve.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/owScatterplot.png` & `orange-widget-base-4.9.0/doc/source/images/owScatterplot.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/progressbar-title.png` & `orange-widget-base-4.9.0/doc/source/images/progressbar-title.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/progressbar.png` & `orange-widget-base-4.9.0/doc/source/images/progressbar.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/samplewidgetontoolbox.png` & `orange-widget-base-4.9.0/doc/source/images/samplewidgetontoolbox.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/schemawithdatasamplerB.png` & `orange-widget-base-4.9.0/doc/source/images/schemawithdatasamplerB.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/schemawithdatatable.png` & `orange-widget-base-4.9.0/doc/source/images/schemawithdatatable.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/usertips.png` & `orange-widget-base-4.9.0/doc/source/images/usertips.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/warningmessage.png` & `orange-widget-base-4.9.0/doc/source/images/warningmessage.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/images/widgettoolbox.png` & `orange-widget-base-4.9.0/doc/source/images/widgettoolbox.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWDataSamplerA.py` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWDataSamplerA.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWDataSamplerB.py` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWDataSamplerB.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWDataSamplerC.py` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWDataSamplerC.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWLearningCurveA.py` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWLearningCurveA.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWLearningCurveB.py` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWLearningCurveB.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/OWLearningCurveC.py` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/OWLearningCurveC.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/DataSamplerA.svg` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/DataSamplerA.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/DataSamplerB.svg` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/DataSamplerB.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/DataSamplerC.svg` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/DataSamplerC.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/orange-demo/orangedemo/icons/LearningCurve.svg` & `orange-widget-base-4.9.0/doc/source/orange-demo/orangedemo/icons/LearningCurve.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/testing.rst` & `orange-widget-base-4.9.0/doc/source/testing.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/tutorial-channels.rst` & `orange-widget-base-4.9.0/doc/source/tutorial-channels.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/tutorial-cont.rst` & `orange-widget-base-4.9.0/doc/source/tutorial-cont.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/tutorial-responsive-gui.rst` & `orange-widget-base-4.9.0/doc/source/tutorial-responsive-gui.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/tutorial-settings.rst` & `orange-widget-base-4.9.0/doc/source/tutorial-settings.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/tutorial-utilities.rst` & `orange-widget-base-4.9.0/doc/source/tutorial-utilities.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/tutorial.rst` & `orange-widget-base-4.9.0/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/doc/source/widget.rst` & `orange-widget-base-4.9.0/doc/source/widget.rst`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orange_widget_base.egg-info/PKG-INFO` & `orange-widget-base-4.9.0/orange_widget_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-widget-base
-Version: 4.8.1
+Version: 4.9.0
 Summary: Base Widget for Orange Canvas
 Home-page: http://orange.biolab.si/
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 License: GPLv3+
 Description: 
         This project implements the base OWBaseWidget class and utilities for use in
```

### Comparing `orange-widget-base-4.8.1/orange_widget_base.egg-info/SOURCES.txt` & `orange-widget-base-4.9.0/orange_widget_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/gui.py` & `orange-widget-base-4.9.0/orangewidget/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             if hasattr(self, "controlled_attributes"):
                 for callback in self.controlled_attributes.get(name, ()):
                     callback(value)
 
 
 def miscellanea(control, box, parent,
                 addToLayout=True, stretch=0, sizePolicy=None, addSpace=False,
-                disabled=False, tooltip=None, **kwargs):
+                disabled=False, tooltip=None, disabledBy=None, **kwargs):
     """
     Helper function that sets various properties of the widget using a common
     set of arguments.
 
     The function
     - sets the `control`'s attribute `box`, if `box` is given and `control.box`
     is not yet set,
@@ -221,14 +221,16 @@
     :param addToLayout: If set to `False` the widget is not added to the layout
     :type addToLayout: bool
     :param stretch: the stretch factor for this widget, used when adding to
         the layout (default: 0)
     :type stretch: int
     :param tooltip: tooltip that is attached to the widget
     :type tooltip: str or None
+    :param disabledBy: checkbox created with checkBox() function
+    :type disabledBy: QCheckBox or None
     :param sizePolicy: the size policy for the box or the control
     :type sizePolicy: QSizePolicy
     """
     for prop, val in kwargs.items():
         if prop == "sizePolicy":
             control.setSizePolicy(QSizePolicy(*val))
         else:
@@ -242,14 +244,17 @@
         box = None
     elif box and box is not control and not hasattr(control, "box"):
         control.box = box
     if box and box.layout() is not None and \
             isinstance(control, QtWidgets.QWidget) and \
             box.layout().indexOf(control) == -1:
         box.layout().addWidget(control)
+    if disabledBy is not None:
+        disabledBy.disables.append(control)
+        disabledBy.makeConsistent()
     if sizePolicy is not None:
         if isinstance(sizePolicy, tuple):
             sizePolicy = QSizePolicy(*sizePolicy)
         (box or control).setSizePolicy(sizePolicy)
     if addToLayout and parent and parent.layout() is not None:
         parent.layout().addWidget(box or control, stretch)
         _addSpace(parent, addSpace)
@@ -1218,15 +1223,15 @@
     :rtype: :obj:`QSlider` or :obj:`FloatSlider`
     """
     sliderBox = hBox(widget, box, addToLayout=False)
     if label:
         widgetLabel(sliderBox, label)
     sliderOrient = Qt.Vertical if vertical else Qt.Horizontal
     if intOnly:
-        slider = QSlider(sliderOrient, sliderBox)
+        slider = Slider(sliderOrient, sliderBox)
         slider.setRange(minValue, maxValue)
         if step:
             slider.setSingleStep(step)
             slider.setPageStep(step)
             slider.setTickInterval(step)
         signal = slider.valueChanged[int]
     else:
@@ -1295,15 +1300,15 @@
     :type width: int
     :rtype: :obj:`QSlider`
     """
     sliderBox = hBox(widget, box, addToLayout=False)
     if label:
         widgetLabel(sliderBox, label)
     sliderOrient = Qt.Vertical if vertical else Qt.Horizontal
-    slider = QSlider(sliderOrient, sliderBox)
+    slider = Slider(sliderOrient, sliderBox)
     slider.ogValue = value
     slider.setRange(0, len(labels) - 1)
     slider.setSingleStep(1)
     slider.setPageStep(1)
     slider.setTickInterval(1)
     sliderBox.layout().addWidget(slider)
     slider.setValue(labels.index(getdeepattr(master, value)))
@@ -1371,15 +1376,15 @@
     if isinstance(labelFormat, str):
         labelFormat = lambda x, f=labelFormat: f % x
 
     sliderBox = hBox(widget, box, addToLayout=False)
     if label:
         widgetLabel(sliderBox, label)
     slider_orient = Qt.Vertical if vertical else Qt.Horizontal
-    slider = QSlider(slider_orient, sliderBox)
+    slider = Slider(slider_orient, sliderBox)
     slider.ogValue = value
     slider.setRange(0, len(values) - 1)
     slider.setSingleStep(1)
     slider.setPageStep(1)
     slider.setTickInterval(1)
     sliderBox.layout().addWidget(slider)
     slider.setValue(values.index(getdeepattr(master, value)))
@@ -2596,15 +2601,27 @@
 
     button_size = \
         style.pixelMetric(QStyle.PM_SmallIconSize) + \
         style.pixelMetric(QStyle.PM_ButtonMargin)
     return button_size
 
 
-class FloatSlider(QSlider):
+class Slider(QSlider):
+    """
+    Slider that disables wheel events.
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.setFocusPolicy(Qt.StrongFocus)
+
+    def wheelEvent(self, event):
+        event.ignore()
+
+
+class FloatSlider(Slider):
     """
     Slider for continuous values.
 
     The slider is derived from `QtGui.QSlider`, but maps from its discrete
     numbers to the desired continuous interval.
     """
     valueChangedFloat = Signal(float)
```

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/Dlg_down3.png` & `orange-widget-base-4.9.0/orangewidget/icons/Dlg_down3.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/Dlg_pan_hand.png` & `orange-widget-base-4.9.0/orangewidget/icons/Dlg_pan_hand.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/Dlg_up3.png` & `orange-widget-base-4.9.0/orangewidget/icons/Dlg_up3.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/chart-hover.svg` & `orange-widget-base-4.9.0/orangewidget/icons/chart-hover.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/chart.svg` & `orange-widget-base-4.9.0/orangewidget/icons/chart.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/downgreenarrow.png` & `orange-widget-base-4.9.0/orangewidget/icons/downgreenarrow.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/error.png` & `orange-widget-base-4.9.0/orangewidget/icons/error.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/help-hover.svg` & `orange-widget-base-4.9.0/orangewidget/icons/help-hover.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/help.svg` & `orange-widget-base-4.9.0/orangewidget/icons/help.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/information.png` & `orange-widget-base-4.9.0/orangewidget/icons/information.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/input-empty.svg` & `orange-widget-base-4.9.0/orangewidget/icons/input-empty.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/output-empty.svg` & `orange-widget-base-4.9.0/orangewidget/icons/output-empty.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/report-hover.svg` & `orange-widget-base-4.9.0/orangewidget/icons/report-hover.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/report.svg` & `orange-widget-base-4.9.0/orangewidget/icons/report.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/reset-hover.svg` & `orange-widget-base-4.9.0/orangewidget/icons/reset-hover.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/reset.svg` & `orange-widget-base-4.9.0/orangewidget/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/upgreenarrow.png` & `orange-widget-base-4.9.0/orangewidget/icons/upgreenarrow.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/visual-settings-hover.svg` & `orange-widget-base-4.9.0/orangewidget/icons/visual-settings-hover.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/visual-settings.svg` & `orange-widget-base-4.9.0/orangewidget/icons/visual-settings.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/icons/warning.png` & `orange-widget-base-4.9.0/orangewidget/icons/warning.png`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/io.py` & `orange-widget-base-4.9.0/orangewidget/io.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/report/icons/delete.svg` & `orange-widget-base-4.9.0/orangewidget/report/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/report/icons/scheme.svg` & `orange-widget-base-4.9.0/orangewidget/report/icons/scheme.svg`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/report/index.html` & `orange-widget-base-4.9.0/orangewidget/report/index.html`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/report/owreport.py` & `orange-widget-base-4.9.0/orangewidget/report/owreport.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/report/report.py` & `orange-widget-base-4.9.0/orangewidget/report/report.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/report/tests/test_report.py` & `orange-widget-base-4.9.0/orangewidget/report/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/settings.py` & `orange-widget-base-4.9.0/orangewidget/settings.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/base.py` & `orange-widget-base-4.9.0/orangewidget/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         self._changed()
 
 
 class DummySignalManager:
     def __init__(self):
         self.outputs = {}
 
+    def clear(self):
+        self.outputs.clear()
+
     def send(self, widget, signal_name, value, id):
         if not isinstance(signal_name, str):
             signal_name = signal_name.name
         current = self.outputs.get((widget, signal_name), None)
         self.outputs[(widget, signal_name)] = value
         if isinstance(current, _Invalidated):
             current.completed.emit(value)
@@ -159,28 +162,30 @@
     def setUpClass(cls):
         """Prepare for test execution.
 
         Ensure that a (single copy of) QApplication has been created
         """
         global app
         if app is None:
-            app = QApplication([])
+            app = QApplication.instance()
+        if app is None:
+            app = QApplication(["-", "-widgetcount"])
+
         # Disable App Nap on macOS (see
         # https://codereview.qt-project.org/c/qt/qtbase/+/202515 for more)
         if sys.platform == "darwin":
             try:
                 import appnope
             except ImportError:
                 pass
             else:
                 appnope.nope()
         cls.tear_down_stack = ExitStack()
         super().setUpClass()
 
-
     @classmethod
     def tearDownClass(cls) -> None:
         if "pyqtgraph" in sys.modules:
             import pyqtgraph
             pyqtgraph.setConfigOption("exitCleanup", False)
         cls.tear_down_stack.close()
         super().tearDownClass()
@@ -226,31 +231,47 @@
         """
         super().setUpClass()
 
         cls.widgets = []
 
         cls.signal_manager = DummySignalManager()
 
-        report = OWReport()
-        cls.widgets.append(report)
+        report = None
+
+        def get_instance():
+            nonlocal report
+            if report is None:
+                report = OWReport()
+                if not (os.environ.get("TRAVIS") or os.environ.get("APPVEYOR")):
+                    report.show = Mock()
+                cls.widgets.append(report)
+            return report
 
         cls.tear_down_stack.enter_context(
-            patch.object(OWReport, "get_instance", lambda: report)
+            patch.object(OWReport, "get_instance", get_instance)
         )
 
-        if not (os.environ.get("TRAVIS") or os.environ.get("APPVEYOR")):
-            report.show = Mock()
-
     @classmethod
     def tearDownClass(cls) -> None:
+        cls.signal_manager.clear()
+        del cls.signal_manager
+        widgets = cls.widgets[:]
         cls.widgets.clear()
+        while widgets:
+            w = widgets.pop(-1)
+            if not w.__dict__.get("_Cls__didCallOnDeleteWidget", False):
+                w.onDeleteWidget()
+            if not sip.isdeleted(w):
+                w.deleteLater()
+            w.signalManager = None
         super().tearDownClass()
 
     def tearDown(self):
         """Process any pending events before the next test is executed."""
+        self.signal_manager.clear()
         QTest.qWait(0)
         super().tearDown()
 
     def create_widget(self, cls, stored_settings=None, reset_default_settings=True):
         # type: (Type[T], Optional[dict], bool) -> T
         """Create a widget instance using mock signal_manager.
 
@@ -270,17 +291,31 @@
             If set, widget will start with default values for settings,
             if not, values accumulated through the session will be used
 
         Returns
         -------
         Widget instance : cls
         """
+        # Use a substitute subclass to mark calls to onDeleteWidget; Some tests
+        # call this on their own (this used to be done in tearDownClass, then
+        # it was not, so tests did it themself, now it is done again).
+        with open_widget_classes():
+            class Cls(cls):
+                def onDeleteWidget(self):
+                    self.__didCallOnDeleteWidget = True
+                    super(Cls, self).onDeleteWidget()
+                __didCallOnDeleteWidget = False
+
+            Cls.__name__ = cls.__name__
+            Cls.__qualname__ = cls.__qualname__
+            Cls.__module__ = cls.__module__
+
         if reset_default_settings:
-            self.reset_default_settings(cls)
-        widget = cls.__new__(cls, signal_manager=self.signal_manager,
+            self.reset_default_settings(Cls)
+        widget = Cls.__new__(Cls, signal_manager=self.signal_manager,
                              stored_settings=stored_settings)
         widget.__init__()
         self.process_events()
         self.widgets.append(widget)
         return widget
 
     @staticmethod
```

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_context_handler.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_context_handler.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_control_getter.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_control_getter.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_gui.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_io.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_matplotlib_export.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_matplotlib_export.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_setting_provider.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_setting_provider.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_settings_handler.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_settings_handler.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/test_widget.py` & `orange-widget-base-4.9.0/orangewidget/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/tests/utils.py` & `orange-widget-base-4.9.0/orangewidget/tests/utils.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/PDFExporter.py` & `orange-widget-base-4.9.0/orangewidget/utils/PDFExporter.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/SVGExporter.py` & `orange-widget-base-4.9.0/orangewidget/utils/SVGExporter.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/__init__.py` & `orange-widget-base-4.9.0/orangewidget/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/_webview/helpers.js` & `orange-widget-base-4.9.0/orangewidget/utils/_webview/helpers.js`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/_webview/init-webengine-webchannel.js` & `orange-widget-base-4.9.0/orangewidget/utils/_webview/init-webengine-webchannel.js`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/buttons.py` & `orange-widget-base-4.9.0/orangewidget/utils/buttons.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/combobox.py` & `orange-widget-base-4.9.0/orangewidget/utils/combobox.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/concurrent.py` & `orange-widget-base-4.9.0/orangewidget/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/filedialogs.py` & `orange-widget-base-4.9.0/orangewidget/utils/filedialogs.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/itemmodels.py` & `orange-widget-base-4.9.0/orangewidget/utils/itemmodels.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/listview.py` & `orange-widget-base-4.9.0/orangewidget/utils/listview.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/matplotlib_export.py` & `orange-widget-base-4.9.0/orangewidget/utils/matplotlib_export.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/messages.py` & `orange-widget-base-4.9.0/orangewidget/utils/messages.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/messagewidget.py` & `orange-widget-base-4.9.0/orangewidget/utils/messagewidget.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/overlay.py` & `orange-widget-base-4.9.0/orangewidget/utils/overlay.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/progressbar.py` & `orange-widget-base-4.9.0/orangewidget/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/saveplot.py` & `orange-widget-base-4.9.0/orangewidget/utils/saveplot.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/signals.py` & `orange-widget-base-4.9.0/orangewidget/utils/signals.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_buttons.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_buttons.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_combobox.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_combobox.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_concurrent.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_filedialogs.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_filedialogs.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_itemmodels.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_itemmodels.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_listview.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_listview.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_messagewidget.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_messagewidget.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_overlay.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_overlay.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_save_plot.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_save_plot.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_signals.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_visual_settings_dlg.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_visual_settings_dlg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import unittest
 from unittest.mock import Mock
 
 from AnyQt.QtWidgets import QComboBox, QCheckBox, QSpinBox, QLineEdit
 
 from orangewidget.tests.base import GuiTest
-from orangewidget.utils.visual_settings_dlg import SettingsDialog
+from orangewidget.utils.visual_settings_dlg import SettingsDialog, FontList
 
 
 class TestSettingsDialog(GuiTest):
     def setUp(self):
         self.defaults = {
             "Box": {"Items": {
                 "P1": (["Foo", "Bar", "Baz"], "Bar"),
                 "P2": (range(3, 10, 2), 5),
                 "P3": (None, True),
                 "P4": (None, "Foo Bar"),
+                "P5": (FontList([".Foo", ".Bar"]), ".Foo"),
             }}
         }
         self.dlg = SettingsDialog(None, self.defaults)
 
     @property
     def dialog_controls(self):
         return self.dlg._SettingsDialog__controls
@@ -26,62 +27,71 @@
     def test_initialize(self):
         controls = self.dialog_controls
         self.assertEqual(len(controls), len(self.defaults["Box"]["Items"]))
         self.assertIsInstance(controls[("Box", "Items", "P1")][0], QComboBox)
         self.assertIsInstance(controls[("Box", "Items", "P2")][0], QSpinBox)
         self.assertIsInstance(controls[("Box", "Items", "P3")][0], QCheckBox)
         self.assertIsInstance(controls[("Box", "Items", "P4")][0], QLineEdit)
+        self.assertIsInstance(controls[("Box", "Items", "P5")][0], QComboBox)
 
     def test_changed_settings(self):
         self.dialog_controls[("Box", "Items", "P1")][0].setCurrentText("Foo")
         self.dialog_controls[("Box", "Items", "P2")][0].setValue(7)
         self.dialog_controls[("Box", "Items", "P3")][0].setChecked(False)
         self.dialog_controls[("Box", "Items", "P4")][0].setText("Foo Baz")
+        self.dialog_controls[("Box", "Items", "P5")][0].setCurrentIndex(1)
         changed = {("Box", "Items", "P1"): "Foo",
                    ("Box", "Items", "P2"): 7,
                    ("Box", "Items", "P3"): False,
-                   ("Box", "Items", "P4"): "Foo Baz"}
+                   ("Box", "Items", "P4"): "Foo Baz",
+                   ("Box", "Items", "P5"): ".Bar"}
         self.assertDictEqual(self.dlg.changed_settings, changed)
 
     def test_reset(self):
         ctrls = self.dialog_controls
         ctrls[("Box", "Items", "P1")][0].setCurrentText("Foo")
         ctrls[("Box", "Items", "P2")][0].setValue(7)
         ctrls[("Box", "Items", "P3")][0].setChecked(False)
         ctrls[("Box", "Items", "P4")][0].setText("Foo Baz")
+        self.dialog_controls[("Box", "Items", "P5")][0].setCurrentIndex(1)
 
         self.dlg._SettingsDialog__reset()
         self.assertDictEqual(self.dlg.changed_settings, {})
         self.assertEqual(ctrls[("Box", "Items", "P1")][0].currentText(), "Bar")
         self.assertEqual(ctrls[("Box", "Items", "P2")][0].value(), 5)
         self.assertTrue(ctrls[("Box", "Items", "P3")][0].isChecked())
         self.assertEqual(ctrls[("Box", "Items", "P4")][0].text(), "Foo Bar")
+        self.assertEqual(ctrls[("Box", "Items", "P5")][0].currentText(), "Foo")
 
     def test_setting_changed(self):
         handler = Mock()
         self.dlg.setting_changed.connect(handler)
         self.dialog_controls[("Box", "Items", "P1")][0].setCurrentText("Foo")
         handler.assert_called_with(('Box', 'Items', 'P1'), "Foo")
         self.dialog_controls[("Box", "Items", "P2")][0].setValue(7)
         handler.assert_called_with(('Box', 'Items', 'P2'), 7)
         self.dialog_controls[("Box", "Items", "P3")][0].setChecked(False)
         handler.assert_called_with(('Box', 'Items', 'P3'), False)
         self.dialog_controls[("Box", "Items", "P4")][0].setText("Foo Baz")
         handler.assert_called_with(('Box', 'Items', 'P4'), "Foo Baz")
+        self.dialog_controls[("Box", "Items", "P5")][0].setCurrentIndex(1)
+        handler.assert_called_with(('Box', 'Items', 'P5'), ".Bar")
 
     def test_apply_settings(self):
         changed = [(("Box", "Items", "P1"), "Foo"),
                    (("Box", "Items", "P2"), 7),
                    (("Box", "Items", "P3"), False),
-                   (("Box", "Items", "P4"), "Foo Baz")]
+                   (("Box", "Items", "P4"), "Foo Baz"),
+                   (("Box", "Items", "P5"), ".Bar")]
         self.dlg.apply_settings(changed)
         ctrls = self.dialog_controls
         self.assertEqual(ctrls[("Box", "Items", "P1")][0].currentText(), "Foo")
         self.assertEqual(ctrls[("Box", "Items", "P2")][0].value(), 7)
         self.assertFalse(ctrls[("Box", "Items", "P3")][0].isChecked())
         self.assertEqual(ctrls[("Box", "Items", "P4")][0].text(), "Foo Baz")
+        self.assertEqual(ctrls[("Box", "Items", "P5")][0].currentText(), "Bar")
         self.assertDictEqual(self.dlg.changed_settings,
                              {k: v for k, v in changed})
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_webview.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_webview.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/tests/test_widgetpreview.py` & `orange-widget-base-4.9.0/orangewidget/utils/tests/test_widgetpreview.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/visual_settings_dlg.py` & `orange-widget-base-4.9.0/orangewidget/utils/visual_settings_dlg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import sys
 from typing import List, Iterable, Tuple, Callable, Union, Dict
 from functools import singledispatch
 
-from AnyQt.QtCore import Qt, pyqtSignal as Signal, QStringListModel
+from AnyQt.QtCore import Qt, pyqtSignal as Signal, QStringListModel, \
+    QAbstractItemModel
 from AnyQt.QtWidgets import QDialog, QVBoxLayout, QComboBox, QCheckBox, \
-    QDialogButtonBox, QSpinBox, QWidget, QGroupBox, QApplication, \
-    QFormLayout, QLineEdit
+    QDialogButtonBox, QSpinBox, QWidget, QApplication, QFormLayout, QLineEdit
 
 from orangewidget import gui
 from orangewidget.utils.combobox import _ComboBoxListDelegate
-from orangewidget.utils.itemmodels import PyListModel
 from orangewidget.widget import OWBaseWidget
 
 KeyType = Tuple[str, str, str]
 ValueType = Union[str, int, bool]
 ValueRangeType = Union[Iterable, None]
 SettingsType = Dict[str, Tuple[ValueRangeType, ValueType]]
 
@@ -169,15 +168,15 @@
     class FontModel(QStringListModel):
         def data(self, index, role=Qt.DisplayRole):
             if role == Qt.AccessibleDescriptionRole \
                     and super().data(index, Qt.DisplayRole) == "":
                 return "separator"
 
             value = super().data(index, role)
-            if role in (Qt.DisplayRole, Qt.EditRole) and value.startswith("."):
+            if role == Qt.DisplayRole and value.startswith("."):
                 value = value[1:]
             return value
 
         def flags(self, index):
             if index.data(Qt.DisplayRole) == "separator":
                 return Qt.NoItemFlags
             else:
@@ -218,15 +217,18 @@
 @singledispatch
 def _set_control_value(*_):
     raise NotImplementedError
 
 
 @_set_control_value.register(QComboBox)
 def _(combo: QComboBox, value: str):
-    combo.setCurrentText(value)
+    model: QAbstractItemModel = combo.model()
+    values = [model.data(model.index(i, 0), role=Qt.EditRole)
+              for i in range(model.rowCount())]
+    combo.setCurrentIndex(values.index(value))
 
 
 @_set_control_value.register(QSpinBox)
 def _(spin: QSpinBox, value: int):
     spin.setValue(value)
```

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/webview.py` & `orange-widget-base-4.9.0/orangewidget/utils/webview.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/utils/widgetpreview.py` & `orange-widget-base-4.9.0/orangewidget/utils/widgetpreview.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/widget.py` & `orange-widget-base-4.9.0/orangewidget/widget.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/workflow/config.py` & `orange-widget-base-4.9.0/orangewidget/workflow/config.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/workflow/discovery.py` & `orange-widget-base-4.9.0/orangewidget/workflow/discovery.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/workflow/errorreporting.py` & `orange-widget-base-4.9.0/orangewidget/workflow/errorreporting.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/workflow/mainwindow.py` & `orange-widget-base-4.9.0/orangewidget/workflow/mainwindow.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/workflow/tests/test_widgetsscheme.py` & `orange-widget-base-4.9.0/orangewidget/workflow/tests/test_widgetsscheme.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/orangewidget/workflow/widgetsscheme.py` & `orange-widget-base-4.9.0/orangewidget/workflow/widgetsscheme.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/pylintrc` & `orange-widget-base-4.9.0/pylintrc`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/scripts/create_changelog.sh` & `orange-widget-base-4.9.0/scripts/create_changelog.sh`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/scripts/create_widget_catalog.py` & `orange-widget-base-4.9.0/scripts/create_widget_catalog.py`

 * *Files identical despite different names*

### Comparing `orange-widget-base-4.8.1/setup.py` & `orange-widget-base-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 
 import os
 import subprocess
 from setuptools import setup, find_packages, Command
 
 NAME = 'orange-widget-base'
-VERSION = '4.8.1'
+VERSION = '4.9.0'
 ISRELEASED = True
 # full version identifier including a git revision identifier for development
 # build/releases (this is filled/updated in `write_version_py`)
 FULLVERSION = VERSION
 
 DESCRIPTION = 'Base Widget for Orange Canvas'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
```

