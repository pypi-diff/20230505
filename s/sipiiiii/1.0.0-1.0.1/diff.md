# Comparing `tmp/sipiiiii-1.0.0.tar.gz` & `tmp/sipiiiii-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-1.0.0.tar", last modified: Fri May  5 14:40:51 2023, max compression
+gzip compressed data, was "sipiiiii-1.0.1.tar", last modified: Fri May  5 15:41:38 2023, max compression
```

## Comparing `sipiiiii-1.0.0.tar` & `sipiiiii-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.693316 sipiiiii-1.0.0/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.0.0/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 14:40:51.692321 sipiiiii-1.0.0/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3183 2023-05-05 10:00:41.000000 sipiiiii-1.0.0/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-05 14:40:51.693531 sipiiiii-1.0.0/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.658579 sipiiiii-1.0.0/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.0.0/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.671617 sipiiiii-1.0.0/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.0.0/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    12474 2023-05-04 14:34:32.000000 sipiiiii-1.0.0/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    21546 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.681986 sipiiiii-1.0.0/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.0.0/sipiiiii/app/utils/HttpSDK.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-1.0.0/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.0.0/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.0.0/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.0.0/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.0.0/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8056 2023-05-05 10:00:55.000000 sipiiiii-1.0.0/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.666223 sipiiiii-1.0.0/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      792 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.691165 sipiiiii-1.0.0/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.0.0/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.0.0/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.0.0/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.0.0/template/python_streamlit.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.0.0/template/template_fastapi.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.0.0/template/template_flask.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.0.0/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/template/template_streamlit.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:38.004816 sipiiiii-1.0.1/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.0.1/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 15:41:38.004135 sipiiiii-1.0.1/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3183 2023-05-05 10:00:41.000000 sipiiiii-1.0.1/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-05 15:41:38.005312 sipiiiii-1.0.1/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.968376 sipiiiii-1.0.1/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.0.1/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.980482 sipiiiii-1.0.1/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.0.1/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    12474 2023-05-04 14:34:32.000000 sipiiiii-1.0.1/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    21486 2023-05-05 15:40:56.000000 sipiiiii-1.0.1/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.992168 sipiiiii-1.0.1/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.0.1/sipiiiii/app/utils/HttpSDK.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-1.0.1/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.0.1/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.0.1/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.0.1/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.0.1/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8056 2023-05-05 10:00:55.000000 sipiiiii-1.0.1/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.975829 sipiiiii-1.0.1/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      792 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:38.002660 sipiiiii-1.0.1/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.0.1/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.0.1/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.0.1/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.0.1/template/python_streamlit.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.0.1/template/template_fastapi.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.0.1/template/template_flask.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.0.1/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/template/template_streamlit.yaml
```

### Comparing `sipiiiii-1.0.0/PKG-INFO` & `sipiiiii-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.0.0
+Version: 1.0.1
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-1.0.0/README.md` & `sipiiiii-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/pyproject.toml` & `sipiiiii-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-1.0.0/setup.py` & `sipiiiii-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="1.0.0",
+    version="1.0.1",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-1.0.0/sipiiiii/app/core.py` & `sipiiiii-1.0.1/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/sipiiiii/app/new_app.py` & `sipiiiii-1.0.1/sipiiiii/app/new_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,32 +440,28 @@
 
     # bar = ProgPercent(50, monitor=True)
     print("正在远程部署...\r\n")
     i = 0
     while True:
         if i >= 60 * 5:
             return False, "\r\n获取状态超时, 请用 sipiiiii -l查看应用列表"
-
-        status, info_json, _ = get_app_info(filename)
+        i += 1
+        time.sleep(1)
+        status, info_json, _ = get_app_info(filename.lower())
         if not status:
-            # bar.update(50)
-            # return False, "\r\n部署成功，状态获取失败"
             continue
 
         if info_json['ServerStatus'] == "close" or info_json['ServerStatus'] == "exited":
             # bar.update(50)
             return True, f"\r\n应用程序部署出错，日志: \r\n{info_json['Log']}"
 
         if info_json['ServerStatus'] == "created" or info_json['ServerStatus'] == "running":
             # bar.update(50)
             return True, f"\r\n部署成功, \r\n域名: {info_json['Domain']}"
 
-        i += 1
-        time.sleep(1)
-
     # return True, response.data
 
 
 def login(email, password):
     url = f"{server_host}/system/openapi/users/login"
     headers = {
         "Content-type": "application/json"
@@ -550,15 +546,15 @@
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     status, app_name, _, _ = get_app_name(app_name)
     if not status:
         return False, {}, f"获取应用名错误: {app_name}"
-
+    app_name = app_name.lower()
     data = {"app_name": app_name}
 
     response = https_post(url, json_data=data, headers=headers)
     if response.code != 200:
         return False, {}, "服务器内部错误, 请稍后再试"
 
     if not response.success:
@@ -603,15 +599,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "1.0.0"
+    return "1.0.1"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-1.0.0/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-1.0.1/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/sipiiiii/app/utils/Tools.py` & `sipiiiii-1.0.1/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-1.0.1/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-1.0.1/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/sipiiiii/main.py` & `sipiiiii-1.0.1/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-1.0.1/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.0.0
+Version: 1.0.1
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-1.0.0/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-1.0.1/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/template/python_openai.j2` & `sipiiiii-1.0.1/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/template/template_fastapi.yaml` & `sipiiiii-1.0.1/template/template_fastapi.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/template/template_flask.yaml` & `sipiiiii-1.0.1/template/template_flask.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.0/template/template_openai.yaml` & `sipiiiii-1.0.1/template/template_openai.yaml`

 * *Files identical despite different names*

