# Comparing `tmp/irails-1.1.4.tar.gz` & `tmp/irails-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.1.4.tar", last modified: Fri May  5 06:20:41 2023, max compression
+gzip compressed data, was "irails-1.1.5.tar", last modified: Fri May  5 08:41:49 2023, max compression
```

## Comparing `irails-1.1.4.tar` & `irails-1.1.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.022965 irails-1.1.4/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7120 2023-05-05 06:20:41.021967 irails-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6339 2023-05-05 06:20:40.000000 irails-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.947027 irails-1.1.4/irails/
--rw-rw-rw-   0        0        0      318 2023-05-05 06:20:22.000000 irails-1.1.4/irails/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-05-05 06:08:39.000000 irails-1.1.4/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.4/irails/_utils.py
--rw-rw-rw-   0        0        0    11702 2023-05-04 04:55:19.000000 irails-1.1.4/irails/auth.py
--rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.4/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.961082 irails-1.1.4/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.962078 irails-1.1.4/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.4/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.4/irails/cbv.py
--rw-rw-rw-   0        0        0     6464 2023-05-03 14:45:48.000000 irails-1.1.4/irails/config.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.4/irails/controller.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.4/irails/controller_utils.py
--rw-rw-rw-   0        0        0    14422 2023-05-04 05:03:50.000000 irails-1.1.4/irails/core.py
--rw-rw-rw-   0        0        0     6425 2023-05-04 05:29:35.000000 irails-1.1.4/irails/database.py
--rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.4/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.4/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.4/irails/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.971051 irails-1.1.4/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.4/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-05-03 14:35:44.000000 irails-1.1.4/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     8189 2023-05-05 06:14:02.000000 irails-1.1.4/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.4/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.4/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.4/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.915104 irails-1.1.4/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.982073 irails-1.1.4/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.4/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.4/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.4/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1258 2023-05-02 08:55:43.000000 irails-1.1.4/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.4/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.4/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.4/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.4/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.987059 irails-1.1.4/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.4/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.988057 irails-1.1.4/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.4/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.000027 irails-1.1.4/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.4/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.4/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.4/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.4/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.4/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.4/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.4/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.4/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.004016 irails-1.1.4/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.4/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.4/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.008004 irails-1.1.4/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.921089 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.010996 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.015984 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.923082 irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:41.019972 irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.4/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:20:40.958988 irails-1.1.4/irails.egg-info/
--rw-rw-rw-   0        0        0     7120 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      753 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 06:20:40.000000 irails-1.1.4/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 06:20:41.022965 irails-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.459805 irails-1.1.5/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7120 2023-05-05 08:41:49.458808 irails-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6339 2023-05-05 08:41:49.000000 irails-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.408636 irails-1.1.5/irails/
+-rw-rw-rw-   0        0        0      318 2023-05-05 08:36:47.000000 irails-1.1.5/irails/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-05-05 06:08:39.000000 irails-1.1.5/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.1.5/irails/_utils.py
+-rw-rw-rw-   0        0        0    11702 2023-05-04 04:55:19.000000 irails-1.1.5/irails/auth.py
+-rw-rw-rw-   0        0        0    10573 2023-05-02 06:49:08.000000 irails-1.1.5/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.418619 irails-1.1.5/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.419611 irails-1.1.5/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.1.5/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.1.5/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.1.5/irails/cbv.py
+-rw-rw-rw-   0        0        0     6656 2023-05-05 08:24:35.000000 irails-1.1.5/irails/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.1.5/irails/controller.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.1.5/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    14553 2023-05-05 08:31:49.000000 irails-1.1.5/irails/core.py
+-rw-rw-rw-   0        0        0     6425 2023-05-04 05:29:35.000000 irails-1.1.5/irails/database.py
+-rw-rw-rw-   0        0        0     7943 2023-05-01 07:11:01.000000 irails-1.1.5/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.1.5/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.1.5/irails/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.424896 irails-1.1.5/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.1.5/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7773 2023-05-05 08:40:57.000000 irails-1.1.5/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     8189 2023-05-05 06:14:02.000000 irails-1.1.5/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.1.5/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.1.5/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.1.5/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.380869 irails-1.1.5/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.433875 irails-1.1.5/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      233 2023-05-05 05:43:26.000000 irails-1.1.5/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.1.5/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.1.5/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1357 2023-05-05 08:41:21.000000 irails-1.1.5/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.1.5/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.1.5/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.1.5/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.1.5/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.435869 irails-1.1.5/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.1.5/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.436867 irails-1.1.5/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.1.5/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.443848 irails-1.1.5/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 irails-1.1.5/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.1.5/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 irails-1.1.5/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 irails-1.1.5/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 irails-1.1.5/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0     1074 2023-05-02 08:48:52.000000 irails-1.1.5/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.1.5/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.1.5/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.445843 irails-1.1.5/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.1.5/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.1.5/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.448835 irails-1.1.5/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.385857 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.452825 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.455816 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.386854 irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.456814 irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2094 2023-05-01 09:15:49.000000 irails-1.1.5/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:49.414622 irails-1.1.5/irails.egg-info/
+-rw-rw-rw-   0        0        0     7120 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      753 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 08:41:49.000000 irails-1.1.5/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:41:49.459805 irails-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2955 2023-05-03 14:33:36.000000 irails-1.1.5/setup.py
```

### Comparing `irails-1.1.4/PKG-INFO` & `irails-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.4/README.md` & `irails-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/_loader.py` & `irails-1.1.5/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/_utils.py` & `irails-1.1.5/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/auth.py` & `irails-1.1.5/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/base_controller.py` & `irails-1.1.5/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.1.5/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.1.5/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/cbv.py` & `irails-1.1.5/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/config.py` & `irails-1.1.5/irails/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,20 @@
                 if name:
                     if name==key:
                         raise RuntimeError(f"configure file error circular reference `{name}`")
                     
                     if name.find(".")>0:
                         paris = name.split(".")
                         _root_value = self._raw_config[paris.pop(0)]
