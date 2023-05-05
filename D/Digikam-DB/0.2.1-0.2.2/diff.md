# Comparing `tmp/Digikam-DB-0.2.1.tar.gz` & `tmp/Digikam-DB-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digikam-DB-0.2.1.tar", last modified: Fri Apr  7 16:47:15 2023, max compression
+gzip compressed data, was "Digikam-DB-0.2.2.tar", last modified: Fri May  5 18:51:55 2023, max compression
```

## Comparing `Digikam-DB-0.2.1.tar` & `Digikam-DB-0.2.2.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.700128 Digikam-DB-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.700128 Digikam-DB-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/CHANGELOG.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/Digikam_DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/digikamdb/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/digikamdb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/albumroots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/image_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/image_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    23386 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/_ext/_sqla.py
--rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/_ext/digikam4.db
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api_albums.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api_images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api_tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/digikamrc.mysql
--rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/digikamrc.mysql-internal
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/digikamrc.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/empty.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/empty.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/testdb.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/testdb.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/digikamrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/imagedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/newdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.167555 Digikam-DB-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.171555 Digikam-DB-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/CHANGELOG.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.171555 Digikam-DB-0.2.2/Digikam_DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:51:54.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.175555 Digikam-DB-0.2.2/digikamdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/digikamdb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/albumroots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/image_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/image_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.175555 Digikam-DB-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.179555 Digikam-DB-0.2.2/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/_ext/_sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/_ext/digikam4.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api_albums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api_images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.179555 Digikam-DB-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/digikamrc.mysql
+-rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/digikamrc.mysql-internal
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/digikamrc.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty-15.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty-15.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/testdb.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/testdb.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/digikamrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/imagedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/newdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/sqlite.py
```

### Comparing `Digikam-DB-0.2.1/.github/workflows/release.yml` & `Digikam-DB-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/.github/workflows/test.yml` & `Digikam-DB-0.2.2/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -58,49 +58,70 @@
     name: Run Unit Tests
     needs:
     - check
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version:
+        python:
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
-        mysql-version:
+        mysql:
           - "mysql-8.0"
           - "mariadb-10.5"
           - "mariadb-10.6"
           - "mariadb-10.11"
+        sqlalchemy:
+          - "1.4"
+          - "2.0"
+        exclude:
+          - python:     "3.8"
+            mysql:      mariadb-10.11
+          - python:     "3.8"
+            sqlalchemy: "2.0"
+          - python:     "3.9"
+            mysql:      mariadb-10.11
+          - python:     "3.10"
+            mysql:      mariadb-10.5
+          - python:     "3.11"
+            mysql:      mariadb-10.5
+          - python:     "3.11"
+            sqlalchemy: "1.4"
     steps:
-    - uses: actions/checkout@v3
-      name: Checkout Git repository
+    - name: Checkout Git repository
+      uses: actions/checkout@v3
       with:
         fetch-depth:  0
-    - name: Set up MySQL ${{ matrix.mysql-version }}
+    - name: Set up MySQL ${{ matrix.mysql }}
       uses: shogo82148/actions-setup-mysql@v1
       with:
-        #distribution:   ${{ matrix.mysql-flavor }}
-        mysql-version:  ${{ matrix.mysql-version }}
+        mysql-version:  ${{ matrix.mysql }}
         root-password:  ${{ secrets.MYSQL_ROOT_PW }}
-    - name: Set up Python ${{ matrix.python-version }}
+        # log_bin causes errors when creating procedures,
+        # and we don't need replication.
+        my-cnf: |
+          disable_log_bin
+    - name: Set up Python ${{ matrix.python }}
       uses: actions/setup-python@v3
       with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
+        python-version: ${{ matrix.python }}
+    - name: Install Python packages
       run: |
+        # Install SQLAlchemy ${{ matrix.sqlalchemy }}
+        pip install sqlalchemy~=${{ matrix.sqlalchemy }}
         # There seems to be no easy way to install dependencies
         # from pyproject.toml, so we just install the package...
         pip install -e .[mysql]
         pip install coverage[toml]
     - name: Prepare database
       run: |
         # Prepare the MySQL database
