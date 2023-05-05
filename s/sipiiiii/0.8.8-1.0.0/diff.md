# Comparing `tmp/sipiiiii-0.8.8.tar.gz` & `tmp/sipiiiii-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.8.8.tar", last modified: Thu May  4 03:44:11 2023, max compression
+gzip compressed data, was "sipiiiii-1.0.0.tar", last modified: Fri May  5 14:40:51 2023, max compression
```

## Comparing `sipiiiii-0.8.8.tar` & `sipiiiii-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.136856 sipiiiii-0.8.8/
--rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-0.8.8/MANIFEST.in
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-04 03:44:11.135774 sipiiiii-0.8.8/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.8.8/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-04 03:34:11.000000 sipiiiii-0.8.8/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-04 03:44:11.137224 sipiiiii-0.8.8/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-04 03:34:43.000000 sipiiiii-0.8.8/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.099174 sipiiiii-0.8.8/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.8.8/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.114184 sipiiiii-0.8.8/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.8.8/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    11056 2023-05-04 03:25:50.000000 sipiiiii-0.8.8/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    21799 2023-05-04 03:34:11.000000 sipiiiii-0.8.8/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.127700 sipiiiii-0.8.8/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-0.8.8/sipiiiii/app/utils/HttpSDK.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-0.8.8/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.8.8/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.8.8/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-03 08:02:36.000000 sipiiiii-0.8.8/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.8.8/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-04 03:34:11.000000 sipiiiii-0.8.8/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8632 2023-05-04 03:31:44.000000 sipiiiii-0.8.8/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.107385 sipiiiii-0.8.8/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      699 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/requires.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-04 03:44:10.000000 sipiiiii-0.8.8/sipiiiii.egg-info/top_level.txt
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-04 03:44:11.134295 sipiiiii-0.8.8/template/
--rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-0.8.8/template/python_fastapi.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-04-18 15:46:06.000000 sipiiiii-0.8.8/template/python_flask.j2
--rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-0.8.8/template/python_openai.j2
--rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-0.8.8/template/template_openai.yaml
--rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-0.8.8/template/template_other.yaml
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.693316 sipiiiii-1.0.0/
+-rw-r--r--   0 j0hn       (501) staff       (20)       18 2023-05-03 12:00:50.000000 sipiiiii-1.0.0/MANIFEST.in
+-rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 14:40:51.692321 sipiiiii-1.0.0/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3183 2023-05-05 10:00:41.000000 sipiiiii-1.0.0/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      634 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-05 14:40:51.693531 sipiiiii-1.0.0/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     3401 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.658579 sipiiiii-1.0.0/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-1.0.0/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.671617 sipiiiii-1.0.0/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-1.0.0/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    12474 2023-05-04 14:34:32.000000 sipiiiii-1.0.0/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    21546 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.681986 sipiiiii-1.0.0/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7845 2023-05-03 09:19:05.000000 sipiiiii-1.0.0/sipiiiii/app/utils/HttpSDK.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1565 2023-05-04 03:09:45.000000 sipiiiii-1.0.0/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-1.0.0/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-1.0.0/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      151 2023-05-04 12:35:33.000000 sipiiiii-1.0.0/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-1.0.0/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       17 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8056 2023-05-05 10:00:55.000000 sipiiiii-1.0.0/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.666223 sipiiiii-1.0.0/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3700 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      792 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)      104 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/requires.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-05 14:40:51.000000 sipiiiii-1.0.0/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-05 14:40:51.691165 sipiiiii-1.0.0/template/
+-rw-r--r--   0 j0hn       (501) staff       (20)      366 2023-04-18 15:46:14.000000 sipiiiii-1.0.0/template/python_fastapi.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      371 2023-05-04 06:44:54.000000 sipiiiii-1.0.0/template/python_flask.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)     1505 2023-05-01 16:17:11.000000 sipiiiii-1.0.0/template/python_openai.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      238 2023-05-04 06:44:09.000000 sipiiiii-1.0.0/template/python_streamlit.j2
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-01 16:06:57.000000 sipiiiii-1.0.0/template/template_fastapi.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      762 2023-05-04 06:17:59.000000 sipiiiii-1.0.0/template/template_flask.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)      795 2023-05-03 13:15:30.000000 sipiiiii-1.0.0/template/template_openai.yaml
+-rw-r--r--   0 j0hn       (501) staff       (20)       88 2023-05-05 14:39:22.000000 sipiiiii-1.0.0/template/template_streamlit.yaml
```

### Comparing `sipiiiii-0.8.8/PKG-INFO` & `sipiiiii-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.8
+Version: 1.0.0
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 ## 产品优势
 - 简单易用:通过命令行工具,可以极简操作完成应用的部署、管理等
 - 低成本:积分制度,可以零成本体验所有功能
 - 应用生成:支持根据模版一键生成应用框架
 - chatgpt插件专属:深度整合chatgpt插件系统,提供专属托管解决方案
 ## 主要功能
 - 应用部署:支持本地部署与远程部署,可一键部署应用 
