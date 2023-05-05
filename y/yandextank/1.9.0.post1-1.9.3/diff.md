# Comparing `tmp/yandextank-1.9.0.post1.tar.gz` & `tmp/yandextank-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandextank-1.9.0.post1.tar", last modified: Tue Sep  5 14:27:53 2017, max compression
+gzip compressed data, was "dist/yandextank-1.9.3.tar", last modified: Thu Oct 19 13:33:23 2017, max compression
```

## Comparing `yandextank-1.9.0.post1.tar` & `yandextank-1.9.3.tar`

### file list

```diff
@@ -1,194 +1,206 @@
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/
--rw-rw-r--   0 direvius (78873639) LD\Domain Users (593637566)       25 2015-02-09 15:19:04.000000 yandextank-1.9.0.post1/MANIFEST.in
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      985 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/PKG-INFO
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       63 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/setup.cfg
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3299 2017-09-05 14:26:46.000000 yandextank-1.9.0.post1/setup.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      200 2016-12-27 13:12:24.000000 yandextank-1.9.0.post1/yandextank/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/api/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       91 2016-12-27 13:43:10.000000 yandextank-1.9.0.post1/yandextank/api/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6566 2016-12-30 13:22:21.000000 yandextank-1.9.0.post1/yandextank/api/apiworker.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/api/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      706 2017-04-14 09:38:31.000000 yandextank-1.9.0.post1/yandextank/api/config/00-base.ini
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      847 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/api/config/00-base.yaml
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/common/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        0 2016-12-27 13:12:24.000000 yandextank-1.9.0.post1/yandextank/common/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      291 2016-12-27 13:12:24.000000 yandextank-1.9.0.post1/yandextank/common/exceptions.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5871 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/common/interfaces.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    12683 2016-12-30 13:22:21.000000 yandextank-1.9.0.post1/yandextank/common/resource.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    18544 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/common/util.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/config_converter/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/config_converter/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    16325 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/config_converter/converter.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/core/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       93 2016-12-27 13:17:07.000000 yandextank-1.9.0.post1/yandextank/core/__init__.py
--rwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)     2691 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/core/cli.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/core/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      682 2017-04-14 09:38:31.000000 yandextank-1.9.0.post1/yandextank/core/config/00-base.ini
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      893 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/core/config/00-base.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      170 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/core/config/plugins_schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      977 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/core/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    17694 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/core/consoleworker.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2385 2016-12-30 13:22:21.000000 yandextank-1.9.0.post1/yandextank/core/expvar.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    22346 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/core/tankcore.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      200 2016-12-27 13:12:29.000000 yandextank-1.9.0.post1/yandextank/plugins/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:41:47.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5275 2017-04-10 14:58:46.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/aggregator.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1209 2016-12-30 13:22:21.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/chopper.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      474 2016-04-15 13:01:12.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/config/phout.json
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       51 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4287 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Aggregator/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2017-04-10 14:58:46.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/binary/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)  1380128 2017-04-10 14:58:46.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/binary/lightning.apk
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      808 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/config/load-sample.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       28 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2623 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      221 2017-04-10 14:58:46.000000 yandextank-1.9.0.post1/yandextank/plugins/Android/reader.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Appium/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:33:19.000000 yandextank-1.9.0.post1/yandextank/plugins/Appium/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Appium/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      118 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Appium/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2409 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Appium/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       95 2016-12-27 13:33:12.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      122 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    11106 2016-12-30 13:22:22.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/criterions.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    21688 2016-12-30 13:38:15.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/cumulative_criterions.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5454 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Autostop/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/BatteryHistorian/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:33:03.000000 yandextank-1.9.0.post1/yandextank/plugins/BatteryHistorian/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/BatteryHistorian/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       58 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/BatteryHistorian/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2938 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/BatteryHistorian/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:58.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1446 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     9069 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/guns.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4027 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2535 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/reader.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1606 2016-12-30 13:22:22.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/widgets.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     9138 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Bfg/worker.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Console/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:32:47.000000 yandextank-1.9.0.post1/yandextank/plugins/Console/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Console/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      190 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Console/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5758 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Console/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    22082 2016-12-30 13:22:24.000000 yandextank-1.9.0.post1/yandextank/plugins/Console/screen.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-04-10 14:58:46.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5086 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/cli.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    21358 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/client.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1564 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    33045 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/DataUploader/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:42.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      317 2015-02-06 14:24:42.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/jmeter_var_template.xml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1799 2016-09-28 15:42:46.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/jmeter_writer.xml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3455 2016-09-28 15:42:46.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/jmeter_writer_ext.xml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      551 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     9602 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6277 2017-03-24 12:46:15.000000 yandextank-1.9.0.post1/yandextank/plugins/JMeter/reader.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/JsonReport/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:32:37.000000 yandextank-1.9.0.post1/yandextank/plugins/JsonReport/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/JsonReport/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      111 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/JsonReport/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2152 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/JsonReport/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Maven/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:31.000000 yandextank-1.9.0.post1/yandextank/plugins/Maven/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1287 2016-12-27 13:12:38.000000 yandextank-1.9.0.post1/yandextank/plugins/Maven/console.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3160 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Maven/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      217 2016-12-30 13:20:21.000000 yandextank-1.9.0.post1/yandextank/plugins/Maven/reader.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:11.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      613 2016-07-18 09:56:43.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/config/pandora_pool_default.json
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      219 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3292 2016-12-30 13:22:25.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/config.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6045 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1668 2017-04-10 14:58:47.000000 yandextank-1.9.0.post1/yandextank/plugins/Pandora/reader.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:32:03.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      959 2016-01-26 11:47:58.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/phantom.conf.tpl
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      777 2015-02-06 14:24:42.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/phantom_benchmark_additional.tpl
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1194 2015-02-06 14:24:42.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/phantom_benchmark_main.tpl
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3943 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/schema.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2790 2017-07-25 12:13:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/schema.pyc
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    10087 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4744 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/reader.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    13664 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/utils.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6111 2016-12-30 13:22:26.000000 yandextank-1.9.0.post1/yandextank/plugins/Phantom/widget.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Platform/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:23:50.000000 yandextank-1.9.0.post1/yandextank/plugins/Platform/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3508 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Platform/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/RCAssert/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/RCAssert/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/RCAssert/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       75 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/RCAssert/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1235 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/RCAssert/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/ResourceCheck/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/ResourceCheck/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/ResourceCheck/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      125 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/ResourceCheck/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2729 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/ResourceCheck/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/ShellExec/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/ShellExec/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/ShellExec/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      229 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/ShellExec/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2290 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/ShellExec/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/SvgReport/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-30 13:20:00.000000 yandextank-1.9.0.post1/yandextank/plugins/SvgReport/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5591 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/SvgReport/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:22:12.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/agent/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       47 2016-12-27 13:12:52.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/agent/__init__.py
--rwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)    15002 2017-03-24 12:46:15.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/agent/agent.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    12859 2016-12-30 13:22:27.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/client.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5922 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/collector.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       55 2016-06-06 13:38:09.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/config/monitoring_default_config.xml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      217 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    14138 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/config.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2675 2017-02-02 07:05:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/decoder.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    16556 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/plugin.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3699 2017-02-02 07:05:53.000000 yandextank-1.9.0.post1/yandextank/plugins/Telegraf/reader.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/__init__.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/config/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       41 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/config/schema.yaml
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3886 2016-04-15 13:01:12.000000 yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/config/tips.txt
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1966 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/plugin.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/stepper/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      144 2016-12-27 13:17:41.000000 yandextank-1.9.0.post1/yandextank/stepper/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5233 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/config.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2090 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/format.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4560 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/info.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     8698 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/instance_plan.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6562 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/load_plan.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    12127 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/stepper/main.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2319 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/mark.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    14131 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/stepper/missile.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      316 2016-12-27 13:12:59.000000 yandextank-1.9.0.post1/yandextank/stepper/module_exceptions.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1634 2016-12-30 13:22:28.000000 yandextank-1.9.0.post1/yandextank/stepper/util.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank/validator/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/validator/__init__.py
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     7334 2017-09-04 11:15:01.000000 yandextank-1.9.0.post1/yandextank/validator/validator.py
-drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        1 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/dependency_links.txt
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      192 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/entry_points.txt
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       30 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/namespace_packages.txt
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      985 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/PKG-INFO
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      162 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/requires.txt
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5520 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/SOURCES.txt
--rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       11 2017-09-05 14:27:53.000000 yandextank-1.9.0.post1/yandextank.egg-info/top_level.txt
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/
+-rw-rw-r--   0 direvius (78873639) LD\Domain Users (593637566)       25 2015-02-09 15:19:04.000000 yandextank-1.9.3/MANIFEST.in
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      979 2017-10-19 13:33:23.000000 yandextank-1.9.3/PKG-INFO
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       63 2017-10-19 13:33:23.000000 yandextank-1.9.3/setup.cfg
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3398 2017-10-13 14:43:52.000000 yandextank-1.9.3/setup.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      200 2016-12-27 13:12:24.000000 yandextank-1.9.3/yandextank/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/api/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       91 2016-12-27 13:43:10.000000 yandextank-1.9.3/yandextank/api/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6566 2016-12-30 13:22:21.000000 yandextank-1.9.3/yandextank/api/apiworker.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/api/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      706 2017-04-14 09:38:31.000000 yandextank-1.9.3/yandextank/api/config/00-base.ini
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      847 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/api/config/00-base.yaml
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/common/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        0 2016-12-27 13:12:24.000000 yandextank-1.9.3/yandextank/common/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      291 2016-12-27 13:12:24.000000 yandextank-1.9.3/yandextank/common/exceptions.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5871 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/common/interfaces.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    12683 2016-12-30 13:22:21.000000 yandextank-1.9.3/yandextank/common/resource.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    19509 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/common/util.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/config_converter/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/config_converter/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    16543 2017-10-13 14:43:15.000000 yandextank-1.9.3/yandextank/config_converter/converter.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/core/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       93 2016-12-27 13:17:07.000000 yandextank-1.9.3/yandextank/core/__init__.py
+-rwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)     2706 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/core/cli.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/core/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      682 2017-04-14 09:38:31.000000 yandextank-1.9.3/yandextank/core/config/00-base.ini
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      956 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/core/config/00-base.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      272 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/core/config/plugins_schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1247 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/core/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    17892 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/core/consoleworker.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2385 2016-12-30 13:22:21.000000 yandextank-1.9.3/yandextank/core/expvar.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    22346 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/core/tankcore.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      200 2016-12-27 13:12:29.000000 yandextank-1.9.3/yandextank/plugins/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:41:47.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5275 2017-04-10 14:58:46.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/aggregator.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1209 2016-12-30 13:22:21.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/chopper.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      474 2016-04-15 13:01:12.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/config/phout.json
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       51 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4287 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Aggregator/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Android/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2017-04-10 14:58:46.000000 yandextank-1.9.3/yandextank/plugins/Android/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Android/binary/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)  1380128 2017-04-10 14:58:46.000000 yandextank-1.9.3/yandextank/plugins/Android/binary/lightning.apk
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Android/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      808 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Android/config/load-sample.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       28 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Android/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2623 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Android/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      221 2017-04-10 14:58:46.000000 yandextank-1.9.3/yandextank/plugins/Android/reader.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Appium/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:33:19.000000 yandextank-1.9.3/yandextank/plugins/Appium/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Appium/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      118 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Appium/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2409 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Appium/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Autostop/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       95 2016-12-27 13:33:12.000000 yandextank-1.9.3/yandextank/plugins/Autostop/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Autostop/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      219 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/plugins/Autostop/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    11106 2016-12-30 13:22:22.000000 yandextank-1.9.3/yandextank/plugins/Autostop/criterions.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    21688 2016-12-30 13:38:15.000000 yandextank-1.9.3/yandextank/plugins/Autostop/cumulative_criterions.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5454 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Autostop/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/BatteryHistorian/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:33:03.000000 yandextank-1.9.3/yandextank/plugins/BatteryHistorian/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/BatteryHistorian/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       58 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/BatteryHistorian/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2938 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/BatteryHistorian/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Bfg/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:58.000000 yandextank-1.9.3/yandextank/plugins/Bfg/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Bfg/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1446 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Bfg/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     9069 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Bfg/guns.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4027 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Bfg/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2535 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Bfg/reader.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1606 2016-12-30 13:22:22.000000 yandextank-1.9.3/yandextank/plugins/Bfg/widgets.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     9138 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Bfg/worker.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Console/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:32:47.000000 yandextank-1.9.3/yandextank/plugins/Console/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Console/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      190 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Console/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5758 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Console/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    22082 2016-12-30 13:22:24.000000 yandextank-1.9.3/yandextank/plugins/Console/screen.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-04-10 14:58:46.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     7880 2017-10-09 11:28:36.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/cli.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    22308 2017-10-09 11:28:36.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/client.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      314 2017-10-09 11:28:36.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/config/postloader_schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1616 2017-10-19 13:33:09.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    32546 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/DataUploader/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Influx/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Influx/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Influx/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      292 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Influx/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3248 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Influx/decoder.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2677 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Influx/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/JMeter/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:42.000000 yandextank-1.9.3/yandextank/plugins/JMeter/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/JMeter/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      317 2015-02-06 14:24:42.000000 yandextank-1.9.3/yandextank/plugins/JMeter/config/jmeter_var_template.xml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1799 2016-09-28 15:42:46.000000 yandextank-1.9.3/yandextank/plugins/JMeter/config/jmeter_writer.xml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3455 2016-09-28 15:42:46.000000 yandextank-1.9.3/yandextank/plugins/JMeter/config/jmeter_writer_ext.xml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      551 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/JMeter/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    10034 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/plugins/JMeter/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6277 2017-03-24 12:46:15.000000 yandextank-1.9.3/yandextank/plugins/JMeter/reader.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/JsonReport/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:32:37.000000 yandextank-1.9.3/yandextank/plugins/JsonReport/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/JsonReport/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      111 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/JsonReport/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2152 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/JsonReport/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Maven/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:31.000000 yandextank-1.9.3/yandextank/plugins/Maven/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1287 2016-12-27 13:12:38.000000 yandextank-1.9.3/yandextank/plugins/Maven/console.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3160 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Maven/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      217 2016-12-30 13:20:21.000000 yandextank-1.9.3/yandextank/plugins/Maven/reader.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Pandora/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:32:11.000000 yandextank-1.9.3/yandextank/plugins/Pandora/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Pandora/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      613 2016-07-18 09:56:43.000000 yandextank-1.9.3/yandextank/plugins/Pandora/config/pandora_pool_default.json
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      219 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Pandora/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3292 2016-12-30 13:22:25.000000 yandextank-1.9.3/yandextank/plugins/Pandora/config.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6519 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Pandora/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1668 2017-04-10 14:58:47.000000 yandextank-1.9.3/yandextank/plugins/Pandora/reader.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Phantom/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:32:03.000000 yandextank-1.9.3/yandextank/plugins/Phantom/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Phantom/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      959 2016-01-26 11:47:58.000000 yandextank-1.9.3/yandextank/plugins/Phantom/config/phantom.conf.tpl
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      777 2015-02-06 14:24:42.000000 yandextank-1.9.3/yandextank/plugins/Phantom/config/phantom_benchmark_additional.tpl
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1194 2015-02-06 14:24:42.000000 yandextank-1.9.3/yandextank/plugins/Phantom/config/phantom_benchmark_main.tpl
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3943 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Phantom/config/schema.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2790 2017-09-20 16:20:13.000000 yandextank-1.9.3/yandextank/plugins/Phantom/config/schema.pyc
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    10087 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Phantom/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4744 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Phantom/reader.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    13664 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Phantom/utils.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6111 2016-12-30 13:22:26.000000 yandextank-1.9.3/yandextank/plugins/Phantom/widget.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Platform/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       39 2016-12-27 13:23:50.000000 yandextank-1.9.3/yandextank/plugins/Platform/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3508 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/Platform/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/RCAssert/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/RCAssert/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/RCAssert/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       75 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/RCAssert/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1235 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/RCAssert/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/ResourceCheck/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/ResourceCheck/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/ResourceCheck/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      125 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/ResourceCheck/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2729 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/ResourceCheck/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/ShellExec/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/ShellExec/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/ShellExec/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      229 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/ShellExec/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2290 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/ShellExec/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/ShootExec/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       41 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/plugins/ShootExec/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/ShootExec/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      123 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/plugins/ShootExec/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     7785 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/plugins/ShootExec/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/SvgReport/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-30 13:20:00.000000 yandextank-1.9.3/yandextank/plugins/SvgReport/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5591 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/SvgReport/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2016-12-27 13:22:12.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/agent/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       47 2016-12-27 13:12:52.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/agent/__init__.py
+-rwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)    15867 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/agent/agent.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    13671 2017-10-13 14:43:52.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/client.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6013 2017-09-18 17:03:37.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/collector.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       55 2016-06-06 13:38:09.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/config/monitoring_default_config.xml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      259 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    14138 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/config.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2675 2017-02-02 07:05:53.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/decoder.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    16702 2017-10-13 14:43:16.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/plugin.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3699 2017-02-02 07:05:53.000000 yandextank-1.9.3/yandextank/plugins/Telegraf/reader.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/TipsAndTricks/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       40 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/plugins/TipsAndTricks/__init__.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/plugins/TipsAndTricks/config/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       41 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/TipsAndTricks/config/schema.yaml
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     3886 2016-04-15 13:01:12.000000 yandextank-1.9.3/yandextank/plugins/TipsAndTricks/config/tips.txt
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1966 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/plugins/TipsAndTricks/plugin.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/stepper/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      144 2016-12-27 13:17:41.000000 yandextank-1.9.3/yandextank/stepper/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5233 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/config.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2090 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/format.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     4560 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/info.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     8698 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/instance_plan.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     6562 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/load_plan.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    12127 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/stepper/main.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     2319 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/mark.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)    14131 2017-09-07 13:47:13.000000 yandextank-1.9.3/yandextank/stepper/missile.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      316 2016-12-27 13:12:59.000000 yandextank-1.9.3/yandextank/stepper/module_exceptions.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     1634 2016-12-30 13:22:28.000000 yandextank-1.9.3/yandextank/stepper/util.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank/validator/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-09-04 11:15:01.000000 yandextank-1.9.3/yandextank/validator/__init__.py
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     7609 2017-10-19 13:33:09.000000 yandextank-1.9.3/yandextank/validator/validator.py
+drwxr-xr-x   0 direvius (78873639) LD\Domain Users (593637566)        0 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)        1 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/dependency_links.txt
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      192 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/entry_points.txt
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       30 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/namespace_packages.txt
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      979 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/PKG-INFO
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)      162 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/requires.txt
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)     5866 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/SOURCES.txt
+-rw-r--r--   0 direvius (78873639) LD\Domain Users (593637566)       11 2017-10-19 13:33:23.000000 yandextank-1.9.3/yandextank.egg-info/top_level.txt
```

### Comparing `yandextank-1.9.0.post1/PKG-INFO` & `yandextank-1.9.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: yandextank
-Version: 1.9.0.post1
+Version: 1.9.3
 Summary: a performance measurement tool
 Home-page: http://yandex.github.io/yandex-tank/
 Author: Alexey Lavrenuke (load testing)
 Author-email: direvius@yandex-team.ru
 License: LGPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `yandextank-1.9.0.post1/setup.py` & `yandextank-1.9.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yandextank',
-    version='1.9.0.post1',
+    version='1.9.3',
     description='a performance measurement tool',
     longer_description='''
 Yandex.Tank is a performance measurement and load testing automatization tool.
 It uses other load generators such as JMeter, ab or phantom inside of it for
 load generation and provides a common configuration system for them and
 analytic tools for the results they produce.
 ''',
@@ -59,19 +59,21 @@
         'yandextank.plugins.Appium': ['config/*'],
         'yandextank.plugins.Autostop': ['config/*'],
         'yandextank.plugins.BatteryHistorian': ['config/*'],
         'yandextank.plugins.Bfg': ['config/*'],
         'yandextank.plugins.Console': ['config/*'],
         'yandextank.plugins.DataUploader': ['config/*'],
         'yandextank.plugins.GraphiteUploader': ['config/*'],
+        'yandextank.plugins.Influx': ['config/*'],
         'yandextank.plugins.JMeter': ['config/*'],
         'yandextank.plugins.JsonReport': ['config/*'],
         'yandextank.plugins.Monitoring': ['config/*'],
         'yandextank.plugins.Pandora': ['config/*'],
         'yandextank.plugins.Phantom': ['config/*'],
         'yandextank.plugins.RCAssert': ['config/*'],
         'yandextank.plugins.ResourceCheck': ['config/*'],
         'yandextank.plugins.ShellExec': ['config/*'],
+        'yandextank.plugins.ShootExec': ['config/*'],
         'yandextank.plugins.Telegraf': ['config/*'],
         'yandextank.plugins.TipsAndTricks': ['config/*'],
     },
     use_2to3=False, )
```

