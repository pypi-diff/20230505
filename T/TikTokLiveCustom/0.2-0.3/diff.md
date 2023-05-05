# Comparing `tmp/TikTokLiveCustom-0.2-py3.9.egg` & `tmp/TikTokLiveCustom-0.3-py3.9.egg`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 38798 bytes, number of entries: 22
--rw-r--r--  2.0 unx    29109 b- defN 23-May-01 11:39 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      679 b- defN 23-May-01 11:39 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-01 11:39 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx      113 b- defN 23-May-01 11:39 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-01 11:39 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-01 11:39 EGG-INFO/zip-safe
+Zip file size: 37583 bytes, number of entries: 22
+-rw-r--r--  2.0 unx    30857 b- defN 23-May-05 20:19 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      679 b- defN 23-May-05 20:19 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 20:19 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx      113 b- defN 23-May-05 20:19 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 20:19 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 20:19 EGG-INFO/zip-safe
 -rw-r--r--  2.0 unx       44 b- defN 23-Feb-21 22:39 TikTokLive/__init__.py
 -rw-r--r--  2.0 unx     1355 b- defN 23-Feb-21 22:39 TikTokLive/utilities.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-21 22:39 TikTokLive/client/__init__.py
--rw-r--r--  2.0 unx    21647 b- defN 23-May-01 10:47 TikTokLive/client/base.py
--rw-r--r--  2.0 unx     7324 b- defN 23-May-01 10:36 TikTokLive/client/client.py
+-rw-r--r--  2.0 unx    21654 b- defN 23-May-04 19:49 TikTokLive/client/base.py
+-rw-r--r--  2.0 unx     7425 b- defN 23-May-04 19:42 TikTokLive/client/client.py
 -rw-r--r--  2.0 unx     2024 b- defN 23-Feb-21 22:39 TikTokLive/client/config.py
--rw-r--r--  2.0 unx    10081 b- defN 23-May-01 10:36 TikTokLive/client/httpx.py
+-rw-r--r--  2.0 unx    10081 b- defN 23-May-04 19:50 TikTokLive/client/httpx.py
 -rw-r--r--  2.0 unx     4724 b- defN 23-Feb-21 22:39 TikTokLive/client/wsclient.py
 -rw-r--r--  2.0 unx       50 b- defN 23-Feb-21 22:39 TikTokLive/proto/__init__.py
--rw-r--r--  2.0 unx    41517 b- defN 23-Mar-14 22:36 TikTokLive/proto/tiktok_schema_pb2.py
--rw-r--r--  2.0 unx     2964 b- defN 23-May-01 10:36 TikTokLive/proto/utilities.py
+-rw-r--r--  2.0 unx    19933 b- defN 23-May-04 19:42 TikTokLive/proto/tiktok_schema_pb2.py
+-rw-r--r--  2.0 unx     3006 b- defN 23-May-04 19:42 TikTokLive/proto/utilities.py
 -rw-r--r--  2.0 unx       44 b- defN 23-Feb-21 22:39 TikTokLive/types/__init__.py
 -rw-r--r--  2.0 unx     3362 b- defN 23-Feb-21 22:39 TikTokLive/types/errors.py
--rw-r--r--  2.0 unx    14837 b- defN 23-Mar-14 22:36 TikTokLive/types/events.py
--rw-r--r--  2.0 unx    14797 b- defN 23-May-01 10:36 TikTokLive/types/objects.py
+-rw-r--r--  2.0 unx    16163 b- defN 23-May-04 19:42 TikTokLive/types/events.py
+-rw-r--r--  2.0 unx    15021 b- defN 23-May-04 19:42 TikTokLive/types/objects.py
 -rw-r--r--  2.0 unx     1023 b- defN 23-Feb-21 22:39 TikTokLive/types/utilities.py
-22 files, 155707 bytes uncompressed, 35976 bytes compressed:  76.9%
+22 files, 137571 bytes uncompressed, 34761 bytes compressed:  74.7%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TikTokLiveCustom
-Version: 0.2
+Version: 0.3
 Summary: TikTok Live Connection Client
 Home-page: https://github.com/robinyang0909/TikTokLive
 Author: robinyang
 Author-email: robinyang_beijing@163.com
 License: MIT
 Keywords: tiktok,tiktok live,python3,api,unofficial
 Classifier: Development Status :: 4 - Beta
@@ -121,34 +121,34 @@
 
 ## Params & Options
 
 To create a new `TikTokLiveClient` object the following parameter is required. You can optionally add configuration options to this via kwargs.
 
 `TikTokLiveClient(unique_id, **options)`
 
-| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-|------------|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
-| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer. |
+| Param Name | Required | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+|------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| unique_id  | Yes      | The unique username of the broadcaster. You can find this name in the URL.<br>Example: `https://www.tiktok.com/@isaackogz` => `isaackogz`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| **options  | No       | Here you can set the following optional connection properties. If you do not specify a value, the default value will be used.<br><br>`process_initial_data` (default: `True`) <br> Define if you want to process initial data upon connecting (e.g. first 1-10 messages from BEFORE you connected).<br><br>`fetch_room_info_on_connect` (default: `True`) <br> Define if you want to fetch all room information on start. If this option is enabled, connection to offline rooms will be prevented. If enabled, the connect result contains the room info via the `room_info` attribute. You can also manually retrieve the room info (even in an unconnected state) using the `retrieve_room_info()` method.<br><br>`enable_detailed_gifts` (default: `False`) <br> Define if you want to receive extended information about gifts like gift name, cost and images which you can retrieve via the `available_gifts` attribute. When enabled, the `details` attribute in a `Gift` object will be populated.<br><br>`ws_ping_interval` (default: `10.0`) <br> The interval between keepalive pings on the websocket connection (in seconds).<br><br>`ws_timeout` (default: `10.0`)<br>How long to wait before the websocket connection is considered timed out (in seconds).<br><br>`http_timeout` (default: `10.0`) <br> How long to wait before considering an HTTP request in the http client timed out (in seconds).<br><br>`http_headers` (default: `{}`) <br> Additional HTTP client headers to include when making requests to the Webcast API AND connecting to the websocket server.<br><br>`http_params` (default: `{}`) <br>Additional HTTP client parameters to include when making requests to the Webcast API AND connecting to the websocket.<br><br>`loop` (default: `None`)<br>Optionally supply your own asyncio event loop for usage by the client. When set to None, the client pulls the current active loop or creates a new one. This option is mostly useful for people trying to nest asyncio.<br/><br/>`trust_env` (default: `False`)<br/>Whether to trust environment variables that provide proxies in httpx requests<br/><br/>`proxies` (default: `None`)<br/>Enable proxied requests by turning on forwarding for the HTTP "proxies" argument. Websocket connections will NOT be proxied<br/><br/>`lang` (default: `en-US`)<br/>Change the language. Payloads *will* be in English, but front-end content will be in the desired language!<br/><br/>`sign_api_key` (default: `None`)<br/>Parameter to increase the amount of connections allowed to be made per minute via a Sign Server API key. If you need this, contact the project maintainer.<br/><br/>`ssl_context` (default: `None`)<br/>Providing an SSLContext object overrides the default context used in HTTP requests made to TikTok. This is useful if TikTok sends invalid SSL signatures, as you can provide a "no verify" context. |
 
 
 ## Methods
 
 A `TikTokLiveClient` object contains the following methods:
 
-| Method Name              | Description                                                                                                                                                                       |
-|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                               |
-| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                |
-| stop                     | Turns off the connection to the live chat.                                                                                                                                        |
-| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                |
-| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                 |
-| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent ||
-| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method                                                                       |
-| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                         |
+| Method Name              | Description                                                                                                                                                                                                                   |
+|--------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| run                      | Starts a connection to the live chat while blocking the main thread                                                                                                                                                           |
+| start                    | (async) Connects to the live chat without blocking the main thread                                                                                                                                                            |
+| stop                     | Turns off the connection to the live chat.                                                                                                                                                                                    |
+| retrieve_room_info       | (async) Gets the current room info from TikTok API                                                                                                                                                                            |
+| retrieve_available_gifts | (async) Retrieves a list of the available gifts for the room and adds it to the `extended_gift` attribute of the `Gift` object on the `gift` event, when enabled.                                                             |
+| add_listener             | Adds an *asynchronous* listener function (or, you can decorate a function with `@client.on("<event>")`) and takes two parameters, an event name and the payload, an AbstractEvent                                             ||
+| download                 | Start downloading the livestream video for a given duration or until stopped via the `stop_download` method. Supports the ability to add different flags, like `-c copy` which may reduce CPU usage by disabling transcoding. |
+| stop_download            | Stop downloading the livestream video if currently downloading, otherwise throws an error                                                                                                                                     |
 
 ## Attributes
 
 A `TikTokLiveClient` object contains the following attributes:
 
 | Attribute Name  | Description                                                                                                                                  |
 |-----------------|----------------------------------------------------------------------------------------------------------------------------------------------|
@@ -319,22 +319,32 @@
 
 ```python
 @client.on("envelope")
 async def on_connect(event: EnvelopeEvent):
     print(f"{event.treasure_box_user.unique_id} -> {event.treasure_box_data}")
 ```
 
-### `weekly_ranking`
+### `ranking_update`
 
-Triggered when a weekly ranking update is sent out.
+Triggered when a **stream** rank update is sent out. Can be `Weekly Ranking` or `Rising Star`!
 
 ```python
-@client.on("weekly_ranking")
-async def on_connect(event: WeeklyRankingEvent):
-    print(f"{client.unique_id} has the rank #{event.data.rank} of all streamers!")
+@client.on("ranking_update")
+async def on_connect(event: RankingUpdateEvent):
+    print(f"{event.user.unique_id} has the rank #{event.rank} for the {event.type} leaderboard.")
+```
+
+### `user_ranking_update`
+
+Triggered when a **user** rank update is sent out. Can be `Top Viewer`
+ status.
+```python
+@client.on("user_ranking_update")
+async def on_connect(event: UserRankingUpdateEvent):
+    print(f"{event.user.unique_id} just became a #{event.rank} top viewer!")
 ```
 
 ### `mic_battle_start`
 
 Triggered when a Mic Battle starts!
 
 ```python
```

## TikTokLive/client/base.py

```diff
@@ -27,15 +27,15 @@
     Base client responsible for long polling to the TikTok Webcast API
 
     """
 
     def __init__(
             self,
             unique_id: str,
-            final_room_id: str,
+            final_room_id: str = None,
             loop: Optional[AbstractEventLoop] = None,
             http_params: Optional[dict] = None,
             http_headers: Optional[dict] = None,
             http_timeout: float = 10.0,
             ws_timeout: float = 10.0,
             ws_ping_interval: float = 10.0,
             ws_headers: Optional[dict] = None,
```

## TikTokLive/client/client.py

