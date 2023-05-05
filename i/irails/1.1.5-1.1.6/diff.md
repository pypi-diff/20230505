# Comparing `tmp/irails-1.1.5.tar.gz` & `tmp/irails-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.5.tar", last modified: Fri May  5 08:41:49 2023, max compression
+gzip compressed data, was "irails-1.1.6.tar", last modified: Fri May  5 14:48:27 2023, max compression
```

## Comparing `irails-1.1.5.tar` & `irails-1.1.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.459805 irails-1.1.5/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7120 2023-05-05 08:41:49.458808 irails-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6339 2023-05-05 08:41:49.000000 irails-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.408636 irails-1.1.5/irails/
--rw-rw-rw-   0        0        0      318 2023-05-05 08:36:47.000000 irails-1.1.5/irails/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-05-05 06:08:39.000000 irails-1.1.5/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.5/irails/_utils.py
--rw-rw-rw-   0        0        0    11702 2023-05-04 04:55:19.000000 irails-1.1.5/irails/auth.py
--rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.5/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.418619 irails-1.1.5/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.419611 irails-1.1.5/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.5/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.5/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.5/irails/cbv.py
--rw-rw-rw-   0        0        0     6656 2023-05-05 08:24:35.000000 irails-1.1.5/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.5/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.5/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14553 2023-05-05 08:31:49.000000 irails-1.1.5/irails/core.py
--rw-rw-rw-   0        0        0     6425 2023-05-04 05:29:35.000000 irails-1.1.5/irails/database.py
--rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.5/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.5/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.5/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.424896 irails-1.1.5/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.5/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7773 2023-05-05 08:40:57.000000 irails-1.1.5/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     8189 2023-05-05 06:14:02.000000 irails-1.1.5/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.5/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.5/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.5/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.380869 irails-1.1.5/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.433875 irails-1.1.5/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.5/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.5/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.5/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1357 2023-05-05 08:41:21.000000 irails-1.1.5/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.5/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.5/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.5/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.5/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.435869 irails-1.1.5/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.5/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.436867 irails-1.1.5/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.5/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.443848 irails-1.1.5/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.5/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.5/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.5/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.5/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.5/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.5/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.5/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.5/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.445843 irails-1.1.5/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.5/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.5/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.448835 irails-1.1.5/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.385857 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.452825 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.455816 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.386854 irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.456814 irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.5/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.414622 irails-1.1.5/irails.egg-info/
--rw-rw-rw-   0        0        0     7120 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 08:41:49.459805 irails-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.564814 irails-1.1.6/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7120 2023-05-05 14:48:27.564814 irails-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6339 2023-05-05 14:48:27.000000 irails-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.505604 irails-1.1.6/irails/
+-rw-rw-rw-   0        0        0      318 2023-05-05 14:48:24.000000 irails-1.1.6/irails/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-05-05 06:08:39.000000 irails-1.1.6/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.6/irails/_utils.py
+-rw-rw-rw-   0        0        0    11702 2023-05-04 04:55:19.000000 irails-1.1.6/irails/auth.py
+-rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.6/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.515577 irails-1.1.6/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.516575 irails-1.1.6/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.6/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.6/irails/cbv.py
+-rw-rw-rw-   0        0        0     6656 2023-05-05 08:24:35.000000 irails-1.1.6/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.6/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.6/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14397 2023-05-05 11:09:47.000000 irails-1.1.6/irails/core.py
+-rw-rw-rw-   0        0        0     6338 2023-05-05 11:07:47.000000 irails-1.1.6/irails/database.py
+-rw-rw-rw-   0        0        0     8134 2023-05-05 14:29:33.000000 irails-1.1.6/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.6/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.6/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.522347 irails-1.1.6/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.6/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7785 2023-05-05 10:17:36.000000 irails-1.1.6/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     8189 2023-05-05 06:14:02.000000 irails-1.1.6/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.6/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.6/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.6/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.476691 irails-1.1.6/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.533316 irails-1.1.6/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.6/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.6/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.6/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.1.6/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.6/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.6/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.6/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.6/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.535311 irails-1.1.6/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.6/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.537306 irails-1.1.6/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.6/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.547287 irails-1.1.6/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.6/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.6/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.6/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.6/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.6/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.6/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.6/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.6/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.550379 irails-1.1.6/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.6/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.6/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.552376 irails-1.1.6/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.483663 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.555382 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.559357 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.485657 irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.562350 irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.1.6/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:48:27.513583 irails-1.1.6/irails.egg-info/
+-rw-rw-rw-   0        0        0     7120 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 14:48:27.000000 irails-1.1.6/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:48:27.565813 irails-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.6/setup.py
```

### Comparing `irails-1.1.5/PKG-INFO` & `irails-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.5
+Version: 1.1.6
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.5/README.md` & `irails-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/_loader.py` & `irails-1.1.6/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/_utils.py` & `irails-1.1.6/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/auth.py` & `irails-1.1.6/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/base_controller.py` & `irails-1.1.6/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.1.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.1.6/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/cbv.py` & `irails-1.1.6/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/config.py` & `irails-1.1.6/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/controller.py` & `irails-1.1.6/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/controller_utils.py` & `irails-1.1.6/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/core.py` & `irails-1.1.6/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,22 +70,19 @@
 __all_controller__ = []
 
 application = __app
 api.init(application)
 
 
 
