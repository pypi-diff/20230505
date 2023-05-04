# Comparing `tmp/haruka-bot-1.5.3a3.tar.gz` & `tmp/haruka-bot-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka-bot-1.5.3a3.tar", last modified: Mon Feb  6 00:04:56 2023, max compression
+gzip compressed data, was "haruka-bot-1.5.4.tar", last modified: Thu May  4 22:55:35 2023, max compression
```

## Comparing `haruka-bot-1.5.3a3.tar` & `haruka-bot-1.5.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-rw-rw-   0        0        0      397 2023-02-04 07:19:56.998350 haruka-bot-1.5.3a3/haruka_bot/__init__.py
--rw-rw-rw-   0        0        0       61 2022-11-22 23:51:45.819393 haruka-bot-1.5.3a3/haruka_bot/__main__.py
--rw-rw-rw-   0        0        0      189 2022-11-22 23:51:45.823393 haruka-bot-1.5.3a3/haruka_bot/cli/__init__.py
--rw-rw-rw-   0        0        0      734 2022-11-22 23:51:45.827394 haruka-bot-1.5.3a3/haruka_bot/cli/bot.py
--rw-rw-rw-   0        0        0     1169 2022-11-22 23:51:45.829393 haruka-bot-1.5.3a3/haruka_bot/cli/utils.py
--rw-rw-rw-   0        0        0     1235 2023-02-05 22:31:31.403938 haruka-bot-1.5.3a3/haruka_bot/config.py
--rw-rw-rw-   0        0        0       49 2022-11-26 12:34:38.721371 haruka-bot-1.5.3a3/haruka_bot/database/__init__.py
--rw-rw-rw-   0        0        0    10005 2023-01-15 04:57:02.989711 haruka-bot-1.5.3a3/haruka_bot/database/db.py
--rw-rw-rw-   0        0        0     1936 2022-11-27 04:46:03.991442 haruka-bot-1.5.3a3/haruka_bot/database/models.py
--rw-rw-rw-   0        0        0       30 2022-11-22 23:51:45.847394 haruka-bot-1.5.3a3/haruka_bot/libs/__init__.py
--rw-rw-rw-   0        0        0     1464 2022-11-22 23:51:45.854393 haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/__init__.py
--rw-rw-rw-   0        0        0     1084 2022-11-22 23:51:45.859394 haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/card.py
--rw-rw-rw-   0        0        0      597 2022-11-22 23:51:45.863395 haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/desc.py
--rw-rw-rw-   0        0        0     1023 2022-11-22 23:51:45.866393 haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/display.py
--rw-rw-rw-   0        0        0      810 2022-11-22 23:51:45.870393 haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/user_profile.py
--rw-rw-rw-   0        0        0      456 2023-02-04 10:05:24.795329 haruka-bot-1.5.3a3/haruka_bot/plugins/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-04 10:06:14.581915 haruka-bot-1.5.3a3/haruka_bot/plugins/at/__init__.py
--rw-rw-rw-   0        0        0     1458 2023-02-05 22:30:14.335873 haruka-bot-1.5.3a3/haruka_bot/plugins/at/at_off.py
--rw-rw-rw-   0        0        0     1449 2023-02-05 22:30:14.335873 haruka-bot-1.5.3a3/haruka_bot/plugins/at/at_on.py
--rw-rw-rw-   0        0        0      678 2022-11-22 23:51:45.892393 haruka-bot-1.5.3a3/haruka_bot/plugins/auto_agree.py
--rw-rw-rw-   0        0        0      875 2022-11-27 04:46:04.049517 haruka-bot-1.5.3a3/haruka_bot/plugins/auto_delete.py
--rw-rw-rw-   0        0        0        0 2023-02-04 10:06:09.437473 haruka-bot-1.5.3a3/haruka_bot/plugins/dynamic/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-02-05 22:30:14.335873 haruka-bot-1.5.3a3/haruka_bot/plugins/dynamic/dynamic_off.py
--rw-rw-rw-   0        0        0     1076 2023-02-05 22:30:14.335873 haruka-bot-1.5.3a3/haruka_bot/plugins/dynamic/dynamic_on.py
--rw-rw-rw-   0        0        0      734 2023-02-05 22:30:33.858400 haruka-bot-1.5.3a3/haruka_bot/plugins/help.py
--rw-rw-rw-   0        0        0        0 2023-02-04 10:06:03.362155 haruka-bot-1.5.3a3/haruka_bot/plugins/live/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-02-05 22:30:14.316813 haruka-bot-1.5.3a3/haruka_bot/plugins/live/live_off.py
--rw-rw-rw-   0        0        0     1049 2023-02-05 22:30:14.316813 haruka-bot-1.5.3a3/haruka_bot/plugins/live/live_on.py
--rw-rw-rw-   0        0        0        0 2023-02-04 10:05:49.834436 haruka-bot-1.5.3a3/haruka_bot/plugins/permission/__init__.py
--rw-rw-rw-   0        0        0     1180 2023-02-05 22:30:13.709602 haruka-bot-1.5.3a3/haruka_bot/plugins/permission/permission_off.py
--rw-rw-rw-   0        0        0     1201 2023-02-05 22:30:13.706601 haruka-bot-1.5.3a3/haruka_bot/plugins/permission/permission_on.py
--rw-rw-rw-   0        0        0       58 2023-02-04 10:02:46.749451 haruka-bot-1.5.3a3/haruka_bot/plugins/pusher/__init__.py
--rw-rw-rw-   0        0        0     4406 2023-01-15 19:33:56.931057 haruka-bot-1.5.3a3/haruka_bot/plugins/pusher/dynamic_pusher.py
--rw-rw-rw-   0        0        0     2269 2023-02-04 10:08:03.399183 haruka-bot-1.5.3a3/haruka_bot/plugins/pusher/live_pusher.py
--rw-rw-rw-   0        0        0        0 2023-02-04 10:05:35.423776 haruka-bot-1.5.3a3/haruka_bot/plugins/sub/__init__.py
--rw-rw-rw-   0        0        0     2049 2023-02-05 23:01:49.907389 haruka-bot-1.5.3a3/haruka_bot/plugins/sub/add_sub.py
--rw-rw-rw-   0        0        0     1021 2023-02-05 22:30:13.706601 haruka-bot-1.5.3a3/haruka_bot/plugins/sub/delete_sub.py
--rw-rw-rw-   0        0        0     1567 2023-02-05 23:20:49.934158 haruka-bot-1.5.3a3/haruka_bot/plugins/sub/sub_list.py
--rw-rw-rw-   0        0        0     8365 2023-02-05 23:52:37.662279 haruka-bot-1.5.3a3/haruka_bot/utils/__init__.py
--rw-rw-rw-   0        0        0     7017 2023-02-06 00:00:49.134537 haruka-bot-1.5.3a3/haruka_bot/utils/browser.py
--rw-rw-rw-   0        0        0      730 2023-01-15 05:04:28.094272 haruka-bot-1.5.3a3/haruka_bot/utils/fonts_provider.py
--rw-rw-rw-   0        0        0     7512 2023-01-15 19:24:18.170204 haruka-bot-1.5.3a3/haruka_bot/utils/mobile.js
--rw-rw-rw-   0        0        0      146 2022-11-22 23:51:45.983394 haruka-bot-1.5.3a3/haruka_bot/version.py
--rw-rw-rw-   0        0        0    34522 2022-11-22 23:51:45.311395 haruka-bot-1.5.3a3/LICENSE
--rw-rw-rw-   0        0        0     1405 2023-02-06 00:02:30.067329 haruka-bot-1.5.3a3/pyproject.toml
--rw-rw-rw-   0        0        0     2763 2022-11-27 04:46:03.922919 haruka-bot-1.5.3a3/README.md
--rw-rw-rw-   0        0        0     3314 2023-02-06 00:04:56.719162 haruka-bot-1.5.3a3/PKG-INFO
+-rw-r--r--   0        0        0      263 2023-05-01 05:18:50.706789 haruka-bot-1.5.4/haruka_bot/__init__.py
+-rw-r--r--   0        0        0       61 2022-11-22 23:51:45.819393 haruka-bot-1.5.4/haruka_bot/__main__.py
+-rw-r--r--   0        0        0      189 2022-11-22 23:51:45.823393 haruka-bot-1.5.4/haruka_bot/cli/__init__.py
+-rw-r--r--   0        0        0      734 2022-11-22 23:51:45.827394 haruka-bot-1.5.4/haruka_bot/cli/bot.py
+-rw-r--r--   0        0        0     1169 2022-11-22 23:51:45.829393 haruka-bot-1.5.4/haruka_bot/cli/utils.py
+-rw-r--r--   0        0        0     1363 2023-05-04 21:46:30.610407 haruka-bot-1.5.4/haruka_bot/config.py
+-rw-r--r--   0        0        0       49 2022-11-26 12:34:38.721371 haruka-bot-1.5.4/haruka_bot/database/__init__.py
+-rw-r--r--   0        0        0    10476 2023-05-04 21:32:01.721909 haruka-bot-1.5.4/haruka_bot/database/db.py
+-rw-r--r--   0        0        0     2017 2023-02-13 19:22:21.855406 haruka-bot-1.5.4/haruka_bot/database/models.py
+-rw-r--r--   0        0        0       30 2022-11-22 23:51:45.847394 haruka-bot-1.5.4/haruka_bot/libs/__init__.py
+-rw-r--r--   0        0        0     1464 2022-11-22 23:51:45.854393 haruka-bot-1.5.4/haruka_bot/libs/dynamic/__init__.py
+-rw-r--r--   0        0        0     1084 2022-11-22 23:51:45.859394 haruka-bot-1.5.4/haruka_bot/libs/dynamic/card.py
+-rw-r--r--   0        0        0      597 2022-11-22 23:51:45.863395 haruka-bot-1.5.4/haruka_bot/libs/dynamic/desc.py
+-rw-r--r--   0        0        0     1023 2022-11-22 23:51:45.866393 haruka-bot-1.5.4/haruka_bot/libs/dynamic/display.py
+-rw-r--r--   0        0        0      810 2022-11-22 23:51:45.870393 haruka-bot-1.5.4/haruka_bot/libs/dynamic/user_profile.py
+-rw-r--r--   0        0        0      465 2023-05-01 05:18:50.709789 haruka-bot-1.5.4/haruka_bot/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:18:50.709789 haruka-bot-1.5.4/haruka_bot/plugins/at/__init__.py
+-rw-r--r--   0        0        0     1478 2023-05-01 05:18:50.710789 haruka-bot-1.5.4/haruka_bot/plugins/at/at_off.py
+-rw-r--r--   0        0        0     1469 2023-05-01 05:18:50.711789 haruka-bot-1.5.4/haruka_bot/plugins/at/at_on.py
+-rw-r--r--   0        0        0      678 2022-11-22 23:51:45.892393 haruka-bot-1.5.4/haruka_bot/plugins/auto_agree.py
+-rw-r--r--   0        0        0      897 2023-02-13 19:22:21.859410 haruka-bot-1.5.4/haruka_bot/plugins/auto_delete.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:18:50.711789 haruka-bot-1.5.4/haruka_bot/plugins/dynamic/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-01 05:18:50.712789 haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_off.py
+-rw-r--r--   0        0        0     1076 2023-05-01 05:18:50.712789 haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_on.py
+-rw-r--r--   0        0        0      755 2023-05-01 05:18:50.713791 haruka-bot-1.5.4/haruka_bot/plugins/help.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:18:50.713791 haruka-bot-1.5.4/haruka_bot/plugins/live/__init__.py
+-rw-r--r--   0        0        0     1058 2023-05-01 05:18:50.714789 haruka-bot-1.5.4/haruka_bot/plugins/live/live_off.py
+-rw-r--r--   0        0        0     1049 2023-05-01 05:18:50.715792 haruka-bot-1.5.4/haruka_bot/plugins/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:18:50.715792 haruka-bot-1.5.4/haruka_bot/plugins/permission/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-01 05:18:50.716789 haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_off.py
+-rw-r--r--   0        0        0     1232 2023-05-01 05:18:50.717790 haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_on.py
+-rw-r--r--   0        0        0       59 2023-05-01 05:18:50.717790 haruka-bot-1.5.4/haruka_bot/plugins/pusher/__init__.py
+-rw-r--r--   0        0        0     4847 2023-05-04 22:04:19.503423 haruka-bot-1.5.4/haruka_bot/plugins/pusher/dynamic_pusher.py
+-rw-r--r--   0        0        0     2360 2023-05-01 05:18:50.719789 haruka-bot-1.5.4/haruka_bot/plugins/pusher/live_pusher.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:18:50.719789 haruka-bot-1.5.4/haruka_bot/plugins/sub/__init__.py
+-rw-r--r--   0        0        0     2113 2023-05-01 05:18:50.720789 haruka-bot-1.5.4/haruka_bot/plugins/sub/add_sub.py
+-rw-r--r--   0        0        0     1058 2023-05-01 05:18:50.721790 haruka-bot-1.5.4/haruka_bot/plugins/sub/delete_sub.py
+-rw-r--r--   0        0        0     1594 2023-05-01 05:18:50.721790 haruka-bot-1.5.4/haruka_bot/plugins/sub/sub_list.py
+-rw-r--r--   0        0        0     8441 2023-05-01 05:18:50.722790 haruka-bot-1.5.4/haruka_bot/utils/__init__.py
+-rw-r--r--   0        0        0     6952 2023-05-01 05:18:50.723790 haruka-bot-1.5.4/haruka_bot/utils/browser.py
+-rw-r--r--   0        0        0      730 2023-05-01 05:18:50.723790 haruka-bot-1.5.4/haruka_bot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     7512 2023-05-01 05:18:50.724790 haruka-bot-1.5.4/haruka_bot/utils/mobile.js
+-rw-r--r--   0        0        0       96 2023-05-04 22:55:27.792965 haruka-bot-1.5.4/haruka_bot/version.py
+-rw-r--r--   0        0        0    34522 2022-11-22 23:51:45.311395 haruka-bot-1.5.4/LICENSE
+-rw-r--r--   0        0        0     1560 2023-05-04 22:20:40.010725 haruka-bot-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2837 2023-05-01 05:18:50.695791 haruka-bot-1.5.4/README.md
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 haruka-bot-1.5.4/PKG-INFO
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/cli/bot.py` & `haruka-bot-1.5.4/haruka_bot/cli/bot.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/cli/utils.py` & `haruka-bot-1.5.4/haruka_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/config.py` & `haruka-bot-1.5.4/haruka_bot/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List, Optional
 
