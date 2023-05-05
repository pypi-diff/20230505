# Comparing `tmp/nonebot_plugin_analysis_bilibili-2.4.9.tar.gz` & `tmp/nonebot_plugin_analysis_bilibili-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.4.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_analysis_bilibili-2.5.0.tar", max compression
```

## Comparing `nonebot_plugin_analysis_bilibili-2.4.9.tar` & `nonebot_plugin_analysis_bilibili-2.5.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     2011 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/README.md
--rw-r--r--   0        0        0     1503 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/__init__.py
--rw-r--r--   0        0        0    14823 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
--rw-r--r--   0        0        0      576 2023-02-09 18:26:30.646797 nonebot_plugin_analysis_bilibili-2.4.9/pyproject.toml
--rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.4.9/setup.py
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.4.9/PKG-INFO
+-rw-r--r--   0        0        0     2432 2023-05-05 08:33:46.692408 nonebot_plugin_analysis_bilibili-2.5.0/README.md
+-rw-r--r--   0        0        0     2937 2023-05-05 08:33:46.692408 nonebot_plugin_analysis_bilibili-2.5.0/nonebot_plugin_analysis_bilibili/__init__.py
+-rw-r--r--   0        0        0    14482 2023-05-05 08:33:46.692408 nonebot_plugin_analysis_bilibili-2.5.0/nonebot_plugin_analysis_bilibili/analysis_bilibili.py
+-rw-r--r--   0        0        0      603 2023-05-05 08:33:46.692408 nonebot_plugin_analysis_bilibili-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 nonebot_plugin_analysis_bilibili-2.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.9/README.md` & `nonebot_plugin_analysis_bilibili-2.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -27,38 +27,41 @@
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-analysis-bilibili.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
 ## 使用方式
 
-私聊或群聊发送 bilibili 的小程序/链接
+私聊或群聊发送 bilibili 的小程序/链接，所有适配器均可使用，目前某些特性仅在 onebot 适配器中能够使用，例如下面可选项的几个。
 
 ## 额外配置项(可选)
 
-在配置文件中加入
+在配置文件中加入(需要什么加什么)
 
 ```
 analysis_blacklist = [123456789] # 不解析里面填写的QQ号发的链接 List[int]
 analysis_group_blacklist = [123456789] # 不解析里面填写的QQ群号发的链接 List[int]
+analysis_desc_blacklist = [123456789] # 里面填写的群号，发送的解析内容不包含简介 List[int]
 analysis_display_image = true # 是否显示封面 true/false
 
 # 哪种类型需要显示封面，与上一项相冲突，上一项为true则全开 List[str]
 analysis_display_image_list = ["video", "bangumi", "live", "article", "dynamic"]
+
+analysis_trust_env = false # 是否使用环境变量或者当前系统正在使用中的代理设置 true/false
 ```
 
 ## 安装
 
-1. 使用 nb-cli 安装，不需要手动添加入口，更新使用 pip
+1. 使用 nb-cli 安装，不需要手动添加入口，更新使用 pip (推荐)
 
 ```
 nb plugin install nonebot_plugin_analysis_bilibili
 ```
 
-2. 使用 pip 安装和更新，初次安装需要手动添加入口
+2. 使用 pip 安装和更新，初次安装需要手动添加入口 （新版默认不带 bot.py 文件）
 
 ```
 pip install --upgrade nonebot_plugin_analysis_bilibili
 ```
 
 pip 安装后在 Nonebot2 入口文件（例如 bot.py ）增加：
```

#### html2text {}

```diff
@@ -1,19 +1,25 @@
                                    [nonebot]
            # nonebot_plugin_analysis_bilibili _â¨ NoneBot bilibili
                        è§é¢ãçªå§è§£ææä»¶ â¨_
                            [license] [pypi] [python]
