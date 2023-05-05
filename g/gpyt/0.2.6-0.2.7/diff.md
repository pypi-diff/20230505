# Comparing `tmp/gpyt-0.2.6.tar.gz` & `tmp/gpyt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.6.tar", max compression
+gzip compressed data, was "gpyt-0.2.7.tar", max compression
```

## Comparing `gpyt-0.2.6.tar` & `gpyt-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1060 2023-05-05 04:39:38.087304 gpyt-0.2.6/README.md
--rw-r--r--   0        0        0     1964 2023-05-05 05:05:45.027304 gpyt-0.2.6/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.6/gpyt/__main__.py
--rw-r--r--   0        0        0    14325 2023-05-05 04:57:58.727304 gpyt-0.2.6/gpyt/app.py
--rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.6/gpyt/assistant.py
--rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.6/gpyt/conversation.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.6/gpyt/exception.py
--rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.6/gpyt/id.py
--rw-r--r--   0        0        0     1152 2023-05-04 19:26:06.307304 gpyt-0.2.6/gpyt/styles.cssx
--rw-r--r--   0        0        0      494 2023-05-05 05:06:51.477304 gpyt-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 gpyt-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-05-05 05:19:46.977304 gpyt-0.2.7/README.md
+-rw-r--r--   0        0        0     1964 2023-05-05 05:05:45.027304 gpyt-0.2.7/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.7/gpyt/__main__.py
+-rw-r--r--   0        0        0    15474 2023-05-05 06:20:36.987304 gpyt-0.2.7/gpyt/app.py
+-rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.7/gpyt/assistant.py
+-rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.7/gpyt/conversation.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.7/gpyt/exception.py
+-rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.7/gpyt/id.py
+-rw-r--r--   0        0        0     1281 2023-05-05 06:09:18.137304 gpyt-0.2.7/gpyt/styles.cssx
+-rw-r--r--   0        0        0      494 2023-05-05 06:21:33.427304 gpyt-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 gpyt-0.2.7/PKG-INFO
```

### Comparing `gpyt-0.2.6/README.md` & `gpyt-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 - [ ] `new` to start a new chat (clear all history and console window)
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
 - [ ] add special error handling for RateLimiting or early stops to generation of text stream
 - [ ] gpt4free integration (for 3.5 and 4)
-
+- [ ] live upate past convo view (ctrl+s show instantly)
 
 ### Completed Features
 
 - [x] loading wheel
 - [x] textual !!!
 - [x] scrolling text (adjustable speed, or disable all together)
 - [x] use streams api?
```

### Comparing `gpyt-0.2.6/gpyt/__init__.py` & `gpyt-0.2.7/gpyt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.6/gpyt/app.py` & `gpyt-0.2.7/gpyt/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 from pathlib import Path
 from typing import Callable, Generator
