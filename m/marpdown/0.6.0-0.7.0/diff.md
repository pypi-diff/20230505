# Comparing `tmp/marpdown-0.6.0.tar.gz` & `tmp/marpdown-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marpdown-0.6.0.tar", last modified: Fri May  5 09:24:28 2023, max compression
+gzip compressed data, was "marpdown-0.7.0.tar", last modified: Fri May  5 20:50:47 2023, max compression
```

## Comparing `marpdown-0.6.0.tar` & `marpdown-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:24:28.506815 marpdown-0.6.0/
--rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      404 2023-05-05 09:24:28.506815 marpdown-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 09:24:28.495892 marpdown-0.6.0/marpdown/
--rw-rw-rw-   0        0        0      124 2023-04-12 22:07:50.000000 marpdown-0.6.0/marpdown/__init__.py
--rw-rw-rw-   0        0        0     2886 2023-05-05 09:16:47.000000 marpdown-0.6.0/marpdown/css.py
--rw-rw-rw-   0        0        0     2545 2023-04-12 15:26:33.000000 marpdown-0.6.0/marpdown/ppt.py
--rw-rw-rw-   0        0        0     4045 2023-05-05 09:16:23.000000 marpdown-0.6.0/marpdown/slide.py
--rw-rw-rw-   0        0        0     1277 2023-05-05 08:41:55.000000 marpdown-0.6.0/marpdown/utils.py
--rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.6.0/marpdown/writer.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:24:28.504791 marpdown-0.6.0/marpdown.egg-info/
--rw-rw-rw-   0        0        0      404 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 09:24:28.508084 marpdown-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-05-05 09:22:58.000000 marpdown-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:50:47.668695 marpdown-0.7.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-05-05 20:50:47.667661 marpdown-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 20:50:47.649412 marpdown-0.7.0/marpdown/
+-rw-rw-rw-   0        0        0      124 2023-04-12 22:07:50.000000 marpdown-0.7.0/marpdown/__init__.py
+-rw-rw-rw-   0        0        0     2886 2023-05-05 09:16:47.000000 marpdown-0.7.0/marpdown/css.py
+-rw-rw-rw-   0        0        0     2545 2023-04-12 15:26:33.000000 marpdown-0.7.0/marpdown/ppt.py
+-rw-rw-rw-   0        0        0     4143 2023-05-05 20:03:01.000000 marpdown-0.7.0/marpdown/slide.py
+-rw-rw-rw-   0        0        0     1279 2023-05-05 19:58:03.000000 marpdown-0.7.0/marpdown/utils.py
+-rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.7.0/marpdown/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:50:47.664947 marpdown-0.7.0/marpdown.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-05-05 20:50:47.000000 marpdown-0.7.0/marpdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-05 20:50:47.000000 marpdown-0.7.0/marpdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:50:47.000000 marpdown-0.7.0/marpdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 20:50:47.000000 marpdown-0.7.0/marpdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 20:50:47.668695 marpdown-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-05-05 20:50:40.000000 marpdown-0.7.0/setup.py
```

### Comparing `marpdown-0.6.0/LICENSE` & `marpdown-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marpdown-0.6.0/marpdown/css.py` & `marpdown-0.7.0/marpdown/css.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.6.0/marpdown/ppt.py` & `marpdown-0.7.0/marpdown/ppt.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.6.0/marpdown/slide.py` & `marpdown-0.7.0/marpdown/slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,52 +47,55 @@
     <div class="boxline-marker">{i+1}</div>
     <div class="boxline-content"><h2>{box}</h2></div>
   </li>''')
         self.__writer__.append('</ul>')
         super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
 
 class CardSlide(BaseSlide):
-    def __init__(self, *, title: str,text:str, cards: list[tuple[str,list[str]]], card_width:int = 450 ,backgroundImage: str = None):
+  COUNT = 0
+  
+  def __init__(self, *, title: str,text:str, cards: list[tuple[str,list[str]]], card_width:int = 450 ,backgroundImage: str = None):
+        self.__class__.COUNT += 1
         self.__writer__ = Writer()
         CARD = f'''<style>
         .card-container {{
   display: flex;
   justify-content: center;
   flex-wrap: wrap;
   padding: 20px;
   width: 100%;
 }}
 
-.card {{
+.card{self.COUNT} {{
   background-color: #cceeff;
   border-radius: 5px;
   padding: 20px;
   width: {card_width}px;
   box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
   margin: 20px 30px; /* 上下边距为 20px，左右边距为 10px */
   display: inline-block;
 }}
 
-.card h2 {{
+.card{self.COUNT} h2 {{
   margin-top: 0;
   margin-bottom: 10px;
 }}
 
-.card p {{
+.card{self.COUNT} p {{
   margin: 0;
 }}</style>
         '''
 
         self.__writer__.append(CARD)
         self.__writer__.append(f"# {title}")
         self.__writer__.append(text)
         self.__writer__.append(' <div class="card-container">')
         for card in cards:
             name,bulletpoints = card
-            self.__writer__.append(f'''<div class="card">
+            self.__writer__.append(f'''<div class="card{self.COUNT}">
     <h2>{name}</h2>
     <p>
       {utils.list_to_html_ul(bulletpoints)}
     </p>
   </div>''')
         self.__writer__.append('</div>')
         super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
```

### Comparing `marpdown-0.6.0/marpdown/utils.py` & `marpdown-0.7.0/marpdown/utils.py`

 * *Ordering differences only*

 * *Files identical despite different names*

```diff
@@ -61,8 +61,8 @@
   <div class="column2">
     {column2}
   </div>
 </div>
     
     '''
     return ret
-    
+
```

### Comparing `marpdown-0.6.0/marpdown/writer.py` & `marpdown-0.7.0/marpdown/writer.py`

 * *Files identical despite different names*

### Comparing `marpdown-0.6.0/setup.py` & `marpdown-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
 
 ]
 
 setup(
     name="marpdown",
-    version="0.6.0",
+    version="0.7.0",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of RL algorithms",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/marpdown",
     packages=find_packages(),
```