-## ä½¿ç¨æ¹å¼ ç§èæç¾¤èåé bilibili çå°ç¨åº/é¾æ¥ ##
-é¢å¤éç½®é¡¹(å¯é) å¨éç½®æä»¶ä¸­å å¥ ``` analysis_blacklist =
-[123456789] # ä¸è§£æéé¢å¡«åçQQå·åçé¾æ¥ List[int]
+## ä½¿ç¨æ¹å¼ ç§èæç¾¤èåé bilibili çå°ç¨åº/
+é¾æ¥ï¼ææééå¨åå¯ä½¿ç¨ï¼ç®åæäºç¹æ§ä»å¨ onebot
+ééå¨ä¸­è½å¤ä½¿ç¨ï¼ä¾å¦ä¸é¢å¯éé¡¹çå ä¸ªã ## é¢å¤éç½®é¡¹
+(å¯é) å¨éç½®æä»¶ä¸­å å¥(éè¦ä»ä¹å ä»ä¹) ``` analysis_blacklist
+= [123456789] # ä¸è§£æéé¢å¡«åçQQå·åçé¾æ¥ List[int]
 analysis_group_blacklist = [123456789] #
-ä¸è§£æéé¢å¡«åçQQç¾¤å·åçé¾æ¥ List[int] analysis_display_image =
-true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
+ä¸è§£æéé¢å¡«åçQQç¾¤å·åçé¾æ¥ List[int] analysis_desc_blacklist
+= [123456789] # éé¢å¡«åçç¾¤å·ï¼åéçè§£æåå®¹ä¸åå«ç®ä»
+List[int] analysis_display_image = true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
 åªç§ç±»åéè¦æ¾ç¤ºå°é¢ï¼ä¸ä¸ä¸é¡¹ç¸å²çªï¼ä¸ä¸é¡¹ä¸ºtrueåå¨å¼
 List[str] analysis_display_image_list = ["video", "bangumi", "live", "article",
-"dynamic"] ``` ## å®è£ 1. ä½¿ç¨ nb-cli
-å®è£ï¼ä¸éè¦æå¨æ·»å å¥å£ï¼æ´æ°ä½¿ç¨ pip ``` nb plugin install
-nonebot_plugin_analysis_bilibili ``` 2. ä½¿ç¨ pip
-å®è£åæ´æ°ï¼åæ¬¡å®è£éè¦æå¨æ·»å å¥å£ ``` pip install --
-upgrade nonebot_plugin_analysis_bilibili ``` pip å®è£åå¨ Nonebot2
-å¥å£æä»¶ï¼ä¾å¦ bot.py ï¼å¢å ï¼ ```python nonebot.load_plugin
-("nonebot_plugin_analysis_bilibili") ``` éï¼æ¯æ a16 æåä¸çä¸º 2.4.3
+"dynamic"] analysis_trust_env = false #
+æ¯å¦ä½¿ç¨ç¯å¢åéæèå½åç³»ç»æ­£å¨ä½¿ç¨ä¸­çä»£çè®¾ç½® true/
+false ``` ## å®è£ 1. ä½¿ç¨ nb-cli
+å®è£ï¼ä¸éè¦æå¨æ·»å å¥å£ï¼æ´æ°ä½¿ç¨ pip (æ¨è) ``` nb plugin
+install nonebot_plugin_analysis_bilibili ``` 2. ä½¿ç¨ pip
+å®è£åæ´æ°ï¼åæ¬¡å®è£éè¦æå¨æ·»å å¥å£ ï¼æ°çé»è®¤ä¸å¸¦
+bot.py æä»¶ï¼ ``` pip install --upgrade nonebot_plugin_analysis_bilibili ```
+pip å®è£åå¨ Nonebot2 å¥å£æä»¶ï¼ä¾å¦ bot.py ï¼å¢å ï¼ ```python
+nonebot.load_plugin("nonebot_plugin_analysis_bilibili") ``` éï¼æ¯æ a16
+æåä¸çä¸º 2.4.3
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.9/nonebot_plugin_analysis_bilibili/analysis_bilibili.py` & `nonebot_plugin_analysis_bilibili-2.5.0/nonebot_plugin_analysis_bilibili/analysis_bilibili.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 import re
 import urllib.parse
 import json