-        mysql -u root -h 127.0.0.1 -p"${{ secrets.MYSQL_ROOT_PW }}" <<EOF
+        mysql -v -u root -h 127.0.0.1 -p"${{ secrets.MYSQL_ROOT_PW }}" <<EOF
         CREATE DATABASE digikam;
         CREATE USER digikam@localhost IDENTIFIED BY '${{ secrets.MYSQL_USER_PW }}';
         GRANT ALL PRIVILEGES ON digikam.* TO digikam@localhost;
         EOF
     - name: Prepare test configuration
       run: |
         # Generate test MySQL configuration
@@ -144,16 +165,16 @@
     
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10"]
     
     steps:
-    - uses: actions/checkout@v3
-      name: Checkout Git repository
+    - name: Checkout Git repository
+      uses: actions/checkout@v3
       with:
         fetch-depth:  0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -170,39 +191,40 @@
         coverage combine
         cp .coverage ..
     - name: Coverage report
       run: |
         # Run coverage report
         coverage report -m
   
-  publish_test:
+  packaging_test:
     
-    name: Publish to Test PyPi
+    name: Test Packaging
     needs:
     - build_and_test
     
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10"]
     
     steps:
-    - uses: actions/checkout@v3
-      name: Checkout Git repository
+    - name: Checkout Git repository
+      uses: actions/checkout@v3
       with:
         fetch-depth:  0
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Generate Packages
       run: |
         pip install build
         python -m build
     - name: Upload to test.pypi.org
+      if:   false
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository_url: https://test.pypi.org/legacy/
```

### Comparing `Digikam-DB-0.2.1/CHANGELOG.rst` & `Digikam-DB-0.2.2/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v0.2.2 (2023-??-??)
+--------------------
+*   Added support for MySQL without nested sets in `Tags` (DBVersion > 10)
+*   Raise ``DigikamVersionError`` when trying to access properties not supported
+    by the used database version.
+*   Added ``Album.modificationDate`` and ``AlbumRoot.caseSensitivity``
+
 v0.2.1 (2023-04-07)
 --------------------
 * Digikam.__init__: don't log sensitive data.
 * BasicProperties: added get method.
 * Imageinformation.orientation can be None.
 
 v0.2.0 (2023-04-03)
@@ -9,15 +16,15 @@
 * Changes may break existing code.
 * Image.caption returns string instead of tuple.
 * ExifMeteringMode: Fixed typo in CENTER_WEIGHTED_AVERAGE.
 
 v0.1.3 (2023-04-01)
 --------------------
 * Fixed exceptions when some ImageMetadata columns contain NULL.
-* Fixed column names in nestet tags check.
+* Fixed column names in nested tags check.
 
 v0.1.2 (2023-03-27)
 --------------------
 * Fixed SQLAlchemy 2.0 compatibility issues.
 
 v0.1.1 (2023-03-27)
 --------------------
```

### Comparing `Digikam-DB-0.2.1/Digikam_DB.egg-info/PKG-INFO` & `Digikam-DB-0.2.2/Digikam_DB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.2.1/Digikam_DB.egg-info/SOURCES.txt` & `Digikam-DB-0.2.2/Digikam_DB.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,11 +46,13 @@
 tests/mysql.py
 tests/newdata.py
 tests/sanity.py
 tests/sqlite.py
 tests/data/digikamrc.mysql
 tests/data/digikamrc.mysql-internal
 tests/data/digikamrc.sqlite
+tests/data/empty-15.sql.xz
+tests/data/empty-15.tar.xz
 tests/data/empty.sql.xz
 tests/data/empty.tar.xz
 tests/data/testdb.sql.xz
 tests/data/testdb.tar.gz
```

### Comparing `Digikam-DB-0.2.1/LICENSE` & `Digikam-DB-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/PKG-INFO` & `Digikam-DB-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.2.1/README.rst` & `Digikam-DB-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/digikamdb/albumroots.py` & `Digikam-DB-0.2.2/digikamdb/albumroots.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 import stat
 from typing import Iterable, List, Mapping, Optional
 
 from sqlalchemy.orm import relationship, validates
 
 from .table import DigikamTable
-from .exceptions import DigikamFileError
+from .exceptions import DigikamFileError, DigikamVersionError
 from .types import AlbumRootStatus as Status, AlbumRootType as Type
 
 
 log = logging.getLogger(__name__)
 
 
 def _albumroot_class(dk: 'Digikam') -> type:                # noqa: F821, C901
