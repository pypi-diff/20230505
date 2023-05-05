# Comparing `tmp/pyqt-openai-0.0.171.tar.gz` & `tmp/pyqt-openai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.0.171.tar", last modified: Sat Mar 11 06:20:39 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.2.tar", last modified: Fri May  5 02:49:50 2023, max compression
```

## Comparing `pyqt-openai-0.0.171.tar` & `pyqt-openai-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 06:20:39.741450 pyqt-openai-0.0.171/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.0.171/LICENSE
--rw-rw-rw-   0        0        0     2453 2023-03-11 06:20:39.740415 pyqt-openai-0.0.171/PKG-INFO
--rw-rw-rw-   0        0        0     2114 2023-03-11 04:27:05.000000 pyqt-openai-0.0.171/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 06:20:39.698530 pyqt-openai-0.0.171/pyqt_openai/
--rw-rw-rw-   0        0        0       30 2023-02-26 06:32:38.000000 pyqt-openai-0.0.171/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     3710 2023-02-26 08:39:58.000000 pyqt-openai-0.0.171/pyqt_openai/chatWidget.py
-drwxrwxrwx   0        0        0        0 2023-03-11 06:20:39.736463 pyqt-openai-0.0.171/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.0.171/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      526 2023-02-26 06:05:36.000000 pyqt-openai-0.0.171/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.0.171/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0    17642 2023-03-11 03:36:28.000000 pyqt-openai-0.0.171/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     3281 2023-02-26 06:58:16.000000 pyqt-openai-0.0.171/pyqt_openai/notifier.py
-drwxrwxrwx   0        0        0        0 2023-03-11 06:20:39.731474 pyqt-openai-0.0.171/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     2453 2023-03-11 06:20:39.000000 pyqt-openai-0.0.171/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-03-11 06:20:39.000000 pyqt-openai-0.0.171/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 06:20:39.000000 pyqt-openai-0.0.171/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-03-11 06:20:39.000000 pyqt-openai-0.0.171/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-11 06:20:39.000000 pyqt-openai-0.0.171/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-11 06:20:39.742412 pyqt-openai-0.0.171/setup.cfg
--rw-rw-rw-   0        0        0      767 2023-03-11 03:38:15.000000 pyqt-openai-0.0.171/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.450469 pyqt-openai-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4736 2023-05-05 02:49:50.449469 pyqt-openai-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4351 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.342585 pyqt-openai-0.1.2/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6738 2023-04-09 06:45:06.000000 pyqt-openai-0.1.2/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2144 2023-05-05 02:48:09.000000 pyqt-openai-0.1.2/pyqt_openai/apiData.py
+-rw-rw-rw-   0        0        0     6771 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/chatWidget.py
+-rw-rw-rw-   0        0        0     8132 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/clickableTooltip.py
+-rw-rw-rw-   0        0        0     5072 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/convListWidget.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.405931 pyqt-openai-0.1.2/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.2/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.2/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0      654 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/download.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.2/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.2/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.2/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1383 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3768 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    21864 2023-05-05 02:49:02.000000 pyqt-openai-0.1.2/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1788 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3270 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.413224 pyqt-openai-0.1.2/pyqt_openai/prompt/
+-rw-rw-rw-   0        0        0        0 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     1574 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/propPage.py
+-rw-rw-rw-   0        0        0     3351 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/prompt/templatePage.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.428156 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2220 2023-05-05 00:11:49.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4706 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    11101 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0    21685 2023-05-05 02:31:02.000000 pyqt-openai-0.1.2/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5931 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-04-08 11:47:46.000000 pyqt-openai-0.1.2/pyqt_openai/svgLabel.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.447474 pyqt-openai-0.1.2/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0     1773 2023-04-22 00:05:31.000000 pyqt-openai-0.1.2/pyqt_openai/test/htmlformat.py
+-rw-rw-rw-   0        0        0     1280 2023-04-23 09:02:45.000000 pyqt-openai-0.1.2/pyqt_openai/test/rightSideBarTab.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:49:50.379999 pyqt-openai-0.1.2/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0     4736 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2023-05-05 02:49:50.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 02:49:49.000000 pyqt-openai-0.1.2/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 02:49:50.450469 pyqt-openai-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      958 2023-05-05 02:31:28.000000 pyqt-openai-0.1.2/setup.py
```

### Comparing `pyqt-openai-0.0.171/LICENSE` & `pyqt-openai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.0.171/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.2/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.0.171/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.2/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.0.171/pyqt_openai/main.py` & `pyqt-openai-0.1.2/pyqt_openai/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,110 +1,221 @@
-import openai, requests, os, platform, subprocess
+import inspect
+import json, webbrowser
+
+import openai, requests, os
 
 from chatWidget import Prompt, ChatBrowser
 
-# this API key should be yours
 from notifier import NotifierWidget
 