```diff
@@ -2,16 +2,18 @@
 import traceback
 from typing import Optional, List
 
 from pyee import AsyncIOEventEmitter
 
 from .base import WebcastPushConnection
 from ..types import FailedParseMessage, TopViewer
-from ..types.events import AbstractEvent, ConnectEvent, DisconnectEvent, ViewerUpdateEvent, JoinEvent, LikeEvent, FollowEvent, ShareEvent, QuestionEvent, LiveEndEvent, \
-    IntroMessageEvent, EmoteEvent, MicBattleStartEvent, MicBattleUpdateEvent, MoreShareEvent, UnknownEvent, WeeklyRankingEvent, CommentEvent, GiftEvent
+from ..types.events import AbstractEvent, ConnectEvent, DisconnectEvent, ViewerUpdateEvent, JoinEvent, LikeEvent, \
+    FollowEvent, ShareEvent, QuestionEvent, LiveEndEvent, \
+    IntroMessageEvent, EmoteEvent, MicBattleStartEvent, MicBattleUpdateEvent, MoreShareEvent, UnknownEvent, \
+    CommentEvent, GiftEvent, RankingUpdateEvent, UserRankingUpdateEvent
 
 
 class TikTokLiveClient(WebcastPushConnection, AsyncIOEventEmitter):
     """
     TikTokLive Client responsible for emitting events asynchronously
 
     """
@@ -160,22 +162,22 @@
         mapping: Optional[AbstractEvent] = (
             {
                 "WebcastGiftMessage": GiftEvent,
                 "WebcastChatMessage": CommentEvent,
                 "WebcastRoomUserSeqMessage": ViewerUpdateEvent,
                 "WebcastMemberMessage": JoinEvent,
                 "WebcastLikeMessage": LikeEvent,
-                "WebcastRankUpdateMessage": WeeklyRankingEvent,
-                "WebcastHourlyRankMessage": WeeklyRankingEvent,
+                "WebcastRankUpdateMessage": RankingUpdateEvent,
+                "WebcastHourlyRankMessage": RankingUpdateEvent,
                 "WebcastQuestionNewMessage": QuestionEvent,
                 "WebcastLiveIntroMessage": IntroMessageEvent,
                 "WebcastEmoteChatMessage": EmoteEvent,
                 "WebcastLinkMicBattle": MicBattleStartEvent,
-                "WebcastLinkMicArmies": MicBattleUpdateEvent
-
+                "WebcastLinkMicArmies": MicBattleUpdateEvent,
+                "WebcastRankTextMessage": UserRankingUpdateEvent
             }.get(webcast_message.get('type'))
         )
 
         # Sometimes, we need to use the display_type attribute
         mapping: Optional[AbstractEvent] = mapping or (
             {
                 "pm_main_follow_message_viewer_2": FollowEvent,
```

## TikTokLive/proto/tiktok_schema_pb2.py

