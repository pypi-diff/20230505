# Comparing `tmp/gpyt-0.2.5.tar.gz` & `tmp/gpyt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.5.tar", max compression
+gzip compressed data, was "gpyt-0.2.6.tar", max compression
```

## Comparing `gpyt-0.2.5.tar` & `gpyt-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      892 2023-05-03 06:35:37.777304 gpyt-0.2.5/README.md
--rw-r--r--   0        0        0     1906 2023-05-03 03:53:32.417304 gpyt-0.2.5/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.5/gpyt/__main__.py
--rw-r--r--   0        0        0     1863 2023-05-03 03:53:32.417304 gpyt-0.2.5/gpyt/_app.py
--rw-r--r--   0        0        0     4660 2023-05-03 20:39:43.137304 gpyt-0.2.5/gpyt/app.py
--rw-r--r--   0        0        0     2044 2023-05-03 06:34:17.987304 gpyt-0.2.5/gpyt/assistant.py
--rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.2.5/gpyt/debug.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.5/gpyt/exception.py
--rw-r--r--   0        0        0      780 2023-05-03 06:34:17.987304 gpyt-0.2.5/gpyt/styles.cssx
--rw-r--r--   0        0        0      427 2023-05-03 20:39:50.347304 gpyt-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 gpyt-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-05 04:39:38.087304 gpyt-0.2.6/README.md
+-rw-r--r--   0        0        0     1964 2023-05-05 05:05:45.027304 gpyt-0.2.6/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.6/gpyt/__main__.py
+-rw-r--r--   0        0        0    14325 2023-05-05 04:57:58.727304 gpyt-0.2.6/gpyt/app.py
+-rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.6/gpyt/assistant.py
+-rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.6/gpyt/conversation.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.6/gpyt/exception.py
+-rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.6/gpyt/id.py
+-rw-r--r--   0        0        0     1152 2023-05-04 19:26:06.307304 gpyt-0.2.6/gpyt/styles.cssx
+-rw-r--r--   0        0        0      494 2023-05-05 05:06:51.477304 gpyt-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 gpyt-0.2.6/PKG-INFO
```

### Comparing `gpyt-0.2.5/README.md` & `gpyt-0.2.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 ```
 
 ### Desired Features
 
 - [ ] `copy` to copy GPT's response to clipboard
 - [ ] add gpt jailbreaks (DAN-esque)
 - [ ] `new` to start a new chat (clear all history and console window)
-- [ ] store chat logs somewhere.
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
+- [ ] add special error handling for RateLimiting or early stops to generation of text stream
+- [ ] gpt4free integration (for 3.5 and 4)
 
 
 ### Completed Features
 
 - [x] loading wheel
 - [x] textual !!!
 - [x] scrolling text (adjustable speed, or disable all together)
 - [x] use streams api?
+- [x] store chat logs somewhere.
+- [x] load saved conversations
```

### Comparing `gpyt-0.2.5/gpyt/__init__.py` & `gpyt-0.2.6/gpyt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import argparse
 import os
 
 from dotenv import find_dotenv, get_key
 
 ENV_PATH = find_dotenv()
 
 API_KEY = get_key(dotenv_path=ENV_PATH, key_to_get="OPENAI_API_KEY")
@@ -10,15 +9,27 @@
 # try to get from os envrionment variables
 
 if API_KEY is None:
     API_KEY = os.getenv("OPENAI_API_KEY") or None
 
 assert (
     API_KEY is not None
-), "⚠ Missing API KEY: Please set one in your `.env` via `OPENAI_API_KEY=<your_key>` or using your OS's enviroment variables like `export OPENAI_API_KEY=<my_key>`⚠"
+), """
+
+❗Missing OpenAI API Key ❗
+
+Steps to fix this issue:
+
+    1) Get an OpenAI Key from https://platform.openai.com/account/api-keys
+    2) Create a `.env` file located in your $HOME directory.
+    3) add `OPENAI_API_KEY="your_api_key"` to the `.env` file.
+    4) or, you can run `$ EXPORT OPENAI_API_KEY="your_api_key"` to set a key for the active shell session.
+    5) rerun this program with `$ gpyt` or `$ python -m gpyt`
+
+"""
 
 PROMPT = """
 You are a helpful assistant. Be accurate and concise with your responses.
 You are being used as a command-line tool by the user and you may be asked
 technical/programming type questions.
 
 Use basic Markdown syntax.
@@ -36,39 +47,21 @@
 # Football
 
 <the rest of your response>
 
 --end intermediate to complex topics instructions--
 """
 
