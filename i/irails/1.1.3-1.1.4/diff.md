# Comparing `tmp/irails-1.1.3.tar.gz` & `tmp/irails-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.3.tar", last modified: Thu May  4 04:33:18 2023, max compression
+gzip compressed data, was "irails-1.1.4.tar", last modified: Fri May  5 06:20:41 2023, max compression
```

## Comparing `irails-1.1.3.tar` & `irails-1.1.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.847989 irails-1.1.3/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6937 2023-05-04 04:33:18.846994 irails-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6156 2023-05-04 04:33:18.000000 irails-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.798123 irails-1.1.3/irails/
--rw-rw-rw-   0        0        0      318 2023-05-04 04:32:01.000000 irails-1.1.3/irails/__init__.py
--rw-rw-rw-   0        0        0     1682 2023-05-02 08:43:36.000000 irails-1.1.3/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.3/irails/_utils.py
--rw-rw-rw-   0        0        0    11616 2023-05-02 08:29:17.000000 irails-1.1.3/irails/auth.py
--rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.3/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.807101 irails-1.1.3/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.808103 irails-1.1.3/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.3/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.3/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.3/irails/cbv.py
--rw-rw-rw-   0        0        0     6464 2023-05-03 14:45:48.000000 irails-1.1.3/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.3/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.3/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14305 2023-05-04 04:15:21.000000 irails-1.1.3/irails/core.py
--rw-rw-rw-   0        0        0     6110 2023-04-30 14:34:13.000000 irails-1.1.3/irails/database.py
--rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.3/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.3/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.3/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.813083 irails-1.1.3/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.3/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-05-03 14:35:44.000000 irails-1.1.3/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7133 2023-05-03 07:16:46.000000 irails-1.1.3/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.3/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.3/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1702 2023-05-03 14:31:14.000000 irails-1.1.3/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.774300 irails-1.1.3/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.821063 irails-1.1.3/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0     1517 2023-04-30 09:03:04.000000 irails-1.1.3/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.3/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.3/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1258 2023-05-02 08:55:43.000000 irails-1.1.3/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.3/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.3/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.3/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.3/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.824054 irails-1.1.3/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.3/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.825051 irails-1.1.3/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.3/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.831036 irails-1.1.3/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.3/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.3/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.3/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.3/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.3/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.3/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.3/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.3/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.833034 irails-1.1.3/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.3/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.3/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.835026 irails-1.1.3/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.778288 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.840021 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.844019 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.779285 irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.844999 irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.3/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-04 04:33:18.804108 irails-1.1.3/irails.egg-info/
--rw-rw-rw-   0        0        0     6937 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 04:33:18.000000 irails-1.1.3/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 04:33:18.847989 irails-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.022965 irails-1.1.4/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7120 2023-05-05 06:20:41.021967 irails-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6339 2023-05-05 06:20:40.000000 irails-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.947027 irails-1.1.4/irails/
+-rw-rw-rw-   0        0        0      318 2023-05-05 06:20:22.000000 irails-1.1.4/irails/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-05-05 06:08:39.000000 irails-1.1.4/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.4/irails/_utils.py
+-rw-rw-rw-   0        0        0    11702 2023-05-04 04:55:19.000000 irails-1.1.4/irails/auth.py
+-rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.4/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.961082 irails-1.1.4/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.962078 irails-1.1.4/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.4/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.4/irails/cbv.py
+-rw-rw-rw-   0        0        0     6464 2023-05-03 14:45:48.000000 irails-1.1.4/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.4/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.4/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14422 2023-05-04 05:03:50.000000 irails-1.1.4/irails/core.py
+-rw-rw-rw-   0        0        0     6425 2023-05-04 05:29:35.000000 irails-1.1.4/irails/database.py
+-rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.4/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.4/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.4/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.971051 irails-1.1.4/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.4/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-05-03 14:35:44.000000 irails-1.1.4/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     8189 2023-05-05 06:14:02.000000 irails-1.1.4/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.4/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.4/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.4/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.915104 irails-1.1.4/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.982073 irails-1.1.4/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.4/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.4/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.4/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1258 2023-05-02 08:55:43.000000 irails-1.1.4/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.4/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.4/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.4/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.4/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.987059 irails-1.1.4/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.4/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.988057 irails-1.1.4/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.4/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.000027 irails-1.1.4/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.4/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.4/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.4/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.4/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.4/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.4/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.4/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.4/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.004016 irails-1.1.4/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.4/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.4/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.008004 irails-1.1.4/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.921089 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.010996 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.015984 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.923082 irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.019972 irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.4/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.958988 irails-1.1.4/irails.egg-info/
+-rw-rw-rw-   0        0        0     7120 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:20:41.022965 irails-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.4/setup.py
```

### Comparing `irails-1.1.3/PKG-INFO` & `irails-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,17 +72,22 @@
 from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
 from pydantic import conlist
 from app.services import UserService
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
- 
+@application.on_event("startup")
+def startup():
+    application.modify_authorization('bruce','/xml','GET',True)
 @api_router(auth='public')
 class TestController(BaseController): 
