# Comparing `tmp/joern_lib-0.7.1.tar.gz` & `tmp/joern_lib-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.7.1.tar", max compression
+gzip compressed data, was "joern_lib-0.7.2.tar", max compression
```

## Comparing `joern_lib-0.7.1.tar` & `joern_lib-0.7.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-04 20:10:33.342101 joern_lib-0.7.1/LICENSE
--rw-r--r--   0        0        0     3441 2023-05-04 20:10:33.342101 joern_lib-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/__init__.py
--rw-r--r--   0        0        0     8105 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/client.py
--rw-r--r--   0        0        0        0 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/c.py
--rw-r--r--   0        0        0     7124 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     2814 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/java.py
--rw-r--r--   0        0        0     3914 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/detectors/js.py
--rw-r--r--   0        0        0    10805 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/utils.py
--rw-r--r--   0        0        0     4535 2023-05-04 20:10:33.354101 joern_lib-0.7.1/joern_lib/workspace.py
--rw-r--r--   0        0        0     1188 2023-05-04 20:10:33.354101 joern_lib-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 joern_lib-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-02 22:16:36.336281 joern_lib-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3722 2023-05-04 20:26:07.824853 joern_lib-0.7.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-04 21:19:10.842784 joern_lib-0.7.2/joern_lib/__init__.py
+-rw-r--r--   0        0        0     9514 2023-05-04 23:50:46.832580 joern_lib-0.7.2/joern_lib/client.py
+-rw-r--r--   0        0        0       61 2023-05-04 21:19:10.842784 joern_lib-0.7.2/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-04-28 20:22:02.075618 joern_lib-0.7.2/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0     8445 2023-05-04 23:14:53.536043 joern_lib-0.7.2/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     2814 2023-05-04 20:09:52.512192 joern_lib-0.7.2/joern_lib/detectors/java.py
+-rw-r--r--   0        0        0     3914 2023-04-02 22:16:36.347281 joern_lib-0.7.2/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0    11061 2023-05-04 22:05:54.090370 joern_lib-0.7.2/joern_lib/utils.py
+-rw-r--r--   0        0        0     4535 2023-04-28 20:22:02.075618 joern_lib-0.7.2/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1206 2023-05-05 00:13:27.557001 joern_lib-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 joern_lib-0.7.2/PKG-INFO
```

### Comparing `joern_lib-0.7.1/LICENSE` & `joern_lib-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.1/README.md` & `joern_lib-0.7.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Introduction
 
