# Comparing `tmp/web-render-0.1.8.tar.gz` & `tmp/web-render-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-render-0.1.8.tar", last modified: Thu Sep  8 11:27:37 2022, max compression
+gzip compressed data, was "web-render-0.1.9.tar", last modified: Fri May  5 19:01:46 2023, max compression
```

## Comparing `web-render-0.1.8.tar` & `web-render-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.489363 web-render-0.1.8/
--rw-rw-r--   0 repente   (1000) repente   (1000)       38 2022-06-14 15:11:38.000000 web-render-0.1.8/MANIFEST.in
--rw-rw-r--   0 repente   (1000) repente   (1000)      454 2022-09-08 11:27:37.489363 web-render-0.1.8/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      223 2022-06-18 18:30:21.000000 web-render-0.1.8/README.md
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.325348 web-render-0.1.8/pyrender/
--rw-rw-r--   0 repente   (1000) repente   (1000)      441 2022-07-27 14:57:39.000000 web-render-0.1.8/pyrender/abstract_cls.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.381353 web-render-0.1.8/pyrender/http_service/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-06-14 12:20:12.000000 web-render-0.1.8/pyrender/http_service/__init__.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.393355 web-render-0.1.8/pyrender/http_service/api/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-06-14 12:20:22.000000 web-render-0.1.8/pyrender/http_service/api/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     2576 2022-07-21 20:50:28.000000 web-render-0.1.8/pyrender/http_service/api/view.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      662 2022-06-17 10:48:07.000000 web-render-0.1.8/pyrender/http_service/main.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      194 2022-06-17 10:46:53.000000 web-render-0.1.8/pyrender/http_service/routing.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      986 2022-06-17 10:47:14.000000 web-render-0.1.8/pyrender/http_service/service.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     2543 2022-07-21 20:58:31.000000 web-render-0.1.8/pyrender/interface.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.401355 web-render-0.1.8/pyrender/playwright_service/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-07-27 13:04:20.000000 web-render-0.1.8/pyrender/playwright_service/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     5643 2022-09-08 11:25:22.000000 web-render-0.1.8/pyrender/playwright_service/main.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.401355 web-render-0.1.8/pyrender/selenium_service/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-06-14 12:19:58.000000 web-render-0.1.8/pyrender/selenium_service/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     9365 2022-07-27 13:24:13.000000 web-render-0.1.8/pyrender/selenium_service/main.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1481 2022-06-17 10:46:21.000000 web-render-0.1.8/pyrender/tool.py
--rw-rw-r--   0 repente   (1000) repente   (1000)       38 2022-09-08 11:27:37.489363 web-render-0.1.8/setup.cfg
--rw-rw-r--   0 repente   (1000) repente   (1000)     3427 2022-09-08 11:27:21.000000 web-render-0.1.8/setup.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2022-09-08 11:27:37.489363 web-render-0.1.8/web_render.egg-info/
--rw-rw-r--   0 repente   (1000) repente   (1000)      454 2022-09-08 11:27:37.000000 web-render-0.1.8/web_render.egg-info/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      613 2022-09-08 11:27:37.000000 web-render-0.1.8/web_render.egg-info/SOURCES.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        1 2022-09-08 11:27:37.000000 web-render-0.1.8/web_render.egg-info/dependency_links.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       89 2022-09-08 11:27:37.000000 web-render-0.1.8/web_render.egg-info/requires.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        9 2022-09-08 11:27:37.000000 web-render-0.1.8/web_render.egg-info/top_level.txt
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.587660 web-render-0.1.9/
+-rw-rw-r--   0 repente   (1000) repente   (1000)       38 2022-06-14 15:11:38.000000 web-render-0.1.9/MANIFEST.in
+-rw-rw-r--   0 repente   (1000) repente   (1000)      454 2023-05-05 19:01:46.583660 web-render-0.1.9/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      223 2022-06-18 18:30:21.000000 web-render-0.1.9/README.md
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.583660 web-render-0.1.9/pyrender/
+-rw-rw-r--   0 repente   (1000) repente   (1000)      441 2022-07-27 14:57:39.000000 web-render-0.1.9/pyrender/abstract_cls.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.583660 web-render-0.1.9/pyrender/http_service/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-06-14 12:20:12.000000 web-render-0.1.9/pyrender/http_service/__init__.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.583660 web-render-0.1.9/pyrender/http_service/api/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-06-14 12:20:22.000000 web-render-0.1.9/pyrender/http_service/api/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2576 2022-07-21 20:50:28.000000 web-render-0.1.9/pyrender/http_service/api/view.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      662 2022-06-17 10:48:07.000000 web-render-0.1.9/pyrender/http_service/main.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      194 2022-06-17 10:46:53.000000 web-render-0.1.9/pyrender/http_service/routing.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      986 2022-06-17 10:47:14.000000 web-render-0.1.9/pyrender/http_service/service.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2543 2022-07-21 20:58:31.000000 web-render-0.1.9/pyrender/interface.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.583660 web-render-0.1.9/pyrender/playwright_service/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-07-27 13:04:20.000000 web-render-0.1.9/pyrender/playwright_service/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     5645 2023-05-05 19:00:51.000000 web-render-0.1.9/pyrender/playwright_service/main.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.583660 web-render-0.1.9/pyrender/selenium_service/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2022-06-14 12:19:58.000000 web-render-0.1.9/pyrender/selenium_service/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     9365 2022-07-27 13:24:13.000000 web-render-0.1.9/pyrender/selenium_service/main.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1481 2022-06-17 10:46:21.000000 web-render-0.1.9/pyrender/tool.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)       38 2023-05-05 19:01:46.587660 web-render-0.1.9/setup.cfg
+-rw-rw-r--   0 repente   (1000) repente   (1000)     3427 2023-05-05 19:00:51.000000 web-render-0.1.9/setup.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2023-05-05 19:01:46.583660 web-render-0.1.9/web_render.egg-info/
+-rw-rw-r--   0 repente   (1000) repente   (1000)      454 2023-05-05 19:01:46.000000 web-render-0.1.9/web_render.egg-info/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      613 2023-05-05 19:01:46.000000 web-render-0.1.9/web_render.egg-info/SOURCES.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        1 2023-05-05 19:01:46.000000 web-render-0.1.9/web_render.egg-info/dependency_links.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       89 2023-05-05 19:01:46.000000 web-render-0.1.9/web_render.egg-info/requires.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        9 2023-05-05 19:01:46.000000 web-render-0.1.9/web_render.egg-info/top_level.txt
```

### Comparing `web-render-0.1.8/pyrender/http_service/api/view.py` & `web-render-0.1.9/pyrender/http_service/api/view.py`

 * *Files identical despite different names*

### Comparing `web-render-0.1.8/pyrender/http_service/main.py` & `web-render-0.1.9/pyrender/http_service/main.py`

 * *Files identical despite different names*

### Comparing `web-render-0.1.8/pyrender/http_service/service.py` & `web-render-0.1.9/pyrender/http_service/service.py`

 * *Files identical despite different names*

### Comparing `web-render-0.1.8/pyrender/interface.py` & `web-render-0.1.9/pyrender/interface.py`

 * *Files identical despite different names*

### Comparing `web-render-0.1.8/pyrender/playwright_service/main.py` & `web-render-0.1.9/pyrender/playwright_service/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         _web_wait.until(handler(args))
 
 
     def set_url_for_task(self, message: MessageProtocol, single_page=False) -> Dict:
         ren_req = IRenderRequestFlask(**message.payload)
         page = self.get_page()
 