```diff
@@ -1,615 +1,148 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tiktok_schema.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13tiktok_schema.proto\x12\x06TikTok\"C\n\x17WebcastWebsocketMessage\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06\x62inary\x18\x08 \x01(\x0c\"/\n\x13WebcastWebsocketAck\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0c\n\x04type\x18\x07 \x01(\t\"\xf8\x02\n\x0fWebcastResponse\x12\x31\n\x08messages\x18\x01 \x03(\x0b\x32\x1f.TikTok.WebcastResponse.Message\x12\x0e\n\x06\x63ursor\x18\x02 \x01(\t\x12\x15\n\rfetchInterval\x18\x03 \x01(\x05\x12\x17\n\x0fserverTimestamp\x18\x04 \x01(\x03\x12\x13\n\x0binternalExt\x18\x05 \x01(\t\x12\x11\n\tfetchType\x18\x06 \x01(\x05\x12\x37\n\x07wsParam\x18\x07 \x01(\x0b\x32&.TikTok.WebcastResponse.WebsocketParam\x12\x19\n\x11heartbeatDuration\x18\x08 \x01(\x05\x12\x0f\n\x07needAck\x18\t \x01(\x08\x12\r\n\x05wsUrl\x18\n \x01(\t\x1a\'\n\x07Message\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x62inary\x18\x02 \x01(\x0c\x1a-\n\x0eWebsocketParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\"\n\x0bRoomMessage\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"\'\n\x15WebcastControlMessage\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\"\xbf\x01\n\x19WebcastRoomUserSeqMessage\x12@\n\x0btop_viewers\x18\x02 \x03(\x0b\x32+.TikTok.WebcastRoomUserSeqMessage.TopViewer\x12\x14\n\x0cviewer_count\x18\x03 \x01(\x05\x1aJ\n\tTopViewer\x12\x13\n\x0b\x63oins_given\x18\x01 \x01(\r\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x0c\n\x04rank\x18\x03 \x01(\r\"\xc3\x02\n\x12WebcastChatMessage\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x0f\n\x07\x63omment\x18\x03 \x01(\t\x12\x1e\n\x08mentions\x18\x0c \x03(\x0b\x32\x0c.TikTok.User\x12\x34\n\x06images\x18\r \x03(\x0b\x32$.TikTok.WebcastChatMessage.ChatImage\x12\x10\n\x08language\x18\x0e \x01(\t\x1a\x97\x01\n\tChatImage\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x42\n\x05image\x18\x02 \x01(\x0b\x32\x33.TikTok.WebcastChatMessage.ChatImage.ChatImageImage\x1a\x34\n\x0e\x43hatImageImage\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.TikTok.TikTokImage\"\x82\x01\n\x14WebcastMemberMessage\x12*\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x1b.TikTok.WebcastMessageEvent\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x0f\n\x07viewers\x18\x03 \x01(\x05\x12\x11\n\taction_id\x18\n \x01(\x05\"\xd2\x03\n\x12WebcastGiftMessage\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x13\n\x0brepeatCount\x18\x05 \x01(\x05\x12\x1a\n\x04user\x18\x07 \x01(\x0b\x32\x0c.TikTok.User\x12\x11\n\trepeatEnd\x18\t \x01(\x05\x12\x45\n\x04info\x18\x0f \x01(\x0b\x32\x37.TikTok.WebcastGiftMessage.WebcastGiftMessageGiftDetail\x12I\n\trecipient\x18\x17 \x01(\x0b\x32\x36.TikTok.WebcastGiftMessage.WebcastGiftMessageRecipient\x1a\x41\n\x1bWebcastGiftMessageRecipient\x12\x11\n\ttimestamp\x18\x06 \x01(\x04\x12\x0f\n\x07user_id\x18\x08 \x01(\x04\x1a\x96\x01\n\x1cWebcastGiftMessageGiftDetail\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.TikTok.TikTokImage\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\n\n\x02id\x18\x05 \x01(\x05\x12\x0c\n\x04type\x18\x0b \x01(\x05\x12\x15\n\rdiamond_count\x18\x0c \x01(\x05\"\xd6\x03\n\x14WebcastLinkMicBattle\x12K\n\x0b\x62\x61ttleUsers\x18\n \x03(\x0b\x32\x36.TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems\x1a\xf0\x02\n\x19WebcastLinkMicBattleItems\x12\x65\n\x0b\x62\x61ttleGroup\x18\x02 \x01(\x0b\x32P.TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup\x1a\xeb\x01\n\x19WebcastLinkMicBattleGroup\x12g\n\x04user\x18\x01 \x01(\x0b\x32Y.TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup.LinkUser\x1a\x65\n\x08LinkUser\x12\x0f\n\x07user_id\x18\x01 \x01(\x04\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12#\n\x06\x61vatar\x18\x03 \x01(\x0b\x32\x13.TikTok.TikTokImage\x12\x11\n\tunique_id\x18\x04 \x01(\t\"\xdd\x02\n\x14WebcastLinkMicArmies\x12K\n\x0b\x62\x61ttleItems\x18\x03 \x03(\x0b\x32\x36.TikTok.WebcastLinkMicArmies.WebcastLinkMicArmiesItems\x12\x14\n\x0c\x62\x61ttleStatus\x18\x07 \x01(\x05\x1a\xe1\x01\n\x19WebcastLinkMicArmiesItems\x12\x12\n\nhostUserId\x18\x01 \x01(\x04\x12\x66\n\x0c\x62\x61ttleGroups\x18\x02 \x03(\x0b\x32P.TikTok.WebcastLinkMicArmies.WebcastLinkMicArmiesItems.WebcastLinkMicArmiesGroup\x1aH\n\x19WebcastLinkMicArmiesGroup\x12\x1b\n\x05users\x18\x01 \x03(\x0b\x32\x0c.TikTok.User\x12\x0e\n\x06points\x18\x02 \x01(\x05\"w\n\x14WebcastSocialMessage\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x17\n\x0ftotal_followers\x18\x06 \x01(\r\x12*\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x1b.TikTok.WebcastMessageEvent\"\x80\x01\n\x12WebcastLikeMessage\x12\x1a\n\x04user\x18\x05 \x01(\x0b\x32\x0c.TikTok.User\x12*\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x1b.TikTok.WebcastMessageEvent\x12\r\n\x05likes\x18\x02 \x01(\x05\x12\x13\n\x0btotal_likes\x18\x03 \x01(\x05\"\xa8\x01\n\x19WebcastQuestionNewMessage\x12J\n\x0fquestionDetails\x18\x02 \x01(\x0b\x32\x31.TikTok.WebcastQuestionNewMessage.QuestionDetails\x1a?\n\x0fQuestionDetails\x12\x10\n\x08question\x18\x02 \x01(\t\x12\x1a\n\x04user\x18\x05 \x01(\x0b\x32\x0c.TikTok.User\"m\n\x17WebcastLiveIntroMessage\x12\x0f\n\x07room_id\x18\x02 \x01(\x04\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x1e\n\x08streamer\x18\x05 \x01(\x0b\x32\x0c.TikTok.User\x12\x10\n\x08language\x18\x08 \x01(\t\"$\n\rSystemMessage\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"*\n\x1aWebcastInRoomBannerMessage\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\x92\x01\n\x18WebcastRankUpdateMessage\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..TikTok.WebcastRankUpdateMessage.RankContainer\x1a\x38\n\rRankContainer\x12\'\n\x08rankings\x18\x03 \x01(\x0b\x32\x15.TikTok.WeeklyRanking\"\x9e\x01\n\x18WebcastHourlyRankMessage\x12\x42\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x34.TikTok.WebcastHourlyRankMessage.HourlyRankContainer\x1a>\n\x13HourlyRankContainer\x12\'\n\x08rankings\x18\x04 \x01(\x0b\x32\x15.TikTok.WeeklyRanking\"\xf8\x01\n\x17WebcastEmoteChatMessage\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12;\n\x05\x65mote\x18\x03 \x01(\x0b\x32,.TikTok.WebcastEmoteChatMessage.EmoteDetails\x1a\x83\x01\n\x0c\x45moteDetails\x12\x10\n\x08\x65mote_id\x18\x01 \x01(\t\x12\x46\n\x05image\x18\x02 \x01(\x0b\x32\x37.TikTok.WebcastEmoteChatMessage.EmoteDetails.EmoteImage\x1a\x19\n\nEmoteImage\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x82\x05\n\x16WebcastEnvelopeMessage\x12G\n\x0ftreasureBoxData\x18\x02 \x01(\x0b\x32..TikTok.WebcastEnvelopeMessage.TreasureBoxData\x12G\n\x0ftreasureBoxUser\x18\x01 \x01(\x0b\x32..TikTok.WebcastEnvelopeMessage.TreasureBoxUser\x1a\x8e\x03\n\x0fTreasureBoxUser\x12N\n\x05user2\x18\x08 \x01(\x0b\x32?.TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2\x1a\xaa\x02\n\x10TreasureBoxUser2\x12_\n\x05user3\x18\x04 \x03(\x0b\x32P.TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3\x1a\xb4\x01\n\x10TreasureBoxUser3\x12p\n\x05user4\x18\x15 \x01(\x0b\x32\x61.TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3.TreasureBoxUser4\x1a.\n\x10TreasureBoxUser4\x12\x1a\n\x04user\x18\x01 \x01(\x0b\x32\x0c.TikTok.User\x1a\x45\n\x0fTreasureBoxData\x12\r\n\x05\x63oins\x18\x05 \x01(\r\x12\x10\n\x08openable\x18\x06 \x01(\r\x12\x11\n\ttimestamp\x18\x07 \x01(\x04\"(\n\x0bTikTokImage\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\"\xa1\x01\n\x13WebcastMessageEvent\x12G\n\x07\x64\x65tails\x18\x08 \x01(\x0b\x32\x36.TikTok.WebcastMessageEvent.WebcastMessageEventDetails\x1a\x41\n\x1aWebcastMessageEventDetails\x12\x14\n\x0c\x64isplay_type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\"\xcf\x05\n\x04User\x12\x0f\n\x07user_id\x18\x01 \x01(\x04\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12#\n\x06\x61vatar\x18\t \x01(\x0b\x32\x13.TikTok.TikTokImage\x12#\n\x04info\x18\x16 \x01(\x0b\x32\x15.TikTok.User.UserInfo\x12\x11\n\tunique_id\x18& \x01(\t\x12\x0f\n\x07sec_uid\x18. \x01(\t\x12&\n\x06\x62\x61\x64ges\x18@ \x03(\x0b\x32\x16.TikTok.User.UserBadge\x1a\x45\n\x08UserInfo\x12\x11\n\tfollowing\x18\x01 \x01(\x05\x12\x11\n\tfollowers\x18\x02 \x01(\x05\x12\x13\n\x0b\x66ollow_role\x18\x03 \x01(\x05\x1a\xc6\x03\n\tUserBadge\x12\x18\n\x10\x62\x61\x64ge_scene_type\x18\x03 \x01(\x05\x12.\n\x04text\x18\x15 \x01(\x0b\x32 .TikTok.User.UserBadge.BadgeText\x12\x30\n\x05image\x18\x14 \x01(\x0b\x32!.TikTok.User.UserBadge.BadgeImage\x12\x34\n\x07\x63omplex\x18\x17 \x01(\x0b\x32#.TikTok.User.UserBadge.BadgeComplex\x1a(\n\tBadgeText\x12\r\n\x05label\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x1a\x30\n\nBadgeImage\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.TikTok.TikTokImage\x1a\xaa\x01\n\x0c\x42\x61\x64geComplex\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.TikTok.TikTokImage\x12=\n\x05label\x18\x03 \x01(\x0b\x32..TikTok.User.UserBadge.BadgeComplex.BadgeLabel\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x1a)\n\nBadgeLabel\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd5\x01\n\rWeeklyRanking\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12,\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x1e.TikTok.WeeklyRanking.RankData\x12\x32\n\x05\x65xtra\x18\x03 \x01(\x0b\x32#.TikTok.WeeklyRanking.ExtraRankData\x1a\x18\n\x08RankData\x12\x0c\n\x04rank\x18\x0b \x01(\t\x1a+\n\rExtraRankData\x12\x0e\n\x06\x63olour\x18\x01 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x04\x62\x06proto3')
-
-
-
-_WEBCASTWEBSOCKETMESSAGE = DESCRIPTOR.message_types_by_name['WebcastWebsocketMessage']
-_WEBCASTWEBSOCKETACK = DESCRIPTOR.message_types_by_name['WebcastWebsocketAck']
-_WEBCASTRESPONSE = DESCRIPTOR.message_types_by_name['WebcastResponse']
-_WEBCASTRESPONSE_MESSAGE = _WEBCASTRESPONSE.nested_types_by_name['Message']
-_WEBCASTRESPONSE_WEBSOCKETPARAM = _WEBCASTRESPONSE.nested_types_by_name['WebsocketParam']
-_ROOMMESSAGE = DESCRIPTOR.message_types_by_name['RoomMessage']
-_WEBCASTCONTROLMESSAGE = DESCRIPTOR.message_types_by_name['WebcastControlMessage']
-_WEBCASTROOMUSERSEQMESSAGE = DESCRIPTOR.message_types_by_name['WebcastRoomUserSeqMessage']
-_WEBCASTROOMUSERSEQMESSAGE_TOPVIEWER = _WEBCASTROOMUSERSEQMESSAGE.nested_types_by_name['TopViewer']
-_WEBCASTCHATMESSAGE = DESCRIPTOR.message_types_by_name['WebcastChatMessage']
-_WEBCASTCHATMESSAGE_CHATIMAGE = _WEBCASTCHATMESSAGE.nested_types_by_name['ChatImage']
-_WEBCASTCHATMESSAGE_CHATIMAGE_CHATIMAGEIMAGE = _WEBCASTCHATMESSAGE_CHATIMAGE.nested_types_by_name['ChatImageImage']
-_WEBCASTMEMBERMESSAGE = DESCRIPTOR.message_types_by_name['WebcastMemberMessage']
-_WEBCASTGIFTMESSAGE = DESCRIPTOR.message_types_by_name['WebcastGiftMessage']
-_WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGERECIPIENT = _WEBCASTGIFTMESSAGE.nested_types_by_name['WebcastGiftMessageRecipient']
-_WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGEGIFTDETAIL = _WEBCASTGIFTMESSAGE.nested_types_by_name['WebcastGiftMessageGiftDetail']
-_WEBCASTLINKMICBATTLE = DESCRIPTOR.message_types_by_name['WebcastLinkMicBattle']
-_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS = _WEBCASTLINKMICBATTLE.nested_types_by_name['WebcastLinkMicBattleItems']
-_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP = _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS.nested_types_by_name['WebcastLinkMicBattleGroup']
-_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP_LINKUSER = _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP.nested_types_by_name['LinkUser']
-_WEBCASTLINKMICARMIES = DESCRIPTOR.message_types_by_name['WebcastLinkMicArmies']
-_WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS = _WEBCASTLINKMICARMIES.nested_types_by_name['WebcastLinkMicArmiesItems']
-_WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS_WEBCASTLINKMICARMIESGROUP = _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS.nested_types_by_name['WebcastLinkMicArmiesGroup']
-_WEBCASTSOCIALMESSAGE = DESCRIPTOR.message_types_by_name['WebcastSocialMessage']
-_WEBCASTLIKEMESSAGE = DESCRIPTOR.message_types_by_name['WebcastLikeMessage']
-_WEBCASTQUESTIONNEWMESSAGE = DESCRIPTOR.message_types_by_name['WebcastQuestionNewMessage']
-_WEBCASTQUESTIONNEWMESSAGE_QUESTIONDETAILS = _WEBCASTQUESTIONNEWMESSAGE.nested_types_by_name['QuestionDetails']
-_WEBCASTLIVEINTROMESSAGE = DESCRIPTOR.message_types_by_name['WebcastLiveIntroMessage']
-_SYSTEMMESSAGE = DESCRIPTOR.message_types_by_name['SystemMessage']
-_WEBCASTINROOMBANNERMESSAGE = DESCRIPTOR.message_types_by_name['WebcastInRoomBannerMessage']
-_WEBCASTRANKUPDATEMESSAGE = DESCRIPTOR.message_types_by_name['WebcastRankUpdateMessage']
-_WEBCASTRANKUPDATEMESSAGE_RANKCONTAINER = _WEBCASTRANKUPDATEMESSAGE.nested_types_by_name['RankContainer']
-_WEBCASTHOURLYRANKMESSAGE = DESCRIPTOR.message_types_by_name['WebcastHourlyRankMessage']
-_WEBCASTHOURLYRANKMESSAGE_HOURLYRANKCONTAINER = _WEBCASTHOURLYRANKMESSAGE.nested_types_by_name['HourlyRankContainer']
-_WEBCASTEMOTECHATMESSAGE = DESCRIPTOR.message_types_by_name['WebcastEmoteChatMessage']
-_WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS = _WEBCASTEMOTECHATMESSAGE.nested_types_by_name['EmoteDetails']
-_WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS_EMOTEIMAGE = _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS.nested_types_by_name['EmoteImage']
-_WEBCASTENVELOPEMESSAGE = DESCRIPTOR.message_types_by_name['WebcastEnvelopeMessage']
-_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER = _WEBCASTENVELOPEMESSAGE.nested_types_by_name['TreasureBoxUser']
-_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2 = _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER.nested_types_by_name['TreasureBoxUser2']
-_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3 = _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2.nested_types_by_name['TreasureBoxUser3']
-_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3_TREASUREBOXUSER4 = _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3.nested_types_by_name['TreasureBoxUser4']
-_WEBCASTENVELOPEMESSAGE_TREASUREBOXDATA = _WEBCASTENVELOPEMESSAGE.nested_types_by_name['TreasureBoxData']
-_TIKTOKIMAGE = DESCRIPTOR.message_types_by_name['TikTokImage']
-_WEBCASTMESSAGEEVENT = DESCRIPTOR.message_types_by_name['WebcastMessageEvent']
-_WEBCASTMESSAGEEVENT_WEBCASTMESSAGEEVENTDETAILS = _WEBCASTMESSAGEEVENT.nested_types_by_name['WebcastMessageEventDetails']
-_USER = DESCRIPTOR.message_types_by_name['User']
-_USER_USERINFO = _USER.nested_types_by_name['UserInfo']
-_USER_USERBADGE = _USER.nested_types_by_name['UserBadge']
-_USER_USERBADGE_BADGETEXT = _USER_USERBADGE.nested_types_by_name['BadgeText']
-_USER_USERBADGE_BADGEIMAGE = _USER_USERBADGE.nested_types_by_name['BadgeImage']
-_USER_USERBADGE_BADGECOMPLEX = _USER_USERBADGE.nested_types_by_name['BadgeComplex']
-_USER_USERBADGE_BADGECOMPLEX_BADGELABEL = _USER_USERBADGE_BADGECOMPLEX.nested_types_by_name['BadgeLabel']
-_WEEKLYRANKING = DESCRIPTOR.message_types_by_name['WeeklyRanking']
-_WEEKLYRANKING_RANKDATA = _WEEKLYRANKING.nested_types_by_name['RankData']
-_WEEKLYRANKING_EXTRARANKDATA = _WEEKLYRANKING.nested_types_by_name['ExtraRankData']
-WebcastWebsocketMessage = _reflection.GeneratedProtocolMessageType('WebcastWebsocketMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTWEBSOCKETMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastWebsocketMessage)
-  })
-_sym_db.RegisterMessage(WebcastWebsocketMessage)
-
-WebcastWebsocketAck = _reflection.GeneratedProtocolMessageType('WebcastWebsocketAck', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTWEBSOCKETACK,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastWebsocketAck)
-  })
-_sym_db.RegisterMessage(WebcastWebsocketAck)
-
-WebcastResponse = _reflection.GeneratedProtocolMessageType('WebcastResponse', (_message.Message,), {
-
-  'Message' : _reflection.GeneratedProtocolMessageType('Message', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTRESPONSE_MESSAGE,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastResponse.Message)
-    })
-  ,
-
-  'WebsocketParam' : _reflection.GeneratedProtocolMessageType('WebsocketParam', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTRESPONSE_WEBSOCKETPARAM,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastResponse.WebsocketParam)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTRESPONSE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastResponse)
-  })
-_sym_db.RegisterMessage(WebcastResponse)
-_sym_db.RegisterMessage(WebcastResponse.Message)
-_sym_db.RegisterMessage(WebcastResponse.WebsocketParam)
-
-RoomMessage = _reflection.GeneratedProtocolMessageType('RoomMessage', (_message.Message,), {
-  'DESCRIPTOR' : _ROOMMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.RoomMessage)
-  })
-_sym_db.RegisterMessage(RoomMessage)
-
-WebcastControlMessage = _reflection.GeneratedProtocolMessageType('WebcastControlMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTCONTROLMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastControlMessage)
-  })
-_sym_db.RegisterMessage(WebcastControlMessage)
-
-WebcastRoomUserSeqMessage = _reflection.GeneratedProtocolMessageType('WebcastRoomUserSeqMessage', (_message.Message,), {
-
-  'TopViewer' : _reflection.GeneratedProtocolMessageType('TopViewer', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTROOMUSERSEQMESSAGE_TOPVIEWER,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastRoomUserSeqMessage.TopViewer)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTROOMUSERSEQMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastRoomUserSeqMessage)
-  })
-_sym_db.RegisterMessage(WebcastRoomUserSeqMessage)
-_sym_db.RegisterMessage(WebcastRoomUserSeqMessage.TopViewer)
-
-WebcastChatMessage = _reflection.GeneratedProtocolMessageType('WebcastChatMessage', (_message.Message,), {
-
-  'ChatImage' : _reflection.GeneratedProtocolMessageType('ChatImage', (_message.Message,), {
-
-    'ChatImageImage' : _reflection.GeneratedProtocolMessageType('ChatImageImage', (_message.Message,), {
-      'DESCRIPTOR' : _WEBCASTCHATMESSAGE_CHATIMAGE_CHATIMAGEIMAGE,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.WebcastChatMessage.ChatImage.ChatImageImage)
-      })
-    ,
-    'DESCRIPTOR' : _WEBCASTCHATMESSAGE_CHATIMAGE,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastChatMessage.ChatImage)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTCHATMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastChatMessage)
-  })
-_sym_db.RegisterMessage(WebcastChatMessage)
-_sym_db.RegisterMessage(WebcastChatMessage.ChatImage)
-_sym_db.RegisterMessage(WebcastChatMessage.ChatImage.ChatImageImage)
-
-WebcastMemberMessage = _reflection.GeneratedProtocolMessageType('WebcastMemberMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTMEMBERMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastMemberMessage)
-  })
-_sym_db.RegisterMessage(WebcastMemberMessage)
-
-WebcastGiftMessage = _reflection.GeneratedProtocolMessageType('WebcastGiftMessage', (_message.Message,), {
-
-  'WebcastGiftMessageRecipient' : _reflection.GeneratedProtocolMessageType('WebcastGiftMessageRecipient', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGERECIPIENT,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastGiftMessage.WebcastGiftMessageRecipient)
-    })
-  ,
-
-  'WebcastGiftMessageGiftDetail' : _reflection.GeneratedProtocolMessageType('WebcastGiftMessageGiftDetail', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGEGIFTDETAIL,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastGiftMessage.WebcastGiftMessageGiftDetail)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTGIFTMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastGiftMessage)
-  })
-_sym_db.RegisterMessage(WebcastGiftMessage)
-_sym_db.RegisterMessage(WebcastGiftMessage.WebcastGiftMessageRecipient)
-_sym_db.RegisterMessage(WebcastGiftMessage.WebcastGiftMessageGiftDetail)
-
-WebcastLinkMicBattle = _reflection.GeneratedProtocolMessageType('WebcastLinkMicBattle', (_message.Message,), {
-
-  'WebcastLinkMicBattleItems' : _reflection.GeneratedProtocolMessageType('WebcastLinkMicBattleItems', (_message.Message,), {
-
-    'WebcastLinkMicBattleGroup' : _reflection.GeneratedProtocolMessageType('WebcastLinkMicBattleGroup', (_message.Message,), {
-
-      'LinkUser' : _reflection.GeneratedProtocolMessageType('LinkUser', (_message.Message,), {
-        'DESCRIPTOR' : _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP_LINKUSER,
-        '__module__' : 'tiktok_schema_pb2'
-        # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup.LinkUser)
-        })
-      ,
-      'DESCRIPTOR' : _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup)
-      })
-    ,
-    'DESCRIPTOR' : _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTLINKMICBATTLE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicBattle)
-  })
-_sym_db.RegisterMessage(WebcastLinkMicBattle)
-_sym_db.RegisterMessage(WebcastLinkMicBattle.WebcastLinkMicBattleItems)
-_sym_db.RegisterMessage(WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup)
-_sym_db.RegisterMessage(WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup.LinkUser)
-
-WebcastLinkMicArmies = _reflection.GeneratedProtocolMessageType('WebcastLinkMicArmies', (_message.Message,), {
-
-  'WebcastLinkMicArmiesItems' : _reflection.GeneratedProtocolMessageType('WebcastLinkMicArmiesItems', (_message.Message,), {
-
-    'WebcastLinkMicArmiesGroup' : _reflection.GeneratedProtocolMessageType('WebcastLinkMicArmiesGroup', (_message.Message,), {
-      'DESCRIPTOR' : _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS_WEBCASTLINKMICARMIESGROUP,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicArmies.WebcastLinkMicArmiesItems.WebcastLinkMicArmiesGroup)
-      })
-    ,
-    'DESCRIPTOR' : _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicArmies.WebcastLinkMicArmiesItems)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTLINKMICARMIES,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastLinkMicArmies)
-  })
-_sym_db.RegisterMessage(WebcastLinkMicArmies)
-_sym_db.RegisterMessage(WebcastLinkMicArmies.WebcastLinkMicArmiesItems)
-_sym_db.RegisterMessage(WebcastLinkMicArmies.WebcastLinkMicArmiesItems.WebcastLinkMicArmiesGroup)
-
-WebcastSocialMessage = _reflection.GeneratedProtocolMessageType('WebcastSocialMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTSOCIALMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastSocialMessage)
-  })
-_sym_db.RegisterMessage(WebcastSocialMessage)
-
-WebcastLikeMessage = _reflection.GeneratedProtocolMessageType('WebcastLikeMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTLIKEMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastLikeMessage)
-  })
-_sym_db.RegisterMessage(WebcastLikeMessage)
-
-WebcastQuestionNewMessage = _reflection.GeneratedProtocolMessageType('WebcastQuestionNewMessage', (_message.Message,), {
-
-  'QuestionDetails' : _reflection.GeneratedProtocolMessageType('QuestionDetails', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTQUESTIONNEWMESSAGE_QUESTIONDETAILS,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastQuestionNewMessage.QuestionDetails)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTQUESTIONNEWMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastQuestionNewMessage)
-  })
-_sym_db.RegisterMessage(WebcastQuestionNewMessage)
-_sym_db.RegisterMessage(WebcastQuestionNewMessage.QuestionDetails)
-
-WebcastLiveIntroMessage = _reflection.GeneratedProtocolMessageType('WebcastLiveIntroMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTLIVEINTROMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastLiveIntroMessage)
-  })
-_sym_db.RegisterMessage(WebcastLiveIntroMessage)
-
-SystemMessage = _reflection.GeneratedProtocolMessageType('SystemMessage', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.SystemMessage)
-  })
-_sym_db.RegisterMessage(SystemMessage)
-
-WebcastInRoomBannerMessage = _reflection.GeneratedProtocolMessageType('WebcastInRoomBannerMessage', (_message.Message,), {
-  'DESCRIPTOR' : _WEBCASTINROOMBANNERMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastInRoomBannerMessage)
-  })
-_sym_db.RegisterMessage(WebcastInRoomBannerMessage)
-
-WebcastRankUpdateMessage = _reflection.GeneratedProtocolMessageType('WebcastRankUpdateMessage', (_message.Message,), {
-
-  'RankContainer' : _reflection.GeneratedProtocolMessageType('RankContainer', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTRANKUPDATEMESSAGE_RANKCONTAINER,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastRankUpdateMessage.RankContainer)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTRANKUPDATEMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastRankUpdateMessage)
-  })
-_sym_db.RegisterMessage(WebcastRankUpdateMessage)
-_sym_db.RegisterMessage(WebcastRankUpdateMessage.RankContainer)
-
-WebcastHourlyRankMessage = _reflection.GeneratedProtocolMessageType('WebcastHourlyRankMessage', (_message.Message,), {
-
-  'HourlyRankContainer' : _reflection.GeneratedProtocolMessageType('HourlyRankContainer', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTHOURLYRANKMESSAGE_HOURLYRANKCONTAINER,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastHourlyRankMessage.HourlyRankContainer)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTHOURLYRANKMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastHourlyRankMessage)
-  })
-_sym_db.RegisterMessage(WebcastHourlyRankMessage)
-_sym_db.RegisterMessage(WebcastHourlyRankMessage.HourlyRankContainer)
-
-WebcastEmoteChatMessage = _reflection.GeneratedProtocolMessageType('WebcastEmoteChatMessage', (_message.Message,), {
-
-  'EmoteDetails' : _reflection.GeneratedProtocolMessageType('EmoteDetails', (_message.Message,), {
-
-    'EmoteImage' : _reflection.GeneratedProtocolMessageType('EmoteImage', (_message.Message,), {
-      'DESCRIPTOR' : _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS_EMOTEIMAGE,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.WebcastEmoteChatMessage.EmoteDetails.EmoteImage)
-      })
-    ,
-    'DESCRIPTOR' : _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastEmoteChatMessage.EmoteDetails)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTEMOTECHATMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastEmoteChatMessage)
-  })
-_sym_db.RegisterMessage(WebcastEmoteChatMessage)
-_sym_db.RegisterMessage(WebcastEmoteChatMessage.EmoteDetails)
-_sym_db.RegisterMessage(WebcastEmoteChatMessage.EmoteDetails.EmoteImage)
-
-WebcastEnvelopeMessage = _reflection.GeneratedProtocolMessageType('WebcastEnvelopeMessage', (_message.Message,), {
-
-  'TreasureBoxUser' : _reflection.GeneratedProtocolMessageType('TreasureBoxUser', (_message.Message,), {
-
-    'TreasureBoxUser2' : _reflection.GeneratedProtocolMessageType('TreasureBoxUser2', (_message.Message,), {
-
-      'TreasureBoxUser3' : _reflection.GeneratedProtocolMessageType('TreasureBoxUser3', (_message.Message,), {
-
-        'TreasureBoxUser4' : _reflection.GeneratedProtocolMessageType('TreasureBoxUser4', (_message.Message,), {
-          'DESCRIPTOR' : _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3_TREASUREBOXUSER4,
-          '__module__' : 'tiktok_schema_pb2'
-          # @@protoc_insertion_point(class_scope:TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3.TreasureBoxUser4)
-          })
-        ,
-        'DESCRIPTOR' : _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3,
-        '__module__' : 'tiktok_schema_pb2'
-        # @@protoc_insertion_point(class_scope:TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3)
-        })
-      ,
-      'DESCRIPTOR' : _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2)
-      })
-    ,
-    'DESCRIPTOR' : _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastEnvelopeMessage.TreasureBoxUser)
-    })
-  ,
-
-  'TreasureBoxData' : _reflection.GeneratedProtocolMessageType('TreasureBoxData', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTENVELOPEMESSAGE_TREASUREBOXDATA,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastEnvelopeMessage.TreasureBoxData)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTENVELOPEMESSAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastEnvelopeMessage)
-  })
-_sym_db.RegisterMessage(WebcastEnvelopeMessage)
-_sym_db.RegisterMessage(WebcastEnvelopeMessage.TreasureBoxUser)
-_sym_db.RegisterMessage(WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2)
-_sym_db.RegisterMessage(WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3)
-_sym_db.RegisterMessage(WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3.TreasureBoxUser4)
-_sym_db.RegisterMessage(WebcastEnvelopeMessage.TreasureBoxData)
-
-TikTokImage = _reflection.GeneratedProtocolMessageType('TikTokImage', (_message.Message,), {
-  'DESCRIPTOR' : _TIKTOKIMAGE,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.TikTokImage)
-  })
-_sym_db.RegisterMessage(TikTokImage)
-
-WebcastMessageEvent = _reflection.GeneratedProtocolMessageType('WebcastMessageEvent', (_message.Message,), {
-
-  'WebcastMessageEventDetails' : _reflection.GeneratedProtocolMessageType('WebcastMessageEventDetails', (_message.Message,), {
-    'DESCRIPTOR' : _WEBCASTMESSAGEEVENT_WEBCASTMESSAGEEVENTDETAILS,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WebcastMessageEvent.WebcastMessageEventDetails)
-    })
-  ,
-  'DESCRIPTOR' : _WEBCASTMESSAGEEVENT,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WebcastMessageEvent)
-  })
-_sym_db.RegisterMessage(WebcastMessageEvent)
-_sym_db.RegisterMessage(WebcastMessageEvent.WebcastMessageEventDetails)
-
-User = _reflection.GeneratedProtocolMessageType('User', (_message.Message,), {
-
-  'UserInfo' : _reflection.GeneratedProtocolMessageType('UserInfo', (_message.Message,), {
-    'DESCRIPTOR' : _USER_USERINFO,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.User.UserInfo)
-    })
-  ,
-
-  'UserBadge' : _reflection.GeneratedProtocolMessageType('UserBadge', (_message.Message,), {
-
-    'BadgeText' : _reflection.GeneratedProtocolMessageType('BadgeText', (_message.Message,), {
-      'DESCRIPTOR' : _USER_USERBADGE_BADGETEXT,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.User.UserBadge.BadgeText)
-      })
-    ,
-
-    'BadgeImage' : _reflection.GeneratedProtocolMessageType('BadgeImage', (_message.Message,), {
-      'DESCRIPTOR' : _USER_USERBADGE_BADGEIMAGE,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.User.UserBadge.BadgeImage)
-      })
-    ,
-
-    'BadgeComplex' : _reflection.GeneratedProtocolMessageType('BadgeComplex', (_message.Message,), {
-
-      'BadgeLabel' : _reflection.GeneratedProtocolMessageType('BadgeLabel', (_message.Message,), {
-        'DESCRIPTOR' : _USER_USERBADGE_BADGECOMPLEX_BADGELABEL,
-        '__module__' : 'tiktok_schema_pb2'
-        # @@protoc_insertion_point(class_scope:TikTok.User.UserBadge.BadgeComplex.BadgeLabel)
-        })
-      ,
-      'DESCRIPTOR' : _USER_USERBADGE_BADGECOMPLEX,
-      '__module__' : 'tiktok_schema_pb2'
-      # @@protoc_insertion_point(class_scope:TikTok.User.UserBadge.BadgeComplex)
-      })
-    ,
-    'DESCRIPTOR' : _USER_USERBADGE,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.User.UserBadge)
-    })
-  ,
-  'DESCRIPTOR' : _USER,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.User)
-  })
-_sym_db.RegisterMessage(User)
-_sym_db.RegisterMessage(User.UserInfo)
-_sym_db.RegisterMessage(User.UserBadge)
-_sym_db.RegisterMessage(User.UserBadge.BadgeText)
-_sym_db.RegisterMessage(User.UserBadge.BadgeImage)
-_sym_db.RegisterMessage(User.UserBadge.BadgeComplex)
-_sym_db.RegisterMessage(User.UserBadge.BadgeComplex.BadgeLabel)
-
-WeeklyRanking = _reflection.GeneratedProtocolMessageType('WeeklyRanking', (_message.Message,), {
-
-  'RankData' : _reflection.GeneratedProtocolMessageType('RankData', (_message.Message,), {
-    'DESCRIPTOR' : _WEEKLYRANKING_RANKDATA,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WeeklyRanking.RankData)
-    })
-  ,
-
-  'ExtraRankData' : _reflection.GeneratedProtocolMessageType('ExtraRankData', (_message.Message,), {
-    'DESCRIPTOR' : _WEEKLYRANKING_EXTRARANKDATA,
-    '__module__' : 'tiktok_schema_pb2'
-    # @@protoc_insertion_point(class_scope:TikTok.WeeklyRanking.ExtraRankData)
-    })
-  ,
-  'DESCRIPTOR' : _WEEKLYRANKING,
-  '__module__' : 'tiktok_schema_pb2'
-  # @@protoc_insertion_point(class_scope:TikTok.WeeklyRanking)
-  })
-_sym_db.RegisterMessage(WeeklyRanking)
-_sym_db.RegisterMessage(WeeklyRanking.RankData)
-_sym_db.RegisterMessage(WeeklyRanking.ExtraRankData)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13tiktok_schema.proto\x12\x06TikTok\"C\n\x17WebcastWebsocketMessage\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06\x62inary\x18\x08 \x01(\x0c\"/\n\x13WebcastWebsocketAck\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0c\n\x04type\x18\x07 \x01(\t\"\xf8\x02\n\x0fWebcastResponse\x12\x31\n\x08messages\x18\x01 \x03(\x0b\x32\x1f.TikTok.WebcastResponse.Message\x12\x0e\n\x06\x63ursor\x18\x02 \x01(\t\x12\x15\n\rfetchInterval\x18\x03 \x01(\x05\x12\x17\n\x0fserverTimestamp\x18\x04 \x01(\x03\x12\x13\n\x0binternalExt\x18\x05 \x01(\t\x12\x11\n\tfetchType\x18\x06 \x01(\x05\x12\x37\n\x07wsParam\x18\x07 \x01(\x0b\x32&.TikTok.WebcastResponse.WebsocketParam\x12\x19\n\x11heartbeatDuration\x18\x08 \x01(\x05\x12\x0f\n\x07needAck\x18\t \x01(\x08\x12\r\n\x05wsUrl\x18\n \x01(\t\x1a\'\n\x07Message\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06\x62inary\x18\x02 \x01(\x0c\x1a-\n\x0eWebsocketParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\"\n\x0bRoomMessage\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"\'\n\x15WebcastControlMessage\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\"\xbf\x01\n\x19WebcastRoomUserSeqMessage\x12@\n\x0btop_viewers\x18\x02 \x03(\x0b\x32+.TikTok.WebcastRoomUserSeqMessage.TopViewer\x12\x14\n\x0cviewer_count\x18\x03 \x01(\x05\x1aJ\n\tTopViewer\x12\x13\n\x0b\x63oins_given\x18\x01 \x01(\r\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x0c\n\x04rank\x18\x03 \x01(\r\"\xc3\x02\n\x12WebcastChatMessage\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x0f\n\x07\x63omment\x18\x03 \x01(\t\x12\x1e\n\x08mentions\x18\x0c \x03(\x0b\x32\x0c.TikTok.User\x12\x34\n\x06images\x18\r \x03(\x0b\x32$.TikTok.WebcastChatMessage.ChatImage\x12\x10\n\x08language\x18\x0e \x01(\t\x1a\x97\x01\n\tChatImage\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x42\n\x05image\x18\x02 \x01(\x0b\x32\x33.TikTok.WebcastChatMessage.ChatImage.ChatImageImage\x1a\x34\n\x0e\x43hatImageImage\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.TikTok.TikTokImage\"\x82\x01\n\x14WebcastMemberMessage\x12*\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x1b.TikTok.WebcastMessageEvent\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x0f\n\x07viewers\x18\x03 \x01(\x05\x12\x11\n\taction_id\x18\n \x01(\x05\"\xd2\x03\n\x12WebcastGiftMessage\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x13\n\x0brepeatCount\x18\x05 \x01(\x05\x12\x1a\n\x04user\x18\x07 \x01(\x0b\x32\x0c.TikTok.User\x12\x11\n\trepeatEnd\x18\t \x01(\x05\x12\x45\n\x04info\x18\x0f \x01(\x0b\x32\x37.TikTok.WebcastGiftMessage.WebcastGiftMessageGiftDetail\x12I\n\trecipient\x18\x17 \x01(\x0b\x32\x36.TikTok.WebcastGiftMessage.WebcastGiftMessageRecipient\x1a\x41\n\x1bWebcastGiftMessageRecipient\x12\x11\n\ttimestamp\x18\x06 \x01(\x04\x12\x0f\n\x07user_id\x18\x08 \x01(\x04\x1a\x96\x01\n\x1cWebcastGiftMessageGiftDetail\x12\"\n\x05image\x18\x01 \x01(\x0b\x32\x13.TikTok.TikTokImage\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\n\n\x02id\x18\x05 \x01(\x05\x12\x0c\n\x04type\x18\x0b \x01(\x05\x12\x15\n\rdiamond_count\x18\x0c \x01(\x05\"\xd6\x03\n\x14WebcastLinkMicBattle\x12K\n\x0b\x62\x61ttleUsers\x18\n \x03(\x0b\x32\x36.TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems\x1a\xf0\x02\n\x19WebcastLinkMicBattleItems\x12\x65\n\x0b\x62\x61ttleGroup\x18\x02 \x01(\x0b\x32P.TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup\x1a\xeb\x01\n\x19WebcastLinkMicBattleGroup\x12g\n\x04user\x18\x01 \x01(\x0b\x32Y.TikTok.WebcastLinkMicBattle.WebcastLinkMicBattleItems.WebcastLinkMicBattleGroup.LinkUser\x1a\x65\n\x08LinkUser\x12\x0f\n\x07user_id\x18\x01 \x01(\x04\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12#\n\x06\x61vatar\x18\x03 \x01(\x0b\x32\x13.TikTok.TikTokImage\x12\x11\n\tunique_id\x18\x04 \x01(\t\"\xdd\x02\n\x14WebcastLinkMicArmies\x12K\n\x0b\x62\x61ttleItems\x18\x03 \x03(\x0b\x32\x36.TikTok.WebcastLinkMicArmies.WebcastLinkMicArmiesItems\x12\x14\n\x0c\x62\x61ttleStatus\x18\x07 \x01(\x05\x1a\xe1\x01\n\x19WebcastLinkMicArmiesItems\x12\x12\n\nhostUserId\x18\x01 \x01(\x04\x12\x66\n\x0c\x62\x61ttleGroups\x18\x02 \x03(\x0b\x32P.TikTok.WebcastLinkMicArmies.WebcastLinkMicArmiesItems.WebcastLinkMicArmiesGroup\x1aH\n\x19WebcastLinkMicArmiesGroup\x12\x1b\n\x05users\x18\x01 \x03(\x0b\x32\x0c.TikTok.User\x12\x0e\n\x06points\x18\x02 \x01(\x05\"w\n\x14WebcastSocialMessage\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12\x17\n\x0ftotal_followers\x18\x06 \x01(\r\x12*\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x1b.TikTok.WebcastMessageEvent\"\x80\x01\n\x12WebcastLikeMessage\x12\x1a\n\x04user\x18\x05 \x01(\x0b\x32\x0c.TikTok.User\x12*\n\x05\x65vent\x18\x01 \x01(\x0b\x32\x1b.TikTok.WebcastMessageEvent\x12\r\n\x05likes\x18\x02 \x01(\x05\x12\x13\n\x0btotal_likes\x18\x03 \x01(\x05\"\xa8\x01\n\x19WebcastQuestionNewMessage\x12J\n\x0fquestionDetails\x18\x02 \x01(\x0b\x32\x31.TikTok.WebcastQuestionNewMessage.QuestionDetails\x1a?\n\x0fQuestionDetails\x12\x10\n\x08question\x18\x02 \x01(\t\x12\x1a\n\x04user\x18\x05 \x01(\x0b\x32\x0c.TikTok.User\"\xde\x01\n\x17WebcastLiveIntroMessage\x12\x0f\n\x07room_id\x18\x02 \x01(\x04\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x1e\n\x08streamer\x18\x05 \x01(\x0b\x32\x0c.TikTok.User\x12\x10\n\x08language\x18\x08 \x01(\t\x12=\n\nextra_info\x18\x07 \x01(\x0b\x32).TikTok.WebcastLiveIntroMessage.IntroData\x1a\x30\n\tIntroData\x12#\n\x07\x64\x65tails\x18\x15 \x01(\x0b\x32\x12.TikTok.ValueLabel\"$\n\rSystemMessage\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"*\n\x1aWebcastInRoomBannerMessage\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\xdb\x04\n\x16WebcastRankTextMessage\x12K\n\x0c\x64\x65tailsSmall\x18\x05 \x01(\x0b\x32\x35.TikTok.WebcastRankTextMessage.RankTextMessageSummary\x12?\n\x07\x64\x65tails\x18\x06 \x01(\x0b\x32..TikTok.WebcastRankTextMessage.RankTextMessage\x12\x0b\n\x03id1\x18\x07 \x01(\x04\x1aZ\n\x16RankTextMessageSummary\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12#\n\x07\x64\x65tails\x18\x04 \x01(\x0b\x32\x12.TikTok.ValueLabel\x1a\xc9\x02\n\x0fRankTextMessage\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12N\n\x07\x64\x65tails\x18\x04 \x03(\x0b\x32=.TikTok.WebcastRankTextMessage.RankTextMessage.MessageDetails\x1a\xc8\x01\n\x0eMessageDetails\x12\r\n\x05\x64\x61ta1\x18\x01 \x01(\r\x12\x10\n\x08\x63\x61tegory\x18\x0b \x01(\t\x12Y\n\x04user\x18\x15 \x01(\x0b\x32K.TikTok.WebcastRankTextMessage.RankTextMessage.MessageDetails.UserContainer\x1a:\n\rUserContainer\x12\x1a\n\x04user\x18\x01 \x01(\x0b\x32\x0c.TikTok.User\x12\r\n\x05\x64\x61ta1\x18\x02 \x01(\r\"\x8a\x01\n\x18WebcastRankUpdateMessage\x12=\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32/.TikTok.WebcastRankUpdateMessage.RankUpdateData\x1a/\n\x0eRankUpdateData\x12\x1d\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x0f.TikTok.Ranking\"\x88\x01\n\x18WebcastHourlyRankMessage\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..TikTok.WebcastHourlyRankMessage.RankContainer\x1a.\n\rRankContainer\x12\x1d\n\x04\x64\x61ta\x18\x04 \x01(\x0b\x32\x0f.TikTok.Ranking\"\xf8\x01\n\x17WebcastEmoteChatMessage\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.TikTok.User\x12;\n\x05\x65mote\x18\x03 \x01(\x0b\x32,.TikTok.WebcastEmoteChatMessage.EmoteDetails\x1a\x83\x01\n\x0c\x45moteDetails\x12\x10\n\x08\x65mote_id\x18\x01 \x01(\t\x12\x46\n\x05image\x18\x02 \x01(\x0b\x32\x37.TikTok.WebcastEmoteChatMessage.EmoteDetails.EmoteImage\x1a\x19\n\nEmoteImage\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x82\x05\n\x16WebcastEnvelopeMessage\x12G\n\x0ftreasureBoxData\x18\x02 \x01(\x0b\x32..TikTok.WebcastEnvelopeMessage.TreasureBoxData\x12G\n\x0ftreasureBoxUser\x18\x01 \x01(\x0b\x32..TikTok.WebcastEnvelopeMessage.TreasureBoxUser\x1a\x8e\x03\n\x0fTreasureBoxUser\x12N\n\x05user2\x18\x08 \x01(\x0b\x32?.TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2\x1a\xaa\x02\n\x10TreasureBoxUser2\x12_\n\x05user3\x18\x04 \x03(\x0b\x32P.TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3\x1a\xb4\x01\n\x10TreasureBoxUser3\x12p\n\x05user4\x18\x15 \x01(\x0b\x32\x61.TikTok.WebcastEnvelopeMessage.TreasureBoxUser.TreasureBoxUser2.TreasureBoxUser3.TreasureBoxUser4\x1a.\n\x10TreasureBoxUser4\x12\x1a\n\x04user\x18\x01 \x01(\x0b\x32\x0c.TikTok.User\x1a\x45\n\x0fTreasureBoxData\x12\r\n\x05\x63oins\x18\x05 \x01(\r\x12\x10\n\x08openable\x18\x06 \x01(\r\x12\x11\n\ttimestamp\x18\x07 \x01(\x04\"(\n\x0bTikTokImage\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\"\xa1\x01\n\x13WebcastMessageEvent\x12G\n\x07\x64\x65tails\x18\x08 \x01(\x0b\x32\x36.TikTok.WebcastMessageEvent.WebcastMessageEventDetails\x1a\x41\n\x1aWebcastMessageEventDetails\x12\x14\n\x0c\x64isplay_type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\"\xcf\x05\n\x04User\x12\x0f\n\x07user_id\x18\x01 \x01(\x04\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12#\n\x06\x61vatar\x18\t \x01(\x0b\x32\x13.TikTok.TikTokImage\x12#\n\x04info\x18\x16 \x01(\x0b\x32\x15.TikTok.User.UserInfo\x12\x11\n\tunique_id\x18& \x01(\t\x12\x0f\n\x07sec_uid\x18. \x01(\t\x12&\n\x06\x62\x61\x64ges\x18@ \x03(\x0b\x32\x16.TikTok.User.UserBadge\x1a\x45\n\x08UserInfo\x12\x11\n\tfollowing\x18\x01 \x01(\x05\x12\x11\n\tfollowers\x18\x02 \x01(\x05\x12\x13\n\x0b\x66ollow_role\x18\x03 \x01(\x05\x1a\xc6\x03\n\tUserBadge\x12\x18\n\x10\x62\x61\x64ge_scene_type\x18\x03 \x01(\x05\x12.\n\x04text\x18\x15 \x01(\x0b\x32 .TikTok.User.UserBadge.BadgeText\x12\x30\n\x05image\x18\x14 \x01(\x0b\x32!.TikTok.User.UserBadge.BadgeImage\x12\x34\n\x07\x63omplex\x18\x17 \x01(\x0b\x32#.TikTok.User.UserBadge.BadgeComplex\x1a(\n\tBadgeText\x12\r\n\x05label\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x1a\x30\n\nBadgeImage\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.TikTok.TikTokImage\x1a\xaa\x01\n\x0c\x42\x61\x64geComplex\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x13.TikTok.TikTokImage\x12=\n\x05label\x18\x03 \x01(\x0b\x32..TikTok.User.UserBadge.BadgeComplex.BadgeLabel\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\x1a)\n\nBadgeLabel\x12\r\n\x05label\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa4\x01\n\x07Ranking\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12+\n\x05\x65xtra\x18\x03 \x01(\x0b\x32\x1c.TikTok.Ranking.TikTokColour\x12#\n\x07\x64\x65tails\x18\x04 \x03(\x0b\x32\x12.TikTok.ValueLabel\x1a*\n\x0cTikTokColour\x12\x0e\n\x06\x63olour\x18\x01 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x04\"H\n\nValueLabel\x12\r\n\x05label\x18\x02 \x01(\t\x12\x0e\n\x06label2\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\r\x12\r\n\x05value\x18\x0b \x01(\tb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tiktok_schema_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _WEBCASTWEBSOCKETMESSAGE._serialized_start=31
-  _WEBCASTWEBSOCKETMESSAGE._serialized_end=98
-  _WEBCASTWEBSOCKETACK._serialized_start=100
-  _WEBCASTWEBSOCKETACK._serialized_end=147
-  _WEBCASTRESPONSE._serialized_start=150
-  _WEBCASTRESPONSE._serialized_end=526
-  _WEBCASTRESPONSE_MESSAGE._serialized_start=440
-  _WEBCASTRESPONSE_MESSAGE._serialized_end=479
-  _WEBCASTRESPONSE_WEBSOCKETPARAM._serialized_start=481
-  _WEBCASTRESPONSE_WEBSOCKETPARAM._serialized_end=526
-  _ROOMMESSAGE._serialized_start=528
-  _ROOMMESSAGE._serialized_end=562
-  _WEBCASTCONTROLMESSAGE._serialized_start=564
-  _WEBCASTCONTROLMESSAGE._serialized_end=603
-  _WEBCASTROOMUSERSEQMESSAGE._serialized_start=606
-  _WEBCASTROOMUSERSEQMESSAGE._serialized_end=797
-  _WEBCASTROOMUSERSEQMESSAGE_TOPVIEWER._serialized_start=723
-  _WEBCASTROOMUSERSEQMESSAGE_TOPVIEWER._serialized_end=797
-  _WEBCASTCHATMESSAGE._serialized_start=800
-  _WEBCASTCHATMESSAGE._serialized_end=1123
-  _WEBCASTCHATMESSAGE_CHATIMAGE._serialized_start=972
-  _WEBCASTCHATMESSAGE_CHATIMAGE._serialized_end=1123
-  _WEBCASTCHATMESSAGE_CHATIMAGE_CHATIMAGEIMAGE._serialized_start=1071
-  _WEBCASTCHATMESSAGE_CHATIMAGE_CHATIMAGEIMAGE._serialized_end=1123
-  _WEBCASTMEMBERMESSAGE._serialized_start=1126
-  _WEBCASTMEMBERMESSAGE._serialized_end=1256
-  _WEBCASTGIFTMESSAGE._serialized_start=1259
-  _WEBCASTGIFTMESSAGE._serialized_end=1725
-  _WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGERECIPIENT._serialized_start=1507
-  _WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGERECIPIENT._serialized_end=1572
-  _WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGEGIFTDETAIL._serialized_start=1575
-  _WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGEGIFTDETAIL._serialized_end=1725
-  _WEBCASTLINKMICBATTLE._serialized_start=1728
-  _WEBCASTLINKMICBATTLE._serialized_end=2198
-  _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS._serialized_start=1830
-  _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS._serialized_end=2198
-  _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP._serialized_start=1963
-  _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP._serialized_end=2198
-  _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP_LINKUSER._serialized_start=2097
-  _WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP_LINKUSER._serialized_end=2198
-  _WEBCASTLINKMICARMIES._serialized_start=2201
-  _WEBCASTLINKMICARMIES._serialized_end=2550
-  _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS._serialized_start=2325
-  _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS._serialized_end=2550
-  _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS_WEBCASTLINKMICARMIESGROUP._serialized_start=2478
-  _WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS_WEBCASTLINKMICARMIESGROUP._serialized_end=2550
-  _WEBCASTSOCIALMESSAGE._serialized_start=2552
-  _WEBCASTSOCIALMESSAGE._serialized_end=2671
-  _WEBCASTLIKEMESSAGE._serialized_start=2674
-  _WEBCASTLIKEMESSAGE._serialized_end=2802
-  _WEBCASTQUESTIONNEWMESSAGE._serialized_start=2805
-  _WEBCASTQUESTIONNEWMESSAGE._serialized_end=2973
-  _WEBCASTQUESTIONNEWMESSAGE_QUESTIONDETAILS._serialized_start=2910
-  _WEBCASTQUESTIONNEWMESSAGE_QUESTIONDETAILS._serialized_end=2973
-  _WEBCASTLIVEINTROMESSAGE._serialized_start=2975
-  _WEBCASTLIVEINTROMESSAGE._serialized_end=3084
-  _SYSTEMMESSAGE._serialized_start=3086
-  _SYSTEMMESSAGE._serialized_end=3122
-  _WEBCASTINROOMBANNERMESSAGE._serialized_start=3124
-  _WEBCASTINROOMBANNERMESSAGE._serialized_end=3166
-  _WEBCASTRANKUPDATEMESSAGE._serialized_start=3169
-  _WEBCASTRANKUPDATEMESSAGE._serialized_end=3315
-  _WEBCASTRANKUPDATEMESSAGE_RANKCONTAINER._serialized_start=3259
-  _WEBCASTRANKUPDATEMESSAGE_RANKCONTAINER._serialized_end=3315
-  _WEBCASTHOURLYRANKMESSAGE._serialized_start=3318
-  _WEBCASTHOURLYRANKMESSAGE._serialized_end=3476
-  _WEBCASTHOURLYRANKMESSAGE_HOURLYRANKCONTAINER._serialized_start=3414
-  _WEBCASTHOURLYRANKMESSAGE_HOURLYRANKCONTAINER._serialized_end=3476
-  _WEBCASTEMOTECHATMESSAGE._serialized_start=3479
-  _WEBCASTEMOTECHATMESSAGE._serialized_end=3727
-  _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS._serialized_start=3596
-  _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS._serialized_end=3727
-  _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS_EMOTEIMAGE._serialized_start=3702
-  _WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS_EMOTEIMAGE._serialized_end=3727
-  _WEBCASTENVELOPEMESSAGE._serialized_start=3730
-  _WEBCASTENVELOPEMESSAGE._serialized_end=4372
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER._serialized_start=3903
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER._serialized_end=4301
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2._serialized_start=4003
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2._serialized_end=4301
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3._serialized_start=4121
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3._serialized_end=4301
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3_TREASUREBOXUSER4._serialized_start=4255
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3_TREASUREBOXUSER4._serialized_end=4301
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXDATA._serialized_start=4303
-  _WEBCASTENVELOPEMESSAGE_TREASUREBOXDATA._serialized_end=4372
-  _TIKTOKIMAGE._serialized_start=4374
-  _TIKTOKIMAGE._serialized_end=4414
-  _WEBCASTMESSAGEEVENT._serialized_start=4417
-  _WEBCASTMESSAGEEVENT._serialized_end=4578
-  _WEBCASTMESSAGEEVENT_WEBCASTMESSAGEEVENTDETAILS._serialized_start=4513
-  _WEBCASTMESSAGEEVENT_WEBCASTMESSAGEEVENTDETAILS._serialized_end=4578
-  _USER._serialized_start=4581
-  _USER._serialized_end=5300
-  _USER_USERINFO._serialized_start=4774
-  _USER_USERINFO._serialized_end=4843
-  _USER_USERBADGE._serialized_start=4846
-  _USER_USERBADGE._serialized_end=5300
-  _USER_USERBADGE_BADGETEXT._serialized_start=5037
-  _USER_USERBADGE_BADGETEXT._serialized_end=5077
-  _USER_USERBADGE_BADGEIMAGE._serialized_start=5079
-  _USER_USERBADGE_BADGEIMAGE._serialized_end=5127
-  _USER_USERBADGE_BADGECOMPLEX._serialized_start=5130
-  _USER_USERBADGE_BADGECOMPLEX._serialized_end=5300
-  _USER_USERBADGE_BADGECOMPLEX_BADGELABEL._serialized_start=5259
-  _USER_USERBADGE_BADGECOMPLEX_BADGELABEL._serialized_end=5300
-  _WEEKLYRANKING._serialized_start=5303
-  _WEEKLYRANKING._serialized_end=5516
-  _WEEKLYRANKING_RANKDATA._serialized_start=5447
-  _WEEKLYRANKING_RANKDATA._serialized_end=5471
-  _WEEKLYRANKING_EXTRARANKDATA._serialized_start=5473
-  _WEEKLYRANKING_EXTRARANKDATA._serialized_end=5516
+  _globals['_WEBCASTWEBSOCKETMESSAGE']._serialized_start=31
+  _globals['_WEBCASTWEBSOCKETMESSAGE']._serialized_end=98
+  _globals['_WEBCASTWEBSOCKETACK']._serialized_start=100
+  _globals['_WEBCASTWEBSOCKETACK']._serialized_end=147
+  _globals['_WEBCASTRESPONSE']._serialized_start=150
+  _globals['_WEBCASTRESPONSE']._serialized_end=526
+  _globals['_WEBCASTRESPONSE_MESSAGE']._serialized_start=440
+  _globals['_WEBCASTRESPONSE_MESSAGE']._serialized_end=479
+  _globals['_WEBCASTRESPONSE_WEBSOCKETPARAM']._serialized_start=481
+  _globals['_WEBCASTRESPONSE_WEBSOCKETPARAM']._serialized_end=526
+  _globals['_ROOMMESSAGE']._serialized_start=528
+  _globals['_ROOMMESSAGE']._serialized_end=562
+  _globals['_WEBCASTCONTROLMESSAGE']._serialized_start=564
+  _globals['_WEBCASTCONTROLMESSAGE']._serialized_end=603
+  _globals['_WEBCASTROOMUSERSEQMESSAGE']._serialized_start=606
+  _globals['_WEBCASTROOMUSERSEQMESSAGE']._serialized_end=797
+  _globals['_WEBCASTROOMUSERSEQMESSAGE_TOPVIEWER']._serialized_start=723
+  _globals['_WEBCASTROOMUSERSEQMESSAGE_TOPVIEWER']._serialized_end=797
+  _globals['_WEBCASTCHATMESSAGE']._serialized_start=800
+  _globals['_WEBCASTCHATMESSAGE']._serialized_end=1123
+  _globals['_WEBCASTCHATMESSAGE_CHATIMAGE']._serialized_start=972
+  _globals['_WEBCASTCHATMESSAGE_CHATIMAGE']._serialized_end=1123
+  _globals['_WEBCASTCHATMESSAGE_CHATIMAGE_CHATIMAGEIMAGE']._serialized_start=1071
+  _globals['_WEBCASTCHATMESSAGE_CHATIMAGE_CHATIMAGEIMAGE']._serialized_end=1123
+  _globals['_WEBCASTMEMBERMESSAGE']._serialized_start=1126
+  _globals['_WEBCASTMEMBERMESSAGE']._serialized_end=1256
+  _globals['_WEBCASTGIFTMESSAGE']._serialized_start=1259
+  _globals['_WEBCASTGIFTMESSAGE']._serialized_end=1725
+  _globals['_WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGERECIPIENT']._serialized_start=1507
+  _globals['_WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGERECIPIENT']._serialized_end=1572
+  _globals['_WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGEGIFTDETAIL']._serialized_start=1575
+  _globals['_WEBCASTGIFTMESSAGE_WEBCASTGIFTMESSAGEGIFTDETAIL']._serialized_end=1725
+  _globals['_WEBCASTLINKMICBATTLE']._serialized_start=1728
+  _globals['_WEBCASTLINKMICBATTLE']._serialized_end=2198
+  _globals['_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS']._serialized_start=1830
+  _globals['_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS']._serialized_end=2198
+  _globals['_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP']._serialized_start=1963
+  _globals['_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP']._serialized_end=2198
+  _globals['_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP_LINKUSER']._serialized_start=2097
+  _globals['_WEBCASTLINKMICBATTLE_WEBCASTLINKMICBATTLEITEMS_WEBCASTLINKMICBATTLEGROUP_LINKUSER']._serialized_end=2198
+  _globals['_WEBCASTLINKMICARMIES']._serialized_start=2201
+  _globals['_WEBCASTLINKMICARMIES']._serialized_end=2550
+  _globals['_WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS']._serialized_start=2325
+  _globals['_WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS']._serialized_end=2550
+  _globals['_WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS_WEBCASTLINKMICARMIESGROUP']._serialized_start=2478
+  _globals['_WEBCASTLINKMICARMIES_WEBCASTLINKMICARMIESITEMS_WEBCASTLINKMICARMIESGROUP']._serialized_end=2550
+  _globals['_WEBCASTSOCIALMESSAGE']._serialized_start=2552
+  _globals['_WEBCASTSOCIALMESSAGE']._serialized_end=2671
+  _globals['_WEBCASTLIKEMESSAGE']._serialized_start=2674
+  _globals['_WEBCASTLIKEMESSAGE']._serialized_end=2802
+  _globals['_WEBCASTQUESTIONNEWMESSAGE']._serialized_start=2805
+  _globals['_WEBCASTQUESTIONNEWMESSAGE']._serialized_end=2973
+  _globals['_WEBCASTQUESTIONNEWMESSAGE_QUESTIONDETAILS']._serialized_start=2910
+  _globals['_WEBCASTQUESTIONNEWMESSAGE_QUESTIONDETAILS']._serialized_end=2973
+  _globals['_WEBCASTLIVEINTROMESSAGE']._serialized_start=2976
+  _globals['_WEBCASTLIVEINTROMESSAGE']._serialized_end=3198
+  _globals['_WEBCASTLIVEINTROMESSAGE_INTRODATA']._serialized_start=3150
+  _globals['_WEBCASTLIVEINTROMESSAGE_INTRODATA']._serialized_end=3198
+  _globals['_SYSTEMMESSAGE']._serialized_start=3200
+  _globals['_SYSTEMMESSAGE']._serialized_end=3236
+  _globals['_WEBCASTINROOMBANNERMESSAGE']._serialized_start=3238
+  _globals['_WEBCASTINROOMBANNERMESSAGE']._serialized_end=3280
+  _globals['_WEBCASTRANKTEXTMESSAGE']._serialized_start=3283
+  _globals['_WEBCASTRANKTEXTMESSAGE']._serialized_end=3886
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGESUMMARY']._serialized_start=3464
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGESUMMARY']._serialized_end=3554
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGE']._serialized_start=3557
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGE']._serialized_end=3886
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGE_MESSAGEDETAILS']._serialized_start=3686
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGE_MESSAGEDETAILS']._serialized_end=3886
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGE_MESSAGEDETAILS_USERCONTAINER']._serialized_start=3828
+  _globals['_WEBCASTRANKTEXTMESSAGE_RANKTEXTMESSAGE_MESSAGEDETAILS_USERCONTAINER']._serialized_end=3886
+  _globals['_WEBCASTRANKUPDATEMESSAGE']._serialized_start=3889
+  _globals['_WEBCASTRANKUPDATEMESSAGE']._serialized_end=4027
+  _globals['_WEBCASTRANKUPDATEMESSAGE_RANKUPDATEDATA']._serialized_start=3980
+  _globals['_WEBCASTRANKUPDATEMESSAGE_RANKUPDATEDATA']._serialized_end=4027
+  _globals['_WEBCASTHOURLYRANKMESSAGE']._serialized_start=4030
+  _globals['_WEBCASTHOURLYRANKMESSAGE']._serialized_end=4166
+  _globals['_WEBCASTHOURLYRANKMESSAGE_RANKCONTAINER']._serialized_start=4120
+  _globals['_WEBCASTHOURLYRANKMESSAGE_RANKCONTAINER']._serialized_end=4166
+  _globals['_WEBCASTEMOTECHATMESSAGE']._serialized_start=4169
+  _globals['_WEBCASTEMOTECHATMESSAGE']._serialized_end=4417
+  _globals['_WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS']._serialized_start=4286
+  _globals['_WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS']._serialized_end=4417
+  _globals['_WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS_EMOTEIMAGE']._serialized_start=4392
+  _globals['_WEBCASTEMOTECHATMESSAGE_EMOTEDETAILS_EMOTEIMAGE']._serialized_end=4417
+  _globals['_WEBCASTENVELOPEMESSAGE']._serialized_start=4420
+  _globals['_WEBCASTENVELOPEMESSAGE']._serialized_end=5062
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER']._serialized_start=4593
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER']._serialized_end=4991
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2']._serialized_start=4693
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2']._serialized_end=4991
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3']._serialized_start=4811
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3']._serialized_end=4991
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3_TREASUREBOXUSER4']._serialized_start=4945
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXUSER_TREASUREBOXUSER2_TREASUREBOXUSER3_TREASUREBOXUSER4']._serialized_end=4991
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXDATA']._serialized_start=4993
+  _globals['_WEBCASTENVELOPEMESSAGE_TREASUREBOXDATA']._serialized_end=5062
+  _globals['_TIKTOKIMAGE']._serialized_start=5064
+  _globals['_TIKTOKIMAGE']._serialized_end=5104
+  _globals['_WEBCASTMESSAGEEVENT']._serialized_start=5107
+  _globals['_WEBCASTMESSAGEEVENT']._serialized_end=5268
+  _globals['_WEBCASTMESSAGEEVENT_WEBCASTMESSAGEEVENTDETAILS']._serialized_start=5203
+  _globals['_WEBCASTMESSAGEEVENT_WEBCASTMESSAGEEVENTDETAILS']._serialized_end=5268
+  _globals['_USER']._serialized_start=5271
+  _globals['_USER']._serialized_end=5990
+  _globals['_USER_USERINFO']._serialized_start=5464
+  _globals['_USER_USERINFO']._serialized_end=5533
+  _globals['_USER_USERBADGE']._serialized_start=5536
+  _globals['_USER_USERBADGE']._serialized_end=5990
+  _globals['_USER_USERBADGE_BADGETEXT']._serialized_start=5727
+  _globals['_USER_USERBADGE_BADGETEXT']._serialized_end=5767
+  _globals['_USER_USERBADGE_BADGEIMAGE']._serialized_start=5769
+  _globals['_USER_USERBADGE_BADGEIMAGE']._serialized_end=5817
+  _globals['_USER_USERBADGE_BADGECOMPLEX']._serialized_start=5820
+  _globals['_USER_USERBADGE_BADGECOMPLEX']._serialized_end=5990
+  _globals['_USER_USERBADGE_BADGECOMPLEX_BADGELABEL']._serialized_start=5949
+  _globals['_USER_USERBADGE_BADGECOMPLEX_BADGELABEL']._serialized_end=5990
+  _globals['_RANKING']._serialized_start=5993
+  _globals['_RANKING']._serialized_end=6157
+  _globals['_RANKING_TIKTOKCOLOUR']._serialized_start=6115
+  _globals['_RANKING_TIKTOKCOLOUR']._serialized_end=6157
+  _globals['_VALUELABEL']._serialized_start=6159
+  _globals['_VALUELABEL']._serialized_end=6231
 # @@protoc_insertion_point(module_scope)
```

