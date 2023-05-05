# Comparing `tmp/ffmpeg-progress-yield-0.7.2.tar.gz` & `tmp/ffmpeg-progress-yield-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-progress-yield-0.7.2.tar", last modified: Sat Mar  4 19:31:28 2023, max compression
+gzip compressed data, was "ffmpeg-progress-yield-0.7.3.tar", last modified: Fri May  5 06:39:03 2023, max compression
```

## Comparing `ffmpeg-progress-yield-0.7.2.tar` & `ffmpeg-progress-yield-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-04 19:31:28.537713 ffmpeg-progress-yield-0.7.2/
--rw-r--r--   0 werner     (501) staff       (20)     2160 2023-03-04 19:31:27.000000 ffmpeg-progress-yield-0.7.2/CHANGELOG.md
--rw-r--r--   0 werner     (501) staff       (20)     1081 2021-03-01 12:29:03.000000 ffmpeg-progress-yield-0.7.2/LICENSE
--rw-r--r--   0 werner     (501) staff       (20)     9691 2023-03-04 19:31:28.537857 ffmpeg-progress-yield-0.7.2/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     6755 2023-02-24 19:48:47.000000 ffmpeg-progress-yield-0.7.2/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-04 19:31:28.535352 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/
--rw-r--r--   0 werner     (501) staff       (20)      103 2023-03-04 19:31:26.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     1279 2023-03-04 16:13:54.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)     7197 2023-03-04 19:29:23.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/ffmpeg_progress_yield.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-04 19:31:28.536516 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)     9691 2023-03-04 19:31:28.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      494 2023-03-04 19:31:28.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-03-04 19:31:28.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       78 2023-03-04 19:31:28.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-03-04 19:31:28.000000 ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      279 2023-03-04 19:31:28.538318 ffmpeg-progress-yield-0.7.2/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.2/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-04 19:31:28.537560 ffmpeg-progress-yield-0.7.2/test/
--rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.2/test/test.mp4
--rw-r--r--   0 werner     (501) staff       (20)     4203 2023-02-24 19:46:43.000000 ffmpeg-progress-yield-0.7.2/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.235857 ffmpeg-progress-yield-0.7.3/
+-rw-r--r--   0 werner     (501) staff       (20)     2242 2023-05-05 06:39:02.000000 ffmpeg-progress-yield-0.7.3/CHANGELOG.md
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.3/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)     9791 2023-05-05 06:39:03.236019 ffmpeg-progress-yield-0.7.3/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.3/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.233566 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/
+-rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-05 06:39:01.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     1279 2023-03-04 16:13:54.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     7196 2023-05-05 06:35:33.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/ffmpeg_progress_yield.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.234712 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)     9791 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-05 06:39:03.236380 ffmpeg-progress-yield-0.7.3/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.3/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.235533 ffmpeg-progress-yield-0.7.3/test/
+-rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.3/test/test.mp4
+-rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-05 06:37:46.000000 ffmpeg-progress-yield-0.7.3/test/test.py
```

### Comparing `ffmpeg-progress-yield-0.7.2/CHANGELOG.md` & `ffmpeg-progress-yield-0.7.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog
 
 
+## v0.7.3 (2023-05-05)
+
+* Update readme.
+
+* Add progress as percent, fixes #12.
+
+
 ## v0.7.2 (2023-03-04)
 
 * Do not print input information when probing, addresses #10.
 
 
 ## v0.7.1 (2023-02-24)
```

### Comparing `ffmpeg-progress-yield-0.7.2/LICENSE` & `ffmpeg-progress-yield-0.7.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Werner Robitza
+Copyright (c) 2021-2023 Werner Robitza
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ffmpeg-progress-yield-0.7.2/PKG-INFO` & `ffmpeg-progress-yield-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.2
+Version: 0.7.3
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -73,15 +73,15 @@
 ]
 
 ff = FfmpegProgress(cmd)
 for progress in ff.run_command_with_progress():
     print(f"{progress}/100")
 ```
 
-The command will yield the current progress in percent.
+The command will yield the current progress in percent as a float number.
 
 `run_command_with_progress` takes a `duration_override` argument where you can manually override the duration of the command in seconds. This is useful if your input doesn't have an implicit duration (e.g. if you use `testsrc`).
 
 If you have `tqdm` installed, you can create a fancy progress bar:
 
 ```python
 from tqdm import tqdm
@@ -165,15 +165,15 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## License
 
 The MIT License (MIT)
 
-Copyright (c) 2021-2022 Werner Robitza
+Copyright (c) 2021-2023 Werner Robitza
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -189,14 +189,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.3 (2023-05-05)
+
+* Update readme.
+
+* Add progress as percent, fixes #12.
+
+
 ## v0.7.2 (2023-03-04)
 
 * Do not print input information when probing, addresses #10.
 
 
 ## v0.7.1 (2023-02-24)
```

### Comparing `ffmpeg-progress-yield-0.7.2/README.md` & `ffmpeg-progress-yield-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ]
 
 ff = FfmpegProgress(cmd)
 for progress in ff.run_command_with_progress():
     print(f"{progress}/100")
 ```
 
-The command will yield the current progress in percent.
+The command will yield the current progress in percent as a float number.
 
 `run_command_with_progress` takes a `duration_override` argument where you can manually override the duration of the command in seconds. This is useful if your input doesn't have an implicit duration (e.g. if you use `testsrc`).
 
 If you have `tqdm` installed, you can create a fancy progress bar:
 
 ```python
 from tqdm import tqdm