@@ -168,15 +168,15 @@
                         if mdev == 'UUID=' + uuid or mdev == dev:
                             path = mdir
                             break
             
             if vid.startswith('volumeid:?path='):
                 path = vid[15:]
             
-            if os.path.isdir(path):
+            if path is not None and os.path.isdir(path):
                 self._mountpoint = path
                 log.debug(
                     'Setting mountpoint for %s to %s',
                     self.identifier,
                     self._mountpoint
                 )
                 return path
@@ -204,14 +204,30 @@
                     if path in override['paths']:
                         log.debug('Overriding path')
                         return override['paths'][path]
                 
             return os.path.abspath(os.path.join(
                 self.mountpoint,
                 self.specificPath.lstrip('/')))
+        
+        @property
+        def caseSensitivity(self) -> bool:
+            """
+            Indicates if this album root is case sensitive.
+            
+            Raises:
+                DigikamVersionError:    If DBVersion < 16
+            
+            .. versionadded:: 0.2.2
+            """
+            if self.digikam.db_version < 16:
+                raise DigikamVersionError(
+                    'caseSensitivity is present in DBVersion >= 16'
+                )
+            return self._caseSensitivity != 0
     
     return AlbumRoot
 
 
 class AlbumRoots(DigikamTable):
     """
     Offers access to the album roots in the Digikam instance.
```

### Comparing `Digikam-DB-0.2.1/digikamdb/albums.py` & `Digikam-DB-0.2.2/digikamdb/albums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 """
 Digikam Albums
 """
 
 import logging
 import os
-from datetime import date
+from datetime import date, datetime
 from typing import List, Optional, Union
 
+from sqlalchemy import Column
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import MultipleResultsFound
 
 from .table import DigikamTable
-from .exceptions import DigikamDataIntegrityError
+from .exceptions import DigikamDataIntegrityError, DigikamVersionError
 
 
 log = logging.getLogger(__name__)
 
 
 def _album_class(dk: 'Digikam') -> type:                    # noqa: F821
     """
     Defines the Album class
     """
     
+    if not dk.is_mysql:
+        from sqlalchemy.dialects import sqlite
+    
     class Album(dk.base):
         """
         Represents a row in the table ``Albums``.
         
         See also:
             * Class :class:`~digikamdb.albums.Albums`
         """
 
         __tablename__ = 'Albums'
         
+        if (not dk.is_mysql) and (dk.db_version >= 14):
+            _modificationDate = Column(
+                'modificationDate',
+                sqlite.DATETIME(
+                    storage_format = '%(year)04d-%(month)02d-%(day)02dT%(hour)02d:%(minute)02d:%(second)02d',   # noqa: E501
+                    regexp = r'(\d+)-(\d+)-(\d+)T(\d+):(\d+):(\d+)')
+            )
+        
         _root = relationship(
             'AlbumRoot',
             primaryjoin = 'foreign(Album._albumRoot) == AlbumRoot._id',
             back_populates = '_albums')
         _iconObj = relationship(
             'Image',
             primaryjoin = 'foreign(Album._icon) == Image._id',
@@ -111,14 +123,30 @@
             """
             return self._collection
         
         @collection.setter
         def collection(self, value):
             self._collection = value
         
+        @property
+        def modificationDate(self) -> datetime:
+            """
+            The album's modification date (read-only)
+            
+            Raises:
+                DigikamVersionError:    If DBVersion < 14
+            
+            .. versionadded:: 0.2.2
+            """
+            if self.digikam.db_version < 14:
+                raise DigikamVersionError(
+                    'modificationDate is present in DBVersion >= 14'
+                )
+            return self._modificationDate
+        
         # Other properties and methods
         
         @property
         def abspath(self) -> str:
             """The album folder's absolute path (read-only)"""
             if self.relativePath == '/':
                 return self.root.abspath
```

### Comparing `Digikam-DB-0.2.1/digikamdb/conn.py` & `Digikam-DB-0.2.2/digikamdb/conn.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import logging
 import os
 import re
 from typing import Mapping, Optional, Union
 
-from sqlalchemy import create_engine
+from sqlalchemy import text, create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session, declarative_base
 from sqlalchemy.ext.declarative import DeferredReflection
 
 from .settings import Settings
 from .tags import Tags
 from .albumroots import AlbumRoots
