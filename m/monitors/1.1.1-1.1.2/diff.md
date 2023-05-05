# Comparing `tmp/monitors-1.1.1.tar.gz` & `tmp/monitors-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/utx-monitors/utx-monitors/dist/tmpqw_9vi4t/monitors-1.1.1.tar", last modified: Wed Jun 15 03:27:11 2022, max compression
+gzip compressed data, was "/home/runner/work/utx-monitors/utx-monitors/dist/.tmp-629bxe_u/monitors-1.1.2.tar", last modified: Fri May  5 13:22:43 2023, max compression
```

## Comparing `monitors-1.1.1.tar` & `monitors-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-06-15 03:26:54.000000 monitors-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-06-15 03:26:54.000000 monitors-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4952 2022-06-15 03:27:11.000000 monitors-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3929 2022-06-15 03:26:54.000000 monitors-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors/
--rw-r--r--   0 runner    (1001) docker     (116)      110 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      932 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/default.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (116)     1001 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/monitor_pid.py
--rw-r--r--   0 runner    (1001) docker     (116)      619 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/monitor_set.py
--rw-r--r--   0 runner    (1001) docker     (116)    17983 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/monitor_util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors/page/
--rw-r--r--   0 runner    (1001) docker     (116)      130 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8945 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors/page/classifier/
--rw-r--r--   0 runner    (1001) docker     (116)      196 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18657 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/classifier/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     7139 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/classifier/keras.py
--rw-r--r--   0 runner    (1001) docker     (116)     1174 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/classifier/ssim.py
--rw-r--r--   0 runner    (1001) docker     (116)     6158 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/classifier/svm.py
--rw-r--r--   0 runner    (1001) docker     (116)      293 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     3907 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/core.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors/page/cutter/
--rw-r--r--   0 runner    (1001) docker     (116)      108 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/cutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5557 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/cutter/cut_range.py
--rw-r--r--   0 runner    (1001) docker     (116)    21283 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/cutter/cut_result.py
--rw-r--r--   0 runner    (1001) docker     (116)     8665 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/cutter/cutter.py
--rw-r--r--   0 runner    (1001) docker     (116)     8596 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/hook.py
--rw-r--r--   0 runner    (1001) docker     (116)    12143 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors/page/template/
--rw-r--r--   0 runner    (1001) docker     (116)    11132 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/template/report.html
--rw-r--r--   0 runner    (1001) docker     (116)    10324 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/template/summary_template.html
--rw-r--r--   0 runner    (1001) docker     (116)    10243 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (116)     6402 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/page/video.py
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2022-06-15 03:26:54.000000 monitors-1.1.1/monitors/tradition.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4952 2022-06-15 03:27:10.000000 monitors-1.1.1/monitors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      927 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      274 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-06-15 03:27:11.000000 monitors-1.1.1/monitors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-15 03:27:11.000000 monitors-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1998 2022-06-15 03:26:54.000000 monitors-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 13:22:32.000000 monitors-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 13:22:32.000000 monitors-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-05 13:22:43.000000 monitors-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-05 13:22:32.000000 monitors-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/monitor_pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/monitor_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/monitor_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors/page/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors/page/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/classifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/classifier/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/classifier/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/classifier/svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors/page/cutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/cutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/cutter/cut_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/cutter/cut_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/cutter/cutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors/page/template/
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/template/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/template/summary_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/page/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-05 13:22:32.000000 monitors-1.1.2/monitors/tradition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 13:22:43.000000 monitors-1.1.2/monitors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:22:43.000000 monitors-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-05 13:22:32.000000 monitors-1.1.2/setup.py
```

### Comparing `monitors-1.1.1/LICENSE` & `monitors-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/PKG-INFO` & `monitors-1.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: monitors
-Version: 1.1.1
-Summary: monitor tools
-Home-page: https://github.com/openutx
-Author: lijiawei
-Author-email: jiawei.li2@qq.com
-License: MIT Licence
-Keywords: grafana,monitors,process monitor,system monitor,influxdb
-Platform: any
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console :: Curses
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: System :: Networking :: Monitoring
-Classifier: Topic :: Software Development :: Testing
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # monitors
 
 
 [![Build Status](https://travis-ci.com/Pactortester/monitors.svg?branch=master)](https://travis-ci.com/Pactortester/monitors) ![PyPI](https://img.shields.io/pypi/v/monitors) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monitors) ![GitHub top language](https://img.shields.io/github/languages/top/Pactortester/monitors) [![Downloads](https://pepy.tech/badge/monitors)](https://pepy.tech/project/monitors) ![GitHub stars](https://img.shields.io/github/stars/Pactortester/monitors?style=social) ![https://blog.csdn.net/flower_drop](https://img.shields.io/badge/csdn-%40flower__drop-orange)
 
 
 ## Logo
@@ -139,14 +112,27 @@
 
 ![](https://files.mdnice.com/user/17535/dce8bbb5-2a5c-4ac6-abac-4f9f8c43a620.png)
 
 ## 后续方案
 
 在推广使用过程中，发现尽管已经做的如此简单，还是有同学不会使用，一步三个坑，后续我计划把【minitors】监控服务，打包成可执行文件，有完整的页面交互，防止大家掉坑！
 
+## 视频分析
 
+```
+          点击应用图标              弹窗1   关闭弹窗1     欢迎页     滑动欢迎页    弹窗2    关闭弹窗2   首页
+              ^                     ^                   ^                     ^                  ^ 
+              |                     |                   |                     |                  |
+              |---------logo1-------|-------logo2-------|--------.......------|------......------|
+
+稳定阶段（个）： 2         1          1         1          1                     1                  2
+
+              |                     |                   |                     |                  |
+              v                     v                   v                     v                  v
+              A                     B                   C                     D                  E
+```
 
 ## 
 
 以上便是 monitors 的基本用法介绍。
 
 如果您有发现错误，或者您对 monitors 有任何建议，欢迎到 [monitors Issues](https://github.com/Pactortester/monitors/issues) 发表，非常感谢您的支持。您的反馈和建议非常宝贵，希望您的参与能帮助 monitors 做得更好。
```

### Comparing `monitors-1.1.1/monitors/default.py` & `monitors-1.1.2/monitors/default.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/dynamic.py` & `monitors-1.1.2/monitors/dynamic.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/monitor_pid.py` & `monitors-1.1.2/monitors/monitor_pid.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/monitor_set.py` & `monitors-1.1.2/monitors/monitor_set.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/monitor_util.py` & `monitors-1.1.2/monitors/monitor_util.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/api.py` & `monitors-1.1.2/monitors/page/api.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/classifier/base.py` & `monitors-1.1.2/monitors/page/classifier/base.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/classifier/keras.py` & `monitors-1.1.2/monitors/page/classifier/keras.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/classifier/ssim.py` & `monitors-1.1.2/monitors/page/classifier/ssim.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/classifier/svm.py` & `monitors-1.1.2/monitors/page/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/core.py` & `monitors-1.1.2/monitors/page/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     :param height: video resolution
     :param width: video resolution
     :param original_path: first-hand video path
     :param device_name: device name
     :return:
     """
     global end, start
+    # end = 0
+    # start = 0
 
     if len(list(find_all_cases(base=original_path, types='files', mark='.mp4'))) == 0:
         logger.warning(f'{original_path} No video files to analyze !')
         return
 
     if os.path.isdir(video_path):
         shutil.rmtree(video_path)
@@ -59,47 +61,66 @@
 
         # 0阶段中的倒序第一个时间段0。如果0是最后几帧，就用倒序第二个时间段 以此类推
         # 如果分析后产生的数据中并没有0阶段，取下一个阶段1。以此类推
         try:
             reversed_result = result_dict['0']
         except KeyError as e:
             logger.error(f"第0阶段不存在：{e}")
-            reversed_result = result_dict['1']
-        for i in reversed_result:
+            reversed_result = result_dict.get('1')
+            if not reversed_result:
+                reversed_result = result_dict.get('2')
+        for i in reversed(reversed_result):
             if float(str(i[-1]).replace('>', '').split('timestamp=')[1]) < 1:
                 start = i
                 break
             else:
                 start = reversed_result[-1]
-
-        logger.info(reversed_result)
-        logger.info(start)
-
         if isinstance(start, list):
             start = str(start[-1]).replace('>', '').split('timestamp=')[1]
         else:
             start = str(start).replace('>', '').split('timestamp=')[1]
-        logger.info(start)
+        logger.info(f'start collection: {reversed_result}')
+        logger.info(f'start time: {start}')
 
         # 2阶段中的第一个时间段0。如果0是前几帧，就用第二个时间段 以此类推
-        for s in result_dict['2']:
-            if float(str(s[0]).replace('>', '').split('timestamp=')[1]) > 0.5:
-                end = s
-                break
+        try:
+            positive_order_result = result_dict['2']
+            for s in positive_order_result:
+                if float(str(s[0]).replace('>', '').split('timestamp=')[1]) > 0.5:
+                    end = s
+                    break
+                else:
+                    end = positive_order_result[0]
+            logger.info(f'end collection: {positive_order_result}')
+            logger.info(f'end time: {end}')
+
+            if isinstance(end, list):
+                end = str(end[0]).replace('>', '').split('timestamp=')[1]
             else:
-                end = result_dict['2'][0]
-        logger.info(result_dict['2'])
-        logger.info(end)
+                end = str(end).replace('>', '').split('timestamp=')[1]
+            logger.info(end)
+        except KeyError as e:
+            logger.error(f"第2阶段不存在: {e}")
+            positive_order_result = result_dict['1']
+            end = positive_order_result[-1]
+            logger.info(f'end collection: {positive_order_result}')
+            logger.info(f'end time: {end}')
 
-        if isinstance(end, list):
-            end = str(end[0]).replace('>', '').split('timestamp=')[1]
-        else:
-            end = str(end).replace('>', '').split('timestamp=')[1]
-        logger.info(end)
+            if isinstance(end, list):
+                end = str(end[-1]).replace('>', '').split('timestamp=')[1]
+            else:
+                end = str(end).replace('>', '').split('timestamp=')[1]
+            logger.info(end)
+        try:
+            cost = abs(round((float(end) - float(start)) * 1000))
+            logger.info(f'cost time: {cost}')
+        except ValueError:
+            cost = 'abnormal video'
+            logger.error(f'cost time: {cost}')
 
-        cost = float(end) - float(start)
-        logger.info(round(cost * 1000))
         # 取正整数，保证报告数据展示正常
-        detail.append({'name': case_name, 'cost': abs(round(cost * 1000))})
+        detail.append({'name': case_name, 'cost': cost})
 
     gen_report(results=report_results, report_path=summary_report_path)
+    logger.info(detail)
     logger.info('end of prediction！')
+    return detail
```

### Comparing `monitors-1.1.1/monitors/page/cutter/cut_range.py` & `monitors-1.1.2/monitors/page/cutter/cut_range.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/cutter/cut_result.py` & `monitors-1.1.2/monitors/page/cutter/cut_result.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/cutter/cutter.py` & `monitors-1.1.2/monitors/page/cutter/cutter.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/hook.py` & `monitors-1.1.2/monitors/page/hook.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/reporter.py` & `monitors-1.1.2/monitors/page/reporter.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/template/report.html` & `monitors-1.1.2/monitors/page/template/report.html`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/template/summary_template.html` & `monitors-1.1.2/monitors/page/template/summary_template.html`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/toolbox.py` & `monitors-1.1.2/monitors/page/toolbox.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/page/video.py` & `monitors-1.1.2/monitors/page/video.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors/tradition.py` & `monitors-1.1.2/monitors/tradition.py`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/monitors.egg-info/PKG-INFO` & `monitors-1.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monitors
-Version: 1.1.1
+Version: 1.1.2
 Summary: monitor tools
 Home-page: https://github.com/openutx
 Author: lijiawei
 Author-email: jiawei.li2@qq.com
 License: MIT Licence
 Keywords: grafana,monitors,process monitor,system monitor,influxdb
 Platform: any
@@ -139,14 +139,27 @@
 
 ![](https://files.mdnice.com/user/17535/dce8bbb5-2a5c-4ac6-abac-4f9f8c43a620.png)
 
 ## 后续方案
 
 在推广使用过程中，发现尽管已经做的如此简单，还是有同学不会使用，一步三个坑，后续我计划把【minitors】监控服务，打包成可执行文件，有完整的页面交互，防止大家掉坑！
 
+## 视频分析
 
+```
+          点击应用图标              弹窗1   关闭弹窗1     欢迎页     滑动欢迎页    弹窗2    关闭弹窗2   首页
+              ^                     ^                   ^                     ^                  ^ 
+              |                     |                   |                     |                  |
+              |---------logo1-------|-------logo2-------|--------.......------|------......------|
+
+稳定阶段（个）： 2         1          1         1          1                     1                  2
+
+              |                     |                   |                     |                  |
+              v                     v                   v                     v                  v
+              A                     B                   C                     D                  E
+```
 
 ## 
 
 以上便是 monitors 的基本用法介绍。
 
 如果您有发现错误，或者您对 monitors 有任何建议，欢迎到 [monitors Issues](https://github.com/Pactortester/monitors/issues) 发表，非常感谢您的支持。您的反馈和建议非常宝贵，希望您的参与能帮助 monitors 做得更好。
```

### Comparing `monitors-1.1.1/monitors.egg-info/SOURCES.txt` & `monitors-1.1.2/monitors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monitors-1.1.1/setup.py` & `monitors-1.1.2/setup.py`

 * *Files identical despite different names*