-- 应用管理:可启动、停止、重启、删除应用等
+- 应用管理:可启动、停止、重启应用等
 - 应用生成:可根据yaml模版或者AI自动生成应用框架
 - 账号管理:支持注册、登录、邮件激活等
 - 积分系统:通过各功能消耗积分,可零成本使用
 - chatgpt插件支持:提供chatgpt插件托管解决方案
 ## 未来计划
 - 增加更多语言支持:如Ruby、Rust、Go等
 - 添加更多应用模版
@@ -44,15 +44,15 @@
 ## 账号管理
 ### 登录账号
 
 sipiiiii -L 或 --login  
 登录后,token有效期为3天
 ### 注册账号
 
-sipiiiii -S 或 --register
+sipiiiii -R 或 --register
  
 ### 邮箱激活账号
 
 sipiiiii -A 或 --activate
 激活后的账号赠送10积分
 ### 查看积分余额
 
@@ -91,18 +91,14 @@
 sipiiiii -s <app name> 或 --stop <app name>
 sipiiiii -s <test.yaml> 或 --stop <test.yaml> 
 ### 重启应用(非本地部署)
 
 sipiiiii -r <app name> 或 --restart <app name>  
 sipiiiii -r <test.yaml> 或 --restart <test.yaml>
  
-### 删除应用(非本地部署)
- 
-sipiiiii -DE <app name> 或 --delete <app name>
-sipiiiii -DE <test.yaml> 或 --delete <test.yaml>
 ## 示例
 
 sipiiiii -n test.yaml  
 sipiiiii -LD test.yaml
 sipiiiii -LD your-app-name
 sipiiiii -D
 sipiiiii -L
```

### Comparing `sipiiiii-0.8.8/README.md` & `sipiiiii-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## 产品优势
 - 简单易用:通过命令行工具,可以极简操作完成应用的部署、管理等
 - 低成本:积分制度,可以零成本体验所有功能
 - 应用生成:支持根据模版一键生成应用框架
 - chatgpt插件专属:深度整合chatgpt插件系统,提供专属托管解决方案
 ## 主要功能
 - 应用部署:支持本地部署与远程部署,可一键部署应用 
-- 应用管理:可启动、停止、重启、删除应用等
+- 应用管理:可启动、停止、重启应用等
 - 应用生成:可根据yaml模版或者AI自动生成应用框架
 - 账号管理:支持注册、登录、邮件激活等
 - 积分系统:通过各功能消耗积分,可零成本使用
 - chatgpt插件支持:提供chatgpt插件托管解决方案
 ## 未来计划
 - 增加更多语言支持:如Ruby、Rust、Go等
 - 添加更多应用模版
@@ -29,15 +29,15 @@
 ## 账号管理
 ### 登录账号
 
 sipiiiii -L 或 --login  
 登录后,token有效期为3天
 ### 注册账号
 
-sipiiiii -S 或 --register
+sipiiiii -R 或 --register
  
 ### 邮箱激活账号
 
 sipiiiii -A 或 --activate
 激活后的账号赠送10积分
 ### 查看积分余额
 
