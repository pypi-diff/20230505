# Comparing `tmp/neosekai_api-1.2.0-py3-none-any.whl.zip` & `tmp/neosekai_api-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 6860 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      219 b- defN 23-Apr-12 07:51 neosekai_api/__init__.py
--rw-rw-rw-  2.0 fat     2543 b- defN 23-Apr-20 09:23 neosekai_api/chapter.py
--rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-20 09:24 neosekai_api/constants.py
+Zip file size: 6667 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      221 b- defN 23-May-05 14:54 neosekai_api/__init__.py
+-rw-rw-rw-  2.0 fat     2257 b- defN 23-May-05 16:49 neosekai_api/chapter.py
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-05 16:31 neosekai_api/constants.py
 -rw-rw-rw-  2.0 fat      332 b- defN 23-Apr-20 09:21 neosekai_api/helper.py
--rw-rw-rw-  2.0 fat     4735 b- defN 23-Apr-14 11:29 neosekai_api/novel.py
--rw-rw-rw-  2.0 fat      135 b- defN 23-Apr-14 11:41 neosekai_api/test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3165 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      883 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/RECORD
-11 files, 13227 bytes uncompressed, 5364 bytes compressed:  59.4%
+-rw-rw-rw-  2.0 fat     5571 b- defN 23-May-05 16:31 neosekai_api/novel.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3165 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      807 b- defN 23-May-05 16:55 neosekai_api-2.0.0.dist-info/RECORD
+10 files, 13568 bytes uncompressed, 5287 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -9,26 +9,23 @@
 
 Filename: neosekai_api/helper.py
 Comment: 
 
 Filename: neosekai_api/novel.py
 Comment: 
 
-Filename: neosekai_api/test.py
+Filename: neosekai_api-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: neosekai_api-1.2.0.dist-info/LICENSE
+Filename: neosekai_api-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: neosekai_api-1.2.0.dist-info/METADATA
+Filename: neosekai_api-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: neosekai_api-1.2.0.dist-info/WHEEL
+Filename: neosekai_api-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neosekai_api-1.2.0.dist-info/top_level.txt
-Comment: 
-
-Filename: neosekai_api-1.2.0.dist-info/RECORD
+Filename: neosekai_api-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neosekai_api/__init__.py

```diff
@@ -1,7 +1,8 @@
 from .chapter import NovelChapter
 from .novel import Novel
 from .constants import VERSION
+
 __author__ = "John Erinjery"
 __version__ = VERSION
 __license__ = "MIT"
 __copyright__ = "Copyright (c) 2023 John Erinjery"
```

## neosekai_api/chapter.py

```diff
@@ -10,19 +10,14 @@
 
     :params _url : The Mangadex Chapter URL
     '''
 
     def __init__(self, _url: str) -> None:
         self.url = _url
         self.__response_object = requests.get(self.url, timeout=10)
-        self.details = self.chapter_details()
-        self.volume = self.details['volume']
-        self.name = self.details['chapter_name']
-        self.release_date = self.details['release_date']
-
 
     def chapter_details(self):
         """
         returns chapter details : 
 
         - chapter volume
         - chapter name
@@ -68,11 +63,8 @@
                                    'content': i.span.text.strip() if fancy else heavy_translate(i.span.text.strip())}
                 n += 1
             elif i.img != None:
                 content[str(n)] = {'type': 'img', 'content': i.img['src']}
                 n += 1
             else:
                 continue
-        if fancy:
-            return content
-        else:
-            return heavy_translate(content)
+        return content
```

## neosekai_api/constants.py

```diff
@@ -1 +1 @@
-VERSION = '1.2.0'
+VERSION = '2.0.0'
```

## neosekai_api/novel.py

```diff
@@ -1,24 +1,21 @@
 import requests
 from bs4 import BeautifulSoup
 from neosekai_api.helper import heavy_translate
-import json
-
 
 class Novel:
     """
     Novel Object
     """
 
     def __init__(self, url):
         self.url = url
         self._response_object = requests.get(self.url, timeout=10)
-        self.novel_tags = self.__initialiser()
 
-    def __initialiser(self):
+    def get_novel_tags(self):
         '''
         returns novel tags as ```dict```
         '''
         soup = BeautifulSoup(self._response_object.content, 'lxml')
 
         # finding title
         title = soup.find('title').text.split(' - NeoSekai')[0]
@@ -97,34 +94,55 @@
                     "chapter_name" : '...',
                     "url" : '...',
                     "release_date" : '...'
                 },
 
                 "2" : {'...'}
             }
+        
         ```