-from time import localtime, strftime
-from typing import Dict, Optional, Tuple, Union
-
-import aiohttp
 import nonebot
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
+
+from time import localtime, strftime
+from typing import Dict, List, Optional, Tuple, Union
+from aiohttp import ClientSession
 
 # group_id : last_vurl
 analysis_stat: Dict[int, str] = {}
 
 config = nonebot.get_driver().config
 analysis_display_image = getattr(config, "analysis_display_image", False)
 analysis_display_image_list = getattr(config, "analysis_display_image_list", [])
 
 
-async def bili_keyword(group_id: Optional[int], text: str) -> Union[Message, str]:
+async def bili_keyword(
+    group_id: Optional[int], text: str, session: ClientSession
+) -> Union[List[Union[List[str], str]], str]:
     try:
         # 提取url
         url, page, time_location = extract(text)
         # 如果是小程序就去搜索标题
         if not url:
             if title := re.search(r'"desc":("[^"哔哩]+")', text):
-                vurl = await search_bili_by_title(title[1])
+                vurl = await search_bili_by_title(title[1], session)
                 if vurl:
                     url, page, time_location = extract(vurl)
 
         # 获取视频详细信息
         msg, vurl = "", ""
         if "view?" in url:
-            msg, vurl = await video_detail(url, page=page, time_location=time_location)
+            msg, vurl = await video_detail(
+                url, page=page, time_location=time_location, session=session
+            )
         elif "bangumi" in url:
-            msg, vurl = await bangumi_detail(url, time_location)
+            msg, vurl = await bangumi_detail(url, time_location, session)
         elif "xlive" in url:
-            msg, vurl = await live_detail(url)
+            msg, vurl = await live_detail(url, session)
         elif "article" in url:
-            msg, vurl = await article_detail(url, page)
+            msg, vurl = await article_detail(url, page, session)
         elif "dynamic" in url:
-            msg, vurl = await dynamic_detail(url)
+            msg, vurl = await dynamic_detail(url, session)
 
         # 避免多个机器人解析重复推送
         if group_id:
             if group_id in analysis_stat and analysis_stat[group_id] == vurl:
                 return ""
             analysis_stat[group_id] = vurl
     except Exception as e:
         msg = "bili_keyword Error: {}".format(type(e))
     return msg
 
 
-async def b23_extract(text: str) -> str:
+async def b23_extract(text: str, session: ClientSession) -> str:
     b23 = re.compile(r"b23.tv/(\w+)|(bili(22|23|33|2233).cn)/(\w+)", re.I).search(
         text.replace("\\", "")
     )
     url = f"https://{b23[0]}"
-    async with aiohttp.request(
-        "GET", url, timeout=aiohttp.client.ClientTimeout(10)
-    ) as resp:
+
+    async with session.get(url) as resp:
         return str(resp.url)
 
 
 def extract(text: str) -> Tuple[str, Optional[str], Optional[str]]:
     try:
         url = ""
         # 视频分p
@@ -112,20 +114,23 @@
         elif dynamic_id:
             url = f"https://api.vc.bilibili.com/dynamic_svr/v1/dynamic_svr/get_dynamic_detail?dynamic_id={dynamic_id[2]}"
         return url, page, time
     except Exception:
         return "", None, None
 
 
-async def search_bili_by_title(title: str) -> str:
+async def search_bili_by_title(title: str, session: ClientSession) -> str:
+    mainsite_url = "https://www.bilibili.com"
     search_url = f"https://api.bilibili.com/x/web-interface/wbi/search/all/v2?keyword={urllib.parse.quote(title)}"
 
-    async with aiohttp.request(
-        "GET", search_url, timeout=aiohttp.client.ClientTimeout(10)
-    ) as resp:
+    # set headers
+    async with session.get(mainsite_url) as resp:
+        assert resp.status == 200
+
+    async with session.get(search_url) as resp:
         result = (await resp.json())["data"]["result"]
 
     for i in result:
         if i.get("result_type") != "video":
             continue
         # 只返回第一个结果
         return i["data"][0].get("arcurl")
@@ -134,26 +139,26 @@
 # 处理超过一万的数字
 def handle_num(num: int) -> str:
     if num > 10000:
         num = f"{num / 10000:.2f}万"
     return num
 
 