-# for script
-openai.api_key = '[MY_OPENAPI_API_KEY]'
-# for subprocess (mostly)
-# os.environ['OPENAI_API_KEY'] = '[MY_OPENAPI_API_KEY]'
-
-from PyQt5.QtCore import Qt, QCoreApplication, QThread, pyqtSignal
-from PyQt5.QtGui import QGuiApplication, QFont, QIcon
-from PyQt5.QtWidgets import QMainWindow, QApplication, QVBoxLayout, QWidget, QSplitter, QComboBox, QSpinBox, \
-    QFormLayout, QDoubleSpinBox, QPushButton, QFileDialog, QToolBar, QWidgetAction, QHBoxLayout, QAction, QMenu, \
-    QSystemTrayIcon, QMessageBox, QSizePolicy, QGroupBox, QLineEdit, QLabel
+from qtpy.QtCore import Qt, QCoreApplication, QThread, QSettings, QEvent, Signal
+from qtpy.QtGui import QGuiApplication, QFont, QIcon, QColor, QCursor
+from qtpy.QtWidgets import QMainWindow, QApplication, QVBoxLayout, QWidget, QSplitter, QComboBox, QSpinBox, \
+    QFileDialog, QToolBar, QWidgetAction, QHBoxLayout, QAction, QMenu, \
+    QSystemTrayIcon, QMessageBox, QSizePolicy, QLabel, QListWidgetItem, QLineEdit, QPushButton
+
+from pyqt_openai.apiData import getModelEndpoint
+from pyqt_openai.clickableTooltip import ClickableTooltip
+from pyqt_openai.leftSideBar import LeftSideBar
+from pyqt_openai.apiData import ModelData
+from pyqt_openai.prompt.promptGeneratorWidget import PromptGeneratorWidget
+from pyqt_openai.right_sidebar.aiPlaygroundWidget import AIPlaygroundWidget
+from pyqt_openai.svgButton import SvgButton
+from pyqt_openai.sqlite import SqliteDatabase
 
 QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
 QCoreApplication.setAttribute(Qt.AA_UseHighDpiPixmaps)  # HighDPI support
-QGuiApplication.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
+# qt version should be above 5.14
+# todo check the qt version with qtpy
+if os.environ['QT_API'] == 'pyqt5' or os.environ['QT_API'] != 'pyside6':
+    QGuiApplication.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
 
 QApplication.setFont(QFont('Arial', 12))
 
 
 class OpenAIThread(QThread):
-    replyGenerated = pyqtSignal(str, bool, bool)
+    """
+    == replyGenerated Signal ==
+    First: response
+    Second: user or AI
+    Third: streaming a chat completion or not
+    Forth: Image generation with DALL-E or not
+    """
+    replyGenerated = Signal(str, bool, bool, bool)
+    streamFinished = Signal()
 
