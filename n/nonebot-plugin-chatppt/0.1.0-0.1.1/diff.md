# Comparing `tmp/nonebot_plugin_chatppt-0.1.0.tar.gz` & `tmp/nonebot_plugin_chatppt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chatppt-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_chatppt-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_chatppt-0.1.0.tar` & `nonebot_plugin_chatppt-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1918 2023-04-24 03:11:52.361828 nonebot_plugin_chatppt-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2023-04-24 03:08:30.860464 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/.DS_Store
--rw-r--r--   0        0        0     3169 2023-04-24 02:42:56.609507 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/__init__.py
--rw-r--r--   0        0        0      329 2023-04-24 03:03:45.824081 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/config.py
--rw-r--r--   0        0        0     7974 2023-04-24 03:03:45.824190 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/core.py
--rw-r--r--   0        0        0      593 2023-04-24 03:12:06.800026 nonebot_plugin_chatppt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2789 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.1.0/setup.py
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1918 2023-04-24 03:11:52.361828 nonebot_plugin_chatppt-0.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-04-24 03:08:30.860464 nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/.DS_Store
+-rw-r--r--   0        0        0     3169 2023-04-24 02:42:56.609507 nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-24 03:03:45.824081 nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/config.py
+-rw-r--r--   0        0        0     7928 2023-05-05 08:42:20.933529 nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/core.py
+-rw-r--r--   0        0        0      593 2023-05-05 08:43:17.946694 nonebot_plugin_chatppt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2789 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.1.1/setup.py
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_chatppt-0.1.0/README.md` & `nonebot_plugin_chatppt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/.DS_Store` & `nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/.DS_Store`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/__init__.py` & `nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/core.py` & `nonebot_plugin_chatppt-0.1.1/nonebot_plugin_chatppt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,19 @@
     def get_filename(self, task, default_ext):
         filename = super(PrefixNameDownloader, self).get_filename(
             task, default_ext)
         print(bad_coding_practice)
         return 'prefix_' + bad_coding_practice + filename
 
 
-async def generate_ppt(topic, slide_length, user_id: str):
+async def generate_ppt(file_path, topic, slide_length, user_id: str):
     folder = Path() / "data" / "nonebot-plugin-chatppt" / "caches" / user_id
     folder.mkdir(parents=True, exist_ok=True)
 
-    root = Presentation("./data/nonebot-plugin-chatppt/theme.pptx")
-
-    print(str(folder))
+    root = Presentation(file_path)
 
     message = f"""
     Create content for a slideshow presentation.
     The content's topic is {topic}. 
     The slideshow is {slide_length} slides long. 
     The content is written in the Chinese.
```

### Comparing `nonebot_plugin_chatppt-0.1.0/pyproject.toml` & `nonebot_plugin_chatppt-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-chatppt"
-version = "0.1.0"
+version = "0.1.1"
 description = "A nonebot plugin for generating PPT slides from ChatGPT"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_chatppt-0.1.0/setup.py` & `nonebot_plugin_chatppt-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'openai>=0.27.1,<0.28.0',
  'python-pptx>=0.6.21,<0.7.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-chatppt',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A nonebot plugin for generating PPT slides from ChatGPT',
     'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-chatppt\n</div>\n\n## 介绍\n- 本插件基于OpenAI的API开发，在nonebot框架下实现一个AI生成指定主题PPT的文件并上传到群文件中。\n\n![](demo.png)\n## 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot-plugin-chatppt.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-chatppt"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-chatppt\n  ```\n\n## 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n```\nOPENAI_API_KEY = key\n```\n\n可选内容：\n```\nOPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 中国大陆/香港IP调用API请使用代理访问api,否则有几率会被封禁\nOPENAI_MODEL_NAME = "xxxxx"   # 使用的模型名称\nSLIDES_LIMIT = "xxxxx"   # 生成PPT页数的上限，不设置默认为10\n```\n\n\n## 使用方法\n- 配置PPT模版文件\n\n 在Bot目录下的data文件夹里面新建nonebot-plugin-chatppt/theme文件夹。把PPT主题模版文件放进里面，支持多文件。\n\n- 生成PPT命令\n```\nchatppt\n```\n- 删除当前用户缓存文件命令\n```\n删除缓存PPT\n```\n- 删除所有用户缓存文件命令\n```\n删除所有缓存PPT\n```\n\n## Todo\n\n- [x] 多模版支持\n- [ ] 优化生成内容\n- [ ] 完善插入图片功能\n\n## 核心代码\n\n核心代码来源于：[Python-PPTX-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_chatppt'] package_data = \ {'': ['*']} install_requires = \
 ['icrawler>=0.6.6,<0.7.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
 'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=0.27.1,<0.28.0', 'python-
 pptx>=0.6.21,<0.7.0'] setup_kwargs = { 'name': 'nonebot-plugin-chatppt',
-'version': '0.1.0', 'description': 'A nonebot plugin for generating PPT slides
+'version': '0.1.1', 'description': 'A nonebot plugin for generating PPT slides
 from ChatGPT', 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
                         \n\n# nonebot-plugin-chatppt\n
```

### Comparing `nonebot_plugin_chatppt-0.1.0/PKG-INFO` & `nonebot_plugin_chatppt-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatppt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A nonebot plugin for generating PPT slides from ChatGPT
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatppt Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-chatppt Version: 0.1.1 Summary: A
 nonebot plugin for generating PPT slides from ChatGPT License: MIT Author:
 Alpaca Author-email: alpaca@bupt.edu.cn Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: icrawler (>=0.6.6,<0.7.0) Requires-Dist: nonebot-adapter-onebot
```

