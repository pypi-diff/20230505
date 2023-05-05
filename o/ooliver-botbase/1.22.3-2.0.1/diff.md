# Comparing `tmp/ooliver_botbase-1.22.3.tar.gz` & `tmp/ooliver_botbase-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooliver_botbase-1.22.3.tar", max compression
+gzip compressed data, was "ooliver_botbase-2.0.1.tar", max compression
```

## Comparing `ooliver_botbase-1.22.3.tar` & `ooliver_botbase-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
--rw-r--r--   0        0        0     2179 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/README.md
--rw-r--r--   0        0        0      280 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/__init__.py
--rw-r--r--   0        0        0        0 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/__main__.py
--rw-r--r--   0        0        0     1811 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/blacklist.py
--rw-r--r--   0        0        0    19491 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/botbase.py
--rw-r--r--   0        0        0     8520 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/checks.py
--rw-r--r--   0        0        0      922 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/cli.py
--rw-r--r--   0        0        0        0 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/cogs/__init__.py
--rw-r--r--   0        0        0     2961 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/cogs/blacklist.py
--rw-r--r--   0        0        0    12627 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/cogs/help.py
--rw-r--r--   0        0        0      338 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/emojis.py
--rw-r--r--   0        0        0      151 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/exceptions.py
--rw-r--r--   0        0        0      267 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/models.py
--rw-r--r--   0        0        0        1 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/py.typed
--rw-r--r--   0        0        0      357 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/__init__.py
--rw-r--r--   0        0        0      861 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/channel.py
--rw-r--r--   0        0        0      482 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/context.py
--rw-r--r--   0        0        0     1428 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/inter.py
--rw-r--r--   0        0        0      457 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/member.py
--rw-r--r--   0        0        0      455 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/thread.py
--rw-r--r--   0        0        0      461 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/user.py
--rw-r--r--   0        0        0     5094 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/botbase/wraps/wrap.py
--rw-r--r--   0        0        0      775 2022-10-25 19:12:16.113977 ooliver_botbase-1.22.3/pyproject.toml
--rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 ooliver_botbase-1.22.3/setup.py
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 ooliver_botbase-1.22.3/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/README.md
+-rw-r--r--   0        0        0      275 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/__init__.py
+-rw-r--r--   0        0        0    13364 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/botbase.py
+-rw-r--r--   0        0        0       73 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/__init__.py
+-rw-r--r--   0        0        0      625 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/blacklist.py
+-rw-r--r--   0        0        0      727 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/commands.py
+-rw-r--r--   0        0        0      364 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/db/metadata.py
+-rw-r--r--   0        0        0     6064 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/exts/blacklist.py
+-rw-r--r--   0        0        0     1343 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/exts/log_commands.py
+-rw-r--r--   0        0        0     1637 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/exts/log_guilds.py
+-rw-r--r--   0        0        0      288 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/models.py
+-rw-r--r--   0        0        0        1 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/py.typed
+-rw-r--r--   0        0        0      309 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/wraps/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/wraps/channel.py
+-rw-r--r--   0        0        0     1391 2023-05-05 21:53:52.984180 ooliver_botbase-2.0.1/botbase/wraps/inter.py
+-rw-r--r--   0        0        0      253 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/member.py
+-rw-r--r--   0        0        0      253 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/thread.py
+-rw-r--r--   0        0        0      245 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/user.py
+-rw-r--r--   0        0        0     4398 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/botbase/wraps/wrap.py
+-rw-r--r--   0        0        0      800 2023-05-05 21:53:52.988180 ooliver_botbase-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 ooliver_botbase-2.0.1/PKG-INFO
```

### Comparing `ooliver_botbase-1.22.3/botbase/botbase.py` & `ooliver_botbase-2.0.1/botbase/botbase.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,46 @@
 from __future__ import annotations
 
 from asyncio import TimeoutError as AsyncTimeoutError
-from asyncio import sleep, wait_for
+from asyncio import wait_for
 from contextlib import suppress
-from importlib import import_module
-from logging import CRITICAL, INFO, Formatter, getLogger, StreamHandler
+from logging import CRITICAL, INFO, Formatter, StreamHandler, getLogger
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from random import choice
 from sys import modules