@@ -86,14 +86,16 @@
                 self._engine = create_engine(
                     database,
                     future = True,
                     echo = sql_echo)
         else:
             raise TypeError('Database specification must be Engine or str')
         
+        self._db_version = self._get_db_version()
+        
         self._session = Session(self._engine, future = True)
 
         self._base = self._digikamobject_class(declarative_base())
         
         self._settings  = Settings(self)
         self._tags      = Tags(self)
         self._albumRoots = AlbumRoots(self, override = root_override)
@@ -109,14 +111,40 @@
         db_pass = 'Database Password',
         db_port = 'Database Port',
         db_type = 'Database Type',
         db_user = 'Database Username',
         db_internal = 'Internal Database Server'
     )
     
+    def _get_db_version(self) -> int:
+        with self._engine.connect() as conn:
+            return int(
+                conn.execute(text(
+                    "SELECT value FROM Settings WHERE keyword = 'DBVersion'"
+                )).one().value
+            )
+    
+    @property
+    def db_version(self) -> int:
+        """
+        The Digikam database version
+        
+        .. versionadded:: 0.2.2
+        """
+        return self._db_version
+    
+    @property
+    def has_tags_nested_sets(self) -> bool:
+        """
+        Indicates if the ``Tags`` table has nested sets
+        
+        .. versionadded:: 0.2.2
+        """
+        return self.is_mysql and self.db_version <= 10
+    
     @property
     def base(self) -> type:
         """Base class for table-mapped classes"""
         return self._base
     
     @classmethod
     def db_from_config(cls, sql_echo = False) -> Engine:    # noqa: C901
@@ -254,15 +282,17 @@
     @property
     def session(self) -> Session:
         """The SQLAlchemy ORM session"""
         return self._session
     
     @property
     def is_mysql(self) -> bool:
-        """``True`` if database is MySQL"""
+        """
+        ``True`` if database is MySQL
+        """
         return (self._engine.dialect.name == 'mysql')
     
     def _digikamobject_class(self, base: type) -> type:
         """
         Defines the DigikamObject class
         
         Args:
```

### Comparing `Digikam-DB-0.2.1/digikamdb/exceptions.py` & `Digikam-DB-0.2.2/digikamdb/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,7 +55,12 @@
 
 class DigikamDataIntegrityError(DigikamError):
     """
     The database is in an inconsistent state.
     """
     pass
 
+class DigikamVersionError(DigikamError):
+    """
+    The requested property is not present in the used database version.
+    """
+
```

### Comparing `Digikam-DB-0.2.1/digikamdb/image_comments.py` & `Digikam-DB-0.2.2/digikamdb/image_comments.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/digikamdb/image_helpers.py` & `Digikam-DB-0.2.2/digikamdb/image_helpers.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/digikamdb/images.py` & `Digikam-DB-0.2.2/digikamdb/images.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from sqlalchemy.orm import relationship, validates
 
 from .table import DigikamTable
 from .properties import BasicProperties
 from .image_comments import ImageCaptions, ImageTitles
 from .image_helpers import ImageCopyright, ImageProperties, define_image_helper_tables
 from .types import ImageCategory as Category, ImageStatus as Status
+from .exceptions import DigikamVersionError
 
 
 log = logging.getLogger(__name__)
 
 
 def _image_class(dk: 'Digikam') -> type:                    # noqa: F821, C901
     """
@@ -413,16 +414,27 @@
         def uniqueHash(self) -> str:
             """The image's unique (MD5) hash (read-only)"""
             return self._uniqueHash
         
         @property
         def manualOrder(self) -> int:
             """
-            The image's manual order in its album (no setter)
+            The image's manual order in its album (read-only)
+            
+            Raises:
+                DigikamVersionError:    If DBVersion < 10
+            
+            .. versionchanged:: 0.2.2
+                Raises :exc:`DigikamVersionError` for low DB versions.
+            
             """
