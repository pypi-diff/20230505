# Comparing `tmp/aqtinstall-3.1.5.tar.gz` & `tmp/aqtinstall-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtinstall-3.1.5.tar", last modified: Thu Mar 30 14:08:01 2023, max compression
+gzip compressed data, was "aqtinstall-3.1.6.tar", last modified: Thu May  4 23:47:10 2023, max compression
```

## Comparing `aqtinstall-3.1.5.tar` & `aqtinstall-3.1.6.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.811876 aqtinstall-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-03-30 14:08:01.811876 aqtinstall-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8587 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.791875 aqtinstall-3.1.5/aqt/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25241 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/archives.py
--rw-r--r--   0 runner    (1001) docker     (122)    26266 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/combinations.json
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    19294 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    56222 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/installer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/logging.ini
--rw-r--r--   0 runner    (1001) docker     (122)    42338 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    13217 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/settings.ini
--rw-r--r--   0 runner    (1001) docker     (122)    15062 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/aqt/updater.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.791875 aqtinstall-3.1.5/aqtinstall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqtinstall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3909 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqtinstall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqtinstall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqtinstall.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqtinstall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-03-30 14:08:01.000000 aqtinstall-3.1.5/aqtinstall.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.795875 aqtinstall-3.1.5/ci/
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/accelbubble.7z
--rw-r--r--   0 runner    (1001) docker     (122)    16872 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/generate_azure_pipelines_matrices.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/generate_combinations.py
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/helloworld.7z
--rw-r--r--   0 runner    (1001) docker     (122)  1213852 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/jom_1_1_3.zip
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/logging.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/openglwindow.7z
--rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/openglwindow_qt6.7z
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/redditclient.7z
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/settings.ini
--rw-r--r--   0 runner    (1001) docker     (122)    18931 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/ci/steps.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.799875 aqtinstall-3.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     5907 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5708 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/CONTRIBUTE.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/SECURITY.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)    32418 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9830 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6244 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)    26591 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.787874 aqtinstall-3.1.5/docs/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.787874 aqtinstall-3.1.5/docs/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.799875 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     8165 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/SECURITY.po
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/authors.po
--rw-r--r--   0 runner    (1001) docker     (122)    41059 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/changes.po
--rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/cli.po
--rw-r--r--   0 runner    (1001) docker     (122)    14457 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/configuration.po
--rw-r--r--   0 runner    (1001) docker     (122)    46696 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/getting_started.po
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/installation.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.803875 aqtinstall-3.1.5/docs/locale/pot/
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/CODE_OF_CONDUCT.pot
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/CONTRIBUTE.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/SECURITY.pot
--rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/authors.pot
--rw-r--r--   0 runner    (1001) docker     (122)    40934 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/changes.pot
--rw-r--r--   0 runner    (1001) docker     (122)    20318 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/cli.pot
--rw-r--r--   0 runner    (1001) docker     (122)     7649 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/configuration.pot
--rw-r--r--   0 runner    (1001) docker     (122)    22725 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/getting_started.pot
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/index.pot
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/locale/pot/installation.pot
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)    25779 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/docs/previous_changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6004 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 14:08:01.811876 aqtinstall-3.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.803875 aqtinstall-3.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.811876 aqtinstall-3.1.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/linux-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    18093 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/linux-android.html
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/linux-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    30760 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/linux-desktop.html
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    16521 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-android.html
--rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_cmake-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_cmake-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_ifw-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_ifw-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtcreator-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtcreator-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtdesignstudio-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtdesignstudio-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)    28650 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-desktop.html
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-ios-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    11401 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mac-ios.html
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mirror-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    19653 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mirror-first-td.html
--rw-r--r--   0 runner    (1001) docker     (122)    17200 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mirror-pre-a.html
--rw-r--r--   0 runner    (1001) docker     (122)    23047 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mirror-table-before-pre-a.html
--rw-r--r--   0 runner    (1001) docker     (122)    76947 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/mirror-tag-in-a.html
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/settings.ini
--rw-r--r--   0 runner    (1001) docker     (122)    12460 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/settings_no_concurrency.ini
--rw-r--r--   0 runner    (1001) docker     (122)    79658 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5140-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    72606 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5140-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5140-wasm-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    16692 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5140-wasm-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5150-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)   120616 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5150-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5152-src-doc-example-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    18932 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-5152-src-doc-example-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)    35906 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-620-android-armv7-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-620-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    84709 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-620-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-650-wasm-multi-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    14238 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-650-wasm-multi-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-650-wasm-single-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    14534 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-650-wasm-single-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    16533 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-android.html
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     6580 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-desktop-tools-mingw-updates.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-desktop-tools-qtcreator-updates.xml
--rw-r--r--   0 runner    (1001) docker     (122)     6115 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-desktop-tools_vcredist-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-desktop-tools_vcredist-update.xml
--rw-r--r--   0 runner    (1001) docker     (122)    30718 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-desktop.html
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-winrt-expect.json
--rw-r--r--   0 runner    (1001) docker     (122)    10501 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/data/windows-winrt.html
--rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_archives.py
--rw-r--r--   0 runner    (1001) docker     (122)    19640 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_doc_archives.py
--rw-r--r--   0 runner    (1001) docker     (122)    15284 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    62437 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)    50103 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tests/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 14:08:01.811876 aqtinstall-3.1.5/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tools/build_standalone.py
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-30 14:07:42.000000 aqtinstall-3.1.5/tools/launch_aqt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8587 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.848619 aqtinstall-3.1.6/aqt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25241 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/archives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26751 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/combinations.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19294 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56222 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/installer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    42338 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13217 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    15062 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/aqt/updater.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.848619 aqtinstall-3.1.6/aqtinstall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9826 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3909 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-04 23:47:10.000000 aqtinstall-3.1.6/aqtinstall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.852620 aqtinstall-3.1.6/ci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/accelbubble.7z
+-rw-r--r--   0 runner    (1001) docker     (122)    16872 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/generate_azure_pipelines_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/generate_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/helloworld.7z
+-rw-r--r--   0 runner    (1001) docker     (122)  1213852 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/jom_1_1_3.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/openglwindow.7z
+-rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/openglwindow_qt6.7z
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/redditclient.7z
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    18931 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/ci/steps.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.856620 aqtinstall-3.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5708 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/CONTRIBUTE.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/SECURITY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    32418 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9830 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6244 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    26591 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.844619 aqtinstall-3.1.6/docs/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.844619 aqtinstall-3.1.6/docs/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.860620 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     8165 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/SECURITY.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/authors.po
+-rw-r--r--   0 runner    (1001) docker     (122)    41059 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/changes.po
+-rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/cli.po
+-rw-r--r--   0 runner    (1001) docker     (122)    14457 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/configuration.po
+-rw-r--r--   0 runner    (1001) docker     (122)    46696 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/getting_started.po
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/installation.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.864621 aqtinstall-3.1.6/docs/locale/pot/
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/CODE_OF_CONDUCT.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/CONTRIBUTE.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/SECURITY.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/authors.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    40934 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/changes.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    20318 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/cli.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     7649 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/configuration.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    22725 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/getting_started.pot
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/index.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/locale/pot/installation.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)    25779 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/docs/previous_changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6004 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.864621 aqtinstall-3.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    18093 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-android.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    30760 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/linux-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16521 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-android.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_cmake-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_cmake-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_ifw-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_ifw-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)    28650 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-ios-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    11401 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mac-ios.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    19653 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-first-td.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17200 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-pre-a.html
+-rw-r--r--   0 runner    (1001) docker     (122)    23047 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-table-before-pre-a.html
+-rw-r--r--   0 runner    (1001) docker     (122)    76947 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/mirror-tag-in-a.html
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    12460 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/settings_no_concurrency.ini
+-rw-r--r--   0 runner    (1001) docker     (122)    79658 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    72606 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-wasm-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16692 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5140-wasm-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5150-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)   120616 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5150-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    18932 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)    35906 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-620-android-armv7-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-620-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    84709 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-620-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-multi-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    14238 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-multi-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-single-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    14534 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-650-wasm-single-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16533 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-android.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6580 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools-mingw-updates.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools-qtcreator-updates.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     6115 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-update.xml
+-rw-r--r--   0 runner    (1001) docker     (122)    30718 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-winrt-expect.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10501 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/data/windows-winrt.html
+-rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19640 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_doc_archives.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15284 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62437 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50103 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 23:47:10.876622 aqtinstall-3.1.6/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tools/build_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-04 23:46:50.000000 aqtinstall-3.1.6/tools/launch_aqt.py
```

### Comparing `aqtinstall-3.1.5/LICENSE` & `aqtinstall-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/MANIFEST.in` & `aqtinstall-3.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/PKG-INFO` & `aqtinstall-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtinstall
-Version: 3.1.5
+Version: 3.1.6
 Summary: Another unofficial Qt installer
 Author-email: Hiroshi Miura <miurahr@linux.com>
 License: MIT License
 Project-URL: Documentation, https://aqtinstall.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/miurahr/aqtinstall/issues
 Project-URL: Wiki, https://github.com/miurahr/aqtinstall/wiki
 Project-URL: Source, https://github.com/miurahr/aqtinstall