-from textwrap import dedent
 from types import ModuleType
 from typing import TYPE_CHECKING
 
-from aiohttp import ClientSession
-from asyncpg import create_pool
-from nextcord import Embed, Interaction, Member, Thread, User, abc
-from nextcord.ext.commands import (
-    AutoShardedBot,
-    ExtensionNotFound,
-    when_mentioned,
-    when_mentioned_or,
-)
-
-from .blacklist import Blacklist
-from .emojis import Emojis
-from .wraps import (
-    MyContext,
-    MyInter,
-    WrappedChannel,
-    WrappedMember,
-    WrappedThread,
-    WrappedUser,
-)
+from aiohttp import BaseConnector, BasicAuth, ClientSession
+from nextcord import Intents, Interaction, Member, Thread, User, abc
+from nextcord.ext.commands import AutoShardedBot, ExtensionNotFound
+from nextcord.utils import MISSING
 
-if TYPE_CHECKING:
-    from typing import Any, Callable, Mapping, Optional, Union
-
-    from asyncpg import Pool
-    from nextcord import Guild, Message, PartialMessageable
+from .wraps import MyInter, WrappedChannel, WrappedMember, WrappedThread, WrappedUser
 
+if TYPE_CHECKING:
+    from asyncio import AbstractEventLoop
+    from typing import Any, Awaitable, Callable, Iterable, Mapping, Sequence, Union
 
-log = getLogger(__name__)
-defaulthelpmsg = """
-HI! Welcome to the help page for {name}!
+    from nextcord import (
+        AllowedMentions,
+        BaseActivity,
+        Guild,
+        MemberCacheFlags,
+        Message,
+        PartialMessageable,
+        Status,
+    )
+    from nextcord.ext.commands import Bot, HelpCommand
 
-Use `{prefix}help <command>` for more info on a command,
-or `{prefix}help <category>` for more info on a category,
+    _NonCallablePrefix = Union[str, Sequence[str]]
 
-Use the dropdown below to select a category.
 
-Have fun!
-"""
-defaulthelpindex = """
-I have been up since {created_at} and I serve for you!
-"""
-
-
-initialise = """
-CREATE TABLE IF NOT EXISTS guilds (
-    id BIGINT PRIMARY KEY,
-    prefix VARCHAR
-);
-CREATE TABLE IF NOT EXISTS commands (
-    command VARCHAR NOT NULL,
-    guild BIGINT,
-    channel BIGINT,
-    member BIGINT NOT NULL,
-    amount INT,
-    UNIQUE(command, guild, channel, member)
-);
-CREATE TABLE IF NOT EXISTS blacklist_guilds (
-    id BIGINT PRIMARY KEY,
-    reason VARCHAR
-);
-CREATE TABLE IF NOT EXISTS blacklist_users (
-    id BIGINT PRIMARY KEY,
-    reason VARCHAR
-);
-"""
+log = getLogger(__name__)
 
 
 def get_handlers():
     formatter = Formatter(
         "%(levelname)-7s %(asctime)s %(filename)12s:%(funcName)-28s: %(message)s",
         datefmt="%H:%M:%S %d/%m/%Y",
     )
@@ -97,142 +55,169 @@
     i.setFormatter(formatter)
     h.setFormatter(formatter)
     h.namer = lambda name: name.replace(".log", "") + ".log"
     return h, i
 
 
 class BotBase(AutoShardedBot):
-    db: Pool
     session: ClientSession
-    blacklist: Optional[Blacklist]
 
     @staticmethod
-    def get_config(config_module: str) -> tuple[str, str]:
+    def get_module() -> str:
         file = modules["__main__"].__file__
 
         if file is None:
             raise RuntimeError("how")
 
         path = Path(file)
 
         if path.parts[-1] == "__main__.py":
-            mod = path.parts[-2]
-            return f"{mod}.{config_module}", mod
-        else:
-            return config_module, ""
+            return path.parts[-2]
 
