# Comparing `tmp/laok-0.2.16.tar.gz` & `tmp/laok-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laok-0.2.16.tar", last modified: Mon Aug 29 05:11:11 2022, max compression
+gzip compressed data, was "laok-0.2.17.tar", last modified: Fri May  5 09:26:37 2023, max compression
```

## Comparing `laok-0.2.16.tar` & `laok-0.2.17.tar`

### file list

```diff
@@ -1,126 +1,176 @@
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.925236 laok-0.2.16/
--rw-rw-rw-   0        0        0      213 2022-08-29 05:11:11.925236 laok-0.2.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.836471 laok-0.2.16/laok/
--rw-rw-rw-   0        0        0       23 2022-08-14 16:39:03.000000 laok-0.2.16/laok/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.840460 laok-0.2.16/laok/cv2d/
--rw-rw-rw-   0        0        0      191 2022-08-24 15:07:21.000000 laok-0.2.16/laok/cv2d/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.841457 laok-0.2.16/laok/cv2d/aug/
--rw-rw-rw-   0        0        0        0 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/aug/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.843452 laok-0.2.16/laok/cv2d/cvt/
--rw-rw-rw-   0        0        0        2 2022-08-24 15:07:38.000000 laok-0.2.16/laok/cv2d/cvt/__init__.py
--rw-rw-rw-   0        0        0     4072 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/cvt/cvt.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.844449 laok-0.2.16/laok/cv2d/draw/
--rw-rw-rw-   0        0        0        2 2022-08-24 15:07:38.000000 laok-0.2.16/laok/cv2d/draw/__init__.py
--rw-rw-rw-   0        0        0      953 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/draw/draw.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.847442 laok-0.2.16/laok/cv2d/edge/
--rw-rw-rw-   0        0        0       21 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/edge/__init__.py
--rw-rw-rw-   0        0        0     1956 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/edge/_cv2.py
--rw-rw-rw-   0        0        0      369 2022-08-24 15:06:18.000000 laok-0.2.16/laok/cv2d/edge/_sk.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.850433 laok-0.2.16/laok/cv2d/filter/
--rw-rw-rw-   0        0        0       21 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/filter/__init__.py
--rw-rw-rw-   0        0        0      891 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/filter/_cv2.py
--rw-rw-rw-   0        0        0      390 2022-08-28 01:58:18.000000 laok-0.2.16/laok/cv2d/filter/_sk.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.855420 laok-0.2.16/laok/cv2d/io/
--rw-rw-rw-   0        0        0       64 2022-08-24 08:51:59.000000 laok-0.2.16/laok/cv2d/io/__init__.py
--rw-rw-rw-   0        0        0      333 2022-08-24 08:50:04.000000 laok-0.2.16/laok/cv2d/io/_cv2.py
--rw-rw-rw-   0        0        0      612 2022-08-24 15:02:25.000000 laok-0.2.16/laok/cv2d/io/_pil.py
--rw-rw-rw-   0        0        0      333 2022-08-24 08:52:27.000000 laok-0.2.16/laok/cv2d/io/_sk.py
--rw-rw-rw-   0        0        0     2931 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/io/io.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.857415 laok-0.2.16/laok/cv2d/misc/
--rw-rw-rw-   0        0        0       22 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/misc/__init__.py
--rw-rw-rw-   0        0        0     1135 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/misc/_data.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.860407 laok-0.2.16/laok/cv2d/morph/
--rw-rw-rw-   0        0        0       21 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/morph/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/morph/_cv2.py
--rw-rw-rw-   0        0        0      390 2022-08-28 01:58:17.000000 laok-0.2.16/laok/cv2d/morph/_sk.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.861404 laok-0.2.16/laok/cv2d/photo/
--rw-rw-rw-   0        0        0       31 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/photo/__init__.py
--rw-rw-rw-   0        0        0      790 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/photo/domain_adapter.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.865397 laok-0.2.16/laok/cv2d/show/
--rw-rw-rw-   0        0        0       25 2022-08-24 15:20:07.000000 laok-0.2.16/laok/cv2d/show/__init__.py
--rw-rw-rw-   0        0        0      485 2022-08-24 15:18:45.000000 laok-0.2.16/laok/cv2d/show/_pil.py
--rw-rw-rw-   0        0        0      975 2022-08-25 12:15:26.000000 laok-0.2.16/laok/cv2d/show/_plt.py
--rw-rw-rw-   0        0        0     1130 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv2d/show/gui.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.866391 laok-0.2.16/laok/cv3d/
--rw-rw-rw-   0        0        0        0 2022-08-19 03:40:05.000000 laok-0.2.16/laok/cv3d/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.867389 laok-0.2.16/laok/cv3d/io/
--rw-rw-rw-   0        0        0     1989 2022-08-19 04:21:34.000000 laok-0.2.16/laok/cv3d/io/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.868386 laok-0.2.16/laok/cv3d/model/
--rw-rw-rw-   0        0        0      325 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/model/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.871378 laok-0.2.16/laok/cv3d/show/
--rw-rw-rw-   0        0        0      348 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/show/__init__.py
--rw-rw-rw-   0        0        0     2258 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/show/_show_cld.py
--rw-rw-rw-   0        0        0     2350 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/show/_vtk.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.872390 laok-0.2.16/laok/cv3d/statis/
--rw-rw-rw-   0        0        0      502 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/statis/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.877362 laok-0.2.16/laok/cv3d/trans/
--rw-rw-rw-   0        0        0      369 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/trans/__init__.py
--rw-rw-rw-   0        0        0      338 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/trans/moments.py
--rw-rw-rw-   0        0        0     1803 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/trans/proj_img.py
--rw-rw-rw-   0        0        0      348 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/trans/sample.py
--rw-rw-rw-   0        0        0    22067 2022-08-14 16:39:03.000000 laok-0.2.16/laok/cv3d/trans/trans.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.878359 laok-0.2.16/laok/dnn/
--rw-rw-rw-   0        0        0      150 2022-08-19 12:33:30.000000 laok-0.2.16/laok/dnn/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.880354 laok-0.2.16/laok/dnn/classify/
--rw-rw-rw-   0        0        0      143 2022-08-19 03:13:22.000000 laok-0.2.16/laok/dnn/classify/__init__.py
--rw-rw-rw-   0        0        0     8879 2022-08-23 10:36:13.000000 laok-0.2.16/laok/dnn/classify/_torch.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.881353 laok-0.2.16/laok/gui/
--rw-rw-rw-   0        0        0        0 2022-08-14 16:39:03.000000 laok-0.2.16/laok/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.882349 laok-0.2.16/laok/ml/
--rw-rw-rw-   0        0        0        2 2022-08-18 15:11:34.000000 laok-0.2.16/laok/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.883346 laok-0.2.16/laok/ml/classifier/
--rw-rw-rw-   0        0        0       27 2022-08-14 16:39:03.000000 laok-0.2.16/laok/ml/classifier/__init__.py
--rw-rw-rw-   0        0        0     5374 2022-08-23 23:57:55.000000 laok-0.2.16/laok/ml/classifier/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.885341 laok-0.2.16/laok/ml/cluster/
--rw-rw-rw-   0        0        0      127 2022-08-18 15:55:20.000000 laok-0.2.16/laok/ml/cluster/__init__.py
--rw-rw-rw-   0        0        0     2520 2022-08-23 23:59:23.000000 laok-0.2.16/laok/ml/cluster/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.887336 laok-0.2.16/laok/ml/dataset/
--rw-rw-rw-   0        0        0      147 2022-08-18 15:32:13.000000 laok-0.2.16/laok/ml/dataset/__init__.py
--rw-rw-rw-   0        0        0     6614 2022-08-24 00:01:29.000000 laok-0.2.16/laok/ml/dataset/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.889330 laok-0.2.16/laok/ml/metrics/
--rw-rw-rw-   0        0        0        0 2022-08-18 18:04:35.000000 laok-0.2.16/laok/ml/metrics/__init__.py
--rw-rw-rw-   0        0        0     1841 2022-08-18 18:16:04.000000 laok-0.2.16/laok/ml/metrics/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.890328 laok-0.2.16/laok/ml/misc/
--rw-rw-rw-   0        0        0     1405 2022-08-14 16:39:03.000000 laok-0.2.16/laok/ml/misc/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.893320 laok-0.2.16/laok/ml/plot/
--rw-rw-rw-   0        0        0      450 2022-08-18 16:00:10.000000 laok-0.2.16/laok/ml/plot/__init__.py
--rw-rw-rw-   0        0        0     3758 2022-08-14 16:39:03.000000 laok-0.2.16/laok/ml/plot/draw_types.py
--rw-rw-rw-   0        0        0      678 2022-08-18 15:58:18.000000 laok-0.2.16/laok/ml/plot/ml_data.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.895314 laok-0.2.16/laok/ml/reduce_dim/
--rw-rw-rw-   0        0        0      121 2022-08-18 17:24:02.000000 laok-0.2.16/laok/ml/reduce_dim/__init__.py
--rw-rw-rw-   0        0        0      388 2022-08-18 17:19:34.000000 laok-0.2.16/laok/ml/reduce_dim/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.897309 laok-0.2.16/laok/ml/regress/
--rw-rw-rw-   0        0        0       31 2022-08-14 16:39:03.000000 laok-0.2.16/laok/ml/regress/__init__.py
--rw-rw-rw-   0        0        0     6537 2022-08-24 00:02:51.000000 laok-0.2.16/laok/ml/regress/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.898307 laok-0.2.16/laok/ml/transform/
--rw-rw-rw-   0        0        0        0 2022-08-18 18:00:16.000000 laok-0.2.16/laok/ml/transform/__init__.py
--rw-rw-rw-   0        0        0      410 2022-08-18 18:15:15.000000 laok-0.2.16/laok/ml/transform/_sklearn.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.902297 laok-0.2.16/laok/test/
--rw-rw-rw-   0        0        0     1636 2022-08-29 04:09:53.000000 laok-0.2.16/laok/test/__init__.py
--rw-rw-rw-   0        0        0     5999 2022-08-29 05:10:28.000000 laok-0.2.16/laok/test/_dump.py
--rw-rw-rw-   0        0        0     3806 2022-08-29 00:24:33.000000 laok-0.2.16/laok/test/_run.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.924239 laok-0.2.16/laok/util/
--rw-rw-rw-   0        0        0        0 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/__init__.py
--rw-rw-rw-   0        0        0     8389 2022-08-28 02:25:49.000000 laok-0.2.16/laok/util/color.py
--rw-rw-rw-   0        0        0     2245 2022-08-22 04:36:51.000000 laok-0.2.16/laok/util/fdata.py
--rw-rw-rw-   0        0        0     7225 2022-08-19 03:06:28.000000 laok-0.2.16/laok/util/fpath.py
--rw-rw-rw-   0        0        0      675 2022-08-28 02:27:59.000000 laok-0.2.16/laok/util/http.py
--rw-rw-rw-   0        0        0      950 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/iterfunc.py
--rw-rw-rw-   0        0        0     1752 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/log.py
--rw-rw-rw-   0        0        0      630 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/network.py
--rw-rw-rw-   0        0        0     1007 2022-08-19 03:43:03.000000 laok-0.2.16/laok/util/numpy_.py
--rw-rw-rw-   0        0        0     3044 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/onnx_.py
--rw-rw-rw-   0        0        0     2444 2022-08-28 02:31:35.000000 laok-0.2.16/laok/util/parallel.py
--rw-rw-rw-   0        0        0      754 2022-08-28 06:08:45.000000 laok-0.2.16/laok/util/pickle_.py
--rw-rw-rw-   0        0        0     2738 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/ros_.py
--rw-rw-rw-   0        0        0      475 2022-08-14 16:39:03.000000 laok-0.2.16/laok/util/str.py
--rw-rw-rw-   0        0        0      536 2022-08-28 02:37:20.000000 laok-0.2.16/laok/util/sys_.py
--rw-rw-rw-   0        0        0     3161 2022-08-28 01:50:08.000000 laok-0.2.16/laok/util/time.py
--rw-rw-rw-   0        0        0     2181 2022-08-19 03:12:24.000000 laok-0.2.16/laok/util/torch_.py
-drwxrwxrwx   0        0        0        0 2022-08-29 05:11:11.839463 laok-0.2.16/laok.egg-info/
--rw-rw-rw-   0        0        0      213 2022-08-29 05:11:11.000000 laok-0.2.16/laok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2155 2022-08-29 05:11:11.000000 laok-0.2.16/laok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-29 05:11:11.000000 laok-0.2.16/laok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-08-29 05:11:11.000000 laok-0.2.16/laok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-29 05:11:11.926233 laok-0.2.16/setup.cfg
--rw-rw-rw-   0        0        0      301 2022-08-29 05:10:44.000000 laok-0.2.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.359424 laok-0.2.17/
+-rw-rw-rw-   0        0        0      217 2023-05-05 09:26:37.358426 laok-0.2.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.261685 laok-0.2.17/laok/
+-rw-rw-rw-   0        0        0       21 2023-04-23 12:49:06.000000 laok-0.2.17/laok/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.269662 laok-0.2.17/laok/base/
+-rw-rw-rw-   0        0        0      252 2023-05-04 14:39:27.000000 laok-0.2.17/laok/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.270661 laok-0.2.17/laok/base/alg/
+-rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.17/laok/base/alg/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.17/laok/base/alg/addict.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.272653 laok-0.2.17/laok/base/conf/
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:38:53.000000 laok-0.2.17/laok/base/conf/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.17/laok/base/conf/conf_global.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.275646 laok-0.2.17/laok/base/dataset/
+-rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.17/laok/base/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.17/laok/base/dataset/cvt_voc_yolo.py
+-rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.17/laok/base/dataset/darknet-voc2yolo.py
+-rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.17/laok/base/dataset/voc_label.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.277643 laok-0.2.17/laok/base/dtime/
+-rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/dtime/__init__.py
+-rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.17/laok/base/dtime/datetime_.py
+-rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.17/laok/base/dtime/timer.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.283626 laok-0.2.17/laok/base/fs/
+-rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.17/laok/base/fs/__init__.py
+-rw-rw-rw-   0        0        0     1740 2023-04-19 09:22:34.000000 laok-0.2.17/laok/base/fs/fdata.py
+-rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.17/laok/base/fs/fname.py
+-rw-rw-rw-   0        0        0     4393 2023-05-04 14:09:33.000000 laok-0.2.17/laok/base/fs/fpath.py
+-rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.17/laok/base/fs/fsearch.py
+-rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.17/laok/base/fs/fwalk.py
+-rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.17/laok/base/fs/name_index.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.284624 laok-0.2.17/laok/base/func/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:09:16.000000 laok-0.2.17/laok/base/func/__init__.py
+-rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/func/print_info.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.286619 laok-0.2.17/laok/base/log/
+-rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.17/laok/base/log/__init__.py
+-rw-rw-rw-   0        0        0     2185 2023-04-19 14:41:16.000000 laok-0.2.17/laok/base/log/log.py
+-rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.17/laok/base/log/log_default.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.289610 laok-0.2.17/laok/base/net/
+-rw-rw-rw-   0        0        0       45 2023-05-04 14:42:06.000000 laok-0.2.17/laok/base/net/__init__.py
+-rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.17/laok/base/net/ip.py
+-rw-rw-rw-   0        0        0     2654 2023-04-20 15:19:59.000000 laok-0.2.17/laok/base/net/requests_.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.290607 laok-0.2.17/laok/base/parallel/
+-rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/parallel/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.17/laok/base/parallel/pool.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.295594 laok-0.2.17/laok/base/ser/
+-rw-rw-rw-   0        0        0      136 2023-04-25 06:35:56.000000 laok-0.2.17/laok/base/ser/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.17/laok/base/ser/_json.py
+-rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.17/laok/base/ser/_marshal.py
+-rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.17/laok/base/ser/_pickle.py
+-rw-rw-rw-   0        0        0      719 2023-04-25 06:50:29.000000 laok-0.2.17/laok/base/ser/numpy_.py
+-rw-rw-rw-   0        0        0      778 2023-04-25 06:50:29.000000 laok-0.2.17/laok/base/ser/torch_.py
+-rw-rw-rw-   0        0        0     1361 2023-04-25 06:50:39.000000 laok-0.2.17/laok/base/ser/yaml_.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.298587 laok-0.2.17/laok/base/str/
+-rw-rw-rw-   0        0        0       65 2023-04-21 09:32:10.000000 laok-0.2.17/laok/base/str/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-04-21 09:32:29.000000 laok-0.2.17/laok/base/str/fmt.py
+-rw-rw-rw-   0        0        0     1924 2023-04-19 08:08:18.000000 laok-0.2.17/laok/base/str/misc.py
+-rw-rw-rw-   0        0        0     2599 2023-04-21 09:30:50.000000 laok-0.2.17/laok/base/str/print_info.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.300581 laok-0.2.17/laok/base/sys_/
+-rw-rw-rw-   0        0        0       26 2023-05-04 15:23:17.000000 laok-0.2.17/laok/base/sys_/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.17/laok/base/sys_/platform_.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.302576 laok-0.2.17/laok/base/test/
+-rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.17/laok/base/test/__init__.py
+-rw-rw-rw-   0        0        0     8032 2023-04-19 15:30:44.000000 laok-0.2.17/laok/base/test/_dump.py
+-rw-rw-rw-   0        0        0     4551 2023-03-03 02:51:53.000000 laok-0.2.17/laok/base/test/_run.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.303573 laok-0.2.17/laok/cv2d/
+-rw-rw-rw-   0        0        0       22 2023-04-21 08:27:09.000000 laok-0.2.17/laok/cv2d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.304573 laok-0.2.17/laok/cv3d/
+-rw-rw-rw-   0        0        0       64 2023-04-21 09:21:19.000000 laok-0.2.17/laok/cv3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.305568 laok-0.2.17/laok/cv3d/io/
+-rw-rw-rw-   0        0        0       24 2023-04-21 09:18:03.000000 laok-0.2.17/laok/cv3d/io/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-04-25 06:52:21.000000 laok-0.2.17/laok/cv3d/io/_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.306565 laok-0.2.17/laok/cv3d/show/
+-rw-rw-rw-   0        0        0       21 2023-04-21 09:20:03.000000 laok-0.2.17/laok/cv3d/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.307563 laok-0.2.17/laok/cv3d/show/vtk_/
+-rw-rw-rw-   0        0        0      804 2023-04-21 09:21:01.000000 laok-0.2.17/laok/cv3d/show/vtk_/__init__.py
+-rw-rw-rw-   0        0        0     3916 2022-10-21 10:13:38.000000 laok-0.2.17/laok/cv3d/show/vtk_/win.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.314544 laok-0.2.17/laok/cv3d/trans/
+-rw-rw-rw-   0        0        0      192 2023-04-28 03:50:43.000000 laok-0.2.17/laok/cv3d/trans/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-04-25 05:31:18.000000 laok-0.2.17/laok/cv3d/trans/_dropout.py
+-rw-rw-rw-   0        0        0      726 2023-04-25 05:40:44.000000 laok-0.2.17/laok/cv3d/trans/_jitter.py
+-rw-rw-rw-   0        0        0      660 2023-04-25 03:33:54.000000 laok-0.2.17/laok/cv3d/trans/_normal.py
+-rw-rw-rw-   0        0        0     5025 2023-04-27 08:53:41.000000 laok-0.2.17/laok/cv3d/trans/_rotate.py
+-rw-rw-rw-   0        0        0     2164 2023-04-28 03:50:24.000000 laok-0.2.17/laok/cv3d/trans/_sample.py
+-rw-rw-rw-   0        0        0      618 2023-04-25 02:57:52.000000 laok-0.2.17/laok/cv3d/trans/_scale.py
+-rw-rw-rw-   0        0        0      485 2023-04-25 03:05:55.000000 laok-0.2.17/laok/cv3d/trans/_torch.py
+-rw-rw-rw-   0        0        0      680 2023-04-25 05:38:23.000000 laok-0.2.17/laok/cv3d/trans/_translate.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.315541 laok-0.2.17/laok/dnn/
+-rw-rw-rw-   0        0        0       87 2023-04-23 12:48:28.000000 laok-0.2.17/laok/dnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.316539 laok-0.2.17/laok/dnn/backbones/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/backbones/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.317536 laok-0.2.17/laok/dnn/dataset/
+-rw-rw-rw-   0        0        0       58 2023-04-25 06:10:55.000000 laok-0.2.17/laok/dnn/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.317536 laok-0.2.17/laok/dnn/dataset/cld/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/dataset/cld/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.318534 laok-0.2.17/laok/dnn/dataset/img/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/dataset/img/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.319530 laok-0.2.17/laok/dnn/dataset/txt/
+-rw-rw-rw-   0        0        0       38 2023-04-25 06:10:39.000000 laok-0.2.17/laok/dnn/dataset/txt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.321526 laok-0.2.17/laok/dnn/head/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/head/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-04-23 13:35:33.000000 laok-0.2.17/laok/dnn/head/classify.py
+-rw-rw-rw-   0        0        0     3178 2023-04-23 13:32:56.000000 laok-0.2.17/laok/dnn/head/detect.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.322522 laok-0.2.17/laok/dnn/layer/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/layer/__init__.py
+-rw-rw-rw-   0        0        0     2903 2023-04-25 02:35:22.000000 laok-0.2.17/laok/dnn/layer/pooling.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.323520 laok-0.2.17/laok/dnn/loss/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.324517 laok-0.2.17/laok/dnn/model/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/model/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-04-23 13:41:53.000000 laok-0.2.17/laok/dnn/model/_torch_vision.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.325514 laok-0.2.17/laok/dnn/neck/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.17/laok/dnn/neck/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.326511 laok-0.2.17/laok/ext/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.17/laok/ext/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.327509 laok-0.2.17/laok/ext/flask_/
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.17/laok/ext/flask_/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.17/laok/ext/flask_/app.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.329503 laok-0.2.17/laok/ext/flask_/basic/
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.17/laok/ext/flask_/basic/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.17/laok/ext/flask_/basic/views.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.330501 laok-0.2.17/laok/ext/numpy_/
+-rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.17/laok/ext/numpy_/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-04-19 07:45:14.000000 laok-0.2.17/laok/ext/onnx_.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.330501 laok-0.2.17/laok/ext/torch_/
+-rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.17/laok/ext/torch_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.332496 laok-0.2.17/laok/ext/torch_/datasets/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.335489 laok-0.2.17/laok/ext/torch_/datasets/kitti/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/__init__.py
+-rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/kitti.py
+-rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/obj.py
+-rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/kitti/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.339477 laok-0.2.17/laok/ext/torch_/datasets/model_net/
+-rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/__init__.py
+-rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net.py
+-rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_ineratia.py
+-rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_normals.py
+-rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.17/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.340474 laok-0.2.17/laok/ext/torch_/datasets/shape_net/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/shape_net/__init__.py
+-rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/shape_net/shape_net.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.342469 laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/__init__.py
+-rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.17/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py
+-rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.17/laok/ext/torch_/datasets/ustc_lidar.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.345461 laok-0.2.17/laok/ext/torch_/io/
+-rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/img.py
+-rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/jit.py
+-rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/model.py
+-rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/io/onnx.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.349452 laok-0.2.17/laok/ext/torch_/op/
+-rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.17/laok/ext/torch_/op/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.17/laok/ext/torch_/op/device.py
+-rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.17/laok/ext/torch_/op/module.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.17/laok/ext/torch_/op/print_info.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.354437 laok-0.2.17/laok/ext/torch_/trainval/
+-rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.17/laok/ext/torch_/trainval/__init__.py
+-rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.17/laok/ext/torch_/trainval/check_point.py
+-rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.17/laok/ext/torch_/trainval/infer.py
+-rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.17/laok/ext/torch_/trainval/train.py
+-rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.17/laok/ext/torch_/trainval/val.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.355435 laok-0.2.17/laok/ml/
+-rw-rw-rw-   0        0        0        0 2023-04-21 09:13:48.000000 laok-0.2.17/laok/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.355435 laok-0.2.17/laok/tool/
+-rw-rw-rw-   0        0        0        0 2023-05-04 12:52:02.000000 laok-0.2.17/laok/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.357429 laok-0.2.17/laok/tool/ultralytics_/
+-rw-rw-rw-   0        0        0       28 2023-05-04 12:43:29.000000 laok-0.2.17/laok/tool/ultralytics_/__init__.py
+-rw-rw-rw-   0        0        0      100 2023-05-04 12:56:44.000000 laok-0.2.17/laok/tool/ultralytics_/__main__.py
+-rw-rw-rw-   0        0        0     2094 2023-05-04 14:42:16.000000 laok-0.2.17/laok/tool/ultralytics_/train_det.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:26:37.267669 laok-0.2.17/laok.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-05-05 09:26:36.000000 laok-0.2.17/laok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3661 2023-05-05 09:26:37.000000 laok-0.2.17/laok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:26:36.000000 laok-0.2.17/laok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-05 09:26:36.000000 laok-0.2.17/laok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:26:37.359424 laok-0.2.17/setup.cfg
+-rw-rw-rw-   0        0        0      325 2023-05-05 09:24:17.000000 laok-0.2.17/setup.py
```

### Comparing `laok-0.2.16/laok/cv2d/misc/_data.py` & `laok-0.2.17/laok/base/fs/name_index.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
-Created on 2022/5/26 11:04:35
-
+Created on 2023/4/19 17:21:57
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
-import types
-from pathlib import Path
-import cv2, numpy as np
-from laok.cv2d.gui import show, show_wait
+from collections import OrderedDict
+from ..str import dict_to_str
+from .fdata import file_read_lines
 #===============================================================================