+    def __init__(self) -> None:
+        
+        super().__init__()
     @api.get("/user/login" )
     def login(self):
         """:title Login"""  
         redirect = self.get_param('redirect') if self.get_param('redirect') else '/' 
         return self.view() 
     @api.post("/test/verity_user",auth="none")
     async def verity_user(self):
```

### Comparing `irails-1.1.3/README.md` & `irails-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,22 @@
 from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
 from pydantic import conlist
 from app.services import UserService
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
- 
+@application.on_event("startup")
+def startup():
+    application.modify_authorization('bruce','/xml','GET',True)
 @api_router(auth='public')
 class TestController(BaseController): 
+    def __init__(self) -> None:
+        
+        super().__init__()
     @api.get("/user/login" )
     def login(self):
         """:title Login"""  
         redirect = self.get_param('redirect') if self.get_param('redirect') else '/' 
         return self.view() 
     @api.post("/test/verity_user",auth="none")
     async def verity_user(self):
```

### Comparing `irails-1.1.3/irails/_loader.py` & `irails-1.1.4/irails/_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,38 @@
 def load_module(module_name:str,module_path:str):
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         return module
     return None
-
+def _load_app(app_dir):
+    try:
+        _path = os.path.join(ROOT_PATH,app_dir.split(".")[0])
+        if _path not in sys.path:
+            sys.path.insert(-1,_path)
+        _log.info(f'Loading app: {app_dir}')
+        __import__(app_dir)
+        return True
+    except ImportError as e:
+        _log.error(f"load app{app_dir} failed")
+        _log.error(e.args)
+        raise e
+    
 def _load_apps(debug=False):
     if ROOT_PATH not in sys.path:
         sys.path.insert(-1,ROOT_PATH)
     unloaded = 0
     loaded = 0
     for app_dir in app_dirs:
         app_list =  __list_directories(app_dir)
         for app in app_list:
-            if __check_if_enabled(app): 
-                if debug:
-                    _log.info(f'Loading {app_dir}.{app}')
-                _path = os.path.join(ROOT_PATH,app_dir)
-                if _path not in sys.path:
-                    sys.path.insert(-1,_path)
-                __import__(f'{app_dir}.{app}')
-                loaded = loaded + 1
+            if __check_if_enabled(app):  
+                if _load_app(f'{app_dir}.{app}'):
+                    loaded = loaded + 1
+                else:
+                    unloaded = unloaded + 1
             else:
                 unloaded = unloaded + 1
         
     
     return loaded,unloaded
```

### Comparing `irails-1.1.3/irails/_utils.py` & `irails-1.1.4/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/auth.py` & `irails-1.1.4/irails/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,15 @@
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
 AUTH_EXPIRED='[EXPIRED]!'
 
 _session_name:str = ""
-class AuthenticationBackend_(AuthenticationBackend):
-    def create_access_token(self,**kwargs):
-        raise NotImplementedError()
-    def clear_userinfo(self,request:Request):
-        raise NotImplementedError()
-    pass
+
 class CasbinAuth:
     def __init__(self,enforcer:Enforcer,session_name="user") -> None:
         global _session_name
         self.enforcer = enforcer
         self.__session_name = _session_name = session_name
         pass
     def modify_authorization(self,sub,obj,act,authorize:bool):
@@ -107,14 +102,23 @@
             else:
                 decoded = base64.b64decode(credentials).decode("ascii")
                 username, _, password = decoded.partition(":")
                 if username:
                     return username,password,None
         return "","",None
     
+class AuthenticationBackend_(AuthenticationBackend):
+    def create_access_token(self,**kwargs):
+        raise NotImplementedError()
+    def clear_userinfo(self,request:Request):
+        raise NotImplementedError()
+    @property
+    def casbin_auth(self)->CasbinAuth:
+        return _casbin_auth
+    pass
 class BasicAuth(AuthenticationBackend_):
     def __init__(self,**kwargs) -> None:
         super().__init__()
      
     
     async def authenticate(self, request:Request, **kwargs):
         username,password,_ = _casbin_auth.get_user_from_request(request=request)
```

### Comparing `irails-1.1.3/irails/base_controller.py` & `irails-1.1.4/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.1.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.1.4/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/cbv.py` & `irails-1.1.4/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/config.py` & `irails-1.1.4/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/controller.py` & `irails-1.1.4/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/controller_utils.py` & `irails-1.1.4/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/core.py` & `irails-1.1.4/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ._utils import get_controller_name,get_snaked_name
 
 __is_debug=config.get('debug',False)
 
 
 class MvcApp(FastAPI):
     def __init__(self,  **kwargs):