-    def __init__(self, *args, config_module: str = "config", **kwargs) -> None:
-        cfg, mod = self.get_config(config_module.rstrip(".py"))
-        try:
-            config = import_module(cfg)
-        except ImportError:
-            config = None
-
-        if not getattr(config, "prefix", None):
-            default_getter = when_mentioned
-            kwargs["help_command"] = None
-            set_help = False
-        else:
-            default_getter = self.get_pre
-            set_help = True
-
-        pre = kwargs.pop("command_prefix", default_getter)
-        saf = kwargs.pop("strip_after_prefix", True)
-        ca = kwargs.pop("case_insensitive", True)
+        return "."
 
+    def __init__(
+        self,
+        command_prefix: Union[
+            _NonCallablePrefix,
+            Callable[
+                [Union[Bot, AutoShardedBot], Message],
+                Union[Awaitable[_NonCallablePrefix], _NonCallablePrefix],
+            ],
+        ] = tuple(),
+        *,
+        version: str = "0.0.0",
+        aiohttp_enabled: bool = True,
+        blacklist_enabled: bool = True,
+        db_enabled: bool = True,
+        colours: list[int] = [0x9966CC],
+        name: str | None = None,
+        log_channel: int | None = None,
+        guild_ids: Sequence[int] | None = None,
+        log_commands: bool = True,
+        log_guilds: bool = False,
+        # nextcord
+        help_command: HelpCommand | None = None,
+        description: str | None = None,
+        max_messages: int | None = 1000,
+        connector: BaseConnector | None = None,
+        proxy: str | None = None,
+        proxy_auth: BasicAuth | None = None,
+        shard_id: int | None = None,
+        shard_count: int | None = None,
+        shard_ids: list[int] | None = None,
+        application_id: int | None = None,
+        intents: Intents = Intents.default(),
+        member_cache_flags: MemberCacheFlags = MISSING,
+        chunk_guilds_at_startup: bool = MISSING,
+        status: Status | None = None,
+        activity: BaseActivity | None = None,
+        allowed_mentions: AllowedMentions | None = None,
+        heartbeat_timeout: float = 60.0,
+        guild_ready_timeout: float = 2.0,
+        assume_unsync_clock: bool = True,
+        enable_debug_events: bool = False,
+        loop: AbstractEventLoop | None = None,
+        lazy_load_commands: bool = True,
+        rollout_associate_known: bool = True,
+        rollout_delete_unknown: bool = True,
+        rollout_register_new: bool = True,
+        rollout_update_known: bool = True,
+        rollout_all_guilds: bool = False,
+        default_guild_ids: list[int] | None = None,
+        owner_id: int | None = None,
+        owner_ids: Iterable[int] | None = None,
+        strip_after_prefix: bool = False,
+        case_insensitive: bool = False,
+        **kwargs: Any,  # fallback for missing args
+    ) -> None:
         super().__init__(
-            *args,
-            command_prefix=pre,
-            strip_after_prefix=saf,
-            case_insensitive=ca,
+            command_prefix=command_prefix,
+            help_command=help_command,
+            description=description,
+            max_messages=max_messages,
+            connector=connector,
+            proxy=proxy,
+            proxy_auth=proxy_auth,
+            shard_id=shard_id,
+            shard_count=shard_count,
+            shard_ids=shard_ids,
+            application_id=application_id,
+            intents=intents,
+            member_cache_flags=member_cache_flags,
+            chunk_guilds_at_startup=chunk_guilds_at_startup,
+            status=status,
+            activity=activity,
+            allowed_mentions=allowed_mentions,
+            heartbeat_timeout=heartbeat_timeout,
+            guild_ready_timeout=guild_ready_timeout,
+            assume_unsync_clock=assume_unsync_clock,
+            enable_debug_events=enable_debug_events,
+            loop=loop,
+            lazy_load_commands=lazy_load_commands,
+            rollout_associate_known=rollout_associate_known,
+            rollout_delete_unknown=rollout_delete_unknown,
+            rollout_register_new=rollout_register_new,
+            rollout_update_known=rollout_update_known,
+            rollout_all_guilds=rollout_all_guilds,
+            default_guild_ids=default_guild_ids,
+            owner_id=owner_id,
+            owner_ids=owner_ids,
+            strip_after_prefix=strip_after_prefix,
+            case_insensitive=case_insensitive,
             **kwargs,
         )