-async def video_detail(url: str, **kwargs) -> Tuple[Union[Message, str], str]:
+async def video_detail(
+    url: str, session: ClientSession, **kwargs
+) -> Tuple[List[str], str]:
     try:
-        async with aiohttp.request(
-            "GET", url, timeout=aiohttp.client.ClientTimeout(10)
-        ) as resp:
+        async with session.get(url) as resp:
             res = (await resp.json()).get("data")
             if not res:
                 return "解析到视频被删了/稿件不可见或审核中/权限不足", url
         vurl = f"https://www.bilibili.com/video/av{res['aid']}"
         title = f"\n标题：{res['title']}\n"
         cover = (
-            MessageSegment.image(res["pic"])
+            res["pic"]
             if analysis_display_image or "video" in analysis_display_image_list
             else ""
         )
         if page := kwargs.get("page"):
             page = page[0].replace("&amp;", "&")
             p = int(page[3:])
             if p <= len(res["pages"]):
@@ -173,33 +178,31 @@
         stat += f"点赞：{handle_num(res['stat']['like'])} | 硬币：{handle_num(res['stat']['coin'])} | 评论：{handle_num(res['stat']['reply'])}\n"
         desc = f"简介：{res['desc']}"
         desc_list = desc.split("\n")
         desc = "".join(i + "\n" for i in desc_list if i)
         desc_list = desc.split("\n")
         if len(desc_list) > 4:
             desc = desc_list[0] + "\n" + desc_list[1] + "\n" + desc_list[2] + "……"
-        msg = Message([cover, vurl, title, tname, stat, desc])
+        msg = [cover, vurl, title, tname, stat, desc]
         return msg, vurl
     except Exception as e:
         msg = "视频解析出错--Error: {}".format(type(e))
         return msg, None
 
 
 async def bangumi_detail(
-    url: str, time_location: str = None
-) -> Tuple[Union[Message, str], str]:
+    url: str, time_location: str, session: ClientSession
+) -> Tuple[List[str], str]:
     try:
-        async with aiohttp.request(
-            "GET", url, timeout=aiohttp.client.ClientTimeout(10)
-        ) as resp:
+        async with session.get(url) as resp:
             res = (await resp.json()).get("result")
             if not res:
                 return None, None
         cover = (
-            MessageSegment.image(res["cover"])
+            res["cover"]
             if analysis_display_image or "bangumi" in analysis_display_image_list
             else ""
         )
         title = f"番剧：{res['title']}\n"
         desc = f"{res['newest_ep']['desc']}\n"
         index_title = ""
         style = "".join(f"{i}," for i in res["style"])
@@ -215,36 +218,34 @@
                 if str(i["ep_id"]) == epid:
                     index_title = f"标题：{i['index_title']}\n"
                     break
             vurl = f"https://www.bilibili.com/bangumi/play/ep{epid}"
         if time_location:
             time_location = time_location[0].replace("&amp;", "&")[3:]
             vurl += f"?t={time_location}"
-        msg = Message([cover, f"{vurl}\n", title, index_title, desc, style, evaluate])
+        msg = [cover, f"{vurl}\n", title, index_title, desc, style, evaluate]
         return msg, vurl
     except Exception as e:
         msg = "番剧解析出错--Error: {}".format(type(e))
         msg += f"\n{url}"
         return msg, None
 
 
-async def live_detail(url: str) -> Tuple[Union[Message, str], str]:
+async def live_detail(url: str, session: ClientSession) -> Tuple[List[str], str]:
     try:
-        async with aiohttp.request(
-            "GET", url, timeout=aiohttp.client.ClientTimeout(10)
-        ) as resp:
+        async with session.get(url) as resp:
             res = await resp.json()
             if res["code"] != 0:
                 return None, None
         res = res["data"]
         uname = res["anchor_info"]["base_info"]["uname"]
         room_id = res["room_info"]["room_id"]
         title = res["room_info"]["title"]
         cover = (
-            MessageSegment.image(res["room_info"]["cover"])
+            res["room_info"]["cover"]
             if analysis_display_image or "live" in analysis_display_image_list
             else ""
         )
         live_status = res["room_info"]["live_status"]
         lock_status = res["room_info"]["lock_status"]
         parent_area_name = res["room_info"]["parent_area_name"]
         area_name = res["room_info"]["area_name"]