+from nonebot import get_driver
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
 
 
 # 其他地方出现的类似 from .. import config，均是从 __init__.py 导入的 Config 实例
 class Config(BaseSettings):
     fastapi_reload: bool = False
@@ -12,23 +13,27 @@
     haruka_live_off_notify: bool = False
     haruka_proxy: Optional[str] = None
     haruka_interval: int = 10
     haruka_live_interval: int = haruka_interval
     haruka_dynamic_interval: int = 0
     haruka_dynamic_at: bool = False
     haruka_screenshot_style: str = "mobile"
-    haruka_dynamic_timeout: int = 10
+    haruka_dynamic_timeout: int = 30
     haruka_dynamic_font_source: str = "system"
     haruka_dynamic_font: Optional[str] = "Noto Sans CJK SC"
     haruka_command_prefix: str = ""
     # 频道管理员身份组
-    haruka_guild_admin_roles: List[str] = ["频道主", "管理员"]
+    haruka_guild_admin_roles: List[str] = ["频道主", "超级管理员"]
 
     @validator("haruka_interval", "haruka_live_interval", "haruka_dynamic_interval")
     def non_negative(cls, v: int, field: ModelField):
         """定时器为负返回默认值"""
         if v < 1:
             return field.default
         return v
 
     class Config:
         extra = "ignore"