```

### Comparing `aqtinstall-3.1.5/README.rst` & `aqtinstall-3.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/__init__.py` & `aqtinstall-3.1.6/aqt/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/__main__.py` & `aqtinstall-3.1.6/aqt/__main__.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/archives.py` & `aqtinstall-3.1.6/aqt/archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/combinations.json` & `aqtinstall-3.1.6/aqt/combinations.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996590909090909%*

 * *Differences: {'0': "{'tools': {insert: [(9, OrderedDict([('arch', 'qt.tools.opensslv3.src'), ('os_name', "*

 * *      "'linux'), ('target', 'desktop'), ('tool_name', 'tools_opensslv3_src')])), (62, "*

 * *      "OrderedDict([('arch', 'qt.tools.opensslv3.src'), ('os_name', 'windows'), ('target', "*

 * *      "'desktop'), ('tool_name', 'tools_opensslv3_src')])), (63, OrderedDict([('arch', "*

 * *      "'qt.tools.opensslv3.win_x64'), ('os_name', 'windows'), ('target', 'desktop'), ('tool_name', "*

 * *      "'tools_opensslv3_x64')]))]}}"}*

```diff
@@ -597,14 +597,20 @@
             {
                 "arch": "qt.tools.openssl.gcc_64",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_openssl_x64"
             },
             {
+                "arch": "qt.tools.opensslv3.src",
+                "os_name": "linux",
+                "target": "desktop",
+                "tool_name": "tools_opensslv3_src"
+            },
+            {
                 "arch": "qt.tools.qt3dstudio",
                 "os_name": "linux",
                 "target": "desktop",
                 "tool_name": "tools_qt3dstudio"
             },
             {
                 "arch": "qt.tools.qtcreator",
@@ -909,14 +915,26 @@
             {
                 "arch": "qt.tools.openssl.win_x86",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_openssl_x86"
             },
             {
+                "arch": "qt.tools.opensslv3.src",
+                "os_name": "windows",
+                "target": "desktop",
+                "tool_name": "tools_opensslv3_src"
+            },
+            {
+                "arch": "qt.tools.opensslv3.win_x64",
+                "os_name": "windows",
+                "target": "desktop",
+                "tool_name": "tools_opensslv3_x64"
+            },
+            {
                 "arch": "qt.tools.qt3dstudio",
                 "os_name": "windows",
                 "target": "desktop",
                 "tool_name": "tools_qt3dstudio"
             },
             {
                 "arch": "qt.tools.qtcreator",
```