-        self._authObj:auth.AuthenticationBackend_ = None 
+        self.__authObj:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
         self.__user_auth_url=""
         self.__public_auth_url=""
         self._app_views_dirs = {} 
         self.routers_map = {}
         super().__init__(**kwargs)
     @property
@@ -43,22 +43,24 @@
         """internal user auth url"""
         return self.__user_auth_url
     @user_auth_url.setter
     def user_auth_url(self,url):
         if self.__user_auth_url:
             raise RuntimeError(f"user_auth_url only can be setting once time,current is:{self.__user_auth_url}")
         self.__user_auth_url = url
-
+    @property
+    def modify_authorization(self):
+        return self.__authObj.casbin_auth.modify_authorization
     @property
     def authObj(self)->auth.AuthenticationBackend_:
-        return self._authObj
+        return self.__authObj
     
     @authObj.setter
     def authObj(self,value:auth.AuthenticationBackend_):
-        self._authObj = value
+        self.__authObj = value
      
     @property 
     def data_engine(self)->database.Engine:
         return self._data_engine
     @data_engine.setter
     def data_engine(self,value):
         self._data_engine = value
```

### Comparing `irails-1.1.3/irails/database.py` & `irails-1.1.4/irails/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from contextlib import contextmanager
 from sqlalchemy import create_engine,Engine,MetaData, Table, Column, ForeignKey,select,join,TableClause
-from sqlalchemy.orm import DeclarativeBase,Session
+from sqlalchemy.orm import DeclarativeBase,Session,sessionmaker
 from sqlalchemy import text,TextClause
 from sqlalchemy.ext.automap import automap_base
 
 from ._utils import camelize_classname,pluralize_collection
  
 from alembic import command
 from alembic.config import Config
@@ -19,14 +20,32 @@
 
  
 
 class Service():
     __all_generated = {}
     
     @classmethod
+    @contextmanager 
+    def get_session(cls):
+        """Provide a transactional scope around a series of operations."""
+        if hasattr(cls,'_session_local'):
+            session_local = getattr(cls,'_session_local')
+        else:
+            session_local =  sessionmaker(bind=engine)
+            setattr(cls,"_session_local", session_local)
+        session = session_local()
+        try:
+            yield session
+            session.commit()
+        except Exception as e:
+            session.rollback()
+            raise e
+        finally:
+            session.close()
+    @classmethod
     def execute(cls,cmd:Union[str,TextClause],**kwargs):
         if not isinstance(cmd,TextClause):
             cmd = text(str)
         with engine.begin() as conn:
             ret = conn.execute(cmd,**kwargs)
         return ret
     @classmethod
@@ -59,21 +78,16 @@
             tbl = DataMap.tables[table_name]
             tbItem = tblClass()
             setattr(tbItem,"_tableItem",tbl) 
             cls.__all_generated[table_name] = tbItem
             return tbItem
         else:
             raise NameError()
-    # @classmethod 
-    # def query(cls,*args):
-    #     item = Service.mapped('item')
-    #     ba_cls_info = Service.mapped('ba_cls_info')
-    #     with Session(engine) as session:
-    #         p1 = session.query(*args).select_from(item._tableItem).join(
-    #             ba_cls_info._tableItem,item.class_no==ba_cls_info.class_no).first()
+
+
             
 def ismongo_cloud(uri):
     import re 
     # uri = 'mongodb+srv://dbbruce:smjk123@atlascluster.siz4vrp.mongodb.net/?retryWrites=true&w=majority' 
     # 匹配 MongoDB Cloud 连接字符串的正则表达式
     regex = re.compile("mongodb\+srv:\/\/.*@.*\.mongodb\.net\/.*\?.*") 
     return regex.match(uri)
```

### Comparing `irails-1.1.3/irails/midware.py` & `irails-1.1.4/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/midware_casbin.py` & `irails-1.1.4/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/midware_session.py` & `irails-1.1.4/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/_app.py` & `irails-1.1.4/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/_controller.py` & `irails-1.1.4/irails/scripts/_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             if use_micro:
                 template = Template(content)
                 dest_content = template.render(context)
             
             
             with open(dest,'w') as f:
                 f.write(dest_content)
-        print(f"create {dest}")
+            print(f"create {dest}")
         return True
     def str_to_upper(self,name):
         new_name = name.title().replace("_", "")
         return new_name
     def is_valid_class_name(self,name):
         if not isinstance(name, str):
             return False 
@@ -78,15 +78,16 @@
                 file.writelines(lines)
 
     def __call__(self) -> Any:
          
         if not self.args.name:
             print(f'controller name is empty,exit!')
             exit()
