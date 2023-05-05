# Comparing `tmp/sipiiiii-1.0.1.tar.gz` & `tmp/sipiiiii-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-1.0.1.tar", last modified: Fri May  5 15:41:38 2023, max compression
+gzip compressed data, was "sipiiiii-1.0.2.tar", last modified: Fri May  5 16:46:19 2023, max compression
```

## Comparing `sipiiiii-1.0.1.tar` & `sipiiiii-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:38.004816 sipiiiii-1.0.1/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.0.1/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 15:41:38.004135 sipiiiii-1.0.1/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3183 2023-05-05 10:00:41.000000 sipiiiii-1.0.1/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-05 15:41:38.005312 sipiiiii-1.0.1/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.968376 sipiiiii-1.0.1/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.0.1/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.980482 sipiiiii-1.0.1/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.0.1/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    12474 2023-05-04 14:34:32.000000 sipiiiii-1.0.1/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    21486 2023-05-05 15:40:56.000000 sipiiiii-1.0.1/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.992168 sipiiiii-1.0.1/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.0.1/sipiiiii/app/utils/HttpSDK.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-1.0.1/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.0.1/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.0.1/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.0.1/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.0.1/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8056 2023-05-05 10:00:55.000000 sipiiiii-1.0.1/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:37.975829 sipiiiii-1.0.1/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      792 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-05 15:41:37.000000 sipiiiii-1.0.1/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 15:41:38.002660 sipiiiii-1.0.1/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.0.1/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.0.1/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.0.1/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.0.1/template/python_streamlit.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.0.1/template/template_fastapi.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.0.1/template/template_flask.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.0.1/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-05 15:39:09.000000 sipiiiii-1.0.1/template/template_streamlit.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.728312 sipiiiii-1.0.2/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.0.2/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 16:46:19.727863 sipiiiii-1.0.2/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3183 2023-05-05 10:00:41.000000 sipiiiii-1.0.2/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-05 16:46:19.728543 sipiiiii-1.0.2/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.691638 sipiiiii-1.0.2/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.0.2/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.714001 sipiiiii-1.0.2/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.0.2/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    12474 2023-05-04 14:34:32.000000 sipiiiii-1.0.2/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    21490 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.719809 sipiiiii-1.0.2/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.0.2/sipiiiii/app/utils/HttpSDK.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-1.0.2/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.0.2/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.0.2/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.0.2/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.0.2/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8056 2023-05-05 10:00:55.000000 sipiiiii-1.0.2/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.707875 sipiiiii-1.0.2/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      792 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-05 16:46:19.000000 sipiiiii-1.0.2/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 16:46:19.726994 sipiiiii-1.0.2/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.0.2/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.0.2/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.0.2/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.0.2/template/python_streamlit.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.0.2/template/template_fastapi.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.0.2/template/template_flask.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.0.2/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-05 16:45:08.000000 sipiiiii-1.0.2/template/template_streamlit.yaml
```

### Comparing `sipiiiii-1.0.1/PKG-INFO` & `sipiiiii-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.0.1
+Version: 1.0.2
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-1.0.1/README.md` & `sipiiiii-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/pyproject.toml` & `sipiiiii-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-1.0.1/setup.py` & `sipiiiii-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="1.0.1",
+    version="1.0.2",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-1.0.1/sipiiiii/app/core.py` & `sipiiiii-1.0.2/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/sipiiiii/app/new_app.py` & `sipiiiii-1.0.2/sipiiiii/app/new_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "1.0.1"
+    return "1.0.2"
 
 
 def update_template():
     pass
 
 
 def activate_account():
@@ -616,15 +616,15 @@
         return False, _token
 
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
 
-    url = f"{server_host}/system/openapi/user/verify/code"
+    url = f"{server_host}/system/openapi/users/verify/code"
 
     response = https_get(url, headers=headers)
     if response.code != 200:
         return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, f"获取验证码异常: {response.msg}"
@@ -640,15 +640,15 @@
         except ValueError:
             print("验证码为纯6位数字")
             continue
         if verify_code == "":
             continue
         break
 
-    url = f"{server_host}/system/openapi/user/verify/code"
+    url = f"{server_host}/system/openapi/users/verify/code"
 
     response = https_post(
         url, json_data={"code": verify_code}, headers=headers)
     if response.code != 200:
         return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
@@ -657,15 +657,15 @@
     return True, response.msg
 
 
 def register(username, email, password):
     headers = {
         "Content-type": "application/json",
     }
-    url = f"{server_host}/system/openapi/user/register"
+    url = f"{server_host}/system/openapi/users/register"
 
     data = {
         "username": username,
         "password": password,
         "email": email
     }
 
@@ -681,15 +681,15 @@
     print("验证码也可以之后使用 -V 进行重新验证")
 
     home_dir_file = os.path.join(Path.home(), ".sipitoken")
     with open(home_dir_file, 'w', encoding='utf-8') as f:
         f.write(response.data['token'])
 
     headers["authorization"] = response.data['token']
-    url = f"{server_host}/system/openapi/user/verify/code"
+    url = f"{server_host}/system/openapi/users/verify/code"
 
     response = https_get(url, headers=headers)
     if response.code != 200:
         return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, f"获取验证码异常: {response.msg}"
```

### Comparing `sipiiiii-1.0.1/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-1.0.2/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/sipiiiii/app/utils/Tools.py` & `sipiiiii-1.0.2/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-1.0.2/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-1.0.2/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/sipiiiii/main.py` & `sipiiiii-1.0.2/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-1.0.2/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 1.0.1
+Version: 1.0.2
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-1.0.1/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-1.0.2/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/template/python_openai.j2` & `sipiiiii-1.0.2/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/template/template_fastapi.yaml` & `sipiiiii-1.0.2/template/template_fastapi.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/template/template_flask.yaml` & `sipiiiii-1.0.2/template/template_flask.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-1.0.1/template/template_openai.yaml` & `sipiiiii-1.0.2/template/template_openai.yaml`

 * *Files identical despite different names*