+            if self.digikam.db_version < 10:
+                raise DigikamVersionError(
+                    'manualOrder is present in DBVersion >= 10'
+                )
             return self._manualOrder
         
         # Other properties and members
         
         @property
         def abspath(self) -> str:
             """
```

### Comparing `Digikam-DB-0.2.1/digikamdb/properties.py` & `Digikam-DB-0.2.2/digikamdb/properties.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/digikamdb/settings.py` & `Digikam-DB-0.2.2/digikamdb/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Digikam settings class
     
     The Digikam settings can be accessed like a dict:
     
     .. code-block:: python
         
         dk = digikamdb.Digikam()
-        if 'DBVersion in dk.settings':
+        if 'DBVersion' in dk.settings:
             db_version = dk.settings['DBVersion']           # Get DB version
         dk.settings['databaseUserImageFormats'] = '-xcf'    # Exclude GIMP files
         for k in dk.settings:                               # Iterate over settings
             print(k, '=', dk.settings[k])
         for k, v in dk.settings.items():                    # Iterate over settings
             print(k, '=', v)
```

### Comparing `Digikam-DB-0.2.1/digikamdb/table.py` & `Digikam-DB-0.2.2/digikamdb/table.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/digikamdb/tags.py` & `Digikam-DB-0.2.2/digikamdb/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,16 @@
             *   On SQLite, tags at the top level have a ``pid == 0``,
                 and there is no row with ``id == 0``. There can be many
                 tags without a parent tag.
             *   On MySQL, there is a tag ``_Digikam_Root_Tag_`` with
                 ``id == 0`` and ``pid == -1``, and there is no tag with
                 ``id == -1``. All other tags are descendents of
                 ``_Digikam_Root_Tag_``.
-            *   On MySQL, the ``Tags`` table implements an additional
-                *nested sets* structure with columns ``lft`` and ``rgt``.
+            *   On MySQL with DBVersion <= 10, the ``Tags`` table implements an
+                additional *nested sets* structure with columns ``lft`` and ``rgt``.
 
         .. seealso::
             * Class :class:`~digikamdb.tags.Tags`
         """
         
         __tablename__ = 'Tags'
         __mapper_args__ = dk.base.__mapper_args__.copy()
@@ -81,17 +81,20 @@
             primaryjoin = 'foreign(ImageTags.c.tagid) == Tag._id',
             secondaryjoin = 'foreign(ImageTags.c.imageid) == Image._id',
             secondary = 'ImageTags',
             back_populates = '_tags',
             lazy = 'dynamic'
         )
         
-        #: Needed for nested sets operations
+        # Needed to determine if root tag exists
         _is_mysql = dk.is_mysql
         
+        #: Needed for nested sets operations
+        _has_nested_sets = dk.has_tags_nested_sets
+        
         #: Needed for Tagstree operations
         _session = dk.session
         
         @validates('_pid')
         def _check_pid(self, key: str, value: int) -> int:
             if value < 0:
                 raise DigikamAssignmentError('Tag parent id cannot be negative')
@@ -101,15 +104,15 @@
         
         def __repr__(self) -> str:
             return '<Digikam Tag (%s, %d, %d)>' % (self.name, self.id, self.pid)
         
         def __contains__(self, obj: 'Tag') -> bool:
             if not isinstance(obj, Tag):
                 raise TypeError('A tag can only contain other tags')
-            if self._is_mysql:
+            if self._has_nested_sets:
                 return self._lft < obj._lft and self._rgt > obj._rgt
             else:
                 return self.id in obj._ancestors
         
         @property
         def id(self) -> int:
             """The tag's id (read-only)"""
@@ -174,43 +177,49 @@
             
             Returns:
                 In SQLite, an unsorted list with the ancestor's ids.
                 In MySQL, a sorted list (top-down) with the ancestor objects.
             """
             log.debug('Getting ancestors for tag %d', self.id)
             
-            if self._is_mysql:
+            if self._has_nested_sets:
                 # MySQL
                 return self._session.scalars(
                     select(Tag)
                     .where(Tag._lft < self._lft, Tag._rgt > self._rgt)
                     .order_by(Tag._lft)
                 ).all()
             
-            # We're on SQLite
+            # We're on a newer DBVersion or on SQLite
+            if self._is_mysql:
+                min_pid = 0
+            else:
+                min_pid = 1
             return [
                 row._pid
                 for row in self._session.scalars(
                     select(self.digikam.tags.TagsTreeEntry).filter_by(_id = self.id)
                 )
-                if row._pid > 0
+                if row._pid >= min_pid
             ]
             
         # Other properties and methods
         
         # Since Digikam doesn't use a foreign key, this is a regular property.
         @property
         def parent(self) -> Optional['Tag']:                # noqa: F821
             """
             Returns the tag's parent object.
             
             Returns ``None`` for
             
             * the root tag on MySQL or
             * tags at top level on SQLite