+        self.module = self.get_module()
 
         self.prefix: dict[int, list[str]] = {}
 
         log = getLogger()
         log.handlers = []
         log.setLevel(INFO)
         h, i = get_handlers()
 
         log.addHandler(h)
         log.addHandler(i)
         getLogger("asyncio").setLevel(CRITICAL)
 
         self.loop.set_exception_handler(self.asyncio_handler)
 
-        self.mod = mod
-
-        self.db_enabled: bool
-        self.db_args: tuple[Any, ...]
-        self.db_kwargs: dict[str, Any]
-
-        if db_url := getattr(config, "db_url", None):
-            self.db_enabled = True
-            self.db_args = (db_url,)
-            self.db_kwargs = {}
-        elif (db_name := getattr(config, "db_name", None)) and (
-            db_user := getattr(config, "db_user", "ooliver")
-        ):
-            self.db_enabled = True
-            self.db_args = ()
-            self.db_kwargs = {
-                "database": db_name,
-                "user": db_user,
-                "host": getattr(config, "db_host", None),
-            }
-            if port := getattr(config, "db_port", None):
-                self.db_kwargs["port"] = port
-        else:
-            self.db_enabled = False
-            self.db_args = ()
-            self.db_kwargs = {}
-
-        if init := getattr(config, "init", None):
-            self.db_kwargs["init"] = init
-
-        self.version: str = getattr(config, "version", "0.0.0")
-        self.aiohttp_enabled: bool = getattr(config, "aiohttp_enabled", True)
-        self.colors: list[int] = getattr(config, "colors", [0x9966CC])
-        self.blacklist_enabled: bool = getattr(config, "blacklist_enabled", True)
-        self.default_pre: list[str] = getattr(config, "prefix", [])
-        self.helpmsg: str = getattr(config, "helpmsg", defaulthelpmsg)
-        self.helpindex: str = getattr(config, "helpindex", defaulthelpindex)
-        self.helpfields: dict[str, str] = getattr(config, "helpfields", {})
-        self.helptitle: str = getattr(config, "helptitle", "Help Me {name}!")
-        self.helpinsert: str = getattr(config, "helpinsert", "")
-        self.emojiset: Any = getattr(config, "emojiset", Emojis())
-        self.logchannel: int | None = getattr(config, "logchannel", None)
-        self.guild_ids: list[int] | None = getattr(config, "guild_ids", None)
-        self.database_init: str = initialise + getattr(config, "database_init", "")
-        self.name: Optional[str] = getattr(config, "name", None)
+        self.version: str = version
+        self.aiohttp_enabled: bool = aiohttp_enabled
+        self.colours: list[int] = colours
+        self.name: str | None = name
+        self.db_enabled: bool = db_enabled
+        self.log_channel: int | None = log_channel
+        self.guild_ids: Sequence[int] | None = guild_ids
 
         self._single_events: dict[str, Callable] = {
             "on_message": self.get_wrapped_message,
             "on_interaction": self.get_wrapped_interaction,
         }
         self._double_events: dict[str, Callable] = {
             "on_message_edit": lambda before, after: (
                 self.get_wrapped_message(before),
                 self.get_wrapped_message(after),
             )
         }
 
-        self.load_extension("jishaku")
+        self.load_extension("delarva", extras={"guild_ids": guild_ids})
+
+        if blacklist_enabled and db_enabled:
+            self.load_extension("botbase.exts.blacklist")
 
-        if set_help:
-            self.load_extension("botbase.cogs.help")
+        if log_commands and db_enabled:
+            self.load_extension("botbase.exts.log_commands")
 
-        if self.blacklist_enabled:
-            self.load_extension("botbase.cogs.blacklist")
-            self.blacklist = None
+        if log_guilds:
+            self.load_extension("botbase.exts.log_guilds")
 
     @property
-    def color(self) -> int:
-        return choice(self.colors)
+    def colour(self) -> int:
+        return choice(self.colours)
 
     def asyncio_handler(self, _, context: dict) -> None:
         log = getLogger("notasyncio")
         if context["message"] == "Unclosed client session":
             return
 
         log.error(
@@ -241,107 +226,59 @@
             + "\n".join(
                 f"{k}: {v}"
                 for k, v in context.items()
                 if k != "message" and k is not None and v is not None and k != "None"
             )
         )
 