## TikTokLive/proto/utilities.py

```diff
@@ -38,15 +38,16 @@
                 "WebcastInRoomBannerMessage",
                 "SystemMessage",
                 "WebcastEmoteChatMessage",
                 "WebcastEnvelopeMessage",
                 "WebcastLiveIntroMessage",
                 "RoomMessage",
                 "WebcastRankUpdateMessage",
-                "WebcastHourlyRankMessage"
+                "WebcastHourlyRankMessage",
+                "WebcastRankTextMessage"
             ]:
                 continue
 
             _type = message.get("type")
             _schema = getattr(tiktok_schema, _type)()
             _schema.ParseFromString(message.get("binary"))
             _dict_data = protobuf_to_dict(_schema)
```

## TikTokLive/types/events.py

```diff
@@ -7,15 +7,16 @@
 
 import base64
 from dataclasses import field
 from typing import Optional, List, Any, Dict, ClassVar
 
 from mashumaro import DataClassDictMixin, pass_through
 
-from TikTokLive.types import User, Gift, Emote, TreasureBoxData, ExtraRankData, LinkUser, BattleArmy, TopViewer, ChatImage
+from TikTokLive.types import User, Gift, Emote, TreasureBoxData, ExtraRankData, LinkUser, BattleArmy, TopViewer, \
+    ChatImage, ValueLabel
 from TikTokLive.types.utilities import LiveEvent, alias
 
 
 class AbstractEvent(DataClassDictMixin):
     """
     Abstract TikTok Live event from which to build on
 
@@ -332,57 +333,105 @@
     treasure_box_data: Optional[TreasureBoxData] = alias('treasureBoxData')
     """Data about the enclosed Treasure Box in the envelope"""
 
     treasure_box_user: Optional[User] = alias('treasureBoxUser')
     """Data about the user that sent the treasure box"""
 
 
-@LiveEvent("weekly_ranking")
-class WeeklyRankingEvent(AbstractEvent):
+@LiveEvent("user_ranking_update")
+class UserRankingUpdateEvent(AbstractEvent):
     """
-    Event that fires when the weekly rankings are updated
+    Event publishing that a user ranked up in some way
+    e.g. "{0:user} just became a top {1:string} viewer!"
 
     """
 
     @classmethod
     def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
         """
         Pre-process weekly ranking event
 
         """
 
-        ranks: Dict[str, Any] = d.get('data', dict()).get('rankings', dict())  # Do a little flattening
+        data: dict = d.get('details', dict())
+        details: List[dict] = data.get('details', list())
 
-        # Try to flatten rank data & convert to int
+        # Delete Duplicate Entry
         try:
-            ranks['rank'] = int(ranks.get('data', dict()).get('rank', None))
-        except:
+            del data['details']
+        except KeyError:
             pass
 
-        return ranks
+        # Bring out user object
+        for detail in details:
+
+            # data1 = 11
+            if detail.get('user', dict()).get('user'):
+                data['user'] = detail['user']['user']
+
+            # data1 = 1
+            if detail.get('data1') == 1:
+                data['rank'] = detail.get('category')
+
+        return data
 
     type: Optional[str] = None
-    """Unknown"""
+    """The type of update"""
 
     label: Optional[str] = None
-    """Internal TikTok Label"""
+    """Update message text label"""
 
-    extra: Optional[ExtraRankData] = field(default_factory=ExtraRankData)
-    """Extra data relating to the UI, presumably"""
+    user: Optional[User] = None
+    """User who is ranking up"""
 
     rank: Optional[int] = None
-    """The number for the user's TikTok ranking. If the rank is "None", the user is not in the top 99."""
+    """The rank of the user"""
 
-    @property
-    def top_99(self) -> bool:
+
+@LiveEvent("ranking_update")
+class RankingUpdateEvent(AbstractEvent):
+    """
+    Event firing containing updates to rank information. So far, this has been noted to include:
+    - Weekly Ranking
+    - Rising Stars
+    """
+
+    @classmethod
+    def __pre_deserialize__(cls, d: Dict[Any, Any]) -> Dict[Any, Any]:
         """
-        Whether the user is in the top 99 of creators
+        Pre-process weekly ranking event
+
         """
 
-        return self.rank is not None
+        rank: Dict[str, Any] = d.get('data', dict()).get('data', dict())  # Flatten
+
+        # Try to flatten rank data & convert to int to
+        try:
+            details: Optional[List] = rank.get('details', list())
+            if len(details) > 0:
+                rank['rank'] = int(details[0].get('value', None))
+        except:
+            pass
+
+        return rank
+
+    type: Optional[str] = None
+    """The type of rank update (e.g. Rising stars, etc.)"""
+
+    label: Optional[str] = None
+    """Internal TikTok Label"""
+
+    details: List[ValueLabel] = field(default_factory=list)
+    """The user's ranking details. This can be more than just weekly ranking!"""
+
+    extra: Optional[ExtraRankData] = field(default_factory=ExtraRankData)
+    """Extra data relating to the UI, presumably"""
+
+    rank: Optional[int] = None
+    """The number for the user's TikTok ranking. """
 
 
 @LiveEvent("intro_message")
 class IntroMessageEvent(AbstractEvent):
     """
     Event fires giving the current stream description when the stream is joined
     Note: Only fires if "process_initial_data" is enabled and the streamer has an intro message configured
```

