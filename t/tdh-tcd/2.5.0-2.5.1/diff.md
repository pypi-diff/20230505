# Comparing `tmp/tdh-tcd-2.5.0.tar.gz` & `tmp/tdh-tcd-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdh-tcd-2.5.0.tar", last modified: Wed Dec  7 21:18:13 2022, max compression
+gzip compressed data, was "tdh-tcd-2.5.1.tar", last modified: Fri May  5 21:28:06 2023, max compression
```

## Comparing `tdh-tcd-2.5.0.tar` & `tdh-tcd-2.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 21:18:13.319347 tdh-tcd-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2022-12-07 21:18:13.319347 tdh-tcd-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 21:18:13.319347 tdh-tcd-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 21:18:13.319347 tdh-tcd-2.5.0/tcd/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/tcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/tcd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/tcd/example.settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/tcd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/tcd/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2022-12-07 21:18:00.000000 tdh-tcd-2.5.0/tcd/twitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 21:18:13.319347 tdh-tcd-2.5.0/tdh_tcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2022-12-07 21:18:13.000000 tdh-tcd-2.5.0/tdh_tcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-07 21:18:13.000000 tdh-tcd-2.5.0/tdh_tcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 21:18:13.000000 tdh-tcd-2.5.0/tdh_tcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-07 21:18:13.000000 tdh-tcd-2.5.0/tdh_tcd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-07 21:18:13.000000 tdh-tcd-2.5.0/tdh_tcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-07 21:18:13.000000 tdh-tcd-2.5.0/tdh_tcd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:06.516397 tdh-tcd-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-05 21:28:06.516397 tdh-tcd-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:28:06.516397 tdh-tcd-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:06.512397 tdh-tcd-2.5.1/tcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/example.settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/twitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:06.512397 tdh-tcd-2.5.1/tdh_tcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/top_level.txt
```

### Comparing `tdh-tcd-2.5.0/LICENSE` & `tdh-tcd-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.0/PKG-INFO` & `tdh-tcd-2.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.0
+Version: 2.5.1
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Twitch Chat Downloader [![PyPI version](https://badge.fury.io/py/tdh-tcd.svg)](https://badge.fury.io/py/tdh-tcd)
 
 Neat python script to download chat messages from past broadcasts
 
 ## Requirements
 
-* [Python 2.7 or 3.4+](https://www.python.org/downloads/)
+* [Python 3.6+](https://www.python.org/downloads/)
 * [pip](https://pip.pypa.io/en/stable/installing/)
 * [python-requests](http://docs.python-requests.org/en/master/user/install/)
 
 ## Installation and usage
 
 There are multiple ways to install this script.
 
@@ -62,24 +61,29 @@
 | cooldown | *int* | `--cooldown` | Delay (in milliseconds) between API calls. |
 | display_progress | *bool* | `--[no-]progress` | Display animated progress bar in terminal. |
 | formats | *str[]* | `-f/--formats` | List of formats to download. See Formats table below. |
 | directory | *str* | `-t`/`--directory` | Name of directory to save all generated files. |
 | filename_format | *str* | `--filename-format` | Full format of generated filenames. Possible arguments: `directory`, `video_id` and `format`. |
 | max_width | *int* | `--max-width` | Add line breaks to fit messages into specified width. Note: Implemented only for SSA/ASS subtitles. |
 | subtitle_duration | *int* | `--subtitle-duration` | Duration (in seconds) of each line of subtitles. |
-| dynamic_duration | *obj* |  | Convert `Kappa Kappa Kappa` to `Kappa x3`. |
-| —.enabled | *bool* | `--[no-]dynamic-duration` | Increase subtitle duration based on message length. |
+| dynamic_duration | *obj* |  | Increase subtitle duration based on message length. |
+| —.enabled | *bool* | `--[no-]dynamic-duration` | Enable or disable this function. |
 | —.max | *int* | `--dynamic-duration-max` | Maximum duration of subtitle message. |
 | —.max_length | *int* | `--dynamic-duration-max-length` | Maximum length of subtitle message. |
+| millisecond_separator | *str* | `--millisecond-separator` | Separator between seconds and milliseconds in timestamps (IRC only). |
 | group_repeating_emotes | *obj* |  | Convert `Kappa Kappa Kappa` to `Kappa x3`. |
 | —.enabled | *bool* | `--[no-]group` | Enable or disable this function. |
 | —.threshold | *int* | `--group-threshold` | Number of repeating emotes to trigger this function. |
 | —.collocations | *int* | `--group-collocations` | Maximum number of words in repeating collocations (default: 1, more is slower). |
 | —.collocations_threshold | *int* | `--group-collocations-threshold` | Same logic as in —.threshold, but applies only to repeating collocations. |
 | —.format | *str* | `--group-format` | Customize format of replaced emotes. |
+| badges | *obj* |  | Add badges before the username (IRC only). |
+| —.enabled | *bool* | `--[no-]badges` | Enable or disable this function. |
+| —.max_count | *int* | `--badges-max` | Only show the first N badges (default: 1) |
+| —.map | *obj* | | Configure which symbol corresponds to a specific badge. |
 | video_types | *str* | `--video-types` | Comma-separated list of VOD types to detect in Channel Mode. (see [broadcast_type](https://dev.twitch.tv/docs/v5/reference/channels/#get-channel-videos)) |
 
 ## Formats
 
 | Format | Description |
 | ------ | ----------- |
 | `ass` or `ssa` | Advanced SubStation Alpha |
```

### Comparing `tdh-tcd-2.5.0/README.md` & `tdh-tcd-2.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Twitch Chat Downloader [![PyPI version](https://badge.fury.io/py/tdh-tcd.svg)](https://badge.fury.io/py/tdh-tcd)
 
 Neat python script to download chat messages from past broadcasts
 
 ## Requirements
 
-* [Python 2.7 or 3.4+](https://www.python.org/downloads/)
+* [Python 3.6+](https://www.python.org/downloads/)
 * [pip](https://pip.pypa.io/en/stable/installing/)
 * [python-requests](http://docs.python-requests.org/en/master/user/install/)
 
 ## Installation and usage
 
 There are multiple ways to install this script.
 
@@ -45,24 +45,29 @@
 | cooldown | *int* | `--cooldown` | Delay (in milliseconds) between API calls. |
 | display_progress | *bool* | `--[no-]progress` | Display animated progress bar in terminal. |
 | formats | *str[]* | `-f/--formats` | List of formats to download. See Formats table below. |
 | directory | *str* | `-t`/`--directory` | Name of directory to save all generated files. |
 | filename_format | *str* | `--filename-format` | Full format of generated filenames. Possible arguments: `directory`, `video_id` and `format`. |
 | max_width | *int* | `--max-width` | Add line breaks to fit messages into specified width. Note: Implemented only for SSA/ASS subtitles. |
 | subtitle_duration | *int* | `--subtitle-duration` | Duration (in seconds) of each line of subtitles. |
-| dynamic_duration | *obj* |  | Convert `Kappa Kappa Kappa` to `Kappa x3`. |
-| —.enabled | *bool* | `--[no-]dynamic-duration` | Increase subtitle duration based on message length. |
+| dynamic_duration | *obj* |  | Increase subtitle duration based on message length. |
+| —.enabled | *bool* | `--[no-]dynamic-duration` | Enable or disable this function. |
 | —.max | *int* | `--dynamic-duration-max` | Maximum duration of subtitle message. |
 | —.max_length | *int* | `--dynamic-duration-max-length` | Maximum length of subtitle message. |
+| millisecond_separator | *str* | `--millisecond-separator` | Separator between seconds and milliseconds in timestamps (IRC only). |
 | group_repeating_emotes | *obj* |  | Convert `Kappa Kappa Kappa` to `Kappa x3`. |
 | —.enabled | *bool* | `--[no-]group` | Enable or disable this function. |
 | —.threshold | *int* | `--group-threshold` | Number of repeating emotes to trigger this function. |
 | —.collocations | *int* | `--group-collocations` | Maximum number of words in repeating collocations (default: 1, more is slower). |
 | —.collocations_threshold | *int* | `--group-collocations-threshold` | Same logic as in —.threshold, but applies only to repeating collocations. |
 | —.format | *str* | `--group-format` | Customize format of replaced emotes. |
+| badges | *obj* |  | Add badges before the username (IRC only). |
+| —.enabled | *bool* | `--[no-]badges` | Enable or disable this function. |
+| —.max_count | *int* | `--badges-max` | Only show the first N badges (default: 1) |
+| —.map | *obj* | | Configure which symbol corresponds to a specific badge. |
 | video_types | *str* | `--video-types` | Comma-separated list of VOD types to detect in Channel Mode. (see [broadcast_type](https://dev.twitch.tv/docs/v5/reference/channels/#get-channel-videos)) |
 
 ## Formats
 
 | Format | Description |
 | ------ | ----------- |
 | `ass` or `ssa` | Advanced SubStation Alpha |
```

### Comparing `tdh-tcd-2.5.0/setup.py` & `tdh-tcd-2.5.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-#!/usr/bin/env python
-
 from setuptools import setup, find_packages
 
 
 with open('README.md', 'r') as fi:
     long_description = fi.read()
 
 
 setup(
     name='tdh-tcd',
-    version='2.5.0',
+    version='2.5.1',
 
     author='Dmitry Karikh',
     author_email='the.dr.hax@gmail.com',
 
     description='Twitch Chat Downloader',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -32,15 +30,14 @@
     entry_points='''
     [console_scripts]
     tcd=tcd:main
     ''',
 
     classifiers=[
         'Environment :: Console',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.6',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Utilities'
     ]
 )
```

### Comparing `tdh-tcd-2.5.0/tcd/__init__.py` & `tdh-tcd-2.5.1/tcd/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 def generate_config():
     with open('settings.json', 'w') as f:
         f.write(json.dumps(settings, indent=2))
 
 
 def download(video):
-    writer = SubtitleWriter(video)
-    for comment in Messages(video):
+    messages = Messages(video)
+    writer = SubtitleWriter(messages)
+    for comment in messages:
         writer.add(comment)
     writer.close()
 
 
 def download_all(channel, min=0, max=None, count=None):
     videos = Channel(channel).videos()
     to_download = list()
```

### Comparing `tdh-tcd-2.5.0/tcd/example.settings.json` & `tdh-tcd-2.5.1/tcd/example.settings.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'badges'": "OrderedDict([('enabled', False), ('max_count', 1), ('map', "*

 * *             "OrderedDict([('broadcaster', '~'), ('vip', '^'), ('staff', '&'), ('admin', '!'), "*

 * *             "('global_mod', '*'), ('moderator', '@'), ('artist-badge', '|'), ('game-developer', "*

 * *             "'}'), ('founder', '#'), ('sub-gift-leader', '='), ('sub-gifter', '-'), ('partner', "*

 * *             "')'), ('bits', '$'), ('bits-charity', '$'), ('twitchbot', '?'), ('subscriber', '%'), "*

 * *             "('premium', '+'), ('turbo', […]*

```diff
@@ -1,8 +1,35 @@
 {
+    "badges": {
+        "enabled": false,
+        "map": {
+            "admin": "!",
+            "artist-badge": "|",
+            "bits": "$",
+            "bits-charity": "$",
+            "broadcaster": "~",
+            "founder": "#",
+            "game-developer": "}",
+            "global_mod": "*",
+            "hype-train": "+",
+            "moderator": "@",
+            "no_audio": "/",
+            "no_video": "/",
+            "partner": ")",
+            "premium": "+",
+            "staff": "&",
+            "sub-gift-leader": "=",
+            "sub-gifter": "-",
+            "subscriber": "%",
+            "turbo": "+",
+            "twitchbot": "?",
+            "vip": "^"
+        },
+        "max_count": 1
+    },
     "client_id": "jzkbprff40iqj646a697cyrvl0zt2m6",
     "cooldown": 0,
     "directory": "chats",
     "display_progress": true,
     "dynamic_duration": {
         "enabled": false,
         "max": 5,
@@ -18,14 +45,15 @@
         "collocations": 5,
         "collocations_threshold": 2,
         "enabled": false,
         "format": "{emote} x{count}",
         "threshold": 3
     },
     "max_width": -1,
+    "millisecond_separator": ",",
     "ssa_events_format": "Format: Marked, Start, End, Style, Name, MarginL, MarginR, MarginV, Effect, Text",
     "ssa_events_line_format": "Dialogue: Marked=0, {start}, {end}, Default, {user}, 0000, 0000, 0000, , {user}: {message}",
     "ssa_style_default": "Style: Default,Arial,20,16777215,16777215,16777215,-2147483640,-1,0,1,3,0,1,5,0,5,0,0",
     "ssa_style_format": "Format: Name, Fontname, Fontsize, PrimaryColour, SecondaryColour, TertiaryColour, BackColour, Bold, Italic, BorderStyle, Outline, Shadow, Alignment, MarginL, MarginR, MarginV, AlphaLevel, Encoding",
     "subtitle_duration": 2,
     "version": "2.4.4",
     "video_types": "archive"
```

### Comparing `tdh-tcd-2.5.0/tcd/settings.py` & `tdh-tcd-2.5.1/tcd/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 import os
 import sys
 import json
 import inspect
 from argparse import ArgumentParser
 
 
 SELF = inspect.getfile(inspect.currentframe())
 ROOT = os.path.dirname(os.path.abspath(SELF))
 
-settings_file_default = 'settings.json'
-if not os.path.isfile(settings_file_default):
-    settings_file_default = ROOT + '/example.settings.json'
+settings_filename = 'settings.json'
+home_settings_path = os.path.join(os.path.expanduser('~'), '.config/tcd', settings_filename)
+example_settings_path = os.path.join(ROOT, f'example.{settings_filename}')
+
+if os.path.isfile(settings_filename):
+    settings_file_default = settings_filename
+elif os.path.isfile(home_settings_path):
+    settings_file_default = home_settings_path
+else:
+    settings_file_default = example_settings_path
 
 
 def _pre_init_parser(help=False):
     parser = ArgumentParser(
         description='Download VOD chats from Twitch.', add_help=help)
     parser.add_argument(
         '-s', '--settings', metavar='settings.json',
@@ -30,19 +34,21 @@
 settings_file = args.settings
 
 # Read settings from file
 with open(settings_file, 'r') as settings_file:
     settings = json.load(settings_file)
 
 # Check for outdated settings.json
-if settings['version'].startswith("1"):
-    print("Please update your settings.json " +
-          "(see example.settings.json for examples)")
+if settings['version'].startswith('1'):
+    print('Please update your settings.json ' +
+          '(see example.settings.json for examples)')
     sys.exit(1)
 
+if 'millisecond_separator' not in settings:
+    settings['millisecond_separator'] = ','
 if 'group_repeating_emotes' not in settings:
     settings['group_repeating_emotes'] = {'enabled': False,
                                           'threshold': 3,
                                           'collocations': 1,
                                           'format': '{emote} x{count}'}
 if 'collocations' not in settings['group_repeating_emotes']:
     settings['group_repeating_emotes']['collocations'] = 1
@@ -52,14 +58,16 @@
 if 'video_types' not in settings:
     settings['video_types'] = 'archive'
 if 'dynamic_duration' not in settings:
     settings['dynamic_duration'] = {'enabled': False, 'max': 5,
                                     'max_length': 100}
 if 'max_width' not in settings:
     settings['max_width'] = -1
+if 'badges' not in settings:
+    settings['badges'] = {'enabled': False, 'max_count': 1, 'map': {}}
 
 #
 # Post-init settings overrides
 #
 
 
 def _post_init_parser(help=False):
@@ -91,15 +99,16 @@
         '-t', '--directory', metavar='PATH', type=str,
         default=settings['directory'],
         help='Target directory to save all generated subtitles.')
     settings_group.add_argument(
         '--filename-format', metavar='FORMAT', type=str,
         default=settings['filename_format'],
         help=('Python str.format for generating output file names. Available '
-              'variables: {directory}, {video_id} and {format}.'))
+              'variables: {directory}, {video_id}, {format}, {user_name}, '
+              '{title}, and {created_at}.'))
     settings_group.add_argument(
         '--max-width', metavar='chars', type=int,
         default=settings['max_width'],
         help=('Add line breaks to fit messages into specified width. '
               'Note: Implemented only for SSA/ASS subtitles.'))
     settings_group.add_argument(
         '--subtitle-duration', metavar='sec', type=int,
@@ -117,14 +126,18 @@
         '--dynamic-duration-max', metavar='sec', type=int,
         default=settings['dynamic_duration']['max'],
         help='Maximum duration of subtitle message.')
     settings_group.add_argument(
         '--dynamic-duration-max-length', metavar='chars', type=int,
         default=settings['dynamic_duration']['max_length'],
         help='Maximum length of subtitle message.')
+    settings_group.add_argument(
+        '--millisecond-separator', metavar='FORMAT', type=str,
+        default=settings['millisecond_separator'],
+        help='Separator between seconds and milliseconds in timestamps.')
 
     group = settings_group.add_mutually_exclusive_group(required=False)
     group.add_argument(
         '--group', action='store_true', dest='group',
         default=settings['group_repeating_emotes']['enabled'],
         help=('Group repeating emotes in all messages. '
               'Example: Kappa Kappa Kappa → Kappa x3.'))
@@ -148,14 +161,28 @@
               'repeating collocations.'))
     settings_group.add_argument(
         '--group-format', metavar='FORMAT', type=str,
         default=settings['group_repeating_emotes']['format'],
         help=('Python str.format for grouped emotes. Available '
               'variables: {emote} and {count}.'))
 
+    badges = settings_group.add_mutually_exclusive_group(required=False)
+    badges.add_argument(
+        '--badges', action='store_true', dest='badges',
+        default=settings['badges']['enabled'],
+        help=('Add badges before usernames (IRC only).'))
+    badges.add_argument(
+        '--no-badges', action='store_false', dest='group',
+        help='Opposite of --badges.')
+
+    settings_group.add_argument(
+        '--badges-max', metavar='n', type=int,
+        default=settings['badges']['max_count'],
+        help='Maximum number of badges per user.')
+
     channel_group = parser.add_argument_group(
         'Channel Mode Settings',
         'These options will only work with -c/--channel.')
     channel_group.add_argument(
         '--video-min', metavar='ID', type=int, default=0,
         help='ID of the earliest VOD to download.')
     channel_group.add_argument(
@@ -180,19 +207,22 @@
 settings['directory'] = args.directory
 settings['filename_format'] = args.filename_format
 settings['max_width'] = args.max_width
 settings['subtitle_duration'] = args.subtitle_duration
 settings['dynamic_duration']['enabled'] = args.dynamic
 settings['dynamic_duration']['max'] = args.dynamic_duration_max
 settings['dynamic_duration']['max_length'] = args.dynamic_duration_max_length
+settings['millisecond_separator'] = args.millisecond_separator
 settings['group_repeating_emotes']['enabled'] = args.group
 settings['group_repeating_emotes']['threshold'] = args.group_threshold
 settings['group_repeating_emotes']['collocations'] = args.group_collocations
 settings['group_repeating_emotes']['collocations_threshold'] = args.group_collocations_threshold
 settings['group_repeating_emotes']['format'] = args.group_format
+settings['badges']['enabled'] = args.badges
+settings['badges']['max_count'] = args.badges_max
 settings['video_types'] = args.video_types
 
 
 #
 # Post-init arguments
 #
```

### Comparing `tdh-tcd-2.5.0/tcd/subtitles.py` & `tdh-tcd-2.5.1/tcd/subtitles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 from __future__ import unicode_literals
 
 import io
 import os
+import re
 import textwrap
 
 from datetime import timedelta, datetime as dtt
 
 from .settings import settings
+from .twitch import Messages
 
 
 class Subtitle(object):
-    @staticmethod
-    def new_file(video_id, format):
-        if not os.path.exists(settings['directory']):
-            os.makedirs(settings['directory'])
+    def __init__(self, filename: str):
+        if not os.path.exists(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
 
-        filename = settings['filename_format'].format(
-            directory=settings['directory'],
-            video_id=video_id,
-            format=format
-        )
-
-        return io.open(filename, mode='w+', encoding='UTF8')
-
-    def __init__(self, video_id, format):
-        self.file = self.new_file(video_id, format)
+        self.file = io.open(filename, mode='w+', encoding='UTF8')
 
     @staticmethod
     def _duration(msg):
         T_MIN = settings['subtitle_duration']
         T_MAX = settings['dynamic_duration']['max']
         MSG_MAX = settings['dynamic_duration']['max_length']
 
@@ -39,15 +28,15 @@
             part = (MSG_MAX - min(len(msg), MSG_MAX)) / MSG_MAX
             return T_MAX - (T_MAX - T_MIN) * part
         else:
             return T_MIN
 
     @staticmethod
     def ftime(seconds: float) -> str:
-        t = dtt.strptime("00:00", "%H:%M") + timedelta(seconds=seconds)
+        t = dtt.strptime('00:00', '%H:%M') + timedelta(seconds=seconds)
         ts = dtt.strftime(t, '%H:%M:%S.%f')
         return ts[1:] if ts.startswith('00') else ts
 
     @staticmethod
     def wrap(username, text):
         max_width = settings['max_width']
         full_text = username + ': ' + text
@@ -63,16 +52,16 @@
 
     def close(self):
         self.file.flush()
         self.file.close()
 
 
 class SubtitlesASS(Subtitle):
-    def __init__(self, video_id, format="ass"):
-        super(SubtitlesASS, self).__init__(video_id, format)
+    def __init__(self, filename: str):
+        super(SubtitlesASS, self).__init__(filename)
 
         self.line = settings['ssa_events_line_format'] + '\n'
 
         self.file.writelines([
             '[Script Info]\n',
             'PlayResX: 1280\n',
             'PlayResY: 720\n',
@@ -112,66 +101,87 @@
             end=self.ftime(offset + self._duration(comment.message)),
             user=self._color(comment.user, color),
             message=self.wrap(comment.user, comment.message)
         ))
 
 
 class SubtitlesSRT(Subtitle):
-    def __init__(self, video_id):
-        super(SubtitlesSRT, self).__init__(video_id, "srt")
+    def __init__(self, filename: str):
+        super(SubtitlesSRT, self).__init__(filename)
         self.count = 0
 
     @staticmethod
     def ftime(seconds):
         return Subtitle.ftime(seconds)[:-3].replace('.', ',')
 
     def add(self, comment):
         time = comment.offset
 
         self.file.write(str(self.count) + '\n')
-        self.file.write("{start} --> {end}\n".format(
+        self.file.write('{start} --> {end}\n'.format(
             start=self.ftime(time),
             end=self.ftime(time + self._duration(comment.message))
         ))
-        self.file.write("{user}: {message}\n\n".format(
+        self.file.write('{user}: {message}\n\n'.format(
             user=comment.user,
             message=comment.message
         ))
 
         self.count += 1
 
 
 class SubtitlesIRC(Subtitle):
-    def __init__(self, video_id):
-        super(SubtitlesIRC, self).__init__(video_id, "irc")
+    def __init__(self, filename: str):
+        super(SubtitlesIRC, self).__init__(filename)
 
     @staticmethod
     def ftime(seconds):
-        return Subtitle.ftime(seconds)[:-3].replace('.', ',')
+        return Subtitle.ftime(seconds)[:-3].replace('.', settings['millisecond_separator'])
 
     def add(self, comment):
-        self.file.write("[{start}] <{user}> {message}\n".format(
+        self.file.write('[{start}] <{badge}{user}> {message}\n'.format(
             start=self.ftime(comment.offset),
+            badge=comment.badge,
             user=comment.user,
             message=comment.message
         ))
 
 
 class SubtitleWriter:
-    def __init__(self, video_id):
+    @staticmethod
+    def clean_filename(string, valid_filename_regex=re.compile(r'(?u)[^-\w.()\[\]{}@%! ]')):
+        return re.sub(valid_filename_regex, '', string.strip())
+
+    @classmethod
+    def filename(cls, video: Messages, ext: str) -> str:
+        # TODO: make time configurable
+        time_str = str(video.created_at.replace(microsecond=0).replace(tzinfo=None).isoformat())
+
+        return settings['filename_format'].format(
+            directory=settings['directory'],
+            video_id=video.video_id,
+            format=ext,
+            user_name=cls.clean_filename(video.creator_name),
+            title=cls.clean_filename(video.title),
+            created_at=cls.clean_filename(time_str)
+        )
+
+    def __init__(self, video: Messages):
         self.drivers = set()
 
-        for format in settings['formats']:
-            if format in ("ass", "ssa"):
-                self.drivers.add(SubtitlesASS(video_id, format))
+        for ext in settings['formats']:
+            filename = self.filename(video, ext)
+
+            if ext in ('ass', 'ssa'):
+                self.drivers.add(SubtitlesASS(filename))
 
-            if format == "srt":
-                self.drivers.add(SubtitlesSRT(video_id))
+            if ext == 'srt':
+                self.drivers.add(SubtitlesSRT(filename))
 
-            if format == "irc":
-                self.drivers.add(SubtitlesIRC(video_id))
+            if ext == 'irc':
+                self.drivers.add(SubtitlesIRC(filename))
 
     def add(self, comment):
         [driver.add(comment) for driver in self.drivers]
 
     def close(self):
         [driver.close() for driver in self.drivers]
```

### Comparing `tdh-tcd-2.5.0/tcd/twitch.py` & `tdh-tcd-2.5.1/tcd/twitch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 from time import sleep
 from iso8601 import parse_date as parse8601
 from progressbar import ProgressBar
 from requests import Session
 from requests.adapters import HTTPAdapter
-from requests.packages.urllib3 import Retry
+from urllib3 import Retry
 
 from .settings import settings
 
 
 client = Session()
-client.headers["Acccept"] = "application/vnd.twitchtv.v5+json"
-client.headers["Client-ID"] = settings['client_id']
+client.headers['Acccept'] = '*/*'
+client.headers['Client-ID'] = settings['client_id']
 
 # Configure retries for all requests
 retries = Retry(connect=5, read=2, redirect=5)
 http_adapter = HTTPAdapter(max_retries=retries)
-client.mount("http://", http_adapter)
-client.mount("https://", http_adapter)
+client.mount('http://', http_adapter)
+client.mount('https://', http_adapter)
 
 
 def gql(query: str):
     res = client.post('https://gql.twitch.tv/gql', json={'query': query})
 
     if res.status_code == 200:
         return res.json()
@@ -79,14 +76,31 @@
                 words[pos + count * len(chunk):]
 
         return ' '.join(words)
 
     def __init__(self, comment):
         self.user = comment['commenter']['displayName']
 
+        if settings['badges']['enabled']:
+            badge_ids = [badge['setID']
+                         for badge in comment['commenter']['displayBadges']]
+
+            badges = [val
+                      for key, val in settings['badges']['map'].items()
+                      if key in badge_ids]
+
+            max_count = settings['badges']['max_count']
+            if max_count >= 1:
+                if len(badges) > max_count:
+                    badges = badges[0:max_count]
+
+            self.badge = ''.join(badges)
+        else:
+            self.badge = ''
+
         group_prefs = settings.get('group_repeating_emotes')
 
         message = ''.join(frag['text']
                           for frag in comment['message']['fragments']).strip()
 
         if group_prefs['enabled'] is True:
             self.message = self.group(message, **group_prefs)
@@ -96,49 +110,63 @@
         self.offset = comment['contentOffsetSeconds']
 
         if comment['message']['userColor']:
             self.color = comment['message']['userColor'][1:]
         else:
             self.color = 'FFFFFF'
 
+    def hash(self) -> int:
+        return hash((self.offset, self.user, self.message))
 
 class Messages(object):
     def __init__(self, video_id):
         self.video_id = video_id
 
         video = gql(f'''
             query {{
                 video(id: {video_id}) {{
+                    creator {{
+                        displayName
+                        id
+                    }}
                     createdAt
                     lengthSeconds
+                    title
                 }}
             }}
         ''')
 
         self.created_at = parse8601(video['data']['video']['createdAt'])
         self.duration = video['data']['video']['lengthSeconds']
+        self.title = video['data']['video']['title']
+        self.creator_name = video['data']['video']['creator']['displayName']
+        self.creator_id = video['data']['video']['creator']['id']
 
         if settings.get('display_progress') in [None, True]:
             self.progressbar = ProgressBar(max_value=self.duration)
     
     def __iter__(self):
         hasNextPage = True
         cursor = None
+        hashes = set()
 
         while hasNextPage:
             res = gql(f'''
                 query {{
                     video(id: "{self.video_id}") {{
-                        comments{f'(after: "{cursor}")' if cursor else ''} {{
+                        comments{f'(contentOffsetSeconds: {cursor})' if cursor else ''} {{
                             edges {{
                                 cursor
                                 node {{
                                     commenter {{
                                         displayName
                                         login
+                                        displayBadges(channelID: {self.creator_id}) {{
+                                            setID
+                                        }}
                                     }}
                                     createdAt
                                     contentOffsetSeconds
                                     message {{
                                         fragments {{
                                             text
                                         }}
@@ -155,25 +183,34 @@
                 }}
             ''')
 
             comments = res['data']['video']['comments']
             hasNextPage = comments['pageInfo']['hasNextPage']
 
             for comment in comments['edges']:
-                cursor = comment['cursor']
+                cursor = comment['node']['contentOffsetSeconds']
 
                 # Calculate more accurate offset
                 ts = parse8601(comment['node']['createdAt'])
                 offset = (ts - self.created_at).total_seconds()
                 comment['node']['contentOffsetSeconds'] = offset
 
                 try:
-                    yield Message(comment['node'])
+                    msg = Message(comment['node'])
                 except Exception:
                     continue
+            
+                msg_hash = msg.hash()
+
+                if msg_hash in hashes:
+                    continue
+                else:
+                    hashes.add(msg_hash)
+
+                yield msg
 
             if self.progressbar:
                 ts = comments['edges'][-1]['node']['contentOffsetSeconds']
                 self.progressbar.update(min(self.duration, ts))
 
             if settings['cooldown'] > 0:
                 sleep(settings['cooldown'] / 1000)
```

### Comparing `tdh-tcd-2.5.0/tdh_tcd.egg-info/PKG-INFO` & `tdh-tcd-2.5.1/tdh_tcd.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.0
+Version: 2.5.1
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Twitch Chat Downloader [![PyPI version](https://badge.fury.io/py/tdh-tcd.svg)](https://badge.fury.io/py/tdh-tcd)
 
 Neat python script to download chat messages from past broadcasts
 
 ## Requirements
 
-* [Python 2.7 or 3.4+](https://www.python.org/downloads/)
+* [Python 3.6+](https://www.python.org/downloads/)
 * [pip](https://pip.pypa.io/en/stable/installing/)
 * [python-requests](http://docs.python-requests.org/en/master/user/install/)
 
 ## Installation and usage
 
 There are multiple ways to install this script.
 
@@ -62,24 +61,29 @@
 | cooldown | *int* | `--cooldown` | Delay (in milliseconds) between API calls. |
 | display_progress | *bool* | `--[no-]progress` | Display animated progress bar in terminal. |
 | formats | *str[]* | `-f/--formats` | List of formats to download. See Formats table below. |
 | directory | *str* | `-t`/`--directory` | Name of directory to save all generated files. |
 | filename_format | *str* | `--filename-format` | Full format of generated filenames. Possible arguments: `directory`, `video_id` and `format`. |
 | max_width | *int* | `--max-width` | Add line breaks to fit messages into specified width. Note: Implemented only for SSA/ASS subtitles. |
 | subtitle_duration | *int* | `--subtitle-duration` | Duration (in seconds) of each line of subtitles. |
-| dynamic_duration | *obj* |  | Convert `Kappa Kappa Kappa` to `Kappa x3`. |
-| —.enabled | *bool* | `--[no-]dynamic-duration` | Increase subtitle duration based on message length. |
+| dynamic_duration | *obj* |  | Increase subtitle duration based on message length. |
+| —.enabled | *bool* | `--[no-]dynamic-duration` | Enable or disable this function. |
 | —.max | *int* | `--dynamic-duration-max` | Maximum duration of subtitle message. |
 | —.max_length | *int* | `--dynamic-duration-max-length` | Maximum length of subtitle message. |
+| millisecond_separator | *str* | `--millisecond-separator` | Separator between seconds and milliseconds in timestamps (IRC only). |
 | group_repeating_emotes | *obj* |  | Convert `Kappa Kappa Kappa` to `Kappa x3`. |
 | —.enabled | *bool* | `--[no-]group` | Enable or disable this function. |
 | —.threshold | *int* | `--group-threshold` | Number of repeating emotes to trigger this function. |
 | —.collocations | *int* | `--group-collocations` | Maximum number of words in repeating collocations (default: 1, more is slower). |
 | —.collocations_threshold | *int* | `--group-collocations-threshold` | Same logic as in —.threshold, but applies only to repeating collocations. |
 | —.format | *str* | `--group-format` | Customize format of replaced emotes. |
+| badges | *obj* |  | Add badges before the username (IRC only). |
+| —.enabled | *bool* | `--[no-]badges` | Enable or disable this function. |
+| —.max_count | *int* | `--badges-max` | Only show the first N badges (default: 1) |
+| —.map | *obj* | | Configure which symbol corresponds to a specific badge. |
 | video_types | *str* | `--video-types` | Comma-separated list of VOD types to detect in Channel Mode. (see [broadcast_type](https://dev.twitch.tv/docs/v5/reference/channels/#get-channel-videos)) |
 
 ## Formats
 
 | Format | Description |
 | ------ | ----------- |
 | `ass` or `ssa` | Advanced SubStation Alpha |
```