+from rich.style import Style
 
 from textual import work
 from textual.app import App, ComposeResult
 from textual.containers import Container, ScrollableContainer
 from textual.reactive import reactive
 from textual.widgets import (
     Button,
@@ -34,22 +35,24 @@
 
     save -> save the current conversation to disk
     """
 
     def __init__(self):
         super().__init__()
         self.keyword_mappings: dict[str, Callable] = {
-            "save": app.save_active_conversation_to_disk,
+            # "save": app.save_active_conversation_to_disk,
             "new": app.start_new_conversation,
             "clear": app.start_new_conversation,
         }
 
     def compose(self) -> ComposeResult:
         yield Label(f"🤖: {INTRO}", id="help-text")
-        yield Input(placeholder="How far away is the Sun?", id="user-input")
+        self.inp = Input(placeholder="How far away is the Sun?", id="user-input")
+        self.inp.focus()
+        yield self.inp
 
     async def on_input_submitted(self, event: Input.Submitted) -> None:
         user_input = event.input.value
         event.input.value = ""
 
         # empty queries are useless
         if len(user_input) < 1:
@@ -83,15 +86,22 @@
     def select(self) -> None:
         # app.assistant_responses.setup_from_presaved_conversation(self.conversation)
         app.on_select_previous_conversation(self.conversation)
 
 
 class StartNewConversationOption(ListItem):
     def compose(self) -> ComposeResult:
-        yield Label("Start a new conversation")
+        yield Label("<-- Start a new conversation -->", id="new-convo-option")
+
+    def watch_highlighted(self, value: bool) -> None:
+        super().watch_highlighted(value)
+        if value:
+            self.add_class("highlighted")
+        else:
+            self.remove_class("highlighted")
 
     def select(self) -> None:
         app.start_new_conversation()
 
 
 class VimLikeListView(ListView):
     BINDINGS = [("j", "cursor_down", "Cursor Down"), ("k", "cursor_up", "Cursor Up")]
@@ -157,35 +167,40 @@
     def setup_from_presaved_conversation(self, conversation: Conversation) -> None:
         """Load conversation into conversation history widget from Conversation model"""
 
         app.active_conversation = conversation
         app._set_summary_title_id(conversation.summary, conversation.id)
         new_history = []
 
-        for i in range(0, len(conversation.log) - 1, 2):
-            user_message = conversation.log[i]
+        all_user_messages = [m for m in conversation.log if m.role == "user"]
+        all_assistant_messages = [m for m in conversation.log if m.role == "assistant"]
+
+        for user_message, assistant_response in zip(
+            all_user_messages, all_assistant_messages
+        ):
             assert (
                 user_message.role == "user"
             ), "Improper role for setup from presaved convesation"
 
-            assistant_response = conversation.log[i + 1]
             new_response = AssistantResponse(
                 question=user_message.content, id=user_message.id
             )
             self.container.mount(new_response)
             assert (
                 assistant_response.role == "assistant"
             ), "Improper role for setup from presaved convesation"
             new_response.update_response(assistant_response.content)
             new_history.append({"role": "user", "content": user_message.content})
             new_history.append(
                 {"role": "assistant", "content": assistant_response.content}
             )
 
         app.assistant.set_history(new_history)
+        app.action_toggle_sidebar()
+        app.focus_user_input()
 
     @work()
     def add_response(self, stream: Generator, message: Message) -> None:
         new_response = AssistantResponse(question=message.content, id=message.id)
         app.call_from_thread(self.container.mount, new_response)
         app.call_from_thread(new_response.scroll_visible)
         markdown = ""
@@ -207,31 +222,33 @@
             new_response.user_question.scroll_visible, duration=2, easing="out_back"
         )
         app.assistant.log_assistant_response(markdown)
         assistant_message = Message(id=get_id(), role="assistant", content=markdown)
         assert app.active_conversation, "No active conversation during log write"
         app.active_conversation.log.append(assistant_message)
 
+        app.call_from_thread(app.save_active_conversation_to_disk)
+
 
 class AssistantApp(App):
     """Base app for all user->assistant interactions"""
 
     BINDINGS = [
         ("ctrl+b", "toggle_dark", "Toggle Dark Mode"),
         ("ctrl+n", "toggle_sidebar", "Past Conversations"),
-        ("ctrl+s", "save_conversation", "Save Conversation"),
     ]
 
     CSS_PATH = "styles.cssx"
 
     def __init__(self, assistant: Assistant):
         super().__init__()
         self.assistant = assistant
         self.conversations: list[Conversation] = []
         self.active_conversation: Conversation | None = None
+        self._convo_ids_added: set[str] = set()
 
     def compose(self) -> ComposeResult:
         header = Header(show_clock=True)
         header.tall = False
         yield header
         yield Footer()
         self.assistant_responses = AssistantResponses()
@@ -257,30 +274,28 @@
         return Path(
             GPT_CACHE_DIR if GPT_CACHE_DIR else HOME_DIR,  # type: ignore
             ".cache",
             "gpyt",
             "conversations",
         )
 
-    def action_save_conversation(self) -> None:
-        self.save_active_conversation_to_disk()
-
     def load_saved_conversations(self) -> None:
         """Load conversations from saved conversation path"""
         conversations_path = self.get_saved_conversations_path()
         conversation_file_paths = conversations_path.glob(pattern=r"*.json")
         conversation_file_paths = sorted(
             conversation_file_paths, key=lambda f: f.stat().st_mtime
         )
 
         for path in conversation_file_paths:
             with open(path, "r") as fd:
                 raw_json = json.load(fd)
                 conversation = Conversation.parse_obj(raw_json)
                 self.conversations.append(conversation)
+                self._convo_ids_added.add(conversation.id)
                 self.past_conversations.add_conversation_option(conversation)
 
     def save_active_conversation_to_disk(self) -> str:
         """Save the active conversation to disk and return the file path"""
         return self.save_conversation_to_disk()
 
     def save_conversation_to_disk(
@@ -291,23 +306,26 @@
         Will use active conversation if no conversation is given.
         """
         if not conversation:
             assert (
                 self.active_conversation
             ), "When not supplied a conversation to save to disk, there must be an active conversation!"
             conversation = self.active_conversation
+        print("SAVING: ", conversation.id)
 
         conversations_path = self.get_saved_conversations_path()
 
         os.makedirs(conversations_path, exist_ok=True)
 
         path = Path(conversations_path, f"convo-{conversation.id}.json")
         with open(path, "w") as fd:
             json.dump(conversation.dict(), fd)
 
+        self._add_active_as_option()
+
         return str(path)
 
     def _set_summary_title_id(self, summary: str, id: str) -> None:
         self.assistant_responses.border_title = f"Conversation History - {summary}"
         self.assistant_responses.border_subtitle = f"convo-id: 0x{id}"
 
     def _setup_fresh_convo(self, initial_user_input: str) -> None:
@@ -319,29 +337,39 @@
 
     def clear_active_conversation(self) -> None:
         self.assistant_responses.remove()
         self.assistant_responses = AssistantResponses()
         self.mount(self.assistant_responses)
         self.assistant_responses.border_title = "Conversation History"
 
-    def start_new_conversation(self, save_current: bool = True) -> None:
-        """Save current conversation, clear it, start a new fresh one"""
+    def _add_active_as_option(self) -> None:
         if not self.active_conversation:
             return
-
-        self.save_active_conversation_to_disk()
-        self.clear_active_conversation()
         exists_already = Path(
             self.get_saved_conversations_path(),
             f"convo-{self.active_conversation.id}.json",
         ).exists()
 
-        if save_current and not exists_already:
+        if exists_already and self.active_conversation.id not in self._convo_ids_added:
             self.past_conversations.add_conversation_option(self.active_conversation)
+
+        self._convo_ids_added.add(self.active_conversation.id)
+
+    def start_new_conversation(self, add_option: bool = True) -> None:
+        """Save current conversation, clear it, start a new fresh one"""
+        if not self.active_conversation:
+            return
+
+        self.save_active_conversation_to_disk()
+        if add_option:
+            self._add_active_as_option()
+        self.clear_active_conversation()
         self.active_conversation = None
+        self.action_toggle_sidebar()
+        self.focus_user_input()
 
     @work()
     def fetch_assistant_response(self, user_input: str) -> None:
         if self.active_conversation is None:
             self._setup_fresh_convo(user_input)
 
         assert self.active_conversation, "No active conversation during log write"
@@ -356,16 +384,17 @@
         app.call_from_thread(
             self.assistant_responses.add_response,
             message=user_message,
             stream=assistant_response_stream,
         )
 
     def on_select_previous_conversation(self, conversation: Conversation) -> None:
-        self.start_new_conversation(save_current=False)
+        self.start_new_conversation(add_option=False)
         self.assistant_responses.setup_from_presaved_conversation(conversation)
+        self.assistant_responses.container.scroll_end(duration=2.0, easing="in_quart")
 
     def action_toggle_dark(self) -> None:
         self.dark = not self.dark
 
     def action_toggle_sidebar(self) -> None:
         if not self.past_conversations.has_class("opened-gt-once"):
             try:
@@ -378,14 +407,18 @@
                         log=[],
                     )
                 )
         self.past_conversations.add_class("opened-gt-once")
         self.past_conversations.toggle_class("hidden")
         self.set_focus(self.past_conversations.options)
 
