# Comparing `tmp/nautiluszim-1.0.8.tar.gz` & `tmp/nautiluszim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nautiluszim-1.0.8.tar", last modified: Mon Oct  3 10:52:58 2022, max compression
+gzip compressed data, was "nautiluszim-1.1.0.tar", last modified: Fri May  5 12:13:42 2023, max compression
```

## Comparing `nautiluszim-1.0.8.tar` & `nautiluszim-1.1.0.tar`

### file list

```diff
@@ -1,596 +1,588 @@
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.389935 nautiluszim-1.0.8/
--rw-r--r--   0 reg        (501) staff       (20)     3492 2022-09-30 10:30:58.000000 nautiluszim-1.0.8/CONTRIBUTING.md
--rw-r--r--   0 reg        (501) staff       (20)    35149 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/LICENSE
--rw-r--r--   0 reg        (501) staff       (20)       45 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/MANIFEST.in
--rw-r--r--   0 reg        (501) staff       (20)     3946 2022-10-03 10:52:58.389679 nautiluszim-1.0.8/PKG-INFO
--rw-r--r--   0 reg        (501) staff       (20)     3218 2022-09-30 10:39:10.000000 nautiluszim-1.0.8/README.md
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.187972 nautiluszim-1.0.8/nautiluszim/
--rw-r--r--   0 reg        (501) staff       (20)        6 2022-10-03 10:52:22.000000 nautiluszim-1.0.8/nautiluszim/VERSION
--rw-r--r--   0 reg        (501) staff       (20)        0 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/__init__.py
--rw-r--r--   0 reg        (501) staff       (20)      365 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/__main__.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.192177 nautiluszim-1.0.8/nautiluszim/__pycache__/
--rw-r--r--   0 reg        (501) staff       (20)      138 2021-09-23 14:07:41.000000 nautiluszim-1.0.8/nautiluszim/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      435 2021-09-23 14:07:41.000000 nautiluszim-1.0.8/nautiluszim/__pycache__/__main__.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      989 2021-09-23 14:07:41.000000 nautiluszim-1.0.8/nautiluszim/__pycache__/constants.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)     3732 2021-09-23 14:07:41.000000 nautiluszim-1.0.8/nautiluszim/__pycache__/entrypoint.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)    10251 2022-10-01 16:47:06.000000 nautiluszim-1.0.8/nautiluszim/__pycache__/scraper.cpython-38.pyc
--rw-r--r--   0 reg        (501) staff       (20)      662 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/constants.py
--rw-r--r--   0 reg        (501) staff       (20)     4701 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/entrypoint.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.192678 nautiluszim-1.0.8/nautiluszim/locale/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.181402 nautiluszim-1.0.8/nautiluszim/locale/fr/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.193315 nautiluszim-1.0.8/nautiluszim/locale/fr/LC_MESSAGES/
--rw-r--r--   0 reg        (501) staff       (20)      772 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/locale/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 reg        (501) staff       (20)     1201 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/locale/fr/LC_MESSAGES/messages.po
--rw-r--r--   0 reg        (501) staff       (20)     1047 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/locale/messages.pot
--rw-r--r--   0 reg        (501) staff       (20)    13898 2022-10-01 16:47:05.000000 nautiluszim-1.0.8/nautiluszim/scraper.py
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.196284 nautiluszim-1.0.8/nautiluszim/templates/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.197548 nautiluszim-1.0.8/nautiluszim/templates/assets/
--rw-r--r--   0 reg        (501) staff       (20)      641 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/templates/assets/info-circle-solid.svg
--rw-r--r--   0 reg        (501) staff       (20)     5245 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/templates/assets/main-logo.png
--rw-r--r--   0 reg        (501) staff       (20)     4445 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/templates/assets/styles.css
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.197914 nautiluszim-1.0.8/nautiluszim/templates/assets/templates/
--rw-r--r--   0 reg        (501) staff       (20)    10702 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim/templates/assets/templates/precompiled.js
--rw-r--r--   0 reg        (501) staff       (20)      111 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/templates/database.js
--rw-r--r--   0 reg        (501) staff       (20)      439 2022-09-30 11:57:46.000000 nautiluszim-1.0.8/nautiluszim/templates/display_rows.handlebars
--rw-r--r--   0 reg        (501) staff       (20)     2542 2020-08-26 11:52:47.000000 nautiluszim-1.0.8/nautiluszim/templates/favicon.png
--rw-r--r--   0 reg        (501) staff       (20)     3690 2022-09-30 10:31:23.000000 nautiluszim-1.0.8/nautiluszim/templates/home.html
--rw-r--r--   0 reg        (501) staff       (20)      619 2022-01-25 08:39:45.000000 nautiluszim-1.0.8/nautiluszim/templates/init.js
--rw-r--r--   0 reg        (501) staff       (20)      297 2022-10-01 16:44:51.000000 nautiluszim-1.0.8/nautiluszim/templates/media_player.handlebars
--rw-r--r--   0 reg        (501) staff       (20)       23 2022-01-25 08:04:08.000000 nautiluszim-1.0.8/nautiluszim/templates/modal_empty_body.handlebars
--rw-r--r--   0 reg        (501) staff       (20)       10 2022-01-25 08:42:34.000000 nautiluszim-1.0.8/nautiluszim/templates/modal_title.handlebars
--rw-r--r--   0 reg        (501) staff       (20)    19672 2022-10-01 16:48:27.000000 nautiluszim-1.0.8/nautiluszim/templates/nautilus.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.204180 nautiluszim-1.0.8/nautiluszim/templates/vendors/
--rw-r--r--   0 reg        (501) staff       (20)    17430 2020-05-04 16:04:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ScrollMagic.min.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.182297 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.212731 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/
--rw-r--r--   0 reg        (501) staff       (20)    67871 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 reg        (501) staff       (20)   157964 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 reg        (501) staff       (20)    50935 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 reg        (501) staff       (20)   115021 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 reg        (501) staff       (20)     4793 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 reg        (501) staff       (20)    77346 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 reg        (501) staff       (20)     3927 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 reg        (501) staff       (20)    32546 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 reg        (501) staff       (20)   197170 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css
--rw-r--r--   0 reg        (501) staff       (20)   504418 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 reg        (501) staff       (20)   159515 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 reg        (501) staff       (20)   641867 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.221323 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/
--rw-r--r--   0 reg        (501) staff       (20)   227980 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 reg        (501) staff       (20)   410007 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 reg        (501) staff       (20)    80698 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 reg        (501) staff       (20)   318045 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 reg        (501) staff       (20)   135079 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js
--rw-r--r--   0 reg        (501) staff       (20)   256099 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 reg        (501) staff       (20)    60010 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 reg        (501) staff       (20)   194435 2019-11-28 12:59:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.327416 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/
--rw-r--r--   0 reg        (501) staff       (20)    10244 2018-08-05 19:09:20.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/.DS_Store
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/3g2.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/3ga.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/3gp.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/7z.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aa.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aac.svg
--rw-r--r--   0 reg        (501) staff       (20)      555 2018-08-04 18:46:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ac.svg
--rw-r--r--   0 reg        (501) staff       (20)      985 2018-08-05 18:46:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/accdb.svg
--rw-r--r--   0 reg        (501) staff       (20)      982 2018-08-05 18:47:24.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/accdt.svg
--rw-r--r--   0 reg        (501) staff       (20)      982 2018-08-05 18:47:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/adn.svg
--rw-r--r--   0 reg        (501) staff       (20)      515 2018-06-30 00:55:16.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ai.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aif.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aifc.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aiff.svg
--rw-r--r--   0 reg        (501) staff       (20)      515 2018-06-30 00:55:16.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ait.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/amr.svg
--rw-r--r--   0 reg        (501) staff       (20)     1093 2018-06-23 16:58:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ani.svg
--rw-r--r--   0 reg        (501) staff       (20)      829 2018-06-23 17:59:22.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/apk.svg
--rw-r--r--   0 reg        (501) staff       (20)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/app.svg
--rw-r--r--   0 reg        (501) staff       (20)     1412 2018-08-04 19:09:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/applescript.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asax.svg
--rw-r--r--   0 reg        (501) staff       (20)      452 2018-06-19 09:52:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asc.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ascx.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asf.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ash.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ashx.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asmx.svg
--rw-r--r--   0 reg        (501) staff       (20)      730 2018-07-28 14:27:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asp.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aspx.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asx.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/au.svg
--rw-r--r--   0 reg        (501) staff       (20)      839 2018-06-24 12:06:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aup.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-08-05 04:08:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/avi.svg
--rw-r--r--   0 reg        (501) staff       (20)      905 2018-07-28 16:28:25.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/axd.svg
--rw-r--r--   0 reg        (501) staff       (20)      451 2018-06-24 12:27:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aze.svg
--rw-r--r--   0 reg        (501) staff       (20)      309 2018-06-24 12:59:34.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bak.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bash.svg
--rw-r--r--   0 reg        (501) staff       (20)      304 2018-06-30 00:57:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bat.svg
--rw-r--r--   0 reg        (501) staff       (20)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bin.svg
--rw-r--r--   0 reg        (501) staff       (20)      452 2018-06-19 09:52:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/blank.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bmp.svg
--rw-r--r--   0 reg        (501) staff       (20)     5139 2018-08-05 17:23:34.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bowerrc.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bpg.svg
--rw-r--r--   0 reg        (501) staff       (20)     1434 2018-06-24 17:12:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/browser.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bz2.svg
--rw-r--r--   0 reg        (501) staff       (20)      407 2018-06-30 00:29:39.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/c.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cab.svg
--rw-r--r--   0 reg        (501) staff       (20)      924 2018-06-30 04:01:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cad.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/caf.svg
--rw-r--r--   0 reg        (501) staff       (20)     1406 2018-06-29 23:33:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cal.svg
--rw-r--r--   0 reg        (501) staff       (20)     2373 2018-08-05 20:11:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/catalog.json
--rw-r--r--   0 reg        (501) staff       (20)      905 2018-07-28 16:28:25.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cd.svg
--rw-r--r--   0 reg        (501) staff       (20)      607 2018-06-24 16:28:18.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cer.svg
--rw-r--r--   0 reg        (501) staff       (20)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cfg.svg
--rw-r--r--   0 reg        (501) staff       (20)      596 2018-07-27 01:55:44.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cfm.svg
--rw-r--r--   0 reg        (501) staff       (20)      596 2018-07-27 01:55:44.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cfml.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-08-05 03:33:31.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cgi.svg
--rw-r--r--   0 reg        (501) staff       (20)     1390 2018-07-28 15:17:03.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/class.svg
--rw-r--r--   0 reg        (501) staff       (20)      304 2018-06-30 00:57:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cmd.svg
--rw-r--r--   0 reg        (501) staff       (20)      362 2018-08-04 16:34:03.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/codekit.svg
--rw-r--r--   0 reg        (501) staff       (20)     1325 2018-08-04 23:31:11.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/coffee.svg
--rw-r--r--   0 reg        (501) staff       (20)      451 2018-06-23 18:15:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/coffeelintignore.svg
--rw-r--r--   0 reg        (501) staff       (20)      304 2018-06-30 00:57:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/com.svg
--rw-r--r--   0 reg        (501) staff       (20)      461 2018-06-24 16:56:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/compile.svg
--rw-r--r--   0 reg        (501) staff       (20)     1086 2018-08-05 17:39:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/conf.svg
--rw-r--r--   0 reg        (501) staff       (20)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/config.svg
--rw-r--r--   0 reg        (501) staff       (20)      583 2018-06-30 00:30:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cpp.svg
--rw-r--r--   0 reg        (501) staff       (20)      675 2018-07-27 01:50:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cptx.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cr2.svg
--rw-r--r--   0 reg        (501) staff       (20)      709 2018-07-21 22:39:54.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/crdownload.svg
--rw-r--r--   0 reg        (501) staff       (20)      607 2018-06-24 16:28:18.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/crt.svg
--rw-r--r--   0 reg        (501) staff       (20)      607 2018-07-16 05:46:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/crypt.svg
--rw-r--r--   0 reg        (501) staff       (20)      655 2018-06-30 00:30:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cs.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/csh.svg
--rw-r--r--   0 reg        (501) staff       (20)     1365 2018-08-04 23:32:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cson.svg
--rw-r--r--   0 reg        (501) staff       (20)      733 2018-06-24 13:12:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/csproj.svg
--rw-r--r--   0 reg        (501) staff       (20)      699 2018-06-29 21:26:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/css.svg
--rw-r--r--   0 reg        (501) staff       (20)      429 2018-07-18 23:02:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/csv.svg
--rw-r--r--   0 reg        (501) staff       (20)      830 2018-07-16 05:44:20.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cue.svg
--rw-r--r--   0 reg        (501) staff       (20)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dat.svg
--rw-r--r--   0 reg        (501) staff       (20)     1226 2018-08-05 04:11:39.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/db.svg
--rw-r--r--   0 reg        (501) staff       (20)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dbf.svg
--rw-r--r--   0 reg        (501) staff       (20)      517 2018-06-29 23:06:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/deb.svg
--rw-r--r--   0 reg        (501) staff       (20)      924 2018-06-30 04:01:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dgn.svg
--rw-r--r--   0 reg        (501) staff       (20)      400 2018-06-24 17:31:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dist.svg
--rw-r--r--   0 reg        (501) staff       (20)     1621 2018-07-21 20:21:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/diz.svg
--rw-r--r--   0 reg        (501) staff       (20)      360 2018-06-24 13:07:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dll.svg
--rw-r--r--   0 reg        (501) staff       (20)      615 2018-08-04 14:05:39.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dmg.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dng.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-06-19 06:59:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/doc.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-08-05 04:11:50.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/docb.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-06-19 06:59:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/docm.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-08-05 04:11:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/docx.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-06-19 06:59:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dot.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-06-19 06:59:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dotm.svg
--rw-r--r--   0 reg        (501) staff       (20)      319 2018-06-19 06:59:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dotx.svg
--rw-r--r--   0 reg        (501) staff       (20)      740 2018-07-22 03:47:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/download.svg
--rw-r--r--   0 reg        (501) staff       (20)     1192 2018-08-05 19:35:29.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dpj.svg
--rw-r--r--   0 reg        (501) staff       (20)     1242 2018-06-30 18:59:59.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ds_store.svg
--rw-r--r--   0 reg        (501) staff       (20)      555 2018-07-18 23:08:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dtd.svg
--rw-r--r--   0 reg        (501) staff       (20)      924 2018-06-30 04:01:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dwg.svg
--rw-r--r--   0 reg        (501) staff       (20)      924 2018-06-30 04:01:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dxf.svg
--rw-r--r--   0 reg        (501) staff       (20)     1089 2018-08-04 20:17:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/editorconfig.svg
--rw-r--r--   0 reg        (501) staff       (20)      632 2018-08-05 17:16:26.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/el.svg
--rw-r--r--   0 reg        (501) staff       (20)      607 2018-06-24 16:28:18.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/enc.svg
--rw-r--r--   0 reg        (501) staff       (20)     1176 2018-07-28 16:31:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/eot.svg
--rw-r--r--   0 reg        (501) staff       (20)      518 2018-06-30 04:05:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/eps.svg
--rw-r--r--   0 reg        (501) staff       (20)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/epub.svg
--rw-r--r--   0 reg        (501) staff       (20)      451 2018-06-23 18:15:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/eslintignore.svg
--rw-r--r--   0 reg        (501) staff       (20)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/exe.svg
--rw-r--r--   0 reg        (501) staff       (20)      558 2018-07-28 14:46:24.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/f4v.svg
--rw-r--r--   0 reg        (501) staff       (20)     1289 2018-07-18 23:43:24.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/fax.svg
--rw-r--r--   0 reg        (501) staff       (20)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/fb2.svg
--rw-r--r--   0 reg        (501) staff       (20)      343 2018-06-23 16:11:22.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/fla.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/flac.svg
--rw-r--r--   0 reg        (501) staff       (20)      558 2018-07-28 14:46:24.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/flv.svg
--rw-r--r--   0 reg        (501) staff       (20)      288 2018-08-05 19:39:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/folder.svg
--rw-r--r--   0 reg        (501) staff       (20)      360 2018-06-24 13:07:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gadget.svg
--rw-r--r--   0 reg        (501) staff       (20)      994 2018-08-04 20:28:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gdp.svg
--rw-r--r--   0 reg        (501) staff       (20)      949 2018-06-30 04:29:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gem.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gif.svg
--rw-r--r--   0 reg        (501) staff       (20)      694 2018-08-04 20:41:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gitattributes.svg
--rw-r--r--   0 reg        (501) staff       (20)      451 2018-06-23 18:15:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gitignore.svg
--rw-r--r--   0 reg        (501) staff       (20)     1050 2018-07-16 05:26:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/go.svg
--rw-r--r--   0 reg        (501) staff       (20)      478 2018-06-24 19:11:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gpg.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-08-05 19:40:29.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gz.svg
--rw-r--r--   0 reg        (501) staff       (20)      322 2018-07-19 02:16:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/h.svg
--rw-r--r--   0 reg        (501) staff       (20)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/handlebars.svg
--rw-r--r--   0 reg        (501) staff       (20)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/hbs.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/heic.svg
--rw-r--r--   0 reg        (501) staff       (20)      416 2018-07-27 03:50:34.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/hs.svg
--rw-r--r--   0 reg        (501) staff       (20)      416 2018-07-27 03:50:34.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/hsl.svg
--rw-r--r--   0 reg        (501) staff       (20)      593 2018-06-29 21:25:38.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/htm.svg
--rw-r--r--   0 reg        (501) staff       (20)      593 2018-06-29 21:25:38.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/html.svg
--rw-r--r--   0 reg        (501) staff       (20)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ibooks.svg
--rw-r--r--   0 reg        (501) staff       (20)      766 2018-06-23 16:52:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/icns.svg
--rw-r--r--   0 reg        (501) staff       (20)      766 2018-06-23 16:52:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ico.svg
--rw-r--r--   0 reg        (501) staff       (20)      591 2018-06-29 23:32:36.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ics.svg
--rw-r--r--   0 reg        (501) staff       (20)      644 2018-07-18 23:46:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/idx.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/iff.svg
--rw-r--r--   0 reg        (501) staff       (20)      856 2018-08-05 17:40:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ifo.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/image.svg
--rw-r--r--   0 reg        (501) staff       (20)      857 2018-06-23 17:49:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/img.svg
--rw-r--r--   0 reg        (501) staff       (20)      452 2018-06-19 09:52:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/in.svg
--rw-r--r--   0 reg        (501) staff       (20)      504 2018-06-23 16:06:20.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/indd.svg
--rw-r--r--   0 reg        (501) staff       (20)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/inf.svg
--rw-r--r--   0 reg        (501) staff       (20)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ini.svg
--rw-r--r--   0 reg        (501) staff       (20)      857 2018-06-23 17:49:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/iso.svg
--rw-r--r--   0 reg        (501) staff       (20)     1807 2018-07-21 14:30:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/j2.svg
--rw-r--r--   0 reg        (501) staff       (20)     1255 2018-08-05 19:36:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jar.svg
--rw-r--r--   0 reg        (501) staff       (20)     1255 2018-08-05 19:36:50.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/java.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jpe.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jpeg.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jpg.svg
--rw-r--r--   0 reg        (501) staff       (20)      513 2018-06-29 21:26:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/js.svg
--rw-r--r--   0 reg        (501) staff       (20)     2271 2018-06-29 21:39:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/json.svg
--rw-r--r--   0 reg        (501) staff       (20)     1255 2018-08-05 19:37:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jsp.svg
--rw-r--r--   0 reg        (501) staff       (20)     2265 2018-06-29 21:40:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jsx.svg
--rw-r--r--   0 reg        (501) staff       (20)      478 2018-06-24 19:11:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/key.svg
--rw-r--r--   0 reg        (501) staff       (20)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/kf8.svg
--rw-r--r--   0 reg        (501) staff       (20)     1358 2018-08-04 17:53:19.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/kmk.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ksh.svg
--rw-r--r--   0 reg        (501) staff       (20)      698 2018-08-04 18:52:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/kup.svg
--rw-r--r--   0 reg        (501) staff       (20)     1378 2018-07-28 15:17:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/less.svg
--rw-r--r--   0 reg        (501) staff       (20)      545 2018-07-19 02:56:21.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lex.svg
--rw-r--r--   0 reg        (501) staff       (20)      733 2018-06-24 13:12:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/licx.svg
--rw-r--r--   0 reg        (501) staff       (20)      632 2018-08-05 17:15:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lisp.svg
--rw-r--r--   0 reg        (501) staff       (20)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lit.svg
--rw-r--r--   0 reg        (501) staff       (20)      957 2018-08-05 16:10:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lnk.svg
--rw-r--r--   0 reg        (501) staff       (20)      610 2018-06-24 16:25:37.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lock.svg
--rw-r--r--   0 reg        (501) staff       (20)      287 2018-06-19 09:38:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/log.svg
--rw-r--r--   0 reg        (501) staff       (20)      465 2018-07-21 17:43:54.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lua.svg
--rw-r--r--   0 reg        (501) staff       (20)     2079 2018-08-05 17:33:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m2v.svg
--rw-r--r--   0 reg        (501) staff       (20)      839 2018-06-24 12:06:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m3u.svg
--rw-r--r--   0 reg        (501) staff       (20)      839 2018-06-24 12:06:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m3u8.svg
--rw-r--r--   0 reg        (501) staff       (20)     1206 2018-08-05 06:23:21.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4a.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4r.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4v.svg
--rw-r--r--   0 reg        (501) staff       (20)      791 2018-08-05 05:46:31.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/map.svg
--rw-r--r--   0 reg        (501) staff       (20)      452 2018-06-19 09:52:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/master.svg
--rw-r--r--   0 reg        (501) staff       (20)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mc.svg
--rw-r--r--   0 reg        (501) staff       (20)      353 2018-07-21 18:59:04.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/md.svg
--rw-r--r--   0 reg        (501) staff       (20)      985 2018-08-05 18:46:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mdb.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mdf.svg
--rw-r--r--   0 reg        (501) staff       (20)      307 2018-08-05 05:48:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/me.svg
--rw-r--r--   0 reg        (501) staff       (20)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mi.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mid.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/midi.svg
--rw-r--r--   0 reg        (501) staff       (20)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mk.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mkv.svg
--rw-r--r--   0 reg        (501) staff       (20)      482 2018-08-05 17:27:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mm.svg
--rw-r--r--   0 reg        (501) staff       (20)      545 2018-07-19 02:56:21.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mo.svg
--rw-r--r--   0 reg        (501) staff       (20)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mobi.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mod.svg
--rw-r--r--   0 reg        (501) staff       (20)      665 2018-06-30 03:56:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mov.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mp2.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mp3.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mp4.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpa.svg
--rw-r--r--   0 reg        (501) staff       (20)      913 2018-07-18 23:59:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpd.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpe.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpeg.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpg.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpga.svg
--rw-r--r--   0 reg        (501) staff       (20)      916 2018-07-18 23:55:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpp.svg
--rw-r--r--   0 reg        (501) staff       (20)      916 2018-07-18 23:55:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpt.svg
--rw-r--r--   0 reg        (501) staff       (20)      517 2018-06-29 23:06:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/msi.svg
--rw-r--r--   0 reg        (501) staff       (20)      514 2018-06-30 14:04:34.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/msu.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/nef.svg
--rw-r--r--   0 reg        (501) staff       (20)      589 2018-08-05 18:13:39.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/nes.svg
--rw-r--r--   0 reg        (501) staff       (20)      838 2018-07-21 20:21:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/nfo.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-07-27 02:23:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/nix.svg
--rw-r--r--   0 reg        (501) staff       (20)      451 2018-06-23 18:15:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/npmignore.svg
--rw-r--r--   0 reg        (501) staff       (20)     1371 2018-07-19 00:19:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/odb.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2022-10-03 10:52:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/odp.svg
--rw-r--r--   0 reg        (501) staff       (20)      671 2018-06-23 11:58:54.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ods.svg
--rw-r--r--   0 reg        (501) staff       (20)      741 2018-07-19 02:37:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/odt.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ogg.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ogv.svg
--rw-r--r--   0 reg        (501) staff       (20)      580 2018-07-19 00:11:29.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ost.svg
--rw-r--r--   0 reg        (501) staff       (20)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/otf.svg
--rw-r--r--   0 reg        (501) staff       (20)      741 2018-07-19 02:37:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ott.svg
--rw-r--r--   0 reg        (501) staff       (20)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ova.svg
--rw-r--r--   0 reg        (501) staff       (20)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ovf.svg
--rw-r--r--   0 reg        (501) staff       (20)      478 2018-06-24 19:11:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/p12.svg
--rw-r--r--   0 reg        (501) staff       (20)      478 2018-06-24 19:11:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/p7b.svg
--rw-r--r--   0 reg        (501) staff       (20)     1427 2018-07-19 02:45:38.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pages.svg
--rw-r--r--   0 reg        (501) staff       (20)     1019 2018-07-19 02:50:59.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/part.svg
--rw-r--r--   0 reg        (501) staff       (20)      452 2018-06-19 09:52:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pcd.svg
--rw-r--r--   0 reg        (501) staff       (20)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pdb.svg
--rw-r--r--   0 reg        (501) staff       (20)     1047 2018-06-19 08:11:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pdf.svg
--rw-r--r--   0 reg        (501) staff       (20)      607 2018-06-24 16:28:18.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pem.svg
--rw-r--r--   0 reg        (501) staff       (20)      478 2018-06-24 19:11:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pfx.svg
--rw-r--r--   0 reg        (501) staff       (20)      478 2018-06-24 19:11:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pgp.svg
--rw-r--r--   0 reg        (501) staff       (20)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ph.svg
--rw-r--r--   0 reg        (501) staff       (20)     1244 2018-06-30 18:08:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/phar.svg
--rw-r--r--   0 reg        (501) staff       (20)     1184 2018-06-29 22:06:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/php.svg
--rw-r--r--   0 reg        (501) staff       (20)      517 2018-06-29 23:06:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pkg.svg
--rw-r--r--   0 reg        (501) staff       (20)     1829 2018-06-30 11:23:18.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pl.svg
--rw-r--r--   0 reg        (501) staff       (20)     1418 2018-08-04 20:04:37.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/plist.svg
--rw-r--r--   0 reg        (501) staff       (20)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pm.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/png.svg
--rw-r--r--   0 reg        (501) staff       (20)      545 2018-07-19 02:56:21.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/po.svg
--rw-r--r--   0 reg        (501) staff       (20)      663 2018-07-21 17:42:25.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pom.svg
--rw-r--r--   0 reg        (501) staff       (20)      545 2018-07-19 02:56:21.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pot.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2018-06-19 10:03:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/potx.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2018-06-19 10:03:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pps.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2018-06-19 10:03:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ppsx.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2018-06-19 10:03:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ppt.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2018-06-19 10:03:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pptm.svg
--rw-r--r--   0 reg        (501) staff       (20)      399 2018-06-19 10:03:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pptx.svg
--rw-r--r--   0 reg        (501) staff       (20)      452 2018-06-19 09:52:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/prop.svg
--rw-r--r--   0 reg        (501) staff       (20)      518 2018-06-30 04:05:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ps.svg
--rw-r--r--   0 reg        (501) staff       (20)     1644 2018-07-21 21:37:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ps1.svg
--rw-r--r--   0 reg        (501) staff       (20)      702 2018-06-23 16:13:37.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/psd.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/psp.svg
--rw-r--r--   0 reg        (501) staff       (20)      580 2018-07-19 00:11:29.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pst.svg
--rw-r--r--   0 reg        (501) staff       (20)      627 2018-07-19 00:02:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pub.svg
--rw-r--r--   0 reg        (501) staff       (20)     1824 2018-06-24 17:07:41.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/py.svg
--rw-r--r--   0 reg        (501) staff       (20)     1801 2018-07-16 05:23:26.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pyc.svg
--rw-r--r--   0 reg        (501) staff       (20)      665 2018-06-30 03:56:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/qt.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ra.svg
--rw-r--r--   0 reg        (501) staff       (20)      839 2018-06-24 12:06:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ram.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rar.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/raw.svg
--rw-r--r--   0 reg        (501) staff       (20)      912 2018-06-24 14:07:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rb.svg
--rw-r--r--   0 reg        (501) staff       (20)      287 2018-06-19 09:38:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rdf.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-06-23 18:18:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/resx.svg
--rw-r--r--   0 reg        (501) staff       (20)      470 2018-07-28 14:56:03.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/retry.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rm.svg
--rw-r--r--   0 reg        (501) staff       (20)      563 2018-08-05 16:36:39.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rom.svg
--rw-r--r--   0 reg        (501) staff       (20)      517 2018-06-29 23:06:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rpm.svg
--rw-r--r--   0 reg        (501) staff       (20)      607 2018-06-24 16:28:18.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rsa.svg
--rw-r--r--   0 reg        (501) staff       (20)      668 2018-08-05 04:06:37.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rss.svg
--rw-r--r--   0 reg        (501) staff       (20)      287 2018-06-19 09:38:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rtf.svg
--rw-r--r--   0 reg        (501) staff       (20)      926 2018-07-27 04:19:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ru.svg
--rw-r--r--   0 reg        (501) staff       (20)      912 2018-06-24 14:07:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rub.svg
--rw-r--r--   0 reg        (501) staff       (20)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sass.svg
--rw-r--r--   0 reg        (501) staff       (20)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/scss.svg
--rw-r--r--   0 reg        (501) staff       (20)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sdf.svg
--rw-r--r--   0 reg        (501) staff       (20)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sed.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sh.svg
--rw-r--r--   0 reg        (501) staff       (20)      791 2018-08-05 05:46:31.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sitemap.svg
--rw-r--r--   0 reg        (501) staff       (20)      905 2018-07-28 16:28:25.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/skin.svg
--rw-r--r--   0 reg        (501) staff       (20)      391 2018-08-05 19:09:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sldm.svg
--rw-r--r--   0 reg        (501) staff       (20)      391 2018-08-05 19:09:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sldx.svg
--rw-r--r--   0 reg        (501) staff       (20)      906 2018-07-28 15:15:35.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sln.svg
--rw-r--r--   0 reg        (501) staff       (20)     1177 2018-07-21 18:47:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sol.svg
--rw-r--r--   0 reg        (501) staff       (20)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sql.svg
--rw-r--r--   0 reg        (501) staff       (20)     1234 2018-08-05 19:02:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sqlite.svg
--rw-r--r--   0 reg        (501) staff       (20)      924 2018-06-30 04:01:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/step.svg
--rw-r--r--   0 reg        (501) staff       (20)      924 2018-06-30 04:01:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/stl.svg
--rw-r--r--   0 reg        (501) staff       (20)      518 2018-06-30 04:05:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/svg.svg
--rw-r--r--   0 reg        (501) staff       (20)      557 2018-08-05 17:36:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/swd.svg
--rw-r--r--   0 reg        (501) staff       (20)      558 2018-07-28 14:46:24.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/swf.svg
--rw-r--r--   0 reg        (501) staff       (20)      847 2018-06-30 12:16:27.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/swift.svg
--rw-r--r--   0 reg        (501) staff       (20)     1415 2018-08-05 19:41:27.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sys.svg
--rw-r--r--   0 reg        (501) staff       (20)      517 2018-06-29 23:06:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tar.svg
--rw-r--r--   0 reg        (501) staff       (20)      304 2018-06-30 00:57:52.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tcsh.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-07-17 22:25:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tex.svg
--rw-r--r--   0 reg        (501) staff       (20)      451 2018-06-23 18:15:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tfignore.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tga.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tgz.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tif.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tiff.svg
--rw-r--r--   0 reg        (501) staff       (20)     1399 2018-08-05 03:53:26.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tmp.svg
--rw-r--r--   0 reg        (501) staff       (20)      979 2018-06-30 03:47:11.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/torrent.svg
--rw-r--r--   0 reg        (501) staff       (20)      831 2018-08-04 17:10:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ts.svg
--rw-r--r--   0 reg        (501) staff       (20)      429 2018-07-18 23:02:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tsv.svg
--rw-r--r--   0 reg        (501) staff       (20)      807 2018-08-04 16:11:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ttf.svg
--rw-r--r--   0 reg        (501) staff       (20)      358 2018-07-27 01:37:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/twig.svg
--rw-r--r--   0 reg        (501) staff       (20)      287 2018-06-19 09:38:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/txt.svg
--rw-r--r--   0 reg        (501) staff       (20)      857 2018-06-23 17:49:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/udf.svg
--rw-r--r--   0 reg        (501) staff       (20)      555 2018-06-30 00:51:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vb.svg
--rw-r--r--   0 reg        (501) staff       (20)      733 2018-06-24 13:12:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vbproj.svg
--rw-r--r--   0 reg        (501) staff       (20)     2157 2018-08-05 18:09:55.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vbs.svg
--rw-r--r--   0 reg        (501) staff       (20)      857 2018-06-23 17:49:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vcd.svg
--rw-r--r--   0 reg        (501) staff       (20)      453 2018-06-24 19:18:25.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vcs.svg
--rw-r--r--   0 reg        (501) staff       (20)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vdi.svg
--rw-r--r--   0 reg        (501) staff       (20)      845 2018-06-30 19:13:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vdx.svg
--rw-r--r--   0 reg        (501) staff       (20)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vmdk.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vob.svg
--rw-r--r--   0 reg        (501) staff       (20)      736 2018-07-16 04:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg
--rw-r--r--   0 reg        (501) staff       (20)      845 2018-06-30 19:13:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vsd.svg
--rw-r--r--   0 reg        (501) staff       (20)      845 2018-06-30 19:13:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vss.svg
--rw-r--r--   0 reg        (501) staff       (20)      845 2018-06-30 19:13:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vst.svg
--rw-r--r--   0 reg        (501) staff       (20)      845 2018-06-30 19:13:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vsx.svg
--rw-r--r--   0 reg        (501) staff       (20)      845 2018-06-30 19:13:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vtx.svg
--rw-r--r--   0 reg        (501) staff       (20)     1192 2018-08-05 19:36:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/war.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wav.svg
--rw-r--r--   0 reg        (501) staff       (20)      716 2018-08-05 03:42:49.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wbk.svg
--rw-r--r--   0 reg        (501) staff       (20)     1434 2018-08-05 19:41:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/webinfo.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/webm.svg
--rw-r--r--   0 reg        (501) staff       (20)      326 2018-06-19 09:52:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/webp.svg
--rw-r--r--   0 reg        (501) staff       (20)      531 2018-06-22 22:20:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wma.svg
--rw-r--r--   0 reg        (501) staff       (20)      518 2018-06-30 04:05:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wmf.svg
--rw-r--r--   0 reg        (501) staff       (20)      496 2018-06-22 22:03:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wmv.svg
--rw-r--r--   0 reg        (501) staff       (20)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/woff.svg
--rw-r--r--   0 reg        (501) staff       (20)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/woff2.svg
--rw-r--r--   0 reg        (501) staff       (20)      685 2018-06-30 14:11:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wps.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wsf.svg
--rw-r--r--   0 reg        (501) staff       (20)      400 2018-06-24 17:31:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xaml.svg
--rw-r--r--   0 reg        (501) staff       (20)     1860 2018-07-22 02:04:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xcf.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xlm.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xls.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xlsm.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xlsx.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xlt.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xltm.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-06-19 07:21:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xltx.svg
--rw-r--r--   0 reg        (501) staff       (20)      400 2018-07-26 04:04:59.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xml.svg
--rw-r--r--   0 reg        (501) staff       (20)      722 2018-07-22 03:42:57.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xpi.svg
--rw-r--r--   0 reg        (501) staff       (20)      400 2018-06-24 17:31:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xps.svg
--rw-r--r--   0 reg        (501) staff       (20)      517 2018-06-29 23:06:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xrb.svg
--rw-r--r--   0 reg        (501) staff       (20)     1413 2018-07-28 19:17:51.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xsd.svg
--rw-r--r--   0 reg        (501) staff       (20)      400 2018-06-24 17:31:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xsl.svg
--rw-r--r--   0 reg        (501) staff       (20)      839 2018-06-24 12:06:00.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xspf.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xz.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-07-17 22:25:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/yaml.svg
--rw-r--r--   0 reg        (501) staff       (20)      327 2018-07-17 22:25:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/yml.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/z.svg
--rw-r--r--   0 reg        (501) staff       (20)      703 2018-06-23 15:40:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/zip.svg
--rw-r--r--   0 reg        (501) staff       (20)      630 2018-06-23 18:48:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/zsh.svg
--rw-r--r--   0 reg        (501) staff       (20)    20679 2020-04-03 18:10:22.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.6.js
--rw-rw-rw-   0 reg        (501) staff       (20)    20696 2022-01-25 08:23:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js
--rw-r--r--   0 reg        (501) staff       (20)    88145 2019-05-01 21:14:27.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/jquery.min.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.352770 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/
--rw-r--r--   0 reg        (501) staff       (20)     1116 2019-03-12 21:12:44.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING
--rw-r--r--   0 reg        (501) staff       (20)     1317 2019-03-12 21:13:31.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt
--rw-r--r--   0 reg        (501) staff       (20)     1466 2019-03-12 21:13:31.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt
--rw-r--r--   0 reg        (501) staff       (20)     1928 2019-03-12 21:13:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt
--rw-r--r--   0 reg        (501) staff       (20)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt
--rw-r--r--   0 reg        (501) staff       (20)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt
--rw-r--r--   0 reg        (501) staff       (20)      732 2019-03-12 21:13:31.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt
--rw-r--r--   0 reg        (501) staff       (20)     1537 2019-03-12 21:13:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt
--rw-r--r--   0 reg        (501) staff       (20)     1436 2019-03-12 21:13:32.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt
--rw-r--r--   0 reg        (501) staff       (20)    18635 2019-06-18 15:00:08.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/README.md
--rw-r--r--   0 reg        (501) staff       (20)     3327 2019-06-18 15:01:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf
--rw-r--r--   0 reg        (501) staff       (20)     9647 2019-06-18 15:06:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   133919 2019-06-18 15:06:14.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   235857 2019-06-18 15:06:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js
--rw-r--r--   0 reg        (501) staff       (20)     9565 2019-06-18 15:05:09.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   136930 2019-06-18 15:05:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   244171 2019-06-18 15:05:03.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js
--rw-r--r--   0 reg        (501) staff       (20)    66341 2019-06-18 15:09:59.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   120118 2019-06-18 15:09:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
--rw-r--r--   0 reg        (501) staff       (20)   337274 2019-06-18 15:09:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:56.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
--rw-r--r--   0 reg        (501) staff       (20)    11462 2019-06-18 15:09:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   435089 2019-06-18 15:09:02.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   934028 2019-06-18 15:08:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js
--rw-r--r--   0 reg        (501) staff       (20)    10450 2019-06-18 15:07:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    62814 2019-06-18 15:07:01.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   128000 2019-06-18 15:06:59.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js
--rw-r--r--   0 reg        (501) staff       (20)    67131 2019-06-18 15:09:44.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)     7758 2019-06-18 15:09:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
--rw-r--r--   0 reg        (501) staff       (20)   143573 2019-06-18 15:09:44.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:42.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
--rw-r--r--   0 reg        (501) staff       (20)    11878 2019-06-18 15:08:15.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   123379 2019-06-18 15:08:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   260845 2019-06-18 15:08:10.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js
--rw-r--r--   0 reg        (501) staff       (20)    64871 2019-06-18 15:09:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    32370 2019-06-18 15:09:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
--rw-r--r--   0 reg        (501) staff       (20)   223005 2019-06-18 15:09:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)    10452 2019-06-18 15:09:46.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
--rw-r--r--   0 reg        (501) staff       (20)    11883 2019-06-18 15:08:40.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)   238580 2019-06-18 15:08:36.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   465673 2019-06-18 15:08:34.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js
--rw-r--r--   0 reg        (501) staff       (20)    12876 2019-06-18 15:03:36.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    59932 2019-06-18 15:03:33.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   171551 2019-06-18 15:03:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js
--rw-r--r--   0 reg        (501) staff       (20)    13069 2019-06-18 15:04:17.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js
--rw-r--r--   0 reg        (501) staff       (20)    48118 2019-06-18 15:04:13.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm
--rw-r--r--   0 reg        (501) staff       (20)   122752 2019-06-18 15:04:11.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js
--rw-r--r--   0 reg        (501) staff       (20)   140564 2019-06-18 15:01:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js
--rw-r--r--   0 reg        (501) staff       (20)     4142 2019-06-18 15:01:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-support.js
--rw-r--r--   0 reg        (501) staff       (20)     2235 2019-06-18 15:01:27.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-version.js
--rw-r--r--   0 reg        (501) staff       (20)     9543 2019-06-18 15:01:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js
--rw-r--r--   0 reg        (501) staff       (20)     9591 2019-06-18 15:01:28.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js
--rw-r--r--   0 reg        (501) staff       (20)   148482 2019-06-18 15:01:30.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv.js
--rw-r--r--   0 reg        (501) staff       (20)    59078 2020-11-18 14:55:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/pouchdb.find.min.js
--rw-r--r--   0 reg        (501) staff       (20)   125540 2020-11-18 14:55:12.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/pouchdb.min.js
--rw-r--r--   0 reg        (501) staff       (20)    68850 2020-11-18 14:55:13.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/sugar.min.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.366190 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.367802 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/
--rwxr-xr-x   0 reg        (501) staff       (20)    28407 2019-08-28 19:46:06.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/VideoJS.svg
--rwxr-xr-x   0 reg        (501) staff       (20)     7080 2019-08-28 19:46:06.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf
--rwxr-xr-x   0 reg        (501) staff       (20)     4324 2019-08-28 19:46:06.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/VideoJS.woff
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.389299 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/
--rw-r--r--   0 reg        (501) staff       (20)     2329 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ar.js
--rw-r--r--   0 reg        (501) staff       (20)     2302 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ar.json
--rw-r--r--   0 reg        (501) staff       (20)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ba.js
--rw-r--r--   0 reg        (501) staff       (20)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ba.json
--rw-r--r--   0 reg        (501) staff       (20)     1946 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/bg.js
--rw-r--r--   0 reg        (501) staff       (20)     1919 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/bg.json
--rw-r--r--   0 reg        (501) staff       (20)     1494 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ca.js
--rw-r--r--   0 reg        (501) staff       (20)     1467 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ca.json
--rw-r--r--   0 reg        (501) staff       (20)     3869 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cs.js
--rw-r--r--   0 reg        (501) staff       (20)     3842 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cs.json
--rw-r--r--   0 reg        (501) staff       (20)     3848 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cy.js
--rw-r--r--   0 reg        (501) staff       (20)     3739 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cy.json
--rw-r--r--   0 reg        (501) staff       (20)     1425 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/da.js
--rw-r--r--   0 reg        (501) staff       (20)     1398 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/da.json
--rw-r--r--   0 reg        (501) staff       (20)     4419 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/de.js
--rw-r--r--   0 reg        (501) staff       (20)     4393 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/de.json
--rw-r--r--   0 reg        (501) staff       (20)     3616 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/el.js
--rw-r--r--   0 reg        (501) staff       (20)     3589 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/el.json
--rw-r--r--   0 reg        (501) staff       (20)     3992 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/en.js
--rw-r--r--   0 reg        (501) staff       (20)     3965 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/en.json
--rw-r--r--   0 reg        (501) staff       (20)     4542 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/es.js
--rw-r--r--   0 reg        (501) staff       (20)     4514 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/es.json
--rw-r--r--   0 reg        (501) staff       (20)     4534 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fa.js
--rw-r--r--   0 reg        (501) staff       (20)     4507 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fa.json
--rw-r--r--   0 reg        (501) staff       (20)     1376 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fi.js
--rw-r--r--   0 reg        (501) staff       (20)     1349 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fi.json
--rw-r--r--   0 reg        (501) staff       (20)     4447 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fr.js
--rw-r--r--   0 reg        (501) staff       (20)     4420 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fr.json
--rw-r--r--   0 reg        (501) staff       (20)     4438 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gd.js
--rwxr-xr-x   0 reg        (501) staff       (20)     4411 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gd.json
--rw-r--r--   0 reg        (501) staff       (20)     4432 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gl.js
--rw-r--r--   0 reg        (501) staff       (20)     4405 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gl.json
--rw-r--r--   0 reg        (501) staff       (20)     4632 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/he.js
--rw-r--r--   0 reg        (501) staff       (20)     4523 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/he.json
--rw-r--r--   0 reg        (501) staff       (20)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hr.js
--rw-r--r--   0 reg        (501) staff       (20)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hr.json
--rw-r--r--   0 reg        (501) staff       (20)     1430 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hu.js
--rw-r--r--   0 reg        (501) staff       (20)     1403 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hu.json
--rw-r--r--   0 reg        (501) staff       (20)     1474 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/it.js
--rw-r--r--   0 reg        (501) staff       (20)     1447 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/it.json
--rw-r--r--   0 reg        (501) staff       (20)     1663 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ja.js
--rw-r--r--   0 reg        (501) staff       (20)     1636 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ja.json
--rw-r--r--   0 reg        (501) staff       (20)     1537 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ko.js
--rw-r--r--   0 reg        (501) staff       (20)     1510 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ko.json
--rw-r--r--   0 reg        (501) staff       (20)     1421 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nb.js
--rw-r--r--   0 reg        (501) staff       (20)     1394 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nb.json
--rw-r--r--   0 reg        (501) staff       (20)     4130 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nl.js
--rw-r--r--   0 reg        (501) staff       (20)     4102 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nl.json
--rw-r--r--   0 reg        (501) staff       (20)     1399 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nn.js
--rw-r--r--   0 reg        (501) staff       (20)     1372 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nn.json
--rw-r--r--   0 reg        (501) staff       (20)     4331 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/oc.js
--rw-r--r--   0 reg        (501) staff       (20)     4304 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/oc.json
--rw-r--r--   0 reg        (501) staff       (20)     2028 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pl.js
--rw-r--r--   0 reg        (501) staff       (20)     2001 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pl.json
--rw-r--r--   0 reg        (501) staff       (20)     4104 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-BR.js
--rw-r--r--   0 reg        (501) staff       (20)     4178 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-BR.json
--rw-r--r--   0 reg        (501) staff       (20)     2382 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-PT.js
--rw-r--r--   0 reg        (501) staff       (20)     2351 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-PT.json
--rw-r--r--   0 reg        (501) staff       (20)     5418 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ru.js
--rw-r--r--   0 reg        (501) staff       (20)     5391 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ru.json
--rw-r--r--   0 reg        (501) staff       (20)     4097 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sk.js
--rw-r--r--   0 reg        (501) staff       (20)     4069 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sk.json
--rw-r--r--   0 reg        (501) staff       (20)     1348 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sr.js
--rw-r--r--   0 reg        (501) staff       (20)     1321 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sr.json
--rw-r--r--   0 reg        (501) staff       (20)     4158 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sv.js
--rw-r--r--   0 reg        (501) staff       (20)     4131 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sv.json
--rw-r--r--   0 reg        (501) staff       (20)     3443 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/tr.js
--rw-r--r--   0 reg        (501) staff       (20)     3416 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/tr.json
--rw-r--r--   0 reg        (501) staff       (20)     5448 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/uk.js
--rw-r--r--   0 reg        (501) staff       (20)     5431 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/uk.json
--rw-r--r--   0 reg        (501) staff       (20)     4139 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/vi.js
--rw-r--r--   0 reg        (501) staff       (20)     4112 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/vi.json
--rw-r--r--   0 reg        (501) staff       (20)     3716 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-CN.js
--rw-r--r--   0 reg        (501) staff       (20)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-CN.json
--rw-r--r--   0 reg        (501) staff       (20)     3718 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js
--rw-r--r--   0 reg        (501) staff       (20)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json
--rw-r--r--   0 reg        (501) staff       (20)     3746 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js
--rw-r--r--   0 reg        (501) staff       (20)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json
--rw-r--r--   0 reg        (501) staff       (20)     3744 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-TW.js
--rw-r--r--   0 reg        (501) staff       (20)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-TW.json
--rw-r--r--   0 reg        (501) staff       (20)    45293 2019-08-28 19:45:45.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video-js.css
--rw-r--r--   0 reg        (501) staff       (20)    40028 2019-08-28 19:46:05.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video-js.min.css
--rw-r--r--   0 reg        (501) staff       (20)  1361043 2019-08-28 19:45:26.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.cjs.js
--rw-r--r--   0 reg        (501) staff       (20)  1360644 2019-08-28 19:45:26.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.es.js
--rw-r--r--   0 reg        (501) staff       (20)  1797606 2019-08-28 19:45:23.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.js
--rw-r--r--   0 reg        (501) staff       (20)   480256 2019-08-28 19:45:58.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.min.js
--rw-r--r--   0 reg        (501) staff       (20)    17631 2022-10-03 10:52:48.000000 nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs-ogvjs.js
-drwxr-xr-x   0 reg        (501) staff       (20)        0 2022-10-03 10:52:58.190345 nautiluszim-1.0.8/nautiluszim.egg-info/
--rw-r--r--   0 reg        (501) staff       (20)     3946 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim.egg-info/PKG-INFO
--rw-r--r--   0 reg        (501) staff       (20)    28629 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim.egg-info/SOURCES.txt
--rw-r--r--   0 reg        (501) staff       (20)        1 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim.egg-info/dependency_links.txt
--rw-r--r--   0 reg        (501) staff       (20)       59 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim.egg-info/entry_points.txt
--rw-r--r--   0 reg        (501) staff       (20)        1 2021-06-10 11:39:04.000000 nautiluszim-1.0.8/nautiluszim.egg-info/not-zip-safe
--rw-r--r--   0 reg        (501) staff       (20)       45 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim.egg-info/requires.txt
--rw-r--r--   0 reg        (501) staff       (20)       12 2022-10-03 10:52:57.000000 nautiluszim-1.0.8/nautiluszim.egg-info/top_level.txt
--rw-r--r--   0 reg        (501) staff       (20)       38 2022-10-03 10:52:58.390098 nautiluszim-1.0.8/setup.cfg
--rw-r--r--   0 reg        (501) staff       (20)     1920 2021-06-10 11:28:11.000000 nautiluszim-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.519174 nautiluszim-1.1.0/nautiluszim/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.519174 nautiluszim-1.1.0/nautiluszim/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/locale/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/database.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/display_rows.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/info-circle-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/main-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/media_player.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/modal_empty_body.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/modal_title.handlebars
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/nautilus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim/templates/precompiled.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/nautiluszim/templates/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.527174 nautiluszim-1.1.0/nautiluszim/templates/vendors/
+-rw-r--r--   0 runner    (1001) docker     (123)    17430 2020-05-04 16:04:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ScrollMagic.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.519174 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.531174 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    67871 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   157964 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50935 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115021 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77346 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32546 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   197170 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   504418 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   159515 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   641867 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.531174 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   227980 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   410007 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    80698 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   318045 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   135079 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   256099 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    60010 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194435 2019-11-28 12:59:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.575175 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2018-08-05 19:09:20.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3g2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3ga.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3gp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/7z.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2018-08-04 18:46:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/adn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ai.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aif.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aifc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aiff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ait.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/amr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2018-06-23 16:58:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ani.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2018-06-23 17:59:22.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/apk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2018-08-04 19:09:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/applescript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ascx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ashx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asmx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2018-07-28 14:27:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aspx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/au.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-08-05 04:08:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/avi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/axd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-24 12:27:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aze.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2018-06-24 12:59:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/blank.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bmp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2018-08-05 17:23:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bowerrc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-06-24 17:12:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/browser.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bz2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2018-06-30 00:29:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cad.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/caf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2018-06-29 23:33:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2018-08-05 20:11:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 03:33:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cgi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2018-07-28 15:17:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/class.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cmd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2018-08-04 16:34:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/codekit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2018-08-04 23:31:11.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/coffee.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/coffeelintignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/com.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2018-06-24 16:56:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/compile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2018-08-05 17:39:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/conf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/config.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2018-06-30 00:30:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cpp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2018-07-27 01:50:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cptx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cr2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2018-07-21 22:39:54.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crdownload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-07-16 05:46:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crypt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2018-06-30 00:30:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2018-08-04 23:32:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cson.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csproj.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2018-06-29 21:26:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/css.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2018-07-16 05:44:20.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cue.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-08-05 04:11:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/db.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dbf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/deb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dgn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2018-07-21 20:21:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/diz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dll.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2018-08-04 14:05:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dmg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dng.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:50.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/docb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/docm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/docx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dotm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dotx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2018-07-22 03:47:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:35:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dpj.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2018-06-30 18:59:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ds_store.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2018-07-18 23:08:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dtd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dwg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dxf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2018-08-04 20:17:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/editorconfig.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:16:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/el.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/enc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-07-28 16:31:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/epub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eslintignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/exe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/f4v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2018-07-18 23:43:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fb2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2018-06-23 16:11:22.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fla.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2018-08-05 19:39:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gadget.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2018-08-04 20:28:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gdp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2018-06-30 04:29:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gif.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2018-08-04 20:41:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gitattributes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gitignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2018-07-16 05:26:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/go.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-08-05 19:40:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2018-07-19 02:16:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/h.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/handlebars.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hbs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/heic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hsl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/htm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/html.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ibooks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/icns.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2018-06-29 23:32:36.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ics.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2018-07-18 23:46:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/idx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2018-08-05 17:40:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ifo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/img.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/in.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2018-06-23 16:06:20.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/indd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/inf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ini.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iso.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2018-07-21 14:30:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/j2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:50.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/java.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jpe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2018-06-29 21:26:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/js.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2018-06-29 21:39:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:37:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2018-06-29 21:40:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/key.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kf8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2018-08-04 17:53:19.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kmk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ksh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2018-08-04 18:52:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2018-07-28 15:17:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/less.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/licx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:15:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lisp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2018-08-05 16:10:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lnk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2018-06-24 16:25:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/log.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2018-07-21 17:43:54.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lua.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2018-08-05 17:33:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m2v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2018-08-05 06:23:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4r.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4v.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/map.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/master.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2018-07-21 18:59:04.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/md.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2018-08-05 05:48:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/me.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/midi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mkv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2018-08-05 17:27:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mobi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mod.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mov.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2018-07-18 23:59:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpga.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2018-06-30 14:04:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nef.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2018-08-05 18:13:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2018-07-21 20:21:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nfo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-27 02:23:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nix.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/npmignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2018-07-19 00:19:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2018-06-23 11:58:54.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ods.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ogg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ogv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ost.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/otf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ott.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ova.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ovf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/p12.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/p7b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2018-07-19 02:45:38.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pages.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2018-07-19 02:50:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/part.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pcd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2018-06-19 08:11:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pfx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pgp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2018-06-30 18:08:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/phar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2018-06-29 22:06:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/php.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pkg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2018-06-30 11:23:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2018-08-04 20:04:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/plist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/png.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/po.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2018-07-21 17:42:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/potx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ppsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ppt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pptm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pptx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/prop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2018-07-21 21:37:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2018-06-23 16:13:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/psd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/psp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pst.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2018-07-19 00:02:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2018-06-24 17:07:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/py.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2018-07-16 05:23:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pyc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/qt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/raw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/resx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2018-07-28 14:56:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/retry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2018-08-05 16:36:39.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rom.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rpm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rsa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2018-08-05 04:06:37.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rtf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2018-07-27 04:19:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ru.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rub.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/scss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sitemap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/skin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sldm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sldx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2018-07-28 15:15:35.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sln.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2018-07-21 18:47:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sql.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2018-08-05 19:02:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sqlite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/step.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/stl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2018-08-05 17:36:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2018-06-30 12:16:27.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2018-08-05 19:41:27.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sys.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tcsh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tfignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tga.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tgz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tif.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tiff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2018-08-05 03:53:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tmp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2018-06-30 03:47:11.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/torrent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2018-08-04 17:10:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tsv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2018-08-04 16:11:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ttf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2018-07-27 01:37:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/twig.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/txt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/udf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2018-06-30 00:51:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbproj.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2018-08-05 18:09:55.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vcd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2018-06-24 19:18:25.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vcs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vmdk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vob.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2018-07-16 04:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vss.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vst.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vtx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:36:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/war.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wav.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2018-08-05 03:42:49.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wbk.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-08-05 19:41:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webinfo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wma.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wmf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wmv.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2018-06-30 14:11:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wsf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2018-07-22 02:04:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xcf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlsm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlsx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xlt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xltm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xltx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-07-26 04:04:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2018-07-22 03:42:57.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xpi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xrb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2018-07-28 19:17:51.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xsd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xsl.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xspf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/yml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/z.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zsh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20696 2021-02-15 09:49:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    88145 1991-10-18 12:00:00.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.587175 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2019-03-12 21:12:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2019-03-12 21:13:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2019-03-12 21:13:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2019-03-12 21:13:31.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2019-03-12 21:13:32.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2019-06-18 15:00:08.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2019-06-18 15:06:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   133919 2019-06-18 15:06:14.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   235857 2019-06-18 15:06:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2019-06-18 15:05:09.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136930 2019-06-18 15:05:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   244171 2019-06-18 15:05:03.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js
+-rw-r--r--   0 runner    (1001) docker     (123)    66341 2019-06-18 15:09:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   120118 2019-06-18 15:09:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
+-rw-r--r--   0 runner    (1001) docker     (123)   337274 2019-06-18 15:09:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:56.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2019-06-18 15:09:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   435089 2019-06-18 15:09:02.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   934028 2019-06-18 15:08:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2019-06-18 15:07:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62814 2019-06-18 15:07:01.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   128000 2019-06-18 15:06:59.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js
+-rw-r--r--   0 runner    (1001) docker     (123)    67131 2019-06-18 15:09:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2019-06-18 15:09:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
+-rw-r--r--   0 runner    (1001) docker     (123)   143573 2019-06-18 15:09:44.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:42.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2019-06-18 15:08:15.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123379 2019-06-18 15:08:12.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   260845 2019-06-18 15:08:10.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    64871 2019-06-18 15:09:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32370 2019-06-18 15:09:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
+-rw-r--r--   0 runner    (1001) docker     (123)   223005 2019-06-18 15:09:48.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:46.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2019-06-18 15:08:40.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   238580 2019-06-18 15:08:36.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   465673 2019-06-18 15:08:34.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2019-06-18 15:03:36.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    59932 2019-06-18 15:03:33.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   171551 2019-06-18 15:03:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2019-06-18 15:04:17.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    48118 2019-06-18 15:04:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)   122752 2019-06-18 15:04:11.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js
+-rw-r--r--   0 runner    (1001) docker     (123)   140564 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-support.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2019-06-18 15:01:27.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2019-06-18 15:01:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2019-06-18 15:01:28.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js
+-rw-r--r--   0 runner    (1001) docker     (123)   148482 2019-06-18 15:01:30.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv.js
+-rw-r--r--   0 runner    (1001) docker     (123)    59078 2023-05-05 12:13:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.find.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125540 2023-05-05 12:13:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    68850 2023-05-05 12:13:41.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/sugar.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.595175 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.595175 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28407 2019-08-28 19:46:06.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7080 2019-08-28 19:46:06.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4324 2019-08-28 19:46:06.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45293 2019-08-28 19:45:45.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.css
+-rw-r--r--   0 runner    (1001) docker     (123)    40028 2019-08-28 19:46:05.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1361043 2019-08-28 19:45:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.cjs.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1360644 2019-08-28 19:45:26.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.es.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1797606 2019-08-28 19:45:23.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.js
+-rw-r--r--   0 runner    (1001) docker     (123)   480256 2019-08-28 19:45:58.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2016-10-14 10:25:13.000000 nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs-ogvjs.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:13:42.523174 nautiluszim-1.1.0/nautiluszim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 12:13:42.000000 nautiluszim-1.1.0/nautiluszim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:13:42.603175 nautiluszim-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-05 12:13:26.000000 nautiluszim-1.1.0/setup.py
```

### Comparing `nautiluszim-1.0.8/CONTRIBUTING.md` & `nautiluszim-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/LICENSE` & `nautiluszim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/PKG-INFO` & `nautiluszim-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 Metadata-Version: 2.1
 Name: nautiluszim