-    async def start(self, *args, **kwargs) -> None:
+    async def start(self, token: str, *, reconnect: bool = True) -> None:
         if self.db_enabled:
-            for tries in range(5):
-                try:
-                    db = await create_pool(*self.db_args, **self.db_kwargs)
-                    assert db is not None
-                    self.db = db
-                except AssertionError:
-                    await sleep(2.5 * tries + 1)
-                else:
-                    break
+            from .db import database
 
-            await self.db.execute(self.database_init)
+            await database.connect()
 
         if self.aiohttp_enabled:
             self.session = ClientSession()
 
-        if self.blacklist_enabled and self.db_enabled:
-            self.blacklist = Blacklist(self.db)
+        await super().start(token, reconnect=reconnect)
 
-        await super().start(*args, **kwargs)
+    def run(self, token: str, *, reconnect: bool = True) -> None:
+        cogs = Path(self.module)
 
-    def run(self, *args, **kwargs) -> None:
-        cog_dir = f"{self.mod}/cogs" if self.mod else "./cogs"
-        cogs = Path(cog_dir)
-
-        for ext in cogs.glob("**/*.py"):
+        for ext in cogs.glob("exts/**/*.py"):
             log.info("Found file %s", ext)
-            if "extras" in ext.parts or any(part.startswith("_") for part in ext.parts):
+            if any(part.startswith("_") for part in ext.parts):
                 continue
+
             if ext.suffix == ".py":
                 a = ".".join(ext.parts).removesuffix(".py")
                 log.info("Loading ext %s", a)
                 self.load_extension(a)
                 log.info("Loaded ext %s", a)
 
-        super().run(*args, **kwargs)
+        super().run(token, reconnect=reconnect)
 
     async def close(self, *args, **kwargs) -> None:
         if self.aiohttp_enabled and hasattr(self, "session"):
             await self.session.close()
 
-        if self.db_enabled and hasattr(self, "db"):
+        if self.db_enabled:
             with suppress(AsyncTimeoutError):
-                await wait_for(self.db.close(), timeout=5)
+                from .db import database
 
-        await super().close(*args, **kwargs)
+                await wait_for(database.disconnect(), timeout=5)
 
-    @staticmethod
-    async def get_pre(bot: BotBase, message: Message) -> list[str]:
-        if not bot.db_enabled:
-            return bot.default_pre
-
-        if message.guild is not None:
-            try:
-                prefix = bot.prefix[message.guild.id]
-            except KeyError:
-                prefix = [
-                    await bot.db.fetchval(
-                        "SELECT prefix FROM guilds WHERE id=$1", message.guild.id
-                    )
-                ]
-                if prefix[0] is None:
-                    prefix = bot.default_pre
-                    bot.prefix[message.guild.id] = prefix
-        else:
-            prefix = bot.default_pre
-        return when_mentioned_or(*prefix)(bot, message)
+        await super().close(*args, **kwargs)
 
     async def on_application_command_error(*_):
         ...  # hope an event handler exists
 
-    async def process_commands(self, message: Message) -> None:
-        if message.author.bot:
-            return
-
-        if self.blacklist and message.author.id in self.blacklist:
-            return log.debug("Ignoring blacklisted user %s", message.author.id)
-        elif self.blacklist and message.guild and message.guild.id in self.blacklist:
-            return log.debug("Ignoring blacklisted guild %s", message.guild.id)
-
-        ctx = await self.get_context(message, cls=MyContext)
-
-        await self.invoke(ctx)
-
     async def on_interaction(self, interaction: Interaction) -> None:
         i = self.get_wrapped_interaction(interaction)
 
-        if self.blacklist and i.author.id in self.blacklist:
-            return log.debug("Ignoring blacklisted user %s", i.author.id)
-        elif self.blacklist and i.guild and i.guild.id in self.blacklist:
-            return log.debug("Ignoring blacklisted guild %s", i.guild.id)
-
         await self.process_application_commands(i)
 
     async def getch_member(self, guild_id: int, member_id: int) -> WrappedMember:
         guild = await self.getch_guild(guild_id)
         member = guild.get_member(member_id)
         if member is not None:
             return WrappedMember(member, bot=self)