-    def __init__(self, openai_arg, idx, *args, **kwargs):
+    def __init__(self, model, openai_arg, is_img, remember_f, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.__model = model
+        self.__endpoint = getModelEndpoint(model)
         self.__openai_arg = openai_arg
-        self.__idx = idx
+        self.__remember_f = remember_f
+        self.__is_img = is_img
 
     def run(self):
-        if self.__idx == 0:
-            openai_object = openai.Completion.create(
-                **self.__openai_arg
-            )
-
-            response_text = openai_object['choices'][0]['text'].strip()
-
-            self.replyGenerated.emit(response_text, False, False)
-        elif self.__idx == 1:
-            try:
+        try:
+            if self.__is_img:
                 response = openai.Image.create(
                     **self.__openai_arg
                 )
 
+                # TODO get a lot of images
                 image_url = response['data'][0]['url']
 
-                self.replyGenerated.emit(image_url, False, True)
-            except openai.error.InvalidRequestError as e:
-                self.replyGenerated.emit('Your request was rejected as a result of our safety system. \n'
-                                         'Your prompt may contain text that is not allowed by our safety system.', False)
+                self.replyGenerated.emit(image_url, False, False, True)
+            else:
+                if self.__endpoint == '/v1/chat/completions':
+                    response = openai.ChatCompletion.create(
+                           **self.__openai_arg
+                    )
+                    # if it is streaming, type will be generator
+                    if inspect.isgenerator(response):
+                        for chunk in response:
+                            delta = chunk['choices'][0]['delta']
+                            response_text = delta.get('content', '')
+                            if response_text:
+                                self.replyGenerated.emit(response_text, False, True, False)
+                            else:
+                                finish_reason = chunk['choices'][0].get('finish_reason', '')
+                                if finish_reason:
+                                    self.streamFinished.emit()
+                    else:
+                        response_text = response['choices'][0]['message']['content']
+                        self.replyGenerated.emit(response_text, False, False, False)
+                elif self.__endpoint == '/v1/completions':
+                    openai_object = openai.Completion.create(
+                        **self.__openai_arg
+                    )
+
+                    response_text = openai_object['choices'][0]['text'].strip()
+
+                    # this doesn't store any data, so we manually do that every time
+                    if self.__remember_f:
+                        conv = {
+                            'prompt': self.__openai_arg['prompt'],
+                            'response': response_text,
+                        }
+
+                        with open('conv.json', 'a') as f:
+                            f.write(json.dumps(conv) + '\n')
+
+                    self.replyGenerated.emit(response_text, False, False, False)
+        except openai.error.InvalidRequestError as e:
+            print(e)
+            self.replyGenerated.emit('<p style="color:red">Your request was rejected as a result of our safety system.<br/>'
+                                     'Your prompt may contain text that is not allowed by our safety system.</p>', False, False, False)
+        except openai.error.RateLimitError as e:
+            self.replyGenerated.emit(f'<p style="color:red">{e}<br/>Check the usage: https://platform.openai.com/account/usage<br/>Update to paid account: https://platform.openai.com/account/billing/overview', False, False, False)
 
 
 class OpenAIChatBot(QMainWindow):
     def __init__(self):
         super().__init__()
         self.__initVal()
         self.__initUi()
 
     def __initVal(self):
-        self.__engine = "text-davinci-003"
-        self.__temperature = 0.0
-        self.__max_tokens = 256
-        self.__top_p = 1.0
-        self.__frequency_penalty = 0.0
-        self.__presence_penalty = 0.0
+        # db
+        self.__db = SqliteDatabase()
+
+        # managing with ini file or something else
+        self.__ini_etc_dict = {}
+
+        self.__remember_past_conv = False
+        self.__finishReason = False
+        self.__modelData = ModelData()
+
+        self.__ini_etc_dict['remember_past_conv'] = self.__remember_past_conv
+        self.__ini_etc_dict['finishReason'] = self.__finishReason
+        self.__ini_etc_dict['modelData'] = self.__modelData
+
+        self.__settings_struct = QSettings('pyqt_openai.ini', QSettings.IniFormat)
+
+        # make it compatible with version which was used json file as a database
+        if self.__isConvHistoryJsonExists():
+            self.__migrateJsonToSqlite()
+
+        # "remember past conv" feature
+        if self.__settings_struct.contains('REMEMBER_PAST_CONVERSATION'):
+            self.__remember_past_conv = True if self.__settings_struct.value('REMEMBER_PAST_CONVERSATION') == '1' else False
+        else:
+            self.__settings_struct.setValue('REMEMBER_PAST_CONVERSATION', '0')
+
+        # don't care about this - just saving past conversation in gpt 3 and below
+        if os.path.exists('conv.json'):
+            pass
+        else:
+            with open('conv.json', 'w') as f:
+                json.dump({}, f)
+
+    def __isConvHistoryJsonExists(self):
+        return os.path.exists('conv_history.json')
+
+    def __migrateJsonToSqlite(self):
+        self.__db.convertJsonIntoSql()
+        os.remove('conv_history.json')
 
     def __initUi(self):
         self.setWindowTitle('PyQt OpenAI Chatbot')
         self.setWindowIcon(QIcon('ico/openai.svg'))
+
+        self.__leftSideBarWidget = LeftSideBar()
+        self.__browser = ChatBrowser()
         self.__prompt = Prompt()
+        self.__lineEdit = self.__prompt.getTextEdit()
 
-        self.__aiTypeCmbBox = QComboBox()
-        self.__aiTypeCmbBox.addItems(['Text/Code Completion', 'Image Generation'])
+        self.__leftSideBarWidget.initHistory(self.__db)
+        self.__leftSideBarWidget.added.connect(self.__addConv)
+        self.__leftSideBarWidget.changed.connect(self.__changeConv)
+        self.__leftSideBarWidget.deleted.connect(self.__deleteConv)
+        self.__leftSideBarWidget.convUpdated.connect(self.__updateConv)
+        self.__leftSideBarWidget.export.connect(self.__export)
 
-        self.__lineEdit = self.__prompt.getTextEdit()
         self.__lineEdit.setPlaceholderText('Write some text...')
         self.__lineEdit.returnPressed.connect(self.__chat)
 
-        self.__browser = ChatBrowser()
+        self.__browser.convUnitUpdated.connect(self.__updateConvUnit)
 
         lay = QHBoxLayout()
-        lay.addWidget(self.__aiTypeCmbBox)
         lay.addWidget(self.__prompt)
         lay.setSpacing(0)
         lay.setContentsMargins(0, 0, 0, 0)
 
-        self.__aiTypeCmbBox.setMaximumHeight(self.__prompt.sizeHint().height())
-
         self.__queryWidget = QWidget()
         self.__queryWidget.setLayout(lay)
         self.__queryWidget.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
 
         lay = QVBoxLayout()
         lay.addWidget(self.__browser)
         lay.addWidget(self.__queryWidget)
         lay.setSpacing(0)
+        lay.setContentsMargins(0, 0, 0, 0)
         chatWidget = QWidget()
         chatWidget.setLayout(lay)
 
+        self.__aiPlaygroundWidget = AIPlaygroundWidget(self.__db, self.__ini_etc_dict, self.__modelData)
+
+        self.__promptGeneratorWidget = PromptGeneratorWidget()
+
+        self.__rightSideBar = QSplitter()
+        self.__rightSideBar.setOrientation(Qt.Vertical)
+        self.__rightSideBar.addWidget(self.__aiPlaygroundWidget)
+        self.__rightSideBar.addWidget(self.__promptGeneratorWidget)
+        self.__rightSideBar.setSizes([600, 400])
+        self.__rightSideBar.setChildrenCollapsible(False)
+        self.__rightSideBar.setHandleWidth(2)
+        self.__rightSideBar.setStyleSheet(
+        '''
+        QSplitter::handle:vertical
+        {
+            background: #CCC;
+            height: 1px;
+        }
+        ''')
+
         # background app
         menu = QMenu()
 
         action = QAction("Quit", self)
         action.setIcon(QIcon('ico/close.svg'))
 
         action.triggered.connect(app.quit)
@@ -115,295 +226,264 @@
         tray_icon.setIcon(QIcon('ico/openai.svg'))
         tray_icon.activated.connect(self.__activated)
 
         tray_icon.setContextMenu(menu)
 
         tray_icon.show()
 
-        modelComboBox = QComboBox()
-        modelComboBox.addItems([
-            'text-davinci-003',
-            'text-curie-001',
-            'text-babbage-001',
-            'text-ada-001',
-            'code-davinci-002',
-            'code-cushman-001'
-        ])
-        modelComboBox.setCurrentText(self.__engine)
-        modelComboBox.currentTextChanged.connect(self.__modelChanged)
-
-        temperatureSpinBox = QDoubleSpinBox()
-        temperatureSpinBox.setRange(0, 1)
-        temperatureSpinBox.setAccelerated(True)
-        temperatureSpinBox.setSingleStep(0.01)
-        temperatureSpinBox.setValue(self.__temperature)
-        temperatureSpinBox.valueChanged.connect(self.__temperatureChanged)
-
-        maxTokensSpinBox = QSpinBox()
-        maxTokensSpinBox.setRange(0, 4000)
-        maxTokensSpinBox.setAccelerated(True)
-        maxTokensSpinBox.setValue(self.__max_tokens)
-        maxTokensSpinBox.valueChanged.connect(self.__maxTokensChanged)
-
-        toppSpinBox = QDoubleSpinBox()
-        toppSpinBox.setRange(0, 1)
-        toppSpinBox.setAccelerated(True)
-        toppSpinBox.setSingleStep(0.01)
-        toppSpinBox.setValue(self.__top_p)
-        toppSpinBox.valueChanged.connect(self.__toppChanged)
-
-        frequencyPenaltySpinBox = QDoubleSpinBox()
-        frequencyPenaltySpinBox.setRange(0, 2)
-        frequencyPenaltySpinBox.setAccelerated(True)
-        frequencyPenaltySpinBox.setSingleStep(0.01)
-        frequencyPenaltySpinBox.setValue(self.__frequency_penalty)
-        frequencyPenaltySpinBox.valueChanged.connect(self.__frequencyPenaltyChanged)
-
-        presencePenaltySpinBox = QDoubleSpinBox()
-        presencePenaltySpinBox.setRange(0, 2)
-        presencePenaltySpinBox.setAccelerated(True)
-        presencePenaltySpinBox.setSingleStep(0.01)
-        presencePenaltySpinBox.setValue(self.__presence_penalty)
-        presencePenaltySpinBox.valueChanged.connect(self.__presencePenaltyChanged)
-
-        saveAsLogButton = QPushButton('Save')
-        saveAsLogButton.clicked.connect(self.__saveAsLog)
-
-        apiLbl = QLabel('API')
-        self.__apiLineEdit = QLineEdit()
-        self.__apiLineEdit.setPlaceholderText('Write your API Key...')
-        self.__apiLineEdit.returnPressed.connect(self.__setApi)
-        self.__apiLineEdit.setEchoMode(QLineEdit.Password)
-
-        apiBtn = QPushButton('Use')
-        apiBtn.clicked.connect(self.__setApi)
-
-        lay = QHBoxLayout()
-        lay.addWidget(self.__apiLineEdit)
-        lay.addWidget(apiBtn)
-        lay.setContentsMargins(0, 0, 0, 0)
-
-        apiWidget = QWidget()
-        apiWidget.setLayout(lay)
-
-        self.__apiCheckPreviewLbl = QLabel('')
-        self.__apiCheckPreviewLbl.hide()
-        self.__apiCheckPreviewLbl.setFont(QFont('Arial', 10))
-
-        lay = QVBoxLayout()
-        lay.addWidget(apiLbl)
-        lay.addWidget(apiWidget)
-        lay.addWidget(self.__apiCheckPreviewLbl)
-        lay.setAlignment(Qt.AlignTop)
-
-        apiGrpBox = QGroupBox()
-        apiGrpBox.setLayout(lay)
-        apiGrpBox.setFixedHeight(apiGrpBox.sizeHint().height() + self.__apiCheckPreviewLbl.fontMetrics().boundingRect('M').height())
-
-        lay = QFormLayout()
-        lay.addRow('Model', modelComboBox)
-        lay.addRow('Temperature', temperatureSpinBox)
-        lay.addRow('Maximum length', maxTokensSpinBox)
-        lay.addRow('Top P', toppSpinBox)
-        lay.addRow('Frequency penalty', frequencyPenaltySpinBox)
-        lay.addRow('Presence penalty', presencePenaltySpinBox)
-        lay.addWidget(saveAsLogButton)
-
-        optionGrpBox = QGroupBox()
-        optionGrpBox.setTitle('Option')
-        optionGrpBox.setLayout(lay)
-
-        # find the training data
-        self.__findDataLineEdit = QLineEdit()
-
-        findDataBtn = QPushButton('Find...')
-        findDataBtn.clicked.connect(self.__findData)
-
-        self.__fineTuningBtn = QPushButton('Fine Tuning')
-        self.__fineTuningBtn.clicked.connect(self.__fineTuning)
-        self.__fineTuningBtn.setDisabled(True)
-
-        lay = QHBoxLayout()
-        lay.setSpacing(0)
-        lay.addWidget(self.__findDataLineEdit)
-        lay.addWidget(findDataBtn)
-        lay.setAlignment(Qt.AlignTop)
-        lay.setContentsMargins(5, 5, 5, 1)
-
-        fineTuneGrpBoxTopWidget = QWidget()
-        fineTuneGrpBoxTopWidget.setLayout(lay)
-
-        lay = QVBoxLayout()
-        lay.addWidget(self.__fineTuningBtn)
-        lay.setAlignment(Qt.AlignTop)
-
-        fineTuneGrpBoxBottomWidget = QWidget()
-        fineTuneGrpBoxBottomWidget.setLayout(lay)
-        lay.setContentsMargins(5, 1, 5, 5)
-
-        lay = QVBoxLayout()
-        lay.addWidget(fineTuneGrpBoxTopWidget)
-        lay.addWidget(fineTuneGrpBoxBottomWidget)
-        lay.setAlignment(Qt.AlignTop)
-        lay.setSpacing(0)
-        lay.setContentsMargins(0, 0, 0, 0)
-
-        fineTuneGrpBox = QGroupBox()
-        fineTuneGrpBox.setTitle('Fine-tune training (coming soon)')
-        fineTuneGrpBox.setLayout(lay)
-
-        lay = QVBoxLayout()
-        lay.addWidget(apiGrpBox)
-        lay.addWidget(optionGrpBox)
-        lay.addWidget(fineTuneGrpBox)
-
-        self.__sidebarWidget = QWidget()
-        self.__sidebarWidget.setLayout(lay)
-
         mainWidget = QSplitter()
+        mainWidget.addWidget(self.__leftSideBarWidget)
         mainWidget.addWidget(chatWidget)
-        mainWidget.addWidget(self.__sidebarWidget)
-        mainWidget.setSizes([700, 300])
+        mainWidget.addWidget(self.__rightSideBar)
+        mainWidget.setSizes([100, 500, 400])
         mainWidget.setChildrenCollapsible(False)
         mainWidget.setHandleWidth(2)
         mainWidget.setStyleSheet(
         '''
         QSplitter::handle:horizontal
         {
             background: #CCC;
             height: 1px;
         }
         ''')
 
+        # set action and toolbar
+        self.__setActions()
+        self.__setToolBar()
+
+        # load ini file
+        self.__loadApiKeyInIni()
+
+        # check if loaded API_KEY from ini file is not empty
+        if openai.api_key:
+            self.__setApi()
+        # if it is empty
+        else:
+            self.__lineEdit.setEnabled(False)
+            self.__apiCheckPreviewLbl.hide()
+
         self.setCentralWidget(mainWidget)
         self.resize(1024, 768)
 
-        self.__browser.showText('Hello!', True)
-        self.__browser.showText('Hello! How may i help you?', False)
-
-        # TODO "save the api key" option
         self.__lineEdit.setFocus()
-        self.__lineEdit.setEnabled(False)
-
-        self.__setActions()
-        self.__setToolBar()
 
     def __setActions(self):
         self.__stackAction = QWidgetAction(self)
-        self.__stackBtn = QPushButton('Stack on Top')
+        self.__stackBtn = SvgButton()
+        self.__stackBtn.setIcon('ico/stackontop.svg')
         self.__stackBtn.setCheckable(True)
         self.__stackBtn.toggled.connect(self.__stackToggle)
         self.__stackAction.setDefaultWidget(self.__stackBtn)
+        self.__stackBtn.setToolTip('Always On Top')
 
         self.__sideBarAction = QWidgetAction(self)
-        self.__sideBarBtn = QPushButton('Show Sidebar')
+        self.__sideBarBtn = SvgButton()
+        self.__sideBarBtn.setIcon('ico/sidebar.svg')
         self.__sideBarBtn.setCheckable(True)
-        self.__sideBarBtn.setChecked(True)
-        self.__sideBarBtn.toggled.connect(self.__sidebarWidget.setVisible)
+        self.__sideBarBtn.toggled.connect(self.__leftSideBarWidget.setVisible)
         self.__sideBarAction.setDefaultWidget(self.__sideBarBtn)
+        self.__sideBarBtn.setToolTip('Chat List')
+        self.__sideBarBtn.setChecked(True)
+
+        self.__settingAction = QWidgetAction(self)
+        self.__settingBtn = SvgButton()
+        self.__settingBtn.setIcon('ico/setting.svg')
+        self.__settingBtn.toggled.connect(self.__aiPlaygroundWidget.setVisible)
+        self.__settingAction.setDefaultWidget(self.__settingBtn)
+        self.__settingBtn.setToolTip('Settings')
+        self.__settingBtn.setCheckable(True)
+        self.__settingBtn.setChecked(True)
+        self.__settingBtn.setChecked(False)
+
+        self.__promptAction = QWidgetAction(self)
+        self.__promptBtn = SvgButton()
+        self.__promptBtn.setIcon('ico/prompt.svg')
+        self.__promptAction.setDefaultWidget(self.__promptBtn)
+        self.__promptBtn.toggled.connect(self.__promptGeneratorWidget.setVisible)
+        self.__promptBtn.setToolTip('Prompt Generator')
+        self.__promptBtn.setCheckable(True)
+        self.__promptBtn.setChecked(True)
+        self.__promptBtn.setChecked(False)
 
         self.__transparentAction = QWidgetAction(self)
         self.__transparentSpinBox = QSpinBox()
         self.__transparentSpinBox.setRange(0, 100)
         self.__transparentSpinBox.setValue(100)
         self.__transparentSpinBox.valueChanged.connect(self.__setTransparency)
         self.__transparentSpinBox.setToolTip('Set Transparency of Window')
-        self.__transparentAction.setDefaultWidget(self.__transparentSpinBox)
+
+        lay = QHBoxLayout()
+        lay.addWidget(QLabel('Window Transparency'))
+        lay.addWidget(self.__transparentSpinBox)
+
+        transparencyActionWidget = QWidget()
+        transparencyActionWidget.setLayout(lay)
+        self.__transparentAction.setDefaultWidget(transparencyActionWidget)
+
+        self.__apiCheckPreviewLbl = QLabel('API key is valid')
+        self.__apiCheckPreviewLbl.setFont(QFont('Arial', 10))
+
+        self.__apiAction = QWidgetAction(self)
+        apiLbl = QLabel('API')
+
+        self.__apiLineEdit = QLineEdit()
+        self.__apiLineEdit.setPlaceholderText('Write your API Key...')
+        self.__apiLineEdit.returnPressed.connect(self.__setApi)
+        self.__apiLineEdit.setEchoMode(QLineEdit.Password)
+
+        apiBtn = QPushButton('Use')
+        apiBtn.clicked.connect(self.__setApi)
+
+        lay = QHBoxLayout()
+        lay.addWidget(apiLbl)
+        lay.addWidget(self.__apiLineEdit)
+        lay.addWidget(apiBtn)
+        lay.addWidget(self.__apiCheckPreviewLbl)
+
+        apiWidget = QWidget()
+        apiWidget.setLayout(lay)
+        self.__apiAction.setDefaultWidget(apiWidget)
 
     def __activated(self, reason):
         if reason == 3:
             self.show()
 
     def __setToolBar(self):
         toolbar = QToolBar()
         lay = QHBoxLayout()
         toolbar.addAction(self.__stackAction)
         toolbar.addAction(self.__sideBarAction)
+        toolbar.addAction(self.__settingAction)
+        toolbar.addAction(self.__promptAction)
         toolbar.addAction(self.__transparentAction)
+        toolbar.addAction(self.__apiAction)
         toolbar.setLayout(lay)
         toolbar.setMovable(False)
         self.addToolBar(toolbar)
+        # QToolbar's layout can't be set spacing with lay.setSpacing so i've just did this instead
+        toolbar.setStyleSheet('QToolBar { spacing: 2px; }')
 
-    def __setApi(self):
-        api_key = self.__apiLineEdit.text()
-        response = requests.get('https://api.openai.com/v1/engines', headers={'Authorization': f'Bearer {api_key}'})
-        print(response.status_code)
-        if response.status_code == 200:
-            openai.api_key = api_key
-            os.environ['OPENAI_API_KEY'] = api_key
-            self.__apiCheckPreviewLbl.setText('API key is valid.')
-            self.__lineEdit.setEnabled(True)
+    def eventFilter(self, source, event):
+        if event.type() == QEvent.ToolTip and source.toolTip():
+            toolTip = ClickableTooltip.showText(
+                QCursor.pos(), source.toolTip(), source)
+            toolTip.linkActivated.connect(self.toolTipLinkClicked)
+            return True
+        return super().eventFilter(source, event)
+
+    def toolTipLinkClicked(self, url):
+        webbrowser.open(url)
+
+    def __setApiKey(self, api_key):
+        # for script
+        openai.api_key = api_key
+        # for subprocess (mostly)
+        os.environ['OPENAI_API_KEY'] = api_key
+        # for showing to the user
+        self.__apiLineEdit.setText(api_key)
+
+    def __loadApiKeyInIni(self):
+        # this api key should be yours
+        if self.__settings_struct.contains('API_KEY'):
+            self.__setApiKey(self.__settings_struct.value('API_KEY'))
         else:
-            self.__apiCheckPreviewLbl.setText('API key is invalid.')
+            self.__settings_struct.setValue('API_KEY', '')
+
+    def __setApi(self):
+        try:
+            api_key = self.__apiLineEdit.text()
+            response = requests.get('https://api.openai.com/v1/engines', headers={'Authorization': f'Bearer {api_key}'})
+            f = response.status_code == 200
+            self.__lineEdit.setEnabled(f)
+            if f:
+                self.__setApiKey(api_key)
+                self.__settings_struct.setValue('API_KEY', api_key)
+
+                self.__aiPlaygroundWidget.setModelInfoByModel(True)
+
+                self.__apiCheckPreviewLbl.setStyleSheet("color: {}".format(QColor(0, 200, 0).name()))
+                self.__apiCheckPreviewLbl.setText('API key is valid')
+            else:
+                raise Exception
+        except Exception as e:
+            self.__apiCheckPreviewLbl.setStyleSheet("color: {}".format(QColor(255, 0, 0).name()))
+            self.__apiCheckPreviewLbl.setText('API key is invalid')
             self.__lineEdit.setEnabled(False)
-        self.__apiCheckPreviewLbl.show()
+            print(e)
+        finally:
+            self.__apiCheckPreviewLbl.show()
 
     def __chat(self):
-        idx = self.__aiTypeCmbBox.currentIndex()
+        info_dict = self.__db.selectInfo()
+        is_img = info_dict['engine'] in ['DALL-E', 'midjourney', 'stable_diffusion']
         openai_arg = ''
-        if idx == 0:
-            openai_arg = {
-                'engine': self.__engine,
-                'prompt': self.__lineEdit.toPlainText(),
-                'temperature': self.__temperature,
-                'max_tokens': self.__max_tokens,
-                'top_p': self.__top_p,
-                'frequency_penalty': self.__frequency_penalty,
-                'presence_penalty': self.__presence_penalty,
-            }
-        elif idx == 1:
+        if is_img:
             openai_arg = {
                 "prompt": self.__lineEdit.toPlainText(),
-                "n": 1,
-                "size": "1024x1024"
+                "n": info_dict['n'],
+                "size": f"{info_dict['width']}x{info_dict['height']}"
             }
+        else:
+            if self.__remember_past_conv:
+                convs = []
+                with open('conv.json', 'r') as f:
+                    for line in f:
+                        conv = json.loads(line.strip())
+                        convs.append(conv)
+            # TODO refactoring
+            if info_dict['engine'] in ['gpt-3.5-turbo', 'gpt-3.5-turbo-0301']:
+                # "assistant" below is for making the AI remember the last question
+                openai_arg = {
+                    'model': info_dict['engine'],
+                    'messages': [
+                        {"role": "system", "content": info_dict['system']},
+                        {"role": "assistant", "content": self.__browser.getAllText()},
+                        {"role": "user", "content": self.__lineEdit.toPlainText()},
+                    ],
+                    # 'temperature': info_dict['temperature'],
+
+                    # won't use max_tokens, this is set to infinite by default
+                    # and i can't find any reason why should i limit the tokens currently
+                    # https://platform.openai.com/docs/api-reference/chat/create
+                    # 'max_tokens': self.__max_tokens,
+
+                    # 'top_p': info_dict['top_p'],
+                    # 'frequency_penalty': info_dict['frequency_penalty'],
+                    # 'presence_penalty': info_dict['presence_penalty'],
+
+                    'stream': info_dict['stream'],
+                }
+            else:
+                openai_arg = info_dict
+        if self.__leftSideBarWidget.isCurrentConvExists():
+            pass
+        else:
+            self.__addConv()
+
         self.__lineEdit.setEnabled(False)
-        self.__t = OpenAIThread(openai_arg, idx)
-        self.__t.replyGenerated.connect(self.__browser.showReply)
-        self.__browser.showText(self.__lineEdit.toPlainText(), True)
+        self.__leftSideBarWidget.setEnabled(False)
+
+        self.__browser.showLabel(self.__lineEdit.toPlainText(), True, False, False)
+
+        self.__t = OpenAIThread(info_dict['engine'], openai_arg, is_img, self.__remember_past_conv)
+        self.__t.replyGenerated.connect(self.__browser.showLabel)
+        self.__t.streamFinished.connect(self.__browser.streamFinished)
         self.__lineEdit.clear()
         self.__t.start()
         self.__t.finished.connect(self.__afterGenerated)
 
     def __afterGenerated(self):
         self.__lineEdit.setEnabled(True)
+        self.__leftSideBarWidget.setEnabled(True)
         self.__lineEdit.setFocus()
         if not self.isVisible():
-            self.__notifierWidget = NotifierWidget()
+            self.__notifierWidget = NotifierWidget(informative_text='Response 👌', detailed_text='Click this!')
             self.__notifierWidget.show()
             self.__notifierWidget.doubleClicked.connect(self.show)
 
-    def __modelChanged(self, v):
-        self.__engine = v
-
-    def __temperatureChanged(self, v):
-        self.__temperature = round(v, 2)
-
-    def __maxTokensChanged(self, v):
-        self.__max_tokens = round(v, 2)
-
-    def __toppChanged(self, v):
-        self.__topp = round(v, 2)
-
-    def __frequencyPenaltyChanged(self, v):
-        self.__frequency_penalty = round(v, 2)
-
-    def __presencePenaltyChanged(self, v):
-        self.__presence_penalty = round(v, 2)
-
-    def __saveAsLog(self):
-        filename = QFileDialog.getSaveFileName(self, 'Save', os.path.expanduser('~'), 'Text File (*.txt)')
-        if filename[0]:
-            filename = filename[0]
-            file_extension = os.path.splitext(filename)[-1]
-            if file_extension == '.txt':
-                with open(filename, 'w') as f:
-                    f.write(self.__browser.getAllText())
-                os.startfile(os.path.dirname(filename))
-
     def __stackToggle(self, f):
         if f:
             self.setWindowFlags(self.windowFlags() | Qt.WindowStaysOnTopHint)
         else:
             self.setWindowFlags(self.windowFlags() & ~Qt.WindowStaysOnTopHint)
         self.show()
 
@@ -421,52 +501,48 @@
         if reply == 16384:
             e.accept()
         # No
         elif reply == 65536:
             app.quit()
         return super().closeEvent(e)
 
-    def __findData(self):
-        filename = QFileDialog.getOpenFileName(self, 'Open', '', 'JSONL Files (*.jsonl)')
+    def __changeConv(self, item: QListWidgetItem):
+        # If a 'change' event occurs but there are no items, it should mean that list is empty
+        # so reset conv_history.json
+        if item:
+            id = item.data(Qt.UserRole)
+            conv = self.__db.selectConvUnit(id)
+            self.__browser.replaceConv(id, conv)
+        else:
+            self.__browser.resetChatWidget(0)
+
+    def __addConv(self):
+        self.__db.insertConv('New Chat')
+        cur_id = self.__db.getCursor().lastrowid
+        self.__browser.resetChatWidget(cur_id)
+        self.__leftSideBarWidget.addToList(cur_id)
+        self.__lineEdit.setFocus()
+
+    def __updateConv(self, id, title=None):
+        if title:
+            self.__db.updateConv(id, title)
+
+    def __deleteConv(self, id_lst):
+        for id in id_lst:
+            self.__db.deleteConv(id)
+
+    def __export(self, ids):
+        filename = QFileDialog.getSaveFileName(self, 'Save', os.path.expanduser('~'), 'SQLite DB file (*.db)')
         if filename[0]:
             filename = filename[0]
-            self.__findDataLineEdit.setText(filename)
-            self.__fineTuningBtn.setEnabled(True)
-            
-
-    def __fineTuning(self):
-        if platform.system() == 'Windows':
-            subprocess.Popen('cmd.exe', creationflags=subprocess.CREATE_NEW_CONSOLE)
-        elif platform.system() in ['Darwin', 'Linux']:
-            subprocess.Popen('bash', creationflags=subprocess.CREATE_NEW_CONSOLE)
-
-        # https://platform.openai.com/docs/guides/fine-tuning/cli-data-preparation-tool
-        # validating & giving suggestions and reformat the data
-        # subprocess.run('openai tools fine_tunes.prepare_data -f data.jsonl')
-
-        # https://platform.openai.com/docs/guides/fine-tuning/create-a-fine-tuned-model
-        # create a fine-tuned model
-        # subprocess.run('openai api fine_tunes.create -t [TRAIN_FILE_ID_OR_PATH] -m [BASE_MODEL]')
-
-        # run this when event stream is interrupted for any reason
-        # subprocess.run('openai api fine_tunes.follow -i [YOUR_FINE_TUNE_JOB_ID]')
-        # you can see the job done when it is finished
-        # https://platform.openai.com/account/usage
-        # https://platform.openai.com/playground
-
-        # list the jobs
-        # subprocess.run('openai api fine_tunes.list')
-
-        # get the status of certain job. The resulting object includes
-        # job status (which can be one of pending, running, succeeded, or failed)
-        # and other information
-        # subprocess.run('openai api fine_tunes.get -i [YOUR_FINE_TUNE_JOB_ID]')
+            self.__db.export(ids, filename)
 
-        # cancel the job
-        # subprocess.run('openai api fine_tunes.cancel -i [YOUR_FINE_TUNE_JOB_ID]')
+    def __updateConvUnit(self, id, user_f, conv_unit=None):
+        if conv_unit:
+            self.__db.insertConvUnit(id, user_f, conv_unit)
 
 
 if __name__ == "__main__":
     import sys
 
     app = QApplication(sys.argv)
     app.setQuitOnLastWindowClosed(False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyqt-openai-0.0.171/pyqt_openai/notifier.py` & `pyqt-openai-0.1.2/pyqt_openai/notifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from PyQt5.QtGui import QFont, QIcon
-from PyQt5.QtWidgets import QWidget, QLabel, QHBoxLayout, QVBoxLayout, QDesktopWidget, QSizePolicy, qApp, QPushButton, \
+from qtpy.QtGui import QFont, QIcon
+from qtpy.QtWidgets import QWidget, QLabel, QHBoxLayout, QVBoxLayout, QDesktopWidget, QSizePolicy, qApp, QPushButton, \
     QApplication
-from PyQt5.QtCore import Qt, QPoint, QTimer, pyqtSignal, QPropertyAnimation
+from qtpy.QtCore import Qt, QPoint, Signal, QTimer, QPropertyAnimation
 
 
 class NotifierWidget(QWidget):
-    doubleClicked = pyqtSignal()
+    doubleClicked = Signal()
 
     def __init__(self, informative_text='', detailed_text=''):
         super().__init__()
         self.__timerVal = 5000
         self.__initUi(informative_text, detailed_text)
 
     def __initUi(self, informative_text='', detailed_text=''):
```

### Comparing `pyqt-openai-0.0.171/setup.py` & `pyqt-openai-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.0.171',
+    version='0.1.2',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
-    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg']},
+    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'help.svg', 'sidebar.svg', 'prompt.svg', 'download.svg', 'stackontop.svg', 'add.svg', 'delete.svg', 'setting.svg', 'search.svg']},
     description='PyQt OpenAI example',
     url='https://github.com/yjg30737/pyqt-openai.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
-        'PyQt5',
+        'PyQt5>=5.14',
+        'PySide6',
+        'qtpy',
         'aiohttp',
         'openai',
+        'pyperclip'
     ]
 )
```