@@ -76,18 +76,14 @@
 sipiiiii -s <app name> 或 --stop <app name>
 sipiiiii -s <test.yaml> 或 --stop <test.yaml> 
 ### 重启应用(非本地部署)
 
 sipiiiii -r <app name> 或 --restart <app name>  
 sipiiiii -r <test.yaml> 或 --restart <test.yaml>
  
-### 删除应用(非本地部署)
- 
-sipiiiii -DE <app name> 或 --delete <app name>
-sipiiiii -DE <test.yaml> 或 --delete <test.yaml>
 ## 示例
 
 sipiiiii -n test.yaml  
 sipiiiii -LD test.yaml
 sipiiiii -LD your-app-name
 sipiiiii -D
 sipiiiii -L
```

### Comparing `sipiiiii-0.8.8/pyproject.toml` & `sipiiiii-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sipiiiii"
-version = "0.8.8"
+version = "1.0.0"
 authors = [
   { name="DeplRun", email="sipiiiii@example.com" },
 ]
 description = "sipiiiii定位为简单易用的云应用托管平台"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sipiiiii-0.8.8/setup.py` & `sipiiiii-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     print(msg)
     sys.exit(1)
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="sipiiiii",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.8.8",
+    version="1.0.0",
     # 作者名
     author="sipiiiii@admin",
     # 作者邮箱
     author_email="j0hn.wahahaha@gmail.com",
     # 包的简介描述
     description="depl sipiiiii, App Development Framework",
     # 包的详细介绍(一般通过加载README.md)
```

### Comparing `sipiiiii-0.8.8/sipiiiii/app/core.py` & `sipiiiii-1.0.0/sipiiiii/app/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,33 +7,28 @@
 from pathlib import Path
 from jinja2 import Environment, FileSystemLoader
 from .utils.config import fix
 from .utils.Tools import get_current_path, read_app_yaml
 
 
 class ExecAppClass(object):
-    def __init__(self, cwd, file_path, code_type):
+    def __init__(self,file_path):
         self.file_path = file_path
-        self.cwd = cwd
-        self. code_type = code_type
 
     def run_python_app(self):
-        port = input("输入端口:")
-        try:
-            port = int(port)
-        except ValueError:
-            return False, "错误: 输入的端口不是整型."
-
-        sys.path.append(self.cwd)
-        try:
-            from app import app
-        except Exception as e:
-            return False, f"错误: sipiiii项目路径. {e}"
-
-        app.run(debug=True, port=port)
+        cmd_line = input("请输出python解析器[python,python3或pypy](默认python):")
+        if cmd_line is None or cmd_line == "":
+            cmd_line = "python"
+        # sys.path.append(self.cwd)
+        # try:
+        #     from app import app
+        # except Exception as e:
+        #     return False, f"错误: sipiiii项目路径. {e}"
+        os.system(f"{cmd_line} {self.file_path}")
+        # app.run(debug=True, port=port)
         return True, "服务器运行正常过，目前服务器已停止..."
 
 
 class CreateAppTypeClass(object):
     def __init__(self, app_name, app_yaml, app_dir):
         self.app_name = app_name
         self.app_yaml = app_yaml
@@ -48,19 +43,26 @@
                 rmtree(self.app_name)
             elif is_rm == "n":
                 return True, "退出"
 
         path = Path(f"{self.app_name}")
         path.mkdir(parents=True, exist_ok=True)
 
-    def __create_code(self, code_type, app_type):
+    def __create_code(self, code_type, app_type, code="", code_name="app"):
+        if code_name != "app":
+            status, msg = create_app_code(
+                self.app_name, code_type, code, code_name)
+            if not status:
+                return False, f"创建代码出错, {msg}"
+            return True, msg
+
         status, msg = create_framework_code(
-            self.app_dir, self.app_name, self.app_yaml, code_type, app_type)
+            self.app_dir, self.app_name, self.app_yaml, code_type, app_type, code_name)
         if not status:
-            return False, "创建框架代码出错, {msg}"
+            return False, f"创建框架代码出错, {msg}"
         return True, msg
 
     def __create_python_requirements(self, app_type):
         requirements = input("输入导入的库(多个库用逗号分隔):")
         if requirements is None or requirements == "":
             requirements = ""
 
@@ -75,20 +77,56 @@
         if app_type == "fastapi":
             requirements.append('fastapi')
         if app_type == "flask":
             requirements.append('flask')
         if app_type == "openai":
             requirements.append('quart')
             requirements.append('quart_cors')
+        if app_type == "streamlit":
+            requirements.append('streamlit')
 
         status, requirements_file_path = create_requirements(
             self.app_name, requirements)
         if not status:
             return False, requirements_file_path
 
+    def create_streamlit_app(self, code_type):
+        self.__create_app_path()
+        if code_type == "python":
+            self.__create_python_requirements("streamlit")
+
+        status, openapi_file_path = create_app_yaml(
+            self.app_name, self.app_yaml, "streamlit")
+        if not status:
+            return False, openapi_file_path
+
+        code = f"""
+import streamlit as st
+
+def main():
+    st.markdown("hello world!")
+
+if __name__ == "__main__":
+    st.set_page_config(
+        page_title="{self.app_name}", page_icon=":pencil2:"
+    )
+    st.title("{self.app_name}")
+    # st.sidebar.subheader("Configuration")
+    main()
+        """
+        ststus, msg = self.__create_code(
+            code_type, "streamlit", code=code, code_name="main")
+        if not ststus:
+            return False, msg
+
+        ststus, msg = self.__create_code(code_type, "streamlit")
+        if not ststus:
+            return False, msg
+        return True, f"创建streamlit框架代码成功, 项目目录: ./{self.app_name}"
+
     def create_flask_app(self, code_type):
         self.__create_app_path()
 
         if code_type == "python":
             self.__create_python_requirements("flask")
 
         status, openapi_file_path = create_app_yaml(
@@ -219,16 +257,16 @@
     new_fix = {v: k for k, v in fix.items()}
     return True, new_fix[_fix]
 
 
 def yaml_app_info(yaml_file, app_type):
     openapi_yaml = None
     aiapi_dir = get_current_path()
-    if app_type != "openai":
-        app_type = "other"
+    # if app_type != "openai":
+    #     app_type = "other"
     if yaml_file is None:
         openapi_yaml = read_app_yaml(aiapi_dir, app_type)
     else:
         openapi_yaml = read_app_yaml(yaml_file, app_type)
     if openapi_yaml == "":
         return False, "没找到yaml文件.", None, None
     app_name = ""
@@ -240,28 +278,14 @@
     if app_name == "":
         return False, "yaml中没有找到 yaml[info][title]", None, None
 
     app_name = app_name.replace(" ", "")
     return True, app_name, openapi_yaml, aiapi_dir
 
 
-def create_directory(directory_name):
-    current_path = get_current_path()
-    new_directory_path = os.path.join(current_path, directory_name)
-
-    if not os.path.exists(new_directory_path):
-        os.mkdir(new_directory_path)
-        print(f"目录 '{directory_name}' 创建成功!")
-        return True, new_directory_path
-    else:
-        print(f"目录 '{directory_name}' 已存在.")
-
-    return False, ""
-
-
 def create_requirements(directory_path, requirements):
     if type(requirements) != list:
         return False, "requirements 错误!"
 
     if not os.path.exists(directory_path):
         return False, f"{directory_path} 没有找到."
 
@@ -310,27 +334,41 @@
     # plugin_json_data = "\n".join(plugin_json_file_path)
     with open(openapi_yaml_file_path, encoding="utf-8", mode="w") as f:
         yaml.dump(openapi_yaml, stream=f, allow_unicode=True)
 
     return True, openapi_yaml_file_path
 
 
-def create_framework_code(directory_path, app_path, openapi_yaml, code_type, app_type):
+def create_app_code(app_path, code_type, code, code_name):
+    _fix = fix.get(code_type, None)
+    if _fix is None:
+        return False, "没有获取到应用类型"
+
+    app_file = os.path.join(app_path, f"{code_name}.{_fix}")
+    with open(app_file, 'w', encoding="utf-8") as f:
+        f.write(code)
+
+    return True, "创建代码成功"
+
+
+def create_framework_code(directory_path, app_path, openapi_yaml, code_type, app_type, code_name="app"):
+    if openapi_yaml.get("paths", None) is None:
+        openapi_yaml['paths'] = []
     env = Environment(loader=FileSystemLoader(f"{directory_path}"))
     # template.j2
     # if app_type != "openai":
     #     app_type = "other"
     j2_file = f"{code_type}_{app_type}"
     try:
         template = env.get_template(f'{j2_file}.j2')
         output = template.render(paths=openapi_yaml['paths'])
     except Exception as e:
         return False, str(e)
     _fix = fix.get(code_type, None)
     if _fix is None:
         return False, "没有获取到应用类型"
     # Write the output to a Python file
-    app_file = os.path.join(app_path, f"app.{_fix}")
+    app_file = os.path.join(app_path, f"{code_name}.{_fix}")
     with open(app_file, 'w', encoding="utf-8") as f:
         f.write(output)
 
     return True, "创建框架代码成功"
```

### Comparing `sipiiiii-0.8.8/sipiiiii/app/new_app.py` & `sipiiiii-1.0.0/sipiiiii/app/new_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     while True:
         time.sleep(60 * 30)
         outside_ip = get_outside_ip()
         headers = {
             "Content-type": "application/json",
             "authorization": _token
         }
-        url = f"{server_host}/system/openapi/app/stop"
+        url = f"{server_host}/system/openapi/modify/domain/bind/ip"
         data = {
             "domain": domain,
             "ip": outside_ip
         }
         response = https_post(url, json_data=data, headers=headers)
         if not response.success:
             print(f"更新域名错误: {response.msg}")
@@ -56,15 +56,15 @@
 
     print("""
     *** 应用名称必须英文
     *** 可以使用向导模式创建应用和使用模版创建应用
         """)
 
     while True:
-        is_wizard_create = input("是否使用向导创建应用(y/n):")
+        is_wizard_create = input("y使用向导创建应用,n使用模版生成(y/n):")
         is_wizard_create = is_wizard_create.lower()
 
         if is_wizard_create == "y":
             app_name = input("请输入应用名:")
             if app_name == "" or not is_encomm_char(app_name):
                 print("应用名不能为空, 并且应用名只能使用英文字母")
                 continue
@@ -164,14 +164,16 @@
 
     return True, yaml_data
 
 # 通过yaml直接创建APP
 
 
 def create_app(yaml_file=None):
+    if yaml_file is not None and yaml_file.find(".yaml") == -1:
+        return False, "参数错误, 参数并不是Yaml文件, 请查看 sipiiiii -h", "", ""
     status, _token = get_token()
     if not status:
         return False, _token, "", ""
 
     while True:
         code_type = input(
             f"请输入创建编程语言{list(fix.keys())}(默认第一个): "
@@ -217,15 +219,15 @@
     if not file_path.exists():
         return False, "错误: 不存在项目路径, 请到项目路径下运行"
 
     status, code_type = get_app_code_type(file_path)
     if not status:
         return False, code_type
 
-    eac = ExecAppClass(cwd, file_path, code_type)
+    eac = ExecAppClass(file_path)
 
     method_of_catc = getattr(eac, f"run_{code_type}_app")
     status, msg = method_of_catc()
 
     return status, msg
 
 
@@ -234,24 +236,24 @@
     if not status:
         return False, _token
 
     status, app_name, app_yaml, _ = get_app_name(yaml_file_name, True)
     if not status:
         return False, f"获取应用名错误: {app_name}"
 
-    app_cn_name = input("请输出应用别名:")
+    app_cn_name = input("请输入应用别名:")
     if app_cn_name == "":
         app_cn_name = app_name
 
     print(f"本地部署: {app_name} 项目\r\n")
 
     description = ""
     try:
         description = app_yaml.get(
-            'info', {}).get('description')
+            'info', {}).get('description', "")
     except Exception as e:
         return False, str(e)
 
     outside_ip = get_outside_ip()
     if outside_ip == "":
         return False, "无法访问互联网"
 
@@ -265,15 +267,15 @@
     if run_main.find(".") == 0:
         return False, "APP运行文件必须是文件名加文件后缀"
 
     run_main_fix = run_main.split(".")
     if len(run_main_fix) != 2:
         return False, "APP运行文件输入不合法"
 
-    if run_main_fix[-1] not in list(fix.keys()):
+    if run_main_fix[-1] not in list(fix.values()):
         return False, f"APP运行文件不在允许的列表范围内: {list(fix.keys())}"
 
     cwd = os.getcwd()
     file_path = os.path.join(cwd, run_main)
     file_path = Path(f'{file_path}')
     if not file_path.exists():
         return False, "错误: 不存在项目路径, 请到项目路径下运行"
@@ -298,22 +300,22 @@
     if response.code != 200:
         return False, "内部服务器错误，请稍后再试"
 
     if not response.success:
         return False, response.msg
 
     p = multiprocessing.Process(
-        target=process_update_outside_ip, args=(response.domain, _token), daemon=True)
+        target=process_update_outside_ip, args=(response.data['domain'], _token), daemon=True)
     p.start()
 
     status, code_type = get_app_code_type(file_path)
     if not status:
         return False, code_type
 
