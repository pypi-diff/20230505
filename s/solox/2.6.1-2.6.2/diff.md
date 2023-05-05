# Comparing `tmp/solox-2.6.1.tar.gz` & `tmp/solox-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-9295ic1y/solox-2.6.1.tar", last modified: Thu May  4 03:02:47 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-od_7kf29/solox-2.6.2.tar", last modified: Fri May  5 03:08:10 2023, max compression
```

## Comparing `solox-2.6.1.tar` & `solox-2.6.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-04 03:02:34.000000 solox-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 03:02:34.000000 solox-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-04 03:02:47.000000 solox-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-04 03:02:34.000000 solox-2.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-04 03:02:47.000000 solox-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 03:02:34.000000 solox-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 03:02:34.000000 solox-2.6.1/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-04 03:02:34.000000 solox-2.6.1/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 03:02:34.000000 solox-2.6.1/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-04 03:02:34.000000 solox-2.6.1/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-04 03:02:34.000000 solox-2.6.1/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/analysis_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)   100609 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-04 03:02:34.000000 solox-2.6.1/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 03:02:34.000000 solox-2.6.1/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-05-04 03:02:34.000000 solox-2.6.1/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-04 03:02:34.000000 solox-2.6.1/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-04 03:02:34.000000 solox-2.6.1/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 03:02:47.000000 solox-2.6.1/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-05 03:08:00.000000 solox-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 03:08:00.000000 solox-2.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-05 03:08:10.000000 solox-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-05 03:08:00.000000 solox-2.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-05 03:08:10.000000 solox-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 03:08:00.000000 solox-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 03:08:00.000000 solox-2.6.2/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 03:08:00.000000 solox-2.6.2/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-05 03:08:00.000000 solox-2.6.2/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-05 03:08:00.000000 solox-2.6.2/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-05 03:08:00.000000 solox-2.6.2/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   100609 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-05 03:08:00.000000 solox-2.6.2/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 03:08:00.000000 solox-2.6.2/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-05-05 03:08:00.000000 solox-2.6.2/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-05 03:08:00.000000 solox-2.6.2/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-05 03:08:00.000000 solox-2.6.2/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 03:08:10.000000 solox-2.6.2/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.1/LICENSE` & `solox-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/setup.py` & `solox-2.6.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     install_requires=['flask>=2.0.1', 'requests', 'logzero', 'Flask-SocketIO==4.3.1', 'fire',
                       'python-engineio==3.13.2', 'python-socketio==4.6.0', 'Werkzeug==2.0.3',
-                      'Jinja2==3.0.1','tidevice==0.9.7', 'tqdm', 'xlwt','py-ios-device'],
+                      'Jinja2==3.0.1','tidevice==0.9.7', 'tqdm', 'xlwt'],
     version=__version__,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="SoloX - Real-time collection tool for Android/iOS performance data.",
     packages=setuptools.find_namespace_packages(include=["solox", "solox.*"], ),
     include_package_data=True
 )
```

### Comparing `solox-2.6.1/solox/__main__.py` & `solox-2.6.2/solox/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/debug.py` & `solox-2.6.2/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/_iosPerf.py` & `solox-2.6.2/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/adb/mac/adb` & `solox-2.6.2/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/adb.py` & `solox-2.6.2/solox/public/adb.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/apm.py` & `solox-2.6.2/solox/public/apm.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,24 +267,26 @@
     def getAndroidFps(self, noLog=False):
         """get Android Fps, unit:HZ"""
         monitors = FPSMonitor(device_id=self.deviceId, package_name=self.pkgName, frequency=1,
                               surfaceview=self.surfaceview, start_time=TimeUtils.getCurrentTimeUnderline())
         monitors.start()
         fps, jank = monitors.stop()
         if noLog is False:
+            time.sleep(1)
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'fps.log'), apm_time, fps)
             f.add_log(os.path.join(f.report_dir,'jank.log'), apm_time, jank)
         return fps, jank
 
     def getiOSFps(self, noLog=False):
         """get iOS Fps"""
         apm = iosAPM(self.pkgName)
         fps = int(apm.getPerformance(apm.fps))
         if noLog is False:
+            time.sleep(1)
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'fps.log'), apm_time, fps)
         return fps, 0
 
     def getFPS(self, noLog=False):
         """get fps、jank"""
         fps, jank = self.getAndroidFps(noLog) if self.platform == Platform.Android else self.getiOSFps(noLog)
@@ -294,14 +296,15 @@
     def __init__(self, pkgName):
         self.pkgName = pkgName
 
     def getGPU(self, noLog=False):
         apm = iosAPM(self.pkgName)
         gpu = apm.getPerformance(apm.gpu)
         if noLog is False:
