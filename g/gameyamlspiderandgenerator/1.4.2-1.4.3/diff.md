# Comparing `tmp/gameyamlspiderandgenerator-1.4.2.tar.gz` & `tmp/gameyamlspiderandgenerator-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.4.2.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.4.3.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.4.2.tar` & `gameyamlspiderandgenerator-1.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.4.2/LICENSE
--rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.4.2/README.md
--rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-05-05 11:54:39.054374 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     3700 2023-05-05 11:54:39.054640 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      594 2023-05-05 11:54:39.054859 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2788 2023-05-05 11:54:39.055524 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7167 2023-05-05 12:09:58.807408 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7700 2023-05-05 12:22:56.868458 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1472 2023-05-05 12:19:16.287199 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 12:14:11.649300 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      700 2023-05-05 12:32:25.207351 gameyamlspiderandgenerator-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.4.3/LICENSE
+-rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.4.3/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      210 2023-05-05 14:42:52.343793 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     3694 2023-05-05 14:46:20.255955 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      582 2023-05-05 14:42:52.437426 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2606 2023-05-05 14:47:46.986045 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7167 2023-05-05 14:39:08.986302 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1472 2023-05-05 14:39:08.993151 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      700 2023-05-05 14:48:55.735977 gameyamlspiderandgenerator-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.3/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.4.2/LICENSE` & `gameyamlspiderandgenerator-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/README.md` & `gameyamlspiderandgenerator-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,26 +38,26 @@
             f'{config["api"]["google-play"]}&store=apps&q={self.encode}'
         )
         if "organic_results" in data and any(
                 [self.name_filter(i["title"]) == self.pure for i in data["organic_results"][0]["items"]]):
             logger.info("FOUND: google_play")
             return "google-play", {'name': '.play-store',
                                    'uri': f'google-play-store:{data["organic_results"][0]["items"][0]["product_id"]}'}
-        return ([], [])
+        return [], []
 
     def search_apple(self) -> tuple:
         data = get_json(
             "https://serpapi.com/search.json?engine=apple_app_store&term="
             f'{self.encode}&apikey={config["api"]["apple"]}'
         )
         if "organic_results" in data and any(
                 [self.name_filter(i["title"]) == self.pure for i in data["organic_results"]]):
             logger.info("FOUND: apple_app_store")
             return "apple-appstore", {'name': '.apple-appstore', 'uri': data["organic_results"][0]["link"]}
-        return ([], [])
+        return [], []
 
     def search_all(self) -> list:
         func_list = [
             self.__getattribute__(i)
             for i in (list(filter(lambda x: "__" not in x, self.__dir__())))
         ]
         func_list = filter(
@@ -73,15 +73,15 @@
         game_list = api['data']['Catalog']['searchStore']['elements']
         reg = r"[^A-z\d]"
         if game_list and any(
                 [self.name_filter(i["title"]) == self.pure for i in game_list]):
             logger.info("FOUND: epic")
             return "epic", {'name': '.epic',
                             'uri': f'https://store.epicgames.com/p/{self.name_filter(game_list[0]["title"], pattern=reg, repl="-")}'}
-        return [[], []]
+        return [], []
 
     def setup(self, data: dict):
         """
         hook handler
         Args:
             data: yaml daya
```

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from ..util.spider import get_text
 from jsonschema import validate
 from yaml import safe_load
 from loguru import logger
 
 
 class Verify(BaseHook):
-    @staticmethod
-    def setup(data: dict):
+    def setup(self, data: dict):
         try:
             validate(data, safe_load(get_text('https://raw.githubusercontent.com/FurryGamesIndex/games/master/schemas'
                                               '/game.schema.yaml')))
             logger.success("verification complete")
         except Exception as e:
             logger.error(e)
         return data
```

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 
         Args:
             data: 钩子数据
         """
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
         pkg.__init__()
         for i in pkg.hook.values():
-            return i(self.get_name()).setup(data)
-
-        from gameyamlspiderandgenerator.util.plugin_manager import pkg
-        pkg.__init__()
-        for i in pkg.hook.values():
             data = i(self.get_name()).setup(data)
         return data
 
     @abc.abstractmethod
     def get_name(self) -> str:
         """
         获取游戏名称
@@ -142,8 +137,7 @@
     def to_yaml(self) -> str:
         """
         转换为 YAML
 
         Returns:
             YAML
         """
-
```

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.2/pyproject.toml` & `gameyamlspiderandgenerator-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.4.2"
+version = "1.4.3"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.4.2/PKG-INFO` & `gameyamlspiderandgenerator-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.4.2
+Version: 1.4.3
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