-Version: 1.0.8
+Version: 1.1.0
 Summary: turns a collection of documents into a browsable ZIM file
 Home-page: https://github.com/openzim/nautilus
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Nautilus
 =============
 
 [![CodeFactor](https://www.codefactor.io/repository/github/openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/nautilus)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/nautiluszim/)
+[![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/latest_tag?label=docker)](https://ghcr.io/openzim/nautilus)
 
 `nautilus` turns a collection of documents into a browsable [ZIM file](https://openzim.org).
 
-It downloads the video (webm or mp4 format – optionnaly recompress them in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it create a static HTML files folder of it before creating a ZIM off of it.
+It downloads the video (webm or mp4 format – optionally recompress it in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it creates a static HTML files folder of it before creating a ZIM off of it.
 
 # Preparing the archive
 
 To be used with nautilus, your archive should be a ZIP file.
-
 * it doesn't need to be structured, but it can.
 * it doesn't need to be compressed. It's usually recommended not to.
-* it should contain a `collection.json` file, but it can also provided separately (see below).
+* it should contain a `collection.json` file, but it can also be provided separately (see below).
 * it should only contain to-be-included files. No filtering is done.
-* Audio and video files should be in ogg format with `.ogg`/`.ogv` extension to be supported on all platform (`mp3`/`mp4` would work only on platform with native support).
+* Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension to be supported on all platforms (`mp3`/`mp4` would work only on platforms with native support).
 
 ```
 cd content/path
 zip -r -0 -T ../content_name.zip *
 ```
 
 ## JSON collection file
 
 Either inside the archive ZIP as `/collection.json` or elsewhere, 
 specified via `--collection mycollection.json`, you must supply a JSON file describing your content.
 
 The user-interface only gives access to files referenced properly in the collection.
 
-At the moment, the JSON files needs to provide the following fields for each item in an Array:
+At the moment, the JSON file needs to provide the following fields for each item in an array:
 
 ``` JSON
 [
     {
         "title": "...",
         "description": "...",
         "authors": "...",
@@ -64,35 +65,36 @@
      }
 ]
 ```
 
 ## About page
 
 Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--about myabout.html`,
-you may supply an about page in HTML format. It will be displayed in a modal popup and will include
-at its bottom your *secondary-logo* if provided.
+
+- You may supply an about page in HTML format. It will be displayed in a modal popup and will be included.
+- At its bottom your *secondary-logo* if provided.
 
 * Use only content tags (no `<html />` nor `<head />` nor `<script />` etc)
-* Use inline styling if required but no styling is recommended.
+* Use inline styling if required, but no styling is recommended.
 * Include one logo inline if required.
 
 # Requirements
 
 * `wget` and `unzip` to install JS dependencies. See `get_js_deps.sh` if you want to do it manually.
 * `wget` is used to download archive files as well.
 * [`handlebars`](https://handlebarsjs.com) is used to compile JS templates
 
 # Installation
 
-`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtualenv. See `requirements.txt` for the list of python dependencies.
+`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtual-environment. See `requirements.txt` for the list of python dependencies.
 
 ## docker
 
 ```
-docker run -v my_dir:/output openzim/nautilus nautiluszim --help
+docker run -v my_dir:/output ghcr.io/openzim/nautilus nautiluszim --help
 ```
 
 ## pip
 
 ```
 pip install nautiluszim
 nautiluszim --help
@@ -102,18 +104,16 @@
 
 ```
 nautiluszim --archive my-content.zip
 ```
 
 ## Notes
 
-* On macOS, the locale setting is buggy. You need to launch it with `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
+* On macOS, the locale setting is buggy. You need to launch it with the `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
 
 ```
 LANGUAGE=fr nautiluszim --language fra
 ```
 
 ## Development
 
 See [CONTRIBUTING.md](CONTRIBUTING.md)
-
-
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_29k511yl_/tmpsvak5qtw_TarContainer/0/4", line 120, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_29k511yl_/tmpsvak5qtw_TarContainer/0/4", line 120, column 0: CDATA terminal not found*

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: nautiluszim Version: 1.0.8 Summary: turns a
+Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.0 Summary: turns a
 collection of documents into a browsable ZIM file Home-page: https://
 github.com/openzim/nautilus Author: kiwix Author-email: reg@kiwix.org License:
-GPLv3+ Keywords: kiwix zim offline Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+GPLv3+ Keywords: kiwix zim offline Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE Nautilus ============= [![CodeFactor]
-(https://www.codefactor.io/repository/github/openzim/nautilus/badge)](https://
-www.codefactor.io/repository/github/openzim/nautilus) [![License: GPL v3]
-(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
-licenses/gpl-3.0) [![PyPI version shields.io](https://img.shields.io/pypi/v/
-nautiluszim.svg)](https://pypi.org/project/nautiluszim/) `nautilus` turns a
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE Nautilus
+============= [![CodeFactor](https://www.codefactor.io/repository/github/
+openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/
+nautilus) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-
+blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![PyPI version shields.io]
+(https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/
+nautiluszim/) [![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/
+latest_tag?label=docker)](https://ghcr.io/openzim/nautilus) `nautilus` turns a
 collection of documents into a browsable [ZIM file](https://openzim.org). It
-downloads the video (webm or mp4 format â optionnaly recompress them in
-lower-quality, smaller size), the thumbnails, the subtitles and the authors'
-profile pictures ; then, it create a static HTML files folder of it before
-creating a ZIM off of it. # Preparing the archive To be used with nautilus,
-your archive should be a ZIP file. * it doesn't need to be structured, but it
-can. * it doesn't need to be compressed. It's usually recommended not to. * it
-should contain a `collection.json` file, but it can also provided separately
-(see below). * it should only contain to-be-included files. No filtering is
-done. * Audio and video files should be in ogg format with `.ogg`/`.ogv`
-extension to be supported on all platform (`mp3`/`mp4` would work only on
-platform with native support). ``` cd content/path zip -r -0 -T ../
-content_name.zip * ``` ## JSON collection file Either inside the archive ZIP as
-`/collection.json` or elsewhere, specified via `--collection
-mycollection.json`, you must supply a JSON file describing your content. The
-user-interface only gives access to files referenced properly in the
-collection. At the moment, the JSON files needs to provide the following fields
-for each item in an Array: ``` JSON [ { "title": "...", "description": "...",
-"authors": "...", "files": ["relative/path/to/file"] } ] ``` ## About page
-Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--
-about myabout.html`, you may supply an about page in HTML format. It will be
-displayed in a modal popup and will include at its bottom your *secondary-logo*
-if provided. * Use only content tags (no `
+downloads the video (webm or mp4 format â optionally recompress it in lower-
+quality, smaller size), the thumbnails, the subtitles and the authors' profile
+pictures ; then, it creates a static HTML files folder of it before creating a
+ZIM off of it. # Preparing the archive To be used with nautilus, your archive
+should be a ZIP file. * it doesn't need to be structured, but it can. * it
+doesn't need to be compressed. It's usually recommended not to. * it should
+contain a `collection.json` file, but it can also be provided separately (see
+below). * it should only contain to-be-included files. No filtering is done. *
+Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension
+to be supported on all platforms (`mp3`/`mp4` would work only on platforms with
+native support). ``` cd content/path zip -r -0 -T ../content_name.zip * ``` ##
+JSON collection file Either inside the archive ZIP as `/collection.json` or
+elsewhere, specified via `--collection mycollection.json`, you must supply a
+JSON file describing your content. The user-interface only gives access to
+files referenced properly in the collection. At the moment, the JSON file needs
+to provide the following fields for each item in an array: ``` JSON [
+{ "title": "...", "description": "...", "authors": "...", "files": ["relative/
+path/to/file"] } ] ``` ## About page Either inside the archive ZIP as `/
+about.html` or elsewhere, specified via `--about myabout.html`, - You may
+supply an about page in HTML format. It will be displayed in a modal popup and
+will be included. - At its bottom your *secondary-logo* if provided. * Use only
+content tags (no `
 ` nor `
 ` nor `
```

### Comparing `nautiluszim-1.0.8/README.md` & `nautiluszim-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Nautilus
 =============
 
 [![CodeFactor](https://www.codefactor.io/repository/github/openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/nautilus)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/nautiluszim/)
+[![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/latest_tag?label=docker)](https://ghcr.io/openzim/nautilus)
 
 `nautilus` turns a collection of documents into a browsable [ZIM file](https://openzim.org).
 
-It downloads the video (webm or mp4 format – optionnaly recompress them in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it create a static HTML files folder of it before creating a ZIM off of it.
+It downloads the video (webm or mp4 format – optionally recompress it in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it creates a static HTML files folder of it before creating a ZIM off of it.
 
 # Preparing the archive
 
 To be used with nautilus, your archive should be a ZIP file.
-
 * it doesn't need to be structured, but it can.
 * it doesn't need to be compressed. It's usually recommended not to.
-* it should contain a `collection.json` file, but it can also provided separately (see below).
+* it should contain a `collection.json` file, but it can also be provided separately (see below).
 * it should only contain to-be-included files. No filtering is done.
-* Audio and video files should be in ogg format with `.ogg`/`.ogv` extension to be supported on all platform (`mp3`/`mp4` would work only on platform with native support).
+* Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension to be supported on all platforms (`mp3`/`mp4` would work only on platforms with native support).
 
 ```
 cd content/path
 zip -r -0 -T ../content_name.zip *
 ```
 
 ## JSON collection file
 
 Either inside the archive ZIP as `/collection.json` or elsewhere, 
 specified via `--collection mycollection.json`, you must supply a JSON file describing your content.
 
 The user-interface only gives access to files referenced properly in the collection.
 
-At the moment, the JSON files needs to provide the following fields for each item in an Array:
+At the moment, the JSON file needs to provide the following fields for each item in an array:
 
 ``` JSON
 [
     {
         "title": "...",
         "description": "...",
         "authors": "...",
@@ -43,35 +43,36 @@
      }
 ]
 ```
 
 ## About page
 
 Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--about myabout.html`,
-you may supply an about page in HTML format. It will be displayed in a modal popup and will include
-at its bottom your *secondary-logo* if provided.
+
+- You may supply an about page in HTML format. It will be displayed in a modal popup and will be included.
+- At its bottom your *secondary-logo* if provided.
 
 * Use only content tags (no `<html />` nor `<head />` nor `<script />` etc)
-* Use inline styling if required but no styling is recommended.
+* Use inline styling if required, but no styling is recommended.
 * Include one logo inline if required.
 
 # Requirements
 
 * `wget` and `unzip` to install JS dependencies. See `get_js_deps.sh` if you want to do it manually.
 * `wget` is used to download archive files as well.
 * [`handlebars`](https://handlebarsjs.com) is used to compile JS templates
 
 # Installation
 
-`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtualenv. See `requirements.txt` for the list of python dependencies.
+`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtual-environment. See `requirements.txt` for the list of python dependencies.
 
 ## docker
 
 ```
-docker run -v my_dir:/output openzim/nautilus nautiluszim --help
+docker run -v my_dir:/output ghcr.io/openzim/nautilus nautiluszim --help
 ```
 
 ## pip
 
 ```
 pip install nautiluszim
 nautiluszim --help
@@ -81,15 +82,15 @@
 
 ```
 nautiluszim --archive my-content.zip
 ```
 
 ## Notes
 
-* On macOS, the locale setting is buggy. You need to launch it with `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
+* On macOS, the locale setting is buggy. You need to launch it with the `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
 
 ```
 LANGUAGE=fr nautiluszim --language fra
 ```
 
 ## Development
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_29k511yl_/tmpsvak5qtw_TarContainer/0/5.md", line 97, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_29k511yl_/tmpsvak5qtw_TarContainer/0/5.md", line 97, column 0: CDATA terminal not found*

```diff
@@ -1,30 +1,32 @@
 Nautilus ============= [![CodeFactor](https://www.codefactor.io/repository/
 github/openzim/nautilus/badge)](https://www.codefactor.io/repository/github/
 openzim/nautilus) [![License: GPL v3](https://img.shields.io/badge/License-
 GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![PyPI version
 shields.io](https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/
-project/nautiluszim/) `nautilus` turns a collection of documents into a
-browsable [ZIM file](https://openzim.org). It downloads the video (webm or mp4
-format â optionnaly recompress them in lower-quality, smaller size), the
-thumbnails, the subtitles and the authors' profile pictures ; then, it create a
-static HTML files folder of it before creating a ZIM off of it. # Preparing the
-archive To be used with nautilus, your archive should be a ZIP file. * it
-doesn't need to be structured, but it can. * it doesn't need to be compressed.
-It's usually recommended not to. * it should contain a `collection.json` file,
-but it can also provided separately (see below). * it should only contain to-
-be-included files. No filtering is done. * Audio and video files should be in
-ogg format with `.ogg`/`.ogv` extension to be supported on all platform (`mp3`/
-`mp4` would work only on platform with native support). ``` cd content/path zip
--r -0 -T ../content_name.zip * ``` ## JSON collection file Either inside the
-archive ZIP as `/collection.json` or elsewhere, specified via `--collection
-mycollection.json`, you must supply a JSON file describing your content. The
-user-interface only gives access to files referenced properly in the
-collection. At the moment, the JSON files needs to provide the following fields
-for each item in an Array: ``` JSON [ { "title": "...", "description": "...",
-"authors": "...", "files": ["relative/path/to/file"] } ] ``` ## About page
-Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--
-about myabout.html`, you may supply an about page in HTML format. It will be
-displayed in a modal popup and will include at its bottom your *secondary-logo*
-if provided. * Use only content tags (no `
+project/nautiluszim/) [![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/
+latest_tag?label=docker)](https://ghcr.io/openzim/nautilus) `nautilus` turns a
+collection of documents into a browsable [ZIM file](https://openzim.org). It
+downloads the video (webm or mp4 format â optionally recompress it in lower-
+quality, smaller size), the thumbnails, the subtitles and the authors' profile
+pictures ; then, it creates a static HTML files folder of it before creating a
+ZIM off of it. # Preparing the archive To be used with nautilus, your archive
+should be a ZIP file. * it doesn't need to be structured, but it can. * it
+doesn't need to be compressed. It's usually recommended not to. * it should
+contain a `collection.json` file, but it can also be provided separately (see
+below). * it should only contain to-be-included files. No filtering is done. *
+Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension
+to be supported on all platforms (`mp3`/`mp4` would work only on platforms with
+native support). ``` cd content/path zip -r -0 -T ../content_name.zip * ``` ##
+JSON collection file Either inside the archive ZIP as `/collection.json` or
+elsewhere, specified via `--collection mycollection.json`, you must supply a
+JSON file describing your content. The user-interface only gives access to
+files referenced properly in the collection. At the moment, the JSON file needs
+to provide the following fields for each item in an array: ``` JSON [
+{ "title": "...", "description": "...", "authors": "...", "files": ["relative/
+path/to/file"] } ] ``` ## About page Either inside the archive ZIP as `/
+about.html` or elsewhere, specified via `--about myabout.html`, - You may
+supply an about page in HTML format. It will be displayed in a modal popup and
+will be included. - At its bottom your *secondary-logo* if provided. * Use only
+content tags (no `
 ` nor `
 ` nor `
```

### Comparing `nautiluszim-1.0.8/nautiluszim/constants.py` & `nautiluszim-1.1.0/nautiluszim/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # vim: ai ts=4 sts=4 et sw=4 nu
 
-import pathlib
 import logging
+import pathlib
 
 from zimscraperlib.logging import getLogger as lib_getLogger
 
 ROOT_DIR = pathlib.Path(__file__).parent
 NAME = ROOT_DIR.name
 
 with open(ROOT_DIR.joinpath("VERSION"), "r") as fh:
     VERSION = fh.read().strip()
 
 SCRAPER = f"{NAME} {VERSION}"
 
+
 class Global:
     debug = False
 
 
 def setDebug(debug):
-    """ toggle constants global DEBUG flag (used by getLogger) """
+    """toggle constants global DEBUG flag (used by getLogger)"""
     Global.debug = bool(debug)
 
 
 def getLogger():
-    """ configured logger respecting DEBUG flag """
+    """configured logger respecting DEBUG flag"""
     return lib_getLogger(NAME, level=logging.DEBUG if Global.debug else logging.INFO)
```

### Comparing `nautiluszim-1.0.8/nautiluszim/entrypoint.py` & `nautiluszim-1.1.0/nautiluszim/entrypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import argparse
 
 from .constants import NAME, SCRAPER, getLogger, setDebug
 
 
 def main():
     parser = argparse.ArgumentParser(
-        prog=NAME, description="Create a ZIM file off a collection of file documents",
+        prog=NAME,
+        description="Create a ZIM file off a collection of file documents",
     )
 
     parser.add_argument(
         "--archive",
         help="Path or URL to a ZIP archive containing all the documents",
         required=True,
     )
     parser.add_argument(
         "--collection",
-        help="Different collection JSON path or URL. Otherwise using `collection.json` from archive",
+        help="Different collection JSON path or URL. "
+        "Otherwise using `collection.json` from archive",
         required=False,
     )
     parser.add_argument(
         "--name",
         help="ZIM name. Used as identifier and filename (date will be appended)",
         required=True,
     )
@@ -54,20 +56,15 @@
 
     parser.add_argument(
         "--output",
         help="Output folder for ZIM file or build folder",
         default="/output",
         dest="output_dir",
     )
-    parser.add_argument(
-        "--no-zim",
-        help="Don't produce a ZIM file, create HTML folder only.",
-        action="store_true",
-        default=False,
-    )
+
     parser.add_argument(
         "--zim-file",
         help="ZIM file name (based on --name if not provided)",
         dest="fname",
     )
 
     parser.add_argument(
@@ -76,71 +73,83 @@
     parser.add_argument(
         "--keep",
         help="Don't erase build folder on start (for debug/devel)",
         default=False,
         action="store_true",
         dest="keep_build_dir",
     )
-    parser.add_argument(
-        "--skip-download",
-        help="Skip the download and extract step",
-        default=False,
-        action="store_true",
-        dest="skip_download",
-    )
 
     parser.add_argument(
-        "--language", help="ISO-639-3 (3 chars) language code of content", default="eng"
+        "--language",
+        help="ISO-639-3 (3 chars) language code of content. "
+        "comma-separated if multiple ones",
+        default="eng",
     )
     parser.add_argument(
         "--locale",
-        help="Locale name to use for translations (if avail) and time representations. Defaults to --language or English.",
+        help="Locale name to use for translations (if avail) and time representations. "
+        "Defaults to (first) --language or English.",
         dest="locale_name",
     )
     parser.add_argument(
-        "--tags", help="List of comma-separated Tags for the ZIM file.", default="",
+        "--tags",
+        help="List of comma-separated Tags for the ZIM file.",
+        default="",
+    )
+    parser.add_argument(
+        "--title",
+        help="Title for your project and ZIM. Otherwise --name.",
     )
     parser.add_argument(
-        "--title", help="Title for your project and ZIM. Otherwise --name.",
+        "--description",
+        help="Description for your project and ZIM.",
+        required=True,
     )
     parser.add_argument(
-        "--description", help="Description for your project and ZIM.",
+        "--longdescription",
+        help="Long Description for your project and ZIM.",
     )
+
     parser.add_argument(
-        "--creator", help="Name of content creator.",
+        "--creator",
+        help="Name of content creator.",
     )
     parser.add_argument(
         "--publisher", help="Custom publisher name (ZIM metadata)", default="Kiwix"
     )
     parser.add_argument(
         "--favicon",
-        help="Custom favicon. Will be resized to 48x48px. Nautilus otherwise.",
+        help="Custom favicon. Will be resized to 48x48px. Nautilus one otherwise. "
+        "Also used as ZIM illustration",
     )
     parser.add_argument(
         "--main-logo",
         help="Custom logo. Will be resized to 300x65px",
         dest="main_logo",
     )
     parser.add_argument(
         "--secondary-logo",
         help="Custom footer logo. Will be resized to 300x65px. None otherwise",
         dest="secondary_logo",
     )
     parser.add_argument(
         "--main-color",
-        help="Custom header color. Hex/HTML syntax (#DEDEDE). Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
+        help="Custom header color. Hex/HTML syntax (#DEDEDE). "
+        "Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
     )
     parser.add_argument(
         "--secondary-color",
-        help="Custom secondary color. Hex/HTML syntax (#DEDEDE). Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
+        help="Custom secondary color. Hex/HTML syntax (#DEDEDE). "
+        "Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
     )
 
     parser.add_argument(
         "--about",
-        help="Custom about HTML file. Uses file `about.html` of archive if present otherwise.",
+        help="Custom about HTML file. "
+        "Uses file `about.html` of archive if present otherwise.",
     )
 
     parser.add_argument(
         "--version",
         help="Display scraper version and exit",
         action="version",
         version=SCRAPER,
```

### Comparing `nautiluszim-1.0.8/nautiluszim/locale/fr/LC_MESSAGES/messages.mo` & `nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/locale/fr/LC_MESSAGES/messages.po` & `nautiluszim-1.1.0/nautiluszim/locale/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/locale/messages.pot` & `nautiluszim-1.1.0/nautiluszim/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/scraper.py` & `nautiluszim-1.1.0/nautiluszim/scraper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # vim: ai ts=4 sts=4 et sw=4 nu
 
-import os
-import uuid
+import datetime
 import json
 import locale
-import shutil
+import os
 import pathlib
-import datetime
-import subprocess
+import shutil
+import unicodedata
+import uuid
+import zipfile
 from pathlib import Path
+from typing import Optional
 
 import jinja2
-from zimscraperlib.logging import nicer_args_join
+from zimscraperlib.constants import (
+    MAXIMUM_DESCRIPTION_METADATA_LENGTH,
+    MAXIMUM_LONG_DESCRIPTION_METADATA_LENGTH,
+)
 from zimscraperlib.download import save_large_file
-from zimscraperlib.zim.filesystem import make_zim_file
-from zimscraperlib.fix_ogvjs_dist import fix_source_dir
+from zimscraperlib.i18n import _, get_language_details, setlocale
+from zimscraperlib.image.convertion import create_favicon
+from zimscraperlib.image.probing import get_colors, is_hex_color
+from zimscraperlib.image.transformation import resize_image
 from zimscraperlib.inputs import handle_user_provided_file
-from zimscraperlib.i18n import setlocale, get_language_details, _
-from zimscraperlib.imaging import resize_image, get_colors, is_hex_color, create_favicon
+from zimscraperlib.zim.creator import Creator
 
 from .constants import ROOT_DIR, SCRAPER, getLogger
 
 logger = getLogger()
 
 
+def normalized_path(path: str) -> str:
+    """ASCII version of a path for use in URL"""
+    return unicodedata.normalize("NFKC", path)
+
+
 class Nautilus(object):
     def __init__(
         self,
         archive,
         collection,
         nb_items_per_page,
         no_random,
         show_description,
         output_dir,
-        no_zim,
         fname,
         debug,
         keep_build_dir,
-        skip_download,
         language,
         locale_name,
         tags,
         name=None,
         title=None,
         description=None,
+        longdescription=None,
         creator=None,
         publisher=None,
         favicon=None,
         main_logo=None,
         secondary_logo=None,
         main_color=None,
         secondary_color=None,
@@ -62,14 +72,15 @@
         self.show_author = True
         self.show_description = show_description
         self.fname = fname
         self.language = language
         self.tags = [t.strip() for t in tags.split(",")]
         self.title = title
         self.description = description
+        self.long_description = longdescription
         self.creator = creator
         self.publisher = publisher
         self.name = name
         self.favicon = favicon
         self.main_logo = main_logo
         self.secondary_logo = secondary_logo
         self.main_color = main_color
@@ -78,158 +89,131 @@
         self.randomize = not no_random
 
         # process-related
         self.output_dir = Path(output_dir).expanduser().resolve()
         self.period = datetime.datetime.now().strftime("%Y-%m")
 
         # debug/devel options
-        self.no_zim = no_zim
         self.debug = debug
         self.keep_build_dir = keep_build_dir
-        self.skip_download = skip_download
 
         self.build_dir = self.output_dir.joinpath("build")
 
-        # store ZIM-related info
-        self.zim_info = dict(
-            language=language,
-            tags=tags,
-            title=title,
-            description=description,
-            creator=creator,
-            publisher=publisher,
-            name=name,
-            scraper=SCRAPER,
-        )
-
         # set and record locale for translations
-        locale_name = locale_name or get_language_details(self.language)["iso-639-1"]
+        locale_name = (
+            locale_name
+            or get_language_details(self.language.split(",")[0])["iso-639-1"]
+        )
         try:
             self.locale = setlocale(ROOT_DIR, locale_name)
         except locale.Error:
             logger.error(
-                f"No locale for {locale_name}. Use --locale to specify it. defaulting to en_US"
+                f"No locale for {locale_name}. Use --locale to specify it. "
+                "defaulting to en_US"
             )
             self.locale = setlocale(ROOT_DIR, "en")
 
     @property
     def root_dir(self):
         return ROOT_DIR
 
     @property
     def templates_dir(self):
         return self.root_dir.joinpath("templates")
 
     @property
-    def assets_dir(self):
-        return self.templates_dir.joinpath("assets")
-
-    @property
-    def vendors_src_dir(self):
-        return self.templates_dir.joinpath("vendors")
-
-    @property
-    def vendors_dir(self):
-        return self.build_dir.joinpath("vendors")
-
-    @property
-    def main_logo_path(self):
-        return self.build_dir.joinpath("assets", "main-logo.png")
-
-    @property
-    def secondary_logo_path(self):
-        return self.build_dir.joinpath("assets", "secondary-logo.png")
-
-    @property
     def archive_path(self):
         return (
             self.output_dir.joinpath("archive.zip")
             if self.archive.startswith("http")
             else pathlib.Path(self.archive).expanduser().resolve()
         )
 
-    @property
-    def files_path(self):
-        return self.build_dir.joinpath("files")
-
     def run(self):
-        """ execute the scrapper step by step """
+        """execute the scrapper step by step"""
+
+        self.check_description_length()
+
         logger.info(f"starting nautilus scraper for {self.archive}")
 
         logger.info("preparing build folder at {}".format(self.build_dir.resolve()))
         if not self.keep_build_dir and self.build_dir.exists():
             shutil.rmtree(self.build_dir)
         self.make_build_folder()
 
         # fail early if supplied branding files are missing
         self.check_branding_values()
 
-        # download videos (and recompress)
-        if not self.skip_download:
-            self.download_and_extract_archive()
+        # download archive
+        self.download_archive()
 
         if not self.collection:
-            self.collection = self.files_path.joinpath("collection.json")
+            self.collection = self.extract_to_fs("collection.json")
+            if not self.about:
+                self.extract_to_fs("about.html", failsafe=True)
 
         self.test_collection()
 
         logger.info("update general metadata")
         self.update_metadata()
 
-        logger.info("creating HTML files")
-        self.make_html_files()
-
-        # make zim file
-        if not self.no_zim:
-            self.fname = Path(
-                self.fname if self.fname else f"{self.name}_{self.period}.zim"
+        # prepare creator
+        self.zim_creator = Creator(
+            filename=self.output_dir / self.fname,
+            main_path="home",
+            ignore_duplicates=True,
+        ).config_verbose(self.debug)
+
+        with open(self.build_dir.joinpath("favicon.png"), "rb") as fh:
+            self.zim_creator.config_metadata(
+                Name=self.name,
+                Language=self.language,
+                Title=self.title,
+                Description=self.description,
+                LongDescription=self.long_description,
+                Creator=self.creator,
+                Publisher=self.publisher,
+                Date=datetime.date.today(),
+                Illustration_48x48_at_1=fh.read(),
+                Tags=";".join(self.tags),
+                Scraper=SCRAPER,
             )
-            logger.info("building ZIM file")
-            make_zim_file(
-                build_dir=self.build_dir,
-                fpath=self.output_dir / self.fname,
-                main_page="home.html",
-                favicon="favicon.png",
-                date=datetime.date.today(),
-                **self.zim_info)
-            logger.info("removing HTML folder")
-            if not self.keep_build_dir:
-                shutil.rmtree(self.build_dir, ignore_errors=True)
+        self.zim_creator.start()
+
+        logger.info("adding U.I")
+        self.add_ui()
+
+        logger.info("Adding all files")
+        self.process_collection_entries()
+
+        logger.info("Finishing ZIM file")
+        self.zim_creator.finish()
+
+        logger.info("removing HTML folder")
+        if not self.keep_build_dir:
+            shutil.rmtree(self.build_dir, ignore_errors=True)
 
         logger.info("all done!")
 
     def make_build_folder(self):
-        """ prepare build folder before we start downloading data """
+        """prepare build folder before we start downloading data"""
 
         # create build folder
         os.makedirs(self.build_dir, exist_ok=True)
-
-        # copy vendors and assets
-        for folder in ["vendors", "assets"]:
-            target = self.build_dir.joinpath(folder)
-            if target.exists():
-                shutil.rmtree(target)
-            shutil.copytree(self.templates_dir.joinpath(folder), target)
-
-        fix_source_dir(self.build_dir.joinpath("vendors"))
-
-        for fname in ["nautilus.js", "favicon.png"]:
-            target = self.build_dir.joinpath(fname)
-            try:
-                target.unlink()
-            except FileNotFoundError:
-                pass
-            shutil.copy(self.templates_dir.joinpath(fname), target)
-        os.makedirs(self.files_path, exist_ok=True)
+        for fname in ("favicon.png", "main-logo.png"):
+            shutil.copy2(
+                self.templates_dir.joinpath(fname),
+                self.build_dir.joinpath(fname),
+            )
 
     def check_branding_values(self):
-        """ checks that user-supplied images and colors are valid (so to fail early)
+        """checks that user-supplied images and colors are valid (so to fail early)
 
-            Images are checked for existence or downloaded then resized
-            Colors are check for validity """
+        Images are checked for existence or downloaded then resized
+        Colors are check for validity"""
 
         # skip this step if none of related values were supplied
         if not sum(
             [
                 bool(x)
                 for x in (
                     self.favicon,
@@ -243,123 +227,175 @@
         ):
             return
 
         logger.info("checking your branding files and values")
 
         images = [
             (self.favicon, self.build_dir.joinpath("favicon.png"), 48, 48),
-            (self.main_logo, self.main_logo_path, 300, 65),
-            (self.secondary_logo, self.secondary_logo_path, 300, 65),
+            (self.main_logo, self.build_dir.joinpath("main-logo.png"), 300, 65),
+            (
+                self.secondary_logo,
+                self.build_dir.joinpath("secondary-logo.png"),
+                300,
+                65,
+            ),
         ]
 
         for src, dest, width, height in images:
             if src:
                 handle_user_provided_file(source=src, dest=dest)
                 resize_image(dest, width=width, height=height, method="thumbnail")
 
         if self.main_color and not is_hex_color(self.main_color):
             raise ValueError(
                 f"--main-color is not a valid hex color: {self.main_color}"
             )
 
         if self.secondary_color and not is_hex_color(self.secondary_color):
             raise ValueError(
-                f"--secondary_color-color is not a valid hex color: {self.secondary_color}"
+                "--secondary_color-color is not a valid hex color: "
+                f"{self.secondary_color}"
             )
 
         if self.about:
             handle_user_provided_file(
                 source=self.about, dest=self.build_dir / "about.html"
             )
 
+    def check_description_length(self):
+        if len(self.description) > MAXIMUM_DESCRIPTION_METADATA_LENGTH:
+            raise ValueError(
+                "--The description is greater "
+                f"than {MAXIMUM_DESCRIPTION_METADATA_LENGTH} characters: "
+                f"{len(self.description)} characters"
+            )
+        if self.long_description is not None:
+            if len(self.long_description) > MAXIMUM_LONG_DESCRIPTION_METADATA_LENGTH:
+                raise ValueError(
+                    "--The Long Description is greater "
+                    f"than {MAXIMUM_LONG_DESCRIPTION_METADATA_LENGTH} characters: "
+                    f"{len(self.long_description)} characters"
+                )
+
     def update_metadata(self):
+        self.fname = Path(
+            self.fname if self.fname else f"{self.name}_{self.period}.zim"
+        )
         self.title = self.title or self.name
-        self.description = self.description or "-"
         self.creator = self.creator or "Unknown"
-        self.publisher = self.publisher or "Kiwix"
-
+        self.publisher = self.publisher or "openZIM"
         self.tags = self.tags or []
 
         # generate ICO favicon (fallback for browsers)
         create_favicon(
             self.build_dir.joinpath("favicon.png"),
             self.build_dir.joinpath("favicon.ico"),
         )
 
-        self.zim_info.update({
-            "title": self.title,
-            "description": self.description,
-            "creator": self.creator,
-            "publisher": self.publisher,
-            "name": self.name,
-            "tags": self.tags,
-            }
-        )
-
         # set colors from images if not supplied
         main_color, secondary_color = "#95A5A6", "#95A5A6"
         if self.main_logo:
-            main_color = secondary_color = get_colors(self.main_logo_path)[1]
+            main_color = secondary_color = get_colors(
+                self.build_dir.joinpath("main-logo.png")
+            )[1]
         self.main_color = self.main_color or main_color
         self.secondary_color = self.secondary_color or secondary_color
 
         # get about content from param, archive or defaults to desc
-        self.about_content = f"<p>{self.description}</p>"
+
+        # setting the about_content to long_description if it is provided by the user
+        self.about_content = f"<p>{self.long_description or self.description}</p>"
         about_source = self.build_dir / "about.html"
         if about_source.exists():
             with open(about_source, "r") as fh:
                 self.about_content = fh.read()
             about_source.unlink(missing_ok=True)
-        else:
-            about_source = about_source.parent / "files" / "about.html"
-            if about_source.exists():
-                with open(about_source, "r") as fh:
-                    self.about_content = fh.read()
-                about_source.unlink(missing_ok=True)
 
-    def download_and_extract_archive(self):
+    def download_archive(self):
         # download if it's a URL
         if self.archive.startswith("http"):
             logger.info(f"Downloading archive at {self.archive}")
             save_large_file(self.archive, self.archive_path)
 
-        # extract ZIP
-        logger.info(f"Extracting ZIP archive {self.archive_path} to {self.files_path}")
-        args = [
-            "unzip",
-            "-u",
-            "-q",
-            "-D",
-            str(self.archive_path),
-            "-d",
-            str(self.files_path),
-        ]
-        logger.debug(nicer_args_join(args))
-        subprocess.run(args, check=True)
+    def extract_to_fs(
+        self, name: str, failsafe: Optional[bool] = False
+    ) -> pathlib.Path:
+        """extracting single archive member `name` to filesystem at `to`"""
+
+        with zipfile.ZipFile(self.archive, "r") as zh:
+            try:
+                normalized_name = zh.extract(member=name, path=self.build_dir)
+                return self.build_dir.joinpath(normalized_name)
+            except Exception as exc:
+                logger.error(f"Unable to extract {name} from archive: {exc}")
+                if failsafe:
+                    return
+                raise exc
 
     def test_collection(self):
         with open(self.collection, "r") as fp:
             self.json_collection = [i for i in json.load(fp) if i.get("files", [])]
         nb_items = len(self.json_collection)
         nb_files = sum([len(i.get("files", [])) for i in self.json_collection])
         logger.info(f"Collection loaded. {nb_items} items, {nb_files} files")
 
-    def make_html_files(self):
-        """ make up HTML structure to read the content
-        """
+        with zipfile.ZipFile(self.archive, "r") as zh:
+            all_names = zh.namelist()
+
+        missing_files = []
+        for entry in self.json_collection:
+            if not entry.get("files"):
+                continue
+            for relative_path in entry["files"]:
+                if relative_path not in all_names:
+                    missing_files.append(relative_path)
+
+        if missing_files:
+            raise ValueError(
+                "File(s) referenced in collection but missing:\n - "
+                + "\n - ".join(missing_files)
+            )
+
+    def process_collection_entries(self):
+        for entry in self.json_collection:
+            if not entry.get("files"):
+                continue
+
+            for relative_path in entry["files"]:
+                logger.debug(f"> {relative_path}")
+                self.zim_creator.add_item_for(
+                    path="files/" + normalized_path(relative_path),
+                    fpath=self.extract_to_fs(relative_path),
+                    delete_fpath=True,
+                    is_front=False,
+                )
+
+    def add_ui(self):
+        """make up HTML structure to read the content"""
+
+        for fname in (
+            "favicon.ico",
+            "favicon.png",
+            "main-logo.png",
+            "secondary-logo.png",
+        ):
+            fpath = self.build_dir.joinpath(fname)
+            if fpath.exists():
+                self.zim_creator.add_item_for(path=fname, fpath=fpath)
 
         env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(str(self.templates_dir)), autoescape=True
         )
 
         # build homepage
         html = env.get_template("home.html").render(
             debug=str(self.debug).lower(),
             title=self.title,
             description=self.description,
+            long_description=self.long_description,
             main_color=self.main_color,
             secondary_color=self.secondary_color,
             db_name=f"{self.name}_{self.period}_{uuid.uuid4().hex}_db",
             db_version=1,
             nb_items_per_page=self.nb_items_per_page,
             show_author=self.show_author,
             show_description=self.show_description,
@@ -370,42 +406,61 @@
             loading_label=_("Loading…"),
             no_result_text=_("No result for this search request."),
             backtotop_label=_("Back to Top"),
             secondary_logo=self.secondary_logo,
             about_label=_("About this content"),
             about_content=self.about_content,
         )
-        with open(self.build_dir.joinpath("home.html"), "w", encoding="utf-8") as fp:
-            fp.write(html)
+        self.zim_creator.add_item_for(
+            path="home", content=html, mimetype="text/html", is_front=True
+        )
 
         initjs = env.get_template("init.js").render(
             debug=str(self.debug).lower(),
             title=self.title,
             description=self.description,
             db_name=f"{self.name}_{self.period}_{uuid.uuid4().hex}_db",
             db_version=1,
             nb_items_per_page=self.nb_items_per_page,
             show_author=self.show_author,
             show_description=self.show_description,
             randomize=self.randomize,
             loading_label=_("Loading…"),
         )
-        with open(self.build_dir.joinpath("init.js"), "w", encoding="utf-8") as fp:
-            fp.write(initjs)
+        self.zim_creator.add_item_for(
+            path="init.js",
+            content=initjs,
+            mimetype="text/javascript",
+            is_front=False,
+        )
 
-        with open(self.build_dir.joinpath("database.js"), "w", encoding="utf-8") as fp:
-            fp.write("var DATABASE = [\n")
-            for docid, document in enumerate(self.json_collection):
-                fp.write(
-                    "{},\n".format(
-                        str(
-                            {
-                                "_id": str(docid).zfill(5),
-                                "ti": document.get("title") or "Unknown?",
-                                "dsc": document.get("description") or "",
-                                "aut": document.get("authors") or "",
-                                "fp": document.get("files", []),
-                            }
-                        )
-                    )
+        database_js = "var DATABASE = [\n"
+        for docid, document in enumerate(self.json_collection):
+            database_js += "{},\n".format(
+                str(
+                    {
+                        "_id": str(docid).zfill(5),
+                        "ti": document.get("title") or "Unknown?",
+                        "dsc": document.get("description") or "",
+                        "aut": document.get("authors") or "",
+                        "fp": [
+                            normalized_path(path) for path in document.get("files", [])
+                        ],
+                    }
                 )
-            fp.write("];\n")
+            )
+        database_js += "];\n"
+        self.zim_creator.add_item_for(
+            path="database.js",
+            content=database_js,
+            mimetype="text/javascript",
+            is_front=False,
+        )
+
+        # recursively add all templates's folder
+        for fpath in self.templates_dir.glob("**/*"):
+            if not fpath.is_file():
+                continue
+            path = str(fpath.relative_to(self.templates_dir))
+
+            logger.debug(f"> {path}")
+            self.zim_creator.add_item_for(path=path, fpath=fpath, is_front=False)
```

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/assets/info-circle-solid.svg` & `nautiluszim-1.1.0/nautiluszim/templates/info-circle-solid.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/assets/styles.css` & `nautiluszim-1.1.0/nautiluszim/templates/styles.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/assets/templates/precompiled.js` & `nautiluszim-1.1.0/nautiluszim/templates/precompiled.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/favicon.png` & `nautiluszim-1.1.0/nautiluszim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/home.html` & `nautiluszim-1.1.0/nautiluszim/templates/home.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,28 @@
   <head>
     <meta charset="utf-8">
     <title>{{ title }}</title>
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <link id="favicon" rel="icon" href="favicon.png" type="image/png" />
     <link rel="stylesheet" href="vendors/bootstrap/css/bootstrap.min.css">
     <link href="vendors/videojs/video-js.css" rel="stylesheet" />
-    <link href="assets/styles.css" rel="stylesheet" type="text/css">
+    <link href="styles.css" rel="stylesheet" type="text/css">
     <style type="text/css">
         header { background-color: {{ main_color }};}
         #loader { color: {{ main_color }};}
         footer { background-color: {{ secondary_color }};}
     </style>
   </head>
   <body>
     <header class="container-fluid">
         <div class="row">
             <div class="col-xs-12 col-sm-6">
-                <a href="home.html"><img class="logo" src="assets/main-logo.png" /></a>
+                <a href="home.html"><img class="logo" src="main-logo.png" /></a>
                 <a href="#" class="btn about-btn" role="button" data-toggle="tooltip" title="{{ about_label }}">
-                    <img src="assets/info-circle-solid.svg" />
+                    <img src="info-circle-solid.svg" />
                 </a>
             </div>
             <form class="form-check-inline search-box col-xs-12 col-sm-6">
                 <input class="form-control" type="search" placeholder="{{ search_input_label }}" id="search_text" />
                 <button class="btn btn-dark ml-2">{{ search_label }}</button>
             </form>
         </div>
@@ -54,15 +54,15 @@
     </div>
     <a  href="#" class="btn btn-dark back-to-top"
         role="button"
         data-toggle="tooltip"
         title="{{ backtotop_label }}">⇡</span>
     </a>
     <footer>
-        {% if secondary_logo %}<hr /><img src="assets/secondary-logo.png" />{% endif %}
+        {% if secondary_logo %}<hr /><img src="secondary-logo.png" />{% endif %}
     </footer>
 
     <script src="vendors/pouchdb.min.js"></script>
     <script src="vendors/pouchdb.find.min.js"></script>
 
     <script src="vendors/jquery.min.js"></script>
     <script src="vendors/bootstrap/js/bootstrap.bundle.min.js"></script>
@@ -71,17 +71,17 @@
 
     <script src="vendors/videojs/video.js"></script>
     <script src="vendors/ogvjs/ogv-support.js"></script>
     <script src="vendors/ogvjs/ogv.js"></script>
     <script src="vendors/videojs-ogvjs.js"></script>
 
     <script src="vendors/handlebars.runtime.min-v4.7.7.js"></script>
-    <script src="assets/templates/precompiled.js"></script>
+    <script src="precompiled.js"></script>
     <script src="vendors/sugar.min.js"></script>
     <script src="nautilus.js"></script>
     <script src="init.js"></script>
     <div id="about-content">
         {{about_content|safe}}
-        {% if secondary_logo %}<hr /><img src="assets/secondary-logo.png" />{% endif %}
+        {% if secondary_logo %}<hr /><img src="secondary-logo.png" />{% endif %}
     </div>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 
 
 
 
-[assets/main-logo.png] [assets/info-circle-solid.svg]
+[main-logo.png] [info-circle-solid.svg]
 [Unknown INPUT type] {{ search_label }}
  ×
 {{ loading_label }}
 {{ no_result_text }}
 {{ loading_label }}
 â¡  {% if secondary_logo %}
 ===============================================================================
-[assets/secondary-logo.png]{% endif %}
+[secondary-logo.png]{% endif %}
 {{about_content|safe}} {% if secondary_logo %}
 ===============================================================================
-[assets/secondary-logo.png]{% endif %}
+[secondary-logo.png]{% endif %}
```

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/init.js` & `nautiluszim-1.1.0/nautiluszim/templates/init.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/nautilus.js` & `nautiluszim-1.1.0/nautiluszim/templates/nautilus.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -475,14 +475,15 @@
     }
 
     Nautilus.prototype.parsedIdent = function(ident) {
         // format::  {kind}-{modalId}-{options}
         // rando::   random-{modalId}-{id}.{id}.{id}
         // search::  search-{modalId}-{cursor}_{text}
         // list::    list-{modalId}-{cursor}
+        let parent = this;
 
         if (ident === undefined)
             ident = this.ident;
 
         let kind = modalId = options = documentIds = cursor = text = "";
 
         let parts = ident.split("-", 3);
@@ -497,15 +498,15 @@
                 .map(function(sid) {
                     return parseInt(sid);
                 })
                 .filter(function(id) {
                     return !isNaN(id)
                 })
                 .map(function(id) {
-                    return id.toString();
+                    return parent.zfill(id.toString());
                 });
         }
 
         if (kind == "search") {
             let opt_parts = options.split("_", 2);
             cursor = 0;
             text = opt_parts.pop().trim();
@@ -631,25 +632,29 @@
             if (on_complete)
                 on_complete.apply(_this, [rows]);
         }).catch(function(err) {
             _this.console.error("Error querying docs.", err);
         });
     };
 
+    Nautilus.prototype.zfill = function(number) {
+        return ('0000' + number).slice(-5);
+    };
+
     Nautilus.prototype.getRandomDocuments = function(on_complete) {
         var _this = this;
 
         function getRandomInt(max) {
             return Math.floor(Math.random() * max);
         }
 
         _this.console.log("getRandomDocuments", this.doc_count, this.options.nb_items_per_page);
         let seq_ids = [];
         for (var i = 0; i < this.options.nb_items_per_page; i++) {
-            seq_ids.push(getRandomInt(this.doc_count).toString());
+            seq_ids.push(this.zfill(getRandomInt(this.doc_count).toString()));
         }
         this.getRequestedDocuments("random", seq_ids, on_complete);
     };
 
     Nautilus.prototype.getSearchResults = function(text, on_complete) {
         this.console.debug("getting search results for", text);
         var _this = this;
```

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ScrollMagic.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ScrollMagic.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/.DS_Store` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/3ga.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/3ga.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/7z.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/7z.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aa.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aa.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aac.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aac.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ac.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ac.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/accdb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/accdt.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/accdt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/adn.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/adn.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ai.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ai.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aif.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aif.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aifc.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aifc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aiff.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aiff.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ait.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ait.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/amr.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/amr.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ani.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ani.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/apk.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/apk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/app.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/app.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/applescript.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/applescript.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asax.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asax.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ascx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ascx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ash.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ash.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ashx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ashx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asmx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asmx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aspx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aspx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/asx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/asx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/au.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/au.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/aup.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/aup.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/axd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/axd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bash.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bash.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bin.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bin.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bowerrc.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bowerrc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/browser.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/browser.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/bz2.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/bz2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cab.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cab.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cad.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cad.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/caf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/caf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cal.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cal.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/catalog.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/catalog.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cer.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cer.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cfg.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cfm.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cfml.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cfml.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/class.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/class.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/coffee.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/coffee.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/conf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/conf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/config.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/config.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cpp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cpp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cptx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cptx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/crdownload.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crdownload.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/crt.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/crypt.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/crypt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cs.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cs.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/csh.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cson.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cson.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/csproj.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/csproj.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/css.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/css.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/cue.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/cue.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dat.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dat.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/db.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/db.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dbf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dbf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/deb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/deb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dgn.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dgn.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/diz.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/diz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dmg.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dmg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/download.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/download.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dpj.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dpj.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ds_store.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ds_store.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dtd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dtd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dwg.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dwg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/dxf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/dxf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/editorconfig.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/editorconfig.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/el.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/el.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/enc.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/enc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/eot.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eot.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/eps.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/eps.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/epub.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/epub.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/exe.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/exe.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/f4v.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/f4v.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/fax.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fax.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/fb2.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/fb2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/flac.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flac.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/flv.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/flv.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gdp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gdp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gem.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gem.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gitattributes.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gitattributes.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/go.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/go.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/gz.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/gz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/handlebars.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/handlebars.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/hbs.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/hbs.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/htm.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/htm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/html.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/html.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ibooks.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ibooks.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/icns.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/icns.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ico.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ico.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ics.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ics.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/idx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/idx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/iff.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iff.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ifo.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ifo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/img.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/img.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/inf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/inf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ini.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ini.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/iso.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/iso.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/j2.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/j2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jar.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/java.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/java.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/js.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/js.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/json.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/json.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jsp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/jsx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/jsx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/kf8.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kf8.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/kmk.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kmk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ksh.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ksh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/kup.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/kup.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/less.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/less.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lex.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lex.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/licx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/licx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lisp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lisp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lit.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lit.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lnk.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lnk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/lock.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/lock.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m3u.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m3u8.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m3u8.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4a.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4a.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/m4r.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/m4r.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/map.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/map.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mc.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mdb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mdf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mdf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mi.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mid.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mid.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/midi.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/midi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mk.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mo.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mobi.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mobi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mod.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mod.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mov.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mov.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mp2.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mp3.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mp3.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpa.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpa.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpga.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpga.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/mpt.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/mpt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/msi.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/msu.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/msu.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/nes.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nes.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/nfo.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/nfo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/odb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ods.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ods.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/odt.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/odt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ogg.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ogg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ost.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ost.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/otf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/otf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ott.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ott.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ova.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ova.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ovf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ovf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pages.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pages.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/part.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/part.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pdb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pdf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pem.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pem.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ph.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ph.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/phar.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/phar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/php.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/php.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pkg.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pkg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pl.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pl.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/plist.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/plist.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pm.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/po.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/po.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pom.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pom.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pot.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pot.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ps.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ps1.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ps1.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/psd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/psd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pst.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pst.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pub.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pub.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/py.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/py.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/pyc.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/pyc.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/qt.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/qt.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ra.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ra.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ram.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ram.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rar.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/resx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/resx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rom.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rom.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rpm.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rpm.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rsa.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rsa.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rss.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rss.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ru.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ru.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/rub.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/rub.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sass.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sass.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/scss.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/scss.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sdf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sdf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sed.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sed.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sh.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sitemap.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sitemap.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/skin.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/skin.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sln.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sln.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sol.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sol.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sql.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sql.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sqlite.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sqlite.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/step.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/step.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/stl.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/stl.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/svg.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/svg.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/swd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/swf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/swift.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/swift.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/sys.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/sys.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tar.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tar.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tgz.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tgz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/tmp.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/tmp.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/torrent.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/torrent.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ts.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ts.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/ttf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/ttf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/udf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/udf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vbproj.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbproj.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vbs.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vbs.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vcd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vcd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vdi.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vdx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vdx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vmdk.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vmdk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vsd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vss.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vss.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vst.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vst.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vsx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vsx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/vtx.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/vtx.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/war.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/war.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wav.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wav.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wbk.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wbk.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/webinfo.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/webinfo.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wma.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wma.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wmf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wmf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/woff.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/woff2.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/woff2.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wps.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wps.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/wsf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/wsf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xcf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xcf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xpi.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xpi.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xrb.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xrb.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xsd.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xsd.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xspf.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xspf.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/xz.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/xz.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/z.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/z.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/zip.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zip.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ext-icons/zsh.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ext-icons/zsh.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.6.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /**!
 
  @license
- handlebars v4.7.6
+ handlebars v4.7.7
 
 Copyright (C) 2011-2019 by Yehuda Katz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -93,15 +93,15 @@
             g = c(5),
             h = e(g),
             i = c(9),
             j = c(29),
             k = c(31),
             l = e(k),
             m = c(32),
-            n = "4.7.6";
+            n = "4.7.7";
         b.VERSION = n;
         var o = 8;
         b.COMPILER_REVISION = o;
         var p = 7;
         b.LAST_COMPATIBLE_COMPILER_REVISION = p;
         var q = {
             1: "<= 1.0.rc.2",
@@ -701,15 +701,15 @@
             a.main.decorator = a.main_d, b.VM.checkRevision(a.compiler);
             var e = a.compiler && 7 === a.compiler[0],
                 g = {
                     strict: function(a, b, c) {
                         if (!(a && b in a)) throw new u["default"]('"' + b + '" not defined in ' + a, {
                             loc: c
                         });
-                        return a[b]
+                        return g.lookupProperty(a, b)
                     },
                     lookupProperty: function(a, b) {
                         var c = a[b];
                         return null == c ? c : Object.prototype.hasOwnProperty.call(a, b) ? c : y.resultIsAllowed(c, g.protoAccessControl, b) ? c : void 0
                     },
                     lookup: function(a, b) {
                         for (var c = a.length, d = 0; d < c; d++) {
```

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/jquery.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/jquery.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/README.md` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/README.md`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-support.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-support.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-version.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-version.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/ogvjs/ogv.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/ogvjs/ogv.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/pouchdb.find.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.find.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/pouchdb.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/pouchdb.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/sugar.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/sugar.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/VideoJS.svg` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/font/VideoJS.woff` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/font/VideoJS.woff`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ar.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ar.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ar.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ba.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ba.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ba.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/bg.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/bg.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/bg.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ca.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ca.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ca.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cs.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cs.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cs.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cy.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/cy.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/cy.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/da.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/da.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/da.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/de.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/de.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/de.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/el.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/el.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/el.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/en.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/en.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/en.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/es.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/es.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/es.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fa.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fa.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fa.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fi.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fi.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fi.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fr.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/fr.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/fr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gd.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gd.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gd.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gl.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/gl.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/gl.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/he.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/he.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/he.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hr.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hr.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hu.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/hu.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/hu.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/it.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/it.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/it.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ja.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ja.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ja.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ko.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ko.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ko.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nb.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nb.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nb.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nl.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nl.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nl.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nn.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/nn.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/nn.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/oc.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/oc.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/oc.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pl.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pl.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pl.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-BR.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-BR.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-BR.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-PT.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/pt-PT.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/pt-PT.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ru.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/ru.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/ru.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sk.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sk.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sk.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sr.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sr.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sv.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/sv.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/sv.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/tr.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/tr.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/tr.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/uk.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/uk.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/uk.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/vi.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/vi.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/vi.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-CN.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-CN.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-CN.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-TW.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/lang/zh-TW.json` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/lang/zh-TW.json`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video-js.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video-js.min.css` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video-js.min.css`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.cjs.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.cjs.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.es.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.es.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs/video.min.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs/video.min.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.0.8/nautiluszim/templates/vendors/videojs-ogvjs.js` & `nautiluszim-1.1.0/nautiluszim/templates/vendors/videojs-ogvjs.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -742,15 +742,15 @@
                  * Determine if the specified media type can be played back
                  * by the Tech
                  *
                  * @param  {String} type  A media type description
                  * @return {String}         'probably', 'maybe', or '' (empty string)
                  */
                 Ogvjs.canPlayType = function(type) {
-                    return (type.indexOf('/webm') !== -1 || type.indexOf('/ogg') !== -1) ? 'maybe' : '';
+                    return type.indexOf('/ogg') !== -1 ? 'maybe' : '';
                 };
 
                 /*
                  * Check if the tech can support the given source
                  * @param  {Object} srcObj  The source object
                  * @return {String}         'probably', 'maybe', or '' (empty string)
                  */
```

### Comparing `nautiluszim-1.0.8/nautiluszim.egg-info/PKG-INFO` & `nautiluszim-1.1.0/nautiluszim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 Metadata-Version: 2.1
 Name: nautiluszim
-Version: 1.0.8
+Version: 1.1.0
 Summary: turns a collection of documents into a browsable ZIM file
 Home-page: https://github.com/openzim/nautilus
 Author: kiwix
 Author-email: reg@kiwix.org
 License: GPLv3+
 Keywords: kiwix zim offline
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Nautilus
 =============
 
 [![CodeFactor](https://www.codefactor.io/repository/github/openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/nautilus)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/nautiluszim/)
+[![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/latest_tag?label=docker)](https://ghcr.io/openzim/nautilus)
 
 `nautilus` turns a collection of documents into a browsable [ZIM file](https://openzim.org).
 
-It downloads the video (webm or mp4 format – optionnaly recompress them in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it create a static HTML files folder of it before creating a ZIM off of it.
+It downloads the video (webm or mp4 format – optionally recompress it in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it creates a static HTML files folder of it before creating a ZIM off of it.
 
 # Preparing the archive
 
 To be used with nautilus, your archive should be a ZIP file.
-
 * it doesn't need to be structured, but it can.
 * it doesn't need to be compressed. It's usually recommended not to.
-* it should contain a `collection.json` file, but it can also provided separately (see below).
+* it should contain a `collection.json` file, but it can also be provided separately (see below).
 * it should only contain to-be-included files. No filtering is done.
-* Audio and video files should be in ogg format with `.ogg`/`.ogv` extension to be supported on all platform (`mp3`/`mp4` would work only on platform with native support).
+* Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension to be supported on all platforms (`mp3`/`mp4` would work only on platforms with native support).
 
 ```
 cd content/path
 zip -r -0 -T ../content_name.zip *
 ```
 
 ## JSON collection file
 
 Either inside the archive ZIP as `/collection.json` or elsewhere, 
 specified via `--collection mycollection.json`, you must supply a JSON file describing your content.
 
 The user-interface only gives access to files referenced properly in the collection.
 
-At the moment, the JSON files needs to provide the following fields for each item in an Array:
+At the moment, the JSON file needs to provide the following fields for each item in an array:
 
 ``` JSON
 [
     {
         "title": "...",
         "description": "...",
         "authors": "...",
@@ -64,35 +65,36 @@
      }
 ]
 ```
 
 ## About page
 
 Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--about myabout.html`,
-you may supply an about page in HTML format. It will be displayed in a modal popup and will include
-at its bottom your *secondary-logo* if provided.
+
+- You may supply an about page in HTML format. It will be displayed in a modal popup and will be included.
+- At its bottom your *secondary-logo* if provided.
 
 * Use only content tags (no `<html />` nor `<head />` nor `<script />` etc)
-* Use inline styling if required but no styling is recommended.
+* Use inline styling if required, but no styling is recommended.
 * Include one logo inline if required.
 
 # Requirements
 
 * `wget` and `unzip` to install JS dependencies. See `get_js_deps.sh` if you want to do it manually.
 * `wget` is used to download archive files as well.
 * [`handlebars`](https://handlebarsjs.com) is used to compile JS templates
 
 # Installation
 
-`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtualenv. See `requirements.txt` for the list of python dependencies.
+`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtual-environment. See `requirements.txt` for the list of python dependencies.
 
 ## docker
 
 ```
-docker run -v my_dir:/output openzim/nautilus nautiluszim --help
+docker run -v my_dir:/output ghcr.io/openzim/nautilus nautiluszim --help
 ```
 
 ## pip
 
 ```
 pip install nautiluszim
 nautiluszim --help
@@ -102,18 +104,16 @@
 
 ```
 nautiluszim --archive my-content.zip
 ```
 
 ## Notes
 
-* On macOS, the locale setting is buggy. You need to launch it with `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
+* On macOS, the locale setting is buggy. You need to launch it with the `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
 
 ```
 LANGUAGE=fr nautiluszim --language fra
 ```
 
 ## Development
 
 See [CONTRIBUTING.md](CONTRIBUTING.md)
-
-
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_29k511yl_/tmpsvak5qtw_TarContainer/0/587", line 120, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_29k511yl_/tmpsvak5qtw_TarContainer/0/587", line 120, column 0: CDATA terminal not found*

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1 Name: nautiluszim Version: 1.0.8 Summary: turns a
+Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.0 Summary: turns a
 collection of documents into a browsable ZIM file Home-page: https://
 github.com/openzim/nautilus Author: kiwix Author-email: reg@kiwix.org License:
-GPLv3+ Keywords: kiwix zim offline Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+GPLv3+ Keywords: kiwix zim offline Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE Nautilus ============= [![CodeFactor]
-(https://www.codefactor.io/repository/github/openzim/nautilus/badge)](https://
-www.codefactor.io/repository/github/openzim/nautilus) [![License: GPL v3]
-(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
-licenses/gpl-3.0) [![PyPI version shields.io](https://img.shields.io/pypi/v/
-nautiluszim.svg)](https://pypi.org/project/nautiluszim/) `nautilus` turns a
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE Nautilus
+============= [![CodeFactor](https://www.codefactor.io/repository/github/
+openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/
+nautilus) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-
+blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![PyPI version shields.io]
+(https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/
+nautiluszim/) [![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/
+latest_tag?label=docker)](https://ghcr.io/openzim/nautilus) `nautilus` turns a
 collection of documents into a browsable [ZIM file](https://openzim.org). It
-downloads the video (webm or mp4 format â optionnaly recompress them in
-lower-quality, smaller size), the thumbnails, the subtitles and the authors'
-profile pictures ; then, it create a static HTML files folder of it before
-creating a ZIM off of it. # Preparing the archive To be used with nautilus,
-your archive should be a ZIP file. * it doesn't need to be structured, but it
-can. * it doesn't need to be compressed. It's usually recommended not to. * it
-should contain a `collection.json` file, but it can also provided separately
-(see below). * it should only contain to-be-included files. No filtering is
-done. * Audio and video files should be in ogg format with `.ogg`/`.ogv`
-extension to be supported on all platform (`mp3`/`mp4` would work only on
-platform with native support). ``` cd content/path zip -r -0 -T ../
-content_name.zip * ``` ## JSON collection file Either inside the archive ZIP as
-`/collection.json` or elsewhere, specified via `--collection
-mycollection.json`, you must supply a JSON file describing your content. The
-user-interface only gives access to files referenced properly in the
-collection. At the moment, the JSON files needs to provide the following fields
-for each item in an Array: ``` JSON [ { "title": "...", "description": "...",
-"authors": "...", "files": ["relative/path/to/file"] } ] ``` ## About page
-Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--
-about myabout.html`, you may supply an about page in HTML format. It will be
-displayed in a modal popup and will include at its bottom your *secondary-logo*
-if provided. * Use only content tags (no `
+downloads the video (webm or mp4 format â optionally recompress it in lower-
+quality, smaller size), the thumbnails, the subtitles and the authors' profile
+pictures ; then, it creates a static HTML files folder of it before creating a
+ZIM off of it. # Preparing the archive To be used with nautilus, your archive
+should be a ZIP file. * it doesn't need to be structured, but it can. * it
+doesn't need to be compressed. It's usually recommended not to. * it should
+contain a `collection.json` file, but it can also be provided separately (see
+below). * it should only contain to-be-included files. No filtering is done. *
+Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension
+to be supported on all platforms (`mp3`/`mp4` would work only on platforms with
+native support). ``` cd content/path zip -r -0 -T ../content_name.zip * ``` ##
+JSON collection file Either inside the archive ZIP as `/collection.json` or
+elsewhere, specified via `--collection mycollection.json`, you must supply a
+JSON file describing your content. The user-interface only gives access to
+files referenced properly in the collection. At the moment, the JSON file needs
+to provide the following fields for each item in an array: ``` JSON [
+{ "title": "...", "description": "...", "authors": "...", "files": ["relative/
+path/to/file"] } ] ``` ## About page Either inside the archive ZIP as `/
+about.html` or elsewhere, specified via `--about myabout.html`, - You may
+supply an about page in HTML format. It will be displayed in a modal popup and
+will be included. - At its bottom your *secondary-logo* if provided. * Use only
+content tags (no `
 ` nor `
 ` nor `
```

### Comparing `nautiluszim-1.0.8/nautiluszim.egg-info/SOURCES.txt` & `nautiluszim-1.1.0/nautiluszim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 nautiluszim/VERSION
 nautiluszim/__init__.py
 nautiluszim/__main__.py
 nautiluszim/constants.py
 nautiluszim/entrypoint.py
 nautiluszim/scraper.py
 nautiluszim.egg-info/PKG-INFO
 nautiluszim.egg-info/SOURCES.txt
 nautiluszim.egg-info/dependency_links.txt
 nautiluszim.egg-info/entry_points.txt
 nautiluszim.egg-info/not-zip-safe
 nautiluszim.egg-info/requires.txt
 nautiluszim.egg-info/top_level.txt
-nautiluszim/__pycache__/__init__.cpython-38.pyc
-nautiluszim/__pycache__/__main__.cpython-38.pyc
-nautiluszim/__pycache__/constants.cpython-38.pyc
-nautiluszim/__pycache__/entrypoint.cpython-38.pyc
-nautiluszim/__pycache__/scraper.cpython-38.pyc
 nautiluszim/locale/messages.pot
 nautiluszim/locale/fr/LC_MESSAGES/messages.mo
 nautiluszim/locale/fr/LC_MESSAGES/messages.po
 nautiluszim/templates/database.js
 nautiluszim/templates/display_rows.handlebars
 nautiluszim/templates/favicon.png
 nautiluszim/templates/home.html
+nautiluszim/templates/info-circle-solid.svg
 nautiluszim/templates/init.js
+nautiluszim/templates/main-logo.png
 nautiluszim/templates/media_player.handlebars
 nautiluszim/templates/modal_empty_body.handlebars
 nautiluszim/templates/modal_title.handlebars
 nautiluszim/templates/nautilus.js
-nautiluszim/templates/assets/info-circle-solid.svg
-nautiluszim/templates/assets/main-logo.png
-nautiluszim/templates/assets/styles.css
-nautiluszim/templates/assets/templates/precompiled.js
+nautiluszim/templates/precompiled.js
+nautiluszim/templates/styles.css
 nautiluszim/templates/vendors/ScrollMagic.min.js
-nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.6.js
 nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js
 nautiluszim/templates/vendors/jquery.min.js
 nautiluszim/templates/vendors/pouchdb.find.min.js
 nautiluszim/templates/vendors/pouchdb.min.js
 nautiluszim/templates/vendors/sugar.min.js
 nautiluszim/templates/vendors/videojs-ogvjs.js
 nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css
```

### Comparing `nautiluszim-1.0.8/setup.py` & `nautiluszim-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 
 def read(*names, **kwargs):
     with open(root_dir.joinpath(*names), "r") as fh:
         return fh.read()
 
 
-print("Downloading and fixing JS dependencies...")
-subprocess.run([str(root_dir.joinpath("get_js_deps.sh").resolve())], check=True)
-
-print("Compile handlebars templates")
-subprocess.run(
-    [
-        "/usr/bin/env",
-        "handlebars",
-        str(root_dir / "nautiluszim" / "templates"),
-        "-f",
-        str(
-            root_dir.joinpath(
-                "nautiluszim", "templates", "assets", "templates", "precompiled.js"
-            )
-        ),
-    ],
-    check=True,
-)
+if not root_dir.joinpath(
+    "nautiluszim/templates/vendors", "handlebars.runtime.min-v4.7.7.js"
+).exists():
+    print("Downloading and fixing JS dependencies...")
+    subprocess.run([str(root_dir.joinpath("get_js_deps.sh").resolve())], check=True)
+
+if not root_dir.joinpath("nautiluszim/templates/precompiled.js").exists():
+    print("Compile handlebars templates")
+    subprocess.run(
+        [
+            "/usr/bin/env",
+            "handlebars",
+            str(root_dir / "nautiluszim" / "templates"),
+            "-f",
+            str(root_dir.joinpath("nautiluszim", "templates", "precompiled.js")),
+        ],
+        check=True,
+    )
 
 
 setup(
     name="nautiluszim",
     version=read("nautiluszim", "VERSION").strip(),
     description="turns a collection of documents into a browsable ZIM file",
     long_description=read("README.md"),
@@ -52,17 +52,19 @@
         for line in read("requirements.txt").splitlines()
         if not line.strip().startswith("#")
     ],
     zip_safe=False,
     include_package_data=True,
     entry_points={"console_scripts": ["nautiluszim=nautiluszim.__main__:main"]},
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