+
+
+global_config = get_driver().config
+plugin_config = Config.parse_obj(global_config)
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/database/db.py` & `haruka-bot-1.5.4/haruka_bot/database/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,25 +18,41 @@
 
 class DB:
     """数据库交互类，与增删改查无关的部分不应该在这里面实现"""
 
     @classmethod
     async def init(cls):
         """初始化数据库"""
-        from . import models  # noqa: F401
+        config = {
+            "connections": {
+                # "haruka_bot": {
+                #     "engine": "tortoise.backends.sqlite",
+                #     "credentials": {"file_path": get_path("data.sqlite3")},
+                # },
+                "haruka_bot": f"sqlite://{get_path('data.sqlite3')}"
+            },
+            "apps": {
+                "haruka_bot_app": {
+                    "models": ["haruka_bot.database.models"],
+                    "default_connection": "haruka_bot",
+                }
+            },
+        }
+
+        await Tortoise.init(config)
 
-        await Tortoise.init(
-            db_url=f"sqlite://{get_path('data.sqlite3')}",
-            modules={"models": [locals()["models"]]},
-        )
         await Tortoise.generate_schemas()
         await cls.migrate()
         await cls.update_uid_list()
 
     @classmethod
+    async def close(cls):
+        await connections.close_all()
+
+    @classmethod
     async def get_user(cls, **kwargs):
         """获取 UP 主信息"""
         return await User.get(**kwargs).first()
 
     @classmethod
     async def get_name(cls, uid) -> Optional[str]:
         """获取 UP 主昵称"""
