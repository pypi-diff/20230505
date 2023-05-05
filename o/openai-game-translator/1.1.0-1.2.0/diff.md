# Comparing `tmp/openai-game-translator-1.1.0.tar.gz` & `tmp/openai-game-translator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-game-translator-1.1.0.tar", last modified: Fri Apr  7 05:23:21 2023, max compression
+gzip compressed data, was "openai-game-translator-1.2.0.tar", last modified: Fri May  5 04:13:29 2023, max compression
```

## Comparing `openai-game-translator-1.1.0.tar` & `openai-game-translator-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,42 @@
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.990534 openai-game-translator-1.1.0/
--rw-r--r--   0 arika      (501) staff       (20)      304 2023-04-07 04:55:20.000000 openai-game-translator-1.1.0/.bumpversion.cfg
--rw-r--r--   0 arika      (501) staff       (20)      791 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 arika      (501) staff       (20)    11357 2023-03-21 20:15:17.000000 openai-game-translator-1.1.0/LICENSE
--rw-r--r--   0 arika      (501) staff       (20)      462 2023-04-07 05:17:48.000000 openai-game-translator-1.1.0/MANIFEST.in
--rw-r--r--   0 arika      (501) staff       (20)     2133 2023-04-07 05:12:54.000000 openai-game-translator-1.1.0/Makefile
--rw-r--r--   0 arika      (501) staff       (20)    15299 2023-04-07 05:23:21.990319 openai-game-translator-1.1.0/PKG-INFO
--rw-r--r--   0 arika      (501) staff       (20)     1695 2023-04-07 04:15:40.000000 openai-game-translator-1.1.0/README.md
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.985398 openai-game-translator-1.1.0/game_translator/
--rw-r--r--   0 arika      (501) staff       (20)      295 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)       42 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/__main__.py
--rw-r--r--   0 arika      (501) staff       (20)       22 2023-04-07 04:55:20.000000 openai-game-translator-1.1.0/game_translator/_version.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.986058 openai-game-translator-1.1.0/game_translator/audio/
--rw-r--r--   0 arika      (501) staff       (20)       29 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/audio/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)   160044 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/game_translator/audio/audio_sample_little.wav
--rw-r--r--   0 arika      (501) staff       (20)     2557 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/audio/record.py
--rw-r--r--   0 arika      (501) staff       (20)   282668 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/audio/test.wav
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.986809 openai-game-translator-1.1.0/game_translator/aws_streaming_transcription/
--rw-r--r--   0 arika      (501) staff       (20)        0 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/game_translator/aws_streaming_transcription/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)     2630 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/aws_streaming_transcription/live_stream.py
--rw-r--r--   0 arika      (501) staff       (20)     3445 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/aws_streaming_transcription/prerecorded_stream.py
--rw-r--r--   0 arika      (501) staff       (20)     4724 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/game_translator.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.987146 openai-game-translator-1.1.0/game_translator/openai_translation/
--rw-r--r--   0 arika      (501) staff       (20)       37 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/openai_translation/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)      688 2023-04-07 04:45:17.000000 openai-game-translator-1.1.0/game_translator/openai_translation/chat.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.987639 openai-game-translator-1.1.0/game_translator/xunfei_speed_transcription/
--rw-r--r--   0 arika      (501) staff       (20)       70 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/game_translator/xunfei_speed_transcription/__init__.py
--rw-r--r--   0 arika      (501) staff       (20)     7672 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/xunfei_speed_transcription/ost_fast.py
--rw-r--r--   0 arika      (501) staff       (20)     7608 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/game_translator/xunfei_speed_transcription/seve_file.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.988772 openai-game-translator-1.1.0/openai_game_translator.egg-info/
--rw-r--r--   0 arika      (501) staff       (20)    15299 2023-04-07 05:23:21.000000 openai-game-translator-1.1.0/openai_game_translator.egg-info/PKG-INFO
--rw-r--r--   0 arika      (501) staff       (20)     1246 2023-04-07 05:23:21.000000 openai-game-translator-1.1.0/openai_game_translator.egg-info/SOURCES.txt
--rw-r--r--   0 arika      (501) staff       (20)        1 2023-04-07 05:23:21.000000 openai-game-translator-1.1.0/openai_game_translator.egg-info/dependency_links.txt
--rw-r--r--   0 arika      (501) staff       (20)       67 2023-04-07 05:23:21.000000 openai-game-translator-1.1.0/openai_game_translator.egg-info/entry_points.txt
--rw-r--r--   0 arika      (501) staff       (20)      261 2023-04-07 05:23:21.000000 openai-game-translator-1.1.0/openai_game_translator.egg-info/requires.txt
--rw-r--r--   0 arika      (501) staff       (20)       16 2023-04-07 05:23:21.000000 openai-game-translator-1.1.0/openai_game_translator.egg-info/top_level.txt
--rw-r--r--   0 arika      (501) staff       (20)     1242 2023-04-07 05:13:40.000000 openai-game-translator-1.1.0/pyproject.toml
--rw-r--r--   0 arika      (501) staff       (20)       38 2023-04-07 05:23:21.990584 openai-game-translator-1.1.0/setup.cfg
--rw-r--r--   0 arika      (501) staff       (20)       38 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/setup.py
-drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-04-07 05:23:21.990035 openai-game-translator-1.1.0/tests/
--rw-r--r--   0 arika      (501) staff       (20)      179 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/.coveragerc
--rw-r--r--   0 arika      (501) staff       (20)     2059 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/test_all.py
--rw-r--r--   0 arika      (501) staff       (20)     1675 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/test_aws_live.py
--rw-r--r--   0 arika      (501) staff       (20)     1798 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/test_aws_pre.py
--rw-r--r--   0 arika      (501) staff       (20)     2442 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/test_game_translator.py
--rw-r--r--   0 arika      (501) staff       (20)     1201 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/test_openai.py
--rw-r--r--   0 arika      (501) staff       (20)     1094 2023-04-07 04:06:17.000000 openai-game-translator-1.1.0/tests/test_record.py
--rw-r--r--   0 arika      (501) staff       (20)     1229 2023-04-05 01:22:22.000000 openai-game-translator-1.1.0/tests/test_xunfei.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.626423 openai-game-translator-1.2.0/
+-rw-r--r--   0 arika      (501) staff       (20)    11357 2023-03-21 20:15:17.000000 openai-game-translator-1.2.0/LICENSE
+-rw-r--r--   0 arika      (501) staff       (20)    17867 2023-05-05 04:13:29.626189 openai-game-translator-1.2.0/PKG-INFO
+-rw-r--r--   0 arika      (501) staff       (20)     4263 2023-05-05 01:27:26.000000 openai-game-translator-1.2.0/README.md
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.620702 openai-game-translator-1.2.0/game_translator/
+-rw-r--r--   0 arika      (501) staff       (20)      295 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)       42 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/__main__.py
+-rw-r--r--   0 arika      (501) staff       (20)       22 2023-05-05 03:44:24.000000 openai-game-translator-1.2.0/game_translator/_version.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.620991 openai-game-translator-1.2.0/game_translator/audio/
+-rw-r--r--   0 arika      (501) staff       (20)       29 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/audio/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)     3112 2023-05-04 18:51:36.000000 openai-game-translator-1.2.0/game_translator/audio/record.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.621552 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/
+-rw-r--r--   0 arika      (501) staff       (20)        0 2023-04-05 01:22:22.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)     2406 2023-05-05 01:25:40.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/live_stream.py
+-rw-r--r--   0 arika      (501) staff       (20)     2811 2023-05-05 01:25:40.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/prerecorded_stream.py
+-rw-r--r--   0 arika      (501) staff       (20)     1717 2023-05-05 01:25:40.000000 openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/settings.py
+-rw-r--r--   0 arika      (501) staff       (20)     9775 2023-05-05 04:08:39.000000 openai-game-translator-1.2.0/game_translator/game_translator.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.621861 openai-game-translator-1.2.0/game_translator/openai_translation/
+-rw-r--r--   0 arika      (501) staff       (20)       37 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/game_translator/openai_translation/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)      681 2023-05-03 19:14:25.000000 openai-game-translator-1.2.0/game_translator/openai_translation/chat.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.622320 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/
+-rw-r--r--   0 arika      (501) staff       (20)       70 2023-04-05 01:22:22.000000 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/__init__.py
+-rw-r--r--   0 arika      (501) staff       (20)     7697 2023-05-03 21:28:32.000000 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/ost_fast.py
+-rw-r--r--   0 arika      (501) staff       (20)     7608 2023-05-03 19:13:14.000000 openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/seve_file.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.623472 openai-game-translator-1.2.0/openai_game_translator.egg-info/
+-rw-r--r--   0 arika      (501) staff       (20)    17867 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/PKG-INFO
+-rw-r--r--   0 arika      (501) staff       (20)     1153 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 arika      (501) staff       (20)        1 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 arika      (501) staff       (20)       67 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/entry_points.txt
+-rw-r--r--   0 arika      (501) staff       (20)      242 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/requires.txt
+-rw-r--r--   0 arika      (501) staff       (20)       16 2023-05-05 04:13:29.000000 openai-game-translator-1.2.0/openai_game_translator.egg-info/top_level.txt
+-rw-r--r--   0 arika      (501) staff       (20)     1216 2023-05-05 03:44:24.000000 openai-game-translator-1.2.0/pyproject.toml
+-rw-r--r--   0 arika      (501) staff       (20)       38 2023-05-05 04:13:29.626490 openai-game-translator-1.2.0/setup.cfg
+-rw-r--r--   0 arika      (501) staff       (20)       38 2023-04-07 04:06:17.000000 openai-game-translator-1.2.0/setup.py
+drwxr-xr-x   0 arika      (501) staff       (20)        0 2023-05-05 04:13:29.625755 openai-game-translator-1.2.0/tests/
+-rw-r--r--   0 arika      (501) staff       (20)     2047 2023-05-03 18:29:32.000000 openai-game-translator-1.2.0/tests/test_all.py
+-rw-r--r--   0 arika      (501) staff       (20)     1899 2023-05-04 21:43:02.000000 openai-game-translator-1.2.0/tests/test_aws_live.py
+-rw-r--r--   0 arika      (501) staff       (20)     1038 2023-05-04 21:47:09.000000 openai-game-translator-1.2.0/tests/test_aws_pre.py
+-rw-r--r--   0 arika      (501) staff       (20)     2499 2023-05-04 20:00:09.000000 openai-game-translator-1.2.0/tests/test_game_translator.py
+-rw-r--r--   0 arika      (501) staff       (20)     1041 2023-05-04 21:51:09.000000 openai-game-translator-1.2.0/tests/test_openai.py
+-rw-r--r--   0 arika      (501) staff       (20)     1037 2023-05-04 20:02:02.000000 openai-game-translator-1.2.0/tests/test_record.py
+-rw-r--r--   0 arika      (501) staff       (20)     1130 2023-05-04 21:51:33.000000 openai-game-translator-1.2.0/tests/test_xunfei.py
```

### Comparing `openai-game-translator-1.1.0/LICENSE` & `openai-game-translator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-game-translator-1.1.0/PKG-INFO` & `openai-game-translator-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-game-translator
-Version: 1.1.0
+Version: 1.2.0
 Summary: an openai based game audio translator
 Author-email: Yuhan Xia <yx2729@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,42 +216,70 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # openai-game-translator
 ChatGPT API based video game audio translator application and web service
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![GitHub issues](https://img.shields.io/github/issues/Erisae/openai-game-translator)
-![build](https://github.com/Erisae/openai-game-translator/actions/workflows/build.yml/badge.svg)
+[![GitHub issues](https://img.shields.io/github/issues/Erisae/openai-game-translator)](https://github.com/Erisae/openai-game-translator/issues)
+[![build](https://github.com/Erisae/openai-game-translator/actions/workflows/build.yml/badge.svg)](https://github.com/A-Chaudhary/age3d/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/Erisae/openai-game-translator/branch/main/graph/badge.svg?token=NI2HGVWMKI)](https://codecov.io/gh/Erisae/openai-game-translator)
 [![PyPI](https://img.shields.io/pypi/v/openai-game-translator)](https://pypi.org/project/openai-game-translator/)
+[![Documentation Status](https://readthedocs.org/projects/openai-game-translator/badge/?version=latest)](https://openai-game-translator.readthedocs.io/en/latest/?badge=latest)
+[![Doc](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=GitHub%20Pages&logoColor=white)](https://erisae.github.io/openai-game-translator/)
 
 
 ## Overview
-A game translation app that uses the ChatGPT API to recognize in-game speech (and even game visuals) and provide smooth text translations on platforms like Switch and PS5, thanks to the powerful language abilities of GPT.
+A game translation app that uses the ChatGPT API to recognize in-game speech (TODO: and even game visuals) and provide smooth text translations on platforms like Switch and PS5, thanks to the powerful language abilities of GPT.
+
+## Prerequisites
+If you don't already have local credentials setup for your AWS account, you can follow this [guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for configuring them using the AWS CLI.
+
+- Since we use amazon-transcribe SDK, which is built on top of the [AWS Common Runtime (CRT)](<https://github.com/awslabs/aws-crt-python>), non-standard operating systems may need to compile these libraries themselves.
+- Should at least set `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` environment variables and in `[default]` profile `~/.aws/credentials`.
+  
+Also, ensure that you have `portaudio`, which is a prerequisite for `pyAudio`
+```shell
+sudo apt install portaudio19-dev # linux
+brew install portaudio # macos
+```
 
 ## Installation
+Install the latest version from pip
 ```shell
 pip install openai-game-translator
 ```
+Install from github repository
+```shell
+git clone https://github.com/Erisae/openai-game-translator
+cd openai-game-translator
+make install
+```
 
 ## Quick Start
-In terminal, run
+
+### Terminal Usage
+To translate audio to text in the terminal, use the command `translate`. The simplest way to achieve this is through `AWS`'s real-time media transcription and `GPT`-based translation, as shown below:
 ```shell
-translate --xunfei_appid <appid> --xunfei_apikey  <apikey> --xunfei_apisecret <apisecret> --openai_key <key> -t <model> -o <language> --pre_recorded <use_prerecored:0|1> --file <audio_path>
+translate --openai_key <openai_key> -i <input_language> -o <output_language> aws_live
 ```
-- `<model>`: transcription model, choose from `aws_pre`, `aws_live` and `xunfei`.
-- `<language>`: translation target language, for example "English"
-- `<use_prerecored>`: whether to use prerecorded audio, 0 no, 1 yes
-- `<audio_path>`: prerecorded or transcription related audio file path
+- `<openai_key>`: A valid [OpenAI API key](https://platform.openai.com/account/api-keys) is required for inferencing GPT model to translate.
+- `<input_language>`: Language of the audio to be transcribed.
+- `<output_language>`: Target language for the translation.
+- `aws_live`: This option uses the AWS live stream transcription model, allowing the voice data stream to be uploaded to AWS services using the AWS SDK while recording the voice. Other available audio transcription models include `aws_pre` and `xunfei`, but they require additional arguments such as `--file`, `--pre_recorded`, and audio transcription API tokens from [xunfei](https://www.xfyun.cn/).
+- Note that `aws_live`, `aws_pre`, `xunfei` work as subcommands. Ensure that `openai_key`, `input_language` and `output_language` are assigned before running these subcommands, as otherwise the argument values might not be recognized correctly.  For more information about how to use the package in command line, refer to the [documentation](https://erisae.github.io/openai-game-translator/). 
 
-In script, use
+### Script Usage
+In script, simply pass `aws_live` to initialize a `gameTranslator`, `translator.openai_translation()` will translate Chinese audio to English text.
 ```python
 import openai
-from game_translator import  gameTranslator
+from game_translator import gameTranslator
 
 openai.api_key = "<openai_key>"
-translator = gameTranslator("aws_live")
+translator = gameTranslator("aws_live", input_language="chinese", output_language="english")
 translator.openai_translation()
 ```
 
+## Contributing
+See more at [CONTRIBUTING.md](./CONTRIBUTING.md)
+
```

### Comparing `openai-game-translator-1.1.0/game_translator/audio/record.py` & `openai-game-translator-1.2.0/game_translator/audio/record.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 reference: https://github.com/dylanz666/pyaudio-learning
 """
 import audioop
 import wave
 import pyaudio
+import sys
 
 
 class Detector:
     """
     A class representing a audio recorder.
 
     Attributes:
     """
 
     def __init__(
         self,
         channels=1,
         rate=44100,
         chunk=1024,
-        audio_min_rms=500,
+        audio_min_rms=1000,
         max_low_audio_flag=100,
         recording=True,
         recording_file="test.wav",
         stream_format=pyaudio.paInt16,
         pyaudio_instance=pyaudio.PyAudio(),
     ):
         self.channels = channels
@@ -33,45 +34,65 @@
         self.recording = recording
         self.recording_file = recording_file
         self.audio_frames = []
         self.stream_format = stream_format
         self.pyaudio_instance = pyaudio_instance
         self.sample_width = self.pyaudio_instance.get_sample_size(stream_format)
 
+    def show_realtime_rms(self, rms, audio_min_rms=1000):
+        step = 40 / 2000  # 50#s for rms=2000
+        sep = int(audio_min_rms * step)
+        show = int(rms * step)
+        print("\r", end="")
+        progress = "current rms: "
+        if show < sep:
+            progress += "#" * show + " " * (sep - show)
+        else:
+            progress += "#" * sep
+        progress += "|"
+
+        if show > sep:
+            progress += "#" * (show - sep)
+
+        print(progress, end="")
+        print("\033[K", end="")
+        sys.stdout.flush()
+
     def detect_audio(self):
         """
         A function to detect audio.
 
         """
 
-        print("start detecting audio ... ")
+        print("start detecting audio...")
         # print(self.pyaudio_instance.open.read(1024))
         stream = self.pyaudio_instance.open(
             format=self.stream_format,
             channels=self.channels,
             rate=self.rate,
             input=True,
             frames_per_buffer=self.chunk,
         )
         low_audio_flag = 0
         detect_count = 0
         while True:
             detect_count += 1
             stream_data = stream.read(self.chunk)
             rms = audioop.rms(stream_data, 2)
-            # print(f"the {detect_count} time detecting: ", rms)
 
             if rms > self.audio_min_rms:
                 low_audio_flag = 0
             else:
                 low_audio_flag += 1
 
+            self.show_realtime_rms(rms, self.audio_min_rms)
+
             # 100 consecutive samples of low audio
             if low_audio_flag > self.max_low_audio_flag:
-                print("detecting finished ... ")
+                print("\ndetecting finished...")
                 break
             self.audio_frames.append(stream_data)
         stream.stop_stream()
         stream.close()
         self.pyaudio_instance.terminate()
         if self.recording:
             self.record()
```

### Comparing `openai-game-translator-1.1.0/game_translator/aws_streaming_transcription/live_stream.py` & `openai-game-translator-1.2.0/game_translator/aws_streaming_transcription/live_stream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import asyncio
-import sounddevice as sd
-import numpy as np
+import pyaudio
+import audioop
 
-from difflib import SequenceMatcher
 from amazon_transcribe.client import TranscribeStreamingClient
 from amazon_transcribe.handlers import TranscriptResultStreamHandler
 from amazon_transcribe.model import TranscriptEvent
+from .settings import *
 
-"""
-https://python-sounddevice.readthedocs.io/en/0.3.7/
-sd.decault.device = #
-"""
 
-
-class MyEventHandler(TranscriptResultStreamHandler):
+class LiveEventHandler(TranscriptResultStreamHandler):
     def __init__(self, output_stream):
         super().__init__(output_stream)
         self.all_results = []
         self.last = "***"
 
     async def handle_transcript_event(self, transcript_event: TranscriptEvent):
         results = transcript_event.transcript.results
@@ -26,63 +21,55 @@
                 if self.last in alt.transcript:
                     self.all_results[-1] = alt.transcript
                 else:
                     self.all_results.append(alt.transcript)
                 self.last = alt.transcript
 
 
-def similarity(a, b):
-    return SequenceMatcher(None, a, b).ratio()
-
-
-def select_result(sentences):
-    # filter and concact
-    s = ""
-    last = ""
-    for cur in sentences:
-        if similarity(last, cur) < 0.5:  # not similar: concact
-            s += last
-            last = cur
-        elif len(last) < len(cur):  # similar and longer: update
-            last = cur
-    s += last
-    return "".join(s)
-
-
-async def basic_transcribe(max_low_audio_flag=20, audio_min_rms=100):
-    client = TranscribeStreamingClient(region="us-east-2")
+async def live_transcribe(
+    input_language: str,
+    audio_min_rms=AUDIO_MIN_RMS,
+    max_low_audio_flag=MAX_LOW_AUDIO_FLAG,
+):
+    client = TranscribeStreamingClient(region=REGION)
 
     stream = await client.start_stream_transcription(
-        language_code="en-US",
-        media_sample_rate_hz=16000,
+        language_code=LANGUAGE_MAPPING[input_language],
+        media_sample_rate_hz=SAMPLE_RATE,
         media_encoding="pcm",
     )
 
     async def write_chunks():
         low_audio_flag = 0
-        while True:
-            data = sd.rec(
-                1024 * 8, samplerate=16000, channels=1, blocking=True, dtype="int16"
-            )
+        record_stream = pyaudio.PyAudio().open(
+            format=pyaudio.paInt16,
+            channels=CHANNEL_NUMS,
+            rate=SAMPLE_RATE,
+            input=True,
+            frames_per_buffer=CHUNK_SIZE,
+        )
+        print("start detecting audio...")
 
-            data[np.isnan(data)] = 0
-            rms = np.sqrt(np.mean(np.square(data)))
+        while True:
+            data = record_stream.read(CHUNK_SIZE)
+            rms = audioop.rms(data, 2)
 
             low_audio_flag = 0 if rms > audio_min_rms else low_audio_flag + 1
 
-            # 100 consecutive samples of low audio
+            show_realtime_rms(rms, audio_min_rms=audio_min_rms)
             if low_audio_flag > max_low_audio_flag:
+                print("\ndetecting finished...")
                 break
 
             # convert the audio frame to byte stream and send it to service.
-            await stream.input_stream.send_audio_event(audio_chunk=data.tobytes())
+            await stream.input_stream.send_audio_event(audio_chunk=data)  # tobytes()
 
         await stream.input_stream.end_stream()
 
-    handler = MyEventHandler(stream.output_stream)
+    handler = LiveEventHandler(stream.output_stream)
     await asyncio.gather(write_chunks(), handler.handle_events())
 
     s = select_result(handler.all_results)
     print("transcription success...")
     print(s)
 
     return s
```

### Comparing `openai-game-translator-1.1.0/game_translator/openai_translation/chat.py` & `openai-game-translator-1.2.0/game_translator/openai_translation/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def translate_sentence(content, language):
     """
     A function to use openai to translate
 
     """
 
-    prompt = "please translate the following to " + language + " : " + content
+    prompt = "translate the following to " + language + " : " + content
     completion = openai.ChatCompletion.create(
         model="gpt-3.5-turbo", messages=[{"role": "user", "content": prompt}]
     )
     format = "^['\"]|['\"]$"
     res = completion.choices[0].message.content.strip()
     res = re.sub(format, "", res)
```

### Comparing `openai-game-translator-1.1.0/game_translator/xunfei_speed_transcription/ost_fast.py` & `openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/ost_fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 import json
 import os
 import re
 import requests
 
 from .seve_file import SeveFile
 
+LANGUAGE_MAPPING = {"english": "en_us", "chinese": "zh_cn"}
+
 
 # create and query
 class xf_transcriptor:
     """
     A class representing a xf_transcriptor.
 
     Attributes:
     """
 
-    def __init__(self, appid, apikey, apisecret, file_path):
+    def __init__(self, appid, apikey, apisecret, file_path, input_language):
         # POST request
         self.Host = "ost-api.xfyun.cn"
         self.RequestUriCreate = "/v2/ost/pro_create"
         self.RequestUriQuery = "/v2/ost/query"
         # url setting
         if re.match(r"^\d", self.Host):
             self.urlCreate = "http://" + self.Host + self.RequestUriCreate
@@ -50,19 +52,18 @@
         self.FilePath = file_path
 
         # current time setting
         cur_time_utc = datetime.datetime.utcnow()
         self.Date = self.httpdate(cur_time_utc)
         # test file setting
         self.BusinessArgsCreate = {
-            "language": "zh_cn",
+            "language": LANGUAGE_MAPPING[input_language],
             "accent": "mandarin",
             "language_type": 1,
             "domain": "pro_ost_ed",
-            # "callback_url": "http://IP:port/xxx/"
         }
 
     def hashlib_256(self, res):
         """
         A function to .
 
         """
@@ -189,15 +190,14 @@
         """
         A function to create task
 
         """
         body = self.get_create_body()
         headers_create = self.init_header(body, self.RequestUriCreate)
         task_id = self.call(self.urlCreate, body, headers_create)
-        # print(task_id)
         return task_id
 
     def task_query(self, task_id):
         """
         A function to query task
 
         """
```

### Comparing `openai-game-translator-1.1.0/game_translator/xunfei_speed_transcription/seve_file.py` & `openai-game-translator-1.2.0/game_translator/xunfei_speed_transcription/seve_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,16 @@
             api_secret=api_secret,
             body=file_data,
         )
         try:
             resp = requests.post(url, headers=headerss, data=file_data, timeout=8)
             # print("Chunk upload success. STATUS：", resp.status_code, resp.text)
             return resp.json()
-        except Exception:
-            # print("Chunk upload failed！Exception ：%s" % e)
+        except Exception as e:
+            print("Chunk upload failed! Exception :%s" % e)
             return False
 
     # chunk upload complete
     def upload_cut_complete(self, body_dict):
         file_data_type = "application/json"
         url = lfasr_host + api_cut_complete
         fileurl = self.call(url, json.dumps(body_dict), file_data_type)
```

### Comparing `openai-game-translator-1.1.0/openai_game_translator.egg-info/PKG-INFO` & `openai-game-translator-1.2.0/openai_game_translator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-game-translator
-Version: 1.1.0
+Version: 1.2.0
 Summary: an openai based game audio translator
 Author-email: Yuhan Xia <yx2729@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,42 +216,70 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # openai-game-translator
 ChatGPT API based video game audio translator application and web service
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-![GitHub issues](https://img.shields.io/github/issues/Erisae/openai-game-translator)
-![build](https://github.com/Erisae/openai-game-translator/actions/workflows/build.yml/badge.svg)
+[![GitHub issues](https://img.shields.io/github/issues/Erisae/openai-game-translator)](https://github.com/Erisae/openai-game-translator/issues)
+[![build](https://github.com/Erisae/openai-game-translator/actions/workflows/build.yml/badge.svg)](https://github.com/A-Chaudhary/age3d/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/Erisae/openai-game-translator/branch/main/graph/badge.svg?token=NI2HGVWMKI)](https://codecov.io/gh/Erisae/openai-game-translator)
 [![PyPI](https://img.shields.io/pypi/v/openai-game-translator)](https://pypi.org/project/openai-game-translator/)
+[![Documentation Status](https://readthedocs.org/projects/openai-game-translator/badge/?version=latest)](https://openai-game-translator.readthedocs.io/en/latest/?badge=latest)
+[![Doc](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=GitHub%20Pages&logoColor=white)](https://erisae.github.io/openai-game-translator/)
 
 
 ## Overview
-A game translation app that uses the ChatGPT API to recognize in-game speech (and even game visuals) and provide smooth text translations on platforms like Switch and PS5, thanks to the powerful language abilities of GPT.
+A game translation app that uses the ChatGPT API to recognize in-game speech (TODO: and even game visuals) and provide smooth text translations on platforms like Switch and PS5, thanks to the powerful language abilities of GPT.
+
+## Prerequisites
+If you don't already have local credentials setup for your AWS account, you can follow this [guide](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for configuring them using the AWS CLI.
+
+- Since we use amazon-transcribe SDK, which is built on top of the [AWS Common Runtime (CRT)](<https://github.com/awslabs/aws-crt-python>), non-standard operating systems may need to compile these libraries themselves.
+- Should at least set `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` environment variables and in `[default]` profile `~/.aws/credentials`.
+  
+Also, ensure that you have `portaudio`, which is a prerequisite for `pyAudio`
+```shell
+sudo apt install portaudio19-dev # linux
+brew install portaudio # macos
+```
 
 ## Installation
+Install the latest version from pip
 ```shell
 pip install openai-game-translator
 ```
+Install from github repository
+```shell
+git clone https://github.com/Erisae/openai-game-translator
+cd openai-game-translator
+make install
+```
 
 ## Quick Start
-In terminal, run
+
+### Terminal Usage
+To translate audio to text in the terminal, use the command `translate`. The simplest way to achieve this is through `AWS`'s real-time media transcription and `GPT`-based translation, as shown below:
 ```shell
-translate --xunfei_appid <appid> --xunfei_apikey  <apikey> --xunfei_apisecret <apisecret> --openai_key <key> -t <model> -o <language> --pre_recorded <use_prerecored:0|1> --file <audio_path>
+translate --openai_key <openai_key> -i <input_language> -o <output_language> aws_live
 ```
-- `<model>`: transcription model, choose from `aws_pre`, `aws_live` and `xunfei`.
-- `<language>`: translation target language, for example "English"
-- `<use_prerecored>`: whether to use prerecorded audio, 0 no, 1 yes
-- `<audio_path>`: prerecorded or transcription related audio file path
+- `<openai_key>`: A valid [OpenAI API key](https://platform.openai.com/account/api-keys) is required for inferencing GPT model to translate.
+- `<input_language>`: Language of the audio to be transcribed.
+- `<output_language>`: Target language for the translation.
+- `aws_live`: This option uses the AWS live stream transcription model, allowing the voice data stream to be uploaded to AWS services using the AWS SDK while recording the voice. Other available audio transcription models include `aws_pre` and `xunfei`, but they require additional arguments such as `--file`, `--pre_recorded`, and audio transcription API tokens from [xunfei](https://www.xfyun.cn/).
+- Note that `aws_live`, `aws_pre`, `xunfei` work as subcommands. Ensure that `openai_key`, `input_language` and `output_language` are assigned before running these subcommands, as otherwise the argument values might not be recognized correctly.  For more information about how to use the package in command line, refer to the [documentation](https://erisae.github.io/openai-game-translator/). 
 
-In script, use
+### Script Usage
+In script, simply pass `aws_live` to initialize a `gameTranslator`, `translator.openai_translation()` will translate Chinese audio to English text.
 ```python
 import openai
-from game_translator import  gameTranslator
+from game_translator import gameTranslator
 
 openai.api_key = "<openai_key>"
-translator = gameTranslator("aws_live")
+translator = gameTranslator("aws_live", input_language="chinese", output_language="english")
 translator.openai_translation()
 ```
 
+## Contributing
+See more at [CONTRIBUTING.md](./CONTRIBUTING.md)
+
```

### Comparing `openai-game-translator-1.1.0/openai_game_translator.egg-info/SOURCES.txt` & `openai-game-translator-1.2.0/openai_game_translator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-.bumpversion.cfg
-CONTRIBUTING.md
 LICENSE
-MANIFEST.in
-Makefile
 README.md
 pyproject.toml
 setup.py
 game_translator/__init__.py
 game_translator/__main__.py
 game_translator/_version.py
 game_translator/game_translator.py
 game_translator/audio/__init__.py
-game_translator/audio/audio_sample_little.wav
 game_translator/audio/record.py
-game_translator/audio/test.wav
 game_translator/aws_streaming_transcription/__init__.py
 game_translator/aws_streaming_transcription/live_stream.py
 game_translator/aws_streaming_transcription/prerecorded_stream.py
+game_translator/aws_streaming_transcription/settings.py
 game_translator/openai_translation/__init__.py
 game_translator/openai_translation/chat.py
 game_translator/xunfei_speed_transcription/__init__.py
 game_translator/xunfei_speed_transcription/ost_fast.py
 game_translator/xunfei_speed_transcription/seve_file.py
 openai_game_translator.egg-info/PKG-INFO
 openai_game_translator.egg-info/SOURCES.txt
 openai_game_translator.egg-info/dependency_links.txt
 openai_game_translator.egg-info/entry_points.txt
 openai_game_translator.egg-info/requires.txt
 openai_game_translator.egg-info/top_level.txt
-tests/.coveragerc
 tests/test_all.py
 tests/test_aws_live.py
 tests/test_aws_pre.py
 tests/test_game_translator.py
 tests/test_openai.py
 tests/test_record.py
 tests/test_xunfei.py
```

### Comparing `openai-game-translator-1.1.0/pyproject.toml` & `openai-game-translator-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai-game-translator"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Yuhan Xia", email="yx2729@columbia.edu" },
 ]
 description = "an openai based game audio translator"
 readme = "README.md"
 requires-python = ">=3.9, <3.11"
 classifiers = [
@@ -21,15 +21,14 @@
 dependencies = [
     "aiofile==3.8.5",
     "amazon-transcribe==0.6.1",
     "numpy==1.24.2",
     "openai==0.27.2",
     "pyaudio==0.2.13",
     "requests==2.27.1",
-    "sounddevice==0.4.6",
     "urllib3==1.26.15"
 ]
 
 [project.optional-dependencies]
 develop = [
     "coverage==7.2.2",
     "black==23.3.0",
```

### Comparing `openai-game-translator-1.1.0/tests/test_all.py` & `openai-game-translator-1.2.0/tests/test_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from test_aws_live import TestLiveStream
 from test_aws_pre import TestPrerecorded
 from test_openai import TestOpenai
 from test_record import TestRecord
 from test_game_translator import TranslatorTest
 
 def main():
-    parser_test = argparse.ArgumentParser(description="Description of your program")
+    parser_test = argparse.ArgumentParser(description="Test openai-game-translator")
     parser_test.add_argument(
         "--xunfei_appid", required=True, type=str, help="xunfei transcription appid"
     )
     parser_test.add_argument(
         "--xunfei_apikey", required=True, type=str, help="xunfei transcription apikey"
     )
     parser_test.add_argument(
         "--xunfei_apisecret",
         required=True,
         type=str,
         help="xunfei transccription api secret",
     )
     parser_test.add_argument(
-        "--openai_key", required=True, type=str, help="open ai translatio api key"
+        "--openai_key", required=True, type=str, help="openai api key"
     )
     args_test = parser_test.parse_args()
     openai.api_key = args_test.openai_key
      # define overall testsuite
     test_suite = unittest.TestSuite()
 
     # add testsuites
```

### Comparing `openai-game-translator-1.1.0/tests/test_aws_live.py` & `openai-game-translator-1.2.0/tests/test_aws_live.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import unittest
 import asyncio
 import os
 import sys
 import io
 import numpy as np
+import pyaudio
 
 sys.path.append(os.path.abspath("../"))
 from unittest.mock import patch
-from game_translator.aws_streaming_transcription.live_stream import basic_transcribe, select_result
+from game_translator.aws_streaming_transcription.live_stream import live_transcribe
+from game_translator.aws_streaming_transcription.settings import *
 
 
 class TestLiveStream(unittest.TestCase):
-    @patch("sounddevice.rec")
+    @patch("pyaudio.PyAudio.open")
     def test_transcription_success(self, mock_rec):
         # Set up mock audio data
         with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            mock_rec.return_value = np.array([[1] * 1024 * 8])
+            mock_rec.return_value.read.return_value = bytes([1] * CHUNK_SIZE)
 
             # Run the function under test and get the result
             self.loop = asyncio.get_event_loop()
             result = self.loop.run_until_complete(
-                basic_transcribe(max_low_audio_flag=0)
+                live_transcribe(input_language="english", max_low_audio_flag=10)
             )
 
             # Check that the result is as expected
             self.assertIsNotNone(result)
-            self.assertEqual(fake_out.getvalue().strip(), "transcription success...")
+            self.assertIn("transcription success...", fake_out.getvalue().strip())
 
     def test_select_result(self):
         # Set up test cases for select_result function
         test_cases = [
             (["hello", "world"], "helloworld"),
             (["goodbye", " world", "worldok"], "goodbyeworldok"),
             (["hello.", "hello", "world"], "hello.world"),
             (["hello", "world", "hello ", "world"], "helloworldhello world"),
+            (["hello", "hella word, this is the first publication"], "hella word, this is the first publication"),
         ]
         for sentences, expected in test_cases:
             with self.subTest(sentences=sentences):
                 # Call the function under test
                 result = select_result(sentences)
                 # Check that the result is as expected
                 self.assertEqual(result, expected)
```

### Comparing `openai-game-translator-1.1.0/tests/test_game_translator.py` & `openai-game-translator-1.2.0/tests/test_game_translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     def test_xunfei_openai(self):
         translator1 = gameTranslator(
             "xunfei",
             filepath="../game_translator/audio/audio_sample_little.wav",
             xunfei_appid=self.appid,
             xunfei_apikey=self.apikey,
             xunfei_apisecret=self.apisecret,
-            prerecorded=1,
-            output_language="English",
+            prerecorded=True,
+            input_language="chinese",
+            output_language="english",
+            
         )
 
         with patch("sys.stdout", new=io.StringIO()) as fake_out:
             res = translator1.openai_translation()
             self.assertIsNotNone(res)
             self.assertTrue(
                 contains_substring(
@@ -37,17 +39,17 @@
                     fake_out.getvalue().strip(), "translation success..."
                 )
             )
 
     def test_aws_pre_openai(self):
         translator3 = gameTranslator(
             "aws_pre",
-            prerecorded=1,
+            prerecorded=True,
             filepath="../game_translator/audio/audio_sample_little.wav",
-            output_language="English",
+            output_language="english",
         )
 
         with patch("sys.stdout", new=io.StringIO()) as fake_out:
             res = translator3.openai_translation()
             self.assertIsNotNone(res)
             self.assertTrue(
                 contains_substring(
```

### Comparing `openai-game-translator-1.1.0/tests/test_openai.py` & `openai-game-translator-1.2.0/tests/test_openai.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,27 +14,22 @@
 class TestOpenai(unittest.TestCase):
     def setUp(self):
         self.language = "Japanese"
 
     def test_translation(self):
         test_cases = [
             "this is the first time i do an oss project",
-            "helloworld",
-            "hello world",
-            "",
-        ]
+            # "",
+        ] # 3 per min
         for sentence in test_cases:
             with self.subTest(sentence=sentence):
                 # Call the function under test
                 with patch("sys.stdout", new=io.StringIO()) as fake_out:
                     result = translate_sentence(sentence, self.language)
+
                     # Check that the result is as expected
-                    self.assertTrue(
-                        contains_substring(
-                            fake_out.getvalue().strip(), "translation success..."
-                        )
-                    )
+                    self.assertIn("translation success...", fake_out.getvalue().strip())
                     self.assertIsNotNone(result)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openai-game-translator-1.1.0/tests/test_record.py` & `openai-game-translator-1.2.0/tests/test_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import os
 import sys
 import io
 import pyaudio
-import numpy as np
+
 sys.path.append(os.path.abspath("../"))
 from unittest.mock import patch
 from game_translator.audio.record import Detector
 
 
 def contains_substring(string, substring):
     return substring in string
@@ -23,17 +23,15 @@
             rate=44100,
             input=True,
             frames_per_buffer=1024).read.return_value = mock_data
         
         with patch("sys.stdout", new=io.StringIO()) as fake_out:
             detector = Detector(pyaudio_instance=mock_pyaudio, max_low_audio_flag=mock_flag, recording=False)
             detector.detect_audio()
-            
-        self.assertTrue(
-            "detecting finished ..." in fake_out.getvalue().strip()
-        )
+
+        self.assertIn("detecting finished...", fake_out.getvalue().strip())
         self.assertEqual(len(detector.audio_frames), mock_flag)
 
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openai-game-translator-1.1.0/tests/test_xunfei.py` & `openai-game-translator-1.2.0/tests/test_xunfei.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,23 @@
     return substring in string
 
 
 class TestXFTranscriptor(unittest.TestCase):
     def setUp(self):  #
         self.file_path = "../game_translator/audio/audio_sample_little.wav"
         self.transcriptor = xf_transcriptor(
-            self.appid, self.apikey, self.apisecret, self.file_path
+            self.appid, self.apikey, self.apisecret, self.file_path, input_language="chinese"
         )
 
-    # def test_task_create(self):
-    #     task_id = self.transcriptor.task_create()
-    #     self.assertIsNotNone(task_id)
-
     def test_get_result(self):
         with patch("sys.stdout", new=io.StringIO()) as fake_out:
             self.transcriptor.get_fileurl()
             result = self.transcriptor.get_result()
             self.assertIsNotNone(result)
-            self.assertEqual(result, "科大讯飞是中国最大的智能语音技术提供商。")
+            # self.assertEqual(result, "科大讯飞是中国最大的智能语音技术提供商。")
             self.assertTrue(
                 contains_substring(
                     fake_out.getvalue().strip(), "transcription success..."
                 )
             )
```

