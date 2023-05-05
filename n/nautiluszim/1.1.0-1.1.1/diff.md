# Comparing `tmp/nautiluszim-1.1.0.tar.gz` & `tmp/nautiluszim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautiluszim-1.1.0.tar", last modified: Fri May  5 12:13:42 2023, max compression
+gzip compressed data, was "nautiluszim-1.1.1.tar", last modified: Fri May  5 15:50:05 2023, max compression
```

## Comparing `nautiluszim-1.1.0.tar` & `nautiluszim-1.1.1.tar`

### file list

```diff
@@ -1,588 +1,588 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.519174 nautiluszim-1.1.0/nautiluszim/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.519174 nautiluszim-1.1.0/nautiluszim/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/locale/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/database.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/display_rows.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/info-circle-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/init.js
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/main-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/media_player.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/modal_empty_body.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/modal_title.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/nautilus.js
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim/templates/precompiled.js
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.527174 nautiluszim-1.1.0/nautiluszim/templates/vendors/
--rw-r--r--   0 runner    (1001) docker     (123)    17430 2020-05-04 16:04:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ScrollMagic.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.519174 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.531174 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    67871 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)   157964 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    50935 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   115021 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    77346 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32546 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   197170 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   504418 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   159515 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   641867 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.531174 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   227980 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   410007 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    80698 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   318045 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   135079 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   256099 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    60010 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   194435 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.575175 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2018-08-05 19:09:20.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3g2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3ga.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3gp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/7z.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aac.svg
--rw-r--r--   0 runner    (1001) docker     (123)      555 2018-08-04 18:46:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ac.svg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/adn.svg
--rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ai.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aif.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aifc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aiff.svg
--rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ait.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/amr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2018-06-23 16:58:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ani.svg
--rw-r--r--   0 runner    (1001) docker     (123)      829 2018-06-23 17:59:22.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/apk.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/app.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2018-08-04 19:09:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/applescript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asax.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ascx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ashx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asmx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      730 2018-07-28 14:27:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aspx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/au.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-08-05 04:08:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/avi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/axd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-24 12:27:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aze.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2018-06-24 12:59:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/blank.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bmp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2018-08-05 17:23:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bowerrc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-06-24 17:12:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/browser.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bz2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      407 2018-06-30 00:29:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/c.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cad.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/caf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2018-06-29 23:33:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2018-08-05 20:11:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 03:33:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cgi.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2018-07-28 15:17:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/class.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cmd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2018-08-04 16:34:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/codekit.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2018-08-04 23:31:11.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/coffee.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/coffeelintignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/com.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2018-06-24 16:56:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/compile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2018-08-05 17:39:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/conf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/config.svg
--rw-r--r--   0 runner    (1001) docker     (123)      583 2018-06-30 00:30:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cpp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      675 2018-07-27 01:50:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cptx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cr2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2018-07-21 22:39:54.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crdownload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-07-16 05:46:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crypt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      655 2018-06-30 00:30:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2018-08-04 23:32:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cson.svg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csproj.svg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2018-06-29 21:26:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/css.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2018-07-16 05:44:20.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cue.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-08-05 04:11:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/db.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dbf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/deb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dgn.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2018-07-21 20:21:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/diz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dll.svg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2018-08-04 14:05:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dmg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dng.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/doc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:50.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/docb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/docm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/docx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dotm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dotx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      740 2018-07-22 03:47:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:35:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dpj.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2018-06-30 18:59:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ds_store.svg
--rw-r--r--   0 runner    (1001) docker     (123)      555 2018-07-18 23:08:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dtd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dwg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dxf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2018-08-04 20:17:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/editorconfig.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:16:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/el.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/enc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-07-28 16:31:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/epub.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eslintignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/exe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/f4v.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2018-07-18 23:43:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fax.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fb2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      343 2018-06-23 16:11:22.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fla.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flac.svg
--rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 2018-08-05 19:39:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gadget.svg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2018-08-04 20:28:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gdp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2018-06-30 04:29:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gem.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gif.svg
--rw-r--r--   0 runner    (1001) docker     (123)      694 2018-08-04 20:41:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gitattributes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gitignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2018-07-16 05:26:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/go.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-08-05 19:40:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 2018-07-19 02:16:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/h.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/handlebars.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hbs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/heic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hsl.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/htm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/html.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ibooks.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/icns.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)      591 2018-06-29 23:32:36.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ics.svg
--rw-r--r--   0 runner    (1001) docker     (123)      644 2018-07-18 23:46:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/idx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iff.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2018-08-05 17:40:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ifo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/img.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/in.svg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2018-06-23 16:06:20.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/indd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/inf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ini.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iso.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2018-07-21 14:30:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/j2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jar.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:50.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/java.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jpe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2018-06-29 21:26:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/js.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2018-06-29 21:39:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:37:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2018-06-29 21:40:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/key.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kf8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2018-08-04 17:53:19.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kmk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ksh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2018-08-04 18:52:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2018-07-28 15:17:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/less.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/licx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:15:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lisp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2018-08-05 16:10:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lnk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 2018-06-24 16:25:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/log.svg
--rw-r--r--   0 runner    (1001) docker     (123)      465 2018-07-21 17:43:54.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lua.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2018-08-05 17:33:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m2v.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2018-08-05 06:23:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4a.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4r.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4v.svg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/map.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/master.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2018-07-21 18:59:04.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/md.svg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2018-08-05 05:48:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/me.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/midi.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mkv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2018-08-05 17:27:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mobi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mod.svg
--rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mov.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      913 2018-07-18 23:59:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpga.svg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2018-06-30 14:04:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msu.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nef.svg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2018-08-05 18:13:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2018-07-21 20:21:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nfo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-27 02:23:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nix.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/npmignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2018-07-19 00:19:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      671 2018-06-23 11:58:54.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ods.svg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ogg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ogv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ost.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/otf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ott.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ova.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ovf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/p12.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/p7b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2018-07-19 02:45:38.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pages.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2018-07-19 02:50:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/part.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pcd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdb.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2018-06-19 08:11:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pem.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pfx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pgp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ph.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2018-06-30 18:08:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/phar.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2018-06-29 22:06:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/php.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pkg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2018-06-30 11:23:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pl.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2018-08-04 20:04:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/plist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/png.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/po.svg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2018-07-21 17:42:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pom.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/potx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pps.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ppsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ppt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pptm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pptx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/prop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2018-07-21 21:37:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2018-06-23 16:13:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/psd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/psp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pst.svg
--rw-r--r--   0 runner    (1001) docker     (123)      627 2018-07-19 00:02:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pub.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2018-06-24 17:07:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/py.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2018-07-16 05:23:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pyc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/qt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ra.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ram.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/raw.svg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/resx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2018-07-28 14:56:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/retry.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2018-08-05 16:36:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rom.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rpm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rsa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      668 2018-08-05 04:06:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rss.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rtf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2018-07-27 04:19:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ru.svg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rub.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sass.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/scss.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sed.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sitemap.svg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/skin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sldm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sldx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      906 2018-07-28 15:15:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sln.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2018-07-21 18:47:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sol.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sql.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2018-08-05 19:02:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sqlite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/step.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/stl.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2018-08-05 17:36:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2018-06-30 12:16:27.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2018-08-05 19:41:27.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sys.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tcsh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tfignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tga.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tgz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tif.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tiff.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2018-08-05 03:53:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tmp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2018-06-30 03:47:11.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/torrent.svg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2018-08-04 17:10:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ts.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tsv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2018-08-04 16:11:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ttf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      358 2018-07-27 01:37:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/twig.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/txt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/udf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      555 2018-06-30 00:51:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbproj.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2018-08-05 18:09:55.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vcd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      453 2018-06-24 19:18:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vcs.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vmdk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vob.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-07-16 04:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vss.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vst.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vtx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:36:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/war.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wav.svg
--rw-r--r--   0 runner    (1001) docker     (123)      716 2018-08-05 03:42:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wbk.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-08-05 19:41:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webinfo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wma.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wmf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wmv.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      685 2018-06-30 14:11:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wps.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wsf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2018-07-22 02:04:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xcf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xls.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlsm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xltm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xltx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-07-26 04:04:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2018-07-22 03:42:57.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xpi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xps.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xrb.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2018-07-28 19:17:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xsd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xsl.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xspf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/yml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/z.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zsh.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20696 2021-02-15 09:49:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js
--rw-r--r--   0 runner    (1001) docker     (123)    88145 1991-10-18 12:00:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.587175 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2019-03-12 21:12:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2019-03-12 21:13:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2019-03-12 21:13:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2019-03-12 21:13:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2019-06-18 15:00:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2019-06-18 15:06:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   133919 2019-06-18 15:06:14.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   235857 2019-06-18 15:06:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2019-06-18 15:05:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   136930 2019-06-18 15:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   244171 2019-06-18 15:05:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js
--rw-r--r--   0 runner    (1001) docker     (123)    66341 2019-06-18 15:09:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   120118 2019-06-18 15:09:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
--rw-r--r--   0 runner    (1001) docker     (123)   337274 2019-06-18 15:09:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2019-06-18 15:09:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   435089 2019-06-18 15:09:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   934028 2019-06-18 15:08:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2019-06-18 15:07:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    62814 2019-06-18 15:07:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   128000 2019-06-18 15:06:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js
--rw-r--r--   0 runner    (1001) docker     (123)    67131 2019-06-18 15:09:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2019-06-18 15:09:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
--rw-r--r--   0 runner    (1001) docker     (123)   143573 2019-06-18 15:09:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2019-06-18 15:08:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   123379 2019-06-18 15:08:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   260845 2019-06-18 15:08:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js
--rw-r--r--   0 runner    (1001) docker     (123)    64871 2019-06-18 15:09:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    32370 2019-06-18 15:09:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
--rw-r--r--   0 runner    (1001) docker     (123)   223005 2019-06-18 15:09:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2019-06-18 15:08:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   238580 2019-06-18 15:08:36.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   465673 2019-06-18 15:08:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2019-06-18 15:03:36.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    59932 2019-06-18 15:03:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   171551 2019-06-18 15:03:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2019-06-18 15:04:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    48118 2019-06-18 15:04:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   122752 2019-06-18 15:04:11.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js
--rw-r--r--   0 runner    (1001) docker     (123)   140564 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-support.js
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2019-06-18 15:01:27.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-version.js
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2019-06-18 15:01:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2019-06-18 15:01:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js
--rw-r--r--   0 runner    (1001) docker     (123)   148482 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv.js
--rw-r--r--   0 runner    (1001) docker     (123)    59078 2023-05-05 12:13:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.find.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   125540 2023-05-05 12:13:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    68850 2023-05-05 12:13:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/sugar.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.595175 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.595175 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/
--rwxr-xr-x   0 runner    (1001) docker     (123)    28407 2019-08-28 19:46:06.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7080 2019-08-28 19:46:06.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)     4324 2019-08-28 19:46:06.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.js
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.json
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.json
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.js
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.json
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.js
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.json
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.js
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.js
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.json
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.js
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.json
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.js
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.json
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.js
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.js
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.json
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.js
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.js
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.json
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.json
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.js
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.json
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.js
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.json
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.js
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.json
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.json
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.json
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.js
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.js
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.json
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.js
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.json
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.js
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.json
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.js
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.js
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.json
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.json
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.js
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.json
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.json
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.js
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.json
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.js
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.js
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.json
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.js
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.json
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.js
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.json
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.js
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.json
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.json
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.json
--rw-r--r--   0 runner    (1001) docker     (123)    45293 2019-08-28 19:45:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.css
--rw-r--r--   0 runner    (1001) docker     (123)    40028 2019-08-28 19:46:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1361043 2019-08-28 19:45:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.cjs.js
--rw-r--r--   0 runner    (1001) docker     (123)  1360644 2019-08-28 19:45:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.es.js
--rw-r--r--   0 runner    (1001) docker     (123)  1797606 2019-08-28 19:45:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.js
--rw-r--r--   0 runner    (1001) docker     (123)   480256 2019-08-28 19:45:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2016-10-14 10:25:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs-ogvjs.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/locale/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.633405 nautiluszim-1.1.1/nautiluszim/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/database.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/display_rows.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/info-circle-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/main-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/media_player.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/modal_empty_body.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/modal_title.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/nautilus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim/templates/precompiled.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.633405 nautiluszim-1.1.1/nautiluszim/templates/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)    17430 2020-05-04 16:04:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ScrollMagic.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.637405 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    67871 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   157964 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50935 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115021 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77346 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32546 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   197170 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   504418 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   159515 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   641867 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.637405 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   227980 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   410007 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    80698 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   318045 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   135079 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   256099 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    60010 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194435 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.681405 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2018-08-05 19:09:20.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3g2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3ga.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3gp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/7z.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2018-08-04 18:46:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/accdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/accdt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/adn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ai.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aif.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aifc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aiff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ait.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/amr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2018-06-23 16:58:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ani.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2018-06-23 17:59:22.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/apk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2018-08-04 19:09:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/applescript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ascx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ashx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asmx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2018-07-28 14:27:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aspx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/au.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-08-05 04:08:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/avi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/axd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-24 12:27:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aze.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2018-06-24 12:59:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/blank.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bmp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2018-08-05 17:23:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bowerrc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-06-24 17:12:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/browser.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bz2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2018-06-30 00:29:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cad.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/caf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2018-06-29 23:33:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2018-08-05 20:11:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 03:33:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cgi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2018-07-28 15:17:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/class.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cmd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2018-08-04 16:34:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/codekit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2018-08-04 23:31:11.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/coffee.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/coffeelintignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2018-06-24 16:56:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/compile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2018-08-05 17:39:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/conf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/config.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2018-06-30 00:30:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cpp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2018-07-27 01:50:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cptx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cr2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2018-07-21 22:39:54.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crdownload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-07-16 05:46:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crypt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2018-06-30 00:30:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2018-08-04 23:32:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cson.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csproj.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2018-06-29 21:26:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/css.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2018-07-16 05:44:20.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cue.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-08-05 04:11:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/db.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dbf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/deb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dgn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2018-07-21 20:21:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/diz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dll.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2018-08-04 14:05:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dmg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dng.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:50.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/docb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/docm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/docx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dotm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dotx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2018-07-22 03:47:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:35:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dpj.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2018-06-30 18:59:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ds_store.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2018-07-18 23:08:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dtd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dwg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dxf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2018-08-04 20:17:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/editorconfig.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:16:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/el.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/enc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-07-28 16:31:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/epub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eslintignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/exe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/f4v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2018-07-18 23:43:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fb2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2018-06-23 16:11:22.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fla.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/flac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/flv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2018-08-05 19:39:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gadget.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2018-08-04 20:28:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gdp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2018-06-30 04:29:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gif.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2018-08-04 20:41:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gitattributes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gitignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2018-07-16 05:26:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/go.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-08-05 19:40:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2018-07-19 02:16:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/h.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/handlebars.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hbs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/heic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hsl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/htm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/html.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ibooks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/icns.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2018-06-29 23:32:36.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ics.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2018-07-18 23:46:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/idx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/iff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2018-08-05 17:40:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ifo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/img.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/in.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2018-06-23 16:06:20.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/indd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/inf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ini.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/iso.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2018-07-21 14:30:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/j2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:50.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/java.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jpe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2018-06-29 21:26:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/js.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2018-06-29 21:39:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:37:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jsp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2018-06-29 21:40:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/key.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kf8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2018-08-04 17:53:19.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kmk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ksh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2018-08-04 18:52:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2018-07-28 15:17:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/less.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/licx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:15:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lisp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2018-08-05 16:10:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lnk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2018-06-24 16:25:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/log.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2018-07-21 17:43:54.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lua.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2018-08-05 17:33:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m2v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m3u.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m3u8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2018-08-05 06:23:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4r.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/map.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/master.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2018-07-21 18:59:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/md.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2018-08-05 05:48:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/me.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/midi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mkv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2018-08-05 17:27:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mobi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mod.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mov.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2018-07-18 23:59:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpga.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/msi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2018-06-30 14:04:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/msu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nef.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2018-08-05 18:13:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2018-07-21 20:21:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nfo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-27 02:23:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nix.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/npmignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2018-07-19 00:19:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2018-06-23 11:58:54.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ods.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ogg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ogv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ost.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/otf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ott.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ova.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ovf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/p12.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/p7b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2018-07-19 02:45:38.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pages.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2018-07-19 02:50:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/part.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pcd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2018-06-19 08:11:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pfx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pgp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2018-06-30 18:08:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/phar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2018-06-29 22:06:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/php.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2018-06-30 11:23:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2018-08-04 20:04:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/plist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/png.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/po.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2018-07-21 17:42:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/potx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ppsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ppt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pptm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pptx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/prop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2018-07-21 21:37:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ps1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2018-06-23 16:13:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/psd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/psp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pst.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2018-07-19 00:02:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2018-06-24 17:07:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/py.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2018-07-16 05:23:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pyc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/qt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/raw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/resx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2018-07-28 14:56:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/retry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2018-08-05 16:36:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rpm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rsa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2018-08-05 04:06:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rtf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2018-07-27 04:19:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ru.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/scss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sitemap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/skin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sldm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sldx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2018-07-28 15:15:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sln.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2018-07-21 18:47:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sql.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2018-08-05 19:02:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sqlite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/step.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/stl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2018-08-05 17:36:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2018-06-30 12:16:27.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2018-08-05 19:41:27.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sys.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tcsh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tfignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tga.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tgz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tif.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tiff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2018-08-05 03:53:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tmp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2018-06-30 03:47:11.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/torrent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2018-08-04 17:10:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tsv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2018-08-04 16:11:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ttf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2018-07-27 01:37:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/twig.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/txt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/udf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2018-06-30 00:51:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vbproj.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2018-08-05 18:09:55.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vbs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vcd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2018-06-24 19:18:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vcs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vdx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vmdk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vob.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-07-16 04:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vsd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vst.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vtx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:36:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/war.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wav.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2018-08-05 03:42:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wbk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-08-05 19:41:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webinfo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wma.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wmf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wmv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/woff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/woff2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2018-06-30 14:11:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wsf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2018-07-22 02:04:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xcf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlsm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xltm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xltx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-07-26 04:04:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2018-07-22 03:42:57.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xpi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xrb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2018-07-28 19:17:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xsd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xsl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xspf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/yml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/z.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/zsh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20696 2021-02-15 09:49:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    88145 2022-02-16 10:50:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.689405 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2019-03-12 21:12:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2019-03-12 21:13:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2019-03-12 21:13:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2019-03-12 21:13:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2019-06-18 15:00:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2019-06-18 15:06:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   133919 2019-06-18 15:06:14.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   235857 2019-06-18 15:06:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2019-06-18 15:05:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136930 2019-06-18 15:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   244171 2019-06-18 15:05:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js
+-rw-r--r--   0 runner    (1001) docker     (123)    66341 2019-06-18 15:09:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   120118 2019-06-18 15:09:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
+-rw-r--r--   0 runner    (1001) docker     (123)   337274 2019-06-18 15:09:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2019-06-18 15:09:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   435089 2019-06-18 15:09:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   934028 2019-06-18 15:08:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2019-06-18 15:07:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62814 2019-06-18 15:07:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   128000 2019-06-18 15:06:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js
+-rw-r--r--   0 runner    (1001) docker     (123)    67131 2019-06-18 15:09:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2019-06-18 15:09:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
+-rw-r--r--   0 runner    (1001) docker     (123)   143573 2019-06-18 15:09:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2019-06-18 15:08:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123379 2019-06-18 15:08:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   260845 2019-06-18 15:08:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64871 2019-06-18 15:09:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32370 2019-06-18 15:09:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
+-rw-r--r--   0 runner    (1001) docker     (123)   223005 2019-06-18 15:09:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2019-06-18 15:08:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   238580 2019-06-18 15:08:36.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   465673 2019-06-18 15:08:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2019-06-18 15:03:36.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    59932 2019-06-18 15:03:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   171551 2019-06-18 15:03:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2019-06-18 15:04:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    48118 2019-06-18 15:04:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   122752 2019-06-18 15:04:11.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   140564 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-support.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2019-06-18 15:01:27.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2019-06-18 15:01:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2019-06-18 15:01:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js
+-rw-r--r--   0 runner    (1001) docker     (123)   148482 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv.js
+-rw-r--r--   0 runner    (1001) docker     (123)    59078 2023-05-05 15:50:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/pouchdb.find.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125540 2023-05-05 15:50:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/pouchdb.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    68850 2023-05-05 15:50:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/sugar.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.697405 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.697405 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28407 2019-08-28 19:46:06.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7080 2019-08-28 19:46:06.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4324 2019-08-28 19:46:06.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ba.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/bg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ca.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cy.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/da.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/da.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/el.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/el.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gd.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/he.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/he.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hu.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ja.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ko.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nn.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/oc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/oc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-BR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-PT.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-PT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/tr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/uk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/vi.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/vi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-CN.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-TW.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45293 2019-08-28 19:45:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video-js.css
+-rw-r--r--   0 runner    (1001) docker     (123)    40028 2019-08-28 19:46:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video-js.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1361043 2019-08-28 19:45:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.cjs.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1360644 2019-08-28 19:45:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.es.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1797606 2019-08-28 19:45:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.js
+-rw-r--r--   0 runner    (1001) docker     (123)   480256 2019-08-28 19:45:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2016-10-14 10:25:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs-ogvjs.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/setup.py
```

### Comparing `nautiluszim-1.1.0/CONTRIBUTING.md` & `nautiluszim-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/LICENSE` & `nautiluszim-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/PKG-INFO` & `nautiluszim-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautiluszim
-Version: 1.1.0
+Version: 1.1.1
 Summary: turns a collection of documents into a browsable ZIM file
 Home-page: https://github.com/openzim/nautilus
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_iyfwthmv_/tmpktrty5t3_TarContainer/0/4", line 120, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_iyfwthmv_/tmpktrty5t3_TarContainer/0/4", line 120, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.0 Summary: turns a
+Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.1 Summary: turns a
 collection of documents into a browsable ZIM file Home-page: https://
 github.com/openzim/nautilus Author: kiwix Author-email: reg@kiwix.org License:
 GPLv3+ Keywords: kiwix zim offline Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `nautiluszim-1.1.0/README.md` & `nautiluszim-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/constants.py` & `nautiluszim-1.1.1/nautiluszim/constants.py`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/entrypoint.py` & `nautiluszim-1.1.1/nautiluszim/entrypoint.py`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.mo` & `nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.po` & `nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/locale/messages.pot` & `nautiluszim-1.1.1/nautiluszim/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/scraper.py` & `nautiluszim-1.1.1/nautiluszim/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             save_large_file(self.archive, self.archive_path)
 
     def extract_to_fs(
         self, name: str, failsafe: Optional[bool] = False
     ) -> pathlib.Path:
         """extracting single archive member `name` to filesystem at `to`"""
 
-        with zipfile.ZipFile(self.archive, "r") as zh:
+        with zipfile.ZipFile(self.archive_path, "r") as zh:
             try:
                 normalized_name = zh.extract(member=name, path=self.build_dir)
                 return self.build_dir.joinpath(normalized_name)
             except Exception as exc:
                 logger.error(f"Unable to extract {name} from archive: {exc}")
                 if failsafe:
                     return
@@ -334,15 +334,15 @@
     def test_collection(self):
         with open(self.collection, "r") as fp:
             self.json_collection = [i for i in json.load(fp) if i.get("files", [])]
         nb_items = len(self.json_collection)
         nb_files = sum([len(i.get("files", [])) for i in self.json_collection])
         logger.info(f"Collection loaded. {nb_items} items, {nb_files} files")
 
-        with zipfile.ZipFile(self.archive, "r") as zh:
+        with zipfile.ZipFile(self.archive_path, "r") as zh:
             all_names = zh.namelist()
 
         missing_files = []
         for entry in self.json_collection:
             if not entry.get("files"):
                 continue
             for relative_path in entry["files"]:
```

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/favicon.png` & `nautiluszim-1.1.1/nautiluszim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/home.html` & `nautiluszim-1.1.1/nautiluszim/templates/home.html`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/info-circle-solid.svg` & `nautiluszim-1.1.1/nautiluszim/templates/info-circle-solid.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/init.js` & `nautiluszim-1.1.1/nautiluszim/templates/init.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/main-logo.png` & `nautiluszim-1.1.1/nautiluszim/templates/main-logo.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/nautilus.js` & `nautiluszim-1.1.1/nautiluszim/templates/nautilus.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/precompiled.js` & `nautiluszim-1.1.1/nautiluszim/templates/precompiled.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/styles.css` & `nautiluszim-1.1.1/nautiluszim/templates/styles.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ScrollMagic.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ScrollMagic.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/.DS_Store` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3ga.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3ga.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/7z.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/7z.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aa.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aa.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aac.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aac.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ac.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ac.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/accdb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdt.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/accdt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/adn.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/adn.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ai.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ai.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aif.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aif.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aifc.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aifc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aiff.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aiff.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ait.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ait.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/amr.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/amr.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ani.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ani.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/apk.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/apk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/app.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/app.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/applescript.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/applescript.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asax.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asax.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ascx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ascx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ash.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ash.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ashx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ashx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asmx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asmx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aspx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aspx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/au.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/au.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aup.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aup.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/axd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/axd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bash.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bash.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bin.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bin.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bowerrc.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bowerrc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/browser.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/browser.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bz2.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bz2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cab.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cab.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cad.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cad.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/caf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/caf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cal.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cal.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/catalog.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/catalog.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cer.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cer.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfg.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfm.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfml.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfml.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/class.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/class.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/coffee.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/coffee.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/conf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/conf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/config.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/config.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cpp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cpp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cptx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cptx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crdownload.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crdownload.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crt.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crypt.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crypt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cs.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cs.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csh.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cson.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cson.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csproj.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csproj.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/css.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/css.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cue.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cue.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dat.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dat.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/db.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/db.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dbf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dbf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/deb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/deb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dgn.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dgn.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/diz.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/diz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dmg.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dmg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/download.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/download.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dpj.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dpj.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ds_store.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ds_store.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dtd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dtd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dwg.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dwg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dxf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dxf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/editorconfig.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/editorconfig.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/el.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/el.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/enc.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/enc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eot.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eot.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eps.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eps.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/epub.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/epub.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/exe.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/exe.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/f4v.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/f4v.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fax.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fax.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fb2.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fb2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flac.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/flac.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flv.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/flv.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gdp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gdp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gem.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gem.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gitattributes.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gitattributes.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/go.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/go.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gz.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/handlebars.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/handlebars.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hbs.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hbs.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/htm.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/htm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/html.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/html.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ibooks.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ibooks.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/icns.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/icns.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ico.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ico.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ics.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ics.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/idx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/idx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iff.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/iff.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ifo.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ifo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/img.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/img.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/inf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/inf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ini.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ini.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iso.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/iso.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/j2.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/j2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jar.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/java.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/java.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/js.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/js.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/json.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/json.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jsp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jsx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kf8.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kf8.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kmk.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kmk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ksh.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ksh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kup.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kup.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/less.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/less.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lex.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lex.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/licx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/licx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lisp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lisp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lit.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lit.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lnk.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lnk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lock.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lock.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m3u.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u8.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m3u8.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4a.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4a.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4r.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4r.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/map.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/map.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mc.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mdb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mdf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mi.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mid.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mid.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/midi.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/midi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mk.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mo.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mobi.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mobi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mod.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mod.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mov.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mov.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp2.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp3.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp3.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpa.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpa.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpga.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpga.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpt.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msi.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/msi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msu.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/msu.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nes.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nes.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nfo.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nfo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ods.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ods.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odt.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ogg.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ogg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ost.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ost.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/otf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/otf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ott.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ott.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ova.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ova.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ovf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ovf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pages.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pages.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/part.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/part.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pdb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pem.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pem.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ph.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ph.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/phar.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/phar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/php.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/php.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pkg.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pkg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pl.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pl.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/plist.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/plist.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pm.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/po.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/po.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pom.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pom.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pot.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pot.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ps.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps1.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ps1.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/psd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/psd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pst.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pst.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pub.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pub.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/py.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/py.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pyc.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pyc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/qt.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/qt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ra.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ra.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ram.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ram.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rar.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/resx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/resx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rom.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rom.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rpm.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rpm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rsa.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rsa.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rss.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rss.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ru.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ru.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rub.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rub.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sass.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sass.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/scss.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/scss.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sdf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sdf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sed.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sed.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sh.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sitemap.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sitemap.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/skin.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/skin.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sln.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sln.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sol.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sol.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sql.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sql.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sqlite.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sqlite.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/step.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/step.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/stl.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/stl.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/svg.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/svg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swift.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swift.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sys.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sys.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tar.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tgz.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tgz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tmp.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tmp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/torrent.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/torrent.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ts.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ts.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ttf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ttf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/udf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/udf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbproj.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vbproj.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbs.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vbs.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vcd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vcd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdi.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vdi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vdx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vmdk.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vmdk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vsd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vss.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vss.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vst.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vst.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vsx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vtx.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vtx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/war.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/war.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wav.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wav.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wbk.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wbk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webinfo.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webinfo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wma.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wma.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wmf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wmf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/woff.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff2.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/woff2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wps.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wps.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wsf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wsf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xcf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xcf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xpi.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xpi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xrb.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xrb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xsd.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xsd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xspf.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xspf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xz.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/z.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/z.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zip.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/zip.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zsh.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/zsh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/jquery.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/jquery.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/README.md` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/README.md`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-support.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-support.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-version.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-version.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.find.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/pouchdb.find.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/pouchdb.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/sugar.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/sugar.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.svg` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.woff` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.woff`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ar.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ba.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ba.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/bg.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ca.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cs.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cy.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/da.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/da.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/de.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/de.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/el.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/el.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/en.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/en.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/es.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/es.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fa.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fi.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gd.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gd.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gl.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/he.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/he.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hu.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/it.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/it.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ja.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ko.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nb.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nl.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nn.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nn.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/oc.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pl.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-BR.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-BR.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-PT.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-PT.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ru.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sk.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sv.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/tr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/uk.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/vi.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-CN.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-CN.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-TW.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.json` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-TW.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video-js.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.min.css` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video-js.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.cjs.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.cjs.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.es.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.es.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.min.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs-ogvjs.js` & `nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs-ogvjs.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/nautiluszim.egg-info/PKG-INFO` & `nautiluszim-1.1.1/nautiluszim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautiluszim
-Version: 1.1.0
+Version: 1.1.1
 Summary: turns a collection of documents into a browsable ZIM file
 Home-page: https://github.com/openzim/nautilus
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_iyfwthmv_/tmpktrty5t3_TarContainer/0/578", line 120, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_iyfwthmv_/tmpktrty5t3_TarContainer/0/578", line 120, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.0 Summary: turns a
+Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.1 Summary: turns a
 collection of documents into a browsable ZIM file Home-page: https://
 github.com/openzim/nautilus Author: kiwix Author-email: reg@kiwix.org License:
 GPLv3+ Keywords: kiwix zim offline Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `nautiluszim-1.1.0/nautiluszim.egg-info/SOURCES.txt` & `nautiluszim-1.1.1/nautiluszim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.0/setup.py` & `nautiluszim-1.1.1/setup.py`

 * *Files identical despite different names*

