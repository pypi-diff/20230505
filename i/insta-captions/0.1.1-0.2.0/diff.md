# Comparing `tmp/insta-captions-0.1.1.tar.gz` & `tmp/insta-captions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/insta-captions-0.1.1.tar", last modified: Mon Mar 27 02:57:11 2023, max compression
+gzip compressed data, was "dist/insta-captions-0.2.0.tar", last modified: Fri May  5 04:40:17 2023, max compression
```

## Comparing `insta-captions-0.1.1.tar` & `insta-captions-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-03-27 02:57:11.000000 insta-captions-0.1.1/
--rw-r--r--   0 daveeed    (501) staff       (20)      291 2023-03-27 02:51:34.000000 insta-captions-0.1.1/.bumpversion.cfg
--rw-r--r--   0 daveeed    (501) staff       (20)     1071 2023-02-19 20:05:36.000000 insta-captions-0.1.1/LICENSE
--rw-r--r--   0 daveeed    (501) staff       (20)      348 2023-03-11 03:04:37.000000 insta-captions-0.1.1/MANIFEST.in
--rw-r--r--   0 daveeed    (501) staff       (20)     1560 2023-03-11 03:04:37.000000 insta-captions-0.1.1/Makefile
--rw-r--r--   0 daveeed    (501) staff       (20)     5096 2023-03-27 02:57:11.000000 insta-captions-0.1.1/PKG-INFO
--rw-r--r--   0 daveeed    (501) staff       (20)     3116 2023-03-27 02:37:13.000000 insta-captions-0.1.1/README.md
--rw-r--r--   0 daveeed    (501) staff       (20)     2101 2023-03-27 02:51:34.000000 insta-captions-0.1.1/pyproject.toml
--rw-r--r--   0 daveeed    (501) staff       (20)       38 2023-03-27 02:57:11.000000 insta-captions-0.1.1/setup.cfg
--rw-r--r--   0 daveeed    (501) staff       (20)       38 2023-03-11 03:04:44.000000 insta-captions-0.1.1/setup.py
-drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/
--rw-r--r--   0 daveeed    (501) staff       (20)      100 2023-03-11 03:04:44.000000 insta-captions-0.1.1/src/__init__.py
--rw-r--r--   0 daveeed    (501) staff       (20)       22 2023-03-27 02:51:34.000000 insta-captions-0.1.1/src/_version.py
-drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/insta_captions.egg-info/
--rw-r--r--   0 daveeed    (501) staff       (20)     5096 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/insta_captions.egg-info/PKG-INFO
--rw-r--r--   0 daveeed    (501) staff       (20)      369 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/insta_captions.egg-info/SOURCES.txt
--rw-r--r--   0 daveeed    (501) staff       (20)        1 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/insta_captions.egg-info/dependency_links.txt
--rw-r--r--   0 daveeed    (501) staff       (20)      154 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/insta_captions.egg-info/requires.txt
--rw-r--r--   0 daveeed    (501) staff       (20)       32 2023-03-27 02:57:11.000000 insta-captions-0.1.1/src/insta_captions.egg-info/top_level.txt
--rw-r--r--   0 daveeed    (501) staff       (20)     1948 2023-03-11 03:04:44.000000 insta-captions-0.1.1/src/transcription.py
-drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-03-27 02:57:11.000000 insta-captions-0.1.1/tests/
--rw-r--r--   0 daveeed    (501) staff       (20)     3372 2023-03-11 03:04:44.000000 insta-captions-0.1.1/tests/test_transcription.py
+drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-05-05 04:40:17.000000 insta-captions-0.2.0/
+-rw-r--r--   0 daveeed    (501) staff       (20)      291 2023-05-05 04:07:36.000000 insta-captions-0.2.0/.bumpversion.cfg
+-rw-r--r--   0 daveeed    (501) staff       (20)     1444 2023-03-27 02:37:13.000000 insta-captions-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 daveeed    (501) staff       (20)     1071 2023-02-19 20:05:36.000000 insta-captions-0.2.0/LICENSE
+-rw-r--r--   0 daveeed    (501) staff       (20)      348 2023-03-11 03:04:37.000000 insta-captions-0.2.0/MANIFEST.in
+-rw-r--r--   0 daveeed    (501) staff       (20)     1560 2023-03-11 03:04:37.000000 insta-captions-0.2.0/Makefile
+-rw-r--r--   0 daveeed    (501) staff       (20)     5194 2023-05-05 04:40:17.000000 insta-captions-0.2.0/PKG-INFO
+-rw-r--r--   0 daveeed    (501) staff       (20)     3214 2023-05-04 19:58:14.000000 insta-captions-0.2.0/README.md
+drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-05-05 04:40:17.000000 insta-captions-0.2.0/docs/
+-rw-r--r--   0 daveeed    (501) staff       (20)      634 2023-04-05 04:00:06.000000 insta-captions-0.2.0/docs/Makefile
+-rw-r--r--   0 daveeed    (501) staff       (20)     1388 2023-04-05 04:00:06.000000 insta-captions-0.2.0/docs/conf.py
+-rw-r--r--   0 daveeed    (501) staff       (20)     1447 2023-04-05 04:00:06.000000 insta-captions-0.2.0/docs/index.rst
+-rw-r--r--   0 daveeed    (501) staff       (20)      800 2023-04-05 04:00:06.000000 insta-captions-0.2.0/docs/make.bat
+-rw-r--r--   0 daveeed    (501) staff       (20)     2131 2023-05-05 04:07:36.000000 insta-captions-0.2.0/pyproject.toml
+-rw-r--r--   0 daveeed    (501) staff       (20)       38 2023-05-05 04:40:17.000000 insta-captions-0.2.0/setup.cfg
+-rw-r--r--   0 daveeed    (501) staff       (20)       38 2023-03-11 03:04:44.000000 insta-captions-0.2.0/setup.py
+drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/
+-rw-r--r--   0 daveeed    (501) staff       (20)      113 2023-05-05 04:07:36.000000 insta-captions-0.2.0/src/__init__.py
+-rw-r--r--   0 daveeed    (501) staff       (20)       22 2023-05-05 04:07:36.000000 insta-captions-0.2.0/src/_version.py
+drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/insta_captions.egg-info/
+-rw-r--r--   0 daveeed    (501) staff       (20)     5194 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/insta_captions.egg-info/PKG-INFO
+-rw-r--r--   0 daveeed    (501) staff       (20)      550 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/insta_captions.egg-info/SOURCES.txt
+-rw-r--r--   0 daveeed    (501) staff       (20)        1 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/insta_captions.egg-info/dependency_links.txt
+-rw-r--r--   0 daveeed    (501) staff       (20)      177 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/insta_captions.egg-info/requires.txt
+-rw-r--r--   0 daveeed    (501) staff       (20)       46 2023-05-05 04:40:17.000000 insta-captions-0.2.0/src/insta_captions.egg-info/top_level.txt
+-rw-r--r--   0 daveeed    (501) staff       (20)     1966 2023-05-05 04:07:36.000000 insta-captions-0.2.0/src/instacaptions.py
+-rw-r--r--   0 daveeed    (501) staff       (20)     3399 2023-04-05 04:00:06.000000 insta-captions-0.2.0/src/transcription.py
+drwxr-xr-x   0 daveeed    (501) staff       (20)        0 2023-05-05 04:40:17.000000 insta-captions-0.2.0/tests/
+-rw-r--r--   0 daveeed    (501) staff       (20)        0 2023-03-11 03:04:44.000000 insta-captions-0.2.0/tests/__init__.py
+-rw-r--r--   0 daveeed    (501) staff       (20)      986 2023-05-05 04:07:36.000000 insta-captions-0.2.0/tests/test_instacaptions.py
+-rw-r--r--   0 daveeed    (501) staff       (20)     2021 2023-04-05 04:00:06.000000 insta-captions-0.2.0/tests/test_transcription.py
+-rw-r--r--   0 daveeed    (501) staff       (20)       45 2023-03-11 03:04:44.000000 insta-captions-0.2.0/tests/testempty.wav
+-rw-r--r--   0 daveeed    (501) staff       (20)       44 2023-03-11 03:04:44.000000 insta-captions-0.2.0/tests/testempty16.wav
```

### Comparing `insta-captions-0.1.1/LICENSE` & `insta-captions-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insta-captions-0.1.1/Makefile` & `insta-captions-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `insta-captions-0.1.1/PKG-INFO` & `insta-captions-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insta-captions
-Version: 0.1.1
+Version: 0.2.0
 Summary: insta-captions is a tool that will allow for the instant transcription and translation of audio files to and from different languages.
 Author-email: davidcendejas <david.cendejas@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 David Cendejas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,17 +40,21 @@
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ![issues](https://img.shields.io/github/issues/DavidCendejas/insta-captions)
 
 [![Build Status](https://github.com/DavidCendejas/insta-captions/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/DavidCendejas/insta-captions/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/DavidCendejas/insta-captions/branch/main/graph/badge.svg?token=Z2HN4RCJGZ)](https://codecov.io/gh/DavidCendejas/insta-captions)
+[![PyPI](https://img.shields.io/pypi/v/insta-captions)](https://pypi.org/project/insta-captions/)
+[![Documentation Status](https://readthedocs.org/projects/insta-captions/badge/?version=latest)](https://insta-captions.readthedocs.io/en/latest/?badge=latest)
 
 insta-captions is a tool that will allow for the instant transcription and translation of audio files to and from different languages.
 
+View more on our [documentation page](https://insta-captions.readthedocs.io/en/latest/)
+
 ## Installation
 
 "pip install insta-captions"
 
 ## Overview
 
 `insta-captions` is a library that deals with the conversion of audio into "captions". I have been learning Mandarin, my third language. Part of my learning process, as well as maintenance for Spanish, is to watch videos, shows, and movies in the language I am trying to deepen. Sometimes, however, I need to watch content in English but want to read it in another language, and there is no easy way to do this if captions are not provided by the video maker, which is the crux of this issue.
@@ -62,20 +66,24 @@
 
 ## Installation and Running
 
 insta-captions transcriptions are possible with [DeepSpeech](https://github.com/mozilla/DeepSpeech). For installation of DeepSpeech, refer to their [documentation](https://deepspeech.readthedocs.io/en/r0.9/?badge=latest). I use their [pre-trained models](https://github.com/mozilla/DeepSpeech/releases/tag/v0.9.3) on english and mandarin. These models are included in this repository via Git LFS due to large file size.
 
 Additional libraries used are numpy to convert the buffer of the .wav files into int16 numpy arrays as this is what DeepSpeech speech-to-text accepts.
 
-## How to Use
+## Example Usage
+Using a .wav file from the data folder,
+```
+    from insta-captions import Transcribe as Trans
+    t = Trans()
+    print(t.transcribe('./8455-210777-0068.wav'))
+    >>> [('./2830-3980-0043.wav', 'experience proves this')]
+```
+
 
-To get a transcription of an audio file, we have the function *transcribe(wav_files, language)* .
-- *wav_files* is a list of strings that contain the paths to the .wav files that you want the function to transcribe. These files must have a sample rate of 16kHz.
-- *language* is a string indicating the language that the audio file is in. Currently the only supported languages are "english" and "mandarin".
-- This returns a list of strings, one transcription for each file sent.
 
 ## make commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make format`: autoformat this library using `black`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make test`: run automated tests with `unittest`
```