@@ -143,15 +143,15 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## License
 
 The MIT License (MIT)
 
-Copyright (c) 2021-2022 Werner Robitza
+Copyright (c) 2021-2023 Werner Robitza
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/__main__.py` & `ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield/ffmpeg_progress_yield.py` & `ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/ffmpeg_progress_yield.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,29 +109,29 @@
                 "Callback must be a function that accepts only one argument"
             )
 
         self.stderr_callback = callback
 
     def run_command_with_progress(
         self, popen_kwargs=None, duration_override: Union[float, None] = None
-    ) -> Iterator[int]:
+    ) -> Iterator[float]:
         """
         Run an ffmpeg command, trying to capture the process output and calculate
         the duration / progress.
         Yields the progress in percent.
 
         Args:
             popen_kwargs (dict, optional): A dict to specify extra arguments to the popen call, e.g. { creationflags: CREATE_NO_WINDOW }
             duration_override (float, optional): The duration in seconds. If not specified, it will be calculated from the ffmpeg output.
 
         Raises:
             RuntimeError: If the command fails, an exception is raised.
 
         Yields:
-            Iterator[int]: A generator that yields the progress in percent.
+            Iterator[float]: A generator that yields the progress in percent.
         """
         if self.dry_run:
             return self.cmd
 
         total_dur: Union[None, int] = None
         if _uses_error_loglevel(self.cmd):
             total_dur = _probe_duration(self.cmd)
@@ -180,15 +180,15 @@
                     total_dur = int(duration_override * 1000)
                     continue
 
             if total_dur:
                 progress_time = FfmpegProgress.TIME_REGEX.search(stderr_line)
                 if progress_time:
                     elapsed_time = to_ms(**progress_time.groupdict())
-                    yield int(elapsed_time / total_dur * 100)
+                    yield elapsed_time / total_dur * 100
 
         if self.process is None or self.process.returncode != 0:
             _pretty_stderr = "\n".join(stderr)
             raise RuntimeError(f"Error running command {self.cmd}: {_pretty_stderr}")
 
         yield 100
         self.process = None
```

### Comparing `ffmpeg-progress-yield-0.7.2/ffmpeg_progress_yield.egg-info/PKG-INFO` & `ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.2
+Version: 0.7.3
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -73,15 +73,15 @@
 ]
 
 ff = FfmpegProgress(cmd)
 for progress in ff.run_command_with_progress():
     print(f"{progress}/100")
 ```
 
-The command will yield the current progress in percent.
+The command will yield the current progress in percent as a float number.
 
 `run_command_with_progress` takes a `duration_override` argument where you can manually override the duration of the command in seconds. This is useful if your input doesn't have an implicit duration (e.g. if you use `testsrc`).
 
 If you have `tqdm` installed, you can create a fancy progress bar:
 
 ```python
 from tqdm import tqdm
@@ -165,15 +165,15 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## License
 
 The MIT License (MIT)
 
-Copyright (c) 2021-2022 Werner Robitza
+Copyright (c) 2021-2023 Werner Robitza
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -189,14 +189,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.3 (2023-05-05)
+
+* Update readme.
+
+* Add progress as percent, fixes #12.
+
+
 ## v0.7.2 (2023-03-04)
 
 * Do not print input information when probing, addresses #10.
 
 
 ## v0.7.1 (2023-02-24)
```

### Comparing `ffmpeg-progress-yield-0.7.2/setup.py` & `ffmpeg-progress-yield-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.2/test/test.mp4` & `ffmpeg-progress-yield-0.7.3/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.2/test/test.py` & `ffmpeg-progress-yield-0.7.3/test/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import subprocess
 import sys
 
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), "../"))
 
 from ffmpeg_progress_yield import FfmpegProgress  # noqa: E402
 
-
 _TEST_ASSET = os.path.join(os.path.dirname(__file__), "test.mp4")
 
 
 class TestLibrary:
     cmd = [
         "ffmpeg",
         "-i",
@@ -49,23 +48,23 @@
             assert progress >= elapsed
             elapsed = progress
         # assert that we get 100% progress
         assert elapsed == 100
 
     def test_unknown_dur(self):
         ff = FfmpegProgress(TestLibrary.unknown_dur_cmd)
-        progresses = set([0])
+        progresses = set([0.0])
         for progress in ff.run_command_with_progress():
             progresses.add(progress)
         # assert that we get only 0 and 100% progress since we have no implicit duration
         assert list(progresses) == [0, 100]
 
     def test_manual_dur(self):
         ff = FfmpegProgress(TestLibrary.unknown_dur_cmd)
-        progresses = set([0])
+        progresses = set([0.0])
         for progress in ff.run_command_with_progress(duration_override=5):
             progresses.add(progress)
         # assert that we get more than just 0 and 100
         assert len(progresses) > 2
 
     def test_getting_stderr(self):
         ff = FfmpegProgress(TestLibrary.cmd)
@@ -139,8 +138,8 @@
             "fast",
             "-f",
             "null",
             "/dev/null",
         ]
         ret = subprocess.run(cmd, capture_output=True, universal_newlines=True)
         assert "0/100" in ret.stderr
-        assert "100/100" in ret.stderr
+        assert "100.0/100" in ret.stderr or "100/100" in ret.stderr
```