-High level python library to interact with a Joern [server](https://docs.joern.io/server).
+This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods are offered to perform code analysis on complex code bases without knowing [CPGQL](https://docs.joern.io/c-syntaxtree).
 
 ```
 pip install joern-lib
 ```
 
 The repository includes docker compose configuration to interactively query the joern server with polynote notebooks.
 
@@ -12,14 +12,20 @@
 
 ![polynote interface](docs/note2.jpg)
 
 ![polynote interface](docs/note3.jpg)
 
 ![polynote interface](docs/note4.jpg)
 
+![polynote interface](docs/sqli.jpg)
+
+![polynote interface](docs/repl.jpg)
+
+![polynote interface](docs/call-tree.jpg)
+
 ## Usage
 
 Run joern server and polynote locally.
 
 ```
 git clone https://github.com/appthreat/joern-lib.git
 # Edit docker-compose.yml to set sources directory
```

### Comparing `joern_lib-0.7.1/joern_lib/client.py` & `joern_lib-0.7.2/joern_lib/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,47 +5,57 @@
 import orjson
 import uvloop
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 import websockets
 
-from joern_lib.utils import print_md, print_table
+from joern_lib.utils import print_flows, print_md, print_table
 
 headers = {"Content-Type": "application/json", "Accept-Encoding": "gzip"}
 CLIENT_TIMEOUT = os.getenv("HTTP_CLIENT_TIMEOUT")
 
 
 class Connection:
+    """
+    Connection object to hold following connections:
+       - Websocket to joern server
+       - http connection to joern server
+       - http connection to cpggen server
+    """
+
     def __init__(self, cpggenclient, httpclient, websocket):
         self.cpggenclient = cpggenclient
         self.httpclient = httpclient
         self.websocket = websocket
 
     async def __aenter__(self):
         return self
 
     async def ping(self):
+        """Send websocket ping message"""
         await self.websocket.ping()
 
     async def close(self):
+        """Close all connections"""
         await self.cpggenclient.close()
         await self.httpclient.close()
         await self.websocket.close()
 
     async def __aexit__(self, exc_type, exc_value, exc_traceback):
         return await self.close()
 
 
 async def get(
     base_url="http://localhost:9000",
     cpggen_url="http://localhost:7072",
     username=None,
     password=None,
 ):
+    """Method to create a connection to joern and cpggen server"""
     auth = None
     if username and password:
         auth = httpx.BasicAuth(username, password)
     base_url = base_url.rstrip("/")
     client = httpx.AsyncClient(base_url=base_url, auth=auth, timeout=CLIENT_TIMEOUT)
     cpggenclient = None
     if cpggen_url:
@@ -57,22 +67,25 @@
         raise websockets.exceptions.InvalidState(
             "Didn't receive connected message from Joern server"
         )
     return Connection(cpggenclient, client, websocket)
 
 
 async def send(connection, message):
+    """Send message to the joern server via websocket"""
     await connection.websocket.send(message)
 
 
 async def receive(connection):
+    """Receive message from the joern server"""
     return await connection.websocket.recv()
 
 
 def fix_json(sout):
+    """Hacky method to convert the joern stdout string to json"""
     source_sink_mode = False
     try:
         if "defined function source" in sout:
             source_sink_mode = True
             sout = sout.replace("defined function source\n", "")
             sout = sout.replace("defined function sink\n", "")
         else:
@@ -97,49 +110,53 @@
             sout = "[ " + "\n".join(tmpA) + "]"
         return orjson.loads(sout)
     except Exception:
         return {"response": sout}
 
 
 def fix_query(query_str):
+    """Utility method to convert CPGQL queries to become json friendly"""
     if "\\." in query_str and "\\\\." not in query_str:
         query_str = query_str.replace("\\.", "\\\\.")
-    if (
-        query_str.startswith("cpg.")
-        or query_str.startswith("({cpg.")
-        and ".toJson" not in query_str
+    if (query_str.startswith("cpg.") or query_str.startswith("({cpg.")) and (
+        ".toJson" not in query_str
         and ".plotDot" not in query_str
         and not query_str.endswith(".p")
+        and ".store" not in query_str
         and "def" not in query_str
         and "printCallTree" not in query_str
     ):
         query_str = f"{query_str}.toJsonPretty"
     return query_str
 
 
 def parse_error(serr):
+    """Method to parse joern output and identify friendly error messages"""
     if "No projects loaded" in serr:
         return """ERROR: Import code using import_code api. Usage: await workspace.import_code(connection, directory_name, app_name)"""
     return serr
 
 
 async def p(connection, query_str, title="", caption=""):
+    """Method to print the result as a table"""
     result = await query(connection, query_str)
     print_table(result, title, caption)
     return result
 
 
 async def q(connection, query_str):
+    """Query joern server and optionally print the result as a table if the query ends with .p"""
     if query_str.strip().endswith(".p"):
         query_str = f"{query_str[:-2]}.toJsonPretty"
         return await p(connection, query_str)
     return await query(connection, query_str)
 
 
 async def query(connection, query_str):
+    """Query joern server"""
     client = connection.httpclient
     response = await client.post(
         url="/query", headers=headers, json={"query": fix_query(query_str)}
     )
     if response.status_code == httpx.codes.OK:
         j = response.json()
         res_uuid = j.get("uuid")
@@ -155,14 +172,15 @@
                 if sout:
                     return fix_json(sout)
                 return parse_error(serr)
     return None
 
 
 async def bulk_query(connection, query_list):
+    """Bulk query joern server"""
     client = connection.httpclient
     websocket = connection.websocket
     uuid_list = []
     response_list = []
     for query_str in query_list:
         response = await client.post(
             url="/query", headers=headers, json={"query": fix_query(query_str)}
@@ -186,63 +204,79 @@
                     response_list.append({"error": parse_error(serr)})
         if len(response_list) == len(uuid_list):
             return response_list
     return response_list
 
 
 async def flows(connection, source, sink):
+    """Execute reachableByFlows query"""
     return await flowsp(
-        connection, source, sink, print=True if os.getenv("POLYNOTE_VERSION") else False
+        connection,
+        source,
+        sink,
+        print_result=True if os.getenv("POLYNOTE_VERSION") else False,
     )
 
 
-async def flowsp(connection, source, sink, print=True):
+async def flowsp(connection, source, sink, print_result=True):
+    """Execute reachableByFlows query and optionally print the result table"""
     results = await bulk_query(
         connection,
         [
             source,
             sink,
             "sink.reachableByFlows(source).p",
         ],
     )
-    if print and len(results):
+    if print_result and len(results):
         tmpres = results[-1]
         if isinstance(tmpres, dict) and tmpres.get("response"):
             tmpres = tmpres.get("response")
         tmpA = tmpres.split('"""')[1:-1]
         print_md("\n".join([n for n in tmpA if len(n.strip()) > 1]))
     return results
 
 
-async def df(connection, source, sink):
+async def df(
+    connection,
+    source,
+    sink,
+    print_result=True if os.getenv("POLYNOTE_VERSION") else False,
+):
+    """Execute reachableByFlows query"""
+    if isinstance(source, dict):
+        for k, v in source.items():
+            source = f"""cpg.tag.name("{v}").{k}"""
+    if isinstance(sink, dict):
+        for k, v in sink.items():
+            sink = f"""cpg.tag.name("{v}").{k}"""
     if not source.startswith("def"):
         source = f"def source = {source}"
     if not sink.startswith("def"):
         sink = f"def sink = {sink}"
     results = await query(
         connection,
         f"""
         {source}
         {sink}
         sink.reachableByFlows(source).map(m => (m, m.elements.location.l)).toJson
         """,
     )
-    if len(results):
-        tmpres = results[-1]
-        if isinstance(tmpres, dict) and tmpres.get("response"):
-            tmpres = tmpres.get("response")
-        # print(tmpres)
+    if print_result:
+        print_flows(results)
     return results
 
 
-async def reachableByFlows(connection, source, sink):
-    return await df(connection, source, sink)
+async def reachableByFlows(connection, source, sink, print_result=False):
+    """Execute reachableByFlows query"""
+    return await df(connection, source, sink, print_result)
 
 
 async def create_cpg(connection, src, out_dir, lang):
+    """Create CPG using cpggen server"""
     client = connection.cpggenclient
     if not client:
         return {
             "error": "true",
             "message": "No active connection to cpggen server. Pass the cpggen url to the client.get method.",
         }, 500
     # Suppor for url
```

### Comparing `joern_lib-0.7.1/joern_lib/detectors/c.py` & `joern_lib-0.7.2/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.1/joern_lib/detectors/common.py` & `joern_lib-0.7.2/joern_lib/detectors/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,16 +96,60 @@
     return await client.q(connection, "cpg.namespace")
 
 
 async def list_parameters(connection):
     return await client.q(connection, "cpg.parameter")
 
 
-async def list_tags(connection):
-    return await client.q(connection, "cpg.tag")
+async def list_tags(
+    connection,
+    name=None,
+    value=None,
+    is_call=False,
+    is_method=False,
+    is_parameter=False,
+):
+    suffix = ""
+    if is_call:
+        suffix = ".call"
+    elif is_method:
+        suffix = ".method"
+    elif is_parameter:
+        suffix = ".parameter"
+    if name:
+        return await client.q(connection, f"""cpg.tag.name("{name}"){suffix}""")
+    elif value:
+        return await client.q(connection, f"""cpg.tag.value("{value}"){suffix}""")
+    return await client.q(connection, "cpg.tag{suffix}")
+
+
+async def create_tags(connection, query=None, call=None, method=None, tags=[]):
+    if not query and call:
+        query = f"""cpg.call.name("{call}")"""
+    elif not query and method:
+        query = f"""cpg.method.name("{method}")"""
+    if query and tags:
+        for tag in tags:
+            if isinstance(tag, dict):
+                for k, v in tag.items():
+                    await client.q(
+                        connection,
+                        f"""
+                        {query}.newTagNodePair("{k}", "{v}").store
+                        run.commit
+                        """,
+                    )
+            if isinstance(tag, str):
+                await client.q(
+                    connection,
+                    f"""
+                {query}.newTagNode("{tag}").store
+                run.commit
+                """,
+                )
 
 
 async def list_types(connection):
     return await client.q(connection, "cpg.typ")
 
 
 async def list_custom_types(connection):
```

### Comparing `joern_lib-0.7.1/joern_lib/detectors/java.py` & `joern_lib-0.7.2/joern_lib/detectors/java.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.1/joern_lib/detectors/js.py` & `joern_lib-0.7.2/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.1/joern_lib/utils.py` & `joern_lib-0.7.2/joern_lib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,34 +151,42 @@
 
 def print_flows(
     result,
     symbol_highlight_color="bold red",
     filelocation_highlight_color="grey54",
     check_highlight_color="dim green",
 ):
+    if not result:
+        return
     parsed_flows_list = []
     for res in result:
         useful_flows = []
         identifiers_list = []
         ftree = None
         floc_list = []
         flow_fingerprint_list = []
-        if res.get("_2"):
+        if isinstance(res, dict) and res.get("_2"):
             location_list = res.get("_2")
             last_symbol = ""
             for idx, loc in enumerate(location_list):
                 # Allow empty sink
                 if loc.get("filename") == "<empty>" and idx < len(location_list) - 2:
                     continue
-                symbol = loc.get("symbol")
+                symbol = loc.get("symbol", "").encode().decode("unicode_escape")
                 if symbol.startswith("<operator"):
                     continue
                 # Add the various computed fingerprints
                 loc["fingerprints"] = {}
-                code = loc.get("node", {}).get("code", "").strip()
+                code = (
+                    loc.get("node", {})
+                    .get("code", "")
+                    .encode()
+                    .decode("unicode_escape")
+                    .strip()
+                )
                 node_name = loc.get("node", {}).get("name")
                 # Highlight potential check methods
                 if node_name and node_name in code and check_highlight_color:
                     for check_label in check_labels_list:
                         if check_label in node_name.lower():
                             code = code.replace(
                                 node_name,
```

### Comparing `joern_lib-0.7.1/joern_lib/workspace.py` & `joern_lib-0.7.2/joern_lib/workspace.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.1/pyproject.toml` & `joern_lib-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.7.1"
+version = "0.7.2"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
@@ -32,11 +32,12 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
 pyinstaller = "^5.0.1"
+pdoc3 = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `joern_lib-0.7.1/PKG-INFO` & `joern_lib-0.7.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.7,<3.11
@@ -29,15 +29,15 @@
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Project-URL: Repository, https://github.com/AppThreat/joern-lib
 Description-Content-Type: text/markdown
 
 # Introduction
 
-High level python library to interact with a Joern [server](https://docs.joern.io/server).
+This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods are offered to perform code analysis on complex code bases without knowing [CPGQL](https://docs.joern.io/c-syntaxtree).
 
 ```
 pip install joern-lib
 ```
 
 The repository includes docker compose configuration to interactively query the joern server with polynote notebooks.
 
@@ -45,14 +45,20 @@
 
 ![polynote interface](docs/note2.jpg)
 
 ![polynote interface](docs/note3.jpg)
 
 ![polynote interface](docs/note4.jpg)
 
+![polynote interface](docs/sqli.jpg)
+
+![polynote interface](docs/repl.jpg)
+
+![polynote interface](docs/call-tree.jpg)
+
 ## Usage
 
 Run joern server and polynote locally.
 
 ```
 git clone https://github.com/appthreat/joern-lib.git
 # Edit docker-compose.yml to set sources directory
```