### Comparing `insta-captions-0.1.1/README.md` & `insta-captions-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ![issues](https://img.shields.io/github/issues/DavidCendejas/insta-captions)
 
 [![Build Status](https://github.com/DavidCendejas/insta-captions/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/DavidCendejas/insta-captions/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/DavidCendejas/insta-captions/branch/main/graph/badge.svg?token=Z2HN4RCJGZ)](https://codecov.io/gh/DavidCendejas/insta-captions)
+[![PyPI](https://img.shields.io/pypi/v/insta-captions)](https://pypi.org/project/insta-captions/)
+[![Documentation Status](https://readthedocs.org/projects/insta-captions/badge/?version=latest)](https://insta-captions.readthedocs.io/en/latest/?badge=latest)
 
 insta-captions is a tool that will allow for the instant transcription and translation of audio files to and from different languages.
 
+View more on our [documentation page](https://insta-captions.readthedocs.io/en/latest/)
+
 ## Installation
 
 "pip install insta-captions"
 
 ## Overview
 
 `insta-captions` is a library that deals with the conversion of audio into "captions". I have been learning Mandarin, my third language. Part of my learning process, as well as maintenance for Spanish, is to watch videos, shows, and movies in the language I am trying to deepen. Sometimes, however, I need to watch content in English but want to read it in another language, and there is no easy way to do this if captions are not provided by the video maker, which is the crux of this issue.
@@ -24,20 +28,24 @@
 
 ## Installation and Running
 
 insta-captions transcriptions are possible with [DeepSpeech](https://github.com/mozilla/DeepSpeech). For installation of DeepSpeech, refer to their [documentation](https://deepspeech.readthedocs.io/en/r0.9/?badge=latest). I use their [pre-trained models](https://github.com/mozilla/DeepSpeech/releases/tag/v0.9.3) on english and mandarin. These models are included in this repository via Git LFS due to large file size.
 
 Additional libraries used are numpy to convert the buffer of the .wav files into int16 numpy arrays as this is what DeepSpeech speech-to-text accepts.
 
-## How to Use
+## Example Usage
+Using a .wav file from the data folder,
+```
+    from insta-captions import Transcribe as Trans
+    t = Trans()
+    print(t.transcribe('./8455-210777-0068.wav'))
+    >>> [('./2830-3980-0043.wav', 'experience proves this')]
+```
+
 
-To get a transcription of an audio file, we have the function *transcribe(wav_files, language)* .
-- *wav_files* is a list of strings that contain the paths to the .wav files that you want the function to transcribe. These files must have a sample rate of 16kHz.
-- *language* is a string indicating the language that the audio file is in. Currently the only supported languages are "english" and "mandarin".
-- This returns a list of strings, one transcription for each file sent.
 
 ## make commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make format`: autoformat this library using `black`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make test`: run automated tests with `unittest`
```

### Comparing `insta-captions-0.1.1/pyproject.toml` & `insta-captions-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "insta-captions"
 authors = [{name = "davidcendejas", email = "david.cendejas@columbia.edu"}]
 description="insta-captions is a tool that will allow for the instant transcription and translation of audio files to and from different languages."
 readme = "README.md"
-version = "0.1.1"   
+version = "0.2.0"   
 requires-python = ">=3.7"
 
 dependencies = [
     "deepspeech>=0.9.3",
+    "googletrans==4.0.0-rc1",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
```

### Comparing `insta-captions-0.1.1/src/insta_captions.egg-info/PKG-INFO` & `insta-captions-0.2.0/src/insta_captions.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insta-captions
-Version: 0.1.1
+Version: 0.2.0
 Summary: insta-captions is a tool that will allow for the instant transcription and translation of audio files to and from different languages.
 Author-email: davidcendejas <david.cendejas@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 David Cendejas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,17 +40,21 @@
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ![issues](https://img.shields.io/github/issues/DavidCendejas/insta-captions)
 
 [![Build Status](https://github.com/DavidCendejas/insta-captions/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/DavidCendejas/insta-captions/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/DavidCendejas/insta-captions/branch/main/graph/badge.svg?token=Z2HN4RCJGZ)](https://codecov.io/gh/DavidCendejas/insta-captions)
+[![PyPI](https://img.shields.io/pypi/v/insta-captions)](https://pypi.org/project/insta-captions/)
+[![Documentation Status](https://readthedocs.org/projects/insta-captions/badge/?version=latest)](https://insta-captions.readthedocs.io/en/latest/?badge=latest)
 
 insta-captions is a tool that will allow for the instant transcription and translation of audio files to and from different languages.
 
+View more on our [documentation page](https://insta-captions.readthedocs.io/en/latest/)
+
 ## Installation
 
 "pip install insta-captions"
 
 ## Overview
 
 `insta-captions` is a library that deals with the conversion of audio into "captions". I have been learning Mandarin, my third language. Part of my learning process, as well as maintenance for Spanish, is to watch videos, shows, and movies in the language I am trying to deepen. Sometimes, however, I need to watch content in English but want to read it in another language, and there is no easy way to do this if captions are not provided by the video maker, which is the crux of this issue.
@@ -62,20 +66,24 @@
 
 ## Installation and Running
 
 insta-captions transcriptions are possible with [DeepSpeech](https://github.com/mozilla/DeepSpeech). For installation of DeepSpeech, refer to their [documentation](https://deepspeech.readthedocs.io/en/r0.9/?badge=latest). I use their [pre-trained models](https://github.com/mozilla/DeepSpeech/releases/tag/v0.9.3) on english and mandarin. These models are included in this repository via Git LFS due to large file size.
 
 Additional libraries used are numpy to convert the buffer of the .wav files into int16 numpy arrays as this is what DeepSpeech speech-to-text accepts.
 
-## How to Use
+## Example Usage
+Using a .wav file from the data folder,
+```
+    from insta-captions import Transcribe as Trans
+    t = Trans()
+    print(t.transcribe('./8455-210777-0068.wav'))
+    >>> [('./2830-3980-0043.wav', 'experience proves this')]
+```
+
 
-To get a transcription of an audio file, we have the function *transcribe(wav_files, language)* .
-- *wav_files* is a list of strings that contain the paths to the .wav files that you want the function to transcribe. These files must have a sample rate of 16kHz.
-- *language* is a string indicating the language that the audio file is in. Currently the only supported languages are "english" and "mandarin".
-- This returns a list of strings, one transcription for each file sent.
 
 ## make commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make format`: autoformat this library using `black`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make test`: run automated tests with `unittest`
```

### Comparing `insta-captions-0.1.1/src/transcription.py` & `insta-captions-0.2.0/src/transcription.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,93 @@
 import numpy as np
 import wave
 from deepspeech import Model as dsm
 
-models = {
-    "english": "data/language_models/deepspeech-0.9.3-models.pbmm",
-    "mandarin": "data/language_models/deepspeech-0.9.3-models-zh-CN.pbmm",
-}
-
-lm = {
-    "english": "data/language_models/deepspeech-0.9.3-models.scorer",
-    "mandarin": "data/language_models/deepspeech-0.9.3-models-zh-CN.scorer",
-}
-
-alphabeta = {
-    "english": {"alpha": 0.931289039105002, "beta": 1.1834137581510284},
-    "mandarin": {"alpha": 0.6940122363709647, "beta": 4.777924224113021},
-}
-
-beam_width = 100
-
-
-def read_from_wav(filename):
-    with wave.open(filename, "rb") as w:
-        rate = w.getframerate()
-        frames = w.getnframes()
-        buffer = w.readframes(frames)
-    return rate, buffer
-
-
-def wav_to_text(model, filename):
-    rate, buffer = read_from_wav(filename)
-    wav_data = np.frombuffer(buffer, dtype=np.int16)
-    return model.stt(wav_data)
-
-
-# wav_files is a list of .wav files
-def transcribe(wav_files, language="english"):
-    if len(wav_files) == 0:
-        return []
-    if language not in models:
-        return []  # THIS SHOULD RAISE AN EXCEPTION
-    else:
-        # Eventually when incorporating SpeechRecognition library to be
-        # able to detect the language of a file, the model parameters should
-        # be set for each distinct .wav file each loop. Language parameter
-        # would then be refactored out
-
-        model = dsm(models[language])
-        model.enableExternalScorer(lm[language])
-        model.setScorerAlphaBeta(alphabeta[language]["alpha"], alphabeta[language]["beta"])
-        model.setBeamWidth(beam_width)
 
-        transcriptions = []
-
-        for audiofile in wav_files:
+class Transcribe:
+    _models = {
+        "english": "data/language_models/deepspeech-0.9.3-models.pbmm",
+        "mandarin": "data/language_models/deepspeech-0.9.3-models-zh-CN.pbmm",
+    }
+
+    _lm = {
+        "english": "data/language_models/deepspeech-0.9.3-models.scorer",
+        "mandarin": "data/language_models/deepspeech-0.9.3-models-zh-CN.scorer",
+    }
+
+    _alphabeta = {
+        "english": {"alpha": 0.931289039105002, "beta": 1.1834137581510284},
+        "mandarin": {"alpha": 0.6940122363709647, "beta": 4.777924224113021},
+    }
+
+    _beam_width = 100
+
+    __model = None
+
+    __transcriptions = []
+
+    def __init__(self, language="english"):
+        """Constructor
+
+        :param language: What language should this instance transcribe in
+          must be "english" or "mandarin", defaults to "english"
+        :type language: str, optional
+        :raises ValueError: If "english" or "mandarin" is not set, a ValueError is raised
+        """
+        if not (language == "english" or language == "mandarin"):
+            raise ValueError("language param must be either \'english\' or \'mandarin\' .")
+
+        self.__model = dsm(self._models[language])
+        self.__model.enableExternalScorer(self._lm[language])
+        self.__model.setScorerAlphaBeta(self._alphabeta[language]["alpha"], self._alphabeta[language]["beta"])
+        self.__model.setBeamWidth(self._beam_width)
+
+    def read_from_wav(self, filename):
+        with wave.open(filename, "rb") as w:
+            rate = w.getframerate()
+            frames = w.getnframes()
+            buffer = w.readframes(frames)
+        return rate, buffer
+
+    def wav_to_text(self, model, filename):
+        rate, buffer = self.read_from_wav(filename)
+        wav_data = np.frombuffer(buffer, dtype=np.int16)
+        return model.stt(wav_data)
+
+    def get_transcriptions(self):
+        """A getter function that returns a history of transcriptions from the transcribe() function
+
+        :return: A list of transcriptions from each time a Transcribe instance calls transcribe()
+        :rtype: list
+        """
+        return self.__transcriptions
+
+    def get_model(self):
+        """A getter function that gets the DeepSpeech model created in the constructor.
+
+        :return: DeepSpeech model object
+        :rtype: :class: `deepspeech.Model`
+        """
+        return self.__model
+
+    def transcribe(self, wav_files):
+        """Given a list of .wav filepaths, returns a list of tuples where each tuple is (filepath, transcription).
+        Both filepath and transcription are strings.
+
+        :param wav_files: A list of filepaths to .wav files
+        :type wav_files: List of strings (filepaths)
+        :return: A list of tuples where value 1 is the filepath and value 2 is the transcribed string
+        :rtype: list of tuples
+        """
+        if len(wav_files) == 0:
+            return []
+        else:
             try:
-                transcription = wav_to_text(model, audiofile)
-                transcriptions.append((audiofile, transcription))
+                transcriptions = []
+                for audiofile in wav_files:
+                    transcription = self.wav_to_text(self.__model, audiofile)
+                    transcriptions.append((audiofile, transcription))
             except FileNotFoundError:
                 print("Invalid File")
-
-        return transcriptions
+            else:
+                self.__transcriptions.append(transcriptions)
+                return transcriptions
```