@@ -298,8 +314,8 @@
     @classmethod
     async def update_login(cls, tokens):
         """更新登录信息"""
         pass
 
 
 get_driver().on_startup(DB.init)
-get_driver().on_shutdown(connections.close_all)
+get_driver().on_shutdown(DB.close)
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/__init__.py` & `haruka-bot-1.5.4/haruka_bot/libs/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/card.py` & `haruka-bot-1.5.4/haruka_bot/libs/dynamic/card.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/desc.py` & `haruka-bot-1.5.4/haruka_bot/libs/dynamic/desc.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/display.py` & `haruka-bot-1.5.4/haruka_bot/libs/dynamic/display.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/libs/dynamic/user_profile.py` & `haruka-bot-1.5.4/haruka_bot/libs/dynamic/user_profile.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/at/at_off.py` & `haruka-bot-1.5.4/haruka_bot/plugins/at/at_off.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.params import ArgPlainText
 from nonebot.permission import SUPERUSER
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
-from ... import config
+from ...config import plugin_config
 from ...database import DB as db
 from ...utils import (
     GUILD_ADMIN,
     get_type_id,
     group_only,
     handle_uid,
     on_command,
@@ -39,10 +39,10 @@
     if await db.set_sub(
         "at", False, uid=uid, type=event.message_type, type_id=await get_type_id(event)
     ):
         user = await db.get_user(uid=uid)
         assert user is not None
         await at_off.finish(
             f"已关闭 {user.name}（{user.uid}）"
-            f"{'直播推送' if not config.haruka_dynamic_at else ''}的@全体"
+            f"{'直播推送' if not plugin_config.haruka_dynamic_at else ''}的@全体"
         )
     await at_off.finish(f"UID（{uid}）未关注，请先关注后再操作")
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/at/at_on.py` & `haruka-bot-1.5.4/haruka_bot/plugins/at/at_on.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.params import ArgPlainText
 from nonebot.permission import SUPERUSER
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
-from ... import config
+from ...config import plugin_config
 from ...database import DB as db
 from ...utils import (
     GUILD_ADMIN,
     get_type_id,
     group_only,
     handle_uid,
     on_command,
@@ -39,10 +39,10 @@
     if await db.set_sub(
         "at", True, uid=uid, type=event.message_type, type_id=await get_type_id(event)
     ):
         user = await db.get_user(uid=uid)
         assert user is not None
         await at_on.finish(
             f"已开启 {user.name}（{user.uid}）"
-            f"{'直播推送' if not config.haruka_dynamic_at else ''}的@全体"
+            f"{'直播推送' if not plugin_config.haruka_dynamic_at else ''}的@全体"
         )
     await at_on.finish(f"UID（{uid}）未关注，请先关注后再操作")
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/auto_agree.py` & `haruka-bot-1.5.4/haruka_bot/plugins/auto_agree.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/auto_delete.py` & `haruka-bot-1.5.4/haruka_bot/plugins/auto_delete.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Union
-
-from nonebot import on_notice
-from nonebot.adapters.onebot.v11 import GroupDecreaseNoticeEvent
-from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent
-
-from ..database import DB as db
-from ..utils import get_type_id
-
-group_decrease = on_notice(priority=5)
-
-
-@group_decrease.handle()
-async def _(event: Union[GroupDecreaseNoticeEvent, ChannelDestroyedNoticeEvent]):
-    """退群时，自动删除该群订阅列表"""
-    if isinstance(event, GroupDecreaseNoticeEvent):
-        if event.self_id == event.user_id:
-            await db.delete_sub_list(type="group", type_id=event.group_id)
-            await db.delete_group(id=event.group_id)
-    elif isinstance(event, ChannelDestroyedNoticeEvent):
-        await db.delete_sub_list(type="guild", type_id=await get_type_id(event))
-        await db.delete_guild(id=await get_type_id(event))
+from typing import Union
+
+from nonebot import on_notice
+from nonebot.adapters.onebot.v11 import GroupDecreaseNoticeEvent
+from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent
+
+from ..database import DB as db
+from ..utils import get_type_id
+
+group_decrease = on_notice(priority=5)
+
+
+@group_decrease.handle()
+async def _(event: Union[GroupDecreaseNoticeEvent, ChannelDestroyedNoticeEvent]):
+    """退群时，自动删除该群订阅列表"""
+    if isinstance(event, GroupDecreaseNoticeEvent):
+        if event.self_id == event.user_id:
+            await db.delete_sub_list(type="group", type_id=event.group_id)
+            await db.delete_group(id=event.group_id)
+    elif isinstance(event, ChannelDestroyedNoticeEvent):
+        await db.delete_sub_list(type="guild", type_id=await get_type_id(event))
+        await db.delete_guild(id=await get_type_id(event))
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/dynamic/dynamic_off.py` & `haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/dynamic/dynamic_on.py` & `haruka-bot-1.5.4/haruka_bot/plugins/dynamic/dynamic_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/live/live_off.py` & `haruka-bot-1.5.4/haruka_bot/plugins/live/live_off.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/live/live_on.py` & `haruka-bot-1.5.4/haruka_bot/plugins/live/live_on.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/permission/permission_off.py` & `haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_off.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Union
-
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
-from nonebot.permission import SUPERUSER
-from nonebot_plugin_guild_patch import GuildMessageEvent
-
-from ...database import DB as db
-from ...utils import GUILD_ADMIN, group_only, on_command, to_me
-
-permission_off = on_command(
-    "关闭权限",
-    rule=to_me(),
-    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
-    priority=5,
-)
-permission_off.__doc__ = """关闭权限"""
-
-permission_off.handle()(group_only)
-
-
-@permission_off.handle()
-async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
-    """关闭当前群权限"""
-    if isinstance(event, GuildMessageEvent):
-        if await db.set_guild_permission(event.guild_id, event.channel_id, False):
-            await permission_off.finish("已开启权限，只有管理员和主人可以操作")
-    else:
-        if await db.set_permission(event.group_id, False):
-            await permission_off.finish("已关闭权限，所有人均可操作")
-    await permission_off.finish("权限已经关闭了，所有人均可操作")
+from typing import Union
+
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
+from nonebot.permission import SUPERUSER
+from nonebot_plugin_guild_patch import GuildMessageEvent
+
+from ...database import DB as db
+from ...utils import GUILD_ADMIN, group_only, on_command, to_me
+
+permission_off = on_command(
+    "关闭权限",
+    rule=to_me(),
+    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
+    priority=5,
+)
+permission_off.__doc__ = """关闭权限"""
+
+permission_off.handle()(group_only)
+
+
+@permission_off.handle()
+async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
+    """关闭当前群权限"""
+    if isinstance(event, GuildMessageEvent):
+        if await db.set_guild_permission(event.guild_id, event.channel_id, False):
+            await permission_off.finish("已开启权限，只有管理员和主人可以操作")
+    else:
+        if await db.set_permission(event.group_id, False):
+            await permission_off.finish("已关闭权限，所有人均可操作")
+    await permission_off.finish("权限已经关闭了，所有人均可操作")
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/permission/permission_on.py` & `haruka-bot-1.5.4/haruka_bot/plugins/permission/permission_on.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Union
-
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent
-from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
-from nonebot.permission import SUPERUSER
-from nonebot_plugin_guild_patch import GuildMessageEvent
-
-from ...database import DB as db
-from ...utils import GUILD_ADMIN, group_only, on_command, to_me
-
-permission_on = on_command(
-    "开启权限",
-    rule=to_me(),
-    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
-    priority=5,
-)
-permission_on.__doc__ = """开启权限"""
-
-permission_on.handle()(group_only)
-
-
-@permission_on.handle()
-async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
-    """开启当前群权限"""
-    if isinstance(event, GuildMessageEvent):
-        if await db.set_guild_permission(event.guild_id, event.channel_id, True):
-            await permission_on.finish("已开启权限，只有管理员和主人可以操作")
-    else:
-        if await db.set_permission(event.group_id, True):
-            await permission_on.finish("已开启权限，只有管理员和主人可以操作")
-    await permission_on.finish("权限已经开启了，只有管理员和主人可以操作")
+from typing import Union
+
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent
+from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
+from nonebot.permission import SUPERUSER
+from nonebot_plugin_guild_patch import GuildMessageEvent
+
+from ...database import DB as db
+from ...utils import GUILD_ADMIN, group_only, on_command, to_me
+
+permission_on = on_command(
+    "开启权限",
+    rule=to_me(),
+    permission=GROUP_OWNER | GROUP_ADMIN | SUPERUSER | GUILD_ADMIN,
+    priority=5,
+)
+permission_on.__doc__ = """开启权限"""
+
+permission_on.handle()(group_only)
+
+
+@permission_on.handle()
+async def _(event: Union[GroupMessageEvent, GuildMessageEvent]):
+    """开启当前群权限"""
+    if isinstance(event, GuildMessageEvent):
+        if await db.set_guild_permission(event.guild_id, event.channel_id, True):
+            await permission_on.finish("已开启权限，只有管理员和主人可以操作")
+    else:
+        if await db.set_permission(event.group_id, True):
+            await permission_on.finish("已开启权限，只有管理员和主人可以操作")
+    await permission_on.finish("权限已经开启了，只有管理员和主人可以操作")
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/plugins/sub/sub_list.py` & `haruka-bot-1.5.4/haruka_bot/plugins/sub/sub_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-from nonebot.adapters.onebot.v11 import Bot
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent, MessageEvent
-
-from ...database import DB as db
-from ...utils import get_type_id, on_command, permission_check, to_me
-
-sub_list = on_command("关注列表", aliases={"主播列表"}, rule=to_me(), priority=5)
-print(sub_list)
-sub_list.__doc__ = """关注列表"""
-
-sub_list.handle()(permission_check)
-
-
-@sub_list.handle()
-async def _(event: MessageEvent, bot: Bot):
-    """发送当前位置的订阅列表"""
-    message = "关注列表（所有群/好友都是分开的）\n\n"
-    subs = await db.get_sub_list(event.message_type, await get_type_id(event))
-    for sub in subs:
-        user = await db.get_user(uid=sub.uid)
-        assert user is not None
-        message += (
-            f"{user.name}（{user.uid}）"
-            f"直播：{'开' if sub.live else '关'}，"
-            f"动态：{'开' if sub.dynamic else '关'}，"
-            # TODO 私聊不显示全体
-            f"全体：{'开' if sub.at else '关'}\n"
-        )
-    if len(message.splitlines()) > 8 and isinstance(event, GroupMessageEvent):
-        await bot.send_group_forward_msg(
-            group_id=event.group_id,
-            messages=[
-                {
-                    "type": "node",
-                    "data": {
-                        "name": "HarukaBot",
-                        "uin": bot.self_id,
-                        "content": message,
-                    },
-                }
-            ],
-        )
-    else:
-        await sub_list.finish(message)
+from nonebot.adapters.onebot.v11 import Bot
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent, MessageEvent
+
+from ...database import DB as db
+from ...utils import get_type_id, on_command, permission_check, to_me
+
+sub_list = on_command("关注列表", aliases={"主播列表"}, rule=to_me(), priority=5)
+sub_list.__doc__ = """关注列表"""
+
+sub_list.handle()(permission_check)
+
+
+@sub_list.handle()
+async def _(event: MessageEvent, bot: Bot):
+    """发送当前位置的订阅列表"""
+    message = "关注列表（所有群/好友都是分开的）\n\n"
+    subs = await db.get_sub_list(event.message_type, await get_type_id(event))
+    for sub in subs:
+        user = await db.get_user(uid=sub.uid)
+        assert user is not None
+        message += (
+            f"{user.name}（{user.uid}）"
+            f"直播：{'开' if sub.live else '关'}，"
+            f"动态：{'开' if sub.dynamic else '关'}，"
+            # TODO 私聊不显示全体
+            f"全体：{'开' if sub.at else '关'}\n"
+        )
+    if len(message.splitlines()) > 8 and isinstance(event, GroupMessageEvent):
+        await bot.send_group_forward_msg(
+            group_id=event.group_id,
+            messages=[
+                {
+                    "type": "node",
+                    "data": {
+                        "name": "HarukaBot",
+                        "uin": bot.self_id,
+                        "content": message,
+                    },
+                }
+            ],
+        )
+    else:
+        await sub_list.finish(message)
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/utils/__init__.py` & `haruka-bot-1.5.4/haruka_bot/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg, RawCommand
 from nonebot.permission import SUPERUSER, Permission
 from nonebot.rule import Rule
 from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent, GuildMessageEvent
 
-from .. import config
+from ..config import plugin_config
 
 
 def get_path(*other):
     """获取数据文件绝对路径"""
-    if config.haruka_dir:
-        dir_path = Path(config.haruka_dir).resolve()
+    if plugin_config.haruka_dir:
+        dir_path = Path(plugin_config.haruka_dir).resolve()
     else:
         dir_path = Path.cwd().joinpath("data")
         # dir_path = Path.cwd().joinpath('data', 'haruka_bot')
     return str(dir_path.joinpath(*other))
 
 
 async def handle_uid(
@@ -62,15 +62,15 @@
         role["role_name"]
         for role in (
             await bot.get_guild_member_profile(
                 guild_id=event.guild_id, user_id=event.user_id
             )
         )["roles"]
     )
-    return bool(roles & set(config.haruka_guild_admin_roles))
+    return bool(roles & set(plugin_config.haruka_guild_admin_roles))
 
 
 GUILD_ADMIN: Permission = Permission(_guild_admin)
 
 
 async def permission_check(
     bot: Bot, event: Union[GroupMessageEvent, PrivateMessageEvent, GuildMessageEvent]
@@ -98,15 +98,15 @@
 async def group_only(
     matcher: Matcher, event: PrivateMessageEvent, command: str = RawCommand()
 ):
     await matcher.finish(f"只有群里才能{command}")
 
 
 def to_me():
-    if config.haruka_to_me:
+    if plugin_config.haruka_to_me:
         from nonebot.rule import to_me
 
         return to_me()
 
     async def _to_me() -> bool:
         return True
 
@@ -196,29 +196,29 @@
 
         return await db.get_guild_type_id(event.guild_id, event.channel_id)
     return event.group_id if isinstance(event, GroupMessageEvent) else event.user_id
 
 
 def check_proxy():
     """检查代理是否有效"""
-    if config.haruka_proxy:
+    if plugin_config.haruka_proxy:
         logger.info("检查代理是否有效")
         try:
             httpx.get(
                 "https://icanhazip.com/",
-                proxies={"all://": config.haruka_proxy},
+                proxies={"all://": plugin_config.haruka_proxy},
                 timeout=2,
             )
         except Exception:
             raise RuntimeError("加载失败，代理无法连接，请检查 HARUKA_PROXY 后重试")
 
 
 def on_startup():
     """安装依赖并检查当前环境是否满足运行条件"""
-    if config.fastapi_reload and sys.platform == "win32":
+    if plugin_config.fastapi_reload and sys.platform == "win32":
         raise ImportError("加载失败，Windows 必须设置 FASTAPI_RELOAD=false 才能正常运行 HarukaBot")
     try:  # 如果开启 realod 只在第一次运行
         asyncio.get_running_loop()
     except RuntimeError:
         from .browser import check_playwright_env, install
 
         check_proxy()
@@ -226,16 +226,16 @@
         asyncio.get_event_loop().run_until_complete(check_playwright_env())
         # 创建数据存储目录
         if not Path(get_path()).is_dir():
             Path(get_path()).mkdir(parents=True)
 
 
 def on_command(cmd, *args, **kwargs):
-    return _on_command(config.haruka_command_prefix + cmd, *args, **kwargs)
+    return _on_command(plugin_config.haruka_command_prefix + cmd, *args, **kwargs)
 
 
-PROXIES = {"all://": config.haruka_proxy}
+PROXIES = {"all://": plugin_config.haruka_proxy}
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler  # noqa
 
 from .browser import get_dynamic_screenshot  # noqa
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/utils/browser.py` & `haruka-bot-1.5.4/haruka_bot/utils/browser.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,31 +3,24 @@
 import re
 import sys
 from pathlib import Path
 from typing import Optional
 
 from nonebot.log import logger
 from playwright.__main__ import main
+from playwright.async_api import Browser, async_playwright
 
-try:
-    from playwright.async_api import Browser, async_playwright
-except ImportError:
-    raise ImportError(
-        "加载失败，请先安装 Visual C++ Redistributable: "
-        "https://aka.ms/vs/17/release/vc_redist.x64.exe"
-    )
-
-from .. import config
+from ..config import plugin_config
 from .fonts_provider import fill_font
 
 _browser: Optional[Browser] = None
 mobile_js = Path(__file__).parent.joinpath("mobile.js")
 
 
-async def init_browser(proxy=config.haruka_proxy, **kwargs) -> Browser:
+async def init_browser(proxy=plugin_config.haruka_proxy, **kwargs) -> Browser:
     if proxy:
         kwargs["proxy"] = {"server": proxy}
     global _browser
     p = await async_playwright().start()
     _browser = await p.chromium.launch(**kwargs)
     return _browser
 
@@ -35,15 +28,17 @@
 async def get_browser() -> Browser:
     global _browser
     if _browser is None or not _browser.is_connected():
         _browser = await init_browser()
     return _browser
 
 
-async def get_dynamic_screenshot(dynamic_id, style=config.haruka_screenshot_style):
+async def get_dynamic_screenshot(
+    dynamic_id, style=plugin_config.haruka_screenshot_style
+):
     """获取动态截图"""
     if style.lower() == "mobile":
         return await get_dynamic_screenshot_mobile(dynamic_id)
     else:
         return await get_dynamic_screenshot_pc(dynamic_id)
 
 
@@ -60,15 +55,15 @@
         viewport={"width": 460, "height": 780},
     )
     try:
         await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), fill_font)
         await page.goto(
             url,
             wait_until="networkidle",
-            timeout=config.haruka_dynamic_timeout * 1000,
+            timeout=plugin_config.haruka_dynamic_timeout * 1000,
         )
         # 动态被删除或者进审核了
         if page.url == "https://m.bilibili.com/404":
             return None
         # await page.add_script_tag(
         #     content=
         #     # 去除打开app按钮
