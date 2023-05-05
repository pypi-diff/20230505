# Comparing `tmp/nonebot_plugin_send_anything_anywhere-0.2.2.tar.gz` & `tmp/nonebot_plugin_send_anything_anywhere-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.4.tar", max compression
```

## Comparing `nonebot_plugin_send_anything_anywhere-0.2.2.tar` & `nonebot_plugin_send_anything_anywhere-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1066 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/LICENSE
--rw-r--r--   0        0        0     5706 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/README.md
--rw-r--r--   0        0        0      759 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/__init__.py
--rw-r--r--   0        0        0       60 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/__init__.py
--rw-r--r--   0        0        0     4908 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/onebot_v11.py
--rw-r--r--   0        0        0     5825 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/onebot_v12.py
--rw-r--r--   0        0        0     5095 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/qqguild.py
--rw-r--r--   0        0        0      189 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/types/__init__.py
--rw-r--r--   0        0        0     1934 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/types/common_message_segment.py
--rw-r--r--   0        0        0     1110 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/types/custom_message_segment.py
--rw-r--r--   0        0        0     1427 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/__init__.py
--rw-r--r--   0        0        0      443 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/const.py
--rw-r--r--   0        0        0      449 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/exceptions.py
--rw-r--r--   0        0        0      429 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/helpers.py
--rw-r--r--   0        0        0     4754 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/platform_send_target.py
--rw-r--r--   0        0        0    11126 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/types.py
--rw-r--r--   0        0        0     1460 2023-03-26 03:50:17.339572 nonebot_plugin_send_anything_anywhere-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6689 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.2/setup.py
--rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5946 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/README.md
+-rw-r--r--   0        0        0      929 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/__init__.py
+-rw-r--r--   0        0        0     5355 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/kaiheila.py
+-rw-r--r--   0        0        0     5537 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     8274 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     5923 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/qqguild.py
+-rw-r--r--   0        0        0      189 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/__init__.py
+-rw-r--r--   0        0        0     1955 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/common_message_segment.py
+-rw-r--r--   0        0        0     1148 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/custom_message_segment.py
+-rw-r--r--   0        0        0     1741 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/__init__.py
+-rw-r--r--   0        0        0     2093 2023-05-05 14:06:51.445510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/auto_select_bot.py
+-rw-r--r--   0        0        0      553 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/const.py
+-rw-r--r--   0        0        0      449 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/exceptions.py
+-rw-r--r--   0        0        0      429 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/helpers.py
+-rw-r--r--   0        0        0     5586 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/platform_send_target.py
+-rw-r--r--   0        0        0    11545 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/types.py
+-rw-r--r--   0        0        0     1703 2023-05-05 14:06:51.449510 nonebot_plugin_send_anything_anywhere-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6929 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.4/setup.py
+-rw-r--r--   0        0        0     7012 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.4/PKG-INFO
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/LICENSE` & `nonebot_plugin_send_anything_anywhere-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/README.md` & `nonebot_plugin_send_anything_anywhere-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,35 +81,36 @@
 
 ## 支持情况
 
 ✅:支持 ✖️:支持不了 🚧:等待适配
 
 ### 支持的 adapter
 
-| OneBot v11 | OneBot v12 | QQ Guild |
-| :--------: | :--------: | :------: |
-|     ✅     |     ✅     |    ✅    |
+| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |
+| :--------: | :--------: | :------: | :------: |
+|     ✅     |     ✅     |    ✅    |    ✅    |
 
 ### 支持的消息类型
 
-|      | OneBot v11 | OneBot v12 | QQ Guild |
-| :--: | :--------: | :--------: | :------: |
-| 文字 |     ✅     |     ✅     |    ✅    |
-| 图片 |     ✅     |     ✅     |    ✅    |
-|  at  |     ✅     |     ✅     |    ✅    |
-| 回复 |     ✅     |     ✅     |    ✅    |
+|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |
+| :--: | :--------: | :--------: | :------: | :----: |
+| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |
+| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |
+|  at  |     ✅     |     ✅     |    ✅    |   ✅   |
+| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |
 
 ### 支持的发送目标
 
-|                   | OneBot v11 | OneBot v12  | QQ Guild |
-| :---------------: | :--------: | :---------: | :------: |
-|       QQ 群       |     ✅     |     ✅      |          |
-|      QQ 私聊      |     ✅     |     ✅      |          |
-| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |
-|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |
+|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |
+| :---------------: | :--------: | :---------: | :------: | :------: |
+|       QQ 群       |     ✅     |     ✅      |          |          |
+|      QQ 私聊      |     ✅     |     ✅      |          |          |
+| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |
+|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |
+|  开黑啦私聊/频道  |            |             |          |    ✅    |
 
 注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用
 
 ## 问题与例子
 
 因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/onebot_v11.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/onebot_v11.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional
 
 from nonebot.adapters import Bot, Event
 
 from ..types import Text, Image, Reply, Mention
 from ..utils import (
     TargetQQGroup,
     MessageFactory,
@@ -11,14 +11,15 @@
     TargetQQPrivate,
     SupportedAdapters,
     SupportedPlatform,
     MessageSegmentFactory,
     AggregatedMessageFactory,
     register_sender,
     register_ms_adapter,
+    register_list_targets,
     register_convert_to_arg,
     assamble_message_factory,
     register_target_extractor,
 )
 
 try:
     from nonebot.adapters.onebot.v11 import Bot as BotOB11
@@ -57,23 +58,23 @@
 
     @register_target_extractor(GroupMessageEvent)
     def _extract_group_msg_event(event: Event) -> TargetQQGroup:
         assert isinstance(event, GroupMessageEvent)
         return TargetQQGroup(group_id=event.group_id)
 
     @register_convert_to_arg(adapter, SupportedPlatform.qq_private)
-    def _gen_private(target: PlatformTarget) -> dict[str, Any]:
+    def _gen_private(target: PlatformTarget) -> Dict[str, Any]:
         assert isinstance(target, TargetQQPrivate)
         return {
             "message_type": "private",
             "user_id": target.user_id,
         }
 
     @register_convert_to_arg(adapter, SupportedPlatform.qq_group)
