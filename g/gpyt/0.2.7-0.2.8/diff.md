# Comparing `tmp/gpyt-0.2.7.tar.gz` & `tmp/gpyt-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.7.tar", max compression
+gzip compressed data, was "gpyt-0.2.8.tar", max compression
```

## Comparing `gpyt-0.2.7.tar` & `gpyt-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1116 2023-05-05 05:19:46.977304 gpyt-0.2.7/README.md
--rw-r--r--   0        0        0     1964 2023-05-05 05:05:45.027304 gpyt-0.2.7/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.7/gpyt/__main__.py
--rw-r--r--   0        0        0    15474 2023-05-05 06:20:36.987304 gpyt-0.2.7/gpyt/app.py
--rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.7/gpyt/assistant.py
--rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.7/gpyt/conversation.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.7/gpyt/exception.py
--rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.7/gpyt/id.py
--rw-r--r--   0        0        0     1281 2023-05-05 06:09:18.137304 gpyt-0.2.7/gpyt/styles.cssx
--rw-r--r--   0        0        0      494 2023-05-05 06:21:33.427304 gpyt-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 gpyt-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      859 2023-05-05 06:36:00.377304 gpyt-0.2.8/README.md
+-rw-r--r--   0        0        0     1964 2023-05-05 05:05:45.027304 gpyt-0.2.8/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.8/gpyt/__main__.py
+-rw-r--r--   0        0        0    15622 2023-05-05 06:26:52.067304 gpyt-0.2.8/gpyt/app.py
+-rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.8/gpyt/assistant.py
+-rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.8/gpyt/conversation.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.8/gpyt/exception.py
+-rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.8/gpyt/id.py
+-rw-r--r--   0        0        0     1281 2023-05-05 06:09:18.137304 gpyt-0.2.8/gpyt/styles.cssx
+-rw-r--r--   0        0        0      494 2023-05-05 06:36:30.377304 gpyt-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 gpyt-0.2.8/PKG-INFO
```

### Comparing `gpyt-0.2.7/gpyt/__init__.py` & `gpyt-0.2.8/gpyt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.7/gpyt/app.py` & `gpyt-0.2.8/gpyt/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,14 @@
             new_history.append({"role": "user", "content": user_message.content})
             new_history.append(
                 {"role": "assistant", "content": assistant_response.content}
             )
 
         app.assistant.set_history(new_history)
         app.action_toggle_sidebar()
-        app.focus_user_input()
 
     @work()
     def add_response(self, stream: Generator, message: Message) -> None:
         new_response = AssistantResponse(question=message.content, id=message.id)
         app.call_from_thread(self.container.mount, new_response)
         app.call_from_thread(new_response.scroll_visible)
         markdown = ""
@@ -231,14 +230,15 @@
 
 class AssistantApp(App):
     """Base app for all user->assistant interactions"""
 
     BINDINGS = [
         ("ctrl+b", "toggle_dark", "Toggle Dark Mode"),
         ("ctrl+n", "toggle_sidebar", "Past Conversations"),
+        ("ctrl+c", "handle_exit", "Quit"),
     ]
 
     CSS_PATH = "styles.cssx"
 
     def __init__(self, assistant: Assistant):
         super().__init__()
         self.assistant = assistant
@@ -361,15 +361,14 @@
 
         self.save_active_conversation_to_disk()
         if add_option:
             self._add_active_as_option()
         self.clear_active_conversation()
         self.active_conversation = None
         self.action_toggle_sidebar()
-        self.focus_user_input()
 
     @work()
     def fetch_assistant_response(self, user_input: str) -> None:
         if self.active_conversation is None:
             self._setup_fresh_convo(user_input)
 
         assert self.active_conversation, "No active conversation during log write"
@@ -405,20 +404,26 @@
                         summary=f"Failed to load conversations from {self.get_saved_conversations_path()}",
                         id="-1",
                         log=[],
                     )
                 )
         self.past_conversations.add_class("opened-gt-once")
         self.past_conversations.toggle_class("hidden")
+        if self.past_conversations.has_class("hidden"):
+            app.focus_user_input()
+            return
         self.set_focus(self.past_conversations.options)
 
     def focus_user_input(self) -> None:
         inp = self.query_one("#user-input")
         inp.focus()
 
+    def action_handle_exit(self) -> None:
+        exit()
+
 
 class gpyt(AssistantApp):
     """Used strictly for the purposes of renaming the Header widget."""
 
     def __init__(self, assistant: Assistant):
         super().__init__(assistant=assistant)
```

### Comparing `gpyt-0.2.7/gpyt/assistant.py` & `gpyt-0.2.8/gpyt/assistant.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.7/gpyt/id.py` & `gpyt-0.2.8/gpyt/id.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.7/gpyt/styles.cssx` & `gpyt-0.2.8/gpyt/styles.cssx`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.7/PKG-INFO` & `gpyt-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.7
+Version: 0.2.8
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
@@ -13,50 +13,44 @@
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: textual[dev] (>=0.22.3,<0.23.0)
 Description-Content-Type: text/markdown
 
 # gpyt
 
-TUI GPT frontend on the command line with Textual.
+> GPT in your terminal.
 
-> WIP
+>> WIP
 
 
 ## Demo
 
-![gpyt demo](./media/gpyt-show-1.gif)
+![gpyt demo](https://github.com/JustinStitt/gpyt/blob/master/media/gpyt-show-1.gif?raw=true)
 
 Uses [Textual](https://textual.textualize.io).
 
 
-### How to run:
-```sh
-$ pip install gpyt
+### Installation & Usage
+1) `$ pip install gpyt`
 
-add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
+2) add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME or `export OPENAI_API_KEY=<your_key>`
 
-$ python -m gpyt
-```
+3) `$ gpyt`
 
-### Desired Features
+### Keybindings
+
+* `ctrl-b` -> Toggle Dark/Light Mode
+* `ctrl-n` -> Open Past Conversations Sidebar
+* `ctrl-c` -> Quit
+
+
+### TODO
 
 - [ ] `copy` to copy GPT's response to clipboard
 - [ ] add gpt jailbreaks (DAN-esque)
-- [ ] `new` to start a new chat (clear all history and console window)
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
-- [ ] add special error handling for RateLimiting or early stops to generation of text stream
 - [ ] gpt4free integration (for 3.5 and 4)
-- [ ] live upate past convo view (ctrl+s show instantly)
-
-### Completed Features
-
-- [x] loading wheel
-- [x] textual !!!
-- [x] scrolling text (adjustable speed, or disable all together)
-- [x] use streams api?
-- [x] store chat logs somewhere.
-- [x] load saved conversations
+- [ ] refactor the f**k out of `app.py`
```