-def __init_database(): 
+def check_init_database(): 
     db_cfg = config.get("database")
     db_uri:str = db_cfg.get("uri")
     alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
-    if db_uri:
-        if db_uri.startswith('sqlite'):
-            db_directory = os.path.dirname(db_uri.split(':///')[1])
-            os.makedirs(db_directory, exist_ok=True) 
+    if db_uri: 
         application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini,cfg=db_cfg)
     else:
         _log.warn(f"Warning: database.uri is empty in config")
     return db_cfg
 
 def __init_auth(app,auth_type:str,casbin_adapter_class,__adapter_uri):
     
@@ -295,15 +292,15 @@
     _register_controllers()
 
     _log.info("static files mouting...")
     midware.init(app=application,debug=__is_debug)
 
     if __is_debug:
         _log.info("checking database configure...")
-    db_cfg = __init_database()
+    db_cfg = check_init_database()
     auth_type = config.get("auth",None)
     _casbin_adapter_class=None
     _adapter_uri:str=None
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
             __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
```

### Comparing `irails-1.1.5/irails/database.py` & `irails-1.1.6/irails/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,19 +134,17 @@
     params :uri sqlalchemy connection string
     :params debug mode of debug 
     :params alembic_ini alembic config file path,when debug=True will auto migrate the changes 
     '''
     global DataMap,mapped_base ,engine
     dbencode = cfg.get('dbencode')
     dbdecode = cfg.get('dbdecode')
-    # if ismongo_cloud(uri=uri):
-    #     from pymongo import MongoClient
-    #     client = MongoClient(uri)
-    #     database = client.get_database("<DATABASE>")
-    #     collection = database.get_collection("<COLLECTION>")
+    if uri.startswith('sqlite'):
+        db_directory = os.path.dirname(uri.split(':///')[1])
+        os.makedirs(db_directory, exist_ok=True) 
 
     engine = create_engine(uri,  echo=debug)
     dbfirst = cfg.get("dbfirst")
     maptables = cfg.get("maptables")
     
     if not dbfirst :
         pass
```

### Comparing `irails-1.1.5/irails/midware.py` & `irails-1.1.6/irails/midware.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,23 +138,29 @@
             context = {'error':e,'debug':debug,'debug_info':content}
             
             return viewObj(file,context,status_code=404)
         return None
     
     @app.exception_handler(StarletteHTTPException)
     async def custom_http_exception_handler(request, e:StarletteHTTPException):
-        
-        ret = error_page(404,request=request,e=e)
+        e_no = 404
+        if e.args and isinstance(e.args,tuple):
+            e_no = e.args[0]
+            if debug:
+                e_info = e.args[1]
+        else:
+            e_info = e.args
+        ret = error_page(e_no,request=request,e=e)
         if ret:
             return ret
         else:
             content = "<h1>404 Not Found(URL Exception)</h1>"
             content += '<h3>please check url</h3>'
             if debug:
-                content += '<p>' + str(e.detail) + '</p>'
+                content += '<p>' + str(e_info) + '</p>'
             return HTMLResponse(content=content, status_code=404)
    
     @app.exception_handler(Exception)
     async def validation_exception_handler(request, e:Exception):
         ret = error_page(500,request=request,e=e)
         if ret:
             return ret
```

### Comparing `irails-1.1.5/irails/midware_casbin.py` & `irails-1.1.6/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/midware_session.py` & `irails-1.1.6/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/_app.py` & `irails-1.1.6/irails/scripts/_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,23 @@
                  
                 template = Template(content)
                 dest_content = template.render(context) 
             with open(dest_file,'w') as f:
                 f.write(dest_content)
         print(f"create {dest_file}")
 
-    def add_home_view(self,app_dir,app_name):
+    def add_home_view(self,app_dir,app_name:str):
         dist_file = os.path.join(app_dir,app_name,"views","home","home.html")
         tpl_file = os.path.dirname(__file__)+"/tpls/app/home.tpl"
         
         
         self.do_copy(tpl_file,dist_file)
         tpl_file = os.path.dirname(__file__)+"/tpls/app/home.css.tpl"
         dist_file = os.path.join(app_dir,app_name,"views","home","home.css")
-        self.do_copy(tpl_file,dist_file,micro = True,context={'app_name':app_name})
+        self.do_copy(tpl_file,dist_file,micro = True,context={'app_name':app_name.title()})
         return True
     
     def add_home_controller(self,app_dir,app_name):
         dest_file = os.path.join(app_dir,app_name,"controllers","home_controller.py")
         dest_file = os.path.normpath(dest_file)
         if os.path.exists(dest_file):
             print(f'{dest_file} is exists,skip...')
```

### Comparing `irails-1.1.5/irails/scripts/_controller.py` & `irails-1.1.6/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/_project.py` & `irails-1.1.6/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/_run.py` & `irails-1.1.6/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/main.py` & `irails-1.1.6/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.6/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/app/home.tpl` & `irails-1.1.6/irails/scripts/tpls/app/home.tpl`

 * *Files 25% similar despite different names*

```diff
@@ -20,17 +20,15 @@
                 {% if routers_map[item]['auth']=='none' or request.session['user'] %}
         <a href="${routers_map[item]['path']}">
             ${routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}
         </a> 
                 {% endif %} 
             {% endif %} 
         {% endfor %}
-
-        <a href="#">About</a>
-        <a href="#">Contact</a> 
+ 
         {% if request.session['user'] %}
             <a href="/user/logout">
             <b> ${request.session['user']['username']} </b> Logout</a> 
         {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ****** Python ******
 *** on FastApi ***
   {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
 {% if routers_map[item]['auth']=='none' or request.session['user'] %} $
 {routers_map[item]['doc']_and_routers_map[item]['doc']['title']_or_item} {%
-endif %} {% endif %} {% endfor %} About Contact {% if request.session['user']
-%} ${request.session['user']['username']}_Logout {% endif %}
+endif %} {% endif %} {% endfor %} {% if request.session['user'] %} $
+{request.session['user']['username']}_Logout {% endif %}
 ***** Welcome to my website *****
 This is an example of a responsive design that works well on both desktop and
 mobile devices.
 here is the `text` variable in class method:${text}
 ${flash}
 
 © 2023 My Website
```

### Comparing `irails-1.1.5/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.6/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.6/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.6/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.6/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.6/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails/view.py` & `irails-1.1.6/irails/view.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Any, Mapping
 from fastapi import BackgroundTasks, Request,Response
 from fastapi.templating import Jinja2Templates
 from fastapi.exceptions import HTTPException
- 
+import jinja2
  
 from .config import ROOT_PATH,config,_log
 
 env_configs = {} 
 static_format = []
 def __get_view_configure():
     global static_format,env_configs
@@ -48,16 +48,28 @@
         if not request or not isinstance(request, Request):
             raise ValueError("request instance type must be fastapi.Request") 
 
         if not view_path.endswith(".html"):
             view_path = f"{view_path}.html"
 
         context["request"] = request
+        view_path_real = os.path.join(self.views_directory,view_path).replace(ROOT_PATH,"").replace("\\","/")
         try:
             res = self._templates.TemplateResponse(view_path, context,**kwargs)
             return res
+        except jinja2.exceptions.TemplateSyntaxError as e:
+            source = e.source.split('\n')[e.lineno-1:e.lineno]
+            info = f"TemplateSyntaxError on {view_path_real}:line:{e.lineno},{source}"
+            _log.error(info)
+            raise HTTPException(500,info)
+        except jinja2.exceptions.TemplateNotFound as e:
+            source = e.args[0]
+            info = f"{view_path_real} raised TemplatesNotFound Error: `{source}`"
+            _log.error(info)
+            raise HTTPException(500,info)
         except Exception as e:
-            _log.error("template not found"+e.args)
-            view_path = os.path.join(self.views_directory,view_path).replace(ROOT_PATH,"").replace("\\","/")
-            raise HTTPException(500,f"template not found ![{e.args}]")
+            info =f"Tempate {view_path_real} raised Exception {e.args}"
+            _log.error(info)
+            
+            raise HTTPException(500,info)
```

### Comparing `irails-1.1.5/irails.egg-info/PKG-INFO` & `irails-1.1.6/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.5
+Version: 1.1.6
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.5/irails.egg-info/SOURCES.txt` & `irails-1.1.6/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/irails.egg-info/requires.txt` & `irails-1.1.6/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.5/setup.py` & `irails-1.1.6/setup.py`

 * *Files identical despite different names*