+SUMMARY_PROMPT = "Summarize the user's input in 6 words or less. Try to capture the big idea. DO NOT USE more than 6 words and DO NOT answer their question. Simply echo back to them your summary."
+API_ERROR_FALLBACK = [
+    {
+        "choices": [
+            {"delta": {"content": "There was an error with OpenAI, try again later."}}
+        ]
+    }
+]
+
+
 INTRO = "Ask me anything. I'll try to assist you!"
 
 AVAILABLE_MODELS = ("gpt-3.5-turbo", "gpt4")
 MODEL = "gpt-3.5-turbo"
-
-arg_parser = argparse.ArgumentParser(
-    prog="gpyt", description="Infer with GPT on the command line!"
-)
-
-arg_parser.add_argument(
-    "--no-memory",
-    action="store_true",
-    required=False,
-    default=False,
-    help="Disable assistant memory during conversation. (saves tokens, $$$)",
-)
-
-arg_parser.add_argument(
-    "--debug",
-    action="store_true",
-    required=False,
-    default=False,
-    help="Enable debug mode (for development).",
-)
-
-
-ARGS = arg_parser.parse_args()
-
-DEBUG = ARGS.debug
-
-if DEBUG:
-    print(f"🔧: {ENV_PATH=}")
```

### Comparing `gpyt-0.2.5/gpyt/assistant.py` & `gpyt-0.2.6/gpyt/assistant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,48 @@
-import openai
 from typing import Generator
 
+import openai
+
+from gpyt import API_ERROR_FALLBACK, SUMMARY_PROMPT
+
 
 class Assistant:
     """
     Represents an OpenAI GPT assistant.
 
     It can generate responses based on user input and conversation history.
     """
 
-    def __init__(self, *, api_key: str, model: str, prompt: str, memory: bool = True):
+    kDEFAULT_PROMPT_FALLTHROUGH = "User Question"
+
+    def __init__(
+        self,
+        *,
+        api_key: str,
+        model: str,
+        prompt: str,
+        memory: bool = True,
+    ):
         self.api_key = api_key
         self.model = model
         self.prompt = prompt
+        self.summary_prompt = SUMMARY_PROMPT
         self.memory = memory
         self.messages = [
             {"role": "system", "content": self.prompt},
         ]
+        self.error_fallback_message = API_ERROR_FALLBACK
         openai.api_key = self.api_key
 
+    def set_history(self, new_history: list):
+        """Reassign all message history except for system message"""
+        sys_prompt = self.messages[0]
+        self.messages = new_history[::]
+        self.messages.insert(0, sys_prompt)
+
     def clear_history(self):
         """
         Wipe all message history during this conversation, except for the
         first system message
         """
         self.messages = [self.messages[0]]
 
@@ -41,30 +61,51 @@
             model=self.model,
             messages=self.messages,
             stream=True,
         )
 
         return response  # type: ignore
 