-    eac = ExecAppClass(cwd, file_path, code_type)
+    eac = ExecAppClass(file_path)
 
     method_of_catc = getattr(eac, f"run_{code_type}_app")
     status, msg = method_of_catc()
 
     return status, msg
 
 
@@ -428,33 +430,42 @@
         return False, "内部服务器错误，请稍后再试"
 
     if not response.success:
         return False, response.msg
 
     # return True, "ok"
 
-    status, info_json, _ = get_app_info(filename)
-    if not status:
-        return False, "部署成功，状态获取失败"
+    # status, info_json, _ = get_app_info(filename)
+    # if not status:
+    #     return False, "部署成功，状态获取失败"
 
     # bar = ProgPercent(50, monitor=True)
     print("正在远程部署...\r\n")
+    i = 0
     while True:
+        if i >= 60 * 5:
+            return False, "\r\n获取状态超时, 请用 sipiiiii -l查看应用列表"
+
         status, info_json, _ = get_app_info(filename)
         if not status:
             # bar.update(50)
-            return False, "\r\n部署成功，状态获取失败"
+            # return False, "\r\n部署成功，状态获取失败"
+            continue
+
         if info_json['ServerStatus'] == "close" or info_json['ServerStatus'] == "exited":
             # bar.update(50)
             return True, f"\r\n应用程序部署出错，日志: \r\n{info_json['Log']}"
 
         if info_json['ServerStatus'] == "created" or info_json['ServerStatus'] == "running":
             # bar.update(50)
             return True, f"\r\n部署成功, \r\n域名: {info_json['Domain']}"
 
