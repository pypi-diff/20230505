# Comparing `tmp/gameyamlspiderandgenerator-1.4.1.tar.gz` & `tmp/gameyamlspiderandgenerator-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.4.1.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.4.2.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.4.1.tar` & `gameyamlspiderandgenerator-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0     1069 2023-04-20 06:26:01.842563 gameyamlspiderandgenerator-1.4.1/LICENSE
--rwxr-xr-x   0        0        0      809 2023-04-20 06:26:01.842841 gameyamlspiderandgenerator-1.4.1/README.md
--rwxr-xr-x   0        0        0      568 2023-05-04 06:30:54.477413 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1751 2023-05-04 06:30:54.478145 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-04-20 06:26:01.843909 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-04-20 06:26:01.844401 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-04-20 06:26:01.844722 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     3700 2023-05-04 06:54:55.150398 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      594 2023-05-04 06:30:54.480635 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-04-20 06:26:01.845620 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2788 2023-05-04 06:30:54.481787 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7159 2023-05-04 07:20:47.389833 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7709 2023-05-04 06:30:54.483703 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-04-20 06:26:01.847280 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-04 07:27:21.532018 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1459 2023-05-04 06:30:54.484835 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1892 2023-05-04 07:20:24.611440 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-05-04 03:20:05.673595 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-04-20 06:26:01.849061 gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      646 2023-05-04 07:30:57.763989 gameyamlspiderandgenerator-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.4.2/LICENSE
+-rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.4.2/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-05-05 11:54:39.054374 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     3700 2023-05-05 11:54:39.054640 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      594 2023-05-05 11:54:39.054859 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2788 2023-05-05 11:54:39.055524 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7167 2023-05-05 12:09:58.807408 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7700 2023-05-05 12:22:56.868458 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1472 2023-05-05 12:19:16.287199 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 12:14:11.649300 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      700 2023-05-05 12:32:25.207351 gameyamlspiderandgenerator-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.2/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.4.1/LICENSE` & `gameyamlspiderandgenerator-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/hook/validate.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def get_authors(self) -> list[dict]:
         temp = []
         if "Authors" in self.more_info:
             temp = self.more_info["Authors"]
         elif "Author" in self.more_info:
             temp = self.more_info["Author"]
-        return [{"name": i, "role": ["producer"]} for i in temp]
+        return [{"name": i.strip(), "role": ["producer"]} for i in temp]
 
     def get_tags(self) -> list[str]:
         temp = self.more_info["Genre"] if "Genre" in self.more_info else []
         temp1 = self.more_info["Made with"] if "Made with" in self.more_info else []
         temp2 = self.more_info["Tags"]
         return [i.strip() for i in (temp2 + temp1 + temp)]