+    def focus_user_input(self) -> None:
+        inp = self.query_one("#user-input")
+        inp.focus()
+
 
 class gpyt(AssistantApp):
     """Used strictly for the purposes of renaming the Header widget."""
 
     def __init__(self, assistant: Assistant):
         super().__init__(assistant=assistant)
```

### Comparing `gpyt-0.2.6/gpyt/assistant.py` & `gpyt-0.2.7/gpyt/assistant.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.6/gpyt/id.py` & `gpyt-0.2.7/gpyt/id.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.6/gpyt/styles.cssx` & `gpyt-0.2.7/gpyt/styles.cssx`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-* {
-  transition: color 1000ms in_quint;
-}
 
 Screen {
   overflow: hidden;
   layers: base overlay;
 }
 
 UserInput {
@@ -70,7 +67,17 @@
 PastConversations:focus-within {
   offset-x: 0 !important;
 }
 
 PastConversations.hidden {
   offset-x: -100%;
 }
+
+StartNewConversationOption {
+  text-style: italic;
+  color: $primary-lighten-3;
+  align: center middle;
+}
+
+StartNewConversationOption.highlighted {
+  color: $secondary;
+}
```

### Comparing `gpyt-0.2.6/PKG-INFO` & `gpyt-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.6
+Version: 0.2.7
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
@@ -45,15 +45,15 @@
 - [ ] `new` to start a new chat (clear all history and console window)
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
 - [ ] add special error handling for RateLimiting or early stops to generation of text stream
 - [ ] gpt4free integration (for 3.5 and 4)
-
+- [ ] live upate past convo view (ctrl+s show instantly)
 
 ### Completed Features
 
 - [x] loading wheel
 - [x] textual !!!
 - [x] scrolling text (adjustable speed, or disable all together)
 - [x] use streams api?
```

