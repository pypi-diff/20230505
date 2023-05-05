# Comparing `tmp/yeref-0.1.54.tar.gz` & `tmp/yeref-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.54.tar", last modified: Thu May  4 14:51:02 2023, max compression
+gzip compressed data, was "yeref-0.1.55.tar", last modified: Fri May  5 13:12:35 2023, max compression
```

## Comparing `yeref-0.1.54.tar` & `yeref-0.1.55.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 14:51:02.605005 yeref-0.1.54/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 14:51:02.605188 yeref-0.1.54/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-04 14:51:02.605824 yeref-0.1.54/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-04 14:50:49.000000 yeref-0.1.54/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 14:51:02.599314 yeref-0.1.54/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.54/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   508262 2023-05-04 14:44:17.000000 yeref-0.1.54/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.54/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 14:51:02.604210 yeref-0.1.54/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-05 13:12:35.792867 yeref-0.1.55/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-05 13:12:35.793152 yeref-0.1.55/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-05 13:12:35.794153 yeref-0.1.55/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-05 13:12:14.000000 yeref-0.1.55/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-05 13:12:35.785848 yeref-0.1.55/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.55/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   508189 2023-05-05 13:09:46.000000 yeref-0.1.55/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.55/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-05 13:12:35.792120 yeref-0.1.55/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.54/setup.py` & `yeref-0.1.55/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.54',
+      version='0.1.55',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,14 +39,14 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.54-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.55-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
```

### Comparing `yeref-0.1.54/yeref/l_.py` & `yeref-0.1.55/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1141,15 +1141,15 @@
     'en': "👩🏽‍💻 <b>Insert</b> a link to the Telegram channel to analyze financial performance",
     'es': "👩🏽‍💻 <b>Inserta</b> un enlace al canal de Telegram para analizar el desempeño financiero",
     'fr': "👩🏽‍💻 <b>Insérez</b> un lien vers la chaîne Telegram pour analyser les performances financières",
     'zh': "👩🏽‍💻<b>插入</b>到 Telegram 频道的链接以分析财务绩效",
     'ar': "👩🏽‍💻 <b>أدخل</b> رابطًا إلى قناة Telegram لتحليل الأداء المالي",
 }
 l_generate_wait = {
-    'ru': "👩🏽‍💻 <b>Дождись</b> окончания генерации..",
+    'ru': "👩🏽‍💻 <b>Выбери режим</b> и <b>дождись</b> окончания генерации..",
     'en': "👩🏽‍💻 <b>Wait for</b> the generation to finish..",
     'es': "👩🏽‍💻 <b>Espera a</b> que termine la generación..",
     'fr': "👩🏽‍💻 <b>Attendez que</b> la génération se termine..",
     'zh': "👩🏽‍💻<b>等待</b>生成结束..",
     'ar': "👩🏽‍💻 <b>انتظر حتى</b> ينتهي الجيل ..",
 }
 l_generate_subcribe = {
@@ -2737,15 +2737,15 @@
     'en': "👇🏽 Push the ‹channel› to add into your channel (with default settings): @{0}\n\n👮🏽‍♀️ Or add bot as <b>Admin</b> via Settings of your channel: ‹👤Add Admin›\n\n👮🏽‍♀️ If you can't add channel, try to change <b>Custom Title</b> (look screenshot)",
     'es': "👇🏽 Presione ‹➕ Agregar grupo› para agregar a su grupo (con la configuración predeterminada): @{0}\n\n👮🏽‍♀️ O agregue bot como <b>Administrador</b> a través de la Configuración de su grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si no puede agregar un grupo, intente cambiar <b>Título personalizado</b> (ver captura de pantalla)",
     'fr': "👇🏽 Appuyez sur ‹➕ Ajouter un channele› pour ajouter à votre channele (avec les paramètres par défaut): @{0}\n\n👮🏽‍♀️ Ou ajoutez le bot en tant qu'<b>administrateur</b> via les paramètres de votre channele : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si vous ne pouvez pas ajouter de channele, essayez de modifier le <b>Titre personnalisé</b> (regardez la capture d'écran)",
     'zh': "👇🏽 按下‹➕添加群組›以添加到您的群組（使用默認設置）: @{0}\n\n👮🏽‍♀️ 或通過您組的設置將機器人添加為 <b>Admin</b>：‹👤添加管理員›\n\n👮🏽‍♀️ 如果無法添加組，請嘗試更改 <b>自定義標題</b>（看截圖）",
     'ar': "👇🏽 اضغط على ‹➕ إضافة مجموعة› لإضافتها إلى مجموعتك (بالإعدادات الافتراضية): @{0}\n\n👮🏽‍♀️ أو أضف البوت كـ <b> مسؤول </b> عبر إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتمكن من إضافة مجموعة ، فحاول تغيير <b> عنوان مخصص </b> (انظر في لقطة الشاشة)",
 }
 l_add_chn_txt_call = {
-    'ru': "👮🏽‍♀️ Добавь @{0}-бота как Administrator через настройки своего канала: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется канал, то измени Должность",
+    'ru': "👮🏽‍♀️ Добавь @{0}-бота как Administrator через настройки своего канала: ‹👤Add Admin›",
     'en': "👇🏽 Push the ‹channel› to add into your channel (with default settings): @{0}\n\n👮🏽‍♀️ Or add bot as <b>Admin</b> via Settings of your channel: ‹👤Add Admin›\n\n👮🏽‍♀️ If you can't add channel, try to change <b>Custom Title</b> (look screenshot)",
     'es': "👇🏽 Presione ‹➕ Agregar grupo› para agregar a su grupo (con la configuración predeterminada): @{0}\n\n👮🏽‍♀️ O agregue bot como <b>Administrador</b> a través de la Configuración de su grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si no puede agregar un grupo, intente cambiar <b>Título personalizado</b> (ver captura de pantalla)",
     'fr': "👇🏽 Appuyez sur ‹➕ Ajouter un channele› pour ajouter à votre channele (avec les paramètres par défaut): @{0}\n\n👮🏽‍♀️ Ou ajoutez le bot en tant qu'<b>administrateur</b> via les paramètres de votre channele : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si vous ne pouvez pas ajouter de channele, essayez de modifier le <b>Titre personnalisé</b> (regardez la capture d'écran)",
     'zh': "👇🏽 按下‹➕添加群組›以添加到您的群組（使用默認設置）: @{0}\n\n👮🏽‍♀️ 或通過您組的設置將機器人添加為 <b>Admin</b>：‹👤添加管理員›\n\n👮🏽‍♀️ 如果無法添加組，請嘗試更改 <b>自定義標題</b>（看截圖）",
     'ar': "👇🏽 اضغط على ‹➕ إضافة مجموعة› لإضافتها إلى مجموعتك (بالإعدادات الافتراضية): @{0}\n\n👮🏽‍♀️ أو أضف البوت كـ <b> مسؤول </b> عبر إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتمكن من إضافة مجموعة ، فحاول تغيير <b> عنوان مخصص </b> (انظر في لقطة الشاشة)",
 }
 l_add_chn_button = {
```

### Comparing `yeref-0.1.54/yeref/yeref.py` & `yeref-0.1.55/yeref/yeref.py`

 * *Files identical despite different names*

