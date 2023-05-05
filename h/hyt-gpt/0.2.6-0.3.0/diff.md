# Comparing `tmp/hyt-gpt-0.2.6.tar.gz` & `tmp/hyt-gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.2.6.tar", last modified: Tue Apr 25 15:41:43 2023, max compression
+gzip compressed data, was "hyt-gpt-0.3.0.tar", last modified: Fri May  5 18:28:51 2023, max compression
```

## Comparing `hyt-gpt-0.2.6.tar` & `hyt-gpt-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/hyt_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.2.6/hyt_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-04-12 04:46:33.000000 hyt-gpt-0.2.6/hyt_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.2.6/hyt_gpt/notion.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     6408 2023-04-25 06:23:34.000000 hyt-gpt-0.2.6/hyt_gpt/youtube.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/hyt_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-04-25 15:39:58.000000 hyt-gpt-0.2.6/setup.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/PKG-INFO
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/hyt_gpt/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        0 2023-04-19 01:16:56.000000 hyt-gpt-0.3.0/hyt_gpt/__init__.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     4000 2023-04-19 01:16:56.000000 hyt-gpt-0.3.0/hyt_gpt/gpt.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     2886 2023-04-19 01:16:56.000000 hyt-gpt-0.3.0/hyt_gpt/notion.py
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)     6904 2023-05-05 18:26:17.000000 hyt-gpt-0.3.0/hyt_gpt/youtube.py
+drwxr-x---   0 haibinzh (778454) primarygroup (89939)        0 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/hyt_gpt.egg-info/
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      702 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/PKG-INFO
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      204 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/SOURCES.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        1 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/dependency_links.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)        8 2023-05-05 18:28:51.000000 hyt-gpt-0.3.0/hyt_gpt.egg-info/top_level.txt
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)       38 2023-05-05 18:28:51.722092 hyt-gpt-0.3.0/setup.cfg
+-rw-r-----   0 haibinzh (778454) primarygroup (89939)      837 2023-05-05 18:28:33.000000 hyt-gpt-0.3.0/setup.py
```

### Comparing `hyt-gpt-0.2.6/PKG-INFO` & `hyt-gpt-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.6
+Version: 0.3.0
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.2.6/hyt_gpt/gpt.py` & `hyt-gpt-0.3.0/hyt_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.6/hyt_gpt/notion.py` & `hyt-gpt-0.3.0/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.6/hyt_gpt/youtube.py` & `hyt-gpt-0.3.0/hyt_gpt/youtube.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import requests
-import yt_dlp
 from typing import Dict, Any, List
 from .gpt import seg_transcript, chat_gpt
 from datetime import datetime
+from youtube_transcript_api import YouTubeTranscriptApi
 import traceback
 import re
 
 headers = {
     'authority': 'api.youtube.com',
     'accept': 'application/json, text/plain, */*',
     'user-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3',
@@ -71,15 +70,26 @@
     
     @staticmethod
     def get_timestamp_diff(start_time, end_time):
         start_time = datetime.strptime(start_time, '%H:%M:%S.%f')
         end_time = datetime.strptime(end_time, '%H:%M:%S.%f')
         diff = (end_time - start_time).total_seconds()
         return diff
+    
+    def __youtube_subtitle(self, url: str) -> List[Dict[str, str]]:
+        video_id = self.get_youtube_id(url)
+        list = YouTubeTranscriptApi.list_transcripts(video_id)
+        en_transicript = list.find_transcript(['en'])
+        if 'zh-Hans' in en_transicript.translation_languages:
+            translated = en_transicript.translate('zh-Hans').fetch()
+            return translated
+        return en_transicript.fetch()        
 
+"""
+5/5/23: Older version
 
     def __youtube_player_list(self, yvid):
         url = f"https://www.youtube.com/watch?v={yvid}"
         response = requests.request("GET", url, headers=headers)
         return response.text
 
 
@@ -163,7 +173,8 @@
 
     def __to_subtitle_list(self, subtitles):
         results = []
         for subtitle in subtitles:
             if 'text' in subtitle:
                 results.append(subtitle.get('text'))
         return results
+"""
```

### Comparing `hyt-gpt-0.2.6/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.3.0/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.6
+Version: 0.3.0
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.2.6/setup.py` & `hyt-gpt-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.2.6',
+    version='0.3.0',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

