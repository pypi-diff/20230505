# Comparing `tmp/streamlit-deckgl-0.1.1.tar.gz` & `tmp/streamlit-deckgl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deckgl-0.1.1.tar", last modified: Thu May  4 01:05:33 2023, max compression
+gzip compressed data, was "streamlit-deckgl-0.2.0.tar", last modified: Fri May  5 06:22:19 2023, max compression
```

## Comparing `streamlit-deckgl-0.1.1.tar` & `streamlit-deckgl-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1274 2023-04-28 04:00:31.000000 streamlit-deckgl-0.1.1/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-04 01:05:19.000000 streamlit-deckgl-0.1.1/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.843577 streamlit-deckgl-0.1.1/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.847577 streamlit-deckgl-0.1.1/src/streamlit_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1919 2023-05-04 01:05:08.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.851577 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-04-29 06:28:45.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 01:05:33.847577 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-04 01:05:33.000000 streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.939309 streamlit-deckgl-0.2.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1274 2023-04-28 04:00:31.000000 streamlit-deckgl-0.2.0/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-05 06:22:19.939309 streamlit-deckgl-0.2.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-05 06:11:32.000000 streamlit-deckgl-0.2.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.931309 streamlit-deckgl-0.2.0/src/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/src/streamlit_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2208 2023-05-05 06:11:18.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2004 2023-05-05 05:17:15.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/main.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/style.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/top_level.txt
```

### Comparing `streamlit-deckgl-0.1.1/LICENSE` & `streamlit-deckgl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.1/PKG-INFO` & `streamlit-deckgl-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.1.1
+Version: 0.2.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-deckgl-0.1.1/README.md` & `streamlit-deckgl-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.1/setup.py` & `streamlit-deckgl-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-deckgl",
-    version="0.1.1",
+    version="0.2.0",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for deck.gl visualisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_deckgl"],
     package_dir={"": "src"},
```

### Comparing `streamlit-deckgl-0.1.1/src/streamlit_deckgl/__init__.py` & `streamlit-deckgl-0.2.0/src/streamlit_deckgl/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,56 +12,58 @@
 _component_func = components.declare_component(
     "streamlit_deckgl", path=str(frontend_dir)
 )
 
 # Create the python function that will be called
 def st_deckgl(
     deck: pdk.Deck,
-    width: int = 1000,
     height: int = 500,
-    configuration: Optional[Dict] = None,
+    configuration: Optional[dict] = None,
     key: Optional[str] = "deck_gl",
     events: Optional[list] = None,
+    description: Optional[dict] = None,
 ):
     """Create a deck.gl map in Streamlit.
 
     Parameters
     ==========
     deck : pydeck.Deck instance
         The pydeck map to render.
-    width : int, default 1000
-        The width of the map in pixels.
     height : int, default 500
         The height of the map in pixels.
     configuration : dict, default None
         A dictionary of configuration options for the map.
     key : str, default "deck_gl"
         The key for the component. This must be unique for each map in the app.
     events : list, default ['click','hover','drag']
         A dict of events to listen for. Can be one or more of:
         - 'click'
         - 'hover'
         - 'drag'
+    description : dict, default None
+        A dictionary with additional description components to overlay on the map
+        The keys are the position which can be one of 'top-right','top-left','bottom-right','bottom-left'
+        The values are the html elements to place in each position
+        Example {'top-right':<div>This is a nice map</div>}
 
     Returns
     =======
     component_value : dict
         A dictionary containing the info dictionary of the event.
 
     """
     json = deck.to_json()
-    tooltip = deck._tooltip
     customLibraries = pdk.settings.custom_libraries
     configuration = pdk.settings.configuration
 
     component_value = _component_func(
         key=key,
-        width=width,
         height=height,
         spec=json,
-        tooltip=tooltip,
+        tooltip=deck._tooltip,
         customLibraries=customLibraries,
         configuration=configuration,
         events=events,
+        description=description,
     )
 
     return component_value
```

### Comparing `streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/index.html` & `streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/main.js` & `streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/main.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -11,27 +11,28 @@
  */
 
 function onRender(event) {
     // Only run the render code the first time the component is loaded.
     if (!window.rendered) {
         const {
             spec,
-            width,
-            height,
             tooltip,
+            height,
             customLibraries,
             configuration,
+            decription,
             events,
+            description,
         } = event.detail.args;
 
         const eventlist = events && events.map((event) => `deck-${event}-event`);
 
         const container = document.getElementById("root");
-        container.style.width = width + "px";
-        container.style.height = height + "px";
+        container.style.width = window.innerWidth - 10 + "px";
+        container.style.height = height - 10 + "px";
 
         const mapEventHandler = (eventType, info) => {
             if (events && eventlist.includes(eventType) && info.object) {
                 Streamlit.setComponentValue(info.object);
             }
         };
 
@@ -40,14 +41,29 @@
             jsonInput: JSON.parse(spec),
             tooltip,
             customLibraries,
             configuration,
             handleEvent: mapEventHandler,
         });
 
+        if (description) {
+            for (const key in description) {
+                if (
+                    ["top-right", "top-left", "bottom-right", "bottom-left"].includes(key)
+                ) {
+                    const pos = key.split("-");
+                    const style = `position: absolute; ${pos[0]}:10px; ${pos[1]}:10px;`;
+                    const div = document.createElement("div");
+                    div.innerHTML = description[key];
+                    div.style = style;
+                    container.appendChild(div);
+                }
+            }
+        }
+
         Streamlit.setFrameHeight(height);
         window.rendered = true;
     }
 }
 
 // Render the component whenever python send a "render event"
 Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender);
```

### Comparing `streamlit-deckgl-0.1.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js` & `streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.1.1/src/streamlit_deckgl.egg-info/PKG-INFO` & `streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.1.1
+Version: 0.2.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