```

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,22 @@
     def get_brief_desc(self):
         return pss_dedent(
             html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
         )
 
     def get_authors(self) -> list[dict]:
         temp = self.data[str(self.id)]["data"]
-        developers = [{"name": i, "role": ["producer"]} for i in temp["developers"]]
-        publishers = [{"name": i, "role": ["publisher"]} for i in temp["publishers"]]
+        developers = [{"name": i.strip(), "role": ["producer"]} for i in temp["developers"]]
+        publishers = [{"name": i.strip(), "role": ["publisher"]} for i in temp["publishers"]]
         return developers + publishers
 
     def get_platforms(self):
         temp = self.data[str(self.id)]["data"]["platforms"]
         repl = {"windows": "windows", "mac": "macos", "linux": "linux"}
-        return [repl[i] for i in temp if i]
+        return [repl[i] for i in temp if temp[i]]
 
     def get_type_tag(self):
         repl = {
             "Adventure": "adventure",
             "Action": "action",
             "Visual Novel": "visual-novel",
             "Strategy": "strategy",
@@ -183,15 +183,15 @@
 
     def get_links(self) -> list[dict]:
         def remove_query_string(x: str):
             return parse_qs(urlparse(x).query)["url"][0] if "linkfilter" in x else x  # type: ignore
 
         temp1 = self.soup.body.find(
             "div",
-            attrs={"id": "game_area_description", "class": "game_area_description"},
+            attrs={"class": "game_area_description"},
         )
         temp3 = self.soup.body.find("div", attrs={"style": "padding-top: 14px;"})
         temp2 = temp3.find_all("a")
         temp4 = [
             remove_query_string(i["data-tooltip-text"])
             for i in temp2
             if "data-tooltip-text" in i.attrs
```

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 fgi_dict = [
     {
-        "match": "^https://www.youtube.com/(?!watch\?v=)(@?.+)",
+        "match": "^https://www.youtube.com/(?!watch\?v=)(?!channel/)(@?.+)",
         "prefix": ".youtube",
         "replace": "youtube:@\\g<1>",
     },
     {
-        "match": "^https://www.youtube.com/channel/(.+[^/])",
+        "match": "^https://www.youtube.com/channel/(.+[^/])/",
         "prefix": ".youtube",
         "replace": "youtube:\\g<1>",
     },
     {
         "match": "^https://twitter.com/(.{1,})",
         "prefix": ".twitter",
         "replace": "twitter:\\g<1>",
```

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 fgi.width = 4096
 
 
 def dump_to_yaml(data: dict) -> str:
     temp = fgi.dump_to_string(data)
     for i in list(data.keys())[1:]:
         temp = temp.replace("\n" + i, "\n\n" + i)
+    temp = temp.replace("description: |-", "description: |")
     return temp
 
 
 def process_thumbnail(img_byte: bytes):
     img = Image.open(BytesIO(img_byte))
     if img.size == (460, 215):
         img_resize = img.resize((360, 168))
```

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.4.2/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.1/PKG-INFO` & `gameyamlspiderandgenerator-1.4.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.4.1
-Summary: 
+Version: 1.4.2
+Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -22,39 +22,52 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: ruamel.yaml.string (>=0.1.0,<0.2.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Description-Content-Type: text/markdown
 
-# Start
-
+# Quick Start
+## Install
 ```commandline
 pip install gameyamlspiderandgenerator -i https://pypi.org/simple
 python3.10
 ```
-
-```python
-from gameyamlspiderandgenerator import produce_yaml
-from gameyamlspiderandgenerator.util.config import config
-from gameyamlspiderandgenerator.util.plugin_manager import pkg
-
-config.load("/home/user/desktop/config.yaml")
-pkg.__init__()
-print(produce_yaml("https://store.steampowered.com/app/1470120/Atopes/"))
-```
-config.yaml:
+## Create a new configuration file
+- config.yaml
 ```yaml
 plugin:
   - steam
   - itchio
 hook:
   - search
+  - validate
 # if you don't want to set proxy, please fill in {}
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
 proxy: { }
 gitToken: 'your token'
 api:
   google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
+
 ```
+## Try to make yaml data file
+```bash
+ python3.10 -m gameyamlspiderandgenerator -f /home/user/desktop/config.yaml  https://store.steampowered.com/app/290340/Armello/ -o 1.zip
+ # or omit some options
+ python3.10 -m gameyamlspiderandgenerator https://store.steampowered.com/app/290340/Armello/
+
+```
+*or use the library in your script*
+```python
+from gameyamlspiderandgenerator import produce_yaml
+from gameyamlspiderandgenerator.util.config import config
+from gameyamlspiderandgenerator.util.plugin_manager import pkg
+
+config.load("/home/user/desktop/config.yaml")
+pkg.__init__()
+print(produce_yaml("https://store.steampowered.com/app/1470120/Atopes/"))
+```
+
+### More: see [API Reference](https://github.com/FurryGamesIndex/GameYamlSpiderAndGenerator/wiki/Api-Reference)
+
```

