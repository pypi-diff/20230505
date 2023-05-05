# Comparing `tmp/transcribe-anything-2.1.2.tar.gz` & `tmp/transcribe-anything-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.1.2.tar", last modified: Mon Mar 20 23:50:31 2023, max compression
+gzip compressed data, was "transcribe-anything-2.2.0.tar", last modified: Fri May  5 03:40:15 2023, max compression
```

## Comparing `transcribe-anything-2.1.2.tar` & `transcribe-anything-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 23:50:31.372371 transcribe-anything-2.1.2/
--rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.1.2/LICENSE
--rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8650 2023-03-20 23:50:31.371368 transcribe-anything-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7632 2023-03-20 23:49:40.000000 transcribe-anything-2.1.2/README.md
--rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.1.2/requirements.testing.txt
--rw-rw-rw-   0        0        0       63 2023-03-20 23:48:49.000000 transcribe-anything-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 23:50:31.373369 transcribe-anything-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3043 2023-03-20 23:49:52.000000 transcribe-anything-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 23:50:31.331370 transcribe-anything-2.1.2/transcribe_anything/
--rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.1.2/transcribe_anything/__init__.py
--rw-rw-rw-   0        0        0     4657 2023-03-20 23:48:49.000000 transcribe-anything-2.1.2/transcribe_anything/api.py
--rw-rw-rw-   0        0        0     3071 2023-03-20 23:48:49.000000 transcribe-anything-2.1.2/transcribe_anything/audio.py
--rw-rw-rw-   0        0        0     2836 2023-03-20 23:48:49.000000 transcribe-anything-2.1.2/transcribe_anything/cmd.py
--rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.1.2/transcribe_anything/logger.py
--rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.1.2/transcribe_anything/parse_whisper_options.py
--rw-rw-rw-   0        0        0     1532 2022-12-09 00:33:26.000000 transcribe-anything-2.1.2/transcribe_anything/util.py
-drwxrwxrwx   0        0        0        0 2023-03-20 23:50:31.369368 transcribe-anything-2.1.2/transcribe_anything.egg-info/
--rw-rw-rw-   0        0        0     8650 2023-03-20 23:50:31.000000 transcribe-anything-2.1.2/transcribe_anything.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-03-20 23:50:31.000000 transcribe-anything-2.1.2/transcribe_anything.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 23:50:31.000000 transcribe-anything-2.1.2/transcribe_anything.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-03-20 23:50:31.000000 transcribe-anything-2.1.2/transcribe_anything.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-03-20 23:50:31.000000 transcribe-anything-2.1.2/transcribe_anything.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-03-20 23:50:31.000000 transcribe-anything-2.1.2/transcribe_anything.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 03:40:15.249953 transcribe-anything-2.2.0/
+-rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8827 2023-05-05 03:40:15.248951 transcribe-anything-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7808 2023-05-05 03:39:32.000000 transcribe-anything-2.2.0/README.md
+-rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.2.0/requirements.testing.txt
+-rw-rw-rw-   0        0        0       63 2023-03-20 23:48:49.000000 transcribe-anything-2.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 03:40:15.249953 transcribe-anything-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3109 2023-05-05 03:37:04.000000 transcribe-anything-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:40:15.203954 transcribe-anything-2.2.0/tests/
+-rw-rw-rw-   0        0        0     2789 2023-05-05 03:33:34.000000 transcribe-anything-2.2.0/tests/test_transcribe_anything.py
+-rw-rw-rw-   0        0        0      449 2022-12-01 20:48:45.000000 transcribe-anything-2.2.0/tests/test_whisper.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:40:15.218954 transcribe-anything-2.2.0/transcribe_anything/
+-rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.2.0/transcribe_anything/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-05-05 02:50:27.000000 transcribe-anything-2.2.0/transcribe_anything/api.py
+-rw-rw-rw-   0        0        0     3071 2023-03-20 23:48:49.000000 transcribe-anything-2.2.0/transcribe_anything/audio.py
+-rw-rw-rw-   0        0        0     2836 2023-03-20 23:48:49.000000 transcribe-anything-2.2.0/transcribe_anything/cmd.py
+-rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.2.0/transcribe_anything/logger.py
+-rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.2.0/transcribe_anything/parse_whisper_options.py
+-rw-rw-rw-   0        0        0     1532 2022-12-09 00:33:26.000000 transcribe-anything-2.2.0/transcribe_anything/util.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:40:15.246951 transcribe-anything-2.2.0/transcribe_anything.egg-info/
+-rw-rw-rw-   0        0        0     8827 2023-05-05 03:40:14.000000 transcribe-anything-2.2.0/transcribe_anything.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-05-05 03:40:15.000000 transcribe-anything-2.2.0/transcribe_anything.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 03:40:14.000000 transcribe-anything-2.2.0/transcribe_anything.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-05-05 03:40:14.000000 transcribe-anything-2.2.0/transcribe_anything.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-05-05 03:40:14.000000 transcribe-anything-2.2.0/transcribe_anything.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-05 03:40:14.000000 transcribe-anything-2.2.0/transcribe_anything.egg-info/top_level.txt
```

### Comparing `transcribe-anything-2.1.2/LICENSE` & `transcribe-anything-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.1.2/PKG-INFO` & `transcribe-anything-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.1.2
+Version: 2.2.0
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -37,15 +37,15 @@
 
 ```bash
 > pip install transcribe-anything
 # Outputs the srt, vtt and txt files in title/out.vtt
 > transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
 ```
 