### Comparing `aqtinstall-3.1.5/aqt/exceptions.py` & `aqtinstall-3.1.6/aqt/exceptions.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/helper.py` & `aqtinstall-3.1.6/aqt/helper.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/installer.py` & `aqtinstall-3.1.6/aqt/installer.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/logging.ini` & `aqtinstall-3.1.6/aqt/logging.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/metadata.py` & `aqtinstall-3.1.6/aqt/metadata.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/settings.ini` & `aqtinstall-3.1.6/aqt/settings.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqt/updater.py` & `aqtinstall-3.1.6/aqt/updater.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/aqtinstall.egg-info/PKG-INFO` & `aqtinstall-3.1.6/aqtinstall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtinstall
-Version: 3.1.5
+Version: 3.1.6
 Summary: Another unofficial Qt installer
 Author-email: Hiroshi Miura <miurahr@linux.com>
 License: MIT License
 Project-URL: Documentation, https://aqtinstall.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/miurahr/aqtinstall/issues
 Project-URL: Wiki, https://github.com/miurahr/aqtinstall/wiki
 Project-URL: Source, https://github.com/miurahr/aqtinstall
```

### Comparing `aqtinstall-3.1.5/aqtinstall.egg-info/SOURCES.txt` & `aqtinstall-3.1.6/aqtinstall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/accelbubble.7z` & `aqtinstall-3.1.6/ci/accelbubble.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/generate_azure_pipelines_matrices.py` & `aqtinstall-3.1.6/ci/generate_azure_pipelines_matrices.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/generate_combinations.py` & `aqtinstall-3.1.6/ci/generate_combinations.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/jom_1_1_3.zip` & `aqtinstall-3.1.6/ci/jom_1_1_3.zip`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/logging.ini` & `aqtinstall-3.1.6/ci/logging.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/openglwindow.7z` & `aqtinstall-3.1.6/ci/openglwindow.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/openglwindow_qt6.7z` & `aqtinstall-3.1.6/ci/openglwindow_qt6.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/redditclient.7z` & `aqtinstall-3.1.6/ci/redditclient.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/settings.ini` & `aqtinstall-3.1.6/ci/settings.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/ci/steps.yml` & `aqtinstall-3.1.6/ci/steps.yml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/CHANGELOG.rst` & `aqtinstall-3.1.6/docs/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,29 @@
 ==========
 
 All notable changes to this project will be documented in this file.
 
 `Unreleased`_
 =============
 
+`v3.1.6`_ (4, May, 2023)
+========================
+
+Added
+-----
+* Add opensslv3 as known module (#674)
+* Add code signature for standalone binary
+
 `v3.1.5`_ (30, Mar. 2023)
 =========================
 
 Fixed
 -----
 * Fix failure to install Qt 6.4.3 source and docs on Windows(#665)
-* Fix failed .tar.gz extraction in `install-src` and `install-doc`(#663)
+* Fix failed .tar.gz extraction in ``install-src`` and ``install-doc`` (#663)
 
 `v3.1.4`_ (25, Mar. 2023)
 =========================
 
 Changed
 -------
 * Add Qt 6.4.3 as known version(#661)
@@ -215,15 +223,16 @@
 --------
 * Use secrets for secure random numbers(#498)
 * Use defusedxml to parse Updates.xml file to avoid attack(#498)
 * Improve get_hash function(#504)
 * Check Update.xml file with SHA256 hash (#493)
 
 
-.. _Unreleased: https://github.com/miurahr/aqtinstall/compare/v3.1.5...HEAD
+.. _Unreleased: https://github.com/miurahr/aqtinstall/compare/v3.1.6...HEAD
+.. _v3.1.6: https://github.com/miurahr/aqtinstall/compare/v3.1.5...v3.1.6
 .. _v3.1.5: https://github.com/miurahr/aqtinstall/compare/v3.1.4...v3.1.5
 .. _v3.1.4: https://github.com/miurahr/aqtinstall/compare/v3.1.3...v3.1.4
 .. _v3.1.3: https://github.com/miurahr/aqtinstall/compare/v3.1.2...v3.1.3
 .. _v3.1.2: https://github.com/miurahr/aqtinstall/compare/v3.1.1...v3.1.2
 .. _v3.1.1: https://github.com/miurahr/aqtinstall/compare/v3.1.0...v3.1.1
 .. _v3.1.0: https://github.com/miurahr/aqtinstall/compare/v3.0.2...v3.1.0
 .. _v3.0.2: https://github.com/miurahr/aqtinstall/compare/v3.0.1...v3.0.2
```