### Comparing `yandextank-1.9.0.post1/yandextank/api/apiworker.py` & `yandextank-1.9.3/yandextank/api/apiworker.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/api/config/00-base.ini` & `yandextank-1.9.3/yandextank/api/config/00-base.ini`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/api/config/00-base.yaml` & `yandextank-1.9.3/yandextank/api/config/00-base.yaml`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/common/interfaces.py` & `yandextank-1.9.3/yandextank/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/common/resource.py` & `yandextank-1.9.3/yandextank/common/resource.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/common/util.py` & `yandextank-1.9.3/yandextank/common/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,7 +604,43 @@
     for k, v in d2.items():
         if isinstance(v, collections.Mapping):
             r = recursive_dict_update(d1.get(k, {}), v)
             d1[k] = r
         else:
             d1[k] = d2[k]
     return d1
+
+
+class FileScanner(object):
+    """
+    Basic class for stats reader for continiuos reading file line by line
+
+    Default line separator is a newline symbol. You can specify other separator
+    via constructor argument
+    """
+
+    _BUFSIZE = 4096
+
+    def __init__(self, path, sep="\n"):
+        self.__path = path
+        self.__sep = sep
+        self.__closed = False
+        self.__buffer = ""
+
+    def _read_lines(self, chunk):
+        self.__buffer += chunk
+        portions = self.__buffer.split(self.__sep)
+        for portion in portions[:-1]:
+            yield portion
+        self.__buffer = portions[-1]
+
+    def _read_data(self, lines):
+        raise NotImplementedError()
+
+    def __iter__(self):
+        with open(self.__path) as stats_file:
+            while not self.__closed:
+                chunk = stats_file.read(self._BUFSIZE)
+                yield self._read_data(self._read_lines(chunk))
+
+    def close(self):
+        self.__closed = True
```

### Comparing `yandextank-1.9.0.post1/yandextank/config_converter/converter.py` & `yandextank-1.9.3/yandextank/config_converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,22 @@
     'Bfg': 'bfg|ultimate_gun|http_gun|custom_gun|scenario_gun',
     'Phantom': 'phantom(-.*)?',
     'DataUploader': 'meta|overload',
     'Telegraf': 'telegraf|monitoring',
     'JMeter': 'jmeter',
     'ResourceCheck': 'rcheck',
     'ShellExec': 'shell_?exec',