@@ -266,88 +267,83 @@
         watch = f"观看：{watched_show}  直播时的人气上一次刷新值：{handle_num(online)}\n"
         if tags:
             tags = f"标签：{tags}\n"
         if live_status:
             player = f"独立播放器：https://www.bilibili.com/blackboard/live/live-activity-player.html?enterTheRoom=0&cid={room_id}"
         else:
             player = ""
-        msg = Message([cover, vurl, title, up, watch, tags, player])
+        msg = [cover, vurl, title, up, watch, tags, player]
         return msg, vurl
     except Exception as e:
         msg = "直播间解析出错--Error: {}".format(type(e))
         return msg, None
 
 
-async def article_detail(url: str, cvid: str) -> Tuple[Union[Message, str], str]:
+async def article_detail(
+    url: str, cvid: str, session: ClientSession
+) -> Tuple[List[Union[List[str], str]], str]:
     try:
-        async with aiohttp.request(
-            "GET", url, timeout=aiohttp.client.ClientTimeout(10)
-        ) as resp:
+        async with session.get(url) as resp:
             res = (await resp.json()).get("data")
             if not res:
                 return None, None
         images = (
-            [MessageSegment.image(i) for i in res["origin_image_urls"]]
+            res["origin_image_urls"]
             if analysis_display_image or "article" in analysis_display_image_list
             else []
         )
         vurl = f"https://www.bilibili.com/read/cv{cvid}"
         title = f"标题：{res['title']}\n"
         up = f"作者：{res['author_name']} (https://space.bilibili.com/{res['mid']})\n"
         view = f"阅读数：{handle_num(res['stats']['view'])} "
         favorite = f"收藏数：{handle_num(res['stats']['favorite'])} "
         coin = f"硬币数：{handle_num(res['stats']['coin'])}"
         share = f"分享数：{handle_num(res['stats']['share'])} "
         like = f"点赞数：{handle_num(res['stats']['like'])} "
         dislike = f"不喜欢数：{handle_num(res['stats']['dislike'])}"
         desc = view + favorite + coin + "\n" + share + like + dislike + "\n"
-        msg = Message(images)
-        msg.extend([title, up, desc, vurl])
+        msg = [images, title, up, desc, vurl]
         return msg, vurl
     except Exception as e:
         msg = "专栏解析出错--Error: {}".format(type(e))
         return msg, None
 
 
-async def dynamic_detail(url: str) -> Tuple[Union[Message, str], str]:
+async def dynamic_detail(
+    url: str, session: ClientSession
+) -> Tuple[List[Union[List[str], str]], str]:
     try:
-        async with aiohttp.request(
-            "GET", url, timeout=aiohttp.client.ClientTimeout(10)
-        ) as resp:
+        async with session.get(url) as resp:
             res = (await resp.json())["data"].get("card")
             if not res:
                 return None, None
         card = json.loads(res["card"])
         dynamic_id = res["desc"]["dynamic_id"]
         vurl = f"https://t.bilibili.com/{dynamic_id}\n"
         if not (item := card.get("item")):
             return "动态不存在文字内容", vurl
         if not (content := item.get("description")):
             content = item.get("content")
         content = content.replace("\r", "\n")
         if len(content) > 250:
             content = content[:250] + "......"
         images = (
-            item.get("pictures", [])
+            [i.get("img_src") for i in item.get("pictures", [])]
             if analysis_display_image or "dynamic" in analysis_display_image_list
             else []
         )
-        if images:
-            images = [MessageSegment.image(i.get("img_src")) for i in images]
-        else:
+        if not images:
             pics = item.get("pictures_count")
             if pics:
                 content += f"\nPS：动态中包含{pics}张图片"
         if origin := card.get("origin"):
             jorigin = json.loads(origin)
             short_link = jorigin.get("short_link")
             if short_link:
                 content += f"\n动态包含转发视频{short_link}"
             else:
                 content += f"\n动态包含转发其他动态"
