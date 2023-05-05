# Comparing `tmp/pcleaner-1.6.2.tar.gz` & `tmp/pcleaner-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.6.2.tar", last modified: Fri Apr 21 16:14:32 2023, max compression
+gzip compressed data, was "pcleaner-1.6.9.tar", last modified: Fri May  5 16:06:36 2023, max compression
```

## Comparing `pcleaner-1.6.2.tar` & `pcleaner-1.6.9.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.6.2/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11713 2023-04-21 16:14:32.144190 pcleaner-1.6.2/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.6.2/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-04-21 14:42:06.000000 pcleaner-1.6.2/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-04-21 13:38:35.000000 pcleaner-1.6.2/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5841 2023-04-14 16:52:21.000000 pcleaner-1.6.2/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    40890 2023-04-21 14:58:00.000000 pcleaner-1.6.2/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.6.2/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.6.2/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.6.2/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.6.2/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.6.2/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2573 2023-04-21 14:17:14.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1104 2023-04-21 15:08:03.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.6.2/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-04-17 02:04:01.000000 pcleaner-1.6.2/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1904 2023-04-17 01:26:57.000000 pcleaner-1.6.2/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    36580 2023-04-21 14:12:49.000000 pcleaner-1.6.2/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    15167 2023-04-21 15:23:47.000000 pcleaner-1.6.2/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.6.2/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    82099 2023-04-21 14:48:43.000000 pcleaner-1.6.2/pcleaner/gui/rc_generated_files/icons_rc.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    29657 2023-04-21 14:26:59.000000 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-04-17 16:45:08.000000 pcleaner-1.6.2/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1321 2023-04-17 02:10:39.000000 pcleaner-1.6.2/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23339 2023-04-20 18:43:01.000000 pcleaner-1.6.2/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    26308 2023-04-20 18:43:01.000000 pcleaner-1.6.2/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-04-18 15:30:06.000000 pcleaner-1.6.2/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.6.2/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8778 2023-04-18 20:36:25.000000 pcleaner-1.6.2/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.6.2/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-04-18 20:03:45.000000 pcleaner-1.6.2/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11713 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2058 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.6.2/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-04-21 16:14:32.144190 pcleaner-1.6.2/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.6.2/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.177426 pcleaner-1.6.9/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.6.9/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-05 16:06:36.177426 pcleaner-1.6.9/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.6.9/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.170759 pcleaner-1.6.9/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-05-05 15:54:59.000000 pcleaner-1.6.9/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.6.9/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.6.9/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.170759 pcleaner-1.6.9/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.170759 pcleaner-1.6.9/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.174092 pcleaner-1.6.9/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.174092 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.6.9/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    45416 2023-05-05 16:06:03.000000 pcleaner-1.6.9/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.6.9/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.174092 pcleaner-1.6.9/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.6.9/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.6.9/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.6.9/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.6.9/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.174092 pcleaner-1.6.9/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.177426 pcleaner-1.6.9/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1104 2023-04-21 15:08:03.000000 pcleaner-1.6.9/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.6.9/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.6.9/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.6.9/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1119 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.6.9/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    40917 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16292 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.177426 pcleaner-1.6.9/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.6.9/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.6.9/pcleaner/gui/rc_generated_files/icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    75061 2023-04-22 17:01:02.000000 pcleaner-1.6.9/pcleaner/gui/rc_generated_files/theme_icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.177426 pcleaner-1.6.9/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.6.9/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.6.9/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    29795 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.6.9/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.6.9/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23467 2023-05-05 14:10:21.000000 pcleaner-1.6.9/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27027 2023-05-05 16:00:19.000000 pcleaner-1.6.9/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-04-18 15:30:06.000000 pcleaner-1.6.9/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.6.9/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8778 2023-05-04 20:46:40.000000 pcleaner-1.6.9/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7581 2023-05-04 21:08:14.000000 pcleaner-1.6.9/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-04-18 20:03:45.000000 pcleaner-1.6.9/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 16:06:36.170759 pcleaner-1.6.9/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-05 16:06:36.000000 pcleaner-1.6.9/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-05-05 16:06:36.000000 pcleaner-1.6.9/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-05-05 16:06:36.000000 pcleaner-1.6.9/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-05-05 16:06:36.000000 pcleaner-1.6.9/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-05-05 16:06:36.000000 pcleaner-1.6.9/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-05-05 16:06:36.000000 pcleaner-1.6.9/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.6.9/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-05-05 16:06:36.177426 pcleaner-1.6.9/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.6.9/setup.py
```

### Comparing `pcleaner-1.6.2/LICENSE` & `pcleaner-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/PKG-INFO` & `pcleaner-1.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.6.2
+Version: 1.6.9
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -108,14 +108,38 @@
 Install the program with pip from [PyPI](https://pypi.org/project/pcleaner/):
 ```bash
 pip install pcleaner
 ```
 
 Note: The program has only been tested on Linux and on Windows with WSL, but should work on Windows (natively) and Mac as well.
 
+### Install with Docker
+
+Build the image with buildx:
+```bash
+docker buildx build -t pcleaner:v1 .
+
+```
+Or with the legacy builder:
+```bash
+docker image build -t pcleaner:v1 .
+```
+
+Then initialize the docker image, specifying a root folder for the container to access.
+In this example, the current directory (`pwd`) is used:
+```bash
+docker run -it --name pcleaner -v $(pwd):/app pcleaner:v1
+```
+This will also start an interactive shell in the container.
+
+You can open another one later on with:
+```bash
+docker start pcleaner
+docker exec -it pcleaner bash
+```
 
 ## Usage
 
 The program is run from the command line, and, in the most common use, takes any number of images or directories as input. The program will create a new directory called `cleaned` in the same directory as the input files, and place the cleaned images and/or masks there. Often, it's more useful to only export the mask layer, and you can do so by adding the `--save-only-mask`, or `-m` for short, option.
 
 Examples:
 ```bash
```

### Comparing `pcleaner-1.6.2/README.md` & `pcleaner-1.6.9/pcleaner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pcleaner
+Version: 1.6.9
+Summary: An AI-powered tool to clean manga panels.
+Home-page: https://github.com/VoxelCubes/PanelCleaner
+Keywords: image processing,cleaning,text removal,manga,ai,machine learning
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Natural Language :: English
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENSE
+
 # Panel Cleaner
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://img.shields.io/pypi/v/pcleaner)](https://pypi.org/project/pcleaner/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This tool uses machine learning to find text and then generates masks to cover it up with the highest accuracy possible. It is designed to clean easy bubbles, no in-painting or out-of-bubble text removal is done. This is intended to save a lot of monotonous work for people who have to clean a lot of panels, while making sure it doesn't paint over anything that it wasn't supposed to.
@@ -92,14 +108,38 @@
 Install the program with pip from [PyPI](https://pypi.org/project/pcleaner/):
 ```bash
 pip install pcleaner
 ```
 
 Note: The program has only been tested on Linux and on Windows with WSL, but should work on Windows (natively) and Mac as well.
 
+### Install with Docker
+
+Build the image with buildx:
+```bash
+docker buildx build -t pcleaner:v1 .
+
+```
+Or with the legacy builder:
+```bash
+docker image build -t pcleaner:v1 .
+```
+
+Then initialize the docker image, specifying a root folder for the container to access.
+In this example, the current directory (`pwd`) is used:
+```bash
+docker run -it --name pcleaner -v $(pwd):/app pcleaner:v1
+```
+This will also start an interactive shell in the container.
+
+You can open another one later on with:
+```bash
+docker start pcleaner
+docker exec -it pcleaner bash
+```
 
 ## Usage
 
 The program is run from the command line, and, in the most common use, takes any number of images or directories as input. The program will create a new directory called `cleaned` in the same directory as the input files, and place the cleaned images and/or masks there. Often, it's more useful to only export the mask layer, and you can do so by adding the `--save-only-mask`, or `-m` for short, option.
 
 Examples:
 ```bash
```

### Comparing `pcleaner-1.6.2/pcleaner/analytics.py` & `pcleaner-1.6.9/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/cli_utils.py` & `pcleaner-1.6.9/pcleaner/cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     else:  # ???
         raise NotImplementedError("Your OS is currently not supported.")
 
     path.parent.mkdir(parents=True, exist_ok=True)
     return path
 
 
+def get_default_profile_path(profile_name: str | None = None) -> Path:
+    if profile_name is None:
+        return get_config_path().parent / "profiles"
+    return get_config_path().parent / "profiles" / f"{profile_name}.conf"
+
+
 def get_cache_path() -> Path:
     """
     Get the default suggested path to the cache directory for both Linux and Windows.
     """
     if platform.system() == "Linux":
         path = Path(XDG_CACHE_HOME, __program__)
     elif platform.system() == "Windows":
@@ -70,14 +76,19 @@
 
     :param path: The path to the file to open.
     :param configured_opener: The configured editor to use.
     """
     if platform.system() == "Linux":
         opener = "xdg-open" if configured_opener is None else configured_opener
         print(f"Opening {path} with {opener}.")
+        # Test if the configured editor exists. Even xdg-open may be missing, like in a docker container.
+        if shutil.which(opener) is None:
+            print(f"Configured editor '{opener}' not found. "
+                  f"Please open the file manually or configure another program.")
+            return
         # Run and detatch the process, so this one can exit.
         subprocess.Popen([opener, path], start_new_session=True)
 
         print("If nothing happens, try setting the profile_editor option in the config.")
 
     elif platform.system() == "Windows":
         opener = "start" if configured_opener is None else configured_opener
```

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.6.9/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/config.py` & `pcleaner-1.6.9/pcleaner/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, NewType
 
 import configupdater as cu
 from logzero import logger
 
 from pcleaner import cli_utils as cli
 from pcleaner import model_downloader as md
+from pcleaner import helpers as hp
 
 RESERVED_PROFILE_NAMES = ["builtin", "none", "default"]
 
 # Supported image suffixes.
 SUPPORTED_IMG_TYPES = [
     ".jpeg",
     ".jpg",
@@ -82,14 +83,41 @@
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
         try_to_load(self, config_updater, section, str | None, "preferred_file_type")
         try_to_load(self, config_updater, section, str, "preferred_mask_file_type")
         try_to_load(self, config_updater, section, float | GreaterZero, "input_size_scale")
 
+    def fix(self):
+        """
+        Fix the config values.
+        """
+        if (
+            self.preferred_file_type is not None
+            and self.preferred_file_type.lower() not in SUPPORTED_IMG_TYPES
+        ):
+            closest = hp.closest_match(self.preferred_file_type.lower(), SUPPORTED_IMG_TYPES)
+            if closest is None:
+                logger.error(
+                    f"Could not recover from invalid preferred_file_type: {self.preferred_file_type}, using default."
+                )
+            self.preferred_file_type = closest
+
+        if self.preferred_mask_file_type is None:
+            self.preferred_mask_file_type = SUPPORTED_MASK_TYPES[0]
+
+        if self.preferred_mask_file_type.lower() not in SUPPORTED_MASK_TYPES:
+            closest = hp.closest_match(self.preferred_mask_file_type.lower(), SUPPORTED_MASK_TYPES)
+            if closest is None:
+                logger.error(
+                    f"Could not recover from invalid preferred_mask_file_type: {self.preferred_mask_file_type}, using default."
+                )
+                closest = SUPPORTED_MASK_TYPES[0]
+            self.preferred_mask_file_type = closest
+
 
 @dataclass
 class TextDetectorConfig:
     model_path: str | None = None
     concurrent_models: int | GreaterZero = 1
 
     def export_to_conf(
@@ -135,14 +163,24 @@
         if not config_updater.has_section("TextDetector"):
             logger.info("No TextDetector section found in the profile, using defaults.")
             return
 
         try_to_load(self, config_updater, "TextDetector", str | None, "model_path")
         try_to_load(self, config_updater, "TextDetector", int | GreaterZero, "concurrent_models")
 
+    def fix(self):
+        """
+        Fix the config values.
+        Numbers flagged as greater than zero are already fixed then loading.
+        """
+        if self.model_path is not None:
+            if not Path(self.model_path).exists():
+                logger.error(f"Could not find model file: {self.model_path}, using default.")
+                self.model_path = None
+
 
 @dataclass
 class PreProcessorConfig:
     box_min_size: int = 20 * 20
     suspicious_box_min_size: int = 200 * 200
     ocr_enabled: bool = True
     ocr_max_size: int = 30 * 100
@@ -235,14 +273,35 @@
         try_to_load(self, config_updater, section, str, "ocr_blacklist_pattern")
         try_to_load(self, config_updater, section, int, "box_padding_initial")
         try_to_load(self, config_updater, section, int, "box_right_padding_initial")
         try_to_load(self, config_updater, section, int, "box_padding_extended")
         try_to_load(self, config_updater, section, int, "box_right_padding_extended")
         try_to_load(self, config_updater, section, int, "box_reference_padding")
 
+    def fix(self):
+        """
+        Ensure all numbers are greater equal 0.
+        """
+        if self.box_min_size < 0:
+            self.box_min_size = 0
+        if self.suspicious_box_min_size < 0:
+            self.suspicious_box_min_size = 0
+        if self.ocr_max_size < 0:
+            self.ocr_max_size = 0
+        if self.box_padding_initial < 0:
+            self.box_padding_initial = 0
+        if self.box_right_padding_initial < 0:
+            self.box_right_padding_initial = 0
+        if self.box_padding_extended < 0:
+            self.box_padding_extended = 0
+        if self.box_right_padding_extended < 0:
+            self.box_right_padding_extended = 0
+        if self.box_reference_padding < 0:
+            self.box_reference_padding = 0
+
 
 @dataclass
 class MaskerConfig:
     mask_growth_step_pixels: int | GreaterZero = 2
     mask_growth_steps: int = 11
     off_white_max_threshold: int = 240
     mask_improvement_threshold: float = 0.1
@@ -332,27 +391,41 @@
                     f"Invalid color tuple length. Expected 4: 'Red, Green, Blue, Alpha' got {len(color_tuple)}"
                 )
             color_tuple: tuple[int, int, int, int]
             self.debug_mask_color = color_tuple
         except (cu.NoOptionError, ValueError):
             pass
 
+    def fix(self):
+        """
+        Keep the numbers greater or equal to zero.
+        For numbers, ensure the range 0-255.
+        """
+        self.mask_growth_steps = max(0, self.mask_growth_steps)
+        self.off_white_max_threshold = max(0, min(255, self.off_white_max_threshold))
+        if self.mask_improvement_threshold < 0:
+            self.mask_improvement_threshold = 0
+        if self.mask_max_standard_deviation < 0:
+            self.mask_max_standard_deviation = 0
+        # We already ensured that it's a tuple of 4 ints.
+        # noinspection PyTypeChecker
+        self.debug_mask_color = tuple(max(0, min(255, x)) for x in self.debug_mask_color)
+
 
 @dataclass
 class DenoiserConfig:
     denoising_enabled: bool = True
     noise_min_standard_deviation: float = 0.25
     noise_outline_size: int = 5
     noise_fade_radius: int = 1
     colored_images: bool = False
     filter_strength: int = 10
     color_filter_strength: int = 10
     template_window_size: int = 7
     search_window_size: int = 21
-    # TODO respect denoising enabled
 
     def export_to_conf(
         self, config_updater: cu.ConfigUpdater, add_after_section: str, gui_mode: bool = False
     ) -> None:
         """
         Write the config to the config updater object.
 
@@ -417,35 +490,52 @@
         :param config_updater: An existing config updater object.
         """
         section = "Denoiser"
         if not config_updater.has_section(section):
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
+        try_to_load(self, config_updater, section, bool, "denoising_enabled")
         try_to_load(self, config_updater, section, float, "noise_min_standard_deviation")
         try_to_load(self, config_updater, section, int, "noise_outline_size")
         try_to_load(self, config_updater, section, int, "noise_fade_radius")
         try_to_load(self, config_updater, section, bool, "colored_images")
         try_to_load(self, config_updater, section, int, "filter_strength")
         try_to_load(self, config_updater, section, int, "color_filter_strength")
         try_to_load(self, config_updater, section, int, "template_window_size")
         try_to_load(self, config_updater, section, int, "search_window_size")
 
+    def fix(self):
+        if self.noise_min_standard_deviation < 0:
+            self.noise_min_standard_deviation = 0
+        if self.noise_outline_size < 0:
+            self.noise_outline_size = 0
+        if self.noise_fade_radius < 0:
+            self.noise_fade_radius = 0
+        if self.filter_strength < 0:
+            self.filter_strength = 0
+        if self.color_filter_strength < 0:
+            self.color_filter_strength = 0
+        if self.template_window_size < 0:
+            self.template_window_size = 0
+        if self.search_window_size < 0:
+            self.search_window_size = 0
+
 
 @dataclass
 class Profile:
     """
     A profile is a collection of settings that can be saved and loaded from disk.
     """
 
-    general: GeneralConfig = GeneralConfig()
-    text_detector: TextDetectorConfig = TextDetectorConfig()
-    pre_processor: PreProcessorConfig = PreProcessorConfig()
-    masker: MaskerConfig = MaskerConfig()
-    denoiser: DenoiserConfig = DenoiserConfig()
+    general: GeneralConfig = field(default_factory=GeneralConfig)
+    text_detector: TextDetectorConfig = field(default_factory=TextDetectorConfig)
+    pre_processor: PreProcessorConfig = field(default_factory=PreProcessorConfig)
+    masker: MaskerConfig = field(default_factory=MaskerConfig)
+    denoiser: DenoiserConfig = field(default_factory=DenoiserConfig)
 
     def bundle_config(self, gui_mode: bool = False) -> cu.ConfigUpdater:
         """
         Bundle the config into a ConfigUpdater object.
 
         :param gui_mode: When true, strips out the CLI-specific options and keeps the GUI-specific ones,
             and vice versa.
@@ -454,14 +544,24 @@
         self.general.export_to_conf(config_updater, gui_mode=gui_mode)
         self.text_detector.export_to_conf(config_updater, "General", gui_mode=gui_mode)
         self.pre_processor.export_to_conf(config_updater, "TextDetector", gui_mode=gui_mode)
         self.masker.export_to_conf(config_updater, "PreProcessor", gui_mode=gui_mode)
         self.denoiser.export_to_conf(config_updater, "Masker", gui_mode=gui_mode)
         return config_updater
 
+    def hash_current_values(self) -> int:
+        """
+        Hash the current values of the profile.
+        This isn't implementing __hash__ because these objects are mutable.
+        This is merely useful to tell when the profile has changed.
+
+        :return: A hash of the current values of the profile.
+        """
+        return hash(str(self.bundle_config()))
+
     def write(self, path: Path) -> bool:
         """
         Write the profile to a file.
 
         :param path: The path to write the profile to.
         :return: True if the profile was written successfully, False otherwise.
         """
@@ -475,24 +575,25 @@
             return False
 
     @classmethod
     def load(cls, path: Path) -> "Profile":
         """
         Load a profile from a config file.
         """
-        logger.debug("Loading profile from disk...")
+        logger.debug(f"Loading profile {path} from disk...")
         config = cu.ConfigUpdater()
         try:
             config.read(path)
             profile = cls()
             profile.general.import_from_conf(config)
             profile.text_detector.import_from_conf(config)
             profile.pre_processor.import_from_conf(config)
             profile.masker.import_from_conf(config)
             profile.denoiser.import_from_conf(config)
+            profile.fix()
         except Exception as e:
             logger.error(f"Failed to load profile from {path}:\n{e}")
             profile = cls()
             print("Failed to load profile, using default profile.")
         return profile
 
     def get(self, section: str, option: str) -> Any:
@@ -508,26 +609,36 @@
         # Check that the attribute exists.
         if not hasattr(self, section):
             raise AttributeError(f"No such section: {section}")
         if not hasattr(getattr(self, section), option):
             raise AttributeError(f"No such option: {option}")
         setattr(getattr(self, section), option, value)
 
+    def fix(self):
+        """
+        Correct any invalid values in the profile.
+        """
+        self.general.fix()
+        self.text_detector.fix()
+        self.pre_processor.fix()
+        self.masker.fix()
+        self.denoiser.fix()
+
 
 @dataclass
 class Config:
     """
     The main configuration class.
     These setting are saved to disk.
 
     saved_profiles: Saved profiles contains a mapping from profile name to profile path, where it is saved.
     profile_editor: The program to use to edit the profile files. When blank, the default editor is used.
     """
 
-    current_profile: Profile = Profile()
+    current_profile: Profile = field(default_factory=Profile)
     default_profile: str | None = None
     saved_profiles: dict[str, Path] = field(default_factory=dict)
     profile_editor: str | None = None
     cache_dir: Path | None = None
     default_torch_model_path: Path | None = None  # CUDA
     default_cv2_model_path: Path | None = None  # CPU
 
@@ -710,24 +821,23 @@
         First search if the profile is saved, otherwise treat it like a path.
         For None, attempt to load the default profile.
 
         Special case: Reserve the name "builtin" and "none" (case insensitive) to load the built-in default profile.
 
         :param profile_name: Name or path of the profile to load.
         """
+        logger.debug(f"Loading profile {profile_name!r}...")
         # If no override is given, use the default profile.
         if profile_name is None:
             profile_name = self.default_profile
 
         # If the default profile is not set, use the builtin default profile.
-        if profile_name is None:
-            return
-
-        # Check the reserved names.
-        if profile_name.lower() in RESERVED_PROFILE_NAMES:
+        if profile_name is None or profile_name.lower() in RESERVED_PROFILE_NAMES:
+            logger.debug("Loading builtin default profile")
+            self.current_profile = Profile()
             return
 
         found_profile = cli.closest_match(profile_name, list(self.saved_profiles.keys()))
         if found_profile is not None:
             profile_path = self.saved_profiles[found_profile]
             logger.debug(f"Loading profile {found_profile} from {profile_path}")
         else:
```

### Comparing `pcleaner-1.6.2/pcleaner/ctd_interface.py` & `pcleaner-1.6.9/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-1.6.9/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-1.6.9/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/denoiser.py` & `pcleaner-1.6.9/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-1.6.9/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 # noinspection PyPep8Naming
 class ColorButton(Qw.QPushButton):
 
     colorChanged = Qc.Signal(Qg.QColor)
 
     def __init__(
         self,
+        parent=None,
         color: tuple[int, int, int, int] | tuple[int, int, int] = (255, 255, 255, 255),
         dialog_title: str = "Change Color",
     ):
-        super().__init__()
+        super().__init__(parent)
         self._color: Qg.QColor = Qg.QColor(*color)
         self.use_alpha = len(color) == 4
         self.dialog_title = dialog_title
         self.setFixedHeight(32)
         self.clicked.connect(self._open_color_dialog)
 
     def paintEvent(self, event: Qg.QPaintEvent) -> None:
```

### Comparing `pcleaner-1.6.2/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-1.6.9/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-1.6.9/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/gui/file_table.py` & `pcleaner-1.6.9/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/gui/launcher.py` & `pcleaner-1.6.9/pcleaner/gui/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pcleaner.config as cfg
 import pcleaner.cli_utils as cu
 from pcleaner import __display_name__, __version__
 
 
 # This import is needed to load the icons.
 import pcleaner.gui.rc_generated_files.icons_rc
+import pcleaner.gui.rc_generated_files.theme_icons_rc
 
 
 def launch(input_paths: list[str]) -> None:
     """
     Launch the GUI.
 
     :param input_paths: List of paths to open on startup, may be empty.
```

### Comparing `pcleaner-1.6.2/pcleaner/gui/mainwindow_driver.py` & `pcleaner-1.6.9/pcleaner/gui/mainwindow_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from functools import partial
 from pathlib import Path
 from importlib import resources
 
 import PySide6.QtCore as Qc
 import PySide6.QtGui as Qg
 import PySide6.QtWidgets as Qw
-from PySide6.QtCore import Signal
+from PySide6.QtCore import Signal, Slot
 from logzero import logger
 
 import pcleaner.cli_utils as cu
 import pcleaner.helpers as hp
 import pcleaner.config as cfg
 import pcleaner.gui.profile_parser as pp
+import pcleaner.gui.gui_utils as gu
 from pcleaner.gui.ui_generated_files.ui_Mainwindow import Ui_MainWindow
 from pcleaner.gui.file_table import Column
 from pcleaner import __display_name__, __version__
 from pcleaner import data
+import pcleaner.gui.new_profile_driver as npd
 
 
 # noinspection PyUnresolvedReferences
 class MainWindow(Qw.QMainWindow, Ui_MainWindow):
 
     config: cfg.Config = None
     # glossary: st.Glossary = None
@@ -72,14 +74,15 @@
         self.file_table.setAcceptDrops(True)
         self.file_table.setColumnHidden(Column.ID, True)
         self.file_table.setColumnWidth(Column.FILENAME, 200)
         self.file_table.setColumnWidth(Column.STATUS, 200)
 
         # Connect signals.
         self.connect_combobox_slots()
+        self.comboBox_current_profile.currentIndexChanged.connect(self.change_current_profile)
 
         return
 
         self.checkBox_file_fixed_dir.toggled.connect(self.fixed_output_dir_toggled)
         self.checkBox_use_glossary.toggled.connect(self.use_glossary_toggled)
         self.checkBox_extra_quote_protection.toggled.connect(self.extra_quote_protection_toggled)
         self.pushButton_file_dir_browse.clicked.connect(self.browse_file_out_dir)
@@ -405,21 +408,121 @@
 
         # Load the structure.
         structure = pp.parse_profile_structure(self.config.current_profile)
         self.toolBox_profile.load_profile_structure(structure)
 
         self.load_current_profile()
 
+        # Connect signals.
+        self.toolBox_profile.values_changed.connect(self.handle_profile_values_changed)
+        self.pushButton_reset_profile.clicked.connect(self.reset_profile)
+        self.pushButton_save_profile.clicked.connect(self.save_profile)
+
     def load_current_profile(self):
         """
         Load the current profile.
         """
         logger.debug("Loading current profile.")
         self.toolBox_profile.set_profile_values(self.config.current_profile)
 
+    def change_current_profile(self):
+        """
+        Set the config option to match the current profile selector, then load it.
+        """
+        profile_name = self.comboBox_current_profile.currentText()
+        self.config.load_profile(profile_name)
+        self.load_current_profile()
+
+    @Slot(bool)
+    def handle_profile_values_changed(self, all_default: bool):
+        """
+        Handle the profile values changing.
+
+        :param all_default: Whether all values are default now.
+        """
+        self.pushButton_save_profile.setEnabled(not all_default)
+        self.pushButton_reset_profile.setEnabled(not all_default)
+        self.pushButton_apply_profile.setEnabled(not all_default)
+
+    def reset_profile(self):
+        """
+        Reset the current profile.
+        """
+        self.toolBox_profile.reset_all()
+        self.handle_profile_values_changed(True)
+
+    def save_profile(self, save_as: bool = False):
+        """
+        Save the current profile.
+
+        :param save_as: Whether to save as a new profile.
+        """
+        # Grab the path from the combobox's linked data. If it is none, this is the
+        # default profile, so we need to save it as a new profile.
+        profile_path = self.comboBox_current_profile.currentLinkedData()
+        profile_name = self.comboBox_current_profile.currentText()
+        if profile_path is None:
+            save_as = True
+
+        if profile_path is None:
+            # Trying to save over the default profile.
+            profile_path, profile_name = self.get_new_profile_path(show_protection_hint=True)
+        elif save_as:
+            profile_path, profile_name = self.get_new_profile_path()
+
+        # If the path is still none, the dialog was canceled.
+        if profile_path is None:
+            logger.info("User canceled profile save.")
+            return
+
+        # Proceed to write the profile.
+        logger.info(f"Saving profile to {profile_path}")
+        self.toolBox_profile.get_profile_values(self.config.current_profile)
+        success = self.config.current_profile.write(profile_path)
+        if not success:
+            logger.error("Failed to save profile.")
+            self.statusbar.showMessage(f"Failed to save profile to {profile_path}")
+            gu.show_critical(self, "Save Error", "Failed to save profile.")
+            return
+
+        logger.info("Profile saved successfully.")
+        self.statusbar.showMessage(f"Profile saved to {profile_path}")
+        if save_as:
+            self.config.add_profile(profile_name, profile_path)
+            if not self.config.save():
+                logger.error("Failed to save config.")
+                self.statusbar.showMessage("Failed to save config.")
+                gu.show_critical(
+                    self,
+                    "Save Error",
+                    "Failed to save the new profile to the configuration file.",
+                )
+                return
+            # Add the new profile to the combobox.
+            self.comboBox_current_profile.addTextItemLinkedData(profile_name, profile_path)
+            self.comboBox_current_profile.setCurrentText(profile_name)
+        self.config.load_profile(profile_name)
+        self.load_current_profile()
+
+    def get_new_profile_path(self, show_protection_hint: bool = False) -> tuple[Path, str] | None:
+        """
+        Open a save dialog to save the current profile.
+
+        :param show_protection_hint: Whether to show a hint about protecting the default profile.
+        """
+        default_path = cu.get_default_profile_path()
+        new_profile_dialog = npd.NewProfileDialog(
+            default_path, show_protection_hint, cfg.RESERVED_PROFILE_NAMES
+        )
+        response = new_profile_dialog.exec()
+        if response == Qw.QDialog.Accepted:
+            return new_profile_dialog.get_save_path(), new_profile_dialog.get_name()
+
+        return None
+
     """
     Glossary
     """
 
     def load_glossary(self):
         """
         Open a glossary file and parse it.
```

### Comparing `pcleaner-1.6.2/pcleaner/gui/profile_parser.py` & `pcleaner-1.6.9/pcleaner/gui/profile_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 
 import configupdater as cu
 from logzero import logger
 import PySide6.QtWidgets as qw
 import PySide6.QtGui as qg
 import PySide6.QtCore as qc
+from PySide6.QtCore import Slot
 
 from pcleaner import config as cfg
 from pcleaner.config import GreaterZero
 from pcleaner.gui.CustomQ.CColorButton import ColorButton
 from pcleaner.gui.CustomQ.CComboBox import CComboBox
 
 
@@ -191,25 +192,23 @@
 
     def get_value(self) -> tuple[EntryTypes, Any]:
         """
         Get the value of the data widget.
 
         :return: The entry type and the value.
         """
+        logger.debug(f"Getting value of {self._entry_type}.{self._data_getter()}")
         return self._entry_type, self._data_getter()
 
     def _value_changed(self):
         """
         Called when the value of the data widget changes.
         """
-        if self.value_is_default():
-            self.set_reset_button_enabled(False)
-        else:
-            self.set_reset_button_enabled(True)
-            self.valueChanged.emit()
+        self.set_reset_button_enabled(not self.value_is_default())
+        self.valueChanged.emit()
 
     def set_reset_button_enabled(self, enabled: bool):
         self._reset_button.setEnabled(enabled)
         self._reset_button.setFlat(not enabled)
 
 
 def parse_profile_structure(profile: cfg.Profile) -> list[ProfileSection]:
@@ -294,14 +293,19 @@
 
 
 class ProfileToolBox(qw.QToolBox):
 
     # A subclass that tracks the mapping of widgets to profile options.
     # This is used to save/load the values of the widgets to the profile.
 
+    values_changed = qc.Signal(bool)  # When False, all values are default.
+    values_initialized: bool = (
+        False  # This prevents lookups to the default values before they are set.
+    )
+
     def __init__(self, parent=None):
         qw.QToolBox.__init__(self, parent)
         self._widgets: dict[str, dict[str, ProfileOptionWidget]] = {}
 
     def load_profile_structure(self, structure: list[ProfileSection]) -> None:
         """
         Populate the toolbox widget with the given profile structure.
@@ -316,59 +320,85 @@
             section_widget.setLayout(layout)
             self.addItem(section_widget, to_display_name(section.name))
             self._widgets[section.name] = {}
 
             for item in section.items:
                 if isinstance(item, ProfileComment):
                     item: ProfileComment
-                    label = qw.QLabel(item.comment)
+                    label = qw.QLabel(parent=self, text=item.comment)
                     label.setOpenExternalLinks(True)
                     label.setWordWrap(True)
                     layout.addRow(label)
 
                 elif isinstance(item, ProfileSpace):
-                    layout.addRow(qw.QLabel(""))
+                    layout.addRow(qw.QLabel(parent=self, text=""))
 
                 elif isinstance(item, ProfileEntry):
                     item: ProfileEntry
-                    label = qw.QLabel(to_display_name(item.key))
+                    label = qw.QLabel(parent=self, text=to_display_name(item.key))
                     label.setToolTip(to_display_name(item.key))
                     layout.addRow(label)
                     option_widget = ProfileOptionWidget(item.entry_type)
                     layout.addRow(label, option_widget)
+                    option_widget.valueChanged.connect(self._on_value_changed)
 
                     self._widgets[section.name][item.key] = option_widget
 
     def set_profile_values(self, profile: cfg.Profile) -> None:
         """
         Load the values from the given profile into the widgets.
 
         :param profile: The profile to load.
         """
+        logger.debug("Setting profile values")
         # Assign the value and connect the reset functionality for each widget.
         for section_name, section in self._widgets.items():
             for key, option_widget in section.items():
                 # Get the value from the profile.
                 value = profile.get(section_name, key)
                 option_widget.set_value(value)
 
+        self.values_initialized = True
+
     def get_profile_values(self, profile: cfg.Profile) -> None:
         """
         Save the values from the widgets to the given profile.
         Update in place.
 
         :param profile: The profile to save to.
         """
+        logger.debug("Getting profile values")
         # Assign the value and connect the reset functionality for each widget.
         for section_name, section in self._widgets.items():
             for key, option_widget in section.items():
                 # Get the value from the widget.
                 value = option_widget.get_value()
                 profile.set(section_name, key, value)
 
+    @Slot()
+    def _on_value_changed(self) -> None:
+        """
+        Check if all values are default, then re-emit the signal.
+        """
+        if not self.values_initialized:
+            return
+
+        all_values_default = all(
+            w.value_is_default() for section in self._widgets.values() for w in section.values()
+        )
+        self.values_changed.emit(all_values_default)
+
+    def reset_all(self) -> None:
+        """
+        Reset all widgets to their default values.
+        """
+        for section in self._widgets.values():
+            for widget in section.values():
+                widget.reset()
+
 
 def to_snake_case(name: str) -> str:
     """
     Convert the given name to snake case.
 
     :param name: The name to convert.
     :return: The converted name.
```

### Comparing `pcleaner-1.6.2/pcleaner/gui/rc_generated_files/icons_rc.py` & `pcleaner-1.6.9/pcleaner/gui/rc_generated_files/theme_icons_rc.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,571 +2,262 @@
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 6.4.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
-\x00\x00\x14d\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00@\x00\x00\x00@\x08\x06\x00\x00\x00\xaaiq\xde\
-\x00\x00\x00\xf2zTXtRaw prof\
-ile type exif\x00\x00x\
-\xdamQ\xdb\x8d\xc4 \x0c\xfc\xa7\x8a+\x01?\xb0\xa1\
-\x1c\x16\x88\xb4\x1d\x5c\xf9g\xc0\xc9%\xab\x1d\x09\xdb\xe3\
-\xb1\x06\xe2\x84\xf1\xfb>\xc2\xcf\x04J\x0e\x9c4K\x11\
-\x89\x06.\x5c\xb0Z\x91\xe3F[\x11\x22\xaf\xb8\xc0.\
-\x19\x7f\xf4\xc3%\xa0\xb5\xc82mZ\x86\xcf\x9f}\xb8\
-\x0cv\xaaV\xa5\x9bQu'x=\x85\xda\xdc?\x7f\
-\x18\xf9E4_\x84Vt7z\xb9\x11\xe1\x16\xc0y\
-\xc3\x9d\xa5d\xbd\x7f\xc2\xe1\xba\xb6\x82\xcbH\xdd\xa8\xcb\
-.lQK\x00\xe7}\xc4'\xf2\xff!]\x16\xd7\xa5\
-\x93\x87{\x83\xd5\xd6\xdd\x93M\x11\xe2 \xa0h\x91\x88\
-\xf7\x8bi\x1e\xa2j\x99-\x02\xa9\xcd\xc5\xd5a\x8a\xc1\
-\x12Q1\x93C\xa3$\x19\x0c\x5c\x96i\x17\x10\x96\x84\
-QU\x8a\xb2d|\xcc\x18k6\x81\xea\xfb\x0bs\xfd\
-\xdf\xfe\xca\x89\xf0\x07-\xcfp\xc0\xb9\xafy\xed\x00\x00\
-\x01\x85iCCPICC profil\
-e\x00\x00x\x9c}\x91;H\xc3P\x14\x86\xff>\xa4\
-\x22\x15\x11;\xa8(d\xa8NvQ\x11\xc7Z\x85\x22\
-T\x08\xb5B\xab\x0e&7}A\x93\x86$\xc5\xc5Q\
-p-8\xf8X\xac:\xb88\xeb\xea\xe0*\x08\x82\x0f\
-\x10W\x17'E\x17)\xf1\xdc\xa4\xd0\x22\xc6\x03\x97\xfb\
-\xf1\xdf\xf3\xff\xdc{.\xe0oT\x98j\x06\xe3\x80\xaa\
-YF:\x99\x10\xb2\xb9U!\xf4\x8a \xfa\xe1\xc3(\
-\x86$f\xeas\xa2\x98\x82g}\xddS'\xd5]\x8c\
-gy\xf7\xfdY\xbdJ\xded\x80O \x8e3\xdd\xb0\
-\x887\x88g6-\x9d\xf3>q\x84\x95$\x85\xf8\x9c\
-x\xc2\xa0\x0b\x12?r]v\xf9\x8ds\xd1a?\xcf\
-\x8c\x18\x99\xf4<q\x84X(v\xb0\xdc\xc1\xacd\xa8\
-\xc4\xd3\xc4QE\xd5(\xdf\x9fuY\xe1\xbc\xc5Y\xad\
-\xd4X\xeb\x9e\xfc\x85\xe1\xbc\xb6\xb2\xccuZ#Hb\
-\x11K\x10!@F\x0deT`!F\xbbF\x8a\x89\
-4\x9d'<\xfc\xc3\x8e_$\x97L\xae2\x189\x16\
-P\x85\x0a\xc9\xf1\x83\xff\xc1\xef\xd9\x9a\x85\xa9I7)\
-\x9c\x00\xba^l\xfbc\x0c\x08\xed\x02\xcd\xbam\x7f\x1f\
-\xdbv\xf3\x04\x08<\x03WZ\xdb_m\x00\xb3\x9f\xa4\
-\xd7\xdbZ\xf4\x08\xe8\xdb\x06.\xae\xdb\x9a\xbc\x07\x5c\xee\
-\x00\x83O\xbadH\x8e\x14\xa0\xe5/\x14\x80\xf73\xfa\
-\xa6\x1c0p\x0b\xf4\xac\xb9sk\x9d\xe3\xf4\x01\xc8\xd0\
-\xacR7\xc0\xc1!0^\xa4\xecu\x8fwww\xce\
-\xed\xdf\x9e\xd6\xfc~\x00Y\x04r\x9c\x16\x14.U\x00\
-\x00\x0e[iTXtXML:com.a\
-dobe.xmp\x00\x00\x00\x00\x00<?x\
-packet begin=\x22\xef\xbb\
-\xbf\x22 id=\x22W5M0MpCeh\
-iHzreSzNTczkc9d\x22\
-?>\x0a<x:xmpmeta xm\
-lns:x=\x22adobe:ns:\
-meta/\x22 x:xmptk=\x22\
-XMP Core 4.4.0-E\
-xiv2\x22>\x0a <rdf:RDF\
- xmlns:rdf=\x22http\
-://www.w3.org/19\
-99/02/22-rdf-syn\
-tax-ns#\x22>\x0a  <rdf\
-:Description rdf\
-:about=\x22\x22\x0a    xm\
-lns:xmpMM=\x22http:\
-//ns.adobe.com/x\
-ap/1.0/mm/\x22\x0a    \
-xmlns:stEvt=\x22htt\
-p://ns.adobe.com\
-/xap/1.0/sType/R\
-esourceEvent#\x22\x0a \
-   xmlns:dc=\x22htt\
-p://purl.org/dc/\
-elements/1.1/\x22\x0a \
-   xmlns:GIMP=\x22h\
-ttp://www.gimp.o\
-rg/xmp/\x22\x0a    xml\
-ns:tiff=\x22http://\
-ns.adobe.com/tif\
-f/1.0/\x22\x0a    xmln\
-s:xmp=\x22http://ns\
-.adobe.com/xap/1\
-.0/\x22\x0a   xmpMM:Do\
-cumentID=\x22gimp:d\
-ocid:gimp:fe8a36\
-45-afe3-4c9c-815\
-1-f1f729fe96e7\x22\x0a\
-   xmpMM:Instanc\
-eID=\x22xmp.iid:b71\
-457bb-1de1-4d7c-\
-adce-34e9c9c7f1f\
-a\x22\x0a   xmpMM:Orig\
-inalDocumentID=\x22\
-xmp.did:6ae848d5\
--1f55-484f-b572-\
-b6b18da2f71b\x22\x0a  \
- dc:Format=\x22imag\
-e/png\x22\x0a   GIMP:A\
-PI=\x222.0\x22\x0a   GIMP\
-:Platform=\x22Linux\
-\x22\x0a   GIMP:TimeSt\
-amp=\x2216816956413\
-45459\x22\x0a   GIMP:V\
-ersion=\x222.10.34\x22\
-\x0a   tiff:Orienta\
-tion=\x221\x22\x0a   xmp:\
-CreatorTool=\x22GIM\
-P 2.10\x22\x0a   xmp:M\
-etadataDate=\x22202\
-3:04:17T03:40:39\
-+02:00\x22\x0a   xmp:M\
-odifyDate=\x222023:\
-04:17T03:40:39+0\
-2:00\x22>\x0a   <xmpMM\
-:History>\x0a    <r\
-df:Seq>\x0a     <rd\
-f:li\x0a      stEvt\
-:action=\x22saved\x22\x0a\
-      stEvt:chan\
-ged=\x22/\x22\x0a      st\
-Evt:instanceID=\x22\
-xmp.iid:1594000b\
--7cdb-4be6-ab05-\
-48e01841b2cf\x22\x0a  \
-    stEvt:softwa\
-reAgent=\x22Gimp 2.\
-10 (Linux)\x22\x0a    \
-  stEvt:when=\x2220\
-23-04-15T06:16:3\
-9+02:00\x22/>\x0a     \
-<rdf:li\x0a      st\
-Evt:action=\x22save\
-d\x22\x0a      stEvt:c\
-hanged=\x22/\x22\x0a     \
- stEvt:instanceI\
-D=\x22xmp.iid:375ad\
-661-b1fb-4c5e-b2\
-6c-44f36217cb01\x22\
-\x0a      stEvt:sof\
-twareAgent=\x22Gimp\
- 2.10 (Linux)\x22\x0a \
-     stEvt:when=\
-\x222023-04-17T03:4\
-0:41+02:00\x22/>\x0a  \
-  </rdf:Seq>\x0a   \
-</xmpMM:History>\
-\x0a  </rdf:Descrip\
-tion>\x0a </rdf:RDF\
->\x0a</x:xmpmeta>\x0a \
-                \
-                \
-                \
-                \
-                \
-                \
-   \x0a            \
-                \
-                \
-                \
-                \
-                \
-        \x0a       \
-                \
-                \
-                \
-                \
-                \
-             \x0a  \
-                \
-                \
-                \
-                \
-                \
-                \
-  \x0a             \
-                \
-                \
-                \
-                \
-                \
-       \x0a        \
-                \
-                \
-                \
-                \
-                \
-            \x0a   \
-                \
-                \
-                \
-                \
-                \
-                \
- \x0a              \
-                \
-                \
-                \
-                \
-                \
-      \x0a         \
-                \
-                \
-                \
-                \
-                \
-           \x0a    \
-                \
-                \
-                \
-                \
-                \
-                \
-\x0a               \
-                \
-                \
-                \
-                \
-                \
-     \x0a          \
-                \
-                \
-                \
-                \
-                \
-          \x0a     \
-                \
-                \
-                \
-                \
-                \
-               \x0a\
-                \
-                \
-                \
-                \
-                \
-                \
-    \x0a           \
-                \
-                \
-                \
-                \
-                \
-         \x0a      \
-                \
-                \
-                \
-                \
-                \
-              \x0a \
-                \
-                \
-                \
-                \
-                \
-                \
-   \x0a            \
-                \
-                \
-                \
-                \
-                \
-        \x0a       \
-                \
-                \
-                \
-                \
-                \
-             \x0a  \
-                \
-                \
-                \
-                \
-                \
-                \
-  \x0a             \
-              \x0a<\
-?xpacket end=\x22w\x22\
-?>\xd5\xcd\xbcE\x00\x00\x00\x06bKGD\x00\xff\
-\x00\xff\x00\xff\xa0\xbd\xa7\x93\x00\x00\x00\x09pHYs\
-\x00\x00\x0b\x13\x00\x00\x0b\x13\x01\x00\x9a\x9c\x18\x00\x00\x00\
-\x07tIME\x07\xe7\x04\x11\x01()\xc4\x9dKQ\
-\x00\x00\x02\xfbIDATx\xda\xe5[\xcbq\xdc0\
-\x0c}\xe4\xe8\x90CzI\x07>m\x03q\x19nA\
-G\x8fZ\xd82\x9c\x02\xec&\xdc\x8bg\xb27\xe4\xb0\
-bF\xc3P\x14A\x00\x14\x99\xc5\x8cO\xa6\xb8|\xc0\
-\xc3W\xa2\xc3*D\xf4\x1d\xc0\x0b\x80g\x00?\x00|\
-C$\xce\xb9\xb0\x16\x1a\xa2\xbd\xdf\x81\xdc\x00|\x02x\
-\x03pu\xce}a\x03\xfe\x89\x88\xde\xe9@\x00\xfc\xfd\
-\xd3\x10\xcd\xbd\x98\xf2NDO\x00\xe0V\xcb\xff\x02p\
-)\xb5\x98\x96\xd5\x1a3 \x96\x0f\x00?\xfdJ\xfb\x0b\
-\x1eO.\x00^\xfc\xea\xf3\x8f*\xcf\x8e\x88~\xa7\x02\
-^\x0b\xda\x9e\xec\x02\x00ps\xc4\xfcu\x0b\x05\x9c\xa9\
-\x04\x8f\x07\x97n\x14\xb0e\xc3\xc32\xc09\xd7\x5c\x11\
-\x93\xe4\xb0{~\x1b\x83\x08\xeb:\x08z\xff\x9e\x95*\
-N\x93\x03\xa2e\xc1VJ\x9aF\xf7\xe1S\x14@D\
-\xa7\xf8k\xd7\x0c\xe0\xd2\xba\x17\xe5y\x0d\xba\xe7\xfc5\
-\xfc/^\xb3\xf7L\x1c0\x87H\x83{\x19a\x0f\xfc\
-\x99AO\xac\x80\x9ce\xb8 b\x97\x88\x9fo\xc1\x02\
-\xafE\xfdTj,\x01\x90cN\xf7.\x10[\xad\xb6\
-\xd0\xc9\xad\xb7f\x81\xb7\xa2>7\x98\x95\x06\xc9\xee\x82\
-`l\xf5T\x8b+\xb5\xa2%\x0bT\x9b!m\x7fn\
-\xc1\x02\xaf\xed\xa7\xa1J\xd4\x06b\xc5\x02/\xb1\xc8Q\
-13B\xf5\xe8\xb5\x0ehe!\xeb, j\x87\xad\
-\xfc\xf4\x08\xb4\xe6o\xfa\x9eh\xb9\xd7a.\xcb\x82e\
-YL~s\x92P?\x1c$7\x1d\x92X|\x0b\xba\
-\xcbv8\x15\xf1\xa5\xc0S\xa0\xe7y.n\xc0\x9a\xcf\
-\x03\xb6\xc3\x91\xd2\x03\x95\x00O\x81\xee&\x08\x96T\x84\
-%\xc0K\xad\x1d\xaf\xdd\xae\x91\x1e_M\x01\x9c\x8e\xb0\
-\x16xj\xbd\xf4\xf8\xaa#\xb1\xd8\x1dj-\xce\x09~\
-\xe2\x00L\xca\x89\xbc4\xa2K\x81k\xb9\x82\xfaP\xf4\
-(3h\x00\xef2\x08r\xcbW-\xd0R\x16\x98\xbe\
-\x1b\x8c+8\x0b\x8bK\xf72}/\xd0\x9a\xee5\x01\
-\xd1\x84\x01\xadG\xdc\x92>\xa1\xf9\xebq\x8b\x0aO\xb2\
-\xe7\xd4\xd2B\x9a\xe0s{q\x5c\xc1\x8c\x01\xb9\x03H\
-\x141\xcf\xb3jl\x99Z\xd1>d\x84\x1a\xf0\xdc2\
-\x99\x13\x83L\x15\x90+\x8a\x82R\xb4\x80\xd7\xb2\xaaY\
-\x10\x0c\x07,\xa1j\x8e\xe6G\xcfs3\x90\xb9\x0bp\
-XP\xeb\xdb\x92\x98bR\x0a\xe7J\xe3\xd2\x8c\xc0\x09\
-j\x92\xd6\xb8I\x10\xe4\x8c\xce$\x1da\xb7\x0c8b\
-\x81\xa4<\x96\x0eF\x9a}#\x14\xb3\x80k\xb9x\xfd\
-6\xa5v5\x10\xe1\xb6\xc9\xa5\xd6\xcf)L\x02\xa1\xf9\
-Wb\xb5ct\xab\xa1\xe8\x90_\x8bk\xb6\xd4M]\
-\x80\xdb\xb2\x96V\x8a\xc3\xc4\x80\x1a%\xe4\x14\xa2\xe1\x0a\
-\xa7)\xa0VA{J\xf8\xef\x14PRGh(\xc1\
-\xe3~\xa3\xb2{)\x01W\xe1V7\x8f\xfbu\xd2\xa1\
-$U\x14U\xca\xa7\xc7\xfd.-FgAP\x02\x93\
-\x05o\x1e\xc0\x15\xf7k\xa4C\xb3\xa0\xc2\x15>\x00\x5c\
-\xfdz\x8b\xfau\x14%\x94\xb0\xa0\x10\xfc\xabs\xee\xcb\
-m6>\xbc>?BF\xc8d\x85\xe4\xf5\xf9?\xd5\
-V\xf3\x8co\xe8\xd3\xc6\x00\x00\x00\x00IEND\xae\
-B`\x82\
-\x00\x00\x0d2\
+\x00\x00\x0e\x80\
 \x00\
-\x00I\x9ax\xda\xdd[\xdfo\x1c\xc5\x1d\x7f\xbf\xbfb\
-\x10/\xb6z\xb1\xe5\xdd\xcb\xc9\x89zU\x9c\xd8q\xdd\
-\xc4v\x84\x0d(\x8a,k|7w\xde\xdc\xde\xeei\
-w\xce\xd9\xf3SH M\xf9QA\x15T\xa0\x06\x1a\
-p\x8aJ\x91\x09T\x81 \xc0<\x84>\xf0\x02\xe6\xcd\
-y\xbb\x14\x10\x09\xb8\xea\xbf\xd0\x99\xdd\x9d\x99\xfd1\xbb\
-\xb7\xb6\xcf\x8eK$\xe7\xe6;\xdf\x99\xef|\xbe3\xdf\
-\xf9~\xbf\xb3\xb3{n\xa2l\x1a`v\x115\xd0\x5c\
-n\x0a6P\xe9\xb8\x85\xd02r\xcb\xe7\xa05W\xba\
-{e\xf3\x9fw\x9f\xbd\xfb\x8c_c\xe3\xb9p\x93\xe5\
-0\xbdP\x0b\xd3eHi\xcd\x86\x8c<\xb6\x04ud\
-\x94\xb5H\xbd\x1d\xeeV\x81\x11\x1a\x85i\xa4Ghc\
-~\xfcx\xa4\xca\x0e\x8d\x80\x22\xc0Q+LW\xb5\x08\
-m\x85\xe9Ze\xae4\xada\x04k>\x1dA\xb0H\
-\xfawV\xdf\xeb\xdcx\xa1\xb3z\xb3s\xe3bgu\
-\xa5\xb3\xfa\x99\xcf\x8b\x8c\xa5E\xb4\xd3*\x11\xda\xc3\xba\
-\xbc\xecc?\x1fi_\x8f\xd2f\x98\xd6#\xba\x1a\x11\
-\xac\x86\x11\xa6\x9b.\xbf\xcd\x86k\xe2\xd0\xcc5\xf1\xfc\
-\xf1\xc7\xc2\x1d,w@m\xf9\xcb\xcb>\x1dQ\xd0\xae\
-\xcf\x95\x9e\xb8s\xdd0\xeb>M\x06\x98\x81M\xad\x0c\
-A\x9f\xd7\xae\xdfg\x90Y\xdexsc}\xe3\xc3\x8d\
-[\xdf^\xda\xb8\xf9\xedE\xf2w\x85\xf1\x8ei\xe7Q\
-\x1d.i\xd0\xc8\xd6J\x87X#M\xcf\x98K\x08C\
-\x0b\x96y\x8b\x04\xc6R\x185&\xd3\xdaY{\xb7\xb3\
-\xf6Eg\xedf\xe7\xfd\x8b\x9d\xb5\xdb\x9d\xf7_\xf0y\
-\xc4\xae7^'\xc3>\xb5q{\xc3_VL\xc0\x8f\
-\xd9\x9a\x815\x8fn\xd5\xc3\xf2\x96\x22&\xe5\x1c\xc2\x88\
-\xee\x1f\xc7\xf1j\x1d\xc7\xab_^\x9c?1\xc5\x9a\x82\
-\x1f\xd6\xd7\x1e\xbc\xfdG\xce\x99}\x92\x0b\xc9\x9d0\x1b\
-\x0dd`\xd6r\xa1\x0d\xf0\x22\x02\xa7F\xc7\xc0\x13\xa3\
-\xe3\x8c\x1b\xda\xb5\xe0\xee3w\xaf\x90\xff6\xdf#\x85\
-\xab\x9b\x9fl\xfe\x1dl\xbe\xbby\x8b\x10.\xf3\xf2\xe6\
-\xfbw\x9f\x15\x1d\xc5\xe6\x06MS\xa7BA\xc5\x95/\
-\x9a\xf0\xed\xce\x86\x05\xf8\xabW\xad\xaf^\xadjF\xe5\
-\xabW\x0d\xdeP\xf8\x01\xb0\xb1\xfe\xed\xa5\x18H\xee\x17\
-\xf2\xa0l!\x88A\x13\xb1\x01\xf5\xd0\x88q\x8f\x11\xef\
-\x11\xee\xc0]\x090+\xb1q\x85c\x01\xb0\x1a\xe7r\
-7\x03\x96\x88_\xac +\xd6Dx\x1e\xf0\xf5\x07\xdf\
-\x5c\xfc\xe6y\xf0\xcd\xd3_\x7f\x11o\x16tHI+\
-\xc5]\x14\x99n\xc9H8:\xd7\x87t,\xb8|\xcb\
-\xe5\x19\xbb\x0ePM3 o\x22\x5c\x1akqT\xc7\
-wV\x05\xdf\x12\x22\x9a0\x0e@\xb88\x7f\x8eC\x5c\
-\xcf\xe1\xbd\xdc\xb9\xf1\xfb\xce\xeau\xd7\xe1]\x05\x9d\xd5\
-[n\xe9\xba\xef\x00o\x5c$U\x7fs}\xe2\xad\xce\
-\xea:\xf5\x8c\xab\xeb@\xe2&\xb9\xd0\x96X\x1e\xae5\
-\xfe\xd7K:o!|'u%d\xee\xfa\x89!X\
-@\x8f\x03\x14^\x15\x98:Z\x8c\xf3\xb9\x97eF\x17\
-bS\xa7\xcbl\xfc\xbb\xa7\xfe\xf1\xdd\xa5\xab\xdf]z\
-\x0e\xf8[\x915\x12\x9e\x98\xa3\xbdw\xf9\xfa\xbd\xcb\x7f\
-\xbaw\xf9\xc5{\x97WD;\xd3\x13\xb6\xf5\xdc\xcaO\
-7\x9f\x02?_\xbb\xb6\xf5\xc6\x8b[\xaf\xdf\x06?}\
-|\xfb\xe7\xb7?\xd9\xfa\xf3\x8b[O\xaf\x80\xad\xbf\xae\
-l\xbd\xf1\xd2\x7f^^\x89\x0e\xa3\x076&\xac\xc18\
-X#\xb0T&\xb1%\xc9z\x09\xa7\x0f\xaa\xd6\x9d\x1b\
-1>\x0f\x02\x00\xb6\xb0i\xd9\xf8\x02\x8c\xb7a\x91\x01\
-T\xa0\xb7\xf7\xcc\xd0\xde\x0b\x85\x0a\xbaA\xcd\x98\x08\x11\
-:\xf22\x94\x22\x92\xc8\xfd\x86\x88,\xb2\xddm\xebi\
-{_\xf8{\x00\x97(\xf7\xa8\x0d\x964\xbb\x85t\x9d\
-\x9a\x80\xad\xd5\x8c\x9a\xd5j6y\x87\xb0\xd3\x07\x1b7\
-7>\x8e\x09\xa5A\x80\xd6\x8d\xdf\xf9\xc8\xb2\x89\x19\xcd\
-B\x1bZ_~\xd0\x00\xe3Vk\xa1eT\xa0\x01\xfc\
-\x18\xc1z\x880\x91\xa7\x22?$\x11m\x9dD\xb4\xdb\
-\xe0\xdf\x17\xaf\xc5\xc4\x8b\x18\x92\xf7';\xc4\x8e\x86\x94\
-\x88\xa7!\x11\x86\xb5\x94\x05\x99\xefo\x7f\xfa\xe0\xadW\
-\xfe\xfb\xd9\xf3?^\xfb\x80\xfb\xf3\xbe\xfb\xef\x5c\xb9\xff\
-\xce\x1f\xee\xaf\xad\xdf_\xbb\xfe\xc3_\xdez\xf0\xca\x9b\
-\xfd\xc0\xa7\xae~\xf4\xfd\xe7+A\x914:\x05;\xff\
-\xb0\xf2\xca\x83\xd7\x9e\xbd\xff\xf6\xe7\xa4\xdd\x8f\xaf=\xcd\
-\xec87\xaa\xd9M\x1d\xb6GQ\x13/\x96T%\x97\
-\x9b0\x16\x91\xa5a\xbb\xb4\xa8\x95M\xdd\xb4r\xb91\
-\x076\x9a:*UM\x9d\xf8\xdd\x5c\xee\xa4\xa9\xeb\xe6\
-\x05\xfb\x04\xe5\xce\x94i\x86Z\xc2V\x8b\xcaBv\x1d\
-\x9b\xcdQT\x85-\x1d\x97\x0a\xc3\xacfF[Fv\
-i\xa8\x98W\x94\xbc\xaa\xe4\x0b\xc3\xf9b!?\xa4\x0c\
-\xe7\x95\xc3\xc5\xdc\xaci\xea\x0b\xd0b\xbd\x14\x85\xd5\xc4\
-z\xe5&\xa1f\xc4\x9b\x07j\xe3]f\x1aP\xd7Y\
-\xe3\xa1\xa2G\xc7\x9b\x9d\x81\x06\xd2\x03\xc0]:\x15\xf6\
-\xa8\x06u\xb3\xc6\xba\x90\x99\xf3*R\xfb\xe4\xc8j\x1c\
-\x1as02l\xcd4\xec\xd2\x80\xbdT\xcb\xe5\x1e\xe5\
-\xff\xc0\xa8f\xa12\xd9\xe3\x1a\xb2\x83\xd5\xa6E&\x1e\
-U\xa8\x0d\x95!F5\xd3j\x03hT\x00\xd4\x9b\x8b\
-p\x01a\x92\xbe\xe9z\x9b.&\xef^\x82eL\xc7\
-\x18\x1cR\xf2\xbcX\xe4EE\xd4*\x05^TE-\
-\x01\xce\x8aD\x01hh\x0d(\x84\x08\x8a\xcai6\xbd\
-Z\xfa\xcbh\xd5\xff%b\x9a\x16\xaa\x12\xf4F\x19\xb9\
-\xec \xe9\xb5\xd2\x11f\x02\xdc\xa2\x22j)\x0a\xbfH\
-Q\xb0\xb6\x8a\xa8&\xd3\x9a\xf7\xe7D\xf3$V\xd0\x92\
-F\x85\x13\x89\xac\xa8\x88Z\x22\x065\x16t\xd4\xb0\x07\
-\x87y\x894eE\xd2\x145L\xecujh\x0d\x84\
-\xdbMO\x98 B\x1c5H\x10\xe9d7\xf9\xa3\xfb\
-%\xaa\xb3WRy\x89N\x8bW:\xc2\xdb\x91\xbe6\
-\x86\xb8\xe5\xf6\xf5K\xa4/+q\xae\xca\xeb\x88\x14\xbf\
-T\x14kh\xb7\x1b\x0b\xa6\xae\x95\xb9\xc6\xbc\x82\xa9\xc8\
-+\xfc\x819\xed\x0bctn\x86\x98\x15\xaaH\x8d\xaa\
-xLq\x02vuLu\x02\xa6\x15\xe4\x11*\xc8+\
-\x84x\x85 O\x0d\xf5S\xbd~A\xbbs\xd9\xa1\x0a\
-\xda\xc2\xb3>\x97\xe7\x17Y\xad\x0f\xc4/\x92Za\x19\
-\x94\x11\xa0\x02<\xafS\x80\x22<a&\x94\x17\xa0\x02\
-<\xaf_\x80ry\xbe!y,F\x10N\xd0\xb0(\
-3D\x87\xf8^\xe7\x10M\xf8\xdc\xc8(S\x10\x82\xe3\
-u\x13\x04\xe1p\xe3\xa2\x1cA\x08\x8e\xd7G\x10\xaa\x13\
-\xf2M#\xde\xca$\xf8%[\xa3\xd1\xe4\xd1!\xc5\x19\
-R\xc0!pRsH=\xad\xa4\x04\xc9{&\x8c\xba\
-]\x86M\x94;'\x1c\xd3\x5c\x8ez\xcb\xd2\x90B\x02\
-\x97\x81\x91\x83Kl\x8cY\xa2k\xc9\x95Ae\x16\x9d\
-\xa1\xa2Lf\xcbF@3HM\x05\x11\xdf\xdfg\xf7\
-\x03\x9bzw\x92tb/\x1c\xd0\xaa\xdf<\xf2\xc8#\
-\xd3S\xa7\xcf\x92\x9f_\x1f\x05h\xa06\x00N\x11\x7f\
-\x01\x1a\xe6\x12$\x8b\xc5z\x0f\xfa]@\x9f\x8d\xa0U\
-^t\xfd\xab\x85\xdc\x19$\xe7\x9a\x96E\x5c\x169\xd9\
-X\xe6y\xb2\x19\xf2\x00\xe1\xf2@?\xd1\x1f\xfc\xaeU\
-\x07\x98\xc4R\x92\xaf\xa0\x0b\x04\xd7\xe8\xf4\xfc\xd4\xf4\xec\
-\xfc\xe33c\xf3#Sg\x9f\xfc\xed\xd8cc\xf3c\
-\xa7g\xc6\x08k\xd24\xcc\xf2\xa2e6\x82\x93Pd\
-\x93P\xcc0\x09d}~\xb1\xf3@t\x13S\xe1z\
-\x9eR\x16\xbb V\xfa\xcb\x9d\x1256%j\xfa\x94\
-(\x8a\xa3H\xb7\x1fS\x81\xe4t\x86\x1dR|\xfb\xc0\
-\x14\xb6q\x15%\x03\x9a\x04\x9b\xed- a<\x04S\
-&\xe3\xf1\xb0\xa9\xfb\x81M\x8da\xeb\xb6\x8a\x05G)\
-D\x81\x8d\xcf\x9e\xea\x0d\xa0\x02CS\xc8\x80B\xb2z\
-\xbd\x03\x12X\xb5B\xc6Us1\xa9{\x89I\x8da\
-\xea\xb2Z\xaa\xe2\xa8{\xbe\xe7T\xb6\xe7\xd4\x84\x19\xa2\
-P\xa9\xd3\xcaMj\x06k8\x09\x1dO\x13z\xf4\xf0\
-p\xee\xc3nT\x03\xbbQ\xed\xb2\x1b\xb3\xa2V\xf7\x03\
-\xb5\x1aC\xad\xee\x14ua\xd8)\x0c\xef5\xe4\xc2\xb0\
-\x8f\x97\x9cW\xb3\xe1t\x8f\xd0A\x9c\xc5\x82S,\xec\
-5\xce\x22\xf38\xc5\xc2N\xe73\x90\x85\xf2\x03@\x97\
-DT\x964\x8e\x90C#9+\xd3\xee\xaef4\x09\
-\xa8\x12mGMr\x90\x16\xe9\x02i9}fvb\
-zj\xe44\xf8Ufm\x83'\x13IR'pg\
-\xca\xeb\xf6\x0djz\xde\x95\x8aZ}\x88\xa8SS\xa3\
-\x04\xd4,;\xe2\xf6v.\xf4$C\x92\xd5D\x04\xc5\
-\x0cUI1Tr\xee<h&\xea\x1d\x90%\xc6)\
-\x06=\x08\xe6\xc9\x8f\xf4)\x86\xd9\x05\xb1\xfaP\x10\xa7\
-\x1ae\x22bi\xd2\xfe\xa4i\xd5\xa1e\xb6\xc8Q#\
-\x886pzYha\xec1\xdc\x93\x0b\xd3c\xba\x89\
-\x0c0\x8b\xac\x86f@}pd\xc1la\xc6\xf3)\
-\xfaH\xd8\xebl\xd3\x81\x1e\x9b\x9e\x1a\x9f\x9f81=\
-E\xd4\x1c\x19\x1f\x9b?~v~\xe4\xcc\x19\x99\x86\xd2\
--\x92\xae\x96\xc4t\x0e\xa6f\xe9'\x88.J\xaa\xff\
-/J\xa6\x1eE\x12\x95L\xccpg\xda6F\x0d0\
-\x830\xd6\x8c\x9a-\xcf\x16\x98\xd3$\xca\xbb7 U\
-\xf7\xfa\x80\xb4w%\xd9G\x81'\xbe\xaf\xe2=J\xef\
-\xcf\x037+\xc9\x83!e\xd8\xa1\x8fz\x01q\xad\x0e\
-\xf9K\xcf<\xdc\xeb\x08_Si\xb6\x9c\xa8\x1eK\xd6\
-8PO9\x18q\x18\xdbW\xcc\x13\x1cP\xecH\xd1\
-9Rt\x1f\x1fxG\xbc>\xc3\xc4\xc0Be\xf7\xda\
-\xa6\x82*\xfd\xd9U\x94&\x7f1\x15\xbbg\x80lm\
-#\xca\x1f\xc0\x95\x0d_\x1cdY\xe0\xeeye\xe2\xf3\
-\x92L\xfao\x0f\xf3\xf6\xbc'K\x0e\xa6\x0d\xbdM\x9f\
-fU\x5c\xffQ\x86\x16\xbd3\xca\x03\xbb\xdd\xd05\xa3\
-\xeeW\x9f\x9al\x93\xdd\x8e\xda\xaem\xf8\xd7)\xf1(\
-?\xe3>\xd9\x8d\xf8/\xbe\x00.bW\x9a/C\x08\
-\x93!\x0f\x0a\xeb\x9e\x16e\x1aFf\xd2\xa9\xc3\xa8\xc9\
-\xc3\xf0\xcc\xcd_9:`\x9d\x98&\xbdM\xa67\x92\
-\x00U\xab\xa8\x1c\x1c]vJ\xd9\xe9\xe8b\xa3\xb2\xfb\
-*\xfe\xa8{xw\xf6\xca\x87\x908+2\x14\x18\x04\
-\x17\xb4J\x8d\x96b\x16\x9b\xd5\xb7\xb0k5\xb6\xe6\x87\
-\x8b\xbbr0\x22\x03>\xc1\xaf\xe9\xd2\xf3\xe2\xc4p#\
-\xee\xf9\xe4\xfb\xf1q\xbaM\xc8\x1a\x9f\xd2\xcau\xb3Z\
-\x05}4T\x16\x06\x9c\x01\xa7\xdfu\xba\xa7!\xd9\x88\
-\xba\x89\x07\xc0\x88n\x9b\xde\xae\x22\xcd'Gf\xc7\x5c\
-\xfe\x09\xcd0`\x83\xd8L\xdf\xf9\x96\x8d\xc1\xc9\xb3\x13\
-\xfd\xd9O\xbb\xa1K\xc8\xb8w\x0a(\xbf\xed3\xef\xa8\
-w\x1b\xb5\x83\xd3\x04\x9d5\xf7\xc17\xf0n\xb4vu\
-\x9e\x17\x17fq\xdf\xc2 \x06\x9dK\xfa\xa5\xc5\x1e\xc0\
-J=1\xc8\x10\xa6^!\xec\x05\xc0\xb4\x03\x82\x14`\
-b\x80\xea9:\x99\x93O\x86\xb4_\x8b\xda%1O\
-\x01\xa8\xee\x1b\xc0\xb4\xa4Z\x0a\x90=u\x8b\xf8\xf04\
-T]S-Of \xd5r\xbd\xe8\x0eS-\xf1\xb2\
-D<&\x864\x8aG\xfeB\xa2\x17\x1b\xf3\xee\xc6\xd3\
-\xbd\xd8\xb0\x13\x7fl\xaa\xd1\xab8/\x1f\xf3\xef\xd7\xb3\
-/\x13\x7f\xd7\xc3WD\x84_\x06'\xc3Us/\x00\
-\xc8\x9cf2\x04\xd9\xf6\xea\x0d\x8aT\x1f\x99\x02H\xdd\
-3@i>Q\x0aH\xee\x13{\x81F\xe6\x03\x93!\
-\xec\xd5\x22u\xf1y)\x80\xd4=\x03\x94\xe6\xe3\xa4\x80\
-\x82\xfb\xde\xc4\xaeOK\xdf\xf9\xd2U\xe5}3\xb8\xad\
-\xc1\xaa\x0e1\x05\xed\xbfg#[J\xca\xca\xb6\x92\xbb\
-\x19\xb9\xcb\xf2%\x81P{\x0b\x22}\xc9\xe2 \xc4\xe2\
-L\xb2\xb7\x8dv\x95qV\xa9\xe9Q1\xbb\x8a\xb3\xc1\
-7\xa3\xe2\x1e\x94\x22\x9du\x91\x06Ta\xb1h\xa8\x98\
-)\x05\xed=\xceT\x1f\x9b\x15\xb2\xba\xbf\x90\xd3\xbcp\
-w\xc8]\xd2\xd4^\xe3\x95m\xee\x08\xc8\xd4g\x12\x85\
-Lil\xefQ\xa7:\x86\x9d)\xa0\xee\xaf\x02iN\
-e\xbb\x0a$<z\xec\x82z\x7f3\xe1\xe0{\xbe\xf1\
-C\xbdtc$\xe6\xf7\x07T1Y\x92\xdfm)\x8b\
-\xc9i\xfe\x19\xf7\x9d\xd3\xddE\x0e\xf7C\x83]\x19-\
-\x7f'6\x1e3|\x80\xbb\x08\x18=\x84\x97\x1a*2\
-!U\xf7\x0biZ\x84\xe8\x82\xb477\x9c\xa7&\xa1\
-\xa6\x03lA{\xd1\xed\x91\xf9\xf6\x8b\xbf\x06\x1d\x8f\x1a\
-q\xe0=\xbc\xb8\xdc=\xe0\xd4\x80\x91\x8c]=\x10\xd8\
-\xd3b\x85\x0c{\xe2s\xdf\x1d\x9a1\xbb\x83a\x1f_\
-\xc4\xfd\xb7\x0cE\xe2\xab[=A!\xbb\xe3\x90\xa1H\
-|1\xab'(d._\x86\xc2\xbb\xaf\x8c\x07\xb2\x14\
-\x0c]\xa3\x98'3\x10\xc5vv\x19\xc8\xbe\x9e\xf1\x15\
-9\x22\xf7\xef\xb1\xc0E\xda%\x05.\xff\xb2gg\x81\
-kb\x12x\x1fN\xec\xca\xd9\xf2\xaf2\xb2]\xde\xa5\
-\x85\xaa\x1e\x03\x92\xc4)5\x036u_\xb0\xa9)1\
-Tz\xe9)\x0bG\x13\x01\xb7HL\x88\x04Pj\xbf\
-\x0d4\xe8_\x05\xcfZ\xb0=\x00\xa6LL\xbf\xc8&\
-\xa7\xf2\x96\x0e-v5K\xdc\xa3\xd7e`\xdb\xf0\xbb\
-\xdd\xadv\x0bJ\x0f\x0dvjhJ\xd6@=@\x1a\
-\xa4\x05(\xa9\x06\xb2\xf7\xf2)l\xfa\xfa9}+c\
- s\x94\xe4_\xf5\xc5_\xc6\x97\x8d,\x0d\x8d\x0fi\
-\xe2d\x81T\x8691\x90V\xdc\x0few\x1a\xc2\xf8\
-\xb7\x8f\xe9/\x0bt\x0d\xa4=A\xb1\xed\x97\x06bo\
-F\x80q\x83L.`\xdf\x5czxr\xe2\xe5i\xc6\
-\x98\x8b\xbd:\xcd<\x1e\x13-.\xde\x0f\x0f)\x91\xe1\
-\xc5\x95N\x5c\x1e\xbb\xd0\xd9\x9e\xbc\xe8\xc7\xa4s\xb1\xc7\
-\xc1\xdb\x93\x17\xf9\x16u.\x1a\xce\xb7'-\xf2%\xeb\
-\x5ctq\xb6%-\xf8,{\xfad\xee\x7f\xa1\x92\x18\
-&\
+\x00L\xccx\xda\xdd[\xd1s\xd4\xc6\x19\x7f\xbf\xbfb\
+\x93\xbe\xd8\xd3\xc3\x1eK\x97\x1b\xc3\xf4:\x18l\x5c\x17\
+l3\xb1\xd3\x0c\xc3x<\xeb\xbb\xbd;q:\xe9F\
+\xd2\x1dg?\x01N(!I\x07:\xd0&\xa9\x93\x14\
+0\xcd$\xcd\x18H\x03\x98\x04\xc8\x83\xd3\x87\xbc\x90\xe3\
+\xcd~;J\xd2@\xe2N\xff\x85~+i%\x9d\xb4\
+\xd2\xc9\xf6\xd9\xd0d\x86X\xbb\xfb\xed\xb7\xbfo\xf7\xdb\
+\xef\xf7\xadVwt$\xab*h\xb2H\xcad*1\
+\x86\xcb$\xb3O#d\x8e\xa0A\xac\x95\xcc\x8a\xa3X\
+\x9b\xca\xac\x9d^\xfd\xc7\xda\xd9\xb5\xd7\xd1\xea\xb5\xd5\x8f\
+\xd6\xe6\xd7N\xdbMsS\xb6|\x12\x19+w\x95\x1c\
+*\xaf\xdc\xaa\xcdU\xad\xd6\x99\x02kE\x8d\xcb\x0f\xcf\
+6\xee6n6\xeeYMYL\x9b$\x1d\xa3\xbc\xaa\
+g1\xab\xdc[\xc32Q\xb2\x12\xb7Uw\xb4M\x96\
+qm\xe5c\xab:\x87\xa7\x82\x90s\xc4\xad\xac*%\
+\x22[\xd5D\x9e\xca<\xb8\xf2\xe0\x8b\x07_}\xfb\xda\
+\x83\x9b\x0f\xee<\xb8\xf7\xed[\xc8\x92\xb3\x05\x94\xe9\xe1\
+}\x1c}Dg\x80\x00OUS\xedZ\xc3\x115\xaa\
+e\xa6\xa2\xeaTJrU\xb1\xc1\xe7%\x8e\xd6\xbc\xe6\
+T\xeajyF\xb35\x14rS\x99q\xc9 \xb8\x80\
+rEU\xcb\x16m\x1d\x05\xd9\x11'\x1e\x14EP\xdd\
+\x5c\xfc\xb4y\xf5\xed\xe6\xe2\xf5\xe6\xd5\x13\xcd\xc5\x85\xe6\
+\xe2]\xd4\x5c\xbc\xd4\x5c\xbcoVA\xc3E[\xb6\xca\
+\x81!\xf1fP\xca9\x95\xc3D\xc6\x15\xbb\x96X\xf3\
+@\x90:C!\xd8\xb5\xee\xca\xe4Vn\x95J\x86]\
+mM\xcf\xdc\x1cF\x1e\xb8\xc7\xdc\xd1\x1e\xcf\x9fx<\
+\x7f\xf7\xf1\xa9kVK\x89\x87\xa3\xa4Ne\xd6\xff\xf4\
+\xf9O\xe7\xcf\xad\xbf\xf7y\xcbZ\xc9\x9e\xd9\xc7e\xbd\
+\xaa[\xd5\x8a\xcc\xd1\xa2(Neye\x99\xd5V@\
+t\xbfD\xca\x0a\x06\xc5\xb3s\xf64W\x0c\xb6\xd6C\
+\x14\xb6S;\xbd\xefe\x8efM5\xa5\xe7\xbe\x9eO\
+\xa2\x95%\xc5\xa8*$\x8b\xed\x09\xd0\xaa\xee\xeexx\
+\xea\xe1y\xd8\x00\xf7\x1e\xbe\xd9\xb8\x83\x1a\x9f5\xae?\
+<\xd1Xn\x5c\x87\x8aS\x96\xb0^\x9a\xca\x98~}\
+\x0f\xd5V.)\xaa\xad_\x07\x8c\x13\xb8\x22e1\xea\
+2(\xd4n\xd4\xe5\x01\xd1mK\x81'5>l\xdc\
+\x07\xc57\x1f\x9e2\x95_\x7fx\x1a\xd1G:hc\
+\x99\x89\xed\x95\x8e\x91\x12\xaeIX\xd9p\x07\x19\x1b\x12\
+\xf4:\xac\xd6\x88\x815\x9c\xa5\xb3\xaeH\x8e\x5cds\
+\xcd3\xfd\xb7\xd8\xd4\x19\xb0\xde\xcd\xa5O\x9aK_5\
+\x97\xae7\xaf\x9dh.-7\xaf\xbd\x8d\x9aK\x17\xcd\
+\xf2\xc9\xe6\xd2R\xf3\xda\x19[\x16BI\xe3}\xc0x\
+\x12f\xednc\x99\x22\xbdoN\xe1\x17\xb6\x00\xcc\xc0\
+\x90.)\x86\x84\x0e\xaa\xb3v\x00\xaa\xc2\x9c6.C\
+\xd4\xa1&]o\xf1\x9e\x9a\xbb!'\x1f}y\xde\x06\
+Z\xdfe\x10\x1d\xd6\xbf^\xf7\xccq\xbdn5\xce\x15\
+\xa7\xf7\x8f9\xbd\xbe\xbf\xbf\xf4\xf4\xca\x1f\xfe}\xfb\xc6\
+\x937>s\xda'_mu\x91\xc4~\xb5\x5c&\x8a\
+\xe1\xadD3\xb3\xc8(\x12tpp\x08\xfdnp\x98\
+\x89\xf0\xc3,Z{\xdd\xfd\xdf\xea\xa7\xf0pf\xf5\xce\
+\xea\xc7h\xf5\x93\xd5\x9bP\xa0\xa2k\xf3\xab\xd7\xd6\xce\
+\xbaj\xe6\x5c\xc3\xcc\x88l\x8f\x83\x8co\xde\xd5\xbey\
+7/)\xb9o\xdeU\x1cqn\x8cF0\xb7\xa7\x02\
+\x00}1;\x89\xb2\x1a\xc1\x06\xaa\x10\xd9\xd4\x9f\x83\xbf\
+\xd0\xc5#\xce\x8f\xe6\xc1~\xad\xdd\xf4\x96)Dj.\
+\x00\xc4\x17\xf2\x11\xce\x07E\xfc\x04\x80j@s9\xa2\
+\x05$#8\x01=\xb8\xf1\xed\x09(A\xc3W\xc1~\
+\x01\xaa\x08[X?y\xa0\x8a\xca\x81\xd1\xca%\xac}\
+\x97l\xb8\x22>fI2\xa1\x12\x22\x05\x09\x98\x86\x09\
+\xfa\xc8\x86\x89\xed\x91\x8d\x95EW\xc8O>IT\xc1\
+A\x5c\x01\xd2\xb1\xd7\xabE\xc8\xa2\xa0\x8b\xcd\xab\xbf\xa7\
+\xacC)\xe8\x0c\xf0\xcfM\xf3\xe9\x92MIWO@\
+\xd5\xdfL2\xbai\x13\xd3\xe2}\x14\x83\xb8\x9cA\xaa\
+\xbeUw\xe6\xc8\xf8\xe7y\xd9\x11\xf3\xb1\x19\x8d\x96t\
+\xea\xc7M\xbe\x22\xdd\xe0v\x1a\x92\x83&\xf8\xf9\x0e\xa9\
+2)\x06\xa5|\xfc\xc7\x9c\xbeU\xc8O\x87(\xaf\xad\
+\x5c\x0a\x8a\xf9\xe8\x91\xab\x8b\xb2%\xdb\xc0\x8fO\xfe\xfd\
+\xf1\xa93\x8fO\xbd\x89\x02\xfc\xc9\xc4}\x14\x8a^\xb4\
+\xfb\xbe\xb8\xeb\xd1\xfc\xa5G\xf3\x7f|4\x7f\xee\xd1\xfc\
+\x82+\xaeZ\xda\xd7\xdf\x5c\xf8\xf1\xfaI\xf4\xd3\x85\x0b\
+\xeb\x1f\x9c[\x7f\x7f\x19\xfdx{\xf9\xa7+w\xd6\xff\
+|n\xfd\xb5\x05\xb4\xfe\xd7\x85\xf5\x0f\xce\xff\xe7\x22<\
+\xf9\x89\x98)\x0ap1\xf8R\x01\x07\xcd\xf1\x913\xca\
+\xa9\xaa\xc6s(?_\xd3\x19\xbc\x1a\x90\xf2\xf37\xc2\
+UC\xd5t\xe38\x0e\x8a\xb6\x92:L6\xb6\x82\x8f\
+\xda\x12|\x82,O\xc3\x94\x1aP\xc7g\xfd$\xcf\x14\
+\x9a\x04@d\x0d#\x7f\xb6\x96\xdc\x88\x1b\xc8\x09x\xd1\
+P\x97\xdb\x06L?\xff\x22\x5c\xa32{tT\x93\xf4\
+*\x91e\x0c\xc8u\xa9\xa0\x14\xb4j\xa5\xe2t\x8b \
+]\x04\xe8o\x07\xc6\xa1$L\xeb\x86a\x10\x1d\xbcy\
+\x12\xebX\xfb\xfaF\x19\x0dk\xd5\x99\xaa\x92\xc3\x0a\xf2\
+r4\xebFi\xdacA\x92*\xff\x8c\x8d\x85\xfeu\
+\xe2B` ?{'\xed\x85l\x11\xe2\x92\xb9/H\
+\x03\xb73\xf1pz\xffn\xf9\xcb\xa7\x97\xdf\xf9\xef\xdd\
+\xb7~\xb8p\xc3\xa1\xd3\xae'\x1f\x9d~\xf2\xd1\x1bO\
+\x96\xee?Y\xba\xf4\xfd_.?}\xe7\xc3nd\x97\
+\xce\xdc\xfa\xee\xde\x82W1\xcd\x0b\xbc\x9d\xbf_x\xe7\
+\xe9{g\x9f\x5c\xb9\x07r?\xbc\xf7\x1aj\xc9\x19\x06\
+%\xbd\x22\xe3\xd9AR1\x8a\x19QH$F\x94\x22\
+\xd1$C\xcf\xccX\xc9dQ\xca\xaa\xb2\xaa%\x12C\
+u\x5c\xae\xc8$\x93We\xa0\xb6D\xe2\x80*\xcb\xea\
+q}?m\x9d\xc8\xd23]\xc6\xd0\xaa\x04T\x12\xbd\
+d\xa8\x95A\x92\xc7U\xd9\xc8\xa4\xfaY\xcd\x844G\
+\xf4L_:)\x08IQH\xa6\xfa\x93\xe9T\xb2O\
+\xe8O\x0a/\xa5\x13\x93\xaa*\xcf`\x8d\xf5\x12\x04V\
+\x13\xe8\x95\x18\xc5\x92\x12\x14\xf7\xd4\x06\xbbL\x94\xb1,\
+3\xe1\xbe\xb4U\x0e\x8a\x1d\xc6\x0a\x91=\xc0\xcdr$\
+\xecA\x09\xcbj\x81u\x81\x09\xb4*\x22\xfb$`e\
+v\x0d\xd5\x0d\xa2\xe8\x92\xaa\xe8\x99\x1e\xbdVH$~\
+\xe1\xfc\x87\x06%\x8dd!\xbaHD\xf7V\xab\x1aL\
+<\xc9Q\xaf\x82\x00@\x0a\xaa6\x8b0$]X\xae\
+\x14\xf1\x0c1 o\x97\xe5Y\xba\xa6N\xf7\x0c\xce\x1a\
+t\x8c\xde>!\xe9<\xa6\x9dG\xc1\xad\x15R\xce\xa3\
+\xe8\xd6\x02p\xf6\x08\x06`E*cW\x89[\xa2z\
+*\x15\xab\x96\xfeee\xd1\xfe\x0bj*\x1a\xc9\x03z\
+%K\xccfo\xd1\x92\x92\x89\xc1\x14\x98\x8f\x82[K\
+Q\xd8\x8f\x14\x05\x93\x15\xdcj\x98\xd6\xa4='\x92\xa5\
+1Gj\x12U\x0e\x1a\xd9\xa3\xe0\xd6\x82\x1aR\x9e\x91\
+IY\xef\xedw\x9e@\x94=\x82()\xab\x86\xd5\xa9\
+,\x95\x891[\xb1\x94\xb9\x85\x96\x16\xd1[\x00\xed\xb0\
+\xa9\xec\xd1\xed'j\xb3\xf5$:OtZ\xac\xa7\xdd\
+\x8e\x1c\xf4\xd5\x0dlT\xcd\xbe\xf6\x13\xf4eON\xab\
+\xe8\xd4\x81\x16\xfb)\xed\xae\xa1>[\x9eQe)\xeb\
+X\xecT0\x13\x9d\x0a{`\xa7l+c\xe5\xc4\x04\
+\xb8\x15\xc9q\x9d*\xbdW\xa8{\xfcj\xafX\xf7\xb8\
+\x96\xb7\x0dJ\xde\xb6TK[\xca\xdb&\xb6\xf4\x13\xad\
+~^\xbf3\x9b[*\xa8\x84\xe5}f\x9b\xfd\xc8j\
+m \xf6#\xd4\xba\x9eA\x1b<%O\x9b\xd5\xc9S\
+\x826\xd7Mh\x9b\xa7\xe4i\xb3\xfayJf\x9b\xed\
+HV\x13+@\x8b\xd7\xb1hcK\xb9\xa5\xdd\xea\xdc\
+R\x86v\xc7\xc9h\xa3[p[\xacnn\x01Z\x1c\
+\xe7\xa2-n\xc1m\xb1\xfa\xb8\x05\xb1\xde\x12\x9b\x06\xac\
+\x95\x09\x89K:\xc4=\x10\xef\x13\xea}\x02\xda\x85\x0e\
+Hu\xa8\xa7\x95\xb4\x00\xe9\xd7\x88R\x82SY\x85$\
+\x8e\xba\x81i*A\xa3e\xa6O\x00\x12S\x0cR7\
+2l\x8cI\xb05c\xea\xa0:\xd3\xf5\xbe4Og\
+\x152dI\x81\x9a\x1c\x81\xd8\xdf\xa5w#\x9dFw\
+H\xbd\x0d\x8b\x0eh\xd5\xaf_x\xe1\x85\xf1\xb1CG\
+\xe0\xcf\xaf\xf6 \xd2S\xe8A\x07!^\xa0\xb2Z\xc3\
+\xb0X\xacw\xaf\xdd\x05u\xe9\x04k\xd9\xa2\x19_5\
+b\xce \x9c%\xab\x1a\x84,8Mj\xea1\xd8\x0c\
+ID\x8clO7\xd8\x8f~[-!\x03\x08\x13r\
+\x1cr\x1cp\x0d\x8eO\x8f\x8dON\xbf214=\
+0v\xe4\xd5\xdf\x0c\xbd<4=thb\x08\x9aF\
+UE\xcd\x165\xb5\xec\x9d\x844\x9b\x84t\x8cI\x80\
+\xf5\xf9\xd9\xce\x03\xd8\xe6N\x85\x19y2q\xfc\x02\xbc\
+\xf4\xe7;%b`J\xc4\xe8)\x11\x84\xba\xc0\xdd~\
+\xcc\x04\xc8\xe9\x14\xbd\xc5\xf0\x8d\x03\x13\xd8\xc6\x15\x84\x18\
+hB|\xb6\xb3\x80\x5c\xe7\x01L\xb1\x9c\xc7\xc2&\xee\
+\x0461\x80\xad\xdd*\xa6\xeaB\xca\x0flx\xf2`\
+g\x00\xa5\x18\x9aT\x0c\x14\x9c\xd5\xeb\x1c\x10\xcf\xaa\xa5\
+b\xae\x9a\x89I\xdcNLb\x00S\x9b\xd5\x12\x85\xba\
+\xb8\xed{Nd{N\x0c\x99!\x0a\x95\x06\xad\xc4\xa8\
+\xa40\xc1Q\x5c\xb7,\xa1G\x0f\x0b\xe7\x0e\xecF\xd1\
+\xb3\x1b\xc56\xbb1.jq'P\x8b\x01\xd4\xe2f\
+Q\xa7\xfa\xeb\xa9\xfe\xed\x86\x9c\xea\xb7\xf1\xc2y5\x1e\
+N\xf3\x08\xed\xc5\x99N\xd5\xd3\xa9\xed\xc6\x99f\x11'\
+\x9d\xda\xec|z\xb2P\xe7\x00\xd0&\x11\xe5%\x8d\x03\
+ph\x84\xb32\xednZF\x93\x80<X;\xa8\xc2\
+A\xdaM\x17@r\xfc\xf0\xe4\xc8\xf8\xd8\xc0!\xf4\xcb\
+\xd8\xd6zO&\x9c\xa4\xce\xc5\x1d+\xaf\xdb1\xa8\xd1\
+yW$j\xf1\x19\xa2\x8eL\x8dBP\xb3\xec\xc8\xf1\
+\xb7\xa3-o28Y\x8dOQ\xc0Q\x85\x08G\x85\
+s\xe7\xf3\xe6\xa2\xd6\x01\x99\xe3\x9c\xee\xa0\xcf\x83{:\
+G\xfa\x08\xc7l\x83X|&\x88#\x9d2\x1417\
+i\x7fU\xd5JXS\xabp\xd4\xf0\xa2\xf5\x9c^f\
+\xaa\x86a5\x98'\x17f\xc7x\x85(h\x92he\
+I\xc1r\xef\xc0\x8cZ5X\x9b]\xa2\xaf\x87\xad\xce\
+:\x1d\xe8\xe5\xf1\xb1\xe1\xe9\x91\xfd\xe3c`\xe6\xc0\xf0\
+\xd0\xf4\xbe#\xd3\x03\x87\x0f\xf3,\xe4n\x91h\xb38\
+\xae\xf3|Z\x16}\x82hc\xa4\xf8\xffbd\xe4Q\
+$\xd4\xc8\xd0\x0cwbV7H\x19M\x10\xc3\x90\x94\
+\x82\xce\xcf\x16X\xd0\x04\xe3\xcd;\x91\xbcy}\x00\xf2\
+\xa6&}\x0f\xb2\xd4w\xe5\xacW\xe9\xddIdf%\
+I\xd4'\xf4\xd7\xe9\xab^\x04\xa1\xb5\x0e\xff\xa23\x0f\
+\xf3:\xc2\xb6\x94\x9b-\x87\x9a\xc7\x925\x07\xa8e\x1c\
+\xf6\x05\x8c\x8d\x1bf)\xf6\x18\xb6;]\xdf\x9d6_\
+\x1fXG\xbc.E5\x90F\xb2\xe6\x15N\x8e\xe4\xba\
+\xe3\x9b\xc8M\xfe\x02&\xb6\xcf\x00\xd9\xda\xfa\x8c\x7f\x0e\
+W\xb6\xf5\xe2 \xce\x02\xb7\xcf+C\xdf\x97\xc4\xb2\x7f\
+c\x987\x16=Yr0\xae\xc8\xb3\xf4mV\xce\x8c\
+\x1fY\xac\xd1;\xa3$\xd2g\xcb\xb2\xa4\x94\xec\xea\x83\
+\xa3\xb3\xb0\xdb\xc9\xac\xe9\x1b\xf6uJ\x90\xe5'\xcc7\
+\xbb\xbe\xf8\xe5,\x80\x89\xd8\xd4f\xebp\x95\xf1\x90{\
+\x95\xb5O\x8bb\x0d\xc3s\xe9\xc8a\xc4\xf0a\x9c\xcc\
+\xcd^9:`\x09\x5c\x93\xde@\xd3\x1bID\xf2y\
+\x92\xf5\x8e\xce;\xa5lvtw\xa3\xb2\xfb*\xe7U\
+w\xff\xd6\xfc\xd5\x19\x82\x13\xac`(\xd4\x8b\x8eK\xb9\
+\x02}\x0axl\xdc\xd8\xc2\xae\xd5\xd8\x9a\xbf\x94\xdeR\
+\x80q3\xe0\xfd\xce5]t^\x1cJ7\xee=\x1f\
+\x7f?\xbeB\xb7\x09\xac\xf1A)[R\xf3y\xd4E\
+\xa92\xd5S\xef\xa9w\x9bA\xf7\x10\x86\x8d(\xabF\
+\x0f\x1a\x90u\xd5\xdaU >:09d\xb6\xef\x97\
+\x14\x05\x97\xc1g\xba\x8eUu\x03\x1d82\xd2\x1d\xff\
+\xb4\xdbr\x09\x19\x8cN\x1e\xe37|\xe6\x1d\xb4n\xa3\
+6q\x9a\xa0\xb3f\xbe\xf8F\xd6\x8d\xd6\x96\xce\xf3\xee\
+\x85Y0\xb60\x88\xde\xe0\x12}i\xb1\x0d\xb0\x22O\
+\x0c<\x84\x91W\x08\xdb\x010\xea\x80\xc0\x05\x18JP\
+\x1dG\xc7\x0b\xf2\xe1\x90vjQ\xdb$\xe6\x11\x00\xc5\
+\x1d\x03\x18\x95Ts\x01\xb2\xb7n\xbe\x18\x1e\x85\xaam\
+\xaae\xe9\xf4\xa4Zf\x14\xddd\xaa\xe5~,\x11\xe4\
+\xc4\x16\x8b\x82\xcc\x9f\x0a\x8dbC\xd6\xddxt\x14\xeb\
+\xaf\x07_\x9bJ\xf4*\xce\xca\xc7\xec\xfb\xf5\xf8\xcb\xe4\
+|\xeba\x1b\xe2\xd2/\x83\x13\xe3\xaa\xb9\x13\x00xA\
+3\x1c\x02o{u\x06Ed\x8c\x8c\x00$n\x1b\xa0\
+\xa8\x98\xc8\x05\xc4\x8f\x89\x9d@\xc3\x8b\x81\xe1\x10\xb6k\
+\x91\xda\xc4\xbc\x08@\xe2\xb6\x01\x8a\x8aq\x5c@\xde}\
+\xaf\x1afL\x8b\xde\xf9\xdcUu\xfa\xc6\x08[\xbdy\
+\x19\x1b\x14\xb4\xfd\x9d\x0do)iS\xbc\x95\xdc\xca\xc8\
+m\x96/\x0c\x84\xd8Y\x10\xd1K\x16\x04\xe1.\xce(\
+\xfb\xdahK\x19g\x9e\xba\x1eU\xb3%\x9e\xf5~\x19\
+\x15\x8c\xa0\x14\xe9\xa4\x89\xd4c\x0a\xe3\xa2\xbet\xac\x14\
+\xb4\xf38#cl\x5c\xc8\xe2\xceB\x8e\x8a\xc2\xed!\
+\xb7IS;\x8d\x97\xb7\xb9} #\xdfI\xa4b\xa5\
+\xb1\x9dG\x1d\x19\x186g\x80\xb8\xb3\x06D\x05\x95\x8d\
+\x1a\x10\xf2\xea\xb1\x0d\xea\x9d\xcd\x84\xbd\xdf\xf9\x06\x0f\xf5\
+\xdc\x8d\x11\x9a\xdf?\xa7\x86\xf1\x92\xfcvK\x99\x0eO\
+\xf3\x0f\x9b\xdf\x9cn\x8d9\xcc\x1f\x1al\xc9i\x9do\
+b\x83\x9ca\x03\xdc\x02at\x10^$U\xc4B*\
+\xee\x14\xd2(\x86h\x83\xb437\x9c\x07G\xb1$#\
+C\xc3z\xd1\xec\x11\xfb\xf6\xcb\xf9\x0c:\xc8\x1aA\xe0\
+\x1d\xbc\xb8\xdc:\xe0H\xc2\x08\xc7.>\x17\xd8\xa3\xb8\
+\x82\x87=\xf4\xbd\xef&\xdd\x98\xdd\xc1\xb0\x1f_\x04\xe3\
+7\x0fE\xe8\xa7[\x1dA\xc1\xbb\xe3\xe0\xa1\x08\xfd0\
+\xab#(x!\x9f\x87\xc2\xba\xaf\x0c\x12Y\x04\x86\xb6\
+,f\xe9\xf4\xb0\xd8\xe6.\x03\xd9\xafglCv\xf3\
+\xe3{\x80\xb8@.\x8c\xb8\xec\xcb\x9e\xcd\x11\xd7\xc8(\
+\xb2~8\xb1\xa5`\xeb\xfc*#\xde\xe5]\x14Uu\
+\x18\x10\x87\xa7\xc4\x18\xd8\xc4\x1d\xc1&Fp(\xf7\xd2\
+\x93GG#\x9e\xb0\x08.\x04\x04J\xfd\xb7Lz\xed\
+\xab\xe0I\x0d\xcf\xf6\xa01\xd5\xa0?`\x87SyU\
+\xc6\x1a\xbb\x9a\x85\xf0hu\xe9\xd90\xfcvw\xab\xed\
+H\xe9\x99\xc1\x8e\xa4\xa6p\x0b\xc4\xe7\xc8\x82(\x82\xe2\
+Z\xc0\xfb.\x9f\xc2\xa6\x9f\x9f\xd3\xaf2zb\xb3\xa4\
+\xf3\xab\xbe\xe0\xc7\xf8\xbc\x91\xb9\xd4\xf8\x8c&\x8eG\xa4\
+<\xcc\xa1D\x9a3\x7f(\xbbY\x0as~\xfb\x18\xfd\
+\xb1@[\x22\xed\x08\x8a\x0d\x7f4\x10\xf82\x02\x0d+\
+0\xb9\x88\xfd\xe6\xd2\xc2\x93p?\x9ef\x0dS\x81O\
+\xa7Y\xc4c\xaa\xdd\x8b\xf7\x97\xfa\x04\xdf\xf0\xee\x95N\
+P\x1f\xbb\xd0\xd9\x98>\xff\x8fI\xa7\x02\xaf\x837\xa6\
+\xcf\xf7[\xd4)?\x9doL\x9b\xef\x97\xacS\xfe\xc5\
+\xd9\x906\xef\xbb\xec\xf1\x03\x89\xff\x01\x0d\xa6\xa5u\
 \x00\x00\x03q\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      .ColorSc\
 heme-NegativeTex\
 t {\x0a        colo\
 r:#da4453;\x0a     \
  }\x0a      </style\
 >\x0a  </defs>\x0a  <p\
 ath\x0a     style=\x22\
@@ -618,15 +309,15 @@
 fs>\x0a        <sty\
 le type=\x22text/cs\
 s\x22 id=\x22current-c\
 olor-scheme\x22>\x0a  \
           .Color\
 Scheme-Text {\x0a  \
               co\
-lor:#232629;\x0a   \
+lor:#eff0f1;\x0a   \
          }\x0a     \
    </style>\x0a    \
 </defs>\x0a    <pat\
 h class=\x22ColorSc\
 heme-Text\x22 style\
 =\x22fill:currentCo\
 lor; fill-opacit\
@@ -681,15 +372,15 @@
 /2000/svg\x22>\x0a    \
 <style type=\x22tex\
 t/css\x22 id=\x22curre\
 nt-color-scheme\x22\
 >\x0a        .Color\
 Scheme-Text {\x0a  \
           color:\
-#232629;\x0a       \
+#eff0f1;\x0a       \
  }\x0a    </style>\x0a\
     <g class=\x22Co\
 lorScheme-Text\x22 \
 fill=\x22currentCol\
 or\x22 fill-rule=\x22e\
 venodd\x22>\x0a       \
  <path d=\x22m8 2a6\
@@ -702,28 +393,108 @@
  0 1 -5-5 5 5 0 \
 0 1 5-5z\x22/>\x0a    \
     <path d=\x22m7 \
 4h2v2h-2z\x22/>\x0a   \
      <path d=\x22m7\
  7h2v5h-2z\x22/>\x0a  \
   </g>\x0a</svg>\x0a\
+\x00\x00\x04\xe0\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 viewBox=\x22\
+0 0 16 16\x22>\x0a  <d\
+efs id=\x22defs3051\
+\x22>\x0a    <style ty\
+pe=\x22text/css\x22 id\
+=\x22current-color-\
+scheme\x22>\x0a      .\
+ColorScheme-Text\
+ {\x0a        color\
+:#eff0f1;\x0a      \
+}\x0a      </style>\
+\x0a  </defs>\x0a <pat\
+h \x0a     style=\x22f\
+ill:currentColor\
+;fill-opacity:1;\
+stroke:none\x22 \x0a  \
+   d=\x22M 8 2 A 6 \
+6 0 0 0 2 8 A 6 \
+6 0 0 0 8 14 A 6\
+ 6 0 0 0 14 8 A \
+6 6 0 0 0 8 2 z \
+M 2 3 L 2 5 L 4 \
+3 L 2 3 z M 8 3 \
+A 5 5 0 0 1 10.3\
+90625 3.609375 L\
+ 8.8691406 5.130\
+8594 A 3 3 0 0 0\
+ 8 5 A 3 3 0 0 0\
+ 7.1308594 5.130\
+8594 L 5.6132812\
+ 3.6132812 A 5 5\
+ 0 0 1 8 3 z M 1\
+2 3 L 14 5 L 14 \
+3 L 12 3 z M 3.6\
+09375 5.609375 L\
+ 5.1308594 7.130\
+8594 A 3 3 0 0 0\
+ 5 8 A 3 3 0 0 0\
+ 5.1308594 8.869\
+1406 L 3.6132812\
+ 10.386719 A 5 5\
+ 0 0 1 3 8 A 5 5\
+ 0 0 1 3.609375 \
+5.609375 z M 12.\
+386719 5.6132812\
+ A 5 5 0 0 1 13 \
+8 A 5 5 0 0 1 12\
+.390625 10.39062\
+5 L 10.869141 8.\
+8691406 A 3 3 0 \
+0 0 11 8 A 3 3 0\
+ 0 0 10.869141 7\
+.1308594 L 12.38\
+6719 5.6132812 z\
+ M 8 6 A 2 2 0 0\
+ 1 10 8 A 2 2 0 \
+0 1 8 10 A 2 2 0\
+ 0 1 6 8 A 2 2 0\
+ 0 1 8 6 z M 7.1\
+308594 10.869141\
+ A 3 3 0 0 0 8 1\
+1 A 3 3 0 0 0 8.\
+8691406 10.86914\
+1 L 10.386719 12\
+.386719 A 5 5 0 \
+0 1 8 13 A 5 5 0\
+ 0 1 5.609375 12\
+.390625 L 7.1308\
+594 10.869141 z \
+M 2 11 L 2 13 L \
+4 13 L 2 11 z M \
+14 11 L 12 13 L \
+14 13 L 14 11 z \
+\x22\x0a     class=\x22Co\
+lorScheme-Text\x22\x0a\
+     />\x0a</svg>\x0a\
 \x00\x00\x03\xdd\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a       d\
 =\x22M 10 2.5 C 9.0\
@@ -766,68 +537,28 @@
 72 12.5 4 12.052\
 28 4 11.5 C 4 10\
 .94772 4.44772 1\
 0.5 5 10.5 z \x22\x0a \
     class=\x22Color\
 Scheme-Text\x22\x0a   \
   />\x0a</svg>\x0a\
-\x00\x00\x02[\
-<\
-svg version=\x221.1\
-\x22 viewBox=\x220 0 1\
-6 16\x22 xmlns=\x22htt\
-p://www.w3.org/2\
-000/svg\x22>\x0a    <s\
-tyle type=\x22text/\
-css\x22 id=\x22current\
--color-scheme\x22>\x0a\
-        .ColorSc\
-heme-NeutralText\
- {\x0a            c\
-olor:#f67400;\x0a  \
-      }\x0a    </st\
-yle>\x0a    <path c\
-lass=\x22ColorSchem\
-e-NeutralText\x22 d\
-=\x22m8.0065001 2.0\
-000269a0.7500188\
-1 0.74999832 0 0\
- 0-0.6772669 0.4\
-14749l-5.2501316\
- 10.499976a0.750\
-01881 0.74999832\
- 0 0 0 0.6712668\
- 1.085248h10.500\
-264a0.75001881 0\
-.74999832 0 0 0 \
-0.671266-1.08524\
-8l-5.2501312-10.\
-499976a0.7500188\
-1 0.74999832 0 0\
- 0-0.6652667-0.4\
-14749z\x22 fill=\x22cu\
-rrentColor\x22/>\x0a  \
-  <path d=\x22m7 5v\
-4h2v-4zm0 5v2h2v\
--2z\x22 fill=\x22#fff\x22\
-/>\x0a</svg>\x0a\
 \x00\x00\x06i\
 <\
 svg version=\x221.1\
 \x22 viewBox=\x220 0 1\
 6 16\x22 xmlns=\x22htt\
 p://www.w3.org/2\
 000/svg\x22>\x0a    <d\
 efs>\x0a        <st\
 yle type=\x22text/c\
 ss\x22 id=\x22current-\
 color-scheme\x22>.C\
 olorScheme-Text \
 {\x0a        color:\
-#232629;\x0a      }\
+#eff0f1;\x0a      }\
 </style>\x0a    </d\
 efs>\x0a    <path c\
 lass=\x22ColorSchem\
 e-Text\x22 fill=\x22cu\
 rrentColor\x22 d=\x22m\
 14 8c0 1.1088173\
 -0.319333 2.1400\
@@ -911,94 +642,14 @@
 1299 0.063349-0.\
 01766 0.09375-0.\
 03125 0.08886-0.\
 04062 0.164735-0\
 .108612 0.25-0.1\
 5625h0.03125z\x22/>\
 \x0a</svg>\x0a\
-\x00\x00\x04\xe0\
-<\
-svg xmlns=\x22http:\
-//www.w3.org/200\
-0/svg\x22 viewBox=\x22\
-0 0 16 16\x22>\x0a  <d\
-efs id=\x22defs3051\
-\x22>\x0a    <style ty\
-pe=\x22text/css\x22 id\
-=\x22current-color-\
-scheme\x22>\x0a      .\
-ColorScheme-Text\
- {\x0a        color\
-:#232629;\x0a      \
-}\x0a      </style>\
-\x0a  </defs>\x0a <pat\
-h \x0a     style=\x22f\
-ill:currentColor\
-;fill-opacity:1;\
-stroke:none\x22 \x0a  \
-   d=\x22M 8 2 A 6 \
-6 0 0 0 2 8 A 6 \
-6 0 0 0 8 14 A 6\
- 6 0 0 0 14 8 A \
-6 6 0 0 0 8 2 z \
-M 2 3 L 2 5 L 4 \
-3 L 2 3 z M 8 3 \
-A 5 5 0 0 1 10.3\
-90625 3.609375 L\
- 8.8691406 5.130\
-8594 A 3 3 0 0 0\
- 8 5 A 3 3 0 0 0\
- 7.1308594 5.130\
-8594 L 5.6132812\
- 3.6132812 A 5 5\
- 0 0 1 8 3 z M 1\
-2 3 L 14 5 L 14 \
-3 L 12 3 z M 3.6\
-09375 5.609375 L\
- 5.1308594 7.130\
-8594 A 3 3 0 0 0\
- 5 8 A 3 3 0 0 0\
- 5.1308594 8.869\
-1406 L 3.6132812\
- 10.386719 A 5 5\
- 0 0 1 3 8 A 5 5\
- 0 0 1 3.609375 \
-5.609375 z M 12.\
-386719 5.6132812\
- A 5 5 0 0 1 13 \
-8 A 5 5 0 0 1 12\
-.390625 10.39062\
-5 L 10.869141 8.\
-8691406 A 3 3 0 \
-0 0 11 8 A 3 3 0\
- 0 0 10.869141 7\
-.1308594 L 12.38\
-6719 5.6132812 z\
- M 8 6 A 2 2 0 0\
- 1 10 8 A 2 2 0 \
-0 1 8 10 A 2 2 0\
- 0 1 6 8 A 2 2 0\
- 0 1 8 6 z M 7.1\
-308594 10.869141\
- A 3 3 0 0 0 8 1\
-1 A 3 3 0 0 0 8.\
-8691406 10.86914\
-1 L 10.386719 12\
-.386719 A 5 5 0 \
-0 1 8 13 A 5 5 0\
- 0 1 5.609375 12\
-.390625 L 7.1308\
-594 10.869141 z \
-M 2 11 L 2 13 L \
-4 13 L 2 11 z M \
-14 11 L 12 13 L \
-14 13 L 14 11 z \
-\x22\x0a     class=\x22Co\
-lorScheme-Text\x22\x0a\
-     />\x0a</svg>\x0a\
 \x00\x00\x01\xa1\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
@@ -1020,28 +671,62 @@
 gativeText\x22\x0a    \
  d=\x22m5 2v2h1v-1h\
 4v1h1v-2h-5zm-3 \
 3v1h2v8h8v-8h2v-\
 1zm3 1h6v7h-6z\x22 \
 \x0a     />\x0a</svg>\x0a\
 \
+\x00\x00\x01\xfb\
+<\
+svg viewBox=\x220 0\
+ 16 16\x22 xmlns=\x22h\
+ttp://www.w3.org\
+/2000/svg\x22>\x0a    \
+<style type=\x22tex\
+t/css\x22 id=\x22curre\
+nt-color-scheme\x22\
+>\x0a        .Color\
+Scheme-Text {\x0a  \
+          color:\
+#eff0f1;\x0a       \
+ }\x0a    </style>\x0a\
+    <path d=\x22m3 \
+2v12h7.5c1.385 0\
+ 2.5-1.115 2.5-2\
+.5s-1.115-2.5-2.\
+5-2.5h-1.7929688\
+l1.4999998-1.5-.\
+707031-.7070312-\
+2.7070312 2.7070\
+312 2.7070312 2.\
+707031.707031-.7\
+07031-1.4999998-\
+1.5h1.7929688c.8\
+31 0 1.5.669 1.5\
+ 1.5s-.669 1.5-1\
+.5 1.5h-6.5v-10h\
+5v3h3v2h1v-3l-3-\
+3z\x22 class=\x22Color\
+Scheme-Text\x22 fil\
+l=\x22currentColor\x22\
+/>\x0a</svg>\x0a\
 \x00\x00\x02[\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 2 2 L 2 3 L 2 \
@@ -1060,70 +745,28 @@
 921875 6 L 3 6 L\
  3 3 z M 3 7 L 1\
 3 7 L 13 13 L 3 \
 13 L 3 7 z \x22\x0a   \
   class=\x22ColorSc\
 heme-Text\x22\x0a     \
 />\x0a</svg>\x0a\
-\x00\x00\x02y\
-<\
-svg id=\x22svg6\x22 ve\
-rsion=\x221.1\x22 view\
-Box=\x220 0 16 16\x22 \
-xmlns=\x22http://ww\
-w.w3.org/2000/sv\
-g\x22>\x0a    <style i\
-d=\x22current-color\
--scheme\x22 type=\x22t\
-ext/css\x22>.ColorS\
-cheme-Text {\x0a   \
-         color:#\
-232629;\x0a        \
-}</style>\x0a    <p\
-ath id=\x22path4\x22 c\
-lass=\x22ColorSchem\
-e-Text\x22 d=\x22m7.5 \
-2-3.5 3.5 3.5 3.\
-5 0.71875-0.7187\
-5-2.3125-2.28125\
-h3.59375c1.93299\
-8 0 3.5 1.566998\
-4 3.5 3.5 0 1.93\
-3002-1.567002 3.\
-5-3.5 3.5h-1.5v1\
-h1.5c2.485283 0 \
-4.5-2.014748 4.5\
--4.5 0-2.4852521\
--2.014717-4.5-4.\
-5-4.5h-3.59375l2\
-.3125-2.28125z\x22 \
-fill=\x22currentCol\
-or\x22/>\x0a    <rect \
-id=\x22rect837\x22 cla\
-ss=\x22ColorScheme-\
-Text\x22 x=\x222\x22 y=\x222\
-\x22 width=\x221\x22 heig\
-ht=\x227\x22 fill=\x22cur\
-rentColor\x22 fill-\
-rule=\x22evenodd\x22/>\
-\x0a</svg>\x0a\
 \x00\x00\x02\xdd\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 2 2 L 2 14 L 3\
@@ -1150,28 +793,70 @@
  6 10 L 10 10 L \
 11 10 L 11 13 L \
 10 13 L 6 13 L 5\
  13 L 5 10 z \x22\x0a \
     class=\x22Color\
 Scheme-Text\x22\x0a   \
   />\x0a</svg>\x0a\
+\x00\x00\x02y\
+<\
+svg id=\x22svg6\x22 ve\
+rsion=\x221.1\x22 view\
+Box=\x220 0 16 16\x22 \
+xmlns=\x22http://ww\
+w.w3.org/2000/sv\
+g\x22>\x0a    <style i\
+d=\x22current-color\
+-scheme\x22 type=\x22t\
+ext/css\x22>.ColorS\
+cheme-Text {\x0a   \
+         color:#\
+eff0f1;\x0a        \
+}</style>\x0a    <p\
+ath id=\x22path4\x22 c\
+lass=\x22ColorSchem\
+e-Text\x22 d=\x22m7.5 \
+2-3.5 3.5 3.5 3.\
+5 0.71875-0.7187\
+5-2.3125-2.28125\
+h3.59375c1.93299\
+8 0 3.5 1.566998\
+4 3.5 3.5 0 1.93\
+3002-1.567002 3.\
+5-3.5 3.5h-1.5v1\
+h1.5c2.485283 0 \
+4.5-2.014748 4.5\
+-4.5 0-2.4852521\
+-2.014717-4.5-4.\
+5-4.5h-3.59375l2\
+.3125-2.28125z\x22 \
+fill=\x22currentCol\
+or\x22/>\x0a    <rect \
+id=\x22rect837\x22 cla\
+ss=\x22ColorScheme-\
+Text\x22 x=\x222\x22 y=\x222\
+\x22 width=\x221\x22 heig\
+ht=\x227\x22 fill=\x22cur\
+rentColor\x22 fill-\
+rule=\x22evenodd\x22/>\
+\x0a</svg>\x0a\
 \x00\x00\x02\x0e\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h \x0a     style=\x22f\
 ill:currentColor\
 ;fill-opacity:1;\
 stroke:none\x22 \x0a  \
    d=\x22M 3 2 L 3 \
@@ -1232,15 +917,15 @@
 0 0 16 16\x22>\x0a    \
 <style type=\x22tex\
 t/css\x22 id=\x22curre\
 nt-color-scheme\x22\
 >\x0a        .Color\
 Scheme-Text {\x0a  \
           color:\
-#232629;\x0a       \
+#eff0f1;\x0a       \
  }\x0a    </style>\x0a\
     <path d=\x22m2 \
 2v12l12-6z\x22 clas\
 s=\x22ColorScheme-T\
 ext\x22 fill=\x22curre\
 ntColor\x22/>\x0a</svg\
 >\x0a\
@@ -1253,15 +938,15 @@
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 7 3.0058594 L \
@@ -1286,15 +971,15 @@
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 6 2 L 0.707031\
@@ -1318,60 +1003,28 @@
 .0214844 8 L 7.0\
 117188 5.9902344\
  L 8.0019531 5 z\
  \x22\x0a     class=\x22C\
 olorScheme-Text\x22\
 \x0a     />\x0a</svg>\x0a\
 \
-\x00\x00\x01\xd1\
-<\
-svg version=\x221.1\
-\x22 viewBox=\x220 0 1\
-6 16\x22 xmlns=\x22htt\
-p://www.w3.org/2\
-000/svg\x22>\x0a    <s\
-tyle type=\x22text/\
-css\x22 id=\x22current\
--color-scheme\x22>\x0a\
-        .ColorSc\
-heme-NegativeTex\
-t {\x0a            \
-color:#da4453;\x0a \
-       }\x0a    </s\
-tyle>\x0a    <rect \
-class=\x22ColorSche\
-me-NegativeText\x22\
- x=\x222\x22 y=\x222\x22 wid\
-th=\x2212\x22 height=\x22\
-12\x22 rx=\x222\x22 fill=\
-\x22currentColor\x22/>\
-\x0a    <path d=\x22M \
-5.414,4 4,5.414 \
-6.586,8 4,10.586\
- 5.414,12 8,9.41\
-4 10.586,12 12,1\
-0.586 9.414,8 12\
-,5.414 10.586,4 \
-8,6.586 Z\x22 fill=\
-\x22#fff\x22/>\x0a</svg>\x0a\
-\
 \x00\x00\x02\xfe\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a       d\
 =\x22M 8 2 C 4.6862\
@@ -1413,15 +1066,15 @@
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#232629;\x0a      \
+:#eff0f1;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 13.273438 3.5 \
@@ -1434,14 +1087,86 @@
  L 6.7265625 11.\
 419922 L 14 4.22\
 07031 L 13.27343\
 8 3.5 z \x22\x0a     c\
 lass=\x22ColorSchem\
 e-Text\x22\x0a     />\x0a\
 </svg>\x0a\
+\x00\x00\x02[\
+<\
+svg version=\x221.1\
+\x22 viewBox=\x220 0 1\
+6 16\x22 xmlns=\x22htt\
+p://www.w3.org/2\
+000/svg\x22>\x0a    <s\
+tyle type=\x22text/\
+css\x22 id=\x22current\
+-color-scheme\x22>\x0a\
+        .ColorSc\
+heme-NeutralText\
+ {\x0a            c\
+olor:#f67400;\x0a  \
+      }\x0a    </st\
+yle>\x0a    <path c\
+lass=\x22ColorSchem\
+e-NeutralText\x22 d\
+=\x22m8.0065001 2.0\
+000269a0.7500188\
+1 0.74999832 0 0\
+ 0-0.6772669 0.4\
+14749l-5.2501316\
+ 10.499976a0.750\
+01881 0.74999832\
+ 0 0 0 0.6712668\
+ 1.085248h10.500\
+264a0.75001881 0\
+.74999832 0 0 0 \
+0.671266-1.08524\
+8l-5.2501312-10.\
+499976a0.7500188\
+1 0.74999832 0 0\
+ 0-0.6652667-0.4\
+14749z\x22 fill=\x22cu\
+rrentColor\x22/>\x0a  \
+  <path d=\x22m7 5v\
+4h2v-4zm0 5v2h2v\
+-2z\x22 fill=\x22#fff\x22\
+/>\x0a</svg>\x0a\
+\x00\x00\x01\xd1\
+<\
+svg version=\x221.1\
+\x22 viewBox=\x220 0 1\
+6 16\x22 xmlns=\x22htt\
+p://www.w3.org/2\
+000/svg\x22>\x0a    <s\
+tyle type=\x22text/\
+css\x22 id=\x22current\
+-color-scheme\x22>\x0a\
+        .ColorSc\
+heme-NegativeTex\
+t {\x0a            \
+color:#da4453;\x0a \
+       }\x0a    </s\
+tyle>\x0a    <rect \
+class=\x22ColorSche\
+me-NegativeText\x22\
+ x=\x222\x22 y=\x222\x22 wid\
+th=\x2212\x22 height=\x22\
+12\x22 rx=\x222\x22 fill=\
+\x22currentColor\x22/>\
+\x0a    <path d=\x22M \
+5.414,4 4,5.414 \
+6.586,8 4,10.586\
+ 5.414,12 8,9.41\
+4 10.586,12 12,1\
+0.586 9.414,8 12\
+,5.414 10.586,4 \
+8,6.586 Z\x22 fill=\
+\x22#fff\x22/>\x0a</svg>\x0a\
+\
 \x00\x00\x02^\
 <\
 svg width=\x2216\x22 x\
 mlns=\x22http://www\
 .w3.org/2000/svg\
 \x22 height=\x2216\x22 vi\
 ewBox=\x220 0 16 16\
@@ -1636,261 +1361,244 @@
  color-interpola\
 tion=\x22sRGB\x22 text\
 -rendering=\x22auto\
 \x22 fill=\x22#8542c2\x22\
  shape-rendering\
 =\x22auto\x22/>\x0a</svg>\
 \x0a\
-\x00\x00\x0em\
+\x00\x00\x0dY\
 \x00\
-\x00L\x90x\xda\xdd[\xe1S\xdc\xc6\x15\xff~\x7f\xc5\
-&\xfd\x02\xd33\x0c\xd2\xe5\x06{z\x1dc\xc0\x94b\
-\xc0\x13H3\x1e\x0f\xc3,w{ \xa3\x93n$\xdd\
-\xf9\xe0\x13\x86\xc4u\x9c\xa4cw\xec6IIR\xdb\
-\xb8\x99\xa4\x19l\xa7q\x82\x13\xdb\xf9@\xfa!_\xc8\
-\xf1\x0d\xbe\x9d\xeb\xa4\xb1\x13:\xfd\x17\xfaV\xd2J:\
-i\xa5\x13p`\x9a\xcc8\xec\xee{\xfb\xf6\xf7v\xdf\
-\xbe\xf7V\xbbw\xba?\xab*ht\x8a\x14\xc8Xb\
-\x08\x17H\xe6\x98F\xc8,\xe9\xc1\xda\xb4Y?\x8d\xb5\
-\xb1\xcc\xe6\xf9\x8d\x7fl^\xdc|\x15m\xdc\xda\xf8`\
-sa\xf3\xbcM\xd2\x8d1\x9b\x1fy:\xcc\xb2\xc6$\
-2V\xef+9TX\xfd\xac<[\xb2\xa8\x13\x93N\
-\x97\xea\xf5\xf5\x8b\xd5\xfb\xd5\xbb\xd5\x07\x16)\x8b)I\
-\xd21\xca\xabz\x16\xb3\xc6\xa3e,\x13%+q\xa9\
-\xba#m\xb4\x80\xcb\xab\x1fZ\xcd9\xcc\xc1\x95#\xac\
-\xf1POI\x99&\xb2\xd5L\xe4\xb1\xcc\xda\x8d\xb5/\
-\xd6\xbe\xfa\xf6\x95\xb5\xbbk\xf7\xd6\x1e|\xfb\x06\xb2\xf8\
-l\x06e\xbc\xef\x18G\x1e\xd1\x19 \xc0S\xd2T\xbb\
-\xd5\x9d\x12\xa3T`\x22JN\xa3$\x97\x14\x1b|^\
-\xe2H\xcdkN\xa3\xae\x16&4[\xc2dn,3\
-,\x19\x04O\xa2\xdc\x94\xaae\xa7l\x19\x93\xb2\xc3N\
-<(\xa6@tm\xe9\xe3\xda\xcd7kK\xb7k7\
-\xe7jK\x8b\xb5\xa5\xfb\xa8\xb6t\xad\xb6\xf4\xd0l\x02\
-\xc2U\x9b\xb7\xc4\x81!\xf1fP\xca9\x8d}D\xc6\
-E\xbb\xd5\xd2xv\x16#\x0f\x823\xae\x80\xc7\x0bs\
-\x8f\x17\xee?\x9e\xbfeQ\xa6y\xa2\xa7\xd5\xb1\xcc\xd6\
-\x9f>\xfd\xe9\xf2\xa5\xadw>\xad\x9b~\xd93\xa1\xb8\
-\xa0\x97t\xabY\x919R\x14\xc5i,\xac\xae\xb0\xd6\
-\x22\xb0vK\xa4\xa0`\x10<3k\xcf\x5c\xd1`\xcb\
-\xd7Ka;\xad\xe3\xc7^\xe4H\xd6T\x93{\xf6\xeb\
-\x85$Z]V\x8c\x92B\xb2\xd8\xb0i%\xd7\xe0\xd7\
-\xe7\xd7/\x83M?X\x7f\xbdz\x0fU?\xa9\xde^\
-\x9f\xab\xaeToC\xc3\xbc\xc5\xacO\x8feLS}\
-\x80\xca\xab\xd7\x14\xd5\x96\xaf\x03\xc6\x11\x5c\x94\xb2\x18\xb5\
-\x18\x14j+j\xf1\x80h\xb5\xb9\xc08\xaa\xefW\x1f\
-\x82\xe0\xbb\xeb\xf3\xa6\xf0\xdb\xeb\xe7\x11-\xd2A\xab+\
-\x8c\xed\xa8t\x86L\xe3\xb2\x84\x95mw\x90\xb1!A\
-\xaf\x93j\x99\x18X\xc3Y:\xeb\x8a\xe4\xf0E\x92\xcb\
-\x9e\xe9\xff\x8cM\x9d\x01\xeb][\xfe\xa8\xb6\xfcUm\
-\xf9v\xed\xd6\x5cmy\xa5v\xebMT[\xbej\xd6\
-\xcf\xd5\x96\x97k\xb7.\xd8\xbc\xe0\x1d\xaa\xef\x02\xc6s\
-0k\xf7\xab+\x14\xe9Cs\x0a\xbf\xb0\x19`\x06z\
-uI1$4\xa0\xce\xd8>\xa5\x04sZ\xbd\x0e\x8e\
-\x84\xaat\xbb\xcez\xca\xee\x1e\x1b}\xf4\xe5e\x1bh\
-\xe5\x90A\xa8\xef\xaaT<s\x5c\xa9X\xc4\xd9\xa9\xf1\
-\xee!\xa7\xd7\xf7\x0f\x97\x9f\xde\xf8\xc3\xbf?\xbf\xf3\xe4\
-\xb5O\x1c\xfa\xe8\xcb\xf5&\x92\xe8V\x0b\x05\xa2\x18\xde\
-F41\x83\x8c)\x82\x06zz\xd1\xefz\xfa\x18\x0b\
-\xdf\x9f\xa2\xcdW\xdd\xffm|\x0c\x85\x0b\x1b\xf76>\
-D\x1b\x1fm\xdc\x85\x0ae\xdd\x5c\xd8\xb8\xb5y\xd1\x15\
-\xe3\xf3\xbd\xa8\xa8\xcat\x1c\x943\x87t\xf9f\xdd\x09\
-0\x9d\xb1\x8d\x07\x19\xdf\xbc\xad}\xf3v^Rr\xdf\
-\xbc\xad8\xec\x5c\xf7\x8c`\x0d\xe6\x03\x8a\xf8\xdcu\x12\
-e5\x82\x0dT$\x0c\x87\x5c\x07$\xcc\x91\x07\xfb\xd5\
-w\xd3\xeb\xd5Ts\x01 >o\x8fp>\xc8\xe2\xf7\
-\xfd\xa8\x0ca/G\xb4\x00gD8@kw\xbe\x9d\
-\x83\x1a\x10\xbe\x0a\xf6\x0bD\x890\x03\xf0\xc7\x0dX9\
-\x0e\x8c\xfa0\xc2\xe8\x87d\xc3e\xf1\x05\x95$c\x9a\
-FdR\x82 \xc3\x18}q\x86\xb1\x1d\x91\x8d\xd5%\
-\x97\xc9\x1fw\x92\xa8\x88\x83\xb8\x02\xf1\xc6^\xaf:&\
-+\xfa\x5c\xad\xdd\xfc=\x0d84\xfa\x5c\x80\xd0s\xd7\
-,]\xb3\xa3\xd1\xcd9h\xfa\x9b\x19\x87\xee\xda1i\
-\xe9!\x8a\x11\xb3\x9cAJ\xbeUw\xe6\xc8\xf8\xe7e\
-\xd9a\xf3\x052\xeaU\xe9\xd4\x0fOP\xf4\xa4\x15\xcc\
-NCrP\x05\x7f\xa8C\xaaL\xa6\x82\x5c\xbe\xd0\xc7\
-\x8c\xbe\x8e\x89FB\xb6\xe9\x1e\x9f\xfb\xfb\xe3\xf9\x0b\x8f\
-\xe7_G\x81\xd8\xc8\xd8}\xe1\x11=o\xf7}\xfe\xd0\
-\xa3\x85k\x8f\x16\xfe\xf8h\xe1\xd2\xa3\x85E\x97]\xb5\
-\xa4o\xbd\xbe\xf8\xe3\xeds\xe8\xa7+W\xb6\xde\xbb\xb4\
-\xf5\xee\x0a\xfa\xf1\xf3\x95\x9fn\xdc\xdb\xfa\xf3\xa5\xadW\
-\x16\xd1\xd6_\x17\xb7\xde\xbb\xfc\x9f\xabP\xf2\x07Y&\
-(\x10ga\xfd'qP\x1d_\xe0E9\x15\xcc\x97\
-c\x04\xfeX\x8c\xf2\xda\xea\xcd\x00\x97?6#\x5c2\
-TM7\xce\xe2 k}\xc0\x86\xc9\xc6\x96\xc3P\xeb\
-\x1cF0\x82S\xd7\xa2\x06\xc4\xf1#z\x92\xa7\x0a\x0d\
-\xf0\xe0\x0d\xc3\x02;[K\xae\x97\x0c\xc4{\x9e\x07\xd3\
-\xe5\x86N\xce\x1f[\x11.S\x9e#:*Kz\x89\
-\xc82\x06\xe4\xba4\xa9Lj\xa5b\xd1\xe9\x16\x11P\
-\x11\xa0\xff<0\x0e\x0d\xb0\xb4\xad\x0f\x06\xd1\xc1\x9aG\
-\xb1\x8e\xb5\xaf\xef\x14P\x9fV\x9a()9\xac o\
-\xfce\xddh\x08\xf6h\x90\xa4\xc2?ac\xa1\x7f\xcd\
-]\x09\x0c\xe4\x8f\xccI{!\xeb\x98\xb8\x81\xda\xe7X\
-!n3\xf6\xf0\xd0\xfd\xdd\xca\x97O\xaf\xbf\xf5\xdf\xfb\
-o\xfcp\xe5\x8e\x13\x02[\x9e|p\xfe\xc9\x07\xaf=\
-Y~\xf8d\xf9\xda\xf7\x7f\xb9\xfe\xf4\xad\xf7[\x91]\
-\xbb\xf0\xd9w\x0f\x16\xbd\x82i\xcc\xf7v\xfe~\xf1\xad\
-\xa7\xef\x5c|r\xe3\x01\xf0\xfd\xf0\xce+\xa8.\x1f\xe8\
-\x91\xf4\xa2\x8cgzH\xd1\x98\xca\x88B\x22\xd1\xafL\
-\x11M2\xf4\xcc\x84\x95(NIYUV\xb5D\xa2\
-\xb7\x82\x0bE\x99d\xf2\xaa\x0c\xe1(\x918\xae\xca\xb2\
-zV\xef\xa6\xd4\x91,=\x97e\x0c\xadD@$\xd1\
-\xa7\x0d\xb5\xd8C\xf2\xb8$\x1b\x99T'k\x19\x91f\
-\x89\x9e\xe9H'\x05!)\x0a\xc9Tg2\x9dJv\
-\x08\x9dI\xe1\x85tbTU\xe5\x09\xac\xb1^\x82\xc0\
-Z\x02\xbd\x12\x83XR\x82\xec\x9e\xd6`\x97\x91\x02\x96\
-e\xc6\xdc\x91\xb6\xeaA\xb6\x93X!\xb2\x07\xb8Y\x8f\
-\x84\xdd#aY\x9dd]`\x02\xad\x86\xc8>\x09X\
-\x99C\xbd\x15\x83(\xba\xa4*z\xa6M/O&\x12\
-\xbfp\xfeC=\x92F\xb2\xe0]$\xa2{\x9bU\x0d\
-&\x9e\xe4\xa8U\x81\x03 \x93\xaa6\x830$JX\
-.N\xe1\x09b@N.\xcb3tM\x9d\xee\x19\x9c\
-5\xe8\x18\xed\x1dB\xd2)\xa6\x9d\xa2\xe0\xb6\x0a)\xa7\
-(\xba\xad\x00\x9c\x15A\x01\xacH\x05\xec\x0aqkT\
-N\xb1h\xb5\xd2\xbf\xac.\xda\x7fALQ#y@\
-\xafd\x89I\xf6V-.\x99\x18L\x80Y\x14\xdcV\
-\x8a\xc2.R\x14\x8cWp\x9baZ\x93\xf6\x9cH\x96\
-\xc4\x1c)KT8HdE\xc1m\x051\xa40!\
-\x93\x82\xde\xde\xe9\x94\x80\x95\x15\x81\x95\x14T\xc3\xeaT\
-\x90\x0a\xc4\x98)Z\xc2\xdcJ\x1dE\xf4V@:l\
-*{t\xbbDu\xb6J\xa2S\xa2\xd3b\x95\x0e;\
-|\xd0W7\xb0Q2\xfb\xda%\xe8\xcbJ\x0eUt\
-\xda@\x8a]J\xbbk\xa8\xcf\x14&TY\xca:\x1a\
-;\x0dLE\xa7\xc1\x1e\xd8\xa9\xdb\xc2X=1\x02f\
-Er\x5c\xa3J\x1f\x15*\x1e\xbb:*V<\xa6\xe5\
-\xa5A\xcdKK\xd5\xd1R^\x9aX\xd7O\xb4\xfay\
-\xed\xce$\xd75P\x0e\xcb\xfaL\x9a]d\xad6\x10\
-\xbb\x08\xad\xaeeP\x82\xa7\xe6\xa1Y\x9d<5\xa0\xb9\
-fBi\x9e\x9a\x87f\xf5\xf3\xd4L\x9amH\x16\x89\
-U\x80\xe25,J\xac\xab\xd7\xd1\xad\xceuu\xa0;\
-FF\x89n\xc5\xa5X\xdd\xdc\x0aP\x1c\xe3\xa2\x14\xb7\
-\xe2R\xac>nE\xac\xd4\xf9\xa6.keB\xfc\x92\
-\x0e~\x0f\xd8;\x84J\x87\x80\x0e\xa1\xe3R\x05\xdai\
-#\xad@\xfa\xd5\xafL\xc3I\xaaH\x12\xa7]\xc74\
-\x96\xa0\xde2\xd3!@\x10S\x0cR12l\x8cQ\
-\xd05c\xca\xa02\xd3\x95\x8e4OfI\x87s\x85\
-\x02-9\x02\xbe\xbfEoE:\xf5\xee\x90.\x1bV\
-8\xa0M\xbf~\xee\xb9\xe7\x86\x87N\x9c\x82?\xbf:\
-\x82H\xdbd\x1b\x1a\x00\x7f\x81\x0aj\x19\xc3b\xb1\xde\
-\xedv\x17\xd4\xa2\x13\xace\xa7L\xff\xaa\x11s\x06\xe1\
-\xfcW\xd2\xc0e\xc1\x09PS\xcf\xc0fH\x22bd\
-\xdbZA\x7f\xf4\xdb\xd242 `B\x8eC\xce\x02\
-\xae\x9e\xe1\xf1\xa1\xe1\xd1\xf1\x97Fz\xc7\xbb\x86N\xbd\
-\xfc\x9b\xde\x17{\xc7{O\x8c\xf4\x02iPU\xd4\xec\
-\x94\xa6\x16\xbc\x93\x90f\x93\x90\x8e1\x09\xb0>?\xdb\
-y\x00\xdd\xdc\xa90=O&\x8e]\x80\x95\xfe|\xa7\
-D\x0cL\x89\x18=%\x82P\x11\xb8\xdb\x8f\xa9\x009\
-\x9d\xa2\xd7)\xbe}`\x02\xdb\xb8\x82\x10\x03M\x88\xcd\
-6\x17\x90k<\x80)\x96\xf1X\xd8\xc4\xfd\xc0&\x06\
-\xb05Z\xc5TEH\xf9\x81\xf5\x8d\x0e4\x07P\x8a\
-\xa1I\xc5@\xc1Y\xbd\xe6\x01\xf1\xacZ*\xe6\xaa\x99\
-\x98\xc4\xbd\xc4$\x0605X-Q\xa8\x88{\xbe\xe7\
-D\xb6\xe7\xc4\x90\x19\xa2P\xa9\xd3J\x0cJ\x0ac\x1c\
-\xc4\x15K\x13z\xf4\xb0p\xee\xc3n\x14=\xbbQl\
-\xb0\x1b\xe3\xa2\x16\xf7\x03\xb5\x18@-\xee\x14u\xaa\xb3\
-\x92\xea\xdck\xc8\xa9N\x1b/\x9cW\xe3\xe14\x8f\xd0\
-^\x9c\xe9T%\x9d\xdak\x9ci\xe6q\xd2\xa9\x9d\xce\
-\xa7'\x0bu\x0e\x00\x0d\x12Q^\xd2\xd8\x05\x87F8\
-+\xd3\xee\xa6f4\x09\xc8\x83\xb6=*\x1c\xa4\xddt\
-\x018\x87O\x8e\xf6\x0f\x0fu\x9d@\xbf\x8c\xad\xad\xf7\
-d\xc2I\xea\x5c\xdc\xb1\xf2\xba}\x83\x1a\x9dwE\xa2\
-\x16\x9f!\xea\xc8\xd4(\x045\xcb\x8e\x1c{;]\xf7\
-%\x83\x93\xd5\xf8\x04\x05\x0cU\x880T8w\x1e4\
-\x13\xb5\x0e\xc8\x1c\xe3t\x07=\x08\xe6\xe9\x1c\xe9#\x0c\
-\xb3\x01b\xf1\x99 \x8e4\xcaP\xc4\xdc\xa4\xfdeU\
-\x9b\xc6\x9aZ\x82\xa3\x86\x17\xad\xe7\xf42Q2\x0c\x8b\
-`\x9e\x5c\x98\x1e\xc3E\xa2\xa0Q\xa2\x15$\x05\xcb\xed\
-]\x13j\xc9`4\xbbF?\x0f[\x9du:\xd0\x8b\
-\xc3C}\xe3\xfd\xdd\xc3C\xa0fW_\xef\xf8\xb1S\
-\xe3]'O\xf24\xe4n\x91h\xb58\xa6s05\
-\x8b>A4PR\xfc\x7fQ2\xf2(\x12\xaadh\
-\x86;2\xa3\x1b\xa4\x80F\x88aH\xca\xa4\xce\xcf\x16\
-\x98\xd3\x04\xe5\xcd;\x91\xbcy}\x00\xfc\xa6$\xfd\x08\
-\xb2\xc4\xb7\xe4\xacO\xe9\xadIdf%I\xd4!t\
-V\xe8\xa7^\x04\xae\xb5\x02\xff\xa23\x0f\xf3:\xc2\xd6\
-\x94\x9b-\x87\xaa\xc7\x925\x07\xa8\xa5\x1c\xf69\x8c\xed\
-+f\x09\xf6(v8]9\x9c6?\x1fXG\xbc\
-\x16E5\x90F\xb2\xe6\x15N\x8e\xe4Z\xe3\xab\xc8M\
-\xfe\x02*6\xce\x00\xd9\xda\xfa\x94?\x80+[\x7fq\
-\x10g\x81\x1b\xe7\x95\xa1\xdfKb\xe9\xbf=\xcc\xdb\xf3\
-\x9e,9\x18V\xe4\x19\xfa5+g\xfa\x8f,\xd6\xe8\
-\x9dQ\x12\xe93\x05YR\xa6\xed\xe6\x81\xc1\x19\xd8\xed\
-d\xc6\xb4\x0d\xfb:%\x18\xe5G\xcc/\xbb>\xff\xe5\
-,\x80\x89\xd8\x94f\xcbp\x85\xf1\x90{\x855N\x8b\
-b\x0d\xc33\xe9\xc8a\xc4\xf0a\x9c\xcc\xcd^9:\
-\xe04\x98&\xbd\x81\xa67\x92\x88\xe4\xf3$\xeb\x1d\x9d\
-wJ\xd9\xe9\xe8\xeeFe\xf7U\xce\xa7\xee\xce\xdd\xd9\
-\xab3\x04\xc7Y\xc1P\xa8\x1d\x9d\x95r\x93\xb4\x14\xb0\
-\xd8\xb8\xbe\x85]\xab\xb15\x7f!\xbd+\x07\xe3f\xc0\
-\xdd\xce5]t^\x1c\x1an\xdc{>\xfe~|\x89\
-n\x13X\xe3\x01);\xad\xe6\xf3\xa8\x85\x86\xcaT[\
-\xa5\xad\xd2j:\xdd\x13\x186\xa2\xac\x1am\xa8K\xd6\
-UkW\x01\xfb`\xd7h\xafI\xef\x96\x14\x05\x17\xc0\
-fZ\xce\x94t\x03\x1d?\xd5\xdf\x1a\xff\xb4[w\x09\
-\x19\xf4N\x1e\xe5\xb7}\xe6\xed\xb1n\xa3vp\x9a\xa0\
-\xb3f~\xf8F\xd6\x8d\xd6\xae\xce\xf3\xee\x85Y\xd0\xb7\
-0\x88^\xe7\x12}i\xb1\x07\xb0\x22O\x0c<\x84\x91\
-W\x08{\x010\xea\x80\xc0\x05\x18\x1a\xa0\x9a\x8e\x8e\xe7\
-\xe4\xc3!\xed\xd7\xa26H\xcc#\x00\x8a\xfb\x060*\
-\xa9\xe6\x02d_\xdd|><\x0aU\xc3T\xcb\x92\xe9\
-I\xb5L/\xba\xc3T\xcb},\x11\x8c\x89u\x1a\x05\
-#\x7f*\xd4\x8b\xf5Zw\xe3\xd1^\xac\xb3\x12\xfcl\
-*\xd1\xab8+\x1f\xb3\xef\xd7\xe3/\x93\xf3\xd6\xc3V\
-\xc4\x0d\xbf\x0cN\x8c\xab\xe6f\x00\xe09\xcdp\x08\xbc\
-\xed\xd5\x1c\x14\x91>2\x02\x90\xb8g\x80\xa2|\x22\x17\
-\x10\xdf'6\x03\x0d\xcf\x07\x86C\xd8\xabEj\xe0\xf3\
-\x22\x00\x89{\x06(\xca\xc7q\x01y\xf7\xbdj\x98>\
--z\xe7sW\xd5\xe9\x1b\xc3m\xb5\xe7elP\xd0\
-\xf6;\x1b\xdeRRR\xbc\x95\xdc\xcd\xc8\x0d\x96/\x0c\
-\x84\xd8\x5c\x10\xd1K\x16\x04\xe1.\xce {m\xb4\xab\
-\x8c3OM\x8f\x8a\xd9U\x9c\xf5\xbe\x8c\x0azP\x8a\
-t\xd4D\xeaQ\x85\xc5\xa2\x8et\xac\x14\xb4\xf98#\
-}l\x5c\xc8\xe2\xfeB\x8e\xf2\xc2\x8d!7HS\x9b\
-\x8d\x97\xb7\xb9} #\xbfI\xa4b\xa5\xb1\xcdG\x1d\
-\xe9\x18v\xa6\x80\xb8\xbf\x0aD9\x95\xed*\x10\xf2\xe9\
-\xb1\x01\xea\xfd\xcd\x84\xbd\xef|\x83\x87z\xee\xc6\x08\xcd\
-\xef\x0f\xa8b\xbc$\xbf\xd1R\xa6\xc3\xd3\xfc\x93\xe6\x9b\
-\xd3\xddE\x0e\xf3\x87\x06\xbb2Z\xe7Ml0f\xd8\
-\x00w\x110\x9a\x08/2T\xc4B*\xee\x17\xd2\xa8\
-\x08\xd1\x00isn8\x07\x06\xb1$#C\xc3\xfa\x94\
-\xd9#\xf6\xed\x97\xf3\x0c:\x185\x82\xc0\x9bxq\xb9\
-{\xc0\x91\x01#\x1c\xbbx \xb0G\xc5\x0a\x1e\xf6\xd0\
-\xef\xbe;4cv\x07\xc3~|\x11\xf4\xdf<\x14\xa1\
-O\xb7\x9a\x82\x82w\xc7\xc1C\x11\xfa0\xab)(x\
-.\x9f\x87\xc2\xba\xaf\x0c\x06\xb2\x08\x0c\x0d\xa3\x98%\xd3\
-\x13\xc5vv\x19\xc8~=c+r\x98\xef\xdf\x03\x81\
-\x0b\xf8\xc2\x02\x97}\xd9\xb3\xb3\xc0\xd5?\x88\xac\x1fN\
-\xec\xca\xd9:\xbf\xca\x88wy\x17\x15\xaa\x9a\x0c\x88\x13\
-\xa7\xc4\x18\xd8\xc4}\xc1&F\xc4P\xee\xa5'/\x1c\
-\xf5{\xdc\x22\x98\x10\x04Pj\xbf\x05\xd2n_\x05\x8f\
-jx\xa6\x0d\x0d\xa9\x06\xfd\xd19\x9c\xcaK2\xd6\xd8\
-\xd5,\xb8G\xabK\xdb\xb6\xe17\xba[m\x14\x94\x9e\
-\x19\xec\xc8\xd0\x14\xae\x81x\x804\x88\x0aP\x5c\x0dx\
-\xef\xf2)l\xfa\xfc\x9c\xbe\xcah\x8b\x1d%\x9d_\xf5\
-\x05\x1f\xe3\xf3F\xe6\x86\xc6g4q\xbc@\xca\xc3\x1c\
-\x1aHs\xe6\x0few\x1a\xc2\x9c\xdf>F?\x16h\
-\x18H\x9b\x82b\xdb\x8f\x06\x02/#P\x9f\x02\x93\x8b\
-\xd8o.-<\x09\xf7\xf14#\x8c\x05\x9eN3\x8f\
-\xc7D\xbb\x17\xef/t\x08\xbe\xe1\xdd+\x9d\xa0<v\
-\xa1\xb3=y\xfe\x1f\x93\x8e\x05>\x07oO\x9e\xef\xb7\
-\xa8c\xfep\xbe=i\xbe_\xb2\x8e\xf9\x17g[\xd2\
-\xbc\xdf\xb2\x87\x8f'\xfe\x07u\xaf\x8ew\
+\x00I\xe4x\xda\xdd[\xffo\x1c\xc5\x15\xff\xfd\xfe\x8a\
+A\xfcP[\xbd\xd8\xf2\xeeqr\xa2^\x15'v\x5c\
+7\xb1\x1da\x03\x8a\x22\xcb\x1a\xdf\xcd\xddmno\xf7\
+\xd8\xdds\xd6\xfe)$\x90\xa6|\xa9\xa0\x0a*P\x03\
+\x0d8EPd\x02UhP\xc1\xfc\x10\xfa\x03\xbf\x80\
+\xf9\xcd\xf9\xedR@$\xe0\xaa\xffB\xdf\xec\xee\xec\xec\
+\x97\xd9\xbd\xb5}v\x5c\x2297o\xde\xcc\x9b\xcf\x9b\
+y\xf3\xde\x9b\x9d\xdd\xb3\x13e]C\xb3u\xd2$s\
+\xb9)\xdc$\xa5c\x06!\xcb\xc4)\x9f\xc5\xc6\x5c\xe9\
+\xce\xe5\xcd\xbf\xdfy\xf6\xce3^\xcd\xf2\x5c\xa8\xc5B\
+-L\x971\xa5\x15\x133\xf2\xe8\x22V\x89VV\x22\
+\xf5f\xb8[\x05Gh\x12\xa6\x89\x1a\xa1\xb5\xf9\xf1c\
+\x91*34\x02\xb1\x22\xecv\x98\xae*\x11\xda\x08\xd3\
+\xb5\xca\x5ciZ\xb1\x08\xaeyt\x04A\x1d\xfawV\
+\xdf\xef\x5c\x7f\xa1\xb3z\xa3s\xfdBgu\xa5\xb3\xfa\
+\xa9\xc7\x8b\x8c\xa5D\xb4S*\x11\x9a\xb8\xd0\x19\x19\x99\
+\x1c\xc5Uey\xd9S\xed\x5cD\x5c#J\xebaZ\
+\x8dL\x85\x16QE\xd3\xc2t\xcb\xe1/\xb1\xe1ZV\
+hb[\xd6\xfc\xb1G\xc3\x1d\x0cg@e\xf9\x8bK\
+\x1e\x1d\xd1\xdfl\xcc\x95\x1e\xbf}M\xd3\x1b\x1e\x0d\x03\
+\xcc\xe0\x96R\xc6\xa8\xcfm\xd7\xef1`\x116\xde\xdc\
+X\xdf\xf8h\xe3\xe67\x177n|s\x01\xfe.3\
+\xdeQ\xe5\x1ci\xe0E\x05k\xd9Z\xa9\xd8R\xa0\xe9\
+i}\x91X\xd8\xc0e\xbfE\x02c1\x8c\xda\x82i\
+\xed\xac\xbd\xd7Y\xfb\xbc\xb3v\xa3\xf3\xc1\x85\xce\xda\xad\
+\xce\x07/x<0\xfb\x8d\xd7a\xd8\xa76nmx\
+\xabn\x01\xf81S\xd1,\xc5\xa5\xdb\x8d\xb0\xbc\xc5\x88\
+\xc5\xd9\x87,b\xc2\xdc\xda\xb6[k\xdbn\xfdr}\
+\xfe\xf8\x14k\x8a\xbe__\xbb\xff\xf6\x1f|\xce\xec\x13\
+\xbe\x90\xdcq\xbd\xd9$\x9a\xc5Z.,!\xabN\xd0\
+\xc9\xd11\xf4\xf8\xe88\xe3\x86\xf60\xba\xf3\xcc\x9d\xcb\
+\xf0\xdf\xe6\xfbP\xb8\xb2\xf9\xc9\xe6\xbbh\xf3\xbd\xcd\x9b\
+@8\xccK\x9b\x1f\xdcy\x96w\xf4\xb7:\x93\x89\xac\
+/_5\xbe|\xb5\xaah\x95/_\xd5\xfc\x86\xdc\x07\
+\xa0\x8d\xf5o.\xc6\x10\xf8>!\x8f\xca\x06\xc1\x16j\
+\x11\xd5\x11W\x81_h\x1ch\x18\xf5\x16\xf1\x1e\xe1\x0e\
+\xfeNAz%6.w*\x08W\xe3\x5c\xdf\xc5\xa0\
+Ep\x81\x15b\xc4\x9ap\xaf\x83\xbe\xfa\xf0\xeb\x0b_\
+?\x8f\xbe~\xfa\xab\xcf\xe3\xcd\x82\xce(i\x19|\xf7\
+\x84Z\xba`$+:\xd7\x87T\x8bs\xfd\xfd\x94g\
+\xec\x06\x225E\xc3~\x13\xee\xceX\x8b#\xaau{\
+\x95\xf3\x0d.\xa2\x85\x0d\xa4\xfe\xe2\xf6\xbbO\xb6\x95\x16\
+\xa1S\x0a!\xa0LZ\x96\x02\xd3P3p\xab\xae<\
+\xd9&\xd1\xa9\xe6\xfe\xcf\xe3\x84\xf0\xbb\xde\xf0\xe5\xce\xf5\
+\xdfuV\xaf9\xde\xf0\x0a\xea\xac\xdetJ\xd7<\xef\
+x\xfd\x02T\xfd\xd5q\x987;\xab\xeb\xd4m\xae\xae\
+#\x81\x0f\xf5\x85\xb6\xf9\xfa\xf9\xd3b\xfd\xeb%\xd5o\
+\xc1\x1d+u$0\xb9\xfd`)\xa0\x5c\x1c w\xb9\
+HWI=\xceg.\x98\x19e\x98\xcb\xed\xacj\xdc\
+\xbe\x16\xe7\xfb\x1eZ\xd8\x9d:l\xb6\x85\xbe}\xeao\
+\xdf^\xbc\xf2\xed\xc5\xe7\x90\xb7\x8dY#\xee\xc5}]\
+\xef^\xbav\xf7\xd2\x1f\xef^z\xf1\xee\xa5\x15\xdeN\
+w\x85m=\xb7\xf2\xe3\x8d\xa7\xd0OW\xafn\xbd\xf1\
+\xe2\xd6\xeb\xb7\xd0\x8f\xff\xb8\xf5\xd3\xdb\x9fl\xfd\xe9\xc5\
+\xad\xa7W\xd0\xd6_V\xb6\xdex\xe9?/\xafD\x87\
+\xe1\xc1\x00\xec\xa0\x86\xe3`\xb5\xc0B\xeb`\xaa\x82\xd5\
+\xe6\x01\x83N\xc7\xf5\x18\xdf\x0f \x08\xb7-\xdd0\xad\
+\xf38\xde\x86E\x15T\xc1\xee\xd6\xd6C\xf6\x16\x0a3\
+t\xff\xeb1\x11<\xec\xe4E(y\x14\x12\xbb%\x1e\
+\x95D\xce\xc3T\xd3\x5c\x0b\x8f\x15\x08/R\xee\x11\x13\
+-*f\x9b\xa8*5\x01S\xa9i5\xa3\xddj\xf9\
+\x1d\xc2\x01\x03m\xdc\xd8\xf8GL(\x0d \xb4n\xfc\
+\xf6\xc7\x86\x09f4\x8bMl|\xf1a\x13\x8d\x1b\xed\
+\x85\xb6V\xc1\x1a\xf2\xe2\x0b\xeb\xc1CL\x9e\x8a\xfc\x08\
+\xa2\xe1:D\xc3[\xe8\xdf\x17\xae\xc6\xc4\xf3\xf8\x93\xf7\
+&;\xc4\x8e\x86\xa3\x88#\x83\xe8\xc4Z\x8a\x02\xd4w\
+\xb7\xfey\xff\xadW\xfe\xfb\xe9\xf3?\x5c\xfd\xd0\x0f\x17\
+}\xf7\xde\xb9|\xef\x9d\xdf\xdf[[\xbf\xb7v\xed\xfb\
+?\xbfu\xff\x957\xfb\x91G]\xf9\xf8\xbb\xcfV\x82\
+\x22id\x0bv\xfe~\xe5\x95\xfb\xaf={\xef\xed\xcf\
+\xa0\xdd\x0f\xaf=\xcd\xec87\xaa\x98-\x15/\x8d\x82\
+\xc3\xaa\x97d)\x97\x9b\xd0\xea\xc4P,\xb3TW\xca\
+\xba\xaa\x1b\xb9\xdc\x98\x8d\x9b-\x95\x94\xaa\xba\x0an=\
+\x97;\xa1\xab\xaa~\xde<N\xb93e\x9a\xeb\x96,\
+\xa3Me\x11\xb3a\xe9\xadQR\xc5m\xd5*\x15\x86\
+Y\xcd\x8c\xb2L\xcc\xd2P1/IyY\xca\x17\x86\
+\xf3\xc5B~H\x1a\xceK\x8f\x14s\xb3\xba\xae.`\
+\x83\xf5\x92$V\x13\xeb\x95\x9b\xc4\x8a\x16o\x1e\xa8\x8d\
+w\x99ibUe\x8d\x87\x8a.\x1dov\x1akD\
+\x0d\x00w\xe8T\xd8\xa3\x0aV\xf5\x1a\xeb\x023\xe7V\
+\xa4\xf6\xc9\xc1j\x1c\x1a\xb3-\xa2\x99\x10\x1d\xcc\xd2\x80\
+\xb9X\xcb\xe5\x1e\xf6\xff\xa1Q\xc5 e\xd8\xe3\x0a1\
+\x83\xd5\xba\x01\x13O*\xd4\x86\xca\xd8\x225\xddXB\
+X\xab \xac\xb6\xeax\x81X\x90\xfa\xa9\xea\x12]L\
+\xbf{\x09\x97i\x042\x07\x87\xa4\xbc_,\xfaE\x89\
+\xd7J\x05\xbf(\xf3Z\x00\xce\x8a\xa0\x00\xd6\x94&\xe6\
+B8E\xe5\xb4Zn-\xfde\xb4\xec\xfd\x82\x98\x96\
+A\xaa\x80\x1eb\xa2\xc3\x0e\x92n+\x95XL\x80S\
+\x94x-E\xe1\x15)\x0a\xd6V\xe2\xd50\xadyo\
+N\x14Wb\x85,*T8HdE\x89\xd7\x82\x18\
+\xd2\x5cPI\xd3\x1c\x1c\xf6K\xd0\x94\x15\xa1)i\xea\
+\x96\xdb\xa9\xa94\x89\xb5\xd4r\x85q\x22\xc4\x91\x83\x04\
+H\x87\xdd\xe4\x8d\xee\x95\xa8\xcenI\xf6KtZ\xdc\
+\xd2a\xbf\x1d\xf45-l\xb5\x9d\xbe^\x09\xfa\xb2\x92\
+\xcf\x95\xfd:\x90\xe2\x95\x8a|\x0d\xcd\xa5\xe6\x82\xae*\
+e_c\xbf\x82\xa9\xe8Wx\x03\xfb\xb4'\x8c\xd1\xb9\
+\x190+R\x11\x1aU\xf1\xa8d\x07\xec\xea\xa8l\x07\
+L+\xc8\x03*\xc8+\x84x\x85 O\x0e\xf5\x93\xdd\
+~A\xbbs\xd8\xa1\x0a\xda\xc2\xb5>\x87\xe7\x15Y\xad\
+\x07\xc4+B-\xb7\x0c\xca\x08P\x01\x9e\xdb)@\x01\
+\x8f\x9b\x09\xe5\x05\xa8\x00\xcf\xed\x17\xa0\x1c\x9egH.\
+\x8b\x11\xc0\x09\x1a\x16e\x86\xe8\x10\xdf\xed\x1c\xa2\x81\xef\
+\x1b\x19er\x82s\xdcn\x9c\x00\x8eo\x5c\x94\xc3\x09\
+\xceq\xfbpB\xb6C\xbei\xc4]\x99\x04\xbfd*\
+4\x9a<<$\xd9C\x12:\x84N(6\xd4\xd3J\
+J@\xde3\xa15\xcc2n\x91\xdcY\xee\x98\xe6r\
+\xd4[\x96\x86$\x08\x5c\x9aEl\xab\xc4\xc6\x98\x05]\
+K\x8e\x0c*\xb3h\x0f\x15E2\xdb\x90_*\x1a\xd4\
+T\x08\xf8\xfe>\xb3\x1f\x99\xd4\xbbC\xcaj\xb9\xe1\x80\
+V\xfd\xfa\xa1\x87\x1e\x9a\x9e:u\x06~~u\x04\x91\
+\x81\xda\x00:\x09\xfe\x025\xf5E\x0c\x8b\xc5z\x0fz\
+]P\x9fI\xb0Q\xae;\xfe\xd5 \xce\x0c\xc2\xb1\xa9\
+m\x80\xcb\x82\x83\x93\xa1\x9f\x83\xcd\x90G\xc4*\x0f\xf4\
+\x83\xfe\xe8\xb7\xed\x06\xb2 \x96B\xbeB\xce\x03\xae\xd1\
+\xe9\xf9\xa9\xe9\xd9\xf9\xc7f\xc6\xe6G\xa6\xce<\xf1\x9b\
+\xb1G\xc7\xe6\xc7N\xcd\x8c\x01kR\xd7\xf4r\xdd\xd0\
+\x9b\xc1I(\xb2I(f\x98\x04X\x9f\x9f\xed<\x80\
+n|*\x1c\xcfS\xcab\x17`\xa5?\xdf)\x91c\
+S\x22\xa7O\x89$\xd9\x92p\xfb1\x15 \xa7\xd3\xcc\
+\x90\xe2\xdb\x07&\xb1\x8d+I\x19\xd0$\xd8lo\x01\
+q\xe3\x01L\x99\x8c\xc7\xc5&\xef\x0769\x86\xad\xdb\
+*\x16l\xa9\x10\x056>{\xb27\x80\x0a\x0cM!\
+\x03\x0a\xc1\xea\xf5\x0eH`\xd5\x0a\x19W\xcd\xc1$\xef\
+%&9\x86\xa9\xcbj\xc9\x92-\xef\xf9\x9e\x93\xd9\x9e\
+\x93\x13f\x88B\xa5N+7\xa9h\xac\xe1$\xb6]\
+M\xe8\xd1\xc3\xc5\xb9\x0f\xbbQ\x0e\xecF\xb9\xcbn\xcc\
+\x8aZ\xde\x0f\xd4r\x0c\xb5\xbcS\xd4\x85a\xbb0\xbc\
+\xd7\x90\x0b\xc3\x1e^8\xaff\xc3\xe9\x1c\xa1\x838\x8b\
+\x05\xbbX\xd8k\x9cE\xe6q\x8a\x85\x9d\xceg \x0b\
+\xf5\x0f\x00]\x12QQ\xd28\x02\x87F8+;\x8f\
+f\xa9f4\x09\xa8\x82\xb6\xa3:\x1c\xa4y\xba\x00-\
+\xa7O\xcfNLO\x8d\x9cB\xbf\xcc\xacm\xf0d\x22\
+H\xea8\xeeLy\xdd\xbeAM\xcf\xbbRQ\xcb\x0f\
+\x10ujj\x94\x80\x9aeG\xbe\xbd\x9d\x0d=\xc9\x10\
+d5\x11A1C\x95R\x0c\x15\xce\x9d\x07\xcdD\xdd\
+\x03\xb2\xc08\xf9\xa0\x07\xc1<\xfd#}\x8aavA\
+,?\x10\xc4\xa9F\x99\x88X\x98\xb4?\xa1\x1b\x0dl\
+\xe8m8j\x04\xd1\x06N/\x0bm\xcbr\x19\xce\xc9\
+\x85\xe91\xdd\x22\x1a\x9a%FS\xd1\xb0:8\xb2\xa0\
+\xb7-\xc6\xf3(\xfaH\xd8\xedl\xd2\x81\x1e\x9d\x9e\x1a\
+\x9f\x9f8>=\x05j\x8e\x8c\x8f\xcd\x1f;3?r\
+\xfa\xb4HC\xe1\x16IWK`:\x07S\xb3\xf4\x13\
+D\x17%\xe5\xff\x17%S\x8f\x22\x89J&f\xb83\
+K\xa6E\x9ah\x86X\x96\xa2\xd5Lq\xb6\xc0\x9c&\
+(\xef\xdc\x80T\x9d\xeb\x03h\xefH2\x8f W|\
+_\xc5}\x94\xde\x9fGNV\x92GC\xd2\xb0M\x1f\
+\xf5\x22p\xad6\xfc\xa5g\x1e\xceu\x84\xa7\xa90[\
+NT\x8f%k>PW9\x1cq\x18\xdbW\xcc\x15\
+\x1cP\xecp\xd1>\x5ct\x1e\x1f\xb8G\xbc>M\xb7\
+\x90A\xca\xce\xb5M\x85T\xfa\xb3\xab(L\xfeb*\
+v\xcf\x00\xd9\xdaF\x94?\x80+\x1b\xbe8\xc8\xb2\xc0\
+\xdd\xf3\xca\xc4\xe7%\x99\xf4\xdf\x1e\xe6\xedyO\x96\x1c\
+Lk\xea\x12}\x9aUq\xfcG\x19\x1b\xf4\xce(\x8f\
+\xcc\xa5\xa6\xaah\x0d\xaf\xfa\xe4\xe4\x12\xecv\xb2\xe4\xd8\
+\x86w\x9d\x12\x8f\xf23\xce\x93\xdd\x88\xff\xf2\x17\xc0A\
+\xecH\xf3dpa\x22\xe4Aa\xdd\xd3\xa2L\xc3\x88\
+L:u\x189y\x18?s\xf3V\x8e\x0e\xd8\x00\xd3\
+\xa4\xb7\xc9\xf4F\x12\x91j\x95\x94\x83\xa3\x8bN);\
+\x1d\x9doTv_\xe5?\xea\x1e\xde\x9d\xbd\xfaC\x08\
+\x9c\x15\x0c\x85\x06\xd1y\xa5R\xa3\xa5\x98\xc5f\xf5-\
+\xecZ\x8d\xad\xf9#\xc5]9\x18\x9e\x01\x1f\xf7\xaf\xe9\
+\xd2\xf3\xe2\xc4p\xc3\xef\xf9\xc4\xfb\xf11\xbaM`\x8d\
+O*\xe5\x86^\xad\xa2>\x1a*\x0b\x03\xf6\x80\xdd\xef\
+8\xddS\x186\xa2\xaa[\x03hD5uwWA\
+\xf3\xc9\x91\xd91\x87\x7f\x5c\xd14\xdc\x04\x9b\xe9;\xd7\
+6-t\xe2\xccD\x7f\xf6\xd3n\xe8\x122\xee\x9d\x02\
+\xcao\xfb\xcc;\xea\xdeF\xed\xe04Ag\xcdy\xf0\
+\x8d\xdc\x1b\xad]\x9d\xe7\xf9\x85Y\xdc\xb70\x88A\xe7\
+\x92~i\xb1\x07\xb0RO\x0c\x22\x84\xa9W\x08{\x01\
+0\xed\x80 \x04\x98\x18\xa0z\x8eN\xe4\xe4\x93!\xed\
+\xd7\xa2vI\xccS\x00\xca\xfb\x060-\xa9\x16\x02d\
+O\xdd\x22><\x0dU\xd7T\xcb\x95\x19H\xb5\x1c/\
+\xba\xc3T\x8b\xbf,\x11\x8f\x89!\x8d\xe2\x91\xbf\x90\xe8\
+\xc5\xc6\xdc\xbb\xf1t/6l\xc7\x1f\x9b*\xf4*\xce\
+\xcd\xc7\xbc\xfb\xf5\xec\xcb\xe4\xbf\xeb\xe1)\xc2\xc3/\x83\
+\x93\xe1\xaa\xb9\x17\x00DN3\x19\x82h{\xf5\x06E\
+\xaa\x8fL\x01$\xef\x19\xa04\x9f(\x04$\xf6\x89\xbd\
+@#\xf2\x81\xc9\x10\xf6j\x91\xba\xf8\xbc\x14@\xf2\x9e\
+\x01J\xf3qB@\xc1}\xaf[\x8eOK\xdf\xf9\xc2\
+U\xf5\xfbfp[\x83U\x15[\x14\xb4\xf7\x9e\x8dh\
+))+\xdbJ\xeef\xe4.\xcb\x97\x04B\xee-\x88\
+\xf4%\x8b\x83\xe0\x8b3\xc9\xde6\xdaU\xc6Y\xa5\xa6\
+G\xc5\xec*\xce\x06\xdf\x8c\x8a{P\x8at\xd6A\x1a\
+P\x85\xc5\xa2\xa1b\xa6\x14\xb4\xf78S}lV\xc8\
+\xf2\xfeBN\xf3\xc2\xdd!wIS{\x8dW\xb4\xb9\
+# S\x9fI\x142\xa5\xb1\xbdG\x9d\xea\x18v\xa6\
+\x80\xbc\xbf\x0a\xa49\x95\xed*\x90\xf0\xe8\xb1\x0b\xea\xfd\
+\xcd\x84\x83\xef\xf9\xc6\x0f\xf5\xc2\x8d\x91\x98\xdf\x1fP\xc5\
+DI~\xb7\xa5,&\xa7\xf9\xa7\x9dwNw\x179\
+\x9c\x0f\x0dve\xb4\xfe;\xb1\xf1\x98\xe1\x01\xdcE\xc0\
+\xe8!\xbc\xd4P\x91\x09\xa9\xbc_H\xd3\x22D\x17\xa4\
+\xbd\xb9\xe1<9\x89\x15\x15Y\x066\xebN\x8f\xcc\xb7\
+_\xfek\xd0\xf1\xa8\x11\x07\xde\xc3\x8b\xcb\xdd\x03N\x0d\
+\x18\xc9\xd8\xe5\x03\x81=-V\x88\xb0'>\xf7\xdd\xa1\
+\x19\xb3;\x18\xf6\xf1E\xdc\x7f\x8bP$\xbe\xba\xd5\x13\
+\x14\xa2;\x0e\x11\x8a\xc4\x17\xb3z\x82B\xe4\xf2E(\
+\xdc\xfb\xcax K\xc1\xd05\x8a\xb92\x03Qlg\
+\x97\x81\xec\xeb\x19O\x91\xc3b\xff\x1e\x0b\x5c\xd0.)\
+py\x97=;\x0b\x5c\x13\x93\xc8\xfdpbW\xce\xd6\
+\xff*#\xdb\xe5]Z\xa8\xea1 A\x9c\x923`\
+\x93\xf7\x05\x9b\x9c\x12C\x85\x97\x9e\xa2p4\x11p\x8b\
+`B\x10@\xa9\xfd6\xc9\xa0w\x15<k\xe0\xa5\x01\
+4\xa5[\xf4\x83o8\x95\xb7Ul\xb0\xabYp\x8f\
+n\x97\x81m\xc3\xefv\xb7\xda-(=0\xd8\xa9\xa1\
+)Y\x03\xf9\x00i\x90\x16\xa0\x84\x1a\x88\xde\xcb\xa7\xb0\
+\xe9\xeb\xe7\xf4\xad\x8c\x81\xccQ\xd2\xff\xaa/\xfe2\xbe\
+hdah|@\x13'\x0a\xa4\x22\xcc\x89\x81\xb4\xe2\
+|(\xbb\xd3\x10\xe6\x7f\xfb\x98\xfe\xb2@\xd7@\xda\x13\
+\x14\xdb~i \xf6f\x04\x1a\xd7`r\x11\xfb\xe6\xd2\
+\xc5\x93\xe3/O3\xc6\x5c\xec\xd5i\xe6\xf1\x98h~\
+\xf1\xfe\xc8\x90\x14\x19\x9e_\xe9\xc4\xe5\xb1\x0b\x9d\xed\xc9\
+\x8b~L:\x17{\x1c\xbc=y\x91oQ\xe7\xa2\xe1\
+|{\xd2\x22_\xb2\xceE\x17g[\xd2\x82\xcf\xb2\xa7\
+O\xe4\xfe\x07\xca\xb23\xc4\
 \x00\x00\x03q\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      .ColorSc\
 heme-NegativeTex\
 t {\x0a        colo\
 r:#da4453;\x0a     \
  }\x0a      </style\
 >\x0a  </defs>\x0a  <p\
 ath\x0a     style=\x22\
@@ -1942,15 +1650,15 @@
 fs>\x0a        <sty\
 le type=\x22text/cs\
 s\x22 id=\x22current-c\
 olor-scheme\x22>\x0a  \
           .Color\
 Scheme-Text {\x0a  \
               co\
-lor:#eff0f1;\x0a   \
+lor:#232629;\x0a   \
          }\x0a     \
    </style>\x0a    \
 </defs>\x0a    <pat\
 h class=\x22ColorSc\
 heme-Text\x22 style\
 =\x22fill:currentCo\
 lor; fill-opacit\
@@ -2005,15 +1713,15 @@
 /2000/svg\x22>\x0a    \
 <style type=\x22tex\
 t/css\x22 id=\x22curre\
 nt-color-scheme\x22\
 >\x0a        .Color\
 Scheme-Text {\x0a  \
           color:\
-#eff0f1;\x0a       \
+#232629;\x0a       \
  }\x0a    </style>\x0a\
     <g class=\x22Co\
 lorScheme-Text\x22 \
 fill=\x22currentCol\
 or\x22 fill-rule=\x22e\
 venodd\x22>\x0a       \
  <path d=\x22m8 2a6\
@@ -2026,28 +1734,108 @@
  0 1 -5-5 5 5 0 \
 0 1 5-5z\x22/>\x0a    \
     <path d=\x22m7 \
 4h2v2h-2z\x22/>\x0a   \
      <path d=\x22m7\
  7h2v5h-2z\x22/>\x0a  \
   </g>\x0a</svg>\x0a\
+\x00\x00\x04\xe0\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 viewBox=\x22\
+0 0 16 16\x22>\x0a  <d\
+efs id=\x22defs3051\
+\x22>\x0a    <style ty\
+pe=\x22text/css\x22 id\
+=\x22current-color-\
+scheme\x22>\x0a      .\
+ColorScheme-Text\
+ {\x0a        color\
+:#232629;\x0a      \
+}\x0a      </style>\
+\x0a  </defs>\x0a <pat\
+h \x0a     style=\x22f\
+ill:currentColor\
+;fill-opacity:1;\
+stroke:none\x22 \x0a  \
+   d=\x22M 8 2 A 6 \
+6 0 0 0 2 8 A 6 \
+6 0 0 0 8 14 A 6\
+ 6 0 0 0 14 8 A \
+6 6 0 0 0 8 2 z \
+M 2 3 L 2 5 L 4 \
+3 L 2 3 z M 8 3 \
+A 5 5 0 0 1 10.3\
+90625 3.609375 L\
+ 8.8691406 5.130\
+8594 A 3 3 0 0 0\
+ 8 5 A 3 3 0 0 0\
+ 7.1308594 5.130\
+8594 L 5.6132812\
+ 3.6132812 A 5 5\
+ 0 0 1 8 3 z M 1\
+2 3 L 14 5 L 14 \
+3 L 12 3 z M 3.6\
+09375 5.609375 L\
+ 5.1308594 7.130\
+8594 A 3 3 0 0 0\
+ 5 8 A 3 3 0 0 0\
+ 5.1308594 8.869\
+1406 L 3.6132812\
+ 10.386719 A 5 5\
+ 0 0 1 3 8 A 5 5\
+ 0 0 1 3.609375 \
+5.609375 z M 12.\
+386719 5.6132812\
+ A 5 5 0 0 1 13 \
+8 A 5 5 0 0 1 12\
+.390625 10.39062\
+5 L 10.869141 8.\
+8691406 A 3 3 0 \
+0 0 11 8 A 3 3 0\
+ 0 0 10.869141 7\
+.1308594 L 12.38\
+6719 5.6132812 z\
+ M 8 6 A 2 2 0 0\
+ 1 10 8 A 2 2 0 \
+0 1 8 10 A 2 2 0\
+ 0 1 6 8 A 2 2 0\
+ 0 1 8 6 z M 7.1\
+308594 10.869141\
+ A 3 3 0 0 0 8 1\
+1 A 3 3 0 0 0 8.\
+8691406 10.86914\
+1 L 10.386719 12\
+.386719 A 5 5 0 \
+0 1 8 13 A 5 5 0\
+ 0 1 5.609375 12\
+.390625 L 7.1308\
+594 10.869141 z \
+M 2 11 L 2 13 L \
+4 13 L 2 11 z M \
+14 11 L 12 13 L \
+14 13 L 14 11 z \
+\x22\x0a     class=\x22Co\
+lorScheme-Text\x22\x0a\
+     />\x0a</svg>\x0a\
 \x00\x00\x03\xdd\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a       d\
 =\x22M 10 2.5 C 9.0\
@@ -2090,68 +1878,28 @@
 72 12.5 4 12.052\
 28 4 11.5 C 4 10\
 .94772 4.44772 1\
 0.5 5 10.5 z \x22\x0a \
     class=\x22Color\
 Scheme-Text\x22\x0a   \
   />\x0a</svg>\x0a\
-\x00\x00\x02[\
-<\
-svg version=\x221.1\
-\x22 viewBox=\x220 0 1\
-6 16\x22 xmlns=\x22htt\
-p://www.w3.org/2\
-000/svg\x22>\x0a    <s\
-tyle type=\x22text/\
-css\x22 id=\x22current\
--color-scheme\x22>\x0a\
-        .ColorSc\
-heme-NeutralText\
- {\x0a            c\
-olor:#f67400;\x0a  \
-      }\x0a    </st\
-yle>\x0a    <path c\
-lass=\x22ColorSchem\
-e-NeutralText\x22 d\
-=\x22m8.0065001 2.0\
-000269a0.7500188\
-1 0.74999832 0 0\
- 0-0.6772669 0.4\
-14749l-5.2501316\
- 10.499976a0.750\
-01881 0.74999832\
- 0 0 0 0.6712668\
- 1.085248h10.500\
-264a0.75001881 0\
-.74999832 0 0 0 \
-0.671266-1.08524\
-8l-5.2501312-10.\
-499976a0.7500188\
-1 0.74999832 0 0\
- 0-0.6652667-0.4\
-14749z\x22 fill=\x22cu\
-rrentColor\x22/>\x0a  \
-  <path d=\x22m7 5v\
-4h2v-4zm0 5v2h2v\
--2z\x22 fill=\x22#fff\x22\
-/>\x0a</svg>\x0a\
 \x00\x00\x06i\
 <\
 svg version=\x221.1\
 \x22 viewBox=\x220 0 1\
 6 16\x22 xmlns=\x22htt\
 p://www.w3.org/2\
 000/svg\x22>\x0a    <d\
 efs>\x0a        <st\
 yle type=\x22text/c\
 ss\x22 id=\x22current-\
 color-scheme\x22>.C\
 olorScheme-Text \
 {\x0a        color:\
-#eff0f1;\x0a      }\
+#232629;\x0a      }\
 </style>\x0a    </d\
 efs>\x0a    <path c\
 lass=\x22ColorSchem\
 e-Text\x22 fill=\x22cu\
 rrentColor\x22 d=\x22m\
 14 8c0 1.1088173\
 -0.319333 2.1400\
@@ -2235,94 +1983,14 @@
 1299 0.063349-0.\
 01766 0.09375-0.\
 03125 0.08886-0.\
 04062 0.164735-0\
 .108612 0.25-0.1\
 5625h0.03125z\x22/>\
 \x0a</svg>\x0a\
-\x00\x00\x04\xe0\
-<\
-svg xmlns=\x22http:\
-//www.w3.org/200\
-0/svg\x22 viewBox=\x22\
-0 0 16 16\x22>\x0a  <d\
-efs id=\x22defs3051\
-\x22>\x0a    <style ty\
-pe=\x22text/css\x22 id\
-=\x22current-color-\
-scheme\x22>\x0a      .\
-ColorScheme-Text\
- {\x0a        color\
-:#eff0f1;\x0a      \
-}\x0a      </style>\
-\x0a  </defs>\x0a <pat\
-h \x0a     style=\x22f\
-ill:currentColor\
-;fill-opacity:1;\
-stroke:none\x22 \x0a  \
-   d=\x22M 8 2 A 6 \
-6 0 0 0 2 8 A 6 \
-6 0 0 0 8 14 A 6\
- 6 0 0 0 14 8 A \
-6 6 0 0 0 8 2 z \
-M 2 3 L 2 5 L 4 \
-3 L 2 3 z M 8 3 \
-A 5 5 0 0 1 10.3\
-90625 3.609375 L\
- 8.8691406 5.130\
-8594 A 3 3 0 0 0\
- 8 5 A 3 3 0 0 0\
- 7.1308594 5.130\
-8594 L 5.6132812\
- 3.6132812 A 5 5\
- 0 0 1 8 3 z M 1\
-2 3 L 14 5 L 14 \
-3 L 12 3 z M 3.6\
-09375 5.609375 L\
- 5.1308594 7.130\
-8594 A 3 3 0 0 0\
- 5 8 A 3 3 0 0 0\
- 5.1308594 8.869\
-1406 L 3.6132812\
- 10.386719 A 5 5\
- 0 0 1 3 8 A 5 5\
- 0 0 1 3.609375 \
-5.609375 z M 12.\
-386719 5.6132812\
- A 5 5 0 0 1 13 \
-8 A 5 5 0 0 1 12\
-.390625 10.39062\
-5 L 10.869141 8.\
-8691406 A 3 3 0 \
-0 0 11 8 A 3 3 0\
- 0 0 10.869141 7\
-.1308594 L 12.38\
-6719 5.6132812 z\
- M 8 6 A 2 2 0 0\
- 1 10 8 A 2 2 0 \
-0 1 8 10 A 2 2 0\
- 0 1 6 8 A 2 2 0\
- 0 1 8 6 z M 7.1\
-308594 10.869141\
- A 3 3 0 0 0 8 1\
-1 A 3 3 0 0 0 8.\
-8691406 10.86914\
-1 L 10.386719 12\
-.386719 A 5 5 0 \
-0 1 8 13 A 5 5 0\
- 0 1 5.609375 12\
-.390625 L 7.1308\
-594 10.869141 z \
-M 2 11 L 2 13 L \
-4 13 L 2 11 z M \
-14 11 L 12 13 L \
-14 13 L 14 11 z \
-\x22\x0a     class=\x22Co\
-lorScheme-Text\x22\x0a\
-     />\x0a</svg>\x0a\
 \x00\x00\x01\xa1\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
@@ -2344,28 +2012,62 @@
 gativeText\x22\x0a    \
  d=\x22m5 2v2h1v-1h\
 4v1h1v-2h-5zm-3 \
 3v1h2v8h8v-8h2v-\
 1zm3 1h6v7h-6z\x22 \
 \x0a     />\x0a</svg>\x0a\
 \
+\x00\x00\x01\xfb\
+<\
+svg viewBox=\x220 0\
+ 16 16\x22 xmlns=\x22h\
+ttp://www.w3.org\
+/2000/svg\x22>\x0a    \
+<style type=\x22tex\
+t/css\x22 id=\x22curre\
+nt-color-scheme\x22\
+>\x0a        .Color\
+Scheme-Text {\x0a  \
+          color:\
+#232629;\x0a       \
+ }\x0a    </style>\x0a\
+    <path d=\x22m3 \
+2v12h7.5c1.385 0\
+ 2.5-1.115 2.5-2\
+.5s-1.115-2.5-2.\
+5-2.5h-1.7929688\
+l1.4999998-1.5-.\
+707031-.7070312-\
+2.7070312 2.7070\
+312 2.7070312 2.\
+707031.707031-.7\
+07031-1.4999998-\
+1.5h1.7929688c.8\
+31 0 1.5.669 1.5\
+ 1.5s-.669 1.5-1\
+.5 1.5h-6.5v-10h\
+5v3h3v2h1v-3l-3-\
+3z\x22 class=\x22Color\
+Scheme-Text\x22 fil\
+l=\x22currentColor\x22\
+/>\x0a</svg>\x0a\
 \x00\x00\x02[\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 2 2 L 2 3 L 2 \
@@ -2384,70 +2086,28 @@
 921875 6 L 3 6 L\
  3 3 z M 3 7 L 1\
 3 7 L 13 13 L 3 \
 13 L 3 7 z \x22\x0a   \
   class=\x22ColorSc\
 heme-Text\x22\x0a     \
 />\x0a</svg>\x0a\
-\x00\x00\x02y\
-<\
-svg id=\x22svg6\x22 ve\
-rsion=\x221.1\x22 view\
-Box=\x220 0 16 16\x22 \
-xmlns=\x22http://ww\
-w.w3.org/2000/sv\
-g\x22>\x0a    <style i\
-d=\x22current-color\
--scheme\x22 type=\x22t\
-ext/css\x22>.ColorS\
-cheme-Text {\x0a   \
-         color:#\
-eff0f1;\x0a        \
-}</style>\x0a    <p\
-ath id=\x22path4\x22 c\
-lass=\x22ColorSchem\
-e-Text\x22 d=\x22m7.5 \
-2-3.5 3.5 3.5 3.\
-5 0.71875-0.7187\
-5-2.3125-2.28125\
-h3.59375c1.93299\
-8 0 3.5 1.566998\
-4 3.5 3.5 0 1.93\
-3002-1.567002 3.\
-5-3.5 3.5h-1.5v1\
-h1.5c2.485283 0 \
-4.5-2.014748 4.5\
--4.5 0-2.4852521\
--2.014717-4.5-4.\
-5-4.5h-3.59375l2\
-.3125-2.28125z\x22 \
-fill=\x22currentCol\
-or\x22/>\x0a    <rect \
-id=\x22rect837\x22 cla\
-ss=\x22ColorScheme-\
-Text\x22 x=\x222\x22 y=\x222\
-\x22 width=\x221\x22 heig\
-ht=\x227\x22 fill=\x22cur\
-rentColor\x22 fill-\
-rule=\x22evenodd\x22/>\
-\x0a</svg>\x0a\
 \x00\x00\x02\xdd\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 2 2 L 2 14 L 3\
@@ -2474,28 +2134,70 @@
  6 10 L 10 10 L \
 11 10 L 11 13 L \
 10 13 L 6 13 L 5\
  13 L 5 10 z \x22\x0a \
     class=\x22Color\
 Scheme-Text\x22\x0a   \
   />\x0a</svg>\x0a\
+\x00\x00\x02y\
+<\
+svg id=\x22svg6\x22 ve\
+rsion=\x221.1\x22 view\
+Box=\x220 0 16 16\x22 \
+xmlns=\x22http://ww\
+w.w3.org/2000/sv\
+g\x22>\x0a    <style i\
+d=\x22current-color\
+-scheme\x22 type=\x22t\
+ext/css\x22>.ColorS\
+cheme-Text {\x0a   \
+         color:#\
+232629;\x0a        \
+}</style>\x0a    <p\
+ath id=\x22path4\x22 c\
+lass=\x22ColorSchem\
+e-Text\x22 d=\x22m7.5 \
+2-3.5 3.5 3.5 3.\
+5 0.71875-0.7187\
+5-2.3125-2.28125\
+h3.59375c1.93299\
+8 0 3.5 1.566998\
+4 3.5 3.5 0 1.93\
+3002-1.567002 3.\
+5-3.5 3.5h-1.5v1\
+h1.5c2.485283 0 \
+4.5-2.014748 4.5\
+-4.5 0-2.4852521\
+-2.014717-4.5-4.\
+5-4.5h-3.59375l2\
+.3125-2.28125z\x22 \
+fill=\x22currentCol\
+or\x22/>\x0a    <rect \
+id=\x22rect837\x22 cla\
+ss=\x22ColorScheme-\
+Text\x22 x=\x222\x22 y=\x222\
+\x22 width=\x221\x22 heig\
+ht=\x227\x22 fill=\x22cur\
+rentColor\x22 fill-\
+rule=\x22evenodd\x22/>\
+\x0a</svg>\x0a\
 \x00\x00\x02\x0e\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h \x0a     style=\x22f\
 ill:currentColor\
 ;fill-opacity:1;\
 stroke:none\x22 \x0a  \
    d=\x22M 3 2 L 3 \
@@ -2556,15 +2258,15 @@
 0 0 16 16\x22>\x0a    \
 <style type=\x22tex\
 t/css\x22 id=\x22curre\
 nt-color-scheme\x22\
 >\x0a        .Color\
 Scheme-Text {\x0a  \
           color:\
-#eff0f1;\x0a       \
+#232629;\x0a       \
  }\x0a    </style>\x0a\
     <path d=\x22m2 \
 2v12l12-6z\x22 clas\
 s=\x22ColorScheme-T\
 ext\x22 fill=\x22curre\
 ntColor\x22/>\x0a</svg\
 >\x0a\
@@ -2577,15 +2279,15 @@
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 7 3.0058594 L \
@@ -2610,15 +2312,15 @@
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 6 2 L 0.707031\
@@ -2642,60 +2344,28 @@
 .0214844 8 L 7.0\
 117188 5.9902344\
  L 8.0019531 5 z\
  \x22\x0a     class=\x22C\
 olorScheme-Text\x22\
 \x0a     />\x0a</svg>\x0a\
 \
-\x00\x00\x01\xd1\
-<\
-svg version=\x221.1\
-\x22 viewBox=\x220 0 1\
-6 16\x22 xmlns=\x22htt\
-p://www.w3.org/2\
-000/svg\x22>\x0a    <s\
-tyle type=\x22text/\
-css\x22 id=\x22current\
--color-scheme\x22>\x0a\
-        .ColorSc\
-heme-NegativeTex\
-t {\x0a            \
-color:#da4453;\x0a \
-       }\x0a    </s\
-tyle>\x0a    <rect \
-class=\x22ColorSche\
-me-NegativeText\x22\
- x=\x222\x22 y=\x222\x22 wid\
-th=\x2212\x22 height=\x22\
-12\x22 rx=\x222\x22 fill=\
-\x22currentColor\x22/>\
-\x0a    <path d=\x22M \
-5.414,4 4,5.414 \
-6.586,8 4,10.586\
- 5.414,12 8,9.41\
-4 10.586,12 12,1\
-0.586 9.414,8 12\
-,5.414 10.586,4 \
-8,6.586 Z\x22 fill=\
-\x22#fff\x22/>\x0a</svg>\x0a\
-\
 \x00\x00\x02\xfe\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a       d\
 =\x22M 8 2 C 4.6862\
@@ -2737,15 +2407,15 @@
 efs id=\x22defs3051\
 \x22>\x0a    <style ty\
 pe=\x22text/css\x22 id\
 =\x22current-color-\
 scheme\x22>\x0a      .\
 ColorScheme-Text\
  {\x0a        color\
-:#eff0f1;\x0a      \
+:#232629;\x0a      \
 }\x0a      </style>\
 \x0a  </defs>\x0a <pat\
 h style=\x22fill:cu\
 rrentColor;fill-\
 opacity:1;stroke\
 :none\x22 \x0a     d=\x22\
 M 13.273438 3.5 \
@@ -2758,14 +2428,86 @@
  L 6.7265625 11.\
 419922 L 14 4.22\
 07031 L 13.27343\
 8 3.5 z \x22\x0a     c\
 lass=\x22ColorSchem\
 e-Text\x22\x0a     />\x0a\
 </svg>\x0a\
+\x00\x00\x02[\
+<\
+svg version=\x221.1\
+\x22 viewBox=\x220 0 1\
+6 16\x22 xmlns=\x22htt\
+p://www.w3.org/2\
+000/svg\x22>\x0a    <s\
+tyle type=\x22text/\
+css\x22 id=\x22current\
+-color-scheme\x22>\x0a\
+        .ColorSc\
+heme-NeutralText\
+ {\x0a            c\
+olor:#f67400;\x0a  \
+      }\x0a    </st\
+yle>\x0a    <path c\
+lass=\x22ColorSchem\
+e-NeutralText\x22 d\
+=\x22m8.0065001 2.0\
+000269a0.7500188\
+1 0.74999832 0 0\
+ 0-0.6772669 0.4\
+14749l-5.2501316\
+ 10.499976a0.750\
+01881 0.74999832\
+ 0 0 0 0.6712668\
+ 1.085248h10.500\
+264a0.75001881 0\
+.74999832 0 0 0 \
+0.671266-1.08524\
+8l-5.2501312-10.\
+499976a0.7500188\
+1 0.74999832 0 0\
+ 0-0.6652667-0.4\
+14749z\x22 fill=\x22cu\
+rrentColor\x22/>\x0a  \
+  <path d=\x22m7 5v\
+4h2v-4zm0 5v2h2v\
+-2z\x22 fill=\x22#fff\x22\
+/>\x0a</svg>\x0a\
+\x00\x00\x01\xd1\
+<\
+svg version=\x221.1\
+\x22 viewBox=\x220 0 1\
+6 16\x22 xmlns=\x22htt\
+p://www.w3.org/2\
+000/svg\x22>\x0a    <s\
+tyle type=\x22text/\
+css\x22 id=\x22current\
+-color-scheme\x22>\x0a\
+        .ColorSc\
+heme-NegativeTex\
+t {\x0a            \
+color:#da4453;\x0a \
+       }\x0a    </s\
+tyle>\x0a    <rect \
+class=\x22ColorSche\
+me-NegativeText\x22\
+ x=\x222\x22 y=\x222\x22 wid\
+th=\x2212\x22 height=\x22\
+12\x22 rx=\x222\x22 fill=\
+\x22currentColor\x22/>\
+\x0a    <path d=\x22M \
+5.414,4 4,5.414 \
+6.586,8 4,10.586\
+ 5.414,12 8,9.41\
+4 10.586,12 12,1\
+0.586 9.414,8 12\
+,5.414 10.586,4 \
+8,6.586 Z\x22 fill=\
+\x22#fff\x22/>\x0a</svg>\x0a\
+\
 \x00\x00\x02^\
 <\
 svg width=\x2216\x22 x\
 mlns=\x22http://www\
 .w3.org/2000/svg\
 \x22 height=\x2216\x22 vi\
 ewBox=\x220 0 16 16\
@@ -2963,34 +2705,34 @@
 \x22 fill=\x22#8542c2\x22\
  shape-rendering\
 =\x22auto\x22/>\x0a</svg>\
 \x0a\
 "
 
 qt_resource_name = b"\
-\x00\x0a\
-\x0d\x00\x99\xeb\
-\x00B\
-\x00r\x00e\x00e\x00z\x00e\x00D\x00a\x00r\x00k\
-\x00\x0d\
-\x0a\xe8\x1f\xc7\
-\x00l\
-\x00o\x00g\x00o\x00-\x00t\x00i\x00n\x00y\x00.\x00p\x00n\x00g\
 \x00\x06\
-\x04\x98\xbd\x05\
-\x00B\
+\x06\x98\xbd\x05\
+\x00b\
 \x00r\x00e\x00e\x00z\x00e\
 \x00\x0b\
+\x00\xd0\xbf+\
+\x00b\
+\x00r\x00e\x00e\x00z\x00e\x00-\x00d\x00a\x00r\x00k\
+\x00\x0b\
 \x0b\xba\x81\xb5\
 \x00i\
 \x00n\x00d\x00e\x00x\x00.\x00t\x00h\x00e\x00m\x00e\
 \x00\x09\
 \x03\xcc\xee\xc3\
 \x00m\
 \x00i\x00m\x00e\x00t\x00y\x00p\x00e\x00s\
+\x00\x06\
+\x07\xaa\x8b\xc3\
+\x00s\
+\x00t\x00a\x00t\x00u\x00s\
 \x00\x07\
 \x07\xab\x06\x93\
 \x00a\
 \x00c\x00t\x00i\x00o\x00n\x00s\
 \x00\x02\
 \x00\x00\x03F\
 \x001\
@@ -3004,48 +2746,50 @@
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00p\x00r\x00e\x00v\x00i\x00e\x00w\x00.\
 \x00s\x00v\x00g\
 \x00\x0e\
 \x0e\xa1.G\
 \x00h\
 \x00e\x00l\x00p\x00-\x00a\x00b\x00o\x00u\x00t\x00.\x00s\x00v\x00g\
+\x00\x11\
+\x03E\xe3\x07\
+\x00h\
+\x00e\x00l\x00p\x00-\x00c\x00o\x00n\x00t\x00e\x00n\x00t\x00s\x00.\x00s\x00v\x00g\
+\
 \x00\x0d\
 \x08Q\xc4\xa7\
 \x00c\
 \x00o\x00n\x00f\x00i\x00g\x00u\x00r\x00e\x00.\x00s\x00v\x00g\
 \x00\x10\
-\x08\xcb\xea\xc7\
-\x00d\
-\x00a\x00t\x00a\x00-\x00w\x00a\x00r\x00n\x00i\x00n\x00g\x00.\x00s\x00v\x00g\
-\x00\x10\
 \x08\x15\x1e\xe7\
 \x00v\
 \x00i\x00e\x00w\x00-\x00r\x00e\x00f\x00r\x00e\x00s\x00h\x00.\x00s\x00v\x00g\
 \x00\x0f\
-\x01e6\xc7\
-\x00s\
-\x00y\x00s\x00t\x00e\x00m\x00-\x00h\x00e\x00l\x00p\x00.\x00s\x00v\x00g\
-\x00\x0f\
 \x0cB\xa4G\
 \x00e\
 \x00d\x00i\x00t\x00-\x00d\x00e\x00l\x00e\x00t\x00e\x00.\x00s\x00v\x00g\
+\x00\x13\
+\x0b\x15M\x07\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00r\x00e\x00v\x00e\x00r\x00t\x00.\x00s\
+\x00v\x00g\
 \x00\x18\
 \x0e\x10\x8e\xe7\
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00o\x00p\x00e\x00n\x00-\x00f\x00o\x00l\
 \x00d\x00e\x00r\x00.\x00s\x00v\x00g\
-\x00\x0e\
-\x0f\xc9\xd1\xa7\
-\x00e\
-\x00d\x00i\x00t\x00-\x00r\x00e\x00s\x00e\x00t\x00.\x00s\x00v\x00g\
 \x00\x11\
 \x0f\xe3\xd8\xe7\
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00s\x00a\x00v\x00e\x00.\x00s\x00v\x00g\
 \
+\x00\x0e\
+\x0f\xc9\xd1\xa7\
+\x00e\
+\x00d\x00i\x00t\x00-\x00r\x00e\x00s\x00e\x00t\x00.\x00s\x00v\x00g\
 \x00\x11\
 \x01\xa6\xc9\x07\
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00o\x00p\x00e\x00n\x00.\x00s\x00v\x00g\
 \
 \x00\x16\
 \x0e\x92\x91G\
@@ -3061,28 +2805,32 @@
 \x09\xc6\x14\xa7\
 \x00l\
 \x00i\x00s\x00t\x00-\x00a\x00d\x00d\x00.\x00s\x00v\x00g\
 \x00\x0e\
 \x0d\x8b4g\
 \x00e\
 \x00d\x00i\x00t\x00-\x00c\x00l\x00e\x00a\x00r\x00.\x00s\x00v\x00g\
-\x00\x0e\
-\x08-9G\
-\x00d\
-\x00a\x00t\x00a\x00-\x00e\x00r\x00r\x00o\x00r\x00.\x00s\x00v\x00g\
 \x00\x11\
 \x03S\x8a\x87\
 \x00d\
 \x00i\x00a\x00l\x00o\x00g\x00-\x00c\x00a\x00n\x00c\x00e\x00l\x00.\x00s\x00v\x00g\
 \
 \x00\x13\
 \x04h\xff\xc7\
 \x00d\
 \x00i\x00a\x00l\x00o\x00g\x00-\x00o\x00k\x00-\x00a\x00p\x00p\x00l\x00y\x00.\x00s\
 \x00v\x00g\
+\x00\x10\
+\x08\xcb\xea\xc7\
+\x00d\
+\x00a\x00t\x00a\x00-\x00w\x00a\x00r\x00n\x00i\x00n\x00g\x00.\x00s\x00v\x00g\
+\x00\x0e\
+\x08-9G\
+\x00d\
+\x00a\x00t\x00a\x00-\x00e\x00r\x00r\x00o\x00r\x00.\x00s\x00v\x00g\
 \x00\x0e\
 \x092O\x87\
 \x00i\
 \x00m\x00a\x00g\x00e\x00-\x00t\x00i\x00f\x00f\x00.\x00s\x00v\x00g\
 \x00\x13\
 \x0eR1\xe7\
 \x00i\
@@ -3099,137 +2847,147 @@
 \x00\x0d\
 \x07)\xeb\x87\
 \x00i\
 \x00m\x00a\x00g\x00e\x00-\x00p\x00n\x00g\x00.\x00s\x00v\x00g\
 "
 
 qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00:\x00\x02\x00\x00\x00\x03\x00\x00\x00!\
+\x00\x00\x00\x12\x00\x02\x00\x00\x00\x04\x00\x00\x00#\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x87\x8c\xdf\x0e\xff\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x04\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x04\x00\x00\x00\x03\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x00\x1b\
+\x00\x00\x00J\x00\x02\x00\x00\x00\x01\x00\x00\x00\x1d\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00\x07\
+\x00\x00\x00b\x00\x02\x00\x00\x00\x01\x00\x00\x00\x1a\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00t\x00\x02\x00\x00\x00\x01\x00\x00\x00\x07\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00.\x00\x01\x00\x00\x00\x01\x00\x00Qg\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x88\x00\x02\x00\x00\x00\x12\x00\x00\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00b\x82\
-\x00\x00\x01\x82\xfe\x95\xbc\x1d\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x13\x00\x00\x00\x08\
+\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x00\x82\xb5\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\x08\x00\x00\x00\x00\x00\x01\x00\x00h\x22\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03\x16\x00\x00\x00\x00\x00\x01\x00\x00\x8c\x83\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03>\x00\x00\x00\x00\x00\x01\x00\x00\x8f\x85\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00b9\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00p\xe7\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x010\x00\x00\x00\x00\x00\x01\x00\x00m\x06\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x92\x00\x00\x00\x00\x00\x01\x00\x00^\xc4\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02\xd6\x00\x00\x00\x00\x00\x01\x00\x00\x87\xf0\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\x9a\x00\x00\x00\x00\x00\x01\x00\x00x\xf9\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01v\x00\x00\x00\x00\x00\x01\x00\x00wT\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02\xf4\x00\x00\x00\x00\x00\x01\x00\x00\x89\xde\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\xc6\x00\x00\x00\x00\x00\x01\x00\x00z\xf8\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02n\x00\x00\x00\x00\x00\x01\x00\x00\x84\xc7\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00f/\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x86\xd9\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02$\x00\x00\x00\x00\x00\x01\x00\x00\x808\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\xfc\x00\x00\x00\x00\x00\x01\x00\x00}W\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x88\x00\x02\x00\x00\x00\x02\x00\x00\x00\x1b\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x00\x86\xfe\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02H\x00\x00\x00\x00\x00\x01\x00\x00\x95D\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03:\x00\x00\x00\x00\x00\x01\x00\x00\xa0\xe7\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03b\x00\x00\x00\x00\x00\x01\x00\x00\xa3\xe9\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00th\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00\x80\x91\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00\x9f\x12\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00zQ\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00~2\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00p\xf3\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xd8\x00\x00\x00\x00\x00\x01\x00\x00\x9a\x7f\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\xe2\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x9cm\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x8d\x87\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02p\x00\x00\x00\x00\x00\x01\x00\x00\x97V\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00x^\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xa2\x00\x00\x00\x00\x00\x01\x00\x00\x99h\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x8f\xe6\
-\x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x02 \x00\x00\x00\x00\x00\x01\x00\x00\x92c\
-\x00\x00\x01\x83\x9f\xda\x12\xf9\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x00\x1c\
+\x00\x00\x03\x90\x00\x00\x00\x00\x00\x01\x00\x00\x93\xe0\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03j\x00\x00\x00\x00\x00\x01\x00\x00\x91\x81\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x88\x00\x02\x00\x00\x00\x05\x00\x00\x00\x1e\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00\xad\x0b\
+\x00\x00\x04 \x00\x00\x00\x00\x00\x01\x00\x00\x9c\xdb\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00\xafq\
+\x00\x00\x04B\x00\x00\x00\x00\x00\x01\x00\x00\x9fA\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xdc\x00\x00\x00\x00\x00\x01\x00\x00\xaa\xa9\
+\x00\x00\x04\x00\x00\x00\x00\x00\x00\x01\x00\x00\x9ay\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00\xa5\xe5\
+\x00\x00\x03\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x95\xb5\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xb0\x00\x00\x00\x00\x00\x01\x00\x00\xa8G\
+\x00\x00\x03\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x98\x17\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x008\
+\x00\x00\x00J\x00\x02\x00\x00\x00\x01\x00\x00\x00=\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00$\
+\x00\x00\x00b\x00\x02\x00\x00\x00\x01\x00\x00\x00:\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00\x14h\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x13\x00\x00\x00%\
+\x00\x00\x00t\x00\x02\x00\x00\x00\x01\x00\x00\x00'\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00.\x00\x01\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x88\x00\x02\x00\x00\x00\x12\x00\x00\x00(\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x007\xa9\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02H\x00\x00\x00\x00\x00\x01\x00\x00E\xef\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03:\x00\x00\x00\x00\x00\x01\x00\x00Q\x92\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03b\x00\x00\x00\x00\x00\x01\x00\x00T\x94\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00%\x13\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x001<\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00O\xbd\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00*\xfc\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00.\xdd\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00!\x9e\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xd8\x00\x00\x00\x00\x00\x01\x00\x00K*\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00<\x8d\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00M\x18\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00>2\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02p\x00\x00\x00\x00\x00\x01\x00\x00H\x01\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00)\x09\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xa2\x00\x00\x00\x00\x00\x01\x00\x00J\x13\
-\x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00@\x91\
-\x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x02 \x00\x00\x00\x00\x00\x01\x00\x00C\x0e\
-\x00\x00\x01\x83\x9f\xda\x12\xf9\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x009\
+\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x002u\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\x08\x00\x00\x00\x00\x00\x01\x00\x00\x17\xe2\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03\x16\x00\x00\x00\x00\x00\x01\x00\x00<C\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03>\x00\x00\x00\x00\x00\x01\x00\x00?E\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00\x11\xf9\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00 \xa7\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x010\x00\x00\x00\x00\x00\x01\x00\x00\x1c\xc6\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x92\x00\x00\x00\x00\x00\x01\x00\x00\x0e\x84\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02\xd6\x00\x00\x00\x00\x00\x01\x00\x007\xb0\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\x9a\x00\x00\x00\x00\x00\x01\x00\x00(\xb9\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01v\x00\x00\x00\x00\x00\x01\x00\x00'\x14\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02\xf4\x00\x00\x00\x00\x00\x01\x00\x009\x9e\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\xc6\x00\x00\x00\x00\x00\x01\x00\x00*\xb8\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02n\x00\x00\x00\x00\x00\x01\x00\x004\x87\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x15\xef\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02\xa0\x00\x00\x00\x00\x00\x01\x00\x006\x99\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02$\x00\x00\x00\x00\x00\x01\x00\x00/\xf8\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x01\xfc\x00\x00\x00\x00\x00\x01\x00\x00-\x17\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x88\x00\x02\x00\x00\x00\x02\x00\x00\x00;\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x03\x90\x00\x00\x00\x00\x00\x01\x00\x00C\xa0\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03j\x00\x00\x00\x00\x00\x01\x00\x00AA\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x00\x88\x00\x02\x00\x00\x00\x05\x00\x00\x00>\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00]\xb6\
+\x00\x00\x04 \x00\x00\x00\x00\x00\x01\x00\x00L\x9b\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00`\x1c\
+\x00\x00\x04B\x00\x00\x00\x00\x00\x01\x00\x00O\x01\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xdc\x00\x00\x00\x00\x00\x01\x00\x00[T\
+\x00\x00\x04\x00\x00\x00\x00\x00\x00\x01\x00\x00J9\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00V\x90\
+\x00\x00\x03\xb2\x00\x00\x00\x00\x00\x01\x00\x00Eu\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xb0\x00\x00\x00\x00\x00\x01\x00\x00X\xf2\
+\x00\x00\x03\xd4\x00\x00\x00\x00\x00\x01\x00\x00G\xd7\
 \x00\x00\x01\x86\xac\x9ffH\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-1.6.9/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-1.6.9/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,32 +93,33 @@
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.comboBox_current_profile.sizePolicy().hasHeightForWidth())
         self.comboBox_current_profile.setSizePolicy(sizePolicy)
         self.comboBox_current_profile.setMinimumSize(QSize(48, 0))
 
         self.horizontalLayout_2.addWidget(self.comboBox_current_profile)
 
-        self.pushButton_save_pofile = QPushButton(self.groupBox)
-        self.pushButton_save_pofile.setObjectName(u"pushButton_save_pofile")
+        self.pushButton_save_profile = QPushButton(self.groupBox)
+        self.pushButton_save_profile.setObjectName(u"pushButton_save_profile")
+        self.pushButton_save_profile.setEnabled(False)
         icon = QIcon()
         iconThemeName = u"document-save"
         if QIcon.hasThemeIcon(iconThemeName):
             icon = QIcon.fromTheme(iconThemeName)
         else:
             icon.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
-        self.pushButton_save_pofile.setIcon(icon)
+        self.pushButton_save_profile.setIcon(icon)
 
-        self.horizontalLayout_2.addWidget(self.pushButton_save_pofile)
+        self.horizontalLayout_2.addWidget(self.pushButton_save_profile)
 
         self.pushButton_reset_profile = QPushButton(self.groupBox)
         self.pushButton_reset_profile.setObjectName(u"pushButton_reset_profile")
         self.pushButton_reset_profile.setEnabled(False)
         icon1 = QIcon()
-        iconThemeName = u"edit-reset"
+        iconThemeName = u"document-revert"
         if QIcon.hasThemeIcon(iconThemeName):
             icon1 = QIcon.fromTheme(iconThemeName)
         else:
             icon1.addFile(u".", QSize(), QIcon.Normal, QIcon.Off)
         
         self.pushButton_reset_profile.setIcon(icon1)
 
@@ -283,14 +284,15 @@
 
         self.verticalSpacer_2 = QSpacerItem(20, 1, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_5.addItem(self.verticalSpacer_2)
 
         self.label_4 = QLabel(self.groupBox_3)
         self.label_4.setObjectName(u"label_4")
+        self.label_4.setTextInteractionFlags(Qt.LinksAccessibleByMouse)
 
         self.verticalLayout_5.addWidget(self.label_4)
 
         self.horizontalLayout = QHBoxLayout()
         self.horizontalLayout.setObjectName(u"horizontalLayout")
         self.lineEdit_out_directory = QLineEdit(self.groupBox_3)
         self.lineEdit_out_directory.setObjectName(u"lineEdit_out_directory")
@@ -447,15 +449,15 @@
         self.action_Dark.setText(QCoreApplication.translate("MainWindow", u"Dark", None))
         self.action_Light.setText(QCoreApplication.translate("MainWindow", u"Light", None))
         self.action_temp.setText(QCoreApplication.translate("MainWindow", u"<temp>", None))
         self.action_temp_2.setText(QCoreApplication.translate("MainWindow", u"<temp>", None))
         self.groupBox.setTitle(QCoreApplication.translate("MainWindow", u"Profile", None))
         self.comboBox_current_profile.setItemText(0, QCoreApplication.translate("MainWindow", u"Default", None))
 
-        self.pushButton_save_pofile.setText(QCoreApplication.translate("MainWindow", u"Save", None))
+        self.pushButton_save_profile.setText(QCoreApplication.translate("MainWindow", u"Save", None))
         self.pushButton_reset_profile.setText(QCoreApplication.translate("MainWindow", u"Reset All", None))
         self.pushButton_apply_profile.setText(QCoreApplication.translate("MainWindow", u"Apply", None))
         ___qtablewidgetitem = self.file_table.horizontalHeaderItem(0)
         ___qtablewidgetitem.setText(QCoreApplication.translate("MainWindow", u"id", None));
         ___qtablewidgetitem1 = self.file_table.horizontalHeaderItem(1)
         ___qtablewidgetitem1.setText(QCoreApplication.translate("MainWindow", u"File", None));
         ___qtablewidgetitem2 = self.file_table.horizontalHeaderItem(2)
```

### Comparing `pcleaner-1.6.2/pcleaner/gui/worker_thread.py` & `pcleaner-1.6.9/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/helpers.py` & `pcleaner-1.6.9/pcleaner/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import platform
 import subprocess
 from math import ceil
 from pathlib import Path
+import difflib
 
 from logzero import logger
 
 
 def f_plural(value, singular: str, plural: str):
     """
     Selects which form to use based on the value.
@@ -47,7 +48,23 @@
             subprocess.run(["xdg-open", path])
         elif platform.system() == "Windows":
             subprocess.run(["start", path])
         elif platform.system() == "Darwin":
             subprocess.run(["open", path])
     except Exception as e:
         logger.exception(e)
+
+
+def closest_match(word: str, choices: list[str]) -> str | None:
+    """
+    Return the closest match for the given word in the list of choices.
+    If no good match is found, return None.
+    """
+    if word in choices:
+        return word
+    else:
+        # Find the closest match using difflib:
+        closest = difflib.get_close_matches(word, choices, 1, 0.5)  # 0.6 is the default threshold
+        if closest:
+            return str(closest[0])
+        else:
+            return None
```

### Comparing `pcleaner-1.6.2/pcleaner/image_ops.py` & `pcleaner-1.6.9/pcleaner/image_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,32 +592,38 @@
 
     :param image: The image to save.
     :param path: The path to save the image to, containing a suffix.
     :param original: The original image, used to determine the compression method, if applicable.
     """
     compression_method = None
     original_image_mode = None
+    original_dpi = None
 
     if original is not None:
         if isinstance(original, Path):
             original = Image.open(original)
         if suffix_to_format[path.suffix.lower()] == original.format:
             compression_method = original.info.get("compression", None)
-            original_image_mode = original.mode
 
-    logger.debug(
-        f"Found previous compression method: {compression_method} and image mode: {original_image_mode}"
-    )
+        original_image_mode = original.mode
+        original_dpi = original.info.get("dpi", None)
 
     if original_image_mode is not None:
         image = image.convert(original_image_mode)
 
+    # Image args may be different depending on the image type.
+    kwargs = {"optimize": True}
+
     match path.suffix.lower():
         case ".png":
-            image.save(path, optimize=True, compress_level=9)
+            kwargs["compress_level"] = 9
         case ".jpg" | ".jpeg":
-            image.save(path, optimize=True, quality=95, progressive=True)
+            kwargs["quality"] = 95
+            kwargs["progressive"] = True
         case ".tif" | ".tiff":
-            logger.debug(f"Saving image with compression method: {compression_method}")
-            image.save(path, compression=compression_method if compression_method else "tiff_lzw")
-        case _:
-            image.save(path, optimize=True)
+            # Use tiff_lzw compression by default, rather than leaving them uncompressed.
+            kwargs["compression"] = compression_method if compression_method else "tiff_lzw"
+
+    if original_dpi is not None:
+        kwargs["dpi"] = original_dpi
+    logger.debug(f"Saving image {path.name} with kwargs: {kwargs}")
+    image.save(path, **kwargs)
```

### Comparing `pcleaner-1.6.2/pcleaner/main.py` & `pcleaner-1.6.9/pcleaner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,19 @@
     :param separate_noise_mask: Whether to save the noise mask separately.
     :param hide_analytics: Whether to hide the analytics.
     :param keep_cache: Whether to keep the cache directory for the text detection step.
     :param debug: Whether to show debug information.
     """
     profile = config.current_profile
 
+    # Override the skip denoising flag if the config disables denoising.
+    if not profile.denoiser.denoising_enabled:
+        logger.debug("Denoising is disabled in the config, skipping denoising step.")
+        skip_denoising = True
+
     # Catch jokesters who want to skip all 4 steps.
     if skip_text_detection and skip_pre_processing and skip_masking and skip_denoising:
         print("Well how about that, you want to skip all 4 steps? I guess I'm not needed here.")
         return
 
     cache_dir = config.get_cleaner_cache_dir()
     logger.debug(f"Cache directory: {cache_dir}")
@@ -504,18 +509,29 @@
     prefix = an.longest_common_path_prefix([str(Path(path).parent) for path, _ in removed_texts])
     if prefix:
         removed_texts = [(path[len(prefix) :], text) for path, text in removed_texts]
     # Remove a rogue / or \ from the start of the path, if they all have one.
     if all(path.startswith("/") or path.startswith("\\") for path, _ in removed_texts):
         removed_texts = [(path[1:], text) for path, text in removed_texts]
 
-    removed_texts = natsorted(removed_texts, key=lambda x: x[0])
+    removed_texts: list[tuple[str, str]] = natsorted(removed_texts, key=lambda x: x[0])
 
     print("\nDetected Text:")
-    text = "\n".join(f"{path}: {text}" for path, text in removed_texts)
+    # text = "\n".join(f"{path}: {text}" for path, text in removed_texts)
+    # Place the file path on it's own line, and only if it's different from the previous one.
+    text = ""
+    current_path = ""
+    for path, bubble in removed_texts:
+        if path != current_path:
+            text += f"\n\n{path}: "
+            current_path = path
+        text += f"\n{bubble}"
+        if "\n" in bubble:
+            logger.warning(f"Detected newline in bubble: {path} {bubble}")
+    text = text.strip()  # Remove the leading newline.
     print(text)
 
     if output_path is None:
         path = Path.cwd() / "detected_text.txt"
     else:
         path = Path(output_path)
```

### Comparing `pcleaner-1.6.2/pcleaner/masker.py` & `pcleaner-1.6.9/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/model_downloader.py` & `pcleaner-1.6.9/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/pre_processor.py` & `pcleaner-1.6.9/pcleaner/pre_processor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner/profile_cli.py` & `pcleaner-1.6.9/pcleaner/profile_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     :param profile_path: The path to the profile.
     """
     if not is_valid_profile_name(config, profile_name):
         return
 
     # If no path is given, use the default path.
     if profile_path is None:
-        profile_path = cli.get_config_path().parent / "profiles" / f"{profile_name}.conf"
+        profile_path = cli.get_default_profile_path(profile_name)
     else:
         profile_path = Path(profile_path)
         # If the path is a directory, append a default filename.
         if profile_path.is_dir():
             profile_path = profile_path / f"{profile_name}.conf"
 
     # Check if overwriting an existing file.
@@ -190,14 +190,17 @@
     try:
         profile.load(profile_path)
     except Exception as e:
         print(f"Unfixable error loading profile: {e}")
         profile = cfg.Profile()
         not_salvageable = True
 
+    # Verify the values in the profile.
+    profile.fix()
+
     # If it wasn't salvageable, ask before overwriting.
     if not_salvageable:
         if not cli.get_confirmation(
             f"Reset profile {closest_match} to defaults? This will overwrite the file."
         ):
             print("Aborting.")
             return
```

### Comparing `pcleaner-1.6.2/pcleaner/structures.py` & `pcleaner-1.6.9/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.2/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.6.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pcleaner
-Version: 1.6.2
-Summary: An AI-powered tool to clean manga panels.
-Home-page: https://github.com/VoxelCubes/PanelCleaner
-Keywords: image processing,cleaning,text removal,manga,ai,machine learning
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Natural Language :: English
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENSE
-
 # Panel Cleaner
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://img.shields.io/pypi/v/pcleaner)](https://pypi.org/project/pcleaner/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This tool uses machine learning to find text and then generates masks to cover it up with the highest accuracy possible. It is designed to clean easy bubbles, no in-painting or out-of-bubble text removal is done. This is intended to save a lot of monotonous work for people who have to clean a lot of panels, while making sure it doesn't paint over anything that it wasn't supposed to.
@@ -108,14 +92,38 @@
 Install the program with pip from [PyPI](https://pypi.org/project/pcleaner/):
 ```bash
 pip install pcleaner
 ```
 
 Note: The program has only been tested on Linux and on Windows with WSL, but should work on Windows (natively) and Mac as well.
 
+### Install with Docker
+
+Build the image with buildx:
+```bash
+docker buildx build -t pcleaner:v1 .
+
+```
+Or with the legacy builder:
+```bash
+docker image build -t pcleaner:v1 .
+```
+
+Then initialize the docker image, specifying a root folder for the container to access.
+In this example, the current directory (`pwd`) is used:
+```bash
+docker run -it --name pcleaner -v $(pwd):/app pcleaner:v1
+```
+This will also start an interactive shell in the container.
+
+You can open another one later on with:
+```bash
+docker start pcleaner
+docker exec -it pcleaner bash
+```
 
 ## Usage
 
 The program is run from the command line, and, in the most common use, takes any number of images or directories as input. The program will create a new directory called `cleaned` in the same directory as the input files, and place the cleaned images and/or masks there. Often, it's more useful to only export the mask layer, and you can do so by adding the `--save-only-mask`, or `-m` for short, option.
 
 Examples:
 ```bash
```

### Comparing `pcleaner-1.6.2/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.6.9/pcleaner.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,24 @@
 pcleaner/comic_text_detector/utils/weight_init.py
 pcleaner/comic_text_detector/utils/yolov5_utils.py
 pcleaner/data/LiberationSans-Regular.ttf
 pcleaner/data/NotoMono-Regular.ttf
 pcleaner/data/__init__.py
 pcleaner/gui/__init__.py
 pcleaner/gui/file_table.py
+pcleaner/gui/gui_utils.py
 pcleaner/gui/launcher.py
 pcleaner/gui/mainwindow_driver.py
+pcleaner/gui/new_profile_driver.py
 pcleaner/gui/profile_parser.py
 pcleaner/gui/worker_thread.py
 pcleaner/gui/CustomQ/CColorButton.py
 pcleaner/gui/CustomQ/CComboBox.py
 pcleaner/gui/CustomQ/CTableWidget.py
 pcleaner/gui/CustomQ/__init__.py
 pcleaner/gui/rc_generated_files/__init__.py
 pcleaner/gui/rc_generated_files/icons_rc.py
+pcleaner/gui/rc_generated_files/theme_icons_rc.py
 pcleaner/gui/ui_generated_files/__init__.py
 pcleaner/gui/ui_generated_files/ui_ImageDetails.py
-pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+pcleaner/gui/ui_generated_files/ui_NewProfile.py
```

### Comparing `pcleaner-1.6.2/setup.cfg` & `pcleaner-1.6.9/setup.cfg`

 * *Files identical despite different names*