### Comparing `aqtinstall-3.1.5/docs/CODE_OF_CONDUCT.rst` & `aqtinstall-3.1.6/docs/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/CONTRIBUTE.rst` & `aqtinstall-3.1.6/docs/CONTRIBUTE.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/Makefile` & `aqtinstall-3.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/authors.rst` & `aqtinstall-3.1.6/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/cli.rst` & `aqtinstall-3.1.6/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/conf.py` & `aqtinstall-3.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/configuration.rst` & `aqtinstall-3.1.6/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/getting_started.rst` & `aqtinstall-3.1.6/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/installation.rst` & `aqtinstall-3.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/SECURITY.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/SECURITY.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/authors.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/authors.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/changes.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/changes.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/cli.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/cli.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/configuration.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/configuration.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/getting_started.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/getting_started.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/index.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/ja/LC_MESSAGES/installation.po` & `aqtinstall-3.1.6/docs/locale/ja/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/CODE_OF_CONDUCT.pot` & `aqtinstall-3.1.6/docs/locale/pot/CODE_OF_CONDUCT.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/CONTRIBUTE.pot` & `aqtinstall-3.1.6/docs/locale/pot/CONTRIBUTE.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/SECURITY.pot` & `aqtinstall-3.1.6/docs/locale/pot/SECURITY.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/authors.pot` & `aqtinstall-3.1.6/docs/locale/pot/authors.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/changes.pot` & `aqtinstall-3.1.6/docs/locale/pot/changes.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/cli.pot` & `aqtinstall-3.1.6/docs/locale/pot/cli.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/configuration.pot` & `aqtinstall-3.1.6/docs/locale/pot/configuration.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/getting_started.pot` & `aqtinstall-3.1.6/docs/locale/pot/getting_started.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/index.pot` & `aqtinstall-3.1.6/docs/locale/pot/index.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/locale/pot/installation.pot` & `aqtinstall-3.1.6/docs/locale/pot/installation.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/make.bat` & `aqtinstall-3.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/docs/previous_changes.rst` & `aqtinstall-3.1.6/docs/previous_changes.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/pyproject.toml` & `aqtinstall-3.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/linux-android-expect.json` & `aqtinstall-3.1.6/tests/data/linux-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/linux-android.html` & `aqtinstall-3.1.6/tests/data/linux-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/linux-desktop-expect.json` & `aqtinstall-3.1.6/tests/data/linux-desktop-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/linux-desktop.html` & `aqtinstall-3.1.6/tests/data/linux-desktop.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-android-expect.json` & `aqtinstall-3.1.6/tests/data/mac-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-android.html` & `aqtinstall-3.1.6/tests/data/mac-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-expect.json` & `aqtinstall-3.1.6/tests/data/mac-desktop-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-tools_cmake-update.xml` & `aqtinstall-3.1.6/tests/data/mac-desktop-tools_cmake-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-tools_ifw-update.xml` & `aqtinstall-3.1.6/tests/data/mac-desktop-tools_ifw-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtcreator-expect.json` & `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtcreator-update.xml` & `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtcreator-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtdesignstudio-expect.json` & `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop-tools_qtdesignstudio-update.xml` & `aqtinstall-3.1.6/tests/data/mac-desktop-tools_qtdesignstudio-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-desktop.html` & `aqtinstall-3.1.6/tests/data/mac-desktop.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-ios-expect.json` & `aqtinstall-3.1.6/tests/data/mac-ios-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mac-ios.html` & `aqtinstall-3.1.6/tests/data/mac-ios.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mirror-expect.json` & `aqtinstall-3.1.6/tests/data/mirror-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mirror-first-td.html` & `aqtinstall-3.1.6/tests/data/mirror-first-td.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mirror-pre-a.html` & `aqtinstall-3.1.6/tests/data/mirror-pre-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mirror-table-before-pre-a.html` & `aqtinstall-3.1.6/tests/data/mirror-table-before-pre-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/mirror-tag-in-a.html` & `aqtinstall-3.1.6/tests/data/mirror-tag-in-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/settings_no_concurrency.ini` & `aqtinstall-3.1.6/tests/data/settings_no_concurrency.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5140-expect.json` & `aqtinstall-3.1.6/tests/data/windows-5140-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5140-update.xml` & `aqtinstall-3.1.6/tests/data/windows-5140-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5140-wasm-update.xml` & `aqtinstall-3.1.6/tests/data/windows-5140-wasm-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5150-expect.json` & `aqtinstall-3.1.6/tests/data/windows-5150-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5150-update.xml` & `aqtinstall-3.1.6/tests/data/windows-5150-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5152-src-doc-example-expect.json` & `aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-5152-src-doc-example-update.xml` & `aqtinstall-3.1.6/tests/data/windows-5152-src-doc-example-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-620-android-armv7-update.xml` & `aqtinstall-3.1.6/tests/data/windows-620-android-armv7-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-620-expect.json` & `aqtinstall-3.1.6/tests/data/windows-620-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-620-update.xml` & `aqtinstall-3.1.6/tests/data/windows-620-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-650-wasm-multi-update.xml` & `aqtinstall-3.1.6/tests/data/windows-650-wasm-multi-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-650-wasm-single-update.xml` & `aqtinstall-3.1.6/tests/data/windows-650-wasm-single-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-android-expect.json` & `aqtinstall-3.1.6/tests/data/windows-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-android.html` & `aqtinstall-3.1.6/tests/data/windows-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-desktop-expect.json` & `aqtinstall-3.1.6/tests/data/windows-desktop-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-desktop-tools-mingw-updates.xml` & `aqtinstall-3.1.6/tests/data/windows-desktop-tools-mingw-updates.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-desktop-tools-qtcreator-updates.xml` & `aqtinstall-3.1.6/tests/data/windows-desktop-tools-qtcreator-updates.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-desktop-tools_vcredist-expect.json` & `aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-desktop-tools_vcredist-update.xml` & `aqtinstall-3.1.6/tests/data/windows-desktop-tools_vcredist-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-desktop.html` & `aqtinstall-3.1.6/tests/data/windows-desktop.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-winrt-expect.json` & `aqtinstall-3.1.6/tests/data/windows-winrt-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/data/windows-winrt.html` & `aqtinstall-3.1.6/tests/data/windows-winrt.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_archives.py` & `aqtinstall-3.1.6/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_cli.py` & `aqtinstall-3.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_connection.py` & `aqtinstall-3.1.6/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_doc_archives.py` & `aqtinstall-3.1.6/tests/test_doc_archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_helper.py` & `aqtinstall-3.1.6/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_install.py` & `aqtinstall-3.1.6/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_list.py` & `aqtinstall-3.1.6/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tests/test_updater.py` & `aqtinstall-3.1.6/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.5/tools/build_standalone.py` & `aqtinstall-3.1.6/tools/build_standalone.py`

 * *Files identical despite different names*

