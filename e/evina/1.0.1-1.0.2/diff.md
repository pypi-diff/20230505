# Comparing `tmp/evina-1.0.1.tar.gz` & `tmp/evina-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\evina-1.0.1.tar", last modified: Wed May  3 15:05:37 2023, max compression
+gzip compressed data, was "dist\evina-1.0.2.tar", last modified: Fri May  5 16:39:18 2023, max compression
```

## Comparing `evina-1.0.1.tar` & `evina-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:05:37.664561 evina-1.0.1/
--rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-02 08:57:07.000000 evina-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0       90 2023-05-03 15:05:37.664561 evina-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 15:05:37.633318 evina-1.0.1/evina/
--rw-rw-rw-   0        0        0       90 2023-05-03 09:54:21.000000 evina-1.0.1/evina/__init__.py
--rw-rw-rw-   0        0        0      720 2023-05-03 09:54:21.000000 evina-1.0.1/evina/alipan.py
--rw-rw-rw-   0        0        0     4311 2023-05-03 09:54:21.000000 evina-1.0.1/evina/config.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:05:37.648941 evina-1.0.1/evina/disposition/
--rw-rw-rw-   0        0        0        0 2023-05-03 09:54:21.000000 evina-1.0.1/evina/disposition/__init__.py
--rw-rw-rw-   0        0        0      945 2023-05-03 09:54:21.000000 evina-1.0.1/evina/disposition/config.conf
--rw-rw-rw-   0        0        0      101 2023-05-03 09:54:21.000000 evina-1.0.1/evina/disposition/evina.conf
--rw-rw-rw-   0        0        0    14557 2023-05-03 09:54:21.000000 evina-1.0.1/evina/douyin.py
--rw-rw-rw-   0        0        0     9388 2023-05-03 09:54:21.000000 evina-1.0.1/evina/douyu.py
--rw-rw-rw-   0        0        0     1559 2023-05-03 09:54:21.000000 evina-1.0.1/evina/evina.py
--rw-rw-rw-   0        0        0      921 2023-05-02 15:23:04.000000 evina-1.0.1/evina/replacement.py
--rw-rw-rw-   0        0        0     1342 2023-05-03 09:54:21.000000 evina-1.0.1/evina/ssh.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:05:37.648941 evina-1.0.1/evina.egg-info/
--rw-rw-rw-   0        0        0       90 2023-05-03 15:05:37.000000 evina-1.0.1/evina.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-03 15:05:37.000000 evina-1.0.1/evina.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:05:37.000000 evina-1.0.1/evina.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-03 15:05:37.000000 evina-1.0.1/evina.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-03 15:05:37.000000 evina-1.0.1/evina.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 15:05:37.000000 evina-1.0.1/evina.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 15:05:37.664561 evina-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-03 15:05:23.000000 evina-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.332053 evina-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-05 16:32:20.000000 evina-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0       90 2023-05-05 16:39:18.331054 evina-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.309112 evina-1.0.2/evina/
+-rw-rw-rw-   0        0        0       90 2023-05-05 16:32:20.000000 evina-1.0.2/evina/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-05-05 16:32:20.000000 evina-1.0.2/evina/alipan.py
+-rw-rw-rw-   0        0        0     4757 2023-05-05 16:33:18.000000 evina-1.0.2/evina/config.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.327065 evina-1.0.2/evina/disposition/
+-rw-rw-rw-   0        0        0        0 2023-05-05 16:32:20.000000 evina-1.0.2/evina/disposition/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-05-05 16:34:25.000000 evina-1.0.2/evina/disposition/config.conf
+-rw-rw-rw-   0        0        0      101 2023-05-05 16:32:20.000000 evina-1.0.2/evina/disposition/evina.conf
+-rw-rw-rw-   0        0        0    14557 2023-05-05 16:32:20.000000 evina-1.0.2/evina/douyin.py
+-rw-rw-rw-   0        0        0     9388 2023-05-05 16:32:20.000000 evina-1.0.2/evina/douyu.py
+-rw-rw-rw-   0        0        0     1559 2023-05-05 16:32:20.000000 evina-1.0.2/evina/evina.py
+-rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.2/evina/replacement.py
+-rw-rw-rw-   0        0        0     1342 2023-05-05 16:32:20.000000 evina-1.0.2/evina/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:39:18.322078 evina-1.0.2/evina.egg-info/
+-rw-rw-rw-   0        0        0       90 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 16:39:18.000000 evina-1.0.2/evina.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 16:39:18.333050 evina-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-05 16:35:33.000000 evina-1.0.2/setup.py
```

### Comparing `evina-1.0.1/LICENSE` & `evina-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evina-1.0.1/README.md` & `evina-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `evina-1.0.1/evina/alipan.py` & `evina-1.0.2/evina/alipan.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.1/evina/config.py` & `evina-1.0.2/evina/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @File    : config.py
 '''
 
 import argparse
 import os
 import sys
 
+from aligo import Aligo
 from dynaconf import Dynaconf
 from loguru import logger
 
 from evina import replacement
 
 
 class Conf:
@@ -43,14 +44,21 @@
                                     dotenv_override=True)
 
         self.evina_douyin = Dynaconf(envvar_prefix='douyin',
                                      load_dotenv=True,
                                      dotenv_path=evina_file,
                                      dotenv_override=True)
 
+        replacement.Auth._EMAIL_USER = self.conf.settings.email_user
+        replacement.Auth._EMAIL_PASSWORD = self.conf.settings.email_password
+        email_host = replacement.Auth._EMAIL_USER.split('@')[1].split('.')
+        replacement.Auth._EMAIL_HOST = 'smtp.{}.{}'.format(
+            email_host[0], email_host[1])
+        Aligo(email=(self.conf.settings.email_user, '阿里云盘登录二维码验证'))
+
 
 class Arg(Conf):
     def __init__(self) -> None:
         super().__init__()
         if self.arg.start != None:
             self.start = self.arg.start[0]
             if self.arg.url != None:
```

### Comparing `evina-1.0.1/evina/disposition/config.conf` & `evina-1.0.2/evina/disposition/config.conf`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 EVINA_SETTINGS__DOCKER = false
 # 文件保存路径
 EVINA_SETTINGS__FILE = /home/code/evina
 # nodejs安装路径
 EVINA_SETTINGS__NODEJS = /usr/bin/node
 # nodejs包路径
 EVINA_SETTINGS__NODE_MODULES = /usr/lib/node_modules
-
+# 接收阿里云盘登录二维码的邮箱
+EVINA_SETTINGS__EMAIL_USER = 'xxxxxxx'
+# 接收阿里云盘登录二维码邮箱的STMP授权码
+EVINA_SETTINGS__EMAIL_PASSWORD = 'xxxxxxxxxx'
```

### Comparing `evina-1.0.1/evina/douyin.py` & `evina-1.0.2/evina/douyin.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.1/evina/douyu.py` & `evina-1.0.2/evina/douyu.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.1/evina/evina.py` & `evina-1.0.2/evina/evina.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.1/evina/replacement.py` & `evina-1.0.2/evina/replacement.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @File    : replacement.py
 '''
 
 import io
 import os
 from contextlib import contextmanager
 
+from aligo.core.Auth import Auth
 from dynaconf.vendor.dotenv.compat import StringIO
 from dynaconf.vendor.dotenv.main import DotEnv
 from loguru import logger
 
 
 class ReplaceMent:
     def __init__(self) -> None:
```

### Comparing `evina-1.0.1/evina/ssh.py` & `evina-1.0.2/evina/ssh.py`

 * *Files identical despite different names*