@@ -418,185 +355,50 @@
                 args[0], args[1]
             )
             super().dispatch(event_name, wrapped_first_arg, wrapped_second_arg)
 
         else:
             super().dispatch(event_name, *args, **kwargs)
 
-    async def on_command_completion(self, ctx: MyContext):
-        if not self.db_enabled:
-            return
-
-        if ctx.guild is not None:
-            await self.db.execute(
-                """INSERT INTO commands (command, guild, channel, member, amount) 
-                VALUES ($1,$2,$3,$4,$5) 
-                ON CONFLICT (command, guild, channel, member) DO UPDATE
-                    SET amount = commands.amount + 1""",
-                ctx.command.qualified_name,  # type: ignore
-                ctx.guild.id,
-                ctx.channel.id,
-                ctx.author.id,
-                1,
-            )
-        else:
-            a = await self.db.fetchval(
-                "SELECT * FROM commands WHERE member=$1 AND channel IS NULL and guild IS NULL",
-                ctx.author.id,
-            )
-            if a is None:
-                await self.db.execute(
-                    """INSERT INTO commands (command, guild, channel, member, amount) 
-                    VALUES ($1,$2,$3,$4,$5)""",
-                    ctx.command.qualified_name,  # type: ignore
-                    None,
-                    None,
-                    ctx.author.id,
-                    1,
-                )
-            else:
-                await self.db.execute(
-                    """UPDATE commands SET amount = commands.amount + 1 
-                    WHERE member=$1 AND channel IS NULL and guild IS NULL""",
-                    ctx.author.id,
-                )
-
-    async def on_application_command_completion(self, inter: MyInter):
-        if not self.db_enabled:
-            return
-
-        if inter.guild is not None:
-            await self.db.execute(
-                """INSERT INTO commands (command, guild, channel, member, amount) 
-                VALUES ($1,$2,$3,$4,$5) 
-                ON CONFLICT (command, guild, channel, member) DO UPDATE
-                    SET amount = commands.amount + 1""",
-                inter.command,
-                inter.guild.id,
-                inter.channel.id,  # type: ignore
-                inter.author.id,
-                1,
-            )
-        else:
-            a = await self.db.fetchval(
-                "SELECT * FROM commands WHERE member=$1 AND channel IS NULL and guild IS NULL",
-                inter.author.id,
-            )
-            if a is None:
-                await self.db.execute(
-                    """INSERT INTO commands (command, guild, channel, member, amount) 
-                    VALUES ($1,$2,$3,$4,$5)""",
-                    inter.command,
-                    None,
-                    None,
-                    inter.author.id,
-                    1,
-                )
-            else:
-                await self.db.execute(
-                    """UPDATE commands SET amount = commands.amount + 1 
-                    WHERE member=$1 AND channel IS NULL and guild IS NULL""",
-                    inter.author.id,
-                )
-
-    async def on_guild_join(self, guild: Guild):
-        if not self.logchannel:
-            return
-        elif not self.db_enabled:
-            return
-
-        if self.blacklist and guild.id in self.blacklist.guilds:
-            log.info("Leaving blacklisted Guild(id=%s)", guild.id)
-            await guild.leave()
-            return
-
-        assert guild.owner_id is not None
-
-        embed = Embed(
-            title="New Guild!",
-            description=dedent(
-                f"""
-
-        **{guild.name}**
-        id: `{guild.id}`
-        members: `{guild.member_count}`
-        owner: `{guild.owner or await self.fetch_user(guild.owner_id)}`
-
-        """
-            ),
-            color=self.color,
-        )
-        await self.get_channel(self.logchannel).send(embed=embed)  # type: ignore
-
-    async def on_guild_remove(self, guild: Guild):
-        if guild.unavailable:
-            return
-
-        if not self.logchannel:
-            return
-        elif not self.db_enabled:
-            return
-
-        assert guild.owner_id is not None
-
-        embed = Embed(
-            title="Removed Guild :(",
-            description=dedent(
-                f"""
-
-        **{guild.name}**
-        id: `{guild.id}`
-        members: `{guild.member_count}`
-        owner: `{guild.owner or await self.fetch_user(guild.owner_id)}`
-
-        """
-            ),
-            color=self.color,
-        )
-        try:
-            await self.get_channel(self.logchannel).send(embed=embed)  # type: ignore
-        except AttributeError:
-            pass
-
     def load_extension(
-        self, name: str, *, extras: Optional[dict[str, Any]] = None
+        self, name: str, *, extras: dict[str, Any] | None = None
     ) -> None:
-        ext = f"{self.name}.cogs.{name}" if self.name else name
+        ext = f"{self.name}.exts.{name}" if self.name else name
 
         try:
             super().load_extension(ext, extras=extras)
         except (ExtensionNotFound, ModuleNotFoundError):
             super().load_extension(name, extras=extras)
 
         if self.is_ready():
             self.loop.create_task(self.sync_all_application_commands())
 
     def reload_extension(self, name: str) -> None:
-        ext = f"{self.name}.cogs.{name}" if self.name else name
+        ext = f"{self.name}.exts.{name}" if self.name else name
 
         try:
             super().reload_extension(ext)
         except (ExtensionNotFound, ModuleNotFoundError):
             super().reload_extension(name)
 
         if self.is_ready():
             self.loop.create_task(self.sync_all_application_commands())
 
     def unload_extension(self, name: str) -> None:
-        ext = f"{self.name}.cogs.{name}" if self.name else name
+        ext = f"{self.name}.exts.{name}" if self.name else name
 
         try:
             super().unload_extension(ext)
         except (ExtensionNotFound, ModuleNotFoundError):
             super().unload_extension(name)
 
         self.loop.create_task(self.sync_all_application_commands())
 
     @property
     def extensions(self) -> Mapping[str, ModuleType]:
         if not self.name:
             return super().extensions
 
         return {
-            k.removeprefix(f"{self.name}.cogs."): v
+            k.removeprefix(f"{self.name}.exts."): v
             for k, v in super().extensions.items()
         } | super().extensions
```

### Comparing `ooliver_botbase-1.22.3/botbase/wraps/channel.py` & `ooliver_botbase-2.0.1/botbase/wraps/channel.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,14 @@
 from . import wrap
 
 if TYPE_CHECKING:
     from typing import Union
 
 
 class WrappedChannel(wrap.Wrap, abc.GuildChannel, abc.PrivateChannel):  # type: ignore
-    @classmethod
-    async def convert(cls, ctx, argument: str) -> WrappedChannel:
-        channel: Union[
-            abc.GuildChannel, abc.PrivateChannel
-        ] = await TextChannelConverter().convert(ctx=ctx, argument=argument)
-        return cls(channel, ctx.bot)
-
     def __getattr__(self, item):
         return getattr(self._wrapped, item)
 
     def permissions_for(self, *args, **kwargs):
         if not hasattr(self, "guild"):
             return Permissions.all()
```

### Comparing `ooliver_botbase-1.22.3/botbase/wraps/inter.py` & `ooliver_botbase-2.0.1/botbase/wraps/inter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generic
 
 from nextcord import Interaction, InteractionResponse
+from nextcord.interactions import ClientT
 
 from . import wrap
 
 if TYPE_CHECKING:
-    from nextcord import VoiceProtocol, ClientUser, Member
+    from nextcord import ClientUser, Member, VoiceProtocol
 
     from ..botbase import BotBase
-    from .user import WrappedUser
     from .member import WrappedMember
+    from .user import WrappedUser
 
 
-class MyInter(wrap.Wrap, Interaction):
+class MyInter(wrap.Wrap, Interaction[ClientT], Generic[ClientT]):
     user: WrappedUser | WrappedMember
     author: WrappedUser | WrappedMember
     prefix = "/"
     clean_prefix = "/"
 
     def __init__(self, wrapped, bot: BotBase):
         self._wrapped = wrapped
@@ -38,18 +39,13 @@
     def voice_client(self) -> VoiceProtocol | None:
         return self.guild and self.guild.voice_client
 
     @property
     def me(self) -> ClientUser | Member:
         return self.guild.me if self.guild is not None else self.bot.user  # type: ignore
 