+    'ShootExec': 'shoot_?exec',
     'Console': 'console',
     'TipsAndTricks': 'tips',
     'RCAssert': 'rcassert',
     'JsonReport': 'json_report|jsonreport',
     'Pandora': 'pandora',
+    'Influx': 'influx',
+
 }
 
 
 class ConversionError(Exception):
     pass
 
 
@@ -175,14 +178,17 @@
         },
         'Pandora': {
             'expvar': lambda key, value: {key: value == '1'},
             'config_content': lambda key, value: {key: yaml.load(value)}  # works for json as well
         },
         'Autostop': {
             'autostop': lambda k, v: {k: re.findall('\w+\(.+?\)', v)}
+        },
+        'DataUploader': {
+            'lock_targets': lambda k, v: {k: v.strip().split() if v != 'auto' else v}
         }
     }
     CONVERTERS_FOR_UNKNOWN = {
         'DataUploader': lambda k, v: {'meta': {k: v}},
         'JMeter': lambda k, v: {'variables': {k: v}}
     }
 
@@ -389,14 +395,15 @@
             'Maven': 'maven',
             'Monitoring': 'monitoring',
             'Pandora': 'pandora',
             'Phantom': 'phantom',
             'RCAssert': 'rcassert',
             'ResourceCheck': 'rcheck',
             'ShellExec': 'shellexec',
