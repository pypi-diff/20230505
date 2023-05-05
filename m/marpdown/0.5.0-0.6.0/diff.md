# Comparing `tmp/marpdown-0.5.0.tar.gz` & `tmp/marpdown-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marpdown-0.5.0.tar", last modified: Wed May  3 11:56:26 2023, max compression
+gzip compressed data, was "marpdown-0.6.0.tar", last modified: Fri May  5 09:24:28 2023, max compression
```

## Comparing `marpdown-0.5.0.tar` & `marpdown-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:56:26.716434 marpdown-0.5.0/
--rw-r--r--   0 leo       (1000) leo       (1000)     1066 2023-05-03 08:45:11.000000 marpdown-0.5.0/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      390 2023-05-03 11:56:26.716434 marpdown-0.5.0/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)       41 2023-05-03 08:45:11.000000 marpdown-0.5.0/README.md
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:56:26.712434 marpdown-0.5.0/marpdown/
--rw-r--r--   0 leo       (1000) leo       (1000)      116 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2994 2023-05-03 11:31:06.000000 marpdown-0.5.0/marpdown/css.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2462 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/ppt.py
--rw-r--r--   0 leo       (1000) leo       (1000)     3380 2023-05-03 11:22:09.000000 marpdown-0.5.0/marpdown/slide.py
--rw-r--r--   0 leo       (1000) leo       (1000)      240 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/utils.py
--rw-r--r--   0 leo       (1000) leo       (1000)      584 2023-05-03 08:45:11.000000 marpdown-0.5.0/marpdown/writer.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-03 11:56:26.716434 marpdown-0.5.0/marpdown.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      390 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      262 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        9 2023-05-03 11:56:26.000000 marpdown-0.5.0/marpdown.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-05-03 11:56:26.716434 marpdown-0.5.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      605 2023-05-03 11:55:41.000000 marpdown-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:24:28.506815 marpdown-0.6.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 13:16:28.000000 marpdown-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-05-05 09:24:28.506815 marpdown-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-12 13:16:28.000000 marpdown-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 09:24:28.495892 marpdown-0.6.0/marpdown/
+-rw-rw-rw-   0        0        0      124 2023-04-12 22:07:50.000000 marpdown-0.6.0/marpdown/__init__.py
+-rw-rw-rw-   0        0        0     2886 2023-05-05 09:16:47.000000 marpdown-0.6.0/marpdown/css.py
+-rw-rw-rw-   0        0        0     2545 2023-04-12 15:26:33.000000 marpdown-0.6.0/marpdown/ppt.py
+-rw-rw-rw-   0        0        0     4045 2023-05-05 09:16:23.000000 marpdown-0.6.0/marpdown/slide.py
+-rw-rw-rw-   0        0        0     1277 2023-05-05 08:41:55.000000 marpdown-0.6.0/marpdown/utils.py
+-rw-rw-rw-   0        0        0      607 2023-04-12 14:35:56.000000 marpdown-0.6.0/marpdown/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:24:28.504791 marpdown-0.6.0/marpdown.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 09:24:28.000000 marpdown-0.6.0/marpdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:24:28.508084 marpdown-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-05-05 09:22:58.000000 marpdown-0.6.0/setup.py
```

### Comparing `marpdown-0.5.0/LICENSE` & `marpdown-0.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Tao Xiang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Tao Xiang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `marpdown-0.5.0/marpdown/ppt.py` & `marpdown-0.6.0/marpdown/ppt.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from typing import Union, List
-from .writer import Writer
-from .css import load_css
-from .slide import BaseSlide
-
-
-class PPT:
-    def __init__(self,
-                 footer:str,
-                 paginate:bool,
-                 _class = "lead",
-                 backgroundImage:str = '''url('https://marp.app/assets/hero-background.svg')''',
-                 ) -> None:
-
-        self.writer = Writer()
-        self.slides = []
-        self.footer = footer
-        self.paginate = paginate
-        self._class = _class
-        self.backgroundImage = backgroundImage
-
-
-
-    def __setup__(self):
-        self.writer.append(f'''---\nmarp: true\nfooter: "{self.footer}"\npaginate: {self.paginate}''')
-        if self._class is not None:
-            self.writer.append(f"_class: {self._class}")
-        if self.backgroundImage is not None:
-            self.writer.append(f"backgroundImage: url('{self.backgroundImage}')")
-        self.__start_new_slide__()
-        self.writer.append('<style>')
-        self.writer.append(load_css())
-        self.writer.append('</style>')
-
-    def build(self):
-        self.writer.clear()
-        self.__setup__()
-        s = self.slides[0]
-        self.__build_bgimage__(s)
-        self.writer.append(s.content)
-
-        for s in self.slides[1:]:
-            self.__start_new_slide__()
-            self.__build_bgimage__(s)
-            self.writer.append(s.content)
-        return self.writer.getValue()
-
-    def __build_bgimage__(self, s):
-        if s.bgimage is not None:
-            self.writer.append(f'![bg]({s.bgimage})')
-        else:
-            self.writer.append(f'![bg]({self.backgroundImage})')
-
-    def store(self,path:str, overwrite = True):
-        self.build()
-        self.writer.store(path, overwrite)
-
-    # subscriptable and slice-able
-    def __getitem__(self, item):
-        return self.slides[item]
-
-    def __start_new_slide__(self):
-        self.writer.append('\n')
-        self.writer.append('---\n')
-
-    def __str__(self):
-        return self.build()
-    def __repr__(self):
-        return self.build()
-
-    # return an iterator that can be used in for loop etc.
-    def __iter__(self):
-        return self.slides.__iter__()
-
-    def __len__(self):
-        return len(self.slides)
-
-    def addSlides(self, slides: Union[BaseSlide, List[BaseSlide]]):
-        if isinstance(slides, BaseSlide):
-            self.slides.append(slides)
-        elif isinstance(slides, list):
-            self.slides += slides
-
+from typing import Union, List
+from .writer import Writer
+from .css import load_css
+from .slide import BaseSlide
+
+
+class PPT:
+    def __init__(self,
+                 footer:str,
+                 paginate:bool,
+                 _class = "lead",
+                 backgroundImage:str = '''url('https://marp.app/assets/hero-background.svg')''',
+                 ) -> None:
+
+        self.writer = Writer()
+        self.slides = []
+        self.footer = footer
+        self.paginate = paginate
+        self._class = _class
+        self.backgroundImage = backgroundImage
+
+
+
+    def __setup__(self):
+        self.writer.append(f'''---\nmarp: true\nfooter: "{self.footer}"\npaginate: {self.paginate}''')
+        if self._class is not None:
+            self.writer.append(f"_class: {self._class}")
+        if self.backgroundImage is not None:
+            self.writer.append(f"backgroundImage: url('{self.backgroundImage}')")
+        self.__start_new_slide__()
+        self.writer.append('<style>')
+        self.writer.append(load_css())
+        self.writer.append('</style>')
+
+    def build(self):
+        self.writer.clear()
+        self.__setup__()
+        s = self.slides[0]
+        self.__build_bgimage__(s)
+        self.writer.append(s.content)
+
+        for s in self.slides[1:]:
+            self.__start_new_slide__()
+            self.__build_bgimage__(s)
+            self.writer.append(s.content)
+        return self.writer.getValue()
+
+    def __build_bgimage__(self, s):
+        if s.bgimage is not None:
+            self.writer.append(f'![bg]({s.bgimage})')
+        else:
+            self.writer.append(f'![bg]({self.backgroundImage})')
+
+    def store(self,path:str, overwrite = True):
+        self.build()
+        self.writer.store(path, overwrite)
+
+    # subscriptable and slice-able
+    def __getitem__(self, item):
+        return self.slides[item]
+
+    def __start_new_slide__(self):
+        self.writer.append('\n')
+        self.writer.append('---\n')
+
+    def __str__(self):
+        return self.build()
+    def __repr__(self):
+        return self.build()
+
+    # return an iterator that can be used in for loop etc.
+    def __iter__(self):
+        return self.slides.__iter__()
+
+    def __len__(self):
+        return len(self.slides)
+
+    def addSlides(self, slides: Union[BaseSlide, List[BaseSlide]]):
+        if isinstance(slides, BaseSlide):
+            self.slides.append(slides)
+        elif isinstance(slides, list):
+            self.slides += slides
+
```