+            
+            .. todo:: Check for fresh MySQL DB with DBversion > 10
             """
 
             # Tags without a parent
             if self._is_mysql:
                 if self.pid < 0:
                     return None
             else:
@@ -244,15 +253,15 @@
             if self.pid <= 0:
                 return self.name
             
             # No hierarchical name for internal tags:
             if 'internalTag' in self.properties:
                 return self.name
             
-            if self._is_mysql:
+            if self._has_nested_sets:
                 return '/'.join(
                     [t.name for t in self._ancestors if t.id > 0]
                 ) + '/' + self.name
             
             return self.parent.hierarchicalname() + '/' + self.name
         
         def _check(self):
@@ -385,25 +394,32 @@
             Class :class:`~digikamdb.tags.TagProperties`.
             """
             __tablename__ = 'TagProperties'
             
             _tagid = Column('tagid', Integer, primary_key = True)
             _property = Column('property', String, primary_key = True)
         
-        if not self._is_mysql:
+        self.TagProperty = TagProperty
+        
+        if not self.digikam.has_tags_nested_sets:
             class TagsTreeEntry(self.digikam.base):
-                """Class for the tags tree"""
+                """
+                Class for the tags tree
+                
+                This is a view on MySQL with DBVersion <= 10.
+                
+                .. versionchanged:: 0.2.2
+                    Also defined for MySQL.
+                """
                 __tablename__ = 'TagsTree'
                 
                 _id = Column('id', Integer, primary_key = True)
                 _pid = Column('pid', Integer, primary_key = True)
             
             self.TagsTreeEntry = TagsTreeEntry
-        
-        self.TagProperty = TagProperty
     
     def _before_insert(
         self,
         mapper: 'Mapper',                                   # noqa: F821
         connection: 'Connection',                           # noqa: F821
         instance: 'Tag'                                     # noqa: F821
     ):
@@ -502,27 +518,27 @@
     def setup(self):
         """
         Sets the event listeners for nested sets.
         
         Called by Digikam constructor.
         """
         
-        if self._is_mysql:
+        self._do_before_insert = False
+        self._do_before_update = False
+        self._do_after_delete = False
+        self._has_nested_sets = False
+        
+        if self.digikam.has_tags_nested_sets:
             self._do_before_insert = True
             self._do_before_update = True
             self._do_after_delete = True
 
             event.listen(self.Class, 'before_insert', self._before_insert)
             event.listen(self.Class, 'before_update', self._before_update)
             event.listen(self.Class, 'after_delete', self._after_delete)
-        
-        else:
-            self._do_before_insert = False
-            self._do_before_update = False
-            self._do_after_delete = False
     
     def __getitem__(self, key):
         if isinstance(key, str):
             if '/' in key:
                 name = key.split('/')[-1]
             else:
                 name = key