+            'ShootExec': 'shootexec',
             'SvgReport': 'svgreport',
             'Telegraf': 'telegraf',
             'TipsAndTricks': 'tips'
         }
         name_map = {
             'aggregate': 'aggregator',
             'overload': 'overload',
```

### Comparing `yandextank-1.9.0.post1/yandextank/core/cli.py` & `yandextank-1.9.3/yandextank/core/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 import traceback
 from optparse import OptionParser
 
-from .consoleworker import ConsoleTank, CompletionHelperOptionParser
+from yandextank.core.consoleworker import ConsoleTank, CompletionHelperOptionParser
 
 
 def main():
     parser = OptionParser()
     parser.add_option(
         '-c',
         '--config',
```

### Comparing `yandextank-1.9.0.post1/yandextank/core/config/00-base.ini` & `yandextank-1.9.3/yandextank/core/config/00-base.ini`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/core/config/00-base.yaml` & `yandextank-1.9.3/yandextank/core/config/00-base.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -35,8 +35,11 @@
   enabled: true
   package: yandextank.plugins.TipsAndTricks
 rcassert:
   enabled: true
   package: yandextank.plugins.RCAssert
 overload:
   enabled: false
-  package: yandextank.plugins.DataUploader
+  package: yandextank.plugins.DataUploader
+influx:
+  enabled: false
+  package: yandextank.plugins.Influx
```

### Comparing `yandextank-1.9.0.post1/yandextank/core/config/schema.yaml` & `yandextank-1.9.3/yandextank/core/config/schema.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,78 @@
 00000000: 636f 7265 3a0a 2020 7479 7065 3a20 6469  core:.  type: di
 00000010: 6374 0a20 2061 6c6c 6f77 5f75 6e6b 6e6f  ct.  allow_unkno
 00000020: 776e 3a20 6661 6c73 650a 2020 7363 6865  wn: false.  sche
 00000030: 6d61 3a0a 2020 2020 6166 6669 6e69 7479  ma:.    affinity
 00000040: 3a0a 2020 2020 2020 6465 7363 7269 7074  :.      descript
-00000050: 696f 6e3a 2062 696e 6420 7461 6e6b 2070  ion: bind tank p
-00000060: 726f 6365 7373 2074 6f20 6120 7370 6563  rocess to a spec
-00000070: 6966 6963 2063 7075 2063 6f72 6528 7329  ific cpu core(s)
+00000050: 696f 6e3a 2073 7065 6369 6679 2063 7075  ion: specify cpu
+00000060: 2063 6f72 6528 7329 2074 6f20 6269 6e64   core(s) to bind
+00000070: 2074 616e 6b20 7072 6f63 6573 7320 746f   tank process to
 00000080: 0a20 2020 2020 2074 7970 653a 2073 7472  .      type: str
 00000090: 696e 670a 2020 2020 2020 6465 6661 756c  ing.      defaul
 000000a0: 743a 2027 270a 2020 2020 6170 695f 6a6f  t: ''.    api_jo
 000000b0: 626e 6f3a 0a20 2020 2020 2064 6573 6372  bno:.      descr
 000000c0: 6970 7469 6f6e 3a20 7461 6e6b 6170 6920  iption: tankapi 
 000000d0: 6a6f 6220 6964 2c20 616c 736f 2075 7365  job id, also use
 000000e0: 6420 6173 2074 6573 745c 2773 2064 6972  d as test\'s dir
-000000f0: 6563 746f 7279 206e 616d 650a 2020 2020  ectory name.    
-00000100: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00000110: 2020 2061 7274 6966 6163 7473 5f62 6173     artifacts_bas
-00000120: 655f 6469 723a 0a23 2020 2020 2020 6465  e_dir:.#      de
-00000130: 7363 7269 7074 696f 6e3a 2062 6173 6520  scription: base 
-00000140: 6469 7265 6374 6f72 7920 746f 2073 746f  directory to sto
-00000150: 7265 2074 6573 7473 5c27 2061 7274 6966  re tests\' artif
-00000160: 6163 7473 2064 6972 6563 746f 7269 6573  acts directories
-00000170: 0a20 2020 2020 2074 7970 653a 2073 7472  .      type: str
-00000180: 696e 670a 2020 2020 2020 6465 6661 756c  ing.      defaul
-00000190: 743a 202e 2f6c 6f67 730a 2020 2020 6172  t: ./logs.    ar
-000001a0: 7469 6661 6374 735f 6469 723a 0a23 2020  tifacts_dir:.#  
-000001b0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-000001c0: 2064 6972 6563 746f 7279 2069 6e73 6964   directory insid
-000001d0: 6520 6261 7365 2064 6972 6563 746f 7279  e base directory
-000001e0: 2074 6f20 7374 6f72 6520 7465 7374 5c27   to store test\'
-000001f0: 7320 6172 7469 6661 6374 730a 2020 2020  s artifacts.    
-00000200: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00000210: 2020 2020 206e 756c 6c61 626c 653a 2074       nullable: t
-00000220: 7275 650a 2020 2020 2020 6465 6661 756c  rue.      defaul
-00000230: 743a 206e 756c 6c0a 2020 2020 636d 646c  t: null.    cmdl
-00000240: 696e 653a 0a20 2020 2020 2074 7970 653a  ine:.      type:
-00000250: 2073 7472 696e 670a 2020 2020 6578 6974   string.    exit
-00000260: 636f 6465 3a0a 2020 2020 2020 7479 7065  code:.      type
-00000270: 3a20 696e 7465 6765 720a 2020 2020 666c  : integer.    fl
-00000280: 7573 685f 636f 6e66 6967 5f74 6f3a 0a20  ush_config_to:. 
-00000290: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-000002a0: 670a 2020 2020 6967 6e6f 7265 5f6c 6f63  g.    ignore_loc
-000002b0: 6b73 3a0a 2020 2020 2020 7479 7065 3a20  ks:.      type: 
-000002c0: 626f 6f6c 6561 6e0a 2020 2020 7575 6964  boolean.    uuid
-000002d0: 3a0a 2020 2020 2020 7479 7065 3a20 7374  :.      type: st
-000002e0: 7269 6e67 0a20 2020 2070 6964 3a0a 2020  ring.    pid:.  
-000002f0: 2020 2020 7479 7065 3a20 696e 7465 6765      type: intege
-00000300: 720a 2020 2020 6d65 7373 6167 653a 0a20  r.    message:. 
-00000310: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00000320: 670a 2020 2020 6c6f 636b 5f64 6972 3a0a  g.    lock_dir:.
-00000330: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-00000340: 6e67 0a20 2020 2020 2064 6566 6175 6c74  ng.      default
-00000350: 3a20 2f76 6172 2f6c 6f63 6b2f 0a20 2020  : /var/lock/.   
-00000360: 206f 7065 7261 746f 723a 0a20 2020 2020   operator:.     
-00000370: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
-00000380: 2020 7461 736b 7365 745f 7061 7468 3a0a    taskset_path:.
-00000390: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-000003a0: 6e67 0a20 2020 2020 2064 6566 6175 6c74  ng.      default
-000003b0: 3a20 7461 736b 7365 740a 7665 7273 696f  : taskset.versio
-000003c0: 6e3a 0a20 2074 7970 653a 2073 7472 696e  n:.  type: strin
-000003d0: 67                                       g
+000000f0: 6563 746f 7279 206e 616d 6520 2d20 6465  ectory name - de
+00000100: 7465 726d 696e 6564 2062 7920 7461 6e6b  termined by tank
+00000110: 0a20 2020 2020 2074 7970 653a 2073 7472  .      type: str
+00000120: 696e 670a 2020 2020 6172 7469 6661 6374  ing.    artifact
+00000130: 735f 6261 7365 5f64 6972 3a0a 2020 2020  s_base_dir:.    
+00000140: 2020 6465 7363 7269 7074 696f 6e3a 2062    description: b
+00000150: 6173 6520 6469 7265 6374 6f72 7920 746f  ase directory to
+00000160: 2073 746f 7265 2074 6573 7473 5c27 2061   store tests\' a
+00000170: 7274 6966 6163 7473 2064 6972 6563 746f  rtifacts directo
+00000180: 7269 6573 0a20 2020 2020 2074 7970 653a  ries.      type:
+00000190: 2073 7472 696e 670a 2020 2020 2020 6465   string.      de
+000001a0: 6661 756c 743a 202e 2f6c 6f67 730a 2020  fault: ./logs.  
+000001b0: 2020 6172 7469 6661 6374 735f 6469 723a    artifacts_dir:
+000001c0: 0a20 2020 2020 2064 6573 6372 6970 7469  .      descripti
+000001d0: 6f6e 3a20 6469 7265 6374 6f72 7920 696e  on: directory in
+000001e0: 7369 6465 2062 6173 6520 6469 7265 6374  side base direct
+000001f0: 6f72 7920 746f 2073 746f 7265 2074 6573  ory to store tes
+00000200: 745c 2773 2061 7274 6966 6163 7473 2c20  t\'s artifacts, 
+00000210: 6465 6661 756c 7473 2074 6f20 6170 695f  defaults to api_
+00000220: 6a6f 626e 6f20 6966 206e 756c 6c0a 2020  jobno if null.  
+00000230: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00000240: 0a20 2020 2020 206e 756c 6c61 626c 653a  .      nullable:
+00000250: 2074 7275 650a 2020 2020 2020 6465 6661   true.      defa
+00000260: 756c 743a 206e 756c 6c0a 2020 2020 636d  ult: null.    cm
+00000270: 646c 696e 653a 0a20 2020 2020 2074 7970  dline:.      typ
+00000280: 653a 2073 7472 696e 670a 2020 2020 6578  e: string.    ex
+00000290: 6974 636f 6465 3a0a 2020 2020 2020 7479  itcode:.      ty
+000002a0: 7065 3a20 696e 7465 6765 720a 2020 2020  pe: integer.    
+000002b0: 666c 7573 685f 636f 6e66 6967 5f74 6f3a  flush_config_to:
+000002c0: 0a20 2020 2020 2064 6573 6372 6970 7469  .      descripti
+000002d0: 6f6e 3a20 7061 7468 2074 6f20 7374 6f72  on: path to stor
+000002e0: 6520 636f 6e66 6967 0a20 2020 2020 2074  e config.      t
+000002f0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00000300: 6967 6e6f 7265 5f6c 6f63 6b73 3a0a 2020  ignore_locks:.  
+00000310: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00000320: 2069 6620 7461 6e6b 2069 7320 6c6f 636b   if tank is lock
+00000330: 6564 2028 2a2e 6c6f 636b 2066 696c 6528  ed (*.lock file(
+00000340: 7329 2070 7265 7365 6e74 6564 2069 6e20  s) presented in 
+00000350: 6c6f 636b 5f64 6972 292c 2073 686f 6f74  lock_dir), shoot
+00000360: 206e 6576 6572 7468 656c 6573 730a 2020   nevertheless.  
+00000370: 2020 2020 7479 7065 3a20 626f 6f6c 6561      type: boolea
+00000380: 6e0a 2020 2020 7575 6964 3a0a 2020 2020  n.    uuid:.    
+00000390: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+000003a0: 2020 2070 6964 3a0a 2020 2020 2020 7479     pid:.      ty
+000003b0: 7065 3a20 696e 7465 6765 720a 2020 2020  pe: integer.    
+000003c0: 6d65 7373 6167 653a 0a20 2020 2020 2074  message:.      t
+000003d0: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+000003e0: 6c6f 636b 5f64 6972 3a0a 2020 2020 2020  lock_dir:.      
+000003f0: 6465 7363 7269 7074 696f 6e3a 2064 6972  description: dir
+00000400: 6563 746f 7279 2074 6f20 7374 6f72 6520  ectory to store 
+00000410: 2a2e 6c6f 636b 2066 696c 6573 0a20 2020  *.lock files.   
+00000420: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00000430: 2020 2020 2020 6465 6661 756c 743a 202f        default: /
+00000440: 7661 722f 6c6f 636b 2f0a 2020 2020 6f70  var/lock/.    op
+00000450: 6572 6174 6f72 3a0a 2020 2020 2020 6465  erator:.      de
+00000460: 7363 7269 7074 696f 6e3a 2079 6f75 7220  scription: your 
+00000470: 7573 6572 6e61 6d65 0a20 2020 2020 2074  username.      t
+00000480: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00000490: 7461 736b 7365 745f 7061 7468 3a0a 2020  taskset_path:.  
+000004a0: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+000004b0: 0a20 2020 2020 2064 6566 6175 6c74 3a20  .      default: 
+000004c0: 7461 736b 7365 740a 7665 7273 696f 6e3a  taskset.version:
+000004d0: 0a20 2074 7970 653a 2073 7472 696e 67    .  type: string
```

### Comparing `yandextank-1.9.0.post1/yandextank/core/consoleworker.py` & `yandextank-1.9.3/yandextank/core/consoleworker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Provides classes to run TankCore from console environment """
-from ConfigParser import ConfigParser, MissingSectionHeaderError, NoOptionError
+from ConfigParser import ConfigParser, MissingSectionHeaderError, NoOptionError, NoSectionError
 import datetime
 import fnmatch
 import glob
 import logging
 import os
 import sys
 import tempfile
@@ -80,20 +80,19 @@
 
 
 def load_cfg(cfg_filename):
     """
 
     :type cfg_filename: str
     """
-    if cfg_filename.endswith('.yaml'):
-        with open(cfg_filename) as f:
-            cfg = yaml.load(f)
+    if is_ini(cfg_filename):
+        return convert_ini(cfg_filename)
     else:
-        cfg = convert_ini(cfg_filename)
-    return cfg
+        with open(cfg_filename) as f:
+            return yaml.load(f)
 
 
 def cfg_folder_loader(path):
     """
     :type path: str
     """
     CFG_WILDCARD = '*.yaml'
@@ -179,14 +178,16 @@
             ' is not accessible to get configs list')
 
     configs += [os.path.expanduser('~/.yandex-tank')]
     return configs
 
 
 def is_ini(cfg_file):
+    if cfg_file.endswith('.yaml') or cfg_file.endswith('.json'):
+        return False
     try:
         ConfigParser().read(cfg_file)
         return True
     except MissingSectionHeaderError:
         return False
 
 
@@ -212,29 +213,27 @@
 
         # substitute telegraf config
         def patch_ini_config_with_monitoring(ini_config, mon_section_name):
             """
             :type ini_config: ConfigParser
             """
             CONFIG = 'config'
-            if not ini_config.has_section(mon_section_name):
-                raise NoOptionError
             telegraf_cfg = ini_config.get(mon_section_name, CONFIG)
             if not telegraf_cfg.startswith('<') and not telegraf_cfg.lower() == 'auto':
                 with open(resource_manager.resource_filename(telegraf_cfg), 'rb') as telegraf_cfg_file:
                     config_contents = telegraf_cfg_file.read()
                 ini_config.set(mon_section_name, CONFIG, config_contents)
             return ini_config
 
         try:
             cfg_ini = patch_ini_config_with_monitoring(cfg_ini, 'monitoring')
-        except NoOptionError:
+        except (NoSectionError, NoOptionError):
             try:
                 patch_ini_config_with_monitoring(cfg_ini, 'telegraf')
-            except NoOptionError:
+            except (NoOptionError, NoSectionError):
                 pass
 
         for section, key, value in depr_options:
             if not cfg_ini.has_section(section):
                 cfg_ini.add_section(section)
             cfg_ini.set(section, key, value)
         return apply_shorthand_options(cfg_ini, cmd_options)
@@ -262,27 +261,31 @@
     """    Worker class that runs tank core accepting cmdline params    """
 
     IGNORE_LOCKS = "ignore_locks"
 
     def __init__(self, options, ammofile):
         overwrite_options = {'core': {'lock_dir': options.lock_dir}} if options.lock_dir else {}
         self.options = options
-        self.lock_dir = options.lock_dir if options.lock_dir else '/var/lock'
+        # self.lock_dir = options.lock_dir if options.lock_dir else '/var/lock'
         self.baseconfigs_location = '/etc/yandex-tank'
         self.init_logging()
         self.log = logging.getLogger(__name__)
 
         if ammofile:
             self.log.debug("Ammofile: %s", ammofile)
             overwrite_options['phantom'] = {
                 'use_caching': False,
                 'ammofile': ammofile
             }
 
-        self.core = load_tank_core(options.config, options.option, options.no_rc, [], overwrite_options)
+        self.core = load_tank_core([resource_manager.resource_filename(cfg) for cfg in options.config],
+                                   options.option,
+                                   options.no_rc,
+                                   [],
+                                   overwrite_options)
 
         raw_cfg_file, raw_cfg_path = tempfile.mkstemp(suffix='_pre-validation-config.yaml')
         os.close(raw_cfg_file)
         self.core.config.save_raw(raw_cfg_path)
         self.core.add_artifact_file(raw_cfg_path)
 
         self.core.add_artifact_file(options.log)
@@ -345,15 +348,15 @@
         stderr_hdl.addFilter(f_info)
         stderr_hdl.addFilter(f_debug)
         logger.addHandler(stderr_hdl)
 
     def configure(self):
         while True:
             try:
-                self.core.get_lock(self.options.ignore_lock, self.lock_dir)
+                self.core.get_lock(self.options.ignore_lock)
                 break
             except LockError:
                 if self.options.lock_fail:
                     raise RuntimeError("Lock file present, cannot continue")
                 self.log.exception(
                     "Couldn't get lock. Will retry in 5 seconds...")
                 time.sleep(5)
```

### Comparing `yandextank-1.9.0.post1/yandextank/core/expvar.py` & `yandextank-1.9.3/yandextank/core/expvar.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/core/tankcore.py` & `yandextank-1.9.3/yandextank/core/tankcore.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Aggregator/aggregator.py` & `yandextank-1.9.3/yandextank/plugins/Aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Aggregator/chopper.py` & `yandextank-1.9.3/yandextank/plugins/Aggregator/chopper.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Aggregator/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Aggregator/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Android/binary/lightning.apk` & `yandextank-1.9.3/yandextank/plugins/Android/binary/lightning.apk`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Android/config/load-sample.yaml` & `yandextank-1.9.3/yandextank/plugins/Android/config/load-sample.yaml`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Android/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Android/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Appium/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Appium/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Autostop/criterions.py` & `yandextank-1.9.3/yandextank/plugins/Autostop/criterions.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Autostop/cumulative_criterions.py` & `yandextank-1.9.3/yandextank/plugins/Autostop/cumulative_criterions.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Autostop/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Autostop/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/BatteryHistorian/plugin.py` & `yandextank-1.9.3/yandextank/plugins/BatteryHistorian/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Bfg/config/schema.yaml` & `yandextank-1.9.3/yandextank/plugins/Bfg/config/schema.yaml`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Bfg/guns.py` & `yandextank-1.9.3/yandextank/plugins/Bfg/guns.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Bfg/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Bfg/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Bfg/reader.py` & `yandextank-1.9.3/yandextank/plugins/Bfg/reader.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Bfg/widgets.py` & `yandextank-1.9.3/yandextank/plugins/Bfg/widgets.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Bfg/worker.py` & `yandextank-1.9.3/yandextank/plugins/Bfg/worker.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Console/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Console/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Console/screen.py` & `yandextank-1.9.3/yandextank/plugins/Console/screen.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/DataUploader/client.py` & `yandextank-1.9.3/yandextank/plugins/DataUploader/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 import json
 import time
 import traceback
 import urllib
+import uuid
+
 from future.moves.urllib.parse import urljoin
 from builtins import range
 
 import requests
 import logging
 
 from requests.exceptions import ConnectionError, Timeout
 
 requests.packages.urllib3.disable_warnings()
 logger = logging.getLogger(__name__)  # pylint: disable=C0103
 
 
+def id_gen(base, start=0):
+    i = start
+    while True:
+        yield '%s-%d' % (base, i)
+        i += 1
+
+
 class APIClient(object):
+    REQUEST_ID_HEADER = 'X-Request-ID'
 
     def __init__(
             self,
             base_url=None,
             writer_url=None,
             network_attempts=10,
             api_attempts=10,
@@ -35,14 +45,20 @@
         self.writer_url = writer_url
 
         self.retry_timeout = 10
         self.session = requests.Session()
         self.session.verify = False
         self.session.headers.update({"User-Agent": "tank"})
 
+        if "https" in requests.utils.getproxies():
+            logger.info("Connecting via proxy %s" % requests.utils.getproxies()['https'])
+            self.session.proxies = requests.utils.getproxies()
+        else:
+            logger.info("Proxy not set")
+
         self.network_attempts = network_attempts
         self.network_timeout = network_timeout
         self.api_attempts = api_attempts
         self.api_timeout = api_timeout
         self.maintenance_attempts = maintenance_attempts
         self.maintenance_timeout = maintenance_timeout
         self.params = {'api_token': api_token} if api_token else {}
@@ -99,71 +115,82 @@
                   'X-Content-Type-Options', 'X-Download-Options',
                   'Surrogate-Control']
         for h in boring:
             if h in headers:
                 del (headers[h])
         return headers
 
-    def __send_single_request(self, req, trace=False):
-        p = self.session.prepare_request(req)
+    def __send_single_request(self, request, request_id, trace=False):
+        request.headers[self.REQUEST_ID_HEADER] = request_id
+        p = self.session.prepare_request(request)
         if trace:
-            logger.debug("Making request: %s %s Headers: %s Body: %s",
-                         p.method, p.url, p.headers, p.body)
+            logger.debug(self.format_request_info(p, request_id))
         resp = self.session.send(p, timeout=self.connection_timeout)
         if trace:
-            logger.debug("Got response in %ss: %s %s Headers: %s Body: %s",
-                         resp.elapsed.total_seconds(), resp.reason,
-                         resp.status_code, self.filter_headers(resp.headers),
-                         resp.content)
+            logger.debug(self.format_response_info(resp, request_id))
         if resp.status_code in [500, 502, 503, 504]:
             raise self.NotAvailable(
-                request="request: %s %s\n\tHeaders: %s\n\tBody: %s" %
-                (p.method,
-                 p.url,
-                 p.headers,
-                 p.body),
-                response="Got response in %ss: %s %s\n\tHeaders: %s\n\tBody: %s" %
-                (resp.elapsed.total_seconds(),
-                 resp.reason,
-                 resp.status_code,
-                 self.filter_headers(
-                    resp.headers),
-                    resp.content))
+                request=self.format_request_info(p, request_id),
+                response=self.format_response_info(resp, request_id))
         elif resp.status_code == 410:
             raise self.StoppedFromOnline
         elif resp.status_code == 423:
             raise self.UnderMaintenance
         else:
             resp.raise_for_status()
             return resp
 
+    def format_request_info(self, request, request_id):
+        request_info = {
+            'id': request_id,
+            'method': request.method,
+            'url': request.url,
+            'headers': str(self.filter_headers(request.headers)),
+            'body': request.body.replace('\n', '\\n') if isinstance(request.body, str) else request.body
+        }
+        return """
+        Request: {}""".format(json.dumps(request_info))
+
+    def format_response_info(self, resp, request_id):
+        response_info = {
+            'id': request_id,
+            'elapsed_time': resp.elapsed.total_seconds(),
+            'reason': resp.reason,
+            'status code': resp.status_code,
+            'headers': str(self.filter_headers(resp.headers)),
+            'content': resp.content.replace('\n', '\\n') if isinstance(resp.content, str) else resp.content
+        }
+        return """
+        Response: {}""".format(json.dumps(response_info))
+
     def __make_api_request(
             self,
             http_method,
             path,
             data=None,
             response_callback=lambda x: x,
             writer=False,
             trace=False,
             json=None,
             maintenance_timeouts=None,
             maintenance_msg=None):
         url = urljoin(self.base_url, path)
+        ids = id_gen(str(uuid.uuid4()))
         if json:
             request = requests.Request(
                 http_method, url, json=json, headers={'User-Agent': self.user_agent}, params=self.params)
         else:
             request = requests.Request(
                 http_method, url, data=data, headers={'User-Agent': self.user_agent}, params=self.params)
         network_timeouts = self.network_timeouts()
         maintenance_timeouts = maintenance_timeouts or self.maintenance_timeouts()
         maintenance_msg = maintenance_msg or "%s is under maintenance" % (self._base_url)
         while True:
             try:
-                response = self.__send_single_request(request, trace=trace)
+                response = self.__send_single_request(request, ids.next(), trace=trace)
                 return response_callback(response)
             except (Timeout, ConnectionError):
                 logger.warn(traceback.format_exc())
                 try:
                     timeout = next(network_timeouts)
                     logger.warn(
                         "Network error, will retry in %ss..." %
@@ -194,19 +221,20 @@
         request = requests.Request(
             http_method,
             self.writer_url,
             params=params,
             json=json,
             headers={
                 'User-Agent': self.user_agent})
+        ids = id_gen(str(uuid.uuid4()))
         network_timeouts = self.network_timeouts()
         maintenance_timeouts = self.maintenance_timeouts()
         while True:
             try:
-                response = self.__send_single_request(request, trace=trace)
+                response = self.__send_single_request(request, ids.next(), trace=trace)
                 return response
             except (Timeout, ConnectionError):
                 logger.warn(traceback.format_exc())
                 try:
                     timeout = next(network_timeouts)
                     logger.warn(
                         "Network error, will retry in %ss..." %
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/DataUploader/config/schema.yaml` & `yandextank-1.9.3/yandextank/plugins/DataUploader/config/schema.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
   type: string
   dependencies: upload_token
 jobno_file:
   type: string
   default: jobno_file.txt
 lock_targets:
   default: auto
-  type: string
+  anyof:
+    - type: list
+    - type: string
+      allowed: [auto]
 log_data_requests:
   default: false
   type: boolean
 log_monitoring_requests:
   default: false
   type: boolean
 log_other_requests:
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/DataUploader/plugin.py` & `yandextank-1.9.3/yandextank/plugins/DataUploader/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,34 +272,36 @@
         self.publish("web_link", web_link)
 
         jobno_file = self.get_option("jobno_file", '')
         if jobno_file:
             logger.debug("Saving jobno to: %s", jobno_file)
             with open(jobno_file, 'w') as fdes:
                 fdes.write(str(self.lp_job.number))
+            self.core.add_artifact_file(jobno_file)
         self.__save_conf()
 
     def is_test_finished(self):
         return self.retcode
 
     def end_test(self, retcode):
         self.on_air = False
-        self.monitoring_queue.put(None)
-        self.data_queue.put(None)
         self.__save_conf()
-        self._join_threads(timeout=int(self.get_option('threads_timeout')))
         self.unlock_targets(self.locked_targets)
         return retcode
 
     def post_process(self, rc):
+        self.monitoring_queue.put(None)
+        self.data_queue.put(None)
+        logger.info("Waiting for sender threads to join.")
+        self.monitoring.join()
+        self.upload.join()
         try:
             self.lp_job.close(rc)
         except Exception:  # pylint: disable=W0703
             logger.warning("Failed to close job", exc_info=True)
-
         logger.info(
             "Web link: %s%s",
             self.lp_job.api_client.base_url,
             self.lp_job.number)
 
         autostop = None
         try:
@@ -397,15 +399,14 @@
             except APIClient.StoppedFromOnline:
                 logger.info("Test stopped from Lunapark")
                 lp_job.is_alive = False
                 self.retcode = 8
                 break
             except Exception as e:
                 logger.info("Mysterious exception: %s", e)
-                self.retcode = 8
                 break
         logger.info("Closing Data uploader thread")
 
     def __monitoring_uploader(self):
         logger.info('Monitoring uploader thread started')
         lp_job = self.lp_job
         queue = self.monitoring_queue
@@ -424,41 +425,44 @@
                 logger.warn(e.message)
                 break
             except APIClient.StoppedFromOnline:
                 logger.info("Test stopped from Lunapark")
                 lp_job.is_alive = False
                 self.retcode = 8
                 break
+            except Exception as e:
+                logger.info("Mysterious exception: %s", e)
+                break
         logger.info('Closing Monitoring uploader thread')
 
     # TODO: why we do it here? should be in core
     def __save_conf(self):
         # config = copy.deepcopy(self.core.config)
         try:
             config_filename = self.core.job.monitoring_plugin.config
             if config_filename and config_filename not in ['none', 'auto']:
                 with open(config_filename) as config_file:
                     self.core.job.monitoring_plugin.set_option("config_contents",
                                                                config_file.read())
         except AttributeError:  # pylint: disable=W0703
-            logger.warning("Can't get monitoring config", exc_info=True)
+            logger.warning("Can't get monitoring config")
 
         self.lp_job.send_config_snapshot(self.core.cfg_snapshot)
         self.core.config.save(os.path.join(self.core.artifacts_dir, 'saved_conf.yaml'))
 
     def parse_lock_targets(self):
         # prepare target lock list
-        locks_list_cfg = self.get_option('lock_targets', 'auto').strip()
+        locks_list_cfg = self.get_option('lock_targets', 'auto')
 
         def no_target():
             logging.warn("Target lock set to 'auto', but no target info available")
-            return ''
+            return {}
 
-        locks_list = (self.target or no_target() if locks_list_cfg.lower() == 'auto' else locks_list_cfg).split('\n')
-        targets_to_lock = [host for host in locks_list if host]
+        locks_set = {self.target} or no_target() if locks_list_cfg == 'auto' else set(locks_list_cfg)
+        targets_to_lock = [host for host in locks_set if host]
         return targets_to_lock
 
     def lock_targets(self, targets_to_lock, ignore, strict):
         locked_targets = [target for target in targets_to_lock
                           if self.lp_job.lock_target(target, self.lock_duration, ignore, strict)]
         return locked_targets
 
@@ -622,30 +626,14 @@
     @property
     def target(self):
         if self._target is None:
             self._target = self.generator_info.address
             logger.info("Detected target: %s", self.target)
         return self._target
 
-    def _join_threads(self, timeout):
-        logger.info(
-            'Waiting for sender threads to join for {} seconds ("meta.threads_timeout" config option)'.format(timeout))
-        try:
-            self.monitoring.join(timeout=timeout)
-            if self.monitoring.isAlive():
-                logger.error('Monitoring thread joining timed out. Terminating.')
-        except RuntimeError:
-            pass
-        try:
-            self.upload.join(timeout=timeout)
-            if self.upload.isAlive():
-                logger.error('Upload thread joining timed out. Terminating.')
-        except RuntimeError:
-            pass
-
 
 class JobInfoWidget(AbstractInfoWidget):
     def __init__(self, sender):
         # type: (Plugin) -> object
         AbstractInfoWidget.__init__(self)
         self.owner = sender
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/jmeter_writer.xml` & `yandextank-1.9.3/yandextank/plugins/JMeter/config/jmeter_writer.xml`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/jmeter_writer_ext.xml` & `yandextank-1.9.3/yandextank/plugins/JMeter/config/jmeter_writer_ext.xml`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/JMeter/config/schema.yaml` & `yandextank-1.9.3/yandextank/plugins/JMeter/config/schema.yaml`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/JMeter/plugin.py` & `yandextank-1.9.3/yandextank/plugins/JMeter/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,17 +164,25 @@
     def __add_jmeter_components(self, jmx, jtl, variables):
         """ Genius idea by Alexey Lavrenyuk """
         logger.debug("Original JMX: %s", os.path.realpath(jmx))
         with open(jmx, 'r') as src_jmx:
             source_lines = src_jmx.readlines()
 
         try:
+            # In new Jmeter version (3.2 as example) WorkBench's plugin checkbox enabled by default
+            # It totally crashes Yandex tank injection and raises XML Parse Exception
             closing = source_lines.pop(-1)
-            closing = source_lines.pop(-1) + closing
-            closing = source_lines.pop(-1) + closing
+            if "WorkBenchGui" in source_lines[-5]:
+                logger.info("WorkBench checkbox enabled...bypassing")
+                last_string_count = 6
+            else:
+                last_string_count = 2
+            while last_string_count > 0:
+                closing = source_lines.pop(-1) + closing
+                last_string_count -= 1
             logger.debug("Closing statement: %s", closing)
         except Exception as exc:
             raise RuntimeError("Failed to find the end of JMX XML: %s" % exc)
 
         udv_tpl = resource_string(__name__, 'config/jmeter_var_template.xml')
         udv_set = []
         for var_name, var_value in variables.iteritems():
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/JMeter/reader.py` & `yandextank-1.9.3/yandextank/plugins/JMeter/reader.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/JsonReport/plugin.py` & `yandextank-1.9.3/yandextank/plugins/JsonReport/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Maven/console.py` & `yandextank-1.9.3/yandextank/plugins/Maven/console.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Maven/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Maven/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Pandora/config/pandora_pool_default.json` & `yandextank-1.9.3/yandextank/plugins/Pandora/config/pandora_pool_default.json`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Pandora/config.py` & `yandextank-1.9.3/yandextank/plugins/Pandora/config.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Pandora/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Pandora/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,21 @@
     AbstractInfoWidget, GeneratorPlugin
 
 from .reader import PandoraStatsReader
 from ..Aggregator import Plugin as AggregatorPlugin
 from ..Console import Plugin as ConsolePlugin
 from ..Console import screen as ConsoleScreen
 from ..Phantom import PhantomReader
+from yandextank.common.resource import manager as resource_manager
 
 logger = logging.getLogger(__name__)
 
 
 class Plugin(AbstractPlugin, GeneratorPlugin):
-    '''    Pandora load generator plugin    '''
+    """    Pandora load generator plugin    """
 
     OPTION_CONFIG = "config"
     SECTION = "pandora"
 
     def __init__(self, core, cfg, cfg_updater):
         super(Plugin, self).__init__(core, cfg, cfg_updater)
         self.buffered_seconds = 2
@@ -49,15 +50,15 @@
         self.expvar = self.get_option("expvar")
         self.pandora_cmd = self.get_option("pandora_cmd")
         self.buffered_seconds = self.get_option("buffered_seconds")
         with open(self.sample_log, 'w'):
             pass
         self.core.add_artifact_file(self.sample_log)
 
-        config_content = self.get_option("config_content")
+        config_content = self.patch_config(self.get_option("config_content"))
         if len(config_content) > 0:
             self.pandora_config_file = self.core.mkstemp(
                 ".json", "pandora_config_")
             self.core.add_artifact_file(self.pandora_config_file)
             with open(self.pandora_config_file, 'w') as config_file:
                 json.dump(config_content, config_file)
         else:
@@ -130,14 +131,25 @@
             self.process.terminate()
             if self.process_stderr:
                 self.process_stderr.close()
         else:
             logger.debug("Seems subprocess finished OK")
         return retcode
 
+    @staticmethod
+    def patch_config(config):
+        """
+        download remote resources, replace links with local filenames
+        :param dict config: pandora config
+        """
+        for pool in config['pools']:
+            if 'file' in pool.get('ammo', {}):
+                pool['ammo']['file'] = resource_manager.resource_filename(pool['ammo']['file'])
+        return config
+
 
 class PandoraInfoWidget(AbstractInfoWidget):
     ''' Right panel widget '''
 
     def __init__(self, pandora):
         AbstractInfoWidget.__init__(self)
         self.krutilka = ConsoleScreen.krutilka()
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Pandora/reader.py` & `yandextank-1.9.3/yandextank/plugins/Pandora/reader.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/phantom.conf.tpl` & `yandextank-1.9.3/yandextank/plugins/Phantom/config/phantom.conf.tpl`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/phantom_benchmark_additional.tpl` & `yandextank-1.9.3/yandextank/plugins/Phantom/config/phantom_benchmark_additional.tpl`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/phantom_benchmark_main.tpl` & `yandextank-1.9.3/yandextank/plugins/Phantom/config/phantom_benchmark_main.tpl`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/schema.py` & `yandextank-1.9.3/yandextank/plugins/Phantom/config/schema.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/config/schema.pyc` & `yandextank-1.9.3/yandextank/plugins/Phantom/config/schema.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 3ce2 7159 6300 0000 0000 0000  ....<.qYc.......
+00000000: 03f3 0d0a e14d b159 6300 0000 0000 0000  .....M.Yc.......
 00000010: 0006 0000 0040 0000 0073 0404 0000 692a  .....@...s....i*
 00000020: 0069 0200 6400 0064 0100 3664 0200 6403  .i..d..d..6d..d.
 00000030: 0036 6404 0036 6902 0064 0000 6401 0036  .6d..6i..d..d..6
 00000040: 6500 0064 0500 3664 0600 3669 0200 6400  e..d..6d..6i..d.
 00000050: 0064 0100 3664 0700 6403 0036 6408 0036  .d..6d..d..6d..6
 00000060: 6902 0064 0000 6401 0036 6402 0064 0300  i..d..d..6d..d..
 00000070: 3664 0900 3669 0200 640a 0064 0100 3664  6d..6i..d..d..6d
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Phantom/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/reader.py` & `yandextank-1.9.3/yandextank/plugins/Phantom/reader.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/utils.py` & `yandextank-1.9.3/yandextank/plugins/Phantom/utils.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Phantom/widget.py` & `yandextank-1.9.3/yandextank/plugins/Phantom/widget.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Platform/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Platform/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/RCAssert/plugin.py` & `yandextank-1.9.3/yandextank/plugins/RCAssert/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/ResourceCheck/plugin.py` & `yandextank-1.9.3/yandextank/plugins/ResourceCheck/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/ShellExec/plugin.py` & `yandextank-1.9.3/yandextank/plugins/ShellExec/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/SvgReport/plugin.py` & `yandextank-1.9.3/yandextank/plugins/SvgReport/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/agent/agent.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/agent/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import signal
 import ConfigParser
 import json
 import threading
 import time
 
-from optparse import OptionParser
+from argparse import ArgumentParser
 import Queue as q
 
 logger = logging.getLogger("agent")
 collector_logger = logging.getLogger("telegraf")
 
 
 def signal_handler(sig, frame):
@@ -192,21 +192,21 @@
         self.data_reader = None
         self.telegraf_path = telegraf_path
         self.results = q.Queue()
         self.results_stdout = q.Queue()
         self.results_err = q.Queue()
 
     @staticmethod
-    def popen(cmnd):
+    def __popen(cmnd, shell=False):
         return subprocess.Popen(
             cmnd,
             bufsize=0,
             preexec_fn=os.setsid,
             close_fds=True,
-            shell=True,
+            shell=shell,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             stdin=subprocess.PIPE, )
 
     def read_startup_config(self, cfg_file='agent_startup.cfg'):
         try:
             config = ConfigParser.ConfigParser()
@@ -235,22 +235,23 @@
             logger.error(
                 'Error trying to read agent startup config', exc_info=True)
 
     def run(self):
         logger.info("Running startup commands")
         for cmnd in self.startups:
             logger.debug("Run: %s", cmnd)
-            proc = self.popen(cmnd)
+            # fixme: shell=True is insecure, should save startup script and launch directly
+            proc = self.__popen(cmnd, shell=True)
             logger.info('Started with pid %d', proc.pid)
             self.startup_processes.append(proc)
 
         logger.info('Starting metrics collector..')
-        cmnd = "{telegraf} -config {working_dir}/agent.cfg".format(
-            telegraf=self.telegraf_path, working_dir=self.working_dir)
-        self.collector = self.popen(cmnd)
+        # todo: add identificators into {} for python 2.6
+        args = [self.telegraf_path, '-config', '{0}/agent.cfg'.format(self.working_dir)]
+        self.collector = self.__popen(cmnd=args)
         logger.info('Started with pid %d', self.collector.pid)
 
         telegraf_output = self.working_dir + '/monitoring.rawdata'
         sources = [telegraf_output] + self.custom_sources
 
         for _ in range(10):
             self.collector.poll()
@@ -350,38 +351,59 @@
             subprocess.call(cmnd, shell=True)
 
         self.finished = True
         logger.info("Worker thread finished")
         sys.stderr.write('stopped\n')
 
 
+def kill_old_agents(telegraf_path):
+    my_pid = os.getpid()
+    parent = os.getppid()
+    logger.info('My pid: {0} Parent pid: {1}'.format(my_pid, parent))
+    ps_output = subprocess.check_output(['ps', 'aux'])
+    for line in ps_output.splitlines():
+        if telegraf_path in line:
+            pid = int(line.split()[1])
+            logger.info('Found pid: {0}'.format(pid))
+            if pid not in [my_pid, parent]:
+                logger.info('Killing process {0}:\n{1}'.format(pid, line))
+                os.kill(pid, signal.SIGKILL)
+
+
 def main():
     fname = os.path.dirname(__file__) + "/_agent.log"
     logging.basicConfig(
         level=logging.DEBUG,
         filename=fname,
         format='%(asctime)s [%(levelname)s] %(name)s:%(lineno)d %(message)s')
 
-    parser = OptionParser()
-    parser.add_option(
-        "",
+    parser = ArgumentParser()
+    parser.add_argument(
         "--telegraf",
         dest="telegraf_path",
         help="telegraf_path",
         default="/tmp/telegraf")
-    parser.add_option(
-        "",
+    parser.add_argument(
         "--host",
         dest="hostname_path",
         help="telegraf_path",
         default="/usr/bin/telegraf")
-    (options, args) = parser.parse_args()
+    parser.add_argument(
+        "-k", "--kill-old",
+        action="store_true",
+        dest="kill_old"
+    )
+    options = parser.parse_args()
 
     logger.info('Init')
     customs_script = os.path.dirname(__file__) + '/agent_customs.sh'
+    # todo: deprecate
+    if options.kill_old:
+        kill_old_agents(options.telegraf_path)
+
     try:
         logger.info(
             'Trying to make telegraf executable: %s', options.telegraf_path)
         # 0o755 compatible with old python versions. 744 is NOT enough
         os.chmod(options.telegraf_path, 493)
     except OSError:
         logger.warning(
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/client.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,60 +13,62 @@
 from ..Telegraf.config import AgentConfig
 from ..Telegraf.reader import MonitoringReader
 
 logger = logging.getLogger(__name__)
 logging.getLogger("paramiko.transport").setLevel(logging.WARNING)
 
 
-def generate_file_md5(filename, blocksize=2**20):
+def generate_file_md5(filename, blocksize=2 ** 20):
     m = hashlib.md5()
     with open(filename, "rb") as f:
         while True:
             buf = f.read(blocksize)
             if not buf:
                 break
             m.update(buf)
     return m.hexdigest()
 
 
 class LocalhostClient(object):
     """ localhost client setup """
+    AGENT_FILENAME = 'agent.py'
 
-    def __init__(self, config, old_style_configs):
+    def __init__(self, config, old_style_configs, kill_old):
         # config
+        self.kill_old = '--kill-old' if kill_old else ''
         self.python = config['python']
         self.host = "localhost"
         self.telegraf = config['telegraf']
         self.config = AgentConfig(config, old_style_configs)
 
         # connection
         self.incoming_queue = queue.Queue()
         self.buffer = ""
 
         self.workdir = None
         self.reader = MonitoringReader(self.incoming_queue)
 
         self.path = {
-            'AGENT_LOCAL_FOLDER': os.path.dirname(__file__) + '/agent',
+            'AGENT_LOCAL_FOLDER': os.path.join(os.path.dirname(__file__), 'agent'),
             'TELEGRAF_LOCAL_PATH': self.telegraf,
         }
 
     def install(self):
         self.workdir = tempfile.mkdtemp()
         logger.info("Created temp dir %s", self.workdir)
         agent_config = self.config.create_collector_config(self.workdir)
         startup_config = self.config.create_startup_config()
         customs_script = self.config.create_custom_exec_script()
         try:
             copyfile(
-                self.path['AGENT_LOCAL_FOLDER'] + '/agent.py',
-                self.workdir + '/agent.py')
-            copyfile(agent_config, self.workdir + '/agent.cfg')
-            copyfile(startup_config, self.workdir + '/agent_startup.cfg')
-            copyfile(customs_script, self.workdir + '/agent_customs.sh')
+                os.path.join(self.path['AGENT_LOCAL_FOLDER'], self.AGENT_FILENAME),
+                os.path.join(self.workdir, self.AGENT_FILENAME))
+            copyfile(agent_config, os.path.join(self.workdir, 'agent.cfg'))
+            copyfile(startup_config, os.path.join(self.workdir, 'agent_startup.cfg'))
+            copyfile(customs_script, os.path.join(self.workdir, 'agent_customs.sh'))
             if not os.path.isfile(self.path['TELEGRAF_LOCAL_PATH']):
                 logger.error(
                     'Telegraf binary not found at specified path: %s\n'
                     'You can download telegraf binaries here: https://github.com/influxdata/telegraf\n'
                     'or install debian package: `telegraf`',
                     self.path['TELEGRAF_LOCAL_PATH'])
                 return None, None, None
@@ -75,34 +77,34 @@
                 "Failed to copy agent to %s on localhost",
                 self.workdir,
                 exc_info=True)
             return None, None, None
         return agent_config, startup_config, customs_script
 
     @staticmethod
-    def popen(cmnd):
+    def popen(args):
         return subprocess.Popen(
-            cmnd,
+            args,
             bufsize=0,
             preexec_fn=os.setsid,
             close_fds=True,
-            shell=True,
+            shell=False,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             stdin=subprocess.PIPE, )
 
     def start(self):
         """Start local agent"""
         logger.info('Starting agent on localhost')
-        command = "{python} {work_dir}/agent.py --telegraf {telegraf_path} --host {host}".format(
-            python=self.python,
-            work_dir=self.workdir,
-            telegraf_path=self.path['TELEGRAF_LOCAL_PATH'],
-            host=self.host)
-        self.session = self.popen(command)
+        args = self.python.split() + [os.path.join(self.workdir, self.AGENT_FILENAME),
+                                      '--telegraf', self.path['TELEGRAF_LOCAL_PATH'],
+                                      '--host', self.host]
+        if self.kill_old:
+            args.append(self.kill_old)
+        self.session = self.popen(args)
         self.reader_thread = threading.Thread(target=self.read_buffer)
         self.reader_thread.setDaemon(True)
         return self.session
 
     def read_buffer(self):
         while self.session:
             try:
@@ -143,17 +145,19 @@
 
         logger.info("Removing agent from: localhost")
         return log_filename, data_filename
 
 
 class SSHClient(object):
     """remote agent client setup """
+    AGENT_FILENAME = 'agent.py'
 
-    def __init__(self, config, old_style_configs, timeout):
+    def __init__(self, config, old_style_configs, timeout, kill_old):
         # config
+        self.kill_old = '--kill-old' if kill_old else ''
         self.host = config['host']
         self.username = config['username']
         self.python = config['python']
         self.port = config['port']
         self.telegraf = config['telegraf']
         self.config = AgentConfig(config, old_style_configs)
 
@@ -170,14 +174,15 @@
             # Destination path on remote host
             'AGENT_REMOTE_FOLDER': '/tmp/',
             # Source path on tank
             'AGENT_LOCAL_FOLDER': os.path.dirname(__file__) + '/agent',
             'TELEGRAF_REMOTE_PATH': '/tmp/telegraf',
             'TELEGRAF_LOCAL_PATH': self.telegraf,
         }
+        self.agent_remote_folder = None
 
     def install(self):
         """Create folder and copy agent and metrics scripts to remote host"""
         logger.info(
             "Installing monitoring agent at %s@%s...", self.username, self.host)
 
         # create remote temp dir
@@ -200,14 +205,15 @@
                 "Failed to create remote dir via SSH at %s@%s, code %s: %s" %
                 (self.username, self.host, err_code, out.strip()))
             return None, None, None
 
         remote_dir = out.strip()
         if remote_dir:
             self.path['AGENT_REMOTE_FOLDER'] = remote_dir
+            self.agent_remote_folder = remote_dir
         logger.debug(
             "Remote dir at %s:%s", self.host, self.path['AGENT_REMOTE_FOLDER'])
 
         # create collector config
         agent_config = self.config.create_collector_config(
             self.path['AGENT_REMOTE_FOLDER'])
         startup_config = self.config.create_startup_config()
@@ -252,40 +258,41 @@
                         'Telegraf binary not found neither on %s nor on localhost at specified path: %s\n'
                         'You can download telegraf binaries here: https://github.com/influxdata/telegraf\n'
                         'or install debian package: `telegraf`', self.host,
                         self.path['TELEGRAF_LOCAL_PATH'])
                     return None, None, None
 
             self.ssh.send_file(
-                self.path['AGENT_LOCAL_FOLDER'] + '/agent.py',
-                self.path['AGENT_REMOTE_FOLDER'] + '/agent.py')
+                os.path.join(self.path['AGENT_LOCAL_FOLDER'], self.AGENT_FILENAME),
+                os.path.join(self.path['AGENT_REMOTE_FOLDER'], self.AGENT_FILENAME))
             self.ssh.send_file(
-                agent_config, self.path['AGENT_REMOTE_FOLDER'] + '/agent.cfg')
+                agent_config, os.path.join(self.path['AGENT_REMOTE_FOLDER'], 'agent.cfg'))
             self.ssh.send_file(
                 startup_config,
-                self.path['AGENT_REMOTE_FOLDER'] + '/agent_startup.cfg')
+                os.path.join(self.path['AGENT_REMOTE_FOLDER'], 'agent_startup.cfg'))
             self.ssh.send_file(
                 customs_script,
-                self.path['AGENT_REMOTE_FOLDER'] + '/agent_customs.sh')
+                os.path.join(self.path['AGENT_REMOTE_FOLDER'], 'agent_customs.sh'))
 
         except Exception:
             logger.error(
                 "Failed to install agent on %s", self.host, exc_info=True)
             return None, None, None
 
         return agent_config, startup_config, customs_script
 
     def start(self):
         """Start remote agent"""
         logger.info('Starting agent: %s', self.host)
-        command = "{python} {agent_path}/agent.py --telegraf {telegraf_path} --host {host}".format(
+        command = "{python} {agent_path} --telegraf {telegraf_path} --host {host} {kill_old}".format(
             python=self.python,
-            agent_path=self.path['AGENT_REMOTE_FOLDER'],
+            agent_path=os.path.join(self.path['AGENT_REMOTE_FOLDER'], self.AGENT_FILENAME),
             telegraf_path=self.path['TELEGRAF_REMOTE_PATH'],
-            host=self.host)
+            host=self.host,
+            kill_old=self.kill_old)
         logging.debug('Command to start agent: %s', command)
         self.session = self.ssh.async_session(command)
         self.reader_thread = threading.Thread(target=self.read_buffer)
         self.reader_thread.setDaemon(True)
         return self.session
 
     def read_buffer(self):
@@ -316,18 +323,23 @@
                 self.session = None
         except:
             logger.warning(
                 'Unable to correctly stop monitoring agent - session is broken. Pay attention to agent log (%s).',
                 log_filename,
                 exc_info=True)
         try:
-            self.ssh.get_file(
-                self.path['AGENT_REMOTE_FOLDER'] + "/_agent.log", log_filename)
-            self.ssh.get_file(
-                self.path['AGENT_REMOTE_FOLDER'] + "/monitoring.rawdata",
-                data_filename)
+            self.ssh.get_file(os.path.join(self.path['AGENT_REMOTE_FOLDER'], "_agent.log"), log_filename)
+            self.ssh.get_file(os.path.join(self.path['AGENT_REMOTE_FOLDER'], "monitoring.rawdata"), data_filename)
             self.ssh.rm_r(self.path['AGENT_REMOTE_FOLDER'])
         except Exception:
             logger.error("Unable to get agent artefacts", exc_info=True)
 
-        logger.info("Removing agent from: %s@%s...", self.username, self.host)
+        self._kill_agent()
+
         return log_filename, data_filename
+
+    def _kill_agent(self):
+        if self.agent_remote_folder:
+            cmd = 'pgrep -f {} | xargs kill -9'.format(self.agent_remote_folder)
+            out, errors, err_code = self.ssh.execute(cmd)
+            if errors:
+                logging.error("[%s] error while killing agent: '%s'", self.host, errors)
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/collector.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     agent starts startups on target, then starts telegraf
     agent reads output of telegraf, consolidates output, caches 5 seconds and then sends output to collector
     collector polls agents for data, decodes known metrics and counts diffs for diff-like metrics
     collector sends data to listeners
 
     """
 
-    def __init__(self, disguise_hostnames):
+    def __init__(self, disguise_hostnames, kill_old):
+        self.kill_old = kill_old
         self.disguise_hostnames = disguise_hostnames
         self.config = None
         self.default_target = None
         self.agents = []
         self.agent_sessions = []
         self.listeners = []
         self.first_data_received = False
@@ -56,18 +57,18 @@
             agent_configs = self.config_manager.getconfig(
                 self.config, self.default_target)
 
         # Creating agent for hosts
         for config in agent_configs:
             if config['host'] in ['localhost', '127.0.0.1', '::1']:
                 client = self.clients['localhost'](
-                    config, self.old_style_configs)
+                    config, self.old_style_configs, kill_old=self.kill_old)
             else:
                 client = self.clients['ssh'](
-                    config, self.old_style_configs, timeout=5)
+                    config, self.old_style_configs, timeout=5, kill_old=self.kill_old)
             logger.debug('Installing monitoring agent. Host: %s', client.host)
             agent_config, startup_config, customs_script = client.install()
             if agent_config:
                 self.agents.append(client)
                 self.artifact_files.append(agent_config)
             if startup_config:
                 self.artifact_files.append(startup_config)
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/config.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/config.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/decoder.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/decoder.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/plugin.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     def __init__(self, core, cfg, cfg_updater):
         super(Plugin, self).__init__(core, cfg, cfg_updater)
         self.jobno = None
         self.default_target = None
         self.default_config = "{path}/config/monitoring_default_config.xml".format(
             path=os.path.dirname(__file__))
         self.process = None