-    def _gen_group(target: PlatformTarget) -> dict[str, Any]:
+    def _gen_group(target: PlatformTarget) -> Dict[str, Any]:
         assert isinstance(target, TargetQQGroup)
         return {
             "message_type": "group",
             "group_id": target.group_id,
         }
 
     @register_sender(SupportedAdapters.onebot_v11)
@@ -82,15 +83,15 @@
         msg: MessageFactory[MessageSegmentFactory],
         target,
         event,
         at_sender: bool,
         reply: bool,
     ):
         assert isinstance(bot, BotOB11)
-        assert isinstance(target, TargetQQGroup | TargetQQPrivate)
+        assert isinstance(target, (TargetQQGroup, TargetQQPrivate))
         if event:
             assert isinstance(event, MessageEvent)
             full_msg = assamble_message_factory(
                 msg,
                 Mention(event.get_user_id()),
                 Reply(event.message_id),
                 at_sender,
@@ -103,22 +104,22 @@
             message_segment = await message_segment_factory.build(bot)
             message_to_send += message_segment
         await bot.send_msg(message=message_to_send, **target.arg_dict(bot))
 
     @AggregatedMessageFactory.register_aggragated_sender(adapter)
     async def aggregate_send(
         bot: Bot,
-        message_factories: list[MessageFactory],
+        message_factories: List[MessageFactory],
         target: PlatformTarget,
         event: Optional[Event],
     ):
         assert isinstance(bot, BotOB11)
         login_info = await bot.get_login_info()
 
-        msg_list: list[Message] = []
+        msg_list: List[Message] = []
         for msg_fac in message_factories:
             msg = await msg_fac.build(bot)
             assert isinstance(msg, Message)
             msg_list.append(msg)
         aggregated_message_segment = Message(
             [
                 MessageSegment.node_custom(
@@ -126,23 +127,42 @@
                     nickname=login_info["nickname"],
                     content=msg,
                 )
                 for msg in msg_list
             ]
         )
 
-        match target:
-            case TargetQQGroup(group_id=group_id):
-                await bot.send_group_forward_msg(
-                    group_id=group_id, messages=aggregated_message_segment
-                )
-            case TargetQQPrivate(user_id=user_id):
-                await bot.send_private_forward_msg(
-                    user_id=user_id, messages=aggregated_message_segment
-                )
-            case _:  # pragma: no cover
-                raise RuntimeError(f"{target.__class__.__name__} not supported")
+        if isinstance(target, TargetQQGroup):
+            await bot.send_group_forward_msg(
+                group_id=target.group_id, messages=aggregated_message_segment
+            )
+        elif isinstance(target, TargetQQPrivate):
+            await bot.send_private_forward_msg(
+                user_id=target.user_id, messages=aggregated_message_segment
+            )
+        else:  # pragma: no cover
+            raise RuntimeError(f"{target.__class__.__name__} not supported")
+
+    @register_list_targets(SupportedAdapters.onebot_v11)
+    async def list_targets(bot: Bot) -> List[PlatformTarget]:
+        assert isinstance(bot, BotOB11)
+
+        targets = []
+        groups = await bot.get_group_list()
+        for group in groups:
+            group_id = group["group_id"]
+            target = TargetQQGroup(group_id=group_id)
+            targets.append(target)
+
+        # 获取好友列表
+        users = await bot.get_friend_list()
+        for user in users:
+            user_id = user["user_id"]
+            target = TargetQQPrivate(user_id=user_id)
+            targets.append(target)
+
+        return targets
 
 except ImportError:
     pass
 except Exception as e:
     raise e
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/onebot_v12.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/kaiheila.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,157 @@
-from io import BytesIO
-from pathlib import Path
 from functools import partial
+from typing import Any, Dict, List
 
 from nonebot.adapters import Event
 from nonebot.adapters import Bot as BaseBot
 
 from ..types import Text, Image, Reply, Mention
+from ..utils.platform_send_target import TargetKaiheilaChannel, TargetKaiheilaPrivate
 from ..utils import (
-    TargetQQGroup,
     MessageFactory,
     PlatformTarget,
-    TargetQQPrivate,
-    TargetOB12Unknow,
     SupportedAdapters,
     SupportedPlatform,
-    TargetQQGuildChannel,
     MessageSegmentFactory,
     register_sender,
     register_ms_adapter,
+    register_list_targets,
     register_convert_to_arg,
     assamble_message_factory,
     register_target_extractor,
 )
 
 try:
-    from nonebot.adapters.onebot.v12 import (  # ChannelMessageEvent,
-        Bot,
-        Message,
+    from nonebot.adapters.kaiheila import Bot
+    from nonebot.adapters.kaiheila.api import Guild, Channel, UserChat
+    from nonebot.adapters.kaiheila.message import Message, MessageSegment
+    from nonebot.adapters.kaiheila.event import (
         MessageEvent,
-        MessageSegment,
-        GroupMessageEvent,
+        ChannelMessageEvent,
         PrivateMessageEvent,
     )
 
-    adapter = SupportedAdapters.onebot_v12
-    register_onebot_v12 = partial(register_ms_adapter, adapter)
+    def _unwrap_paging_api(field: str):
+        def decorator(func):
+            async def wrapper(*args, **kwargs):
+                result = await func(*args, **kwargs)
+                while True:
+                    for x in getattr(result, field):
+                        yield x
 
-    MessageFactory.register_adapter_message(adapter, Message)
+                    if result.meta.page != result.meta.page_total:
+                        result = await func(*args, **kwargs, page=result.meta.page + 1)
+                    else:
+                        break
 
-    @register_onebot_v12(Text)
+            return wrapper
+
+        return decorator
+
+    adapter = SupportedAdapters.kaiheila
+    register_kaiheila = partial(register_ms_adapter, adapter)
+
+    MessageFactory.register_adapter_message(SupportedAdapters.kaiheila, Message)
+
+    @register_kaiheila(Text)
     def _text(t: Text) -> MessageSegment:
         return MessageSegment.text(t.data["text"])
 
-    @register_onebot_v12(Image)
+    @register_kaiheila(Image)
     async def _image(i: Image, bot: BaseBot) -> MessageSegment:
         if not isinstance(bot, Bot):
             raise TypeError(f"Unsupported type of bot: {type(bot)}")
-        image = i.data["image"]
-        name = i.data["name"]
-        if isinstance(image, str):
-            resp = await bot.upload_file(type="url", name=name, url=image)
-        elif isinstance(image, Path):
-            resp = await bot.upload_file(
-                type="path", name=name, path=str(image.resolve())
-            )
-        elif isinstance(image, BytesIO):
-            image = image.getvalue()
-            resp = await bot.upload_file(type="data", name=name, data=image)
-        elif isinstance(image, bytes):
-            resp = await bot.upload_file(type="data", name=name, data=image)
-        else:
-            raise TypeError(f"Unsupported type of image: {type(image)}")
 
-        file_id = resp["file_id"]
-        return MessageSegment.image(file_id)
+        file_key = await bot.upload_file(i.data["image"], i.data["name"])
+        return MessageSegment.image(file_key)
 
-    @register_onebot_v12(Mention)
-    async def _mention(m: Mention) -> MessageSegment:
-        return MessageSegment.mention(m.data["user_id"])
-
-    @register_onebot_v12(Reply)
-    async def _reply(r: Reply) -> MessageSegment:
-        return MessageSegment.reply(r.data["message_id"])
+    @register_kaiheila(Mention)
+    def _mention(m: Mention) -> MessageSegment:
+        return MessageSegment.KMarkdown("(met)" + m.data["user_id"] + "(met)")
+
+    @register_kaiheila(Reply)
+    def _reply(r: Reply) -> MessageSegment:
+        return MessageSegment.quote(r.data["message_id"])
 
     @register_target_extractor(PrivateMessageEvent)
-    def _extract_private_msg_event(event: Event) -> PlatformTarget:
+    def _extract_private_msg_event(event: Event) -> TargetKaiheilaPrivate:
         assert isinstance(event, PrivateMessageEvent)
-        if event.self.platform == "qq":
-            return TargetQQPrivate(user_id=int(event.user_id))
-        return TargetOB12Unknow(detail_type="private", user_id=event.user_id)
-
-    @register_target_extractor(GroupMessageEvent)
-    def _extract_group_msg_event(event: Event) -> PlatformTarget:
-        assert isinstance(event, GroupMessageEvent)
-        if event.self.platform == "qq":
-            return TargetQQGroup(group_id=int(event.group_id))
-        return TargetOB12Unknow(detail_type="group", group_id=event.group_id)
-
-    # @register_target_extractor(ChannelMessageEvent)
-    # def _extarct_channel_msg_event(event: Event) -> PlatformTarget:
-    #     assert isinstance(event, ChannelMessageEvent)
-    #     if event.self.platform == 'qqguild': # all4one
-    #         return TargetQQGuildChannel(channel_id=int(event.channel_id))
-    #     return TargetOB12Unknow(
-    #         detail_type="channel", channel_id=event.channel_id,
-    #       guild_id=event.guild_id
-    #     )
-
-    @register_convert_to_arg(adapter, SupportedPlatform.qq_group)
-    def _to_qq_group(target: PlatformTarget):
-        assert isinstance(target, TargetQQGroup)
+        return TargetKaiheilaPrivate(user_id=event.user_id)
+
+    @register_target_extractor(ChannelMessageEvent)
+    def _extract_channel_msg_event(event: Event) -> TargetKaiheilaChannel:
+        assert isinstance(event, ChannelMessageEvent)
+        return TargetKaiheilaChannel(channel_id=event.target_id)
+
+    @register_convert_to_arg(adapter, SupportedPlatform.kaiheila_private)
+    def _gen_private(target: PlatformTarget) -> Dict[str, Any]:
+        assert isinstance(target, TargetKaiheilaPrivate)
         return {
-            "detail_type": "group",
-            "group_id": str(target.group_id),
+            "user_id": target.user_id,
         }
 
-    @register_convert_to_arg(adapter, SupportedPlatform.qq_private)
-    def _to_qq_private(target: PlatformTarget):
-        assert isinstance(target, TargetQQPrivate)
+    @register_convert_to_arg(adapter, SupportedPlatform.kaiheila_channel)
+    def _gen_channel(target: PlatformTarget) -> Dict[str, Any]:
+        assert isinstance(target, TargetKaiheilaChannel)
         return {
-            "detail_type": "private",
-            "user_id": str(target.user_id),
+            "channel_id": target.channel_id,
         }
 
-    # @register_convert_to_arg(adapter, SupportedPlatform.qq_guild_channel)
-    # def _to_qq_guild_channel(target: PlatformTarget):
-    #     assert isinstance(target, TargetQQGuildChannel)
-    #     return {
-    #             "detail_type": "channel",
-    #             "channel_id": target.channel_id,
-    #             }
-
-    # @register_convert_to_arg(adapter, SupportedPlatform.qq_guild_direct)
-    # def _to_qq_guild_direct(target: PlatformTarget):
-    #     assert isinstance(target, TargetQQGuildDirect)
-    #     return {
-    #             "detail_type": "private",
-    #             "guild_id": target.source_guild_id,
-    #             }
-
-    @register_convert_to_arg(adapter, SupportedPlatform.unknown_ob12)
-    def _to_unknow(target: PlatformTarget):
-        assert isinstance(target, TargetOB12Unknow)
-        return target.dict(exclude={"platform_type"})
-
-    @register_sender(SupportedAdapters.onebot_v12)
+    @register_sender(SupportedAdapters.kaiheila)
     async def send(
         bot,
         msg: MessageFactory[MessageSegmentFactory],
         target,
         event,
         at_sender: bool,
         reply: bool,
     ):
         assert isinstance(bot, Bot)
-        assert isinstance(
-            target,
-            TargetQQGroup | TargetQQPrivate | TargetQQGuildChannel | TargetOB12Unknow,
-        )
+        assert isinstance(target, (TargetKaiheilaPrivate, TargetKaiheilaChannel))
 
         if event:
             assert isinstance(event, MessageEvent)
             full_msg = assamble_message_factory(
-                msg, Mention(event.user_id), Reply(event.message_id), at_sender, reply
+                msg,
+                Mention(event.get_user_id()),
+                Reply(event.msg_id),
+                at_sender,
+                reply,
             )
         else:
             full_msg = msg
-        msg_to_send = await full_msg.build(bot)
-        assert isinstance(msg_to_send, Message)
-        await bot.send_message(message=msg_to_send, **target.arg_dict(bot))
+
+        message_to_send = Message()
+        for message_segment_factory in full_msg:
+            message_segment = await message_segment_factory.build(bot)
+            message_to_send += message_segment
+
+        await bot.send_msg(message=message_to_send, **target.arg_dict(bot))
+
+    @register_list_targets(SupportedAdapters.kaiheila)
+    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
+        assert isinstance(bot, Bot)
+
+        targets = []
+
+        async for guild in _unwrap_paging_api("guilds")(bot.guild_list)():
+            guild: Guild
+            async for channel in _unwrap_paging_api("channels")(bot.channel_list)(
+                guild_id=guild.id_
+            ):
+                assert isinstance(channel, Channel)
+                assert channel.id_
+                target = TargetKaiheilaChannel(channel_id=channel.id_)
+                targets.append(target)
+
+        async for user_chat in _unwrap_paging_api("user_chats")(bot.userChat_list)():
+            user_chat: UserChat
+            assert user_chat.target_info and user_chat.target_info.id_
+            target = TargetKaiheilaPrivate(user_id=user_chat.target_info.id_)
+            targets.append(target)
+
+        return targets
 
 except ImportError:
     pass
 except Exception as e:
     raise e
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/adapters/qqguild.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/adapters/qqguild.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from typing import List
 from functools import partial
 
 from nonebot.adapters import Event
+from nonebot.adapters import Bot as BaseBot
 
 from ..types import Text, Image, Reply, Mention
 from ..utils import (
     MessageFactory,
     PlatformTarget,
     SupportedAdapters,
     TargetQQGuildDirect,
     TargetQQGuildChannel,
     MessageSegmentFactory,
     register_sender,
     register_ms_adapter,
+    register_list_targets,
     assamble_message_factory,
     register_target_extractor,
 )
 
 try:
     from nonebot.adapters.qqguild import (
         Bot,
@@ -69,15 +72,15 @@
         msg: MessageFactory[MessageSegmentFactory],
         target,
         event,
         at_sender: bool,
         reply: bool,
     ):
         assert isinstance(bot, Bot)
-        assert isinstance(target, TargetQQGuildChannel | TargetQQGuildDirect)
+        assert isinstance(target, (TargetQQGuildChannel, TargetQQGuildDirect))
 
         full_msg = msg
         if event:
             assert isinstance(event, MessageEvent)
             assert event.author
             assert event.id
             full_msg = assamble_message_factory(
@@ -101,27 +104,27 @@
             markdown = markdown[-1].data["markdown"]
         if reference := (message["reference"] or None):
             reference = reference[-1].data["reference"]
 
         if event:  # reply to user
             if isinstance(event, DirectMessageCreateEvent):
                 await bot.post_dms_messages(
-                    guild_id=event.guild_id,
+                    guild_id=event.guild_id,  # type: ignore
                     msg_id=event.id,
                     content=content,
-                    embed=embed,
+                    embed=embed,  # type: ignore
                     ark=ark,  # type: ignore
                     image=image,  # type: ignore
                     file_image=file_image,  # type: ignore
                     markdown=markdown,  # type: ignore
                     message_reference=reference,  # type: ignore
                 )
             else:
                 await bot.post_messages(
-                    channel_id=event.channel_id,
+                    channel_id=event.channel_id,  # type: ignore
                     msg_id=event.id,
                     content=content,
                     embed=embed,  # type: ignore
                     ark=ark,  # type: ignore
                     image=image,  # type: ignore
                     file_image=file_image,  # type: ignore
                     markdown=markdown,  # type: ignore
@@ -129,21 +132,41 @@
                 )
         else:
             if isinstance(target, TargetQQGuildChannel):
                 assert target.channel_id
                 await bot.post_messages(
                     channel_id=target.channel_id,
                     content=content,
-                    embed=embed,
-                    ark=ark,
-                    image=image,
-                    file_image=file_image,
-                    markdown=markdown,
-                    message_reference=reference,
+                    embed=embed,  # type: ignore
+                    ark=ark,  # type: ignore
+                    image=image,  # type: ignore
+                    file_image=file_image,  # type: ignore
+                    markdown=markdown,  # type: ignore
+                    message_reference=reference,  # type: ignore
                 )
             else:
                 raise NotImplementedError("QQ频道主动发送私信暂未实现")
 
+    @register_list_targets(SupportedAdapters.qqguild)
+    async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
+        assert isinstance(bot, Bot)
+
+        targets = []
+
+        # TODO: 私聊
+
+        guilds = await bot.guilds()
+        for guild in guilds:
+            channels = await bot.get_channels(guild_id=guild.id)  # type: ignore
+            for channel in channels:
+                targets.append(
+                    TargetQQGuildChannel(
+                        channel_id=channel.id,  # type: ignore
+                    )
+                )
+
+        return targets
+
 except ImportError:
     pass
 except Exception as e:
     raise e
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/types/common_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/common_message_segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 from pathlib import Path
-from typing import TypedDict
+from typing import Union, TypedDict
 
 from ..utils import MessageFactory, MessageSegmentFactory
 
 
 class TextData(TypedDict):
     text: str
 
@@ -27,25 +27,25 @@
         return self.data["text"]
 
 
 MessageFactory.register_text_ms(lambda text: Text(text))
 
 
 class ImageData(TypedDict):
-    image: str | bytes | Path | BytesIO
+    image: Union[str, bytes, Path, BytesIO]
     name: str
 
 
 class Image(MessageSegmentFactory):
     """图片消息段"""
 
     data: ImageData
 
     def __init__(
-        self, image: str | bytes | Path | BytesIO, name: str = "image"
+        self, image: Union[str, bytes, Path, BytesIO], name: str = "image"
     ) -> None:
         """图片消息段
 
         支持多种格式的数据
 
         参数:
             image: str 为图片 URL，bytes 为图片数据，Path 为图片路径，BytesIO 为图片文件流
@@ -80,15 +80,15 @@
 
 
 class Reply(MessageSegmentFactory):
     """回复其他消息的消息段"""
 
     data: ReplyData
 
-    def __init__(self, message_id: str | int):
+    def __init__(self, message_id: Union[str, int]):
         """回复其他消息的消息段
 
         参数:
             message_id: 需要回复消息的 ID
         """
 
         super().__init__()
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/types/custom_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/types/custom_message_segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Dict, Union
+
 from nonebot.adapters import Bot, MessageSegment
 
 from ..utils import (
     CustomBuildFunc,
     SupportedAdapters,
     AdapterNotSupported,
     MessageSegmentFactory,
@@ -11,15 +13,15 @@
 
 
 class Custom(MessageSegmentFactory):
     "用户自定义的 MessageSegment"
 
     def __init__(
         self,
-        ms_dict: dict[SupportedAdapters, MessageSegment | CustomBuildFunc],
+        ms_dict: Dict[SupportedAdapters, Union[MessageSegment, CustomBuildFunc]],
     ):
         """
         自定义 MessageSegment
 
         参数:
             ms_dict: 字典，key 为 SupportedAdapters，
                      val 为 MessageSegment 或 Bot -> MessageSegment 的函数，
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/platform_send_target.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/platform_send_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 from abc import ABC
 from typing_extensions import Self
 from typing import (
     TYPE_CHECKING,
     Any,
+    Dict,
     Type,
+    Tuple,
+    Union,
     Literal,
     Callable,
     ClassVar,
     Optional,
     Awaitable,
 )
 
@@ -19,15 +22,15 @@
 from .const import SupportedAdapters, SupportedPlatform
 
 if TYPE_CHECKING:
     from .types import MessageFactory
 
 
 class PlatformTarget(BaseModel, ABC):
-    _deseriazer_map: ClassVar[dict[SupportedPlatform, Type["PlatformTarget"]]] = {}
+    _deseriazer_map: ClassVar[Dict[SupportedPlatform, Type["PlatformTarget"]]] = {}
     platform_type: SupportedPlatform
 
     class Config:
         frozen = True
         orm_mode = True
 
     def __init_subclass__(cls) -> None:
@@ -40,15 +43,15 @@
         if (self.platform_type, adapter_type) not in convert_to_arg_map.keys():
             raise RuntimeError(
                 f"PlatformTarget {self.platform_type} not support {adapter_type}"
             )
         return convert_to_arg_map[(self.platform_type, adapter_type)](self)
 
     @classmethod
-    def deserialize(cls, source: str | dict) -> Self:
+    def deserialize(cls, source: Union[str, dict]) -> Self:
         if isinstance(source, str):
             raw_obj = json.loads(source)
         else:
             raw_obj = source
             assert raw_obj.get("platform_type")
         platform_type = SupportedPlatform(raw_obj["platform_type"])
         return cls._deseriazer_map[platform_type].parse_obj(raw_obj)
@@ -118,28 +121,66 @@
     detail_type: Literal["private", "group", "channel"]
     user_id: Optional[str] = None
     group_id: Optional[str] = None
     guild_id: Optional[str] = None
     channel_id: Optional[str] = None
 
 
-ConvertToArg = Callable[[PlatformTarget], dict[str, Any]]
-convert_to_arg_map: dict[tuple[SupportedPlatform, SupportedAdapters], ConvertToArg] = {}
+class TargetKaiheilaChannel(PlatformTarget):
+    """开黑啦频道
+
+    参数
+        channel_id: 频道ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.kaiheila_channel
+    ] = SupportedPlatform.kaiheila_channel
+    channel_id: str
+
+
+class TargetKaiheilaPrivate(PlatformTarget):
+    """开黑啦私聊
+
+    参数
+        user_id: 接收人ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.kaiheila_private
+    ] = SupportedPlatform.kaiheila_private
+    user_id: str
+
+
+# this union type is for deserialize pydantic model with nested PlatformTarget
+AllSupportedPlatformTarget = Union[
+    TargetQQGroup,
+    TargetQQPrivate,
+    TargetQQGuildChannel,
+    TargetQQGuildDirect,
+    TargetKaiheilaPrivate,
+    TargetKaiheilaChannel,
+    TargetOB12Unknow,
+]
+
+
+ConvertToArg = Callable[[PlatformTarget], Dict[str, Any]]
+convert_to_arg_map: Dict[Tuple[SupportedPlatform, SupportedAdapters], ConvertToArg] = {}
 
 
 def register_convert_to_arg(adapter: SupportedAdapters, platform: SupportedPlatform):
     def wrapper(func: ConvertToArg):
         convert_to_arg_map[(platform, adapter)] = func
         return func
 
     return wrapper
 
 
 Extractor = Callable[[Event], PlatformTarget]
-extractor_map: dict[Type[Event], Extractor] = {}
+extractor_map: Dict[Type[Event], Extractor] = {}
 
 
 def register_target_extractor(event: Type[Event]):
     def wrapper(func: Extractor):
         extractor_map[event] = func
         return func
 
@@ -152,28 +193,28 @@
         if event_type in extractor_map.keys():
             if not issubclass(event_type, Event):
                 break
             return extractor_map[event_type](event)
     raise RuntimeError(f"event {event.__class__} not supported")
 
 
-def get_target(event: Event) -> PlatformTarget | None:
+def get_target(event: Event) -> Optional[PlatformTarget]:
     "从事件中提取出发送目标，如果不能提取就返回 None"
     try:
         return extract_target(event)
     except RuntimeError:
         pass
 
 
 Sender = Callable[
     [Bot, "MessageFactory", "PlatformTarget", Optional[Event], bool, bool],
     Awaitable[None],
 ]
 
-sender_map: dict[SupportedAdapters, Sender] = {}
+sender_map: Dict[SupportedAdapters, Sender] = {}
 
 
 def register_sender(adapter: SupportedAdapters):
     def wrapper(sender: Sender):
         sender_map[adapter] = sender
         return sender
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/nonebot_plugin_saa/utils/types.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/nonebot_plugin_saa/utils/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 import asyncio
 from abc import ABC
 from copy import deepcopy
 from warnings import warn
 from inspect import signature
 from typing_extensions import Self
 from typing import (
+    Dict,
+    List,
     Type,
+    Union,
     TypeVar,
     Callable,
     ClassVar,
     Iterable,
     Optional,
     Awaitable,
     cast,
 )
 
 from nonebot.matcher import current_bot, current_event
 from nonebot.adapters import Bot, Event, Message, MessageSegment
 
+from .auto_select_bot import get_bot
 from .const import SupportedAdapters
 from .helpers import extract_adapter_type
 from .exceptions import FallbackToDefault, AdapterNotInstalled
 from .platform_send_target import PlatformTarget, sender_map, extract_target
 
 TMSF = TypeVar("TMSF", bound="MessageSegmentFactory")
 TMF = TypeVar("TMF", bound="MessageFactory")
-BuildFunc = (
-    Callable[[TMSF], MessageSegment | Awaitable[MessageSegment]]
-    | Callable[[TMSF, Bot], MessageSegment | Awaitable[MessageSegment]]
-)
-CustomBuildFunc = (
-    Callable[[], MessageSegment | Awaitable[MessageSegment]]
-    | Callable[[Bot], MessageSegment | Awaitable[MessageSegment]]
-)
+BuildFunc = Union[
+    Callable[[TMSF], Union[MessageSegment, Awaitable[MessageSegment]]],
+    Callable[[TMSF, Bot], Union[MessageSegment, Awaitable[MessageSegment]]],
+]
+CustomBuildFunc = Union[
+    Callable[[], Union[MessageSegment, Awaitable[MessageSegment]]],
+    Callable[[Bot], Union[MessageSegment, Awaitable[MessageSegment]]],
+]
 
 
 async def do_build(
     msf: "MessageSegmentFactory", builder: BuildFunc, bot: Bot
 ) -> MessageSegment:
     if len(signature(builder).parameters) == 1:
         builder = cast(
             Callable[
-                ["MessageSegmentFactory"], MessageSegment | Awaitable[MessageSegment]
+                ["MessageSegmentFactory"],
+                Union[MessageSegment, Awaitable[MessageSegment]],
             ],
             builder,
         )
         res = builder(msf)
     elif len(signature(builder).parameters) == 2:
         builder = cast(
             Callable[
                 ["MessageSegmentFactory", Bot],
-                MessageSegment | Awaitable[MessageSegment],
+                Union[MessageSegment, Awaitable[MessageSegment]],
             ],
             builder,
         )
         res = builder(msf, bot)
     else:
         raise RuntimeError()
     if asyncio.iscoroutine(res):
@@ -63,47 +68,49 @@
         res = cast(MessageSegment, res)
         return res
 
 
 async def do_build_custom(builder: CustomBuildFunc, bot: Bot) -> MessageSegment:
     if len(signature(builder).parameters) == 0:
         builder = cast(
-            Callable[[], MessageSegment | Awaitable[MessageSegment]],
+            Callable[[], Union[MessageSegment, Awaitable[MessageSegment]]],
             builder,
         )
         res = builder()
     elif len(signature(builder).parameters) == 1:
         builder = cast(
-            Callable[[Bot], MessageSegment | Awaitable[MessageSegment]],
+            Callable[[Bot], Union[MessageSegment, Awaitable[MessageSegment]]],
             builder,
         )
         res = builder(bot)
     else:
         raise RuntimeError()
     if asyncio.iscoroutine(res):
         return await res
     else:
         res = cast(MessageSegment, res)
         return res
 
 
 class MessageSegmentFactory(ABC):
     _builders: ClassVar[
-        dict[
+        Dict[
             SupportedAdapters,
-            Callable[[Self], MessageSegment | Awaitable[MessageSegment]]
-            | Callable[[Self, Bot], MessageSegment | Awaitable[MessageSegment]],
+            Union[
+                Callable[[Self], Union[MessageSegment, Awaitable[MessageSegment]]],
+                Callable[[Self, Bot], Union[MessageSegment, Awaitable[MessageSegment]]],
+            ],
         ]
     ]
 
     data: dict
-    _custom_builders: dict[SupportedAdapters, CustomBuildFunc]
+    _custom_builders: Dict[SupportedAdapters, CustomBuildFunc]
 
     def _register_custom_builder(
-        self, adapter: SupportedAdapters, ms: MessageSegment | CustomBuildFunc
+        self, adapter: SupportedAdapters, ms: Union[MessageSegment, CustomBuildFunc]
     ):
         if isinstance(ms, MessageSegment):
             self._custom_builders[adapter] = lambda _: ms
         else:
             self._custom_builders[adapter] = ms
 
     def _get_custom_builder(
@@ -118,107 +125,107 @@
         cls._builders = {}
         return super().__init_subclass__()
 
     def __eq__(self, other: Self) -> bool:
         return self.data == other.data
 
     def overwrite(
-        self, adapter: SupportedAdapters, ms: MessageSegment | CustomBuildFunc
+        self, adapter: SupportedAdapters, ms: Union[MessageSegment, CustomBuildFunc]
     ) -> Self:
         "为某个 adapter 重写产生的 MessageSegment 或重写产生 MessageSegment 的方法"
         self._register_custom_builder(adapter, ms)
         return self
 
     async def build(self, bot: Bot) -> MessageSegment:
         adapter_name = extract_adapter_type(bot)
         if custom_builder := self._get_custom_builder(adapter_name):
             return await do_build_custom(custom_builder, bot)
         if builder := self._builders[adapter_name]:
             return await do_build(self, builder, bot)
         raise AdapterNotInstalled(adapter_name)
 
-    def __add__(self: TMSF, other: str | TMSF | Iterable[TMSF]):
+    def __add__(self: TMSF, other: Union[str, TMSF, Iterable[TMSF]]):
         return MessageFactory(self) + other
 
-    def __radd__(self: TMSF, other: str | TMSF | Iterable[TMSF]):
+    def __radd__(self: TMSF, other: Union[str, TMSF, Iterable[TMSF]]):
         return MessageFactory(other) + self
 
 
-class MessageFactory(list[TMSF]):
+class MessageFactory(List[TMSF]):
     _text_factory: Callable[[str], TMSF]
-    _message_registry: dict[SupportedAdapters, type[Message]] = {}
+    _message_registry: Dict[SupportedAdapters, Type[Message]] = {}
 
     @classmethod
     def register_text_ms(cls, factory: Callable[[str], TMSF]):
         cls._text_factory = factory
         return factory
 
     @classmethod
     def get_text_factory(cls):
         return cls._text_factory
 
     @classmethod
     def register_adapter_message(
-        cls, adapter: SupportedAdapters, message_class: type[Message]
+        cls, adapter: SupportedAdapters, message_class: Type[Message]
     ):
         cls._message_registry[adapter] = message_class
 
     async def build(self, bot: Bot) -> Message:
         warn(DeprecationWarning("MessageFactory.build is deprecated"))
         return await self._build(bot)
 
     async def _build(self, bot: Bot) -> Message:
         adapter_name = extract_adapter_type(bot)
         if message_type := self._message_registry.get(adapter_name):
-            ms: tuple[MessageSegment] = await asyncio.gather(
+            ms: List[MessageSegment] = await asyncio.gather(
                 *[ms_factory.build(bot) for ms_factory in self]
             )
             return message_type(ms)
         raise AdapterNotInstalled(adapter_name)
 
-    def __init__(self, message: str | Iterable[TMSF] | TMSF):
+    def __init__(self, message: Union[str, Iterable[TMSF], TMSF]):
         super().__init__()
 
         if message is None:
             return
         elif isinstance(message, str):
             self.append(self.get_text_factory()(message))
         elif isinstance(message, MessageSegmentFactory):
             self.append(message)
         elif isinstance(message, Iterable):
             self.extend(message)
 
-    def __add__(self: TMF, other: str | TMSF | Iterable[TMSF]) -> TMF:
+    def __add__(self: TMF, other: Union[str, TMSF, Iterable[TMSF]]) -> TMF:
         result = self.copy()
         result += other
         return result
 
-    def __radd__(self: TMF, other: str | TMSF | Iterable[TMSF]) -> TMF:
+    def __radd__(self: TMF, other: Union[str, TMSF, Iterable[TMSF]]) -> TMF:
         result = self.__class__(other)
         return result + self
 
-    def __iadd__(self: TMF, other: str | TMSF | Iterable[TMSF]) -> TMF:
+    def __iadd__(self: TMF, other: Union[str, TMSF, Iterable[TMSF]]) -> TMF:
         if isinstance(other, str):
             self.append(self.get_text_factory()(other))
         elif isinstance(other, MessageSegmentFactory):
             self.append(other)
         elif isinstance(other, Iterable):
             self.extend(other)
 
         return self
 
-    def append(self: TMF, obj: str | TMSF) -> TMF:
+    def append(self: TMF, obj: Union[str, TMSF]) -> TMF:
         if isinstance(obj, MessageSegmentFactory):
             super().append(obj)
         elif isinstance(obj, str):
             super().append(self.get_text_factory()(obj))
 
         return self
 
-    def extend(self: TMF, obj: TMF | Iterable[TMSF]) -> TMF:
+    def extend(self: TMF, obj: Union[TMF, Iterable[TMSF]]) -> TMF:
         for message_segment_factory in obj:
             self.append(message_segment_factory)
 
         return self
 
     def copy(self: TMF) -> TMF:
         return deepcopy(self)
@@ -230,15 +237,17 @@
             bot = current_bot.get()
         except LookupError:
             raise RuntimeError("send() 仅能在事件相应器中使用，主动发送消息请使用 send_to")
 
         target = extract_target(event)
         await self._do_send(bot, target, event, at_sender, reply)
 
-    async def send_to(self, bot: Bot, target: PlatformTarget):
+    async def send_to(self, target: PlatformTarget, bot: Optional[Bot] = None):
+        if bot is None:
+            bot = get_bot(target)
         await self._do_send(bot, target, None, False, False)
 
     async def _do_send(
         self,
         bot: Bot,
         target: PlatformTarget,
         event: Optional[Event],
@@ -250,23 +259,25 @@
             raise RuntimeError(
                 f"send method for {adapter} not registerd"
             )  # pragma: no cover
         await sender(bot, self, target, event, at_sender, reply)
 
 
 AggregatedSender = Callable[
-    [Bot, list[MessageFactory], PlatformTarget, Optional[Event]], Awaitable[None]
+    [Bot, List[MessageFactory], PlatformTarget, Optional[Event]], Awaitable[None]
 ]
 
 
 class AggregatedMessageFactory:
-    message_factories: list[MessageFactory]
-    sender: ClassVar[dict[SupportedAdapters, AggregatedSender]] = {}
+    message_factories: List[MessageFactory]
+    sender: ClassVar[Dict[SupportedAdapters, AggregatedSender]] = {}
 
-    def __init__(self, msgs: list[MessageFactory | MessageSegmentFactory]) -> None:
+    def __init__(
+        self, msgs: List[Union[MessageFactory, MessageSegmentFactory]]
+    ) -> None:
         self.message_factories = []
         for msg in msgs:
             if isinstance(msg, MessageSegmentFactory):
                 self.message_factories.append(MessageFactory(msg))
             else:
                 self.message_factories.append(msg)
 
@@ -304,15 +315,17 @@
             bot = current_bot.get()
         except LookupError:
             raise RuntimeError("send() 仅能在事件相应器中使用，主动发送消息请使用 send_to")
 
         target = extract_target(event)
         await self._do_send(bot, target, event)
 
-    async def send_to(self, bot: Bot, target: PlatformTarget):
+    async def send_to(self, target: PlatformTarget, bot: Optional[Bot] = None):
+        if bot is None:
+            bot = get_bot(target)
         await self._do_send(bot, target, None)
 
 
 def register_ms_adapter(
     adapter: SupportedAdapters, ms_factory: Type[TMSF]
 ) -> Callable[[BuildFunc], BuildFunc]:
     def decorator(builder: BuildFunc) -> BuildFunc:
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/pyproject.toml` & `nonebot_plugin_send_anything_anywhere-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.poetry]
 name = "nonebot-plugin-send-anything-anywhere"
-version = "0.2.2"
+version = "0.2.4"
 description = "An adaptor for nonebot2 adaptors"
 authors = ["felinae98 <731499577@qq.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "nonebot_plugin_saa"}]
+packages = [{ include = "nonebot_plugin_saa" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
-  "License :: OSI Approved :: MIT License"
+  "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 nonebot2 = "^2.0.0rc1"
 strenum = "^0.4.8"
 pydantic = "^1.10.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.20.2"
 ipdb = "^0.13.9"
 pip = "^23.0"
 pytest-cov = "^4.0.0"
 nonebug = "^0.3.1"
-nonebot2 = {extras = ["fastapi"], version = "^2.0.0rc3"}
+nonebot2 = { extras = ["fastapi"], version = "^2.0.0rc4" }
 ruff = "^0.0.253"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.group.adapters]
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-adapter-qqguild = ">=0.2.1"
+nonebot-adapter-kaiheila = { version = "^0.2.4", python = ">=3.9" }
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
@@ -55,7 +59,11 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+
+[tool.pyright]
+pythonVersion = "3.8"
+pythonPlatform = "All"
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/setup.py` & `nonebot_plugin_send_anything_anywhere-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 install_requires = \
 ['nonebot2>=2.0.0rc1,<3.0.0',
  'pydantic>=1.10.5,<2.0.0',
  'strenum>=0.4.8,<0.5.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-send-anything-anywhere',
-    'version': '0.2.2',
+    'version': '0.2.4',
     'description': 'An adaptor for nonebot2 adaptors',
-    'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n![Codecov](https://img.shields.io/codecov/c/github/felinae98/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为 QQ 号 10000, 以私聊形式发送\ntarget = TargetQQGroup(group_id=2233)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target\n\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    target = extract_target(event)\n\n@matcher.handle()\nasync def handle(target: PlatformTarget = Depends(get_target)):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | QQ Guild |\n| :--------: | :--------: | :------: |\n|     ✅     |     ✅     |    ✅    |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | QQ Guild |\n| :--: | :--------: | :--------: | :------: |\n| 文字 |     ✅     |     ✅     |    ✅    |\n| 图片 |     ✅     |     ✅     |    ✅    |\n|  at  |     ✅     |     ✅     |    ✅    |\n| 回复 |     ✅     |     ✅     |    ✅    |\n\n### 支持的发送目标\n\n|                   | OneBot v11 | OneBot v12  | QQ Guild |\n| :---------------: | :--------: | :---------: | :------: |\n|       QQ 群       |     ✅     |     ✅      |          |\n|      QQ 私聊      |     ✅     |     ✅      |          |\n| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |\n|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\npic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
+    'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n![Codecov](https://img.shields.io/codecov/c/github/felinae98/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为 QQ 号 10000, 以私聊形式发送\ntarget = TargetQQGroup(group_id=2233)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target\n\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    target = extract_target(event)\n\n@matcher.handle()\nasync def handle(target: PlatformTarget = Depends(get_target)):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |\n| :--------: | :--------: | :------: | :------: |\n|     ✅     |     ✅     |    ✅    |    ✅    |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |\n| :--: | :--------: | :--------: | :------: | :----: |\n| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |\n| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |\n|  at  |     ✅     |     ✅     |    ✅    |   ✅   |\n| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |\n\n### 支持的发送目标\n\n|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |\n| :---------------: | :--------: | :---------: | :------: | :------: |\n|       QQ 群       |     ✅     |     ✅      |          |          |\n|      QQ 私聊      |     ✅     |     ✅      |          |          |\n| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |\n|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |\n|  开黑啦私聊/频道  |            |             |          |    ✅    |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\npic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
     'author': 'felinae98',
     'author_email': '731499577@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.2/PKG-INFO` & `nonebot_plugin_send_anything_anywhere-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-send-anything-anywhere
-Version: 0.2.2
+Version: 0.2.4
 Summary: An adaptor for nonebot2 adaptors
 License: MIT
 Author: felinae98
 Author-email: 731499577@qq.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -104,35 +108,36 @@
 
 ## 支持情况
 
 ✅:支持 ✖️:支持不了 🚧:等待适配
 
 ### 支持的 adapter
 
-| OneBot v11 | OneBot v12 | QQ Guild |
-| :--------: | :--------: | :------: |
-|     ✅     |     ✅     |    ✅    |
+| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |
+| :--------: | :--------: | :------: | :------: |
+|     ✅     |     ✅     |    ✅    |    ✅    |
 
 ### 支持的消息类型
 
-|      | OneBot v11 | OneBot v12 | QQ Guild |
-| :--: | :--------: | :--------: | :------: |
-| 文字 |     ✅     |     ✅     |    ✅    |
-| 图片 |     ✅     |     ✅     |    ✅    |
-|  at  |     ✅     |     ✅     |    ✅    |
-| 回复 |     ✅     |     ✅     |    ✅    |
+|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |
+| :--: | :--------: | :--------: | :------: | :----: |
+| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |
+| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |
+|  at  |     ✅     |     ✅     |    ✅    |   ✅   |
+| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |
 
 ### 支持的发送目标
 
-|                   | OneBot v11 | OneBot v12  | QQ Guild |
-| :---------------: | :--------: | :---------: | :------: |
-|       QQ 群       |     ✅     |     ✅      |          |
-|      QQ 私聊      |     ✅     |     ✅      |          |
-| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |
-|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |
+|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |
+| :---------------: | :--------: | :---------: | :------: | :------: |
+|       QQ 群       |     ✅     |     ✅      |          |          |
+|      QQ 私聊      |     ✅     |     ✅      |          |          |
+| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |
+|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |
+|  开黑啦私聊/频道  |            |             |          |    ✅    |
 
 注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用
 
 ## 问题与例子
 
 因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的
```