### Comparing `marpdown-0.5.0/marpdown/slide.py` & `marpdown-0.6.0/marpdown/slide.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,104 @@
-from .writer import Writer
-from . import  utils
-
-class BaseSlide:
-    def __init__(self,*,content:str='',backgroundImage: str = None, ):
-        self.content = content
-        self.bgimage = backgroundImage
-
-
-class TOCSlide(BaseSlide):
-    def __init__(self, title: str, toc: list[str],focus = -1,backgroundImage: str = None):
-        self.toc = toc
-        content = f'''# {title}\n\n'''
-        if focus == -1:
-            tmp = [f'''### {i+1}. {t}''' for i,t in enumerate(toc)]
-            content += '\n'.join(tmp)
-        else:
-            tmp = [f'''### {i + 1}. {t}''' for i, t in enumerate(toc)]
-            tmp[focus] = f'''### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> {focus+1}. {toc[focus]}</div></div></div>'''
-            content += '\n'.join(tmp)
-        super().__init__(content=content, backgroundImage=backgroundImage)
-
-class TimelineSlide(BaseSlide):
-    def __init__(self, title:str,timelines: list[tuple],backgroundImage: str = None,):
-        content ="# " + title + "\n"
-        content += '''<ul class="timeline">\n'''
-        for tl in timelines:
-            name, detail = tl
-            content+=f'''<li class="timeline-item">
-                        <div class="timeline-marker"></div>
-                        <div class="timeline-content">
-                          <h4>{name}</h4>
-                          {detail}
-                        </div></li>'''
-        content += '</ul>'
-
-        super().__init__(content=content, backgroundImage=backgroundImage)
-
-class BoxlineSlide(BaseSlide):
-    def __init__(self, *, title: str,boxlines:list[str] ,backgroundImage: str = None):
-        self.__writer__ = Writer()
-        self.__writer__.append(f"# {title}")
-        self.__writer__.append('<ul class="boxline">')
-
-        for i,box in enumerate(boxlines):
-            self.__writer__.append(f'''<li class="boxline-item">
-    <div class="boxline-marker">{i+1}</div>
-    <div class="boxline-content"><h2>{box}</h2></div>
-  </li>''')
-        self.__writer__.append('</ul>')
-        super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
-
-class CardSlide(BaseSlide):
-    def __init__(self, *, title: str,text:str, cards: list[tuple[str,list[str]]] ,backgroundImage: str = None):
-        self.__writer__ = Writer()
-        self.__writer__.append(f"# {title}")
-        self.__writer__.append(text)
-        self.__writer__.append(' <div class="card-container">')
-        for card in cards:
-            name,bulletpoints = card
-            self.__writer__.append(f'''<div class="card">
-    <h2>{name}</h2>
-    <p>
-      {utils.list_to_html_ul(bulletpoints)}
-    </p>
-  </div>''')
-        self.__writer__.append('</div>')
-        super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
-
-class ThanksSlide(BaseSlide):
-    def __init__(self, backgroundImage:str = None):
-        super().__init__(content='''<div style="display: flex; justify-content: center; align-items: center; height: 100vh; text-align: center;padding-left=200px">
-  <h1 style="margin: 0 auto;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Thanks for Attention! Any Questions?</h1>
+from .writer import Writer
+from . import  utils
+
+class BaseSlide:
+    def __init__(self,*,content:str='',backgroundImage: str = None, ):
+        self.content = content
+        self.bgimage = backgroundImage
+
+
+class TOCSlide(BaseSlide):
+    def __init__(self, title: str, toc: list[str],focus = -1,backgroundImage: str = None):
+        self.toc = toc
+        content = f'''# {title}\n\n'''
+        if focus == -1:
+            tmp = [f'''### {i+1}. {t}''' for i,t in enumerate(toc)]
+            content += '\n'.join(tmp)
+        else:
+            tmp = [f'''### {i + 1}. {t}''' for i, t in enumerate(toc)]
+            tmp[focus] = f'''### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> {focus+1}. {toc[focus]}</div></div></div>'''
+            content += '\n'.join(tmp)
+        super().__init__(content=content, backgroundImage=backgroundImage)
+
+class TimelineSlide(BaseSlide):
+    def __init__(self, title:str,timelines: list[tuple],backgroundImage: str = None,):
+        content ="# " + title + "\n"
+        content += '''<ul class="timeline">\n'''
+        for tl in timelines:
+            name, detail = tl
+            content+=f'''<li class="timeline-item">
+                        <div class="timeline-marker"></div>
+                        <div class="timeline-content">
+                          <h4>{name}</h4>
+                          {detail}
+                        </div></li>'''
+        content += '</ul>'
+
+        super().__init__(content=content, backgroundImage=backgroundImage)
+
+class BoxlineSlide(BaseSlide):
+    def __init__(self, *, title: str,boxlines:list[str] ,backgroundImage: str = None):
+        self.__writer__ = Writer()
+        self.__writer__.append(f"# {title}")
+        self.__writer__.append('<ul class="boxline">')
+
+        for i,box in enumerate(boxlines):
+            self.__writer__.append(f'''<li class="boxline-item">
+    <div class="boxline-marker">{i+1}</div>
+    <div class="boxline-content"><h2>{box}</h2></div>
+  </li>''')
+        self.__writer__.append('</ul>')
+        super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
+
+class CardSlide(BaseSlide):
+    def __init__(self, *, title: str,text:str, cards: list[tuple[str,list[str]]], card_width:int = 450 ,backgroundImage: str = None):
+        self.__writer__ = Writer()
+        CARD = f'''<style>
+        .card-container {{
+  display: flex;
+  justify-content: center;
+  flex-wrap: wrap;
+  padding: 20px;
+  width: 100%;
+}}
+
+.card {{
+  background-color: #cceeff;
+  border-radius: 5px;
+  padding: 20px;
+  width: {card_width}px;
+  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
+  margin: 20px 30px; /* 上下边距为 20px，左右边距为 10px */
+  display: inline-block;
+}}
+
+.card h2 {{
+  margin-top: 0;
+  margin-bottom: 10px;
+}}
+
+.card p {{
+  margin: 0;
+}}</style>
+        '''
+
+        self.__writer__.append(CARD)
+        self.__writer__.append(f"# {title}")
+        self.__writer__.append(text)
+        self.__writer__.append(' <div class="card-container">')
+        for card in cards:
+            name,bulletpoints = card
+            self.__writer__.append(f'''<div class="card">
+    <h2>{name}</h2>
+    <p>
+      {utils.list_to_html_ul(bulletpoints)}
+    </p>
+  </div>''')
+        self.__writer__.append('</div>')
+        super().__init__(content=self.__writer__.getValue(), backgroundImage=backgroundImage)
+
+class ThanksSlide(BaseSlide):
+    def __init__(self, backgroundImage:str = None):
+        super().__init__(content='''<div style="display: flex; justify-content: center; align-items: center; height: 100vh; text-align: center;padding-left=200px">
+  <h1 style="margin: 0 auto;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Thanks for Attention! Any Questions?</h1>
 </div>''', backgroundImage=backgroundImage)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `marpdown-0.5.0/marpdown/writer.py` & `marpdown-0.6.0/marpdown/writer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import io
-from pathlib import Path
-
-
-class Writer:
-    def __init__(self):
-        self.WRITER = io.StringIO()
-
-    def append(self,md: str):
-        self.WRITER.write(md+'\n')
-
-    def clear(self,):
-        self.WRITER.seek(0)
-        self.WRITER.truncate(0)
-
-    def store(self,path:str, overwrite = True):
-        path_ = Path(path)
-        if path_.exists():
-            if not overwrite:
-                raise RuntimeError("The path already exists.")
-
-        path_.write_text(self.WRITER.getvalue(),encoding="utf-8")
-    def getValue(self):
+import io
+from pathlib import Path
+
+
+class Writer:
+    def __init__(self):
+        self.WRITER = io.StringIO()
+
+    def append(self,md: str):
+        self.WRITER.write(md+'\n')
+
+    def clear(self,):
+        self.WRITER.seek(0)
+        self.WRITER.truncate(0)
+
+    def store(self,path:str, overwrite = True):
+        path_ = Path(path)
+        if path_.exists():
+            if not overwrite:
+                raise RuntimeError("The path already exists.")
+
+        path_.write_text(self.WRITER.getvalue(),encoding="utf-8")
+    def getValue(self):
         return self.WRITER.getvalue()
```