-        self.monitoring = MonitoringCollector(disguise_hostnames=self.get_option('disguise_hostnames'))
+        self.monitoring = MonitoringCollector(disguise_hostnames=self.get_option('disguise_hostnames'),
+                                              kill_old=self.get_option('kill_old'))
         self.die_on_fail = True
         self.data_file = None
         self.mon_saver = None
         self._config = None
 
     @staticmethod
     def get_key():
@@ -222,14 +223,17 @@
                 self.core.add_artifact_file(log)
 
             self.monitoring.send_rest_data()
         if self.mon_saver:
             self.mon_saver.close()
         return retcode
 
+    def post_process(self, retcode):
+        logger.info('')
+
 
 class SaveMonToFile(MonitoringDataListener):
     """
     Default listener - saves data to file
     """
 
     def __init__(self, out_file):
```

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/Telegraf/reader.py` & `yandextank-1.9.3/yandextank/plugins/Telegraf/reader.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/config/tips.txt` & `yandextank-1.9.3/yandextank/plugins/TipsAndTricks/config/tips.txt`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/plugins/TipsAndTricks/plugin.py` & `yandextank-1.9.3/yandextank/plugins/TipsAndTricks/plugin.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/config.py` & `yandextank-1.9.3/yandextank/stepper/config.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/format.py` & `yandextank-1.9.3/yandextank/stepper/format.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/info.py` & `yandextank-1.9.3/yandextank/stepper/info.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/instance_plan.py` & `yandextank-1.9.3/yandextank/stepper/instance_plan.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/load_plan.py` & `yandextank-1.9.3/yandextank/stepper/load_plan.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/main.py` & `yandextank-1.9.3/yandextank/stepper/main.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/mark.py` & `yandextank-1.9.3/yandextank/stepper/mark.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/missile.py` & `yandextank-1.9.3/yandextank/stepper/missile.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/stepper/util.py` & `yandextank-1.9.3/yandextank/stepper/util.py`

 * *Files identical despite different names*

### Comparing `yandextank-1.9.0.post1/yandextank/validator/validator.py` & `yandextank-1.9.3/yandextank/validator/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,22 +63,32 @@
     }
 
     def __init__(self, configs, with_dynamic_options=True, core_section='core', error_output='validation_error.yaml'):
         self._errors = None
         if not isinstance(configs, list):
             configs = [configs]
         self.raw_config_dict = self.__load_multiple([config for config in configs if config is not None])