-# Usage (GPU Accelerated Version)
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
 
 ```bash
 > curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
 # Outputs the srt, vtt and txt files in title/out.vtt
 > transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
 ```
 
@@ -163,14 +163,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
   * 2.0.13: Now works with python 3.9
   * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
   * 2.0.11: Automatically deletes files in the out directory if they already exist.
   * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
```

### Comparing `transcribe-anything-2.1.2/README.md` & `transcribe-anything-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ```bash
 > pip install transcribe-anything
 # Outputs the srt, vtt and txt files in title/out.vtt
 > transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
 ```
 
-# Usage (GPU Accelerated Version)
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
 
 ```bash
 > curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
 # Outputs the srt, vtt and txt files in title/out.vtt
 > transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
 ```
 
@@ -143,14 +143,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
   * 2.0.13: Now works with python 3.9
   * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
   * 2.0.11: Automatically deletes files in the out directory if they already exist.
   * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
```

### Comparing `transcribe-anything-2.1.2/setup.py` & `transcribe-anything-2.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Uses whisper AI to transcribe speach from video and audio files. "
     "Also accepts urls for youtube, rumble, bitchute, clear file, etc."
 )
 URL = "https://github.com/zackees/transcribe-anything"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "2.1.2"
+VERSION = "2.2.0"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="r") as fd:
     README = fd.read()
 
 
 def parse_requirements(filename):
@@ -92,14 +92,15 @@
         "Operating System :: MacOS :: MacOS X",
         "Environment :: Console",
     ],
     install_requires=REQUIREMENTS,
     entry_points={
         "console_scripts": [
             "transcribe_anything = transcribe_anything.cmd:main",
+            "transcribe-anything = transcribe_anything.cmd:main",
         ],
     },
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     package_data={},
     include_package_data=True,
     cmdclass={
         "upload": UploadCommand,
```

### Comparing `transcribe-anything-2.1.2/transcribe_anything/api.py` & `transcribe-anything-2.2.0/transcribe_anything/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     """
     basename = os.path.basename(url_or_file)
     if not basename or basename == ".":  # if url_or_file is a directory
         # Defense against paths with a trailing /, for example:
         # https://example.com/, which will yield a basename of "".
         basename = os.path.basename(os.path.dirname(url_or_file))
         basename = sanitize_path(basename)
+    output_dir_was_generated = False
     if output_dir is None:
+        output_dir_was_generated = True
         if url_or_file.startswith("http"):
             # Try and the title of the video using yt-dlp
             # If that fails, use the basename of the url
             try:
                 yt_dlp = subprocess.run(
                     ["yt-dlp", "--get-title", url_or_file],
                     capture_output=True,
@@ -56,14 +58,16 @@
                 output_dir = "text_" + yt_dlp.stdout.strip()
                 output_dir = sanitize_path(output_dir[:80].strip())
             except Exception:
                 log_error("yt-dlp failed to get title, using basename instead.")
                 output_dir = basename
         else:
             output_dir = os.path.splitext(basename)[0]
+    if output_dir_was_generated and language is not None:
+        output_dir = os.path.join(output_dir, language)
     if os.path.exists(output_dir):
         shutil.rmtree(output_dir)
     os.makedirs(output_dir, exist_ok=True)
     tmp_mp3 = os.path.join(output_dir, "out.mp3")
     fetch_audio(url_or_file, tmp_mp3)
     assert os.path.exists(tmp_mp3), f"Path {tmp_mp3} doesn't exist."
     device = device or get_computing_device()
```

### Comparing `transcribe-anything-2.1.2/transcribe_anything/audio.py` & `transcribe-anything-2.2.0/transcribe_anything/audio.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.1.2/transcribe_anything/cmd.py` & `transcribe-anything-2.2.0/transcribe_anything/cmd.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.1.2/transcribe_anything/logger.py` & `transcribe-anything-2.2.0/transcribe_anything/logger.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.1.2/transcribe_anything/parse_whisper_options.py` & `transcribe-anything-2.2.0/transcribe_anything/parse_whisper_options.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.1.2/transcribe_anything/util.py` & `transcribe-anything-2.2.0/transcribe_anything/util.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.1.2/transcribe_anything.egg-info/PKG-INFO` & `transcribe-anything-2.2.0/transcribe_anything.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.1.2
+Version: 2.2.0
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -37,15 +37,15 @@
 
 ```bash
 > pip install transcribe-anything
 # Outputs the srt, vtt and txt files in title/out.vtt
 > transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
 ```
 
-# Usage (GPU Accelerated Version)
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
 
 ```bash
 > curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
 # Outputs the srt, vtt and txt files in title/out.vtt
 > transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
 ```
 
@@ -163,14 +163,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
   * 2.0.13: Now works with python 3.9
   * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
   * 2.0.11: Automatically deletes files in the out directory if they already exist.
   * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
```

### Comparing `transcribe-anything-2.1.2/transcribe_anything.egg-info/SOURCES.txt` & `transcribe-anything-2.2.0/transcribe_anything.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.testing.txt
 requirements.txt
 setup.py
+tests/test_transcribe_anything.py
+tests/test_whisper.py
 transcribe_anything/__init__.py
 transcribe_anything/api.py
 transcribe_anything/audio.py
 transcribe_anything/cmd.py
 transcribe_anything/logger.py
 transcribe_anything/parse_whisper_options.py
 transcribe_anything/util.py
```