@@ -552,15 +568,16 @@
         return super().__getitem__(key)
 
     @property
     def _root(self) -> 'Tag':                               # noqa: F821
         """
         Returns the root tag when on MySQL.
         
-        Raises :exc:`~sqlalchemy.exc.NoResultError` in SQLite.
+        Raises:
+            DigikamObjectNotFound:  When called on SQLite.
         """
         try:
             return self._select(_pid = -1).one()
         except NoResultFound:
             raise DigikamObjectNotFound('No tag for pid=-1')
     
     def add(
@@ -629,23 +646,26 @@
         
         Checks that
         
         * each tag is among the children of its parent
         * each tag is contained in its ancestors
         * there are no circular parent-child relations
         * the nested sets and adjacency list structures are consistent
-          (MySQL only)
+          (MySQL with DBVersion <= 10 only)
         
         Raises:
             DigikamDataIntegrityError:  Table is in an inconsistent state.
+        
+        .. versionchanged:: 0.2.2
+            Do not check nested sets for DBVersion > 10
         """
 
         for tag in self:
             tag._check()
-        if self.Class._is_mysql:
+        if self.digikam.has_tags_nested_sets:
             self._root._check_nested_sets()
 
 
 def _tagproperty_class(dk: 'Digikam') -> type:              # noqa: F821
     """Defines the TagProperty class."""
     return dk.tags.TagProperty
```

### Comparing `Digikam-DB-0.2.1/digikamdb/types.py` & `Digikam-DB-0.2.2/digikamdb/types.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/Makefile` & `Digikam-DB-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/_ext/_sqla.py` & `Digikam-DB-0.2.2/docs/_ext/_sqla.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/_ext/digikam4.db` & `Digikam-DB-0.2.2/docs/_ext/digikam4.db`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/api.rst` & `Digikam-DB-0.2.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/api_albums.rst` & `Digikam-DB-0.2.2/docs/api_albums.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/api_images.rst` & `Digikam-DB-0.2.2/docs/api_images.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/conf.py` & `Digikam-DB-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/intro.rst` & `Digikam-DB-0.2.2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/docs/tutorial.rst` & `Digikam-DB-0.2.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/pyproject.toml` & `Digikam-DB-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/__init__.py` & `Digikam-DB-0.2.2/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 # Run SQLite before MySQL tests as they run faster
 from .sqlite import (                                       # noqa: F401
     SQLite_00_FromString as bSQLite_00_FromString,
     SQLite_01_SanityCheck as bSQLite_01_SanityCheck,
     SQLite_02_TestData as bSQLite_02_TestData,
     SQLite_03_CheckImageData as bSQLite_03_CheckImageData,
     SQLite_04_NewData as bSQLite_04_NewData,
+    SQLite_04a_NewData15 as bSQLite_04a_NewData15,
     SQLite_05_RootOverride_01 as bSQLite_05_RootOverride_01,
     SQLite_05_RootOverride_02 as bSQLite_05_RootOverride_02,
     SQLite_05_RootOverride_03 as bSQLite_05_RootOverride_03,
 )
 # Then, MySQL
 from .mysql import (                                        # noqa: F401
     MySQL_00_FromString as cMySQL_00_FromString,
     MySQL_01_SanityCheck as cMySQL_01_SanityCheck,
     MySQL_02_TestData as cMySQL_02_TestData,
     MySQL_03_CheckImageData as cMySQL_03_CheckImageData,
     MySQL_04_NewData as cMySQL_04_NewData,
+    MySQL_04a_NewData15 as cMySQL_04a_NewData15,
     MySQL_05_RootOverride_01 as cMySQL_05_RootOverride_01,
     MySQL_05_RootOverride_02 as cMySQL_05_RootOverride_02,
     MySQL_05_RootOverride_03 as cMySQL_05_RootOverride_03,
 )
 
 
 # Log with debug to test.log
```

### Comparing `Digikam-DB-0.2.1/tests/base.py` & `Digikam-DB-0.2.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/data/digikamrc.mysql` & `Digikam-DB-0.2.2/tests/data/digikamrc.mysql`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/data/digikamrc.mysql-internal` & `Digikam-DB-0.2.2/tests/data/digikamrc.mysql-internal`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/data/digikamrc.sqlite` & `Digikam-DB-0.2.2/tests/data/digikamrc.sqlite`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/data/empty.sql.xz` & `Digikam-DB-0.2.2/tests/data/empty.sql.xz`

 * *Files 15% similar despite different names*

#### empty.sql

```diff
@@ -349,14 +349,15 @@
 (14,	1,	'Color Label Black',	NULL,	NULL,	13,	14),
 (15,	1,	'Color Label White',	NULL,	NULL,	11,	12),
 (16,	1,	'Pick Label None',	NULL,	NULL,	9,	10),
 (17,	1,	'Pick Label Rejected',	NULL,	NULL,	7,	8),
 (18,	1,	'Pick Label Pending',	NULL,	NULL,	5,	6),
 (19,	1,	'Pick Label Accepted',	NULL,	NULL,	3,	4);
 
+DROP TABLE IF EXISTS `TagsTree`;
 DROP VIEW IF EXISTS `TagsTree`;
 CREATE TABLE `TagsTree` (`id` int(11), `pid` int(11));
 
 
 DROP TABLE IF EXISTS `VideoMetadata`;
 CREATE TABLE `VideoMetadata` (
   `imageid` bigint(20) NOT NULL,
```

### Comparing `Digikam-DB-0.2.1/tests/data/empty.tar.xz` & `Digikam-DB-0.2.2/tests/data/empty.tar.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/data/testdb.sql.xz` & `Digikam-DB-0.2.2/tests/data/testdb.sql.xz`

 * *Files 10% similar despite different names*

#### testdb.sql

```diff
@@ -429,14 +429,15 @@
 (21,	0,	'People',	NULL,	NULL,	12,	13),
 (22,	0,	'Normandy',	NULL,	NULL,	10,	11),
 (23,	0,	'Marina',	NULL,	NULL,	8,	9),
 (24,	0,	'Calvados',	NULL,	NULL,	6,	7),
 (25,	0,	'Darmstadt',	NULL,	NULL,	4,	5),
 (26,	0,	'Mathildenhöhe',	NULL,	NULL,	2,	3);
 
+DROP TABLE IF EXISTS `TagsTree`;
 DROP VIEW IF EXISTS `TagsTree`;
 CREATE TABLE `TagsTree` (`id` int(11), `pid` int(11));
 
 
 DROP TABLE IF EXISTS `VideoMetadata`;
 CREATE TABLE `VideoMetadata` (
   `imageid` bigint(20) NOT NULL,
```

### Comparing `Digikam-DB-0.2.1/tests/data/testdb.tar.gz` & `Digikam-DB-0.2.2/tests/data/testdb.tar.gz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/data.py` & `Digikam-DB-0.2.2/tests/data.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/digikamrc.py` & `Digikam-DB-0.2.2/tests/digikamrc.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/imagedata.py` & `Digikam-DB-0.2.2/tests/imagedata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/mysql.py` & `Digikam-DB-0.2.2/tests/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         elif cls.test_db_dump.endswith('bz2'):
             cat = 'bzcat'
         else:
             cat = 'cat'
         
         try:
             run(
-                '{4} {5} | mysql -h {0} -u {1} -p"{2}" {3}'.format(
+                '{4} {5} | mysql -v -h {0} -u {1} -p"{2}" {3}'.format(
                     mysql_data.db_host,
                     mysql_data.db_user,
                     mysql_data.db_pass,
                     mysql_data.db_name,
                     cat,
                     os.path.join(cls.datadir, cls.test_db_dump),
                 ),
@@ -141,16 +141,19 @@
                 capture_output = True
             )
         except CalledProcessError as e:
             # Replace password in command line
             e.cmd = e.cmd.replace(mysql_data.db_pass, 'XXX')
             # Raise another Exception to make stderr visible
             # in unittest output
+            log.error('Error: %s', e)
+            log.debug('STDOUT: %s', e.stdout.decode('utf-8'))
+            log.debug('STDERR: %s', e.stderr.decode('utf-8'))
             raise RuntimeError(e.stderr.decode('utf-8'))
-                
+        
         cls.mysql_db = 'mysql+pymysql://{0}:{1}@{2}/{3}'.format(
             mysql_data.db_user,
             mysql_data.db_pass,
             mysql_data.db_host,
             mysql_data.db_name,
         )
     
@@ -202,14 +205,21 @@
 class MySQL_04_NewData(MySQLTestBase, NewData):
     
     # Use empty database without root_override
     test_db_dump = 'empty.sql.xz'
     root_override = None
 
 
+class MySQL_04a_NewData15(MySQLTestBase, NewData):
+    
+    # Use empty database without root_override
+    test_db_dump = 'empty-15.sql.xz'
+    root_override = None
+
+
 class MySQL_05_RootOverride_01(MySQLTestBase, NewDataRoot):
     
     # Use empty database with empty root_override
     test_db_dump = 'empty.sql.xz'
     root_override = {}
```

### Comparing `Digikam-DB-0.2.1/tests/newdata.py` & `Digikam-DB-0.2.2/tests/newdata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/sanity.py` & `Digikam-DB-0.2.2/tests/sanity.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.1/tests/sqlite.py` & `Digikam-DB-0.2.2/tests/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,21 @@
 class SQLite_04_NewData(SQLiteTestBase, NewData):
     
     # Use empty database without root_override
     test_db = 'empty.tar.xz'
     root_override = None
 
 
+class SQLite_04a_NewData15(SQLiteTestBase, NewData):
+    
+    # Use empty database without root_override
+    test_db = 'empty-15.tar.xz'
+    root_override = None
+
+
 class SQLite_05_RootOverride_01(SQLiteTestBase, NewDataRoot):
     
     # Use empty database without root_override
     test_db = 'empty.tar.xz'
     root_override = {}
```