+        if self.raw_config_dict.get(core_section) is None:
+            self.raw_config_dict[core_section] = {}
         self.with_dynamic_options = with_dynamic_options
         self.CORE_SECTION = core_section
         self._validated = None
         self._plugins = None
         self.ERROR_OUTPUT = error_output
         self.BASE_SCHEMA = load_yaml_schema(pkg_resources.resource_filename('yandextank.core', 'config/schema.yaml'))
         self.PLUGINS_SCHEMA = load_yaml_schema(pkg_resources.resource_filename('yandextank.core', 'config/plugins_schema.yaml'))
 
+        # monkey-patch cerberus validator to allow description field
+        def _validate_description(self, description, field, value):
+            """ {'type': 'string'} """
+            pass
+
+        Validator._validate_description = _validate_description
+        self.PatchedValidator = InspectedValidator('Validator', (Validator,), {})
+
     def get_option(self, section, option):
         return self.validated[section][option]
 
     def has_option(self, section, option):
         return self.validated
 
     @property
@@ -152,45 +162,40 @@
             raise ValidationError((dict(errors)))
 
         for plugin_name, plugin_conf in results.items():
             core_validated[plugin_name] = plugin_conf
         return core_validated
 
     def __validate_core(self):
-        # monkey-patch to allow description field
-        def _validate_description(self, description, field, value):
-            """ {'type': 'string'} """
-            pass
-
-        Validator._validate_description = _validate_description
-        MyValidator = InspectedValidator('Validator', (Validator,), {})
-
-        v = MyValidator(allow_unknown=self.PLUGINS_SCHEMA)
+        v = self.PatchedValidator(allow_unknown=self.PLUGINS_SCHEMA)
         result = v.validate(self.raw_config_dict, self.BASE_SCHEMA)
         if not result:
             errors = v.errors
             for key, value in v.errors.items():
                 if 'must be of dict type' in value:
                     errors[key] = ['unknown field']
             raise ValidationError(errors)
         normalized = v.normalized(self.raw_config_dict)
         return self.__set_core_dynamic_options(normalized) if self.with_dynamic_options else normalized
 
     def __validate_plugin(self, config, schema):
         schema.update(self.PLUGINS_SCHEMA['schema'])