+    def get_response(self, user_input: str) -> str:
+        """Get an entire string back from the assistant"""
+        messages = [
+            {"role": "system", "content": self.summary_prompt},
+            {"role": "user", "content": user_input.rstrip()},
+        ]
+        response = openai.ChatCompletion.create(model=self.model, messages=messages)
+
+        return response["choices"][0]["message"]["content"]  # type: ignore
+
+    def get_conversation_summary(self, initial_message: str) -> str:
+        """Generate a short 6 word or less summary of the user\'s first message"""
+        try:
+            summary = self.get_response(initial_message)
+        except:
+            return Assistant.kDEFAULT_PROMPT_FALLTHROUGH
+
+        return summary
+
     def log_assistant_response(self, final_response: str) -> None:
         if not self.memory:
             return
 
         self.messages.append({"role": "assistant", "content": final_response})
 
 
 def _test() -> None:
     from gpyt import API_KEY, MODEL, PROMPT
 
     gpt = Assistant(api_key=API_KEY or "", model=MODEL, prompt=PROMPT)
 
-    # response = gpt.get_response("Hi, how are you!")
-    response_iterator = gpt.get_response_stream("hi how are you!")
-    for response in response_iterator:
-        try:
-            print(response["choices"][0]["delta"]["content"], end="", flush=True)
-        except:
-            continue
+    # response = gpt.get_response("How do I make carrot cake?")
+    summary = gpt.get_conversation_summary("How do I get into Dirt Biking?")
+    print(f"{summary = }")
+    # response_iterator = gpt.get_response_stream("hi how are you!")
+    # for response in response_iterator:
+    #     try:
+    #         print(response["choices"][0]["delta"]["content"], end="", flush=True)
+    #     except:
+    #         continue
 
 
 if __name__ == "__main__":
     _test()
```

### Comparing `gpyt-0.2.5/gpyt/styles.cssx` & `gpyt-0.2.6/gpyt/styles.cssx`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 * {
   transition: color 1000ms in_quint;
 }
 
 Screen {
   overflow: hidden;
+  layers: base overlay;
 }
 
 UserInput {
   border: panel $primary-background;
   background: $surface-lighten-1;
   margin: 2;
   margin-top: 3;
+  height: 10;
   padding: 1;
   dock: bottom;
   border-subtitle-color: $surface-lighten-3;
 }
 
 AssistantResponses {
   border: panel $primary-background-lighten-1;
   margin: 1;
   border-title-align: center;
-  border-title-color: $text-muted;
+  border-title-color: rgb(225,225,225);
   background: $surface-lighten-1;
 }
 
 AssistantResponse {
   padding: 1;
 }
 
@@ -49,7 +51,26 @@
 .convo {
   margin: 1;
 }
 
 LoadingIndicator {
   height: 1;
 }
+
+PastConversations {
+  layer: overlay;
+  margin-top: 1;
+  width: 40;
+  height: 60%;
+  border: panel $panel-lighten-2;
+  border-title-color: rgb(225,225,225);
+  background: $panel;
+  transition: offset 400ms in_back;
+}
+
+PastConversations:focus-within {
+  offset-x: 0 !important;
+}
+
+PastConversations.hidden {
+  offset-x: -100%;
+}
```

### Comparing `gpyt-0.2.5/PKG-INFO` & `gpyt-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.5
+Version: 0.2.6
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: openai-async (>=0.0.3,<0.0.4)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: textual[dev] (>=0.22.3,<0.23.0)
 Description-Content-Type: text/markdown
 
 # gpyt
 
@@ -38,21 +39,24 @@
 ```
 
 ### Desired Features
 
 - [ ] `copy` to copy GPT's response to clipboard
 - [ ] add gpt jailbreaks (DAN-esque)
 - [ ] `new` to start a new chat (clear all history and console window)
-- [ ] store chat logs somewhere.
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
+- [ ] add special error handling for RateLimiting or early stops to generation of text stream
+- [ ] gpt4free integration (for 3.5 and 4)
 
 
 ### Completed Features
 
 - [x] loading wheel
 - [x] textual !!!
 - [x] scrolling text (adjustable speed, or disable all together)
 - [x] use streams api?
+- [x] store chat logs somewhere.
+- [x] load saved conversations
```