-        msg = Message(content)
-        msg.extend(images)
-        msg.append(f"\n{vurl}")
+        msg = [images, content, f"\n动态链接：{vurl}"]
         return msg, vurl
     except Exception as e:
         msg = "动态解析出错--Error: {}".format(type(e))
         return msg, None
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.9/pyproject.toml` & `nonebot_plugin_analysis_bilibili-2.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-analysis-bilibili"
-version = "2.4.9"
+version = "2.5.0"
 description = "nonebot2解析bilibili插件"
 authors = ["mengshouer"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/mengshouer/nonebot_plugin_analysis_bilibili"
 keywords = ["nonebot", "nonebot2", "bilibili"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.7"
-nonebot2 = "^2.0.0-beta.5"
-nonebot-adapter-onebot = "^2.0.0-beta.1"
+nonebot2 = "^2.0.0rc4"
+nonebot-adapter-onebot = { version = "^2.0.0-beta.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_analysis_bilibili-2.4.9/setup.py` & `nonebot_plugin_analysis_bilibili-2.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-analysis-bilibili
+Version: 2.5.0
+Summary: nonebot2解析bilibili插件
+Home-page: https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
+License: MIT
+Keywords: nonebot,nonebot2,bilibili
+Author: mengshouer
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.7,<4.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Project-URL: Repository, https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
+Description-Content-Type: text/markdown
+
+<!--
+ * @Author         : mengshouer
+ * @Date           : 2021-03-16 00:00:00
+ * @LastEditors    : mengshouer
+ * @LastEditTime   : 2021-03-16 00:00:00
+ * @Description    : None
+ * @GitHub         : https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
+-->
+
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
+
+<div align="center">
+
+# nonebot_plugin_analysis_bilibili
+
+_✨ NoneBot bilibili 视频、番剧解析插件 ✨_
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">
+    <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-analysis-bilibili">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-analysis-bilibili.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</p>
+
+## 使用方式
+
+私聊或群聊发送 bilibili 的小程序/链接，所有适配器均可使用，目前某些特性仅在 onebot 适配器中能够使用，例如下面可选项的几个。
+
+## 额外配置项(可选)
+
+在配置文件中加入(需要什么加什么)
+
+```
+analysis_blacklist = [123456789] # 不解析里面填写的QQ号发的链接 List[int]
+analysis_group_blacklist = [123456789] # 不解析里面填写的QQ群号发的链接 List[int]
+analysis_desc_blacklist = [123456789] # 里面填写的群号，发送的解析内容不包含简介 List[int]
+analysis_display_image = true # 是否显示封面 true/false
+
+# 哪种类型需要显示封面，与上一项相冲突，上一项为true则全开 List[str]
+analysis_display_image_list = ["video", "bangumi", "live", "article", "dynamic"]
+
+analysis_trust_env = false # 是否使用环境变量或者当前系统正在使用中的代理设置 true/false
+```
+
+## 安装
+
+1. 使用 nb-cli 安装，不需要手动添加入口，更新使用 pip (推荐)
+
+```
+nb plugin install nonebot_plugin_analysis_bilibili
+```
+
+2. 使用 pip 安装和更新，初次安装需要手动添加入口 （新版默认不带 bot.py 文件）
+
+```
+pip install --upgrade nonebot_plugin_analysis_bilibili
+```
+
+pip 安装后在 Nonebot2 入口文件（例如 bot.py ）增加：
+
+```python
+nonebot.load_plugin("nonebot_plugin_analysis_bilibili")
+```
 
-packages = \
-['nonebot_plugin_analysis_bilibili']
+附：支持 a16 最后一版为 2.4.3
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.7,<4.0',
- 'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
- 'nonebot2>=2.0.0-beta.5,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-analysis-bilibili',
-    'version': '2.4.9',
-    'description': 'nonebot2解析bilibili插件',
-    'long_description': '<!--\n * @Author         : mengshouer\n * @Date           : 2021-03-16 00:00:00\n * @LastEditors    : mengshouer\n * @LastEditTime   : 2021-03-16 00:00:00\n * @Description    : None\n * @GitHub         : https://github.com/mengshouer/nonebot_plugin_analysis_bilibili\n-->\n\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot_plugin_analysis_bilibili\n\n_✨ NoneBot bilibili 视频、番剧解析插件 ✨_\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/cscs181/QQ-Github-Bot/master/LICENSE">\n    <img src="https://img.shields.io/github/license/cscs181/QQ-Github-Bot.svg" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-analysis-bilibili">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-analysis-bilibili.svg" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</p>\n\n## 使用方式\n\n私聊或群聊发送 bilibili 的小程序/链接\n\n## 额外配置项(可选)\n\n在配置文件中加入\n\n```\nanalysis_blacklist = [123456789] # 不解析里面填写的QQ号发的链接 List[int]\nanalysis_group_blacklist = [123456789] # 不解析里面填写的QQ群号发的链接 List[int]\nanalysis_display_image = true # 是否显示封面 true/false\n\n# 哪种类型需要显示封面，与上一项相冲突，上一项为true则全开 List[str]\nanalysis_display_image_list = ["video", "bangumi", "live", "article", "dynamic"]\n```\n\n## 安装\n\n1. 使用 nb-cli 安装，不需要手动添加入口，更新使用 pip\n\n```\nnb plugin install nonebot_plugin_analysis_bilibili\n```\n\n2. 使用 pip 安装和更新，初次安装需要手动添加入口\n\n```\npip install --upgrade nonebot_plugin_analysis_bilibili\n```\n\npip 安装后在 Nonebot2 入口文件（例如 bot.py ）增加：\n\n```python\nnonebot.load_plugin("nonebot_plugin_analysis_bilibili")\n```\n\n附：支持 a16 最后一版为 2.4.3\n',
-    'author': 'mengshouer',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mengshouer/nonebot_plugin_analysis_bilibili',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,32 +1,37 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_analysis_bilibili'] package_data = \ {'': ['*']}
-install_requires = \ ['aiohttp>=3.7,<4.0', 'nonebot-adapter-onebot>=2.0.0-
-beta.1,<3.0.0', 'nonebot2>=2.0.0-beta.5,<3.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-analysis-bilibili', 'version': '2.4.9', 'description':
-'nonebot2è§£æbilibiliæä»¶', 'long_description': '\n\n
-                                \n [nonebot]\n
-\n\n
-        \n\n# nonebot_plugin_analysis_bilibili\n\n_â¨ NoneBot bilibili
-                     è§é¢ãçªå§è§£ææä»¶ â¨_\n\n
-\n\n
-                 \n \n_[license]\n\n \n_[pypi]\n\n [python]\n
-\n\n## ä½¿ç¨æ¹å¼\n\nç§èæç¾¤èåé bilibili çå°ç¨åº/é¾æ¥\n\n##
-é¢å¤éç½®é¡¹(å¯é)\n\nå¨éç½®æä»¶ä¸­å å¥\n\n```\nanalysis_blacklist
-= [123456789] # ä¸è§£æéé¢å¡«åçQQå·åçé¾æ¥ List
-[int]\nanalysis_group_blacklist = [123456789] #
-ä¸è§£æéé¢å¡«åçQQç¾¤å·åçé¾æ¥ List[int]\nanalysis_display_image
-= true # æ¯å¦æ¾ç¤ºå°é¢ true/false\n\n#
+Metadata-Version: 2.1 Name: nonebot-plugin-analysis-bilibili Version: 2.5.0
+Summary: nonebot2è§£æbilibiliæä»¶ Home-page: https://github.com/mengshouer/
+nonebot_plugin_analysis_bilibili License: MIT Keywords:
+nonebot,nonebot2,bilibili Author: mengshouer Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.7,<4.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.0.0-beta.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Project-
+URL: Repository, https://github.com/mengshouer/nonebot_plugin_analysis_bilibili
+Description-Content-Type: text/markdown
+                                   [nonebot]
+           # nonebot_plugin_analysis_bilibili _â¨ NoneBot bilibili
+                       è§é¢ãçªå§è§£ææä»¶ â¨_
+                           [license] [pypi] [python]
+## ä½¿ç¨æ¹å¼ ç§èæç¾¤èåé bilibili çå°ç¨åº/
+é¾æ¥ï¼ææééå¨åå¯ä½¿ç¨ï¼ç®åæäºç¹æ§ä»å¨ onebot
+ééå¨ä¸­è½å¤ä½¿ç¨ï¼ä¾å¦ä¸é¢å¯éé¡¹çå ä¸ªã ## é¢å¤éç½®é¡¹
+(å¯é) å¨éç½®æä»¶ä¸­å å¥(éè¦ä»ä¹å ä»ä¹) ``` analysis_blacklist
+= [123456789] # ä¸è§£æéé¢å¡«åçQQå·åçé¾æ¥ List[int]
+analysis_group_blacklist = [123456789] #
+ä¸è§£æéé¢å¡«åçQQç¾¤å·åçé¾æ¥ List[int] analysis_desc_blacklist
+= [123456789] # éé¢å¡«åçç¾¤å·ï¼åéçè§£æåå®¹ä¸åå«ç®ä»
+List[int] analysis_display_image = true # æ¯å¦æ¾ç¤ºå°é¢ true/false #
 åªç§ç±»åéè¦æ¾ç¤ºå°é¢ï¼ä¸ä¸ä¸é¡¹ç¸å²çªï¼ä¸ä¸é¡¹ä¸ºtrueåå¨å¼
-List[str]\nanalysis_display_image_list = ["video", "bangumi", "live",
-"article", "dynamic"]\n```\n\n## å®è£\n\n1. ä½¿ç¨ nb-cli
-å®è£ï¼ä¸éè¦æå¨æ·»å å¥å£ï¼æ´æ°ä½¿ç¨ pip\n\n```\nnb plugin
-install nonebot_plugin_analysis_bilibili\n```\n\n2. ä½¿ç¨ pip
-å®è£åæ´æ°ï¼åæ¬¡å®è£éè¦æå¨æ·»å å¥å£\n\n```\npip install --
-upgrade nonebot_plugin_analysis_bilibili\n```\n\npip å®è£åå¨ Nonebot2
-å¥å£æä»¶ï¼ä¾å¦ bot.py ï¼å¢å ï¼\n\n```python\nnonebot.load_plugin
-("nonebot_plugin_analysis_bilibili")\n```\n\néï¼æ¯æ a16 æåä¸çä¸º
-2.4.3\n', 'author': 'mengshouer', 'author_email': 'None', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/mengshouer/
-nonebot_plugin_analysis_bilibili', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.8,<4.0', } setup(**setup_kwargs)
+List[str] analysis_display_image_list = ["video", "bangumi", "live", "article",
+"dynamic"] analysis_trust_env = false #
+æ¯å¦ä½¿ç¨ç¯å¢åéæèå½åç³»ç»æ­£å¨ä½¿ç¨ä¸­çä»£çè®¾ç½® true/
+false ``` ## å®è£ 1. ä½¿ç¨ nb-cli
+å®è£ï¼ä¸éè¦æå¨æ·»å å¥å£ï¼æ´æ°ä½¿ç¨ pip (æ¨è) ``` nb plugin
+install nonebot_plugin_analysis_bilibili ``` 2. ä½¿ç¨ pip
+å®è£åæ´æ°ï¼åæ¬¡å®è£éè¦æå¨æ·»å å¥å£ ï¼æ°çé»è®¤ä¸å¸¦
+bot.py æä»¶ï¼ ``` pip install --upgrade nonebot_plugin_analysis_bilibili ```
+pip å®è£åå¨ Nonebot2 å¥å£æä»¶ï¼ä¾å¦ bot.py ï¼å¢å ï¼ ```python
+nonebot.load_plugin("nonebot_plugin_analysis_bilibili") ``` éï¼æ¯æ a16
+æåä¸çä¸º 2.4.3
```