-        v = Validator(schema, allow_unknown=False)
+        v = self.PatchedValidator(schema, allow_unknown=False)
         # .validate() makes .errors as side effect if there's any
         if not v.validate(config):
             raise ValidationError(v.errors)
         # .normalized() returns config with defaults
         return v.normalized(config)
 
     def __set_core_dynamic_options(self, config):
         for option, setter in self.DYNAMIC_OPTIONS.items():
-            config[self.CORE_SECTION][option] = setter()
+            try:
+                config[self.CORE_SECTION][option] = setter()
+            except KeyError:
+                config[self.CORE_SECTION] = {option: setter()}
         return config
 
     def __get_cfg_updater(self, plugin_name):
         def cfg_updater(key, value):
             self.validated[plugin_name][key] = value
         return cfg_updater
```

### Comparing `yandextank-1.9.0.post1/yandextank.egg-info/PKG-INFO` & `yandextank-1.9.3/yandextank.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: yandextank
-Version: 1.9.0.post1
+Version: 1.9.3
 Summary: a performance measurement tool
 Home-page: http://yandex.github.io/yandex-tank/
 Author: Alexey Lavrenuke (load testing)
 Author-email: direvius@yandex-team.ru
 License: LGPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `yandextank-1.9.0.post1/yandextank.egg-info/SOURCES.txt` & `yandextank-1.9.3/yandextank.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,20 @@
 yandextank/plugins/Console/plugin.py
 yandextank/plugins/Console/screen.py
 yandextank/plugins/Console/config/schema.yaml
 yandextank/plugins/DataUploader/__init__.py
 yandextank/plugins/DataUploader/cli.py
 yandextank/plugins/DataUploader/client.py
 yandextank/plugins/DataUploader/plugin.py
+yandextank/plugins/DataUploader/config/postloader_schema.yaml
 yandextank/plugins/DataUploader/config/schema.yaml
+yandextank/plugins/Influx/__init__.py
+yandextank/plugins/Influx/decoder.py
+yandextank/plugins/Influx/plugin.py
+yandextank/plugins/Influx/config/schema.yaml
 yandextank/plugins/JMeter/__init__.py
 yandextank/plugins/JMeter/plugin.py
 yandextank/plugins/JMeter/reader.py
 yandextank/plugins/JMeter/config/jmeter_var_template.xml
 yandextank/plugins/JMeter/config/jmeter_writer.xml
 yandextank/plugins/JMeter/config/jmeter_writer_ext.xml
 yandextank/plugins/JMeter/config/schema.yaml
@@ -106,14 +111,17 @@
 yandextank/plugins/RCAssert/config/schema.yaml
 yandextank/plugins/ResourceCheck/__init__.py
 yandextank/plugins/ResourceCheck/plugin.py
 yandextank/plugins/ResourceCheck/config/schema.yaml
 yandextank/plugins/ShellExec/__init__.py
 yandextank/plugins/ShellExec/plugin.py
 yandextank/plugins/ShellExec/config/schema.yaml
+yandextank/plugins/ShootExec/__init__.py
+yandextank/plugins/ShootExec/plugin.py
+yandextank/plugins/ShootExec/config/schema.yaml
 yandextank/plugins/SvgReport/__init__.py
 yandextank/plugins/SvgReport/plugin.py
 yandextank/plugins/Telegraf/__init__.py
 yandextank/plugins/Telegraf/client.py
 yandextank/plugins/Telegraf/collector.py
 yandextank/plugins/Telegraf/config.py
 yandextank/plugins/Telegraf/decoder.py
```