-'''     
+r'''
 '''
 #===============================================================================
-__all__ = ['read_smaple_img', 'run_sample_image']
+__all__ = ['NameIndexFile', 'cls_to_name']
+
+# 根据配置文件获取索引
+class NameIndexFile:
+    def __init__(self, cls_file = None):
+        self.cls_data_ = OrderedDict()
+        if cls_file:
+            self.setClsFile(cls_file)
+
+    def setClsFile(self, cls_file):
+        for i,line in enumerate(file_read_lines(cls_file)):
+            self.cls_data_[i] = line
+        return self
+
+    def getName(self, idx):
+        _idx = int(idx)
+        return self.cls_data_.get(_idx, '')
+
+    def getIndex(self, name):
+        if name:
+            for _idx, _name in self.cls_data_.items():
+                if name in _name:
+                    return _idx
+        return -1
+
+    def getData(self):
+        return self.cls_data_
+
+    def show(self, start=10, stop=10):
+        val = dict_to_str(self.cls_data_, start, stop)
+        print(val)
+
 
-def read_smaple_img(is_color=True):
-    fPath = Path(__file__).parent.joinpath('lena.jpg')
-    flags = cv2.IMREAD_COLOR if is_color else cv2.IMREAD_GRAYSCALE
-    return cv2.imdecode(np.fromfile(fPath, dtype=np.uint8), flags=flags)
-
-def _get_name(trans):
-    if hasattr(trans, '__name__'):
-        return trans.__name__
-    if hasattr(trans, 'func'):
-        return trans.func.__name__
-    if hasattr(trans, '__class__'):
-        return trans.__class__.__name__
-
-def run_sample_image(trans, is_color=True):
-    img = read_smaple_img(is_color)
-    img_trans = trans(img)
-    show(img_trans, _get_name(trans))
-    show_wait(img)
+def cls_to_name(index, filename):
+    nameIdx = NameIndexFile(filename)
+    return nameIdx.getName(index)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `laok-0.2.16/laok/util/network.py` & `laok-0.2.17/laok/base/net/ip.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,7 +20,9 @@
         IP = st.getsockname()[0]
     except Exception:
         IP = '127.0.0.1'
     finally:
         st.close()
     return IP
 
+if __name__ == '__main__':
+    print('get_ip =', get_ip())
```

### Comparing `laok-0.2.16/laok/util/onnx_.py` & `laok-0.2.17/laok/ext/onnx_.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 Created on 2022/4/19 11:14:26
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import onnx
 import onnxruntime
-import laok.util.fpath as kpath
+import laok
 #===============================================================================
 '''
 '''
 #===============================================================================
-
 def check_model(onnxFile):
     '''check onnx model if it is valide
     :param onnxFile:
     :return:
     '''
     model = onnx.load_model(onnxFile)
     onnx.checker.check_model(model)
@@ -25,16 +24,15 @@
 def load_model(onnxFile):
     '''
     :param onnxFile:
     :return:
     '''
     return onnx.load_model(onnxFile)
 
-
-def __fmt_NodeArg(nodes):
+def __fmt_node_arg(nodes):
     msg_list = []
     for node in nodes:
         shape_name = "(" + ", ".join( str(s) for s in node.shape) + ")"
         msg_list.append(f'    {node.name} : {shape_name} , type={node.type}')
     return msg_list
 
 def dump_model_info(onnxFile, graphFile = None, skip_exist = False, show_info = True):
@@ -42,17 +40,17 @@
     :param onnxFile:
     :param graphFile:
     :param skip_exist:
     :param show_info:
     :return:
     '''
     if graphFile is None:
-        graphFile = kpath.path_replace_ext(onnxFile, '.graph')
+        graphFile = laok.path_replace_ext(onnxFile, '.graph')
 
-    if skip_exist and kpath.path_exist(graphFile):
+    if skip_exist and laok.path_exist(graphFile):
         return graphFile
 
     if show_info:
         print(f'start read... {onnxFile}')
 
     msg_list = []
     ###################### onnxruntime的模型信息
@@ -66,25 +64,25 @@
     msg_list.append(f'    description:{meta.description}')
     msg_list.append(f'    graph_description:{meta.graph_description}')
     msg_list.append(f'    version:{meta.version}')
 
     # 获取输入信息
     inputs = ort_session.get_inputs()
     msg_list.append(f'\n\nInput Node Name/Shape [{len(inputs)}]:')
-    msg_list.extend(__fmt_NodeArg(inputs))
+    msg_list.extend(__fmt_node_arg(inputs))
 
     # 获取输出信息
     outputs = ort_session.get_outputs()
     msg_list.append(f'\n\nOutput Node Name/Shape [{len(outputs)}]:')
-    msg_list.extend(__fmt_NodeArg(outputs))
+    msg_list.extend(__fmt_node_arg(outputs))
 
     # 获取重载初始化
     overinits = ort_session.get_overridable_initializers()
     msg_list.append(f'\n\nOverridableInitializer Node Name/Shape [{len(overinits)}]:')