-    @property
-    def command(self) -> str | None:
-        if self.data:
-            return self.data.get("name")
-
     @property  # maybe this is why it no worky
     def response(self) -> InteractionResponse:
         return self._wrapped.response
 
     def __getattr__(self, item):
         return getattr(self._wrapped, item)
```

### Comparing `ooliver_botbase-1.22.3/botbase/wraps/wrap.py` & `ooliver_botbase-2.0.1/botbase/wraps/wrap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from nextcord import (
-    Message,
+    DMChannel,
     Embed,
-    WebhookMessage,
+    Message,
+    PartialMessageable,
     TextChannel,
     Thread,
-    DMChannel,
-    PartialMessageable,
+    WebhookMessage,
 )
 from nextcord.abc import Messageable
 from nextcord.utils import utcnow
 
 if TYPE_CHECKING:
     from typing import Any
 
+    from nextcord import Colour
+
     from ..botbase import BotBase
 
 
 channels = (TextChannel, PartialMessageable, Thread, DMChannel, Messageable)
 
 
 class Wrap:
@@ -62,63 +64,50 @@
         self,
         title: str | None = None,
         desc: str | None = None,
         *,
         author: str | None = None,
         image: str | None = None,
         thumbnail: str | None = None,
-        color=None,
+        colour: Colour | None = None,
         target=None,
         reply: bool = False,
         contain_timestamp: bool = True,
         cmd_invoker: bool = True,
         invoker_in_author: bool = False,
         try_channel: bool = False,
         **kwargs,
     ) -> Message | WebhookMessage | None:
-        from .context import MyContext
         from .channel import WrappedChannel
         from .inter import MyInter
-        from .thread import WrappedThread
         from .member import WrappedMember
+        from .thread import WrappedThread
         from .user import WrappedUser
 
-        target = target or (
-            self.message  # ctx, reply=True
-            if reply and isinstance(self, MyContext)
-            else self  # Anything else (member.send)
-        )
+        target = target or self
 
-        embed = Embed(title=title, description=desc, color=color or self._bot.color)
+        embed = Embed(title=title, description=desc, colour=colour or self._bot.colour)
 
-        if contain_timestamp and isinstance(self, MyContext):
-            # Doesnt work on Channels, Users, Members
-            embed.timestamp = self.message.created_at
-        elif contain_timestamp:
+        if contain_timestamp:
             embed.timestamp = utcnow()
 
         if cmd_invoker and not isinstance(self, (WrappedChannel, WrappedThread)):
-            if isinstance(self, (MyContext)):
-                text = self.author.display_name
-                icon_url = self.author.display_avatar.url
-            elif isinstance(self, MyInter):
+            if isinstance(self, MyInter):
                 text = self.user.display_name
                 icon_url = self.user.display_avatar.url
             elif isinstance(self, (WrappedUser, WrappedMember)):
                 text = self.display_name
                 icon_url = self.display_avatar.url
             else:
                 raise TypeError(f"{type(self).__name__} cannot get invoker")
 
             embed.set_footer(text=text, icon_url=icon_url)
 
         if author:
-            if isinstance(self, (MyContext)):
-                icon_url = self.author.display_avatar.url
-            elif isinstance(self, MyInter):
+            if isinstance(self, MyInter):
                 icon_url = self.user.display_avatar.url
             elif isinstance(self, (WrappedUser, WrappedMember)):
                 icon_url = self.display_avatar.url
             else:
                 raise TypeError(f"{type(self).__name__} cannot get invoker")
 
             if invoker_in_author:
@@ -138,19 +127,12 @@
         elif try_channel and isinstance(target, MyInter) and target.response.is_done():
             if isinstance(target.channel, channels):
                 return await target.channel.send(embed=embed, **kwargs)
             else:
                 return await target.send(embed=embed, **kwargs)  # type: ignore
         elif isinstance(
             target,
-            (
-                WrappedUser,
-                WrappedMember,
-                WrappedChannel,
-                WrappedThread,
-                MyInter,
-                MyContext,
-            ),
+            (WrappedUser, WrappedMember, WrappedChannel, WrappedThread, MyInter),
         ):
             return await target.send(embed=embed, **kwargs)  # type: ignore
         else:
             raise TypeError(f"{type(self).__name__} cannot send embeds")
```