-        page.route(re.compile(r"(\.png$)|(\.jpg$)"), lambda route: route.abort())
+        # page.route(re.compile(r"(\.png$)|(\.jpg$)"), lambda route: route.abort())
         page.goto(message.payload['url'], wait_until="domcontentloaded",
                   timeout=self.config.LOAD_TIMEOUT * 1000)
 
         js_data = None
 
         if ren_req.jscript:
             result = page.evaluate(ren_req.jscript)
```

### Comparing `web-render-0.1.8/pyrender/selenium_service/main.py` & `web-render-0.1.9/pyrender/selenium_service/main.py`

 * *Files identical despite different names*

### Comparing `web-render-0.1.8/pyrender/tool.py` & `web-render-0.1.9/pyrender/tool.py`

 * *Files identical despite different names*

### Comparing `web-render-0.1.8/setup.py` & `web-render-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     long_description = fh.read()
 
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setup(
     # Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
     name="web-render",
     # Номер версии вашего пакета. Обычно используется семантическое управление версиями.
-    version="0.1.8",
+    version="0.1.9",
     # Имя автора.
     author="Andrey Plugin",
     # Его почта.
     author_email="9keepa@gmail.com",
     # Краткое описание, которое будет показано на странице PyPi.
     description="Web sites render.",
     # Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
```

### Comparing `web-render-0.1.8/web_render.egg-info/SOURCES.txt` & `web-render-0.1.9/web_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