-    msg_list.extend(__fmt_NodeArg(overinits))
+    msg_list.extend(__fmt_node_arg(overinits))
 
 
     ###################### onnx 的模型信息
     try:
         model = onnx.load_model(onnxFile)
         graph = onnx.helper.printable_graph(model.graph)
         msg_list.append("\n\n" + graph)
```

### Comparing `laok-0.2.16/laok/util/parallel.py` & `laok-0.2.17/laok/base/parallel/pool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,45 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
-'''
-Created on 2022/4/19 13:51:55
-
-@author: LiuKuan
-@copyright: Apache License, Version 2.0
-'''
-import threading
-import concurrent.futures as futures
-from .fpath import (files_under as _files_under,
-                    files_cur as _files_current,
-                    dirs_cur as _dirs_current,
-                    dirs_under as _dirs_under)
-#===============================================================================
-'''     
-'''
-#===============================================================================
-
-__all__ = ['thread_id', 'thread_count', 'paral_seq', 'files_under', 'files_cur', 'dirs_under', 'dirs_cur', ]
-
-####################    线城接口
-def thread_id():
-    return threading.get_ident()
-
-def thread_count():
-    return threading.active_count()
-
-####################    并行接口
-def paral_seq(data_list, handler, max_workers=None, use_thread = True):
-    if use_thread:
-        Executor = futures.ThreadPoolExecutor
-    else:
-        Executor = futures.ProcessPoolExecutor
-
-    with Executor(max_workers=max_workers) as ex:
-        wait_for = [ex.submit(handler, data) for data in data_list]
-        return [f.result() for f in futures.as_completed(wait_for)]
-
-def files_under(dir_name, handler, suffix_list = None, need_join_dir=True, max_workers=None, use_thread = True):
-    '''
-    '''
-    data_iter = _files_under(dir_name, suffix_list, need_join_dir)
-    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
-
-def files_cur(dir_name, handler, suffix_list = None, need_join_dir=True, max_workers=None, use_thread = True):
-    '''
-    '''
-    data_iter = _files_current(dir_name, suffix_list, need_join_dir)
-    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
-
-def dirs_under(dir_name, handler, suffix_list = None, need_join_dir=True, max_workers=None, use_thread = True):
-    '''
-    '''
-    data_iter = _dirs_under(dir_name, suffix_list, need_join_dir)
-    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
-
-def dirs_cur(dir_name, handler, suffix_list = None, need_join_dir=True, max_workers=None, use_thread = True):
-    '''
-    '''
-    data_iter = _dirs_current(dir_name, suffix_list, need_join_dir)
-    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
-
-
+#! /usr/bin/env python
+# -*- coding: utf-8 -*-
+'''
+Created on 2022/4/19 13:51:55
+
+@author: LiuKuan
+@copyright: Apache License, Version 2.0
+'''
+import threading
+import concurrent.futures as futures
+from ..fs import (files_under, files_cur, dirs_cur, dirs_under)
+#===============================================================================
+'''     
+'''
+#===============================================================================
+__all__ = ['thread_id', 'thread_count', 'paral_seq', 'paral_files_under', 'paral_files_cur', 'paral_dirs_under', 'paral_dirs_cur', ]
+
+def thread_id():
+    return threading.get_ident()
+
+def thread_count():
+    return threading.active_count()
+
+####################    并行接口
+def paral_seq(data_list, handler, max_workers=None, use_thread = True):
+    Executor = futures.ThreadPoolExecutor if use_thread else futures.ProcessPoolExecutor
+    with Executor(max_workers=max_workers) as ex:
+        wait_for = [ex.submit(handler, data) for data in data_list]
+        return [f.result() for f in futures.as_completed(wait_for)]
+
+def paral_files_under(dir_name, handler, suffix_list = None, max_workers=None, use_thread = True):
+    data_iter = files_under(dir_name, suffix_list)
+    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
+
+def paral_files_cur(dir_name, handler, suffix_list = None, max_workers=None, use_thread = True):
+    data_iter = files_cur(dir_name, suffix_list)
+    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
+
+def paral_dirs_under(dir_name, handler, suffix_list = None, max_workers=None, use_thread = True):
+    data_iter = dirs_under(dir_name, suffix_list)
+    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
+
+def paral_dirs_cur(dir_name, handler, suffix_list = None, max_workers=None, use_thread = True):
+    data_iter = dirs_cur(dir_name, suffix_list)
+    return paral_seq(data_iter, handler, max_workers=max_workers, use_thread=use_thread)
```