+        i += 1
+        time.sleep(1)
+
     # return True, response.data
 
 
 def login(email, password):
     url = f"{server_host}/system/openapi/users/login"
     headers = {
         "Content-type": "application/json"
@@ -482,15 +493,15 @@
 
 
 def get_tally():
     status, _token = get_token()
     if not status:
         return False, _token
 
-    url = f"{server_host}/system/openapi/user/tally"
+    url = f"{server_host}/system/openapi/users/tally"
     headers = {
         "Content-type": "application/json",
         "authorization": _token
     }
     response = https_get(url, headers=headers)
     # response = requests.get(url, headers=headers, timeout=20)
     if response.code != 200:
@@ -526,36 +537,14 @@
 
     if not response.success:
         return False, response.msg
 
     return True, response.msg
 
 
-def delete_app(app_name):
-    status, _token = get_token()
-    if not status:
-        return False, _token
-
-    status, app_name, _, _ = get_app_name(app_name)
-    if not status:
-        return False, f"获取应用名错误: {app_name}"
-
-    data = {"app_name": app_name}
-    headers = {
-        "Content-type": "application/json",
-        "authorization": _token
-    }
-    url = f"{server_host}/system/openapi/app/del"
-    response = https_post(url, json_data=data, headers=headers)
-    if not response.success:
-        return False, response.msg
-
-    return True, response.msg
-
-
 def get_app_info(app_name=None):
     status, _token = get_token()
     if not status:
         return False, {}, _token
 
     url = f"{server_host}/system/openapi/app/status"
     headers = {
@@ -605,24 +594,24 @@
         return False, "服务器内部错误, 请稍后再试"
 
     if not response.success:
         return False, response.msg
 
     app_list = response.data['data']
     table = pt.PrettyTable(
-        ['应用名', '应用别名', '域名', '服务状态', '应用状态', '创建时间'])
+        ['应用名', '应用别名', '域名', '应用状态', '创建时间'])
     for app in app_list:
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
-                      app['ServerStatus'], app['AppStast'], app['CreateTime']))
+                      app['ServerStatus'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.8.8"
+    return "1.0.0"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.8.8/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-1.0.0/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.8/sipiiiii/app/utils/Tools.py` & `sipiiiii-1.0.0/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.8/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-1.0.0/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.8/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-1.0.0/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.8/sipiiiii/main.py` & `sipiiiii-1.0.0/sipiiiii/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 用法: sipiiiii [选项]
 
   显示帮助信息:
     sipiiiii -h 或 --help
 
   账号管理:
-    登录你的sipiiiii账号, 登录后token有消息为3天:
+    登录你的sipiiiii账号, 登录后token有效期为3天:
       sipiiiii -L 或 --login
 
     注册一个sipiiiii账号:
-      sipiiiii -S 或 --register
+      sipiiiii -R 或 --register
 
     邮件激活你的sipiiiii账号, 每个激活后的账号将赠送10积分:
       sipiiiii -A 或 --activate
 
     查看你的剩余积分:
       sipiiiii -t 或 --tally
 
@@ -70,18 +70,14 @@
       sipiiiii -s <app name> 或 --stop <app name>
       sipiiiii -s <test.yaml> 或 --stop <test.yaml>
 
     重启你的应用(非本地部署):
       sipiiiii -r <app name> 或 --restart <app name>
       sipiiiii -r <test.yaml> 或 --restart <test.yaml>
       
-    删除你的应用(非本地部署):
-      sipiiiii -DE <app name> 或 --delete <app name>
-      sipiiiii -DE <test.yaml> 或 --delete <test.yaml>
-
   示例:
     使用注册邮箱和密码进行登录
     sipiiiii -L 
     创建一个新的应用, 创建后编写相关的业务代码
     sipiiiii -n 
     进入到应用目录后, 进行部署
     sipiiiii -D
@@ -114,16 +110,14 @@
                         required=False, nargs='?', const='default_value')
     parser.add_argument('-i', '--info', help='显示应用信息',
                         required=False, nargs='?', const='default_value')
     parser.add_argument('-s', '--stop', help='停止应用',
                         required=False, nargs='?', const='default_value')
     parser.add_argument('-r', '--restart', help='重启应用',
                         required=False, nargs='?', const='default_value')