+            time.sleep(1)
             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
             f.add_log(os.path.join(f.report_dir,'gpu.log'), apm_time, gpu)
         return gpu   
 
 class iosAPM(object):
 
     def __init__(self, pkgName, deviceId=tidevice.Device()):
```

### Comparing `solox-2.6.1/solox/public/apm_pk.py` & `solox-2.6.2/solox/public/apm_pk.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/common.py` & `solox-2.6.2/solox/public/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,19 @@
             raise Exception('no activity found')
 
     def getStartupTimeByAndroid(self, activity, deviceId):
         result = adb.shell(cmd='am start -W {}'.format(activity), deviceId=deviceId)
         return result
 
     def getStartupTimeByiOS(self, pkgname):
-        result = self.execCmd('pyidevice instruments app_lifecycle -b {}'.format(pkgname))
+        try:
+            import ios_device
+        except ImportError:
+            logger.error('py-ios-devices not found, please run [pip install py-ios-devices]') 
+        result = self.execCmd('pyidevice instruments app_lifecycle -b {}'.format(pkgname))       
         return result          
 
 class File:
 
     def __init__(self, fileroot='.'):
         self.fileroot = fileroot
         self.report_dir = self.get_repordir()
```

### Comparing `solox-2.6.1/solox/public/fps.py` & `solox-2.6.2/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/__main__.py` & `solox-2.6.2/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_crash.py` & `solox-2.6.2/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_device.py` & `solox-2.6.2/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_hexdump.py` & `solox-2.6.2/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_imagemounter.py` & `solox-2.6.2/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_installation.py` & `solox-2.6.2/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_instruments.py` & `solox-2.6.2/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_ipautil.py` & `solox-2.6.2/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_perf.py` & `solox-2.6.2/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_proto.py` & `solox-2.6.2/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_relay.py` & `solox-2.6.2/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_safe_socket.py` & `solox-2.6.2/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_ssl.py` & `solox-2.6.2/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_sync.py` & `solox-2.6.2/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_types.py` & `solox-2.6.2/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_usbmux.py` & `solox-2.6.2/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_utils.py` & `solox-2.6.2/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.2/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/bplist.py` & `solox-2.6.2/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/exceptions.py` & `solox-2.6.2/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/plistlib2.py` & `solox-2.6.2/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.2/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/iosperf/struct2.py` & `solox-2.6.2/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/report_template/android.html` & `solox-2.6.2/solox/public/report_template/android.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/public/report_template/ios.html` & `solox-2.6.2/solox/public/report_template/ios.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/highlight.min.css` & `solox-2.6.2/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.2/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/select2.min.css` & `solox-2.6.2/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/sweetalert2.min.css` & `solox-2.6.2/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/tabler.demo.min.css` & `solox-2.6.2/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/css/tabler.min.css` & `solox-2.6.2/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/404.png` & `solox-2.6.2/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/500.png` & `solox-2.6.2/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/avatar.png` & `solox-2.6.2/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/coffee.png` & `solox-2.6.2/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/empty.png` & `solox-2.6.2/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/readme/home.png` & `solox-2.6.2/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/image/readme/pk.png` & `solox-2.6.2/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/apexcharts.js` & `solox-2.6.2/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/gray.js` & `solox-2.6.2/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/highlight.min.js` & `solox-2.6.2/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/highstock.js` & `solox-2.6.2/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/html2canvas.min.js` & `solox-2.6.2/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/jquery.min.js` & `solox-2.6.2/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/select2.min.js` & `solox-2.6.2/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/socket.io.js` & `solox-2.6.2/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/sweetalert2.min.js` & `solox-2.6.2/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/tabler.demo.min.js` & `solox-2.6.2/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/js/tabler.min.js` & `solox-2.6.2/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/static/logo/logo.png` & `solox-2.6.2/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/404.html` & `solox-2.6.2/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/500.html` & `solox-2.6.2/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/analysis.html` & `solox-2.6.2/solox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/analysis_compare.html` & `solox-2.6.2/solox/templates/analysis_compare.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/analysis_pk.html` & `solox-2.6.2/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/base.html` & `solox-2.6.2/solox/templates/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.1
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.2
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.1
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.2
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * Warning_Value
     * Timer
     * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
```

### Comparing `solox-2.6.1/solox/templates/index.html` & `solox-2.6.2/solox/templates/index.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/pk.html` & `solox-2.6.2/solox/templates/pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/templates/report.html` & `solox-2.6.2/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/view/apis.py` & `solox-2.6.2/solox/view/apis.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/view/pages.py` & `solox-2.6.2/solox/view/pages.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox/web.py` & `solox-2.6.2/solox/web.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.1/solox.egg-info/SOURCES.txt` & `solox-2.6.2/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