+        - if novel is not categorised into volumes, volume will be an empty string
         """
+        content_dict = {}
         url = 'https://www.neosekaitranslations.com/wp-admin/admin-ajax.php'
-        soup = BeautifulSoup(self._response_object.content, 'lxml')
-        data_id = soup.find(
-            'div', attrs={'id': 'manga-chapters-holder'})['data-id']
+        soup_ = BeautifulSoup(self._response_object.content, 'lxml')
+        data_id = soup_.find(
+            'div', attrs={'id': ['manga-chapters-holder']})['data-id']
         data = {'action': 'manga_get_chapters', 'manga': data_id}
         soup_2 = BeautifulSoup(requests.post(url, data).content, 'lxml')
-        content_dict = {}
-        main_wrapper = soup_2.find('ul', attrs={'class': 'main version-chap'})
-        volumes_li = list(main_wrapper.find_all(
-            'li', recursive=False))
-        volumes_li.reverse()
-        n = 1
-        for i in volumes_li:
-            lines = list(i.find_all(
-                'li', attrs={'class': 'wp-manga-chapter'}))
+        li_with_children = list(soup_2.find_all('li', attrs={'class' : ['parent', 'has-child']}))
+
+        if li_with_children:
+            vol_list = []
+
+            for i in soup_2.find_all('a', attrs={'class' : ['has-child']}):
+                vol_num = i.text.strip().split()[1]
+                vol_list.append(int(vol_num))
+
+            if max(vol_list) != vol_list[0]:
+                pass
+            else:
+                li_with_children.reverse()
+            n = 1
+            for index,i in enumerate(li_with_children):
+                lines = list(i.find_all('li', attrs={'class' : ['wp-manga-chapter']}))
+                lines.reverse()
+                for j in lines:
+                    link = j.a['href']
+                    name = j.a.text.strip()
+                    date = j.span.text.strip()
+                    mini_dict = {'volume' : str(index + 1), 'chapter_name' : name, 'url' : link, 'release_date' : date}
+                    content_dict[str(n)] = mini_dict
+                    n += 1
+        else:
+            lines = list(soup_2.find_all('li', attrs={'class' : ['wp-manga-chapter']}))
             lines.reverse()
-            volume = i.a.text.strip()
+            n = 1
             for j in lines:
-                name = j.a.text.strip()
-                _url = j.a['href']
-                date = j.span.text.strip()
-                content_dict[f"{n}"] = {"volume": volume,
-                                        "chapter_name": name, "url": _url, "release_date": date}
-                n += 1
-        return eval(json.dumps(content_dict, indent=4))
+                    link = j.a['href']
+                    name = j.a.text.strip()
+                    date = j.span.text.strip()
+                    mini_dict = {'volume' : "", 'chapter_name' : heavy_translate(name), 'url' : link, 'release_date' : date}
+                    content_dict[str(n)] = mini_dict
+                    n += 1
+        
+        return content_dict
```

## Comparing `neosekai_api-1.2.0.dist-info/LICENSE` & `neosekai_api-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `neosekai_api-1.2.0.dist-info/METADATA` & `neosekai_api-2.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosekai-api
-Version: 1.2.0
+Version: 2.0.0
 Summary: An Unoffical Python API for neosekaitranslations.com
 Home-page: https://github.com/john-erinjery/neosekai-api/
 Author: John Erinjery
 Author-email: jancyvinod415@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
```

## Comparing `neosekai_api-1.2.0.dist-info/RECORD` & `neosekai_api-2.0.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-neosekai_api/__init__.py,sha256=2mTOZgz2NPHku8xLpaSWbESVenEZutISVPG1Zkdkncc,219
-neosekai_api/chapter.py,sha256=qCD2x_8-WiU_fr4BALYXJu1AK_kwZIYhA6sJohpOrnY,2543
-neosekai_api/constants.py,sha256=aa4_gbuOqQcNmMpq2h9EVmmebXOnCIQxU68fB31RZ5c,19
+neosekai_api/__init__.py,sha256=H-S6P2OdLTqUIbRqJqb5wx05nXhTCXTSl7eqWgxnl8I,221
+neosekai_api/chapter.py,sha256=p5pCmKJPjCeOtytW4YdcYecXY6gJnpgwcA0qPgbIfFU,2257
+neosekai_api/constants.py,sha256=c_YWUDV66qxHRCTN79ml7ZFzIV0hWs1zwNzA7VnoR5k,19
 neosekai_api/helper.py,sha256=2EThhUtKQ6_WTnJL7syMr4fjeO_v4dgECIvMjKx165U,332
-neosekai_api/novel.py,sha256=LGdtmM3RvP0J1zslIFQJDxj13smpB8qehJV2TylXkFM,4735
-neosekai_api/test.py,sha256=EMa9zXXfQkG7E5M6bvC4GkMGXjhcFprblBsPL-2A2pQ,135
-neosekai_api-1.2.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-neosekai_api-1.2.0.dist-info/METADATA,sha256=4_Dfg0_0zAHFSMY2rKftFkEKo2BDdvhHvAaSATpDcSM,3165
-neosekai_api-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neosekai_api-1.2.0.dist-info/top_level.txt,sha256=yhhnZQTXvjhjj5sIHCH99u0SXUqWkMfdfXrXuR585Us,13
-neosekai_api-1.2.0.dist-info/RECORD,,
+neosekai_api/novel.py,sha256=wUQPOZw2drcaZ_Dig_obpMgvSfP9E9xil-dXLLk2xis,5571
+neosekai_api-2.0.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+neosekai_api-2.0.0.dist-info/METADATA,sha256=23zTAg1bHWPLet5huuF9fbypQblVqXlRaIU7sSUv_0w,3165
+neosekai_api-2.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neosekai_api-2.0.0.dist-info/top_level.txt,sha256=yhhnZQTXvjhjj5sIHCH99u0SXUqWkMfdfXrXuR585Us,13
+neosekai_api-2.0.0.dist-info/RECORD,,
```