-        for name in self.args.name:
+        name = self.args.name.pop(0)
+        if name:
             if not is_valid_filename(name) :
                 print(f'{name} is not avalided!')
                 exit() 
 
             store_dir = self.dir
             controller_name:str = name
             controler_path_name = get_snaked_name(controller_name)
@@ -117,24 +118,41 @@
                     _item = items
                 else:
                     _item = [items]
                 for item in _item:
                     tpl = item['tpl']
                     dest = os.path.join(_current_dir , item['dest'])
                     micro = item['micro']
-                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=False) 
-
+                    #controller file will generate last time
+                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=dir=='controllers') 
+            controller_file = os.path.join(_current_dir,'controllers',f"{controler_path_name}_controller.py")
             __init_file = os.path.join(_current_dir,'controllers','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_controller")
             __init_file = os.path.join(_current_dir,'models','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_model")
             __init_file = os.path.join(_current_dir,'services','__init__.py')
             self.ensure_line(__init_file,f"from . import {controler_path_name}_service")
-             
-        
+            acts = []
+            for action in self.args.name:
+                acts.append(f"""
+    @api.get('/{action}')
+    def {action}(self):
+        return self.view()                
+""")
+                _view_file = os.path.join(_current_dir,'views',controler_path_name,f"{action}.html")
+                if not os.path.exists(_view_file):
+                    with open(_view_file,'w') as f:
+                        f.write(f"{controller_name}.{action} view file.in:{_view_file}")
+                    print(f'create {_view_file}')
+                else:
+                    print(f'{_view_file} was exists,skip generate')
+            actions = "\n".join(acts)
+            context['actions'] = actions    
+            self.gen_tpl(tpl_file=dirs_items['controllers']['tpl'],dest=controller_file,context=context,use_micro=True,dir_only=False) 
+
         print("Done!")
     pass
 
 def is_in_app(directory):
     """
     check exists controllers , views dir in :directory
     """
@@ -157,15 +175,15 @@
     cur_dir = os.path.abspath(os.curdir)
     root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
     if os.path.exists(root_path) and  os.path.isdir(root_path): 
         if not is_in_irails(root_path) or not is_in_app(cur_dir):
             print(f"Please exec in irails project's app dir ,like `apps/app`")
             exit()
     self_file = __file__.lstrip("_").replace(".py",'')
-    parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [--name] `controller name` ...", description='create new controller')
+    parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [--name] `controller [action ...]` ...", description='create new controller')
     parser.add_argument('--name',help="controller name to create")
     parser.add_argument('args', nargs=argparse.REMAINDER)
      
     args = parser.parse_args()
     if not any(args.__dict__.values()):
         parser.print_help()
     if not args.name:
```

### Comparing `irails-1.1.3/irails/scripts/_project.py` & `irails-1.1.4/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/_run.py` & `irails-1.1.4/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/main.py` & `irails-1.1.4/irails/scripts/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import argparse
 import sys
 import importlib.util
 import os.path
  
 import os
 import re
+def _ensure_cli():
+    executable = os.path.basename(sys.argv[0])
+    if not executable.startswith('irails'):
+        sys.argv[0] = 'irails'
+_ensure_cli()
 from irails import __version__
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
     """
     
     dir_path = os.path.dirname(os.path.abspath(__file__))  
@@ -34,16 +39,15 @@
      
     args = parser.parse_args()
     
     
     args.feature = '_' +args.feature
     
     module_path = os.path.join(module_dir, args.feature + '.py')
-    if sys.argv[0]!='irails':
-        sys.argv[0] = 'irails'
+    
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(args.feature, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         sys.argv.pop(1)
         module.main()
     else:
```

### Comparing `irails-1.1.3/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.4/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/app/home.tpl` & `irails-1.1.4/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.4/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.4/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.4/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.4/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.4/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails/view.py` & `irails-1.1.4/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails.egg-info/PKG-INFO` & `irails-1.1.4/irails.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,17 +72,22 @@
 from irails import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
 from pydantic import conlist
 from app.services import UserService
 application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login'
- 
+@application.on_event("startup")
+def startup():
+    application.modify_authorization('bruce','/xml','GET',True)
 @api_router(auth='public')
 class TestController(BaseController): 
+    def __init__(self) -> None:
+        
+        super().__init__()
     @api.get("/user/login" )
     def login(self):
         """:title Login"""  
         redirect = self.get_param('redirect') if self.get_param('redirect') else '/' 
         return self.view() 
     @api.post("/test/verity_user",auth="none")
     async def verity_user(self):
```

### Comparing `irails-1.1.3/irails.egg-info/SOURCES.txt` & `irails-1.1.4/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/irails.egg-info/requires.txt` & `irails-1.1.4/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.3/setup.py` & `irails-1.1.4/setup.py`

 * *Files identical despite different names*