@@ -79,26 +74,26 @@
         #     "const dyn=document.getElementsByClassName('dyn-card')[0];"
         #     "dyn.style.fontFamily='Noto Sans CJK SC, sans-serif';"
         #     "dyn.style.overflowWrap='break-word'"
         # )
         await page.add_script_tag(path=mobile_js)
 
         await page.evaluate(
-            f'setFont("{config.haruka_dynamic_font}", '
-            f'"{config.haruka_dynamic_font_source}")'
-            if config.haruka_dynamic_font
+            f'setFont("{plugin_config.haruka_dynamic_font}", '
+            f'"{plugin_config.haruka_dynamic_font_source}")'
+            if plugin_config.haruka_dynamic_font
             else "setFont()"
         )
         await page.wait_for_function("getMobileStyle()")
 
         await page.wait_for_load_state("networkidle")
         await page.wait_for_load_state("domcontentloaded")
 
         await page.wait_for_timeout(
-            200 if config.haruka_dynamic_font_source == "remote" else 50
+            200 if plugin_config.haruka_dynamic_font_source == "remote" else 50
         )
 
         # 判断字体是否加载完成
         need_wait = ["imageComplete", "fontsLoaded"]
         await asyncio.gather(*[page.wait_for_function(f"{i}()") for i in need_wait])
 
         card = await page.query_selector(
@@ -132,15 +127,17 @@
                 "path": "/",
             }
         ]
     )
     page = await context.new_page()
     try:
         await page.goto(
-            url, wait_until="networkidle", timeout=config.haruka_dynamic_timeout * 1000
+            url,
+            wait_until="networkidle",
+            timeout=plugin_config.haruka_dynamic_timeout * 1000,
         )
         # 动态被删除或者进审核了
         if page.url == "https://www.bilibili.com/404":
             return None
         card = await page.query_selector(".card")
         assert card
         clip = await card.bounding_box()