-                        _value = _root_value
+                        _value:Dict = _root_value
                         while paris:
-                            _value = _value[paris.pop(0)]
+                            _k = paris.pop(0) 
+                            _value = _value.get(_k,'')
+                            if not _value:
+                                print(f'Warning config: {name} was empty,it\'s quoted by {key}')
                             while _value.find("{")>-1 and value.find("}")>0:
                                 _name = _extract_name(_value)
                                 if _name:
                                     _expr = _root_value.get(_name,"")
                                     _x = f"{_name}"
                                     _value = _value.replace('{'+_x+'}',_expr)
                         return _value
```

### Comparing `irails-1.1.4/irails/controller.py` & `irails-1.1.5/irails/controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/controller_utils.py` & `irails-1.1.5/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/core.py` & `irails-1.1.5/irails/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,16 @@
     db_uri:str = db_cfg.get("uri")
     alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
     if db_uri:
         if db_uri.startswith('sqlite'):
             db_directory = os.path.dirname(db_uri.split(':///')[1])
             os.makedirs(db_directory, exist_ok=True) 
         application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini,cfg=db_cfg)
+    else:
+        _log.warn(f"Warning: database.uri is empty in config")
     return db_cfg
 
 def __init_auth(app,auth_type:str,casbin_adapter_class,__adapter_uri):
     
     
     auth_class = auth.get_auth_backend(auth_type)
     if not auth_class:
@@ -176,15 +178,15 @@
                 return RedirectResponse(url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
             
             @classmethod
             async def _auth__(cls,request:Request,response:Response,**kwargs):
                 '''called by .controller_util.py->route_method'''
                 auth_type = kwargs['auth_type'] 
                 
-                if not hasattr(application,'authObj'):
+                if not hasattr(application,'authObj') or application.authObj is None:
                     return True,None
                 
                 kwargs['session'] = request.session  
                 ret,user = await application.authObj.authenticate(request,**kwargs)
                 if user==auth.AUTH_EXPIRED:
                     request.session['flash']  = "your authencation has been expired!"  
                     user = False
@@ -313,15 +315,16 @@
     
     if __is_debug and db_cfg:
         _log.info("checking database migrations....")
         try:
              
             alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
             uri = db_cfg.get("uri")
-            database.check_migration(application.data_engine,uri,alembic_ini)
+            if uri:
+                database.check_migration(application.data_engine,uri,alembic_ini)
         except Exception as e:
             _log.disabled = False
             _log.error(e.args)
     if _casbin_adapter_class and _adapter_uri:
         _log.info("init casbin auth system...")
         application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
     _log.info("init mvc app end.")
```

### Comparing `irails-1.1.4/irails/database.py` & `irails-1.1.5/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/midware.py` & `irails-1.1.5/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/midware_casbin.py` & `irails-1.1.5/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/midware_session.py` & `irails-1.1.5/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/_app.py` & `irails-1.1.5/irails/scripts/_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,38 +65,40 @@
 
             return changed
         except Exception as e:
             print(f'an error raised {e.args}')
             print(f"now please open configs/general.yaml to modify app.root to add {app_dir}.{app_name}!")
             return
          
-    def do_copy(self,tpl_file,dest_file,over_write=False):
+    def do_copy(self,tpl_file,dest_file,micro=False,over_write=False,context={}):
         dest_file  = os.path.normpath(dest_file)
         if os.path.exists(dest_file) and not over_write:
             print(f'{dest_file} is exists,skip...')
             return True
         os.makedirs(os.path.dirname(dest_file),exist_ok=True)
         with open(tpl_file,'r') as f:
             content = f.read()
             dest_content = content
-            # template = Template(content)
-            # dest_content = template.render(context) 
+            if micro:
+                 
+                template = Template(content)
+                dest_content = template.render(context) 
             with open(dest_file,'w') as f:
                 f.write(dest_content)
         print(f"create {dest_file}")
 
     def add_home_view(self,app_dir,app_name):
         dist_file = os.path.join(app_dir,app_name,"views","home","home.html")
         tpl_file = os.path.dirname(__file__)+"/tpls/app/home.tpl"
         
-        context = {'app_name':app_name}
+        
         self.do_copy(tpl_file,dist_file)
         tpl_file = os.path.dirname(__file__)+"/tpls/app/home.css.tpl"
         dist_file = os.path.join(app_dir,app_name,"views","home","home.css")
-        self.do_copy(tpl_file,dist_file)
+        self.do_copy(tpl_file,dist_file,micro = True,context={'app_name':app_name})
         return True
     
     def add_home_controller(self,app_dir,app_name):
         dest_file = os.path.join(app_dir,app_name,"controllers","home_controller.py")
         dest_file = os.path.normpath(dest_file)
         if os.path.exists(dest_file):
             print(f'{dest_file} is exists,skip...')
```

### Comparing `irails-1.1.4/irails/scripts/_controller.py` & `irails-1.1.5/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/_project.py` & `irails-1.1.5/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/_run.py` & `irails-1.1.5/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/main.py` & `irails-1.1.5/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/app/home.css.tpl` & `irails-1.1.5/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/app/home.tpl` & `irails-1.1.5/irails/scripts/tpls/app/home.tpl`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 <!DOCTYPE html>
 <html>
 
 <head>
     <meta charset="utf-8">
-    <title>FastApi MVC Framework</title>
+    <title>${app_name}-Home</title>
     <link rel="stylesheet" href="home.css" />
 
 </head>
 
 <body>
     <header style="text-align:left;display: flex;">
         <h1>Python</h1>
         <h4>on FastApi</h4>
 
     </header>
     <nav>
-        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
-        <a href="${routers_map[item]['path']}">${routers_map[item]['doc']
-                and routers_map[item]['doc']['title'] or item}</a> {% endif %} {% endif %} {% endfor %}
+        {% for item in routers_map %} 
+            {% if 'GET' in routers_map[item]['methods'] %} 
+                {% if routers_map[item]['auth']=='none' or request.session['user'] %}
+        <a href="${routers_map[item]['path']}">
+            ${routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}
+        </a> 
+                {% endif %} 
+            {% endif %} 
+        {% endfor %}
 
         <a href="#">About</a>
-        <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>${request.session['user']['username']}</b>
-                Logout</a> {% endif %}
+        <a href="#">Contact</a> 
+        {% if request.session['user'] %}
+            <a href="/user/logout">
+            <b> ${request.session['user']['username']} </b> Logout</a> 
+        {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
         <p>here is the `text` variable in class method:${text}</p>
         <p style="color:red"><b>${flash}</b></p>
     </section>
```

### Comparing `irails-1.1.4/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.1.5/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.1.5/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.1.5/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/error_404.html` & `irails-1.1.5/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/error_500.html` & `irails-1.1.5/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.1.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.1.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.1.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails/view.py` & `irails-1.1.5/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails.egg-info/PKG-INFO` & `irails-1.1.5/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.1.4/irails.egg-info/SOURCES.txt` & `irails-1.1.5/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/irails.egg-info/requires.txt` & `irails-1.1.5/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.1.4/setup.py` & `irails-1.1.5/setup.py`

 * *Files identical despite different names*

