# Comparing `tmp/aij-webcam-1.0.8.tar.gz` & `tmp/aij-webcam-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.0.8.tar", last modified: Thu May  4 10:27:27 2023, max compression
+gzip compressed data, was "aij-webcam-1.0.9.tar", last modified: Thu May  4 10:33:33 2023, max compression
```

## Comparing `aij-webcam-1.0.8.tar` & `aij-webcam-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.8/README.md
--rw-rw-rw-   0        0        0     6452 2023-05-04 10:27:18.000000 aij-webcam-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 10:27:28.000000 aij-webcam-1.0.8/src/webcam/
--rw-rw-rw-   0        0        0    11775 2023-05-04 10:26:14.000000 aij-webcam-1.0.8/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.9/README.md
+-rw-rw-rw-   0        0        0     6452 2023-05-04 10:33:22.000000 aij-webcam-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      161 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:33:34.000000 aij-webcam-1.0.9/src/webcam/
+-rw-rw-rw-   0        0        0    12217 2023-05-04 10:33:32.000000 aij-webcam-1.0.9/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.0.8/LICENSE.txt` & `aij-webcam-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.8/PKG-INFO` & `aij-webcam-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.8/README.md` & `aij-webcam-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.8/pyproject.toml` & `aij-webcam-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.8"
+version = "1.0.9"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.0.8/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.0.9/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.8/src/webcam/__init__.py` & `aij-webcam-1.0.9/src/webcam/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,16 +110,25 @@
 
 def generate_audio_from_news():
     """
     Convert text to speech and play it
     """
     # initialize tts, create mp3 and play
     tts = gTTS(text=titles, lang='en')
-    # save the audio file
-    tts.save('news/news.mp3')
+    # get the user profile path
+    user_profile = os.environ['USERPROFILE']
+    _sep = os.path.sep
+    # create a folder named 'audio' to store audio files if not exists
+    audio_home = user_profile + _sep + '.aij' + _sep + 'news' + _sep + 'audio'
+    if not os.path.exists(audio_home):
+        os.mkdir(audio_home)
+
+    # save the audio file if not exists
+    if not os.path.exists(audio_home + _sep + 'news.mp3'):
+        tts.save('news/news.mp3')
     # print the text
     print(
         'The news is: \n' + titles + '\n\n' +
         'The audio file has been saved to news/news.mp3\n\n'
     )
 
 
@@ -166,14 +175,17 @@
 def forward_news_from_audio():
     """
     Forward the news
     """
     mixer.music.forward()
 
 def main():
+    """
+    Main function
+    """
 
     thread_generate_audio_from_news = threading.Thread(target=generate_audio_from_news)
     thread_play_news_from_audio = threading.Thread(target=play_news_from_audio)
 
     # make sure the audio file is generated before playing it
     thread_generate_audio_from_news.start()
     thread_generate_audio_from_news.join()
```