@@ -159,24 +156,24 @@
 
 
 def install():
     """自动安装、更新 Chromium"""
 
     def restore_env():
         del os.environ["PLAYWRIGHT_DOWNLOAD_HOST"]
-        if config.haruka_proxy:
+        if plugin_config.haruka_proxy:
             del os.environ["HTTPS_PROXY"]
         if original_proxy is not None:
             os.environ["HTTPS_PROXY"] = original_proxy
 
     logger.info("检查 Chromium 更新")
     sys.argv = ["", "install", "chromium"]
     original_proxy = os.environ.get("HTTPS_PROXY")
-    if config.haruka_proxy:
-        os.environ["HTTPS_PROXY"] = config.haruka_proxy
+    if plugin_config.haruka_proxy:
+        os.environ["HTTPS_PROXY"] = plugin_config.haruka_proxy
     os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = "https://npmmirror.com/mirrors/playwright/"
     success = False
     try:
         main()
     except SystemExit as e:
         if e.code == 0:
             success = True
```

### Comparing `haruka-bot-1.5.3a3/haruka_bot/utils/fonts_provider.py` & `haruka-bot-1.5.4/haruka_bot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/haruka_bot/utils/mobile.js` & `haruka-bot-1.5.4/haruka_bot/utils/mobile.js`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/LICENSE` & `haruka-bot-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `haruka-bot-1.5.3a3/pyproject.toml` & `haruka-bot-1.5.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 [project]
 authors = [
     { name = "SK-415", email = "2967923486@qq.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
-    "click~=8.1",
-    "httpx~=0.23",
-    "nonebot-adapter-onebot~=2.2",
-    "nonebot-plugin-apscheduler~=0.2",
-    "nonebot2[fastapi]<3,>=2.0.0rc3",
-    "playwright~=1.30",
-    "pydantic~=1.10",
-    "python-dotenv~=0.21",
-    "tortoise-orm[asyncpg]~=0.19",
-    "bilireq~=0.2",
-    "packaging~=23.0",
-    "nonebot-plugin-guild-patch~=0.2",
+    "click>=8.1.3",
+    "httpx>=0.24.0",
+    "nonebot-adapter-onebot>=2.2.3",
+    "nonebot-plugin-apscheduler>=0.2.0",
+    "nonebot2[fastapi]>=2.0.0rc4",
+    "playwright>=1.33.0",
+    "pydantic>=1.10.7",
+    "python-dotenv>=1.0.0",
+    "tortoise-orm[asyncpg]>=0.19.3",
+    "bilireq>=0.2.5",
+    "packaging>=23.1",
+    "nonebot-plugin-guild-patch>=0.2.3",
+    "msvc-runtime>=14.34.31931; sys_platform == \"win32\"",
 ]
+dynamic = []
 name = "haruka-bot"
-version = "1.5.3a3"
 description = "Push dynamics and live informations from bilibili to QQ. Based on nonebot2."
 readme = "README.md"
 keywords = [
     "nonebot",
     "nonebot2",
     "qqbot",
     "bilibili",
     "bot",
 ]
+version = "1.5.4"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/SK-415/HarukaBot"
 repository = "https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot"
 documentation = "https://github.com/SK-415/HarukaBot#readme"
 
 [project.scripts]
 hb = "haruka_bot.__main__:main"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "nonebot-plugin-gocqhttp>=0.6.4",
+    "nonebot-plugin-gocqhttp>=0.6.10",
 ]
 
