# Comparing `tmp/ovos-tts-server-0.0.2.tar.gz` & `tmp/ovos-tts-server-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-server-0.0.2.tar", last modified: Thu Feb 17 22:54:05 2022, max compression
+gzip compressed data, was "ovos-tts-server-0.0.2a3.tar", last modified: Fri May  5 03:15:24 2023, max compression
```

## Comparing `ovos-tts-server-0.0.2.tar` & `ovos-tts-server-0.0.2a3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-02-17 22:54:05.069770 ovos-tts-server-0.0.2/
--rw-r--r--   0 user      (1000) user      (1000)    11347 2022-02-17 14:42:43.000000 ovos-tts-server-0.0.2/LICENSE.md
--rw-r--r--   0 user      (1000) user      (1000)     1054 2022-02-17 22:54:05.069770 ovos-tts-server-0.0.2/PKG-INFO
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-02-17 22:54:05.066437 ovos-tts-server-0.0.2/ovos_tts_server/
--rw-r--r--   0 user      (1000) user      (1000)     1907 2022-02-17 22:42:35.000000 ovos-tts-server-0.0.2/ovos_tts_server/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1187 2022-02-17 14:22:33.000000 ovos-tts-server-0.0.2/ovos_tts_server/__main__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-02-17 22:54:05.069770 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1054 2022-02-17 22:54:05.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      345 2022-02-17 22:54:05.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-02-17 22:54:05.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       67 2022-02-17 22:54:05.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       33 2022-02-17 22:54:05.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       16 2022-02-17 22:54:05.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-02-17 14:44:20.000000 ovos-tts-server-0.0.2/ovos_tts_server.egg-info/zip-safe
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-02-17 22:54:05.069770 ovos-tts-server-0.0.2/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)     1360 2022-02-17 22:52:20.000000 ovos-tts-server-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/ovos_tts_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/ovos_tts_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:15:24.000000 ovos-tts-server-0.0.2a3/ovos_tts_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:15:24.657391 ovos-tts-server-0.0.2a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-05-05 03:15:23.000000 ovos-tts-server-0.0.2a3/setup.py
```

### Comparing `ovos-tts-server-0.0.2/LICENSE.md` & `ovos-tts-server-0.0.2a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.2/ovos_tts_server/__init__.py` & `ovos-tts-server-0.0.2a3/ovos_tts_server/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,53 +5,45 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-from flask import Flask, send_file, request
-from ovos_plugin_manager.tts import load_tts_plugin
-from ovos_plugin_manager.utils.tts_cache import hash_sentence
 
-TTS = None
+import uvicorn
 
+from fastapi import FastAPI
+from fastapi.responses import FileResponse
+from ovos_plugin_manager.tts import load_tts_plugin
+from ovos_utils.log import LOG
+from starlette.requests import Request
 
-def get_tts(sentence, voice=None, lang=None):
-    global TTS
-    sentence_hash = hash_sentence(sentence)
-    cache = TTS.get_cache(lang=lang, voice=voice)
-    if sentence_hash in cache:  # load from cache
-        audio_file, phonemes = TTS._get_from_cache(sentence, sentence_hash, lang=lang, voice=voice)
-    else:  # synth + cache
-        audio_file, phonemes = TTS._synth(sentence, sentence_hash, lang=lang, voice=voice)
-    return audio_file.path
+TTS = None
 
 
 def create_app():
-    app = Flask(__name__)
+    app = FastAPI()
 
-    @app.route("/synthesize/<utterance>", methods=['GET'])
-    def synth(utterance):
-        lang = request.args.get("lang")
-        voice = request.args.get("voice")
-        audio = get_tts(utterance, lang=lang, voice=voice)
-        return send_file(audio, mimetype="audio/wav")
+    @app.get("/synthesize/{utterance}")
+    def synth(utterance: str, request: Request):
+        LOG.debug(f"{utterance}|{request.query_params}")
+        utterance = TTS.validate_ssml(utterance)
+        audio, phonemes = TTS.synth(utterance, **request.query_params)
+        return FileResponse(audio.path)
 
     return app
 
 
-def start_tts_server(engine, port=9666, host="0.0.0.0", cache=False):
+def start_tts_server(engine, cache=False):
     global TTS
 
     # load ovos TTS plugin
     engine = load_tts_plugin(engine)
 
     TTS = engine(config={"persist_cache": cache})  # this will cache every synth even across reboots
     TTS.log_timestamps = True  # enable logging
 
     app = create_app()
-    app.run(port=port, use_reloader=False, host=host)
-    return app
+    return app, TTS
```

### Comparing `ovos-tts-server-0.0.2/ovos_tts_server/__main__.py` & `ovos-tts-server-0.0.2a3/ovos_tts_server/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,50 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
+
+import uvicorn
+
 from ovos_tts_server import start_tts_server
+from ovos_tts_server.gradio_app import bind_gradio_service
+from ovos_utils.log import LOG
 
 
 def main():
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--engine", help="tts plugin to be used")
     parser.add_argument("--port", help="port number",
                         default=9666)
     parser.add_argument("--host", help="host",
                         default="0.0.0.0")
     parser.add_argument("--cache", help="save every synth to disk",
                         action="store_true")
+    parser.add_argument("--lang", help="default language supported by plugin",
+                        default="en-us")
+    parser.add_argument("--gradio", help="Enable Gradio Web UI",
+                        action="store_true")
+    parser.add_argument("--title", help="Title for webUI",
+                        default="TTS")
+    parser.add_argument("--description", help="Text description to print in UI",
+                        default="Get Text-to-Speech")
+    parser.add_argument("--info", help="Text to display at end of UI",
+                        default=None)
+    parser.add_argument("--badge", help="URL of visitor badge", default=None)
     args = parser.parse_args()
 
-    start_tts_server(args.engine, port=args.port, host=args.host, cache=bool(args.cache))
+    server, engine = start_tts_server(args.engine, cache=bool(args.cache))
+    LOG.info("Server Started")
+    if args.gradio:
+        bind_gradio_service(server, engine, args.title, args.description,
+                            args.info, args.badge, args.lang)
+        LOG.info("Gradio Started")
+    uvicorn.run(server, host=args.host, port=args.port)
 
 
 if __name__ == "__main__":
     main()
```