-    parser.add_argument('-DE', '--delete', help='删除应用',
-                        required=False, nargs='?', const='default_value')
     parser.add_argument('-LD', '--localdepl', help='本地部署应用',
                         required=False, nargs='?', const='default_value')
     args = vars(parser.parse_args())
 
     if args is None:
         print(echo_help())
         if version != get_cli_server_version():
@@ -146,15 +140,15 @@
         msg = ""
         if args['new'] == "default_value":
             status, msg, app_name = create_app_project()
         else:
             status, msg, app_name, _ = create_app(args['new'])
 
         if status:
-            print(f"{msg} 项目目录在当前文件夹下的: {app_name}")
+            print(f"{msg}")
         else:
             print(msg)
 
     elif args['login']:
         email = input("输入你的email:")
         password = getpass.getpass('输入你的密码:')
         if email == "" or email is None:
@@ -219,23 +213,15 @@
         msg = ""
         if args['restart'] == "default_value":
             status, msg = restart_app(None)
         else:
             status, msg = restart_app(args['restart'])
 
         print(msg)
-    elif args['delete']:
-        status = False
-        msg = ""
-        if args['delete'] == "default_value":
-            status, msg = delete_app(None)
-        else:
-            status, msg = delete_app(args['delete'])
 
-        print(msg)
     elif args['localdepl']:
         status = False
         msg = ""
         if args['localdepl'] == "default_value":
             status, msg = localdepl(None)
         else:
             status, msg = localdepl(args['localdepl'])
