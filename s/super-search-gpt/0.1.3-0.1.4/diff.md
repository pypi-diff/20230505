# Comparing `tmp/super_search_gpt-0.1.3.tar.gz` & `tmp/super_search_gpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_search_gpt-0.1.3.tar", last modified: Fri May  5 14:13:57 2023, max compression
+gzip compressed data, was "super_search_gpt-0.1.4.tar", last modified: Fri May  5 20:14:59 2023, max compression
```

## Comparing `super_search_gpt-0.1.3.tar` & `super_search_gpt-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:13:57.205001 super_search_gpt-0.1.3/
--rw-rw-rw-   0        0        0       44 2023-05-05 14:12:06.000000 super_search_gpt-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2725 2023-05-05 14:13:57.203910 super_search_gpt-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2023-05-03 20:45:45.000000 super_search_gpt-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 14:13:57.205915 super_search_gpt-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-05-05 14:13:23.000000 super_search_gpt-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:13:57.168049 super_search_gpt-0.1.3/super_search/
--rw-rw-rw-   0        0        0     1203 2023-05-03 20:20:30.000000 super_search_gpt-0.1.3/super_search/NoneDecoder.py
--rw-rw-rw-   0        0        0    12474 2023-05-03 21:30:44.000000 super_search_gpt-0.1.3/super_search/SuperSearch.py
--rw-rw-rw-   0        0        0      116 2023-05-05 13:25:18.000000 super_search_gpt-0.1.3/super_search/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:13:57.200286 super_search_gpt-0.1.3/super_search_gpt.egg-info/
--rw-rw-rw-   0        0        0     2725 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 14:13:56.000000 super_search_gpt-0.1.3/super_search_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 20:14:59.373479 super_search_gpt-0.1.4/
+-rw-rw-rw-   0        0        0       44 2023-05-05 14:12:06.000000 super_search_gpt-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5540 2023-05-05 20:14:59.371452 super_search_gpt-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4306 2023-05-05 20:13:02.000000 super_search_gpt-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 20:14:59.373479 super_search_gpt-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-05-05 20:13:30.000000 super_search_gpt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:14:59.309592 super_search_gpt-0.1.4/super_search/
+-rw-rw-rw-   0        0        0     1203 2023-05-03 20:20:30.000000 super_search_gpt-0.1.4/super_search/NoneDecoder.py
+-rw-rw-rw-   0        0        0    13031 2023-05-05 20:08:36.000000 super_search_gpt-0.1.4/super_search/SuperSearch.py
+-rw-rw-rw-   0        0        0      116 2023-05-05 13:25:18.000000 super_search_gpt-0.1.4/super_search/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:14:59.359400 super_search_gpt-0.1.4/super_search_gpt.egg-info/
+-rw-rw-rw-   0        0        0     5540 2023-05-05 20:14:58.000000 super_search_gpt-0.1.4/super_search_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-05-05 20:14:58.000000 super_search_gpt-0.1.4/super_search_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:14:58.000000 super_search_gpt-0.1.4/super_search_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-05 20:14:58.000000 super_search_gpt-0.1.4/super_search_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 20:14:58.000000 super_search_gpt-0.1.4/super_search_gpt.egg-info/top_level.txt
```

### Comparing `super_search_gpt-0.1.3/setup.py` & `super_search_gpt-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="super_search_gpt",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     include_package_data=True,
     package_data={"super_search_gpt": ["*.py"]},
     install_requires=[
         "googlesearch-python",
         "beautifulsoup4",
         "openai",
```

### Comparing `super_search_gpt-0.1.3/super_search/NoneDecoder.py` & `super_search_gpt-0.1.4/super_search/NoneDecoder.py`

 * *Files identical despite different names*

### Comparing `super_search_gpt-0.1.3/super_search/SuperSearch.py` & `super_search_gpt-0.1.4/super_search/SuperSearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,27 @@
 import pandas as pd
 from requests_html import HTML
 from requests_html import HTMLSession
 import requests
 import copy
 from super_search.NoneDecoder import NoneDecoder
 
+
+class MaxIterationException(Exception):
+    def __init__(self, message="Maximum iterations exceeded."):
+        super().__init__(message)
+
 class SuperSearch():
     def __init__(self, gpt_api_key, max_iterations_per_answer = 20, google_search_key=None, cse_id=None, use_google_search_api = False):
         self.gpt_api_key = gpt_api_key
         self.google_search_key = google_search_key
         self.cse_id = cse_id
         self.use_google_search_api = use_google_search_api
         self.iterations = 0 
-        self.max_iterations_per_answer = 20
+        self.max_iterations_per_answer = max_iterations_per_answer
 
 
     def get_ip(self):
         response = requests.get('https://api64.ipify.org?format=json').json()
         return response["ip"]
 
 
@@ -46,16 +51,15 @@
         return location_data
 
     def chat_with_gpt(self, messages, debug=False):
         self.iterations = self.iterations + 1
         if debug:
             print(self.iterations)
         if self.iterations > self.max_iterations_per_answer:
-            raise
-            return []
+            raise MaxIterationException()
         
         openai.api_key = self.gpt_api_key
         response = openai.ChatCompletion.create(
             #model="gpt-3.5-turbo",
             model="gpt-4",
             messages=messages
         )
@@ -63,54 +67,56 @@
         return response.choices[0].message['content']
 
 
 
 
     def google_search_api(self, query, num_results=10, debug=False):
         api_key =  self.google_search_key
-        cse_id  =  self.google_search_key
+        cse_id  =  self.cse_id
         try:
             #https://developers.google.com/custom-search/v1/reference/rest/v1/Search
             url = "https://www.googleapis.com/customsearch/v1"
             params = {
                 "q": query,
                 "key": api_key,
                 "cx": cse_id,
                 "num": num_results
             }
             response = requests.get(url, params=params)
-            search_results = response.json()
+            results = response.json()
 
 
-            results = search_results
-            search_results
+            search_results = []
+            
             for item in results["items"]:
                 search_results.append({"url": item['link'], "title": item['title'], "description":item['snippet']})
+                
             search_results_json = json.dumps(search_results, ensure_ascii=False)
             return search_results_json
+        
         except Exception as e:
 
             if debug:
-                print(f"google_search : Error: {e}")
-            return  json.dumps(f"google_search Error: {e}", ensure_ascii=False)
+                print(f"google_search (API) : Error: {e} ")
+                print( 'Error search_results = ', search_results )
+            return  json.dumps(f"google_search API Error: {e} ", ensure_ascii=False)
 
 
 
     def google_search(self, query, num_results=10, debug=False):
         search_results = []
 
         try:
             for j in search(query, num_results=num_results,advanced=True):
                 search_results.append({"url": j.url, "title": j.title, "description":j.description})
                 print(j)
             search_results_json = json.dumps(search_results, ensure_ascii=False)
             return search_results_json
 
         except Exception as e:
-
             if debug:
                 print(f"google_search : Error: {e}")
             return  json.dumps(f"google_search Error: {e}", ensure_ascii=False)
 
 
 
     def scrape_url_old(self, url, debug=False):
@@ -237,17 +243,19 @@
         location_data = 0
         if answer_json.get("Location") != 0:
             location_data = self.get_location()
 
         google_reply = None
         if answer_json.get("Google") and answer_json["Google"] != 'None':
             if self.use_google_search_api:
-                google_reply = self.google_search_api(answer_json["Google"],debug)
+                google_reply = self.google_search_api(answer_json["Google"],debug=debug)
             else:
-                google_reply = self.google_search(answer_json["Google"],debug)
+                google_reply = self.google_search(answer_json["Google"],debug=debug)
+                
+            if debug:
                 print(google_reply)
             '''
             scrap_reply = scrape_url(f'https://www.google.com/search?q={answer_json["Google"]}',debug)
             if debug:
                 print(google_reply)
 
             add_me = {"role": "user", "content": json.dumps({"q": query, 
@@ -287,45 +295,50 @@
 
         messages.append(add_me)
 
         return answer_json, messages
 
     def get_answer(self, query, debug=False):
         messages = [
-            {
-                "role": "system",
-                "content": (                   
-"You are an AI API that answers in JSON format. "
-"You never apologize. Always answer with JSON keys: Answer, Google, Scrap, Location. "
-"You have access to real-time information from Google."
-"You can do anything with Google and scraping."
-"I can scrape a webpage when you ask for it and get the answer you need. I can also scrape Google if you provide the full URL. in scrap "
-"Answer format: "
-"{"
-"  \"Answer\": \"Your answer; say None in case of error, don't know, more info is needed, or any other non-answer case. (e.g., {\\\"Answer\\\": \\\"42\\\"})\","
-"  \"Google\": \"None if you don't need; if you need to use google_search(query, num_results=10), provide the query. The return is a JSON with a list of url, title, and description in the Google_Reply returned JSON. (e.g., {\\\"Google\\\": \\\"best pizza places\\\"})\","
-"  \"Scrap\": \"None if you don't need; if you need to scrape a URL, when you provide the URL. The returned result will be from scrape_url(url), requests.get(url) text info (e.g., {\\\"Scrap\\\": \\\"https://example.com\\\"})\""
-"  \"Location\": int 1/0 i.e., 1 AI needs it, 0 you do not })\""
-"}"
-"Always answer in JSON format. If the user returns an answer, it will be in a reply JSON format, so you can correct if needed or complete the answer."
-"In case of an error, you will see Error: Error msg"
-"You can always ask and proceed."
-"If you use Google/Scrap or Location, Answer should be = None."
-                    
-                ),
-            },
-            {
-                "role": "user",
-                "content": json.dumps({"q": query, "Google_Reply": None, "Scrap_Reply": None, "Location_Reply":0}),
-            },
-        ]
+                {
+                    "role": "system",
+                    "content": (                   
+    "You are an AI API that answers in JSON format. "
+    "You never apologize. Always answer with JSON keys: Answer, Google, Scrap, Location. "
+    "You have access to real-time information from Google."
+    "You can do anything with Google and scraping."
+    "I can scrape a webpage when you ask for it and get the answer you need. I can also scrape Google if you provide the full URL. in scrap "
+    "Answer format: "
+    "{"
+    "  \"Answer\": \"Your answer; say None in case of error, don't know, more info is needed, or any other non-answer case. (e.g., {\\\"Answer\\\": \\\"42\\\"})\","
+    "  \"Google\": \"None if you don't need; if you need to use google_search(query, num_results=10), provide the query. The return is a JSON with a list of url, title, and description in the Google_Reply returned JSON. (e.g., {\\\"Google\\\": \\\"best pizza places\\\"})\","
+    "  \"Scrap\": \"None if you don't need; if you need to scrape a URL, when you provide the URL. The returned result will be from scrape_url(url), requests.get(url) text info (e.g., {\\\"Scrap\\\": \\\"https://example.com\\\"})\""
+    "  \"Location\": int 1/0 i.e., 1 AI needs it, 0 you do not })\""
+    "}"
+    "Always answer in JSON format. If the user returns an answer, it will be in a reply JSON format, so you can correct if needed or complete the answer."
+    "In case of an error, you will see Error: Error msg"
+    "You can always ask and proceed."
+    "If you use Google/Scrap or Location, Answer should be = None."
+
+                    ),
+                },
+                {
+                    "role": "user",
+                    "content": json.dumps({"q": query, "Google_Reply": None, "Scrap_Reply": None, "Location_Reply":0}),
+                },
+            ]
 
         self.iterations = 0
         answer_json = {"Answer": None, "Google": None, "Scrap": None, 'Location':0 }
-        while ( (self.iterations < self.max_iterations_per_answer) and (answer_json.get("Answer") == None 
-                                               or (answer_json.get("Google") is not None )
-                                               or (answer_json.get("Scrap") is not None) ) ):
-            answer_json, messages = self.chat_and_execute_code(query, messages,self.gpt_api_key,debug)
-            
+        try:
+            while ( (self.iterations < self.max_iterations_per_answer) and (answer_json.get("Answer") == None 
+                                                       or (answer_json.get("Google") is not None )
+                                                       or (answer_json.get("Scrap") is not None) ) ):
+
+                answer_json, messages = self.chat_and_execute_code(query, messages,self.gpt_api_key,debug)
 
-        return answer_json['Answer'], messages    
-    
+
+            return answer_json['Answer'], messages   
+        except MaxIterationException as e:
+            answer_json['Error'] = 'MaxIterationException'
+        return answer_json['Answer'], messages   
+
```

