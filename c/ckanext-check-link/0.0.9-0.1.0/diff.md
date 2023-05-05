# Comparing `tmp/ckanext-check-link-0.0.9.tar.gz` & `tmp/ckanext-check-link-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-check-link-0.0.9.tar", last modified: Fri Jul 22 01:13:04 2022, max compression
+gzip compressed data, was "ckanext-check-link-0.1.0.tar", last modified: Fri May  5 15:33:58 2023, max compression
```

## Comparing `ckanext-check-link-0.0.9.tar` & `ckanext-check-link-0.1.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.594330 ckanext-check-link-0.0.9/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      205 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3124 2022-07-22 01:13:04.594330 ckanext-check-link-0.0.9/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2466 2022-06-22 21:01:19.000000 ckanext-check-link-0.0.9/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-06-22 03:49:19.000000 ckanext-check-link-0.0.9/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/ckanext/check_link/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/ckanext/check_link/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/ckanext/check_link/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/ckanext/check_link/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2823 2022-07-22 01:06:12.000000 ckanext-check-link-0.0.9/ckanext/check_link/cli.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-06-22 00:21:09.000000 ckanext-check-link-0.0.9/ckanext/check_link/logic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/logic/action/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2022-06-22 03:49:19.000000 ckanext-check-link-0.0.9/ckanext/check_link/logic/action/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4945 2022-07-22 01:10:26.000000 ckanext-check-link-0.0.9/ckanext/check_link/logic/action/check.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3491 2022-07-19 22:06:23.000000 ckanext-check-link-0.0.9/ckanext/check_link/logic/action/report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3395 2022-07-22 01:03:17.000000 ckanext-check-link-0.0.9/ckanext/check_link/logic/schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.587664 ckanext-check-link-0.0.9/ckanext/check_link/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1804 2022-06-22 03:24:46.000000 ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-06-22 03:24:46.000000 ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1103 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2022-06-23 01:21:28.000000 ckanext-check-link-0.0.9/ckanext/check_link/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      138 2022-06-22 03:30:54.000000 ckanext-check-link-0.0.9/ckanext/check_link/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2391 2022-07-19 22:05:08.000000 ckanext-check-link-0.0.9/ckanext/check_link/model/report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      993 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.587664 ckanext-check-link-0.0.9/ckanext/check_link/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      889 2022-06-22 18:25:02.000000 ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      712 2022-06-22 18:25:09.000000 ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/base_admin.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1672 2022-06-22 19:07:04.000000 ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/report.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1538 2022-06-23 06:36:52.000000 ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/snippets/report_item.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-06-22 00:13:52.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      664 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-06-22 14:18:19.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/action/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-06-22 14:18:33.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/action/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3708 2022-07-19 23:36:58.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/action/test_check.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4018 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/action/test_report.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.590997 ckanext-check-link-0.0.9/ckanext/check_link/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-06-22 13:26:06.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1169 2022-06-23 01:21:48.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/model/test_report.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      209 2022-06-22 03:49:19.000000 ckanext-check-link-0.0.9/ckanext/check_link/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1753 2022-07-21 23:05:31.000000 ckanext-check-link-0.0.9/ckanext/check_link/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2022-07-22 01:13:04.594330 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3124 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       60 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2022-07-22 01:13:04.000000 ckanext-check-link-0.0.9/ckanext_check_link.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       27 2022-06-22 03:49:36.000000 ckanext-check-link-0.0.9/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1749 2022-07-22 01:13:04.594330 ckanext-check-link-0.0.9/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-06-22 03:49:19.000000 ckanext-check-link-0.0.9/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      205 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3125 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2466 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5887 2023-05-05 15:31:50.000000 ckanext-check-link-0.1.0/ckanext/check_link/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      383 2023-05-05 15:31:11.000000 ckanext-check-link-0.1.0/ckanext/check_link/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/logic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/logic/action/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      131 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/logic/action/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5377 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/logic/action/check.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3536 2022-08-25 20:38:04.000000 ckanext-check-link-0.1.0/ckanext/check_link/logic/action/report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1791 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3615 2022-08-25 23:59:09.000000 ckanext-check-link-0.1.0/ckanext/check_link/logic/schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.495017 ckanext-check-link-0.1.0/ckanext/check_link/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1804 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1103 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2365 2023-05-05 15:32:57.000000 ckanext-check-link-0.1.0/ckanext/check_link/model/report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1138 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.535017 ckanext-check-link-0.1.0/ckanext/check_link/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      889 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      712 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/base_admin.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2218 2023-05-05 15:06:35.000000 ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/report.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1538 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/snippets/report_item.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      578 2022-11-07 20:13:48.000000 ckanext-check-link-0.1.0/ckanext/check_link/templates/header.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext/check_link/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/action/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/action/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3675 2023-05-05 15:33:16.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/action/test_check.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4019 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/action/test_report.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext/check_link/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/model/test_report.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      210 2023-05-05 15:31:10.000000 ckanext-check-link-0.1.0/ckanext/check_link/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4051 2023-05-05 15:31:11.000000 ckanext-check-link-0.1.0/ckanext/check_link/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3125 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1886 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-05 15:33:58.000000 ckanext-check-link-0.1.0/ckanext_check_link.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4447 2023-05-05 15:32:15.000000 ckanext-check-link-0.1.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1553 2023-05-05 15:33:58.545017 ckanext-check-link-0.1.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-08-25 16:40:07.000000 ckanext-check-link-0.1.0/setup.py
```

### Comparing `ckanext-check-link-0.0.9/LICENSE` & `ckanext-check-link-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/PKG-INFO` & `ckanext-check-link-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ckanext-check-link
-Version: 0.0.9
+Version: 0.1.0
 Summary: Resource URL checker
 Home-page: https://github.com/DataShades/ckanext-check-link
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/DataShades/ckanext-check-link/workflows/Tests/badge.svg?branch=main)](https://github.com/DataShades/ckanext-check-link/actions)
 
 # ckanext-check-link
```

### Comparing `ckanext-check-link-0.0.9/README.md` & `ckanext-check-link-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/logic/action/check.py` & `ckanext-check-link-0.1.0/ckanext/check_link/logic/action/check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 from __future__ import annotations
+
 import logging
 from itertools import islice
 from typing import Any, Iterable
 
-import ckan.plugins.toolkit as tk
 from check_link import Link, check_all
+
+import ckan.plugins.toolkit as tk
 from ckan.lib.search.query import solr_literal
 from ckan.logic import validate
 
 from ckanext.toolbelt.decorators import Collector
 
 from .. import schema
 
+CONFIG_TIMEOUT = "ckanext.check_link.check.timeout"
+DEFAULT_TIMEOUT = 10
+
 log = logging.getLogger(__name__)
 action, get_actions = Collector("check_link").split()
 
 
 @action
 @validate(schema.url_check)
 def url_check(context, data_dict):
     tk.check_access("check_link_url_check", context, data_dict)
+    timeout: int = tk.asint(tk.config.get(CONFIG_TIMEOUT, DEFAULT_TIMEOUT))
+    links: list[Link] = []
+
+    kwargs: dict[str, Any] = data_dict["link_patch"]
+    kwargs.setdefault("timeout", timeout)
 
-    links = []
     for url in data_dict["url"]:
         try:
-            links.append(Link(url))
+            links.append(Link(url, **kwargs))
         except ValueError as e:
             if data_dict["skip_invalid"]:
                 log.debug("Skipping invalid url: %s", url)
             else:
                 raise tk.ValidationError({"url": ["Must be a valid URL"]}) from e
 
     reports = [
@@ -50,15 +59,17 @@
 
 @action
 @validate(schema.resource_check)
 def resource_check(context, data_dict):
     tk.check_access("check_link_resource_check", context, data_dict)
     resource = tk.get_action("resource_show")(context, data_dict)
 
-    result = tk.get_action("check_link_url_check")(context, {"url": [resource["url"]]})
+    result = tk.get_action("check_link_url_check")(
+        context, {"url": [resource["url"]], "link_patch": data_dict["link_patch"]}
+    )
 
     report = dict(
         result[0], resource_id=resource["id"], package_id=resource["package_id"]
     )
 
     if data_dict["save"]:
         _save_reports(context, [report], data_dict["clear_available"])
@@ -136,15 +147,22 @@
     ]
 
     if not pairs:
         return {"reports": []}
 
     patches, urls = zip(*pairs)
 
-    result = tk.get_action("check_link_url_check")(context, {"url": urls, "skip_invalid": data_dict["skip_invalid"]})
+    result = tk.get_action("check_link_url_check")(
+        context,
+        {
+            "url": urls,
+            "skip_invalid": data_dict["skip_invalid"],
+            "link_patch": data_dict["link_patch"],
+        },
+    )
 
     reports = [dict(report, **patch) for patch, report in zip(patches, result)]
     if data_dict["save"]:
         _save_reports(context, reports, data_dict["clear_available"])
 
     return {
         "reports": reports,
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/logic/action/report.py` & `ckanext-check-link-0.1.0/ckanext/check_link/logic/action/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     if "exclude_state" in data_dict:
         q = q.filter(Report.state.notin_(data_dict["exclude_state"]))
 
     if "include_state" in data_dict:
         q = q.filter(Report.state.in_(data_dict["include_state"]))
 
     count = q.count()
+    q = q.order_by(Report.created_at.desc())
     q = q.limit(data_dict["limit"]).offset(data_dict["offset"])
 
     return {
         "count": count,
         "results": [
             r.dictize(dict(context, include_resource=True, include_package=True))
             for r in q
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/logic/auth.py` & `ckanext-check-link-0.1.0/ckanext/check_link/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/logic/schema.py` & `ckanext-check-link-0.1.0/ckanext/check_link/logic/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,41 +7,51 @@
     json_list_or_string,
     default,
     convert_to_json_if_string,
     boolean_validator,
 ):
     return {
         "url": [not_missing, json_list_or_string],
-        "patch": [default("{}"), convert_to_json_if_string],
         "save": [default(False), boolean_validator],
         "clear_available": [default(False), boolean_validator],
         "skip_invalid": [default(False), boolean_validator],
+        "link_patch": [default("{}"), convert_to_json_if_string],
     }
 
 
 @validator_args
-def resource_check(not_missing, resource_id_exists, boolean_validator, default):
+def resource_check(
+    not_missing,
+    resource_id_exists,
+    boolean_validator,
+    default,
+    convert_to_json_if_string,
+):
     return {
         "id": [not_missing, resource_id_exists],
         "save": [default(False), boolean_validator],
         "clear_available": [default(False), boolean_validator],
+        "link_patch": [default("{}"), convert_to_json_if_string],
     }
 
 
 @validator_args
-def base_search_check(boolean_validator, default, int_validator):
+def base_search_check(
+    boolean_validator, default, int_validator, convert_to_json_if_string
+):
     return {
         "save": [default(False), boolean_validator],
         "clear_available": [default(False), boolean_validator],
         "skip_invalid": [default(False), boolean_validator],
         "include_drafts": [default(False), boolean_validator],
         # "include_deleted": [default(False), boolean_validator],
         "include_private": [default(False), boolean_validator],
         "start": [default(0), int_validator],
         "rows": [default(10), int_validator],
+        "link_patch": [default("{}"), convert_to_json_if_string],
     }
 
 
 @validator_args
 def package_check(not_missing, package_id_or_name_exists):
     return dict(base_search_check(), id=[not_missing, package_id_or_name_exists])
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/alembic.ini` & `ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/env.py` & `ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py` & `ckanext-check-link-0.1.0/ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/model/report.py` & `ckanext-check-link-0.1.0/ckanext/check_link/model/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, Iterable, Optional
+from typing import Any, Optional
 
-import ckan.model as model
-from ckan.lib.dictization import table_dictize
-from ckan.lib.dictization.model_dictize import package_dictize, resource_dictize
-from ckan.model.types import make_uuid
 from sqlalchemy import (
     Column,
     DateTime,
     ForeignKey,
     String,
     UnicodeText,
     UniqueConstraint,
 )
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.orm import backref, relationship
 from typing_extensions import Self
 
+import ckan.model as model
+from ckan.lib.dictization import table_dictize
+from ckan.lib.dictization.model_dictize import resource_dictize
+from ckan.model.types import make_uuid
+
 from .base import Base
 
 
 class Report(Base):
     __tablename__ = "check_link_report"
 
     id = Column(UnicodeText, primary_key=True, default=make_uuid)
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/base.html` & `ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/base_admin.html` & `ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/base_admin.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/report.html` & `ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/report.html`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,27 @@
     <li class="active">
         {{ _("Global") }}
     </li>
 {% endblock %}
 
 
 {% block check_link_content %}
+    <div class="content-actions">
+        <ul class="list-unstyled">
+            {% block check_link_actions %}
+                {% block check_link_action_download_csv %}
+                    <li>
+                        <a class="btn btn-primary" href="{{ h.remove_url_param("format", null, "csv") }}">
+                            {{ _("Download as CSV") }}
+                        </a>
+                    </li>
+                {% endblock check_link_action_download_csv %}
+            {% endblock check_link_actions %}
+        </ul>
+    </div>
 
     <div class="check-link-reports">
         {% for report in page %}
             <div class="check-link-reports--item">
                 {% include "check_link/snippets/report_item.html" %}
             </div>
         {% else %}
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/templates/check_link/snippets/report_item.html` & `ckanext-check-link-0.1.0/ckanext/check_link/templates/check_link/snippets/report_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/tests/conftest.py` & `ckanext-check-link-0.1.0/ckanext/check_link/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import factory
 import pytest
-from ckan.tests.factories import CKANFactory, Resource, fake
 from pytest_factoryboy import register
 
+from ckan.tests.factories import CKANFactory, Resource, fake
+
 from ckanext.check_link.model import Report
 
 
 @pytest.fixture
 def clean_db(reset_db, migrate_db_for):
     reset_db()
     migrate_db_for("check_link")
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/action/test_check.py` & `ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/action/test_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest.mock import ANY
 
-import ckan.plugins.toolkit as tk
 import pytest
-from pytest_httpx import HTTPXMock
+
+import ckan.plugins.toolkit as tk
+
 # from aioresponses import aioresponses
 from ckan.tests.helpers import call_action
 
 
 @pytest.fixture
 def rmock(httpx_mock):
     return httpx_mock
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/tests/logic/action/test_report.py` & `ckanext-check-link-0.1.0/ckanext/check_link/tests/logic/action/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import ckan.plugins.toolkit as tk
 import pytest
+
+import ckan.plugins.toolkit as tk
 from ckan.tests.helpers import call_action
 
 
 @pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestSave:
     def test_resource_id_must_be_real(self, resource, faker):
         with pytest.raises(tk.ValidationError):
```

### Comparing `ckanext-check-link-0.0.9/ckanext/check_link/tests/model/test_report.py` & `ckanext-check-link-0.1.0/ckanext/check_link/tests/model/test_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import ckan.model as model
 import pytest
 
+import ckan.model as model
+
 from ckanext.check_link.model import Report
 
 
 @pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestReport:
     def test_removed_with_resource(self, resource, faker):
         report = Report(url=faker.url(), resource_id=resource["id"], state="unknown")
```

### Comparing `ckanext-check-link-0.0.9/ckanext_check_link.egg-info/PKG-INFO` & `ckanext-check-link-0.1.0/ckanext_check_link.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ckanext-check-link
-Version: 0.0.9
+Version: 0.1.0
 Summary: Resource URL checker
 Home-page: https://github.com/DataShades/ckanext-check-link
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/DataShades/ckanext-check-link/workflows/Tests/badge.svg?branch=main)](https://github.com/DataShades/ckanext-check-link/actions)
 
 # ckanext-check-link
```

### Comparing `ckanext-check-link-0.0.9/ckanext_check_link.egg-info/SOURCES.txt` & `ckanext-check-link-0.1.0/ckanext_check_link.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/check_link/__init__.py
 ckanext/check_link/cli.py
+ckanext/check_link/helpers.py
 ckanext/check_link/plugin.py
 ckanext/check_link/views.py
 ckanext/check_link/assets/script.js
 ckanext/check_link/assets/style.css
 ckanext/check_link/assets/webassets.yml
 ckanext/check_link/logic/__init__.py
 ckanext/check_link/logic/auth.py
@@ -21,14 +22,15 @@
 ckanext/check_link/migration/check_link/alembic.ini
 ckanext/check_link/migration/check_link/env.py
 ckanext/check_link/migration/check_link/script.py.mako
 ckanext/check_link/migration/check_link/versions/564f2016af51_create_report_table.py
 ckanext/check_link/model/__init__.py
 ckanext/check_link/model/base.py
 ckanext/check_link/model/report.py
+ckanext/check_link/templates/header.html
 ckanext/check_link/templates/check_link/base.html
 ckanext/check_link/templates/check_link/base_admin.html
 ckanext/check_link/templates/check_link/report.html
 ckanext/check_link/templates/check_link/snippets/report_item.html
 ckanext/check_link/tests/__init__.py
 ckanext/check_link/tests/conftest.py
 ckanext/check_link/tests/test_plugin.py
```

### Comparing `ckanext-check-link-0.0.9/setup.cfg` & `ckanext-check-link-0.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [metadata]
 name = ckanext-check-link
-version = 0.0.9
+version = 0.1.0
 description = Resource URL checker
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-check-link
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 keywords = CKAN
 
 [options]
 packages = find:
 namespace_packages = ckanext
 install_requires = 
-	check-link>=0.0.7, <1.0.0
+	check-link~=0.0.10
 	typing-extensions
 	ckanext-toolbelt
 include_package_data = True
 
 [options.entry_points]
 ckan.plugins = 
 	check_link = ckanext.check_link.plugin:CheckLinkPlugin
@@ -52,19 +52,11 @@
 previous = true
 
 [compile_catalog]
 domain = ckanext-check_link
 directory = ckanext/check_link/i18n
 statistics = true
 
-[tool:pytest]
-filterwarnings = 
-	ignore::sqlalchemy.exc.SADeprecationWarning
-	ignore::sqlalchemy.exc.SAWarning
-	ignore::DeprecationWarning
-addopts = --ckan-ini test.ini
-asyncio_mode = auto
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ckanext-check-link-0.0.9/setup.py` & `ckanext-check-link-0.1.0/setup.py`

 * *Files identical despite different names*