+[tool.pdm.version]
+source = "file"
+path = "haruka_bot/version.py"
+
 [tool.pdm.build]
 
 [tool.nonebot]
 adapters = [
     { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
 ]
 plugins = [
```

### Comparing `haruka-bot-1.5.3a3/README.md` & `haruka-bot-1.5.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: haruka-bot
+Version: 1.5.4
+Summary: Push dynamics and live informations from bilibili to QQ. Based on nonebot2.
+License: AGPL-3.0-or-later
+Keywords: nonebot,nonebot2,qqbot,bilibili,bot
+Author-email: SK-415 <2967923486@qq.com>
+Requires-Python: >=3.8,<4.0
+Project-URL: documentation, https://github.com/SK-415/HarukaBot#readme
+Project-URL: homepage, https://github.com/SK-415/HarukaBot
+Project-URL: repository, https://github.com/SK-415/HarukaBot/tree/master/src/plugins/haruka_bot
+Description-Content-Type: text/markdown
+
 [![HarukaBot](https://socialify.git.ci/SK-415/HarukaBot/image?description=1&font=Source%20Code%20Pro&forks=1&issues=1&language=1&logo=https%3A%2F%2Fraw.githubusercontent.com%2FSK-415%2FHarukaBot%2Fmaster%2Fdocs%2F.vuepress%2Fpublic%2Flogo.png&owner=1&pattern=Charlie%20Brown&stargazers=1&theme=Dark)](https://haruka-bot.sk415.icu/)
 
 # [HarukaBot](https://haruka-bot.sk415.icu)——优雅的 B 站推送 QQ 机器人
 
 名称来源：[@白神遥Haruka](https://space.bilibili.com/477332594)
 
 Logo 画师：[@Ratto](https://space.bilibili.com/23242907)
@@ -33,17 +46,18 @@
 
 - [@mnixry](https://github.com/mnixry)：感谢混淆佬为本项目提供的**技♂术指导**。
 - [@wosiwq](https://github.com/wosiwq)：感谢 W 桑撰写的「小小白白话文」。
 - [NoneBot2](https://github.com/nonebot/nonebot2)：HarukaBot 使用的开发框架。
 - [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)：稳定完善的 CQHTTP 实现。
 - [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect)：非常详细的 B 站 API 文档。
 - [bilibili_api](https://github.com/Passkou/bilibili_api)：Python 实现的 B 站 API 库。
-- [HarukaBot_Guild_Patch](https://github.com/17TheWord/HarukaBot_Guild_Patch) 可以让HarukaBot适用于频道的补丁。
+- [HarukaBot_Guild_Patch](https://github.com/17TheWord/HarukaBot_Guild_Patch) 可以让HarukaBot适用于频道的补丁。（已合入 HarukaBot）
 
 ## 支持与贡献
 
 觉得好用可以给这个项目点个 Star 或者去 [爱发电](https://afdian.net/@HarukaBot) 投喂我。
 
 有意见或者建议也欢迎提交 [Issues](https://github.com/SK-415/HarukaBot/issues) 和 [Pull requests](https://github.com/SK-415/HarukaBot/pulls)。
 
 ## 许可证
 本项目使用 [GNU AGPLv3](https://choosealicense.com/licenses/agpl-3.0/) 作为开源许可证。
+
```