## TikTokLive/types/objects.py

```diff
@@ -395,15 +395,15 @@
 
     id: Optional[int] = None
     """The Internal TikTok ID of the gift"""
 
     count: Optional[int] = alias("repeatCount", default=None)
     """Number of times the gift has repeated"""
 
-    is_repeating: Optional[int] = alias("repeatEnd", default=0)
+    repeat_end: Optional[int] = alias("repeatEnd", default=0)
     """Whether or not the repetition is over"""
 
     info: Optional[GiftInfo] = field(default_factory=GiftInfo)
     """Details about the specific Gift sent"""
 
     recipient: Optional[GiftRecipient] = field(default_factory=GiftRecipient)
     """Who received the gift (for streams with multiple users)"""
@@ -426,15 +426,15 @@
         """
         Whether the streak is over
         
         :return: True if currently streaking, False if not
 
         """
 
-        return bool(self.is_repeating)
+        return not bool(self.repeat_end)
 
 
 @dataclass()
 class EmoteImage(AbstractObject):
     """
     Container encapsulating the image URL for the Emote
 
@@ -567,14 +567,27 @@
     """The number of points the battle army has"""
 
     participants: List[User] = field(default_factory=list)
     """The users involved in the specific battle army"""
 
 
 @dataclass()
+class ValueLabel(AbstractObject):
+    """
+    Label containing a value
+
+    """
+
+    value: Optional[str] = None
+    data: Optional[int] = None
+    label: Optional[str] = None
+    label2: Optional[str] = None
+
+
+@dataclass()
 class FFmpegWrapper:
     """
     A wrapper for the FFmpeg Stream Download utility in the TikTokLive Package
 
     """
 
     runtime: Optional[str]
```