@@ -243,12 +229,12 @@
         print(msg)
 
     elif args['help']:
         print(echo_help())
     else:
         print(echo_help())
         if version != get_cli_server_version():
-            print("\r\npip install sipiiiii")
+            print("\r\npip install sipiiiii -U")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sipiiiii-0.8.8/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-1.0.0/sipiiiii.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.8.8
+Version: 1.0.0
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 ## 产品优势
 - 简单易用:通过命令行工具,可以极简操作完成应用的部署、管理等
 - 低成本:积分制度,可以零成本体验所有功能
 - 应用生成:支持根据模版一键生成应用框架
 - chatgpt插件专属:深度整合chatgpt插件系统,提供专属托管解决方案
 ## 主要功能
 - 应用部署:支持本地部署与远程部署,可一键部署应用 
-- 应用管理:可启动、停止、重启、删除应用等
+- 应用管理:可启动、停止、重启应用等
 - 应用生成:可根据yaml模版或者AI自动生成应用框架
 - 账号管理:支持注册、登录、邮件激活等
 - 积分系统:通过各功能消耗积分,可零成本使用
 - chatgpt插件支持:提供chatgpt插件托管解决方案
 ## 未来计划
 - 增加更多语言支持:如Ruby、Rust、Go等
 - 添加更多应用模版
@@ -44,15 +44,15 @@
 ## 账号管理
 ### 登录账号
 
 sipiiiii -L 或 --login  
 登录后,token有效期为3天
 ### 注册账号
 
-sipiiiii -S 或 --register
+sipiiiii -R 或 --register
  
 ### 邮箱激活账号
 
 sipiiiii -A 或 --activate
 激活后的账号赠送10积分
 ### 查看积分余额
 
@@ -91,18 +91,14 @@
 sipiiiii -s <app name> 或 --stop <app name>
 sipiiiii -s <test.yaml> 或 --stop <test.yaml> 
 ### 重启应用(非本地部署)
 
 sipiiiii -r <app name> 或 --restart <app name>  
 sipiiiii -r <test.yaml> 或 --restart <test.yaml>
  
-### 删除应用(非本地部署)
- 
-sipiiiii -DE <app name> 或 --delete <app name>
-sipiiiii -DE <test.yaml> 或 --delete <test.yaml>
 ## 示例
 
 sipiiiii -n test.yaml  
 sipiiiii -LD test.yaml
 sipiiiii -LD your-app-name
 sipiiiii -D
 sipiiiii -L
```

### Comparing `sipiiiii-0.8.8/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-1.0.0/sipiiiii.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,9 +19,12 @@
 sipiiiii/app/utils/ZipFileTool.py
 sipiiiii/app/utils/__init__.py
 sipiiiii/app/utils/config.py
 sipiiiii/app/utils/formatConversion.py
 template/python_fastapi.j2
 template/python_flask.j2
 template/python_openai.j2
+template/python_streamlit.j2
+template/template_fastapi.yaml
+template/template_flask.yaml
 template/template_openai.yaml
-template/template_other.yaml
+template/template_streamlit.yaml
```

### Comparing `sipiiiii-0.8.8/template/python_openai.j2` & `sipiiiii-1.0.0/template/python_openai.j2`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.8/template/template_openai.yaml` & `sipiiiii-1.0.0/template/template_openai.yaml`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.8.8/template/template_other.yaml` & `sipiiiii-1.0.0/template/template_fastapi.yaml`

 * *Files identical despite different names*

