# Comparing `tmp/skelly_synchronize-2023.5.1009.tar.gz` & `tmp/skelly_synchronize-2023.5.1010.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1009.tar", last modified: Tue May  2 20:29:30 2023, max compression
+gzip compressed data, was "skelly_synchronize-2023.5.1010.tar", last modified: Fri May  5 19:56:55 2023, max compression
```

## Comparing `skelly_synchronize-2023.5.1009.tar` & `skelly_synchronize-2023.5.1010.tar`

### file list

```diff
@@ -1,27 +1,36 @@
--rw-r--r--   0        0        0       65 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0      924 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/LICENSE
--rw-r--r--   0        0        0     2571 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/README.md
--rw-r--r--   0        0        0     1600 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/pyproject.toml
--rw-r--r--   0        0        0      111 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/setup.py
--rw-r--r--   0        0        0      976 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     1799 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0    18727 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0     1449 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0     1018 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/unit_tests.py
--rw-r--r--   0        0        0      577 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-02 20:29:14.965668 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     2048 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1871 2023-05-02 20:29:14.969669 skelly_synchronize-2023.5.1009/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3438 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1009/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.gitattributes
+-rw-r--r--   0        0        0      146 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.gitignore
+-rw-r--r--   0        0        0    34523 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/LICENSE
+-rw-r--r--   0        0        0     3030 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/README.md
+-rw-r--r--   0        0        0     1608 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/setup.py
+-rw-r--r--   0        0        0     1045 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     1961 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      821 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/debug_output.py
+-rw-r--r--   0        0        0     1557 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     2699 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     4536 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1799 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     4702 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      262 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1085 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0      656 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      847 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      577 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1061 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1340 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     2317 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1010/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1009/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.5.1010/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.5.1010/.github/workflows/python-testing.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,16 +18,20 @@
           # Optional - x64 or x86 architecture, defaults to x64
           architecture: 'x64'
           cache: 'pip'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
+      - name: Install FFmpeg
+        run: |
+          sudo apt-get update
+          sudo apt-get install -y ffmpeg
       - name: Run tests with pytest
         run: |
           pip install pytest
-          pytest skelly_synchronize/tests/unit_tests.py
+          pytest skelly_synchronize/tests
       - name: Upload pytest test results
         uses: actions/upload-artifact@v3
         with:
           name: pytest-results-3.9
           path: junit/test-results-3.9.xml
```

### Comparing `skelly_synchronize-2023.5.1009/.gitignore` & `skelly_synchronize-2023.5.1010/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/LICENSE` & `skelly_synchronize-2023.5.1010/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/README.md` & `skelly_synchronize-2023.5.1010/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 # Video Requirements
 
 The following requirements must be met for the script to function:
 
 1. Videos must have audio
 2. Videos must be in the same file format (default is ".mp4")
 3. Videos must have the exact same framerate (frames per second). There are often slight differences between brands/models of camera that lead to one camera's "60 fps" being different from another's. If your frame rates do not match, an error will be thrown.
-3. All videos in folder must have overlapping audio from the same real world event
+4. Videos must have the same audio sample rate. Most cameras record either 44100 or 48000 Hz, so there are not as much variation in audio sample rates as there are in video framerates.
+5. All videos in folder must have overlapping audio from the same real world event
+
+## Downsampling
+
+If you video frame rates or audio sample rates do not match, it is possible to downsample them in a separate tool like VLC to have matching frame rates and sample rates. This must be done *before* trying to synchronize the videos using skelly_synchronize.
 
 
 # How to run from source
 
 First clone this repository and pip install the `requirements.txt` file.
 
 Synchronize your videos by setting the path to your folder of raw videos and the file types of your videos into `skelly_synchronize.py`, lines 343-344, then run the file.
```

### Comparing `skelly_synchronize-2023.5.1009/pyproject.toml` & `skelly_synchronize-2023.5.1010/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -30,25 +30,26 @@
 "librosa",
 "PyQt6",
 "numpy",
 "scipy",
 "setuptools",
 "opencv-python",
 "deffcode",
+"toml",
 ] #add additional dependencies here - try to pin versions as minimally as possible
 
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1009"
+current_version = "v2023.05.1010"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1009"
+__version__ = "v2023.05.1010"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
@@ -20,10 +20,11 @@
 
 base_package_path = Path(__file__).parent
 print(f"adding base_package_path: {base_package_path} : to sys.path")
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from skelly_synchronize.system.default_paths import get_log_file_path
 from skelly_synchronize.system.logging_configuration import configure_logging
+from skelly_synchronize.skelly_synchronize import synchronize_videos
 
 
 configure_logging(log_file_path=get_log_file_path())
```

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1009/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.5.1010/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,13 +49,24 @@
     except Exception as e:
         logging.error(
             f"Error retrieving file name from path: {file_path}. Exception: {e}"
         )
         raise
 
 
+def name_synced_video(raw_video_filename: str) -> str:
+    """Take a raw video filename, remove the raw prefix if its there, and return the synced video filename"""
+    raw_video_filename = str(raw_video_filename)
+    if raw_video_filename.split("_")[0] == "raw":
+        synced_video_name = "synced_" + raw_video_filename[4:] + ".mp4"
+    else:
+        synced_video_name = "synced_" + raw_video_filename + ".mp4"
+
+    return synced_video_name
+
+
 def ensure_path_object(path: Union[str, Path]) -> Path:
     """Ensure the input is a Path object. If the input is a string, convert it to a Path object."""
     if not isinstance(path, Path):
         path = Path(path)
 
     return path
```

### Comparing `skelly_synchronize-2023.5.1009/PKG-INFO` & `skelly_synchronize-2023.5.1010/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1009
+Version: 2023.5.1010
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
@@ -13,14 +13,15 @@
 Requires-Dist: librosa
 Requires-Dist: PyQt6
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: setuptools
 Requires-Dist: opencv-python
 Requires-Dist: deffcode
+Requires-Dist: toml
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Provides-Extra: dev
 
@@ -39,15 +40,20 @@
 # Video Requirements
 
 The following requirements must be met for the script to function:
 
 1. Videos must have audio
 2. Videos must be in the same file format (default is ".mp4")
 3. Videos must have the exact same framerate (frames per second). There are often slight differences between brands/models of camera that lead to one camera's "60 fps" being different from another's. If your frame rates do not match, an error will be thrown.
-3. All videos in folder must have overlapping audio from the same real world event
+4. Videos must have the same audio sample rate. Most cameras record either 44100 or 48000 Hz, so there are not as much variation in audio sample rates as there are in video framerates.
+5. All videos in folder must have overlapping audio from the same real world event
+
+## Downsampling
+
+If you video frame rates or audio sample rates do not match, it is possible to downsample them in a separate tool like VLC to have matching frame rates and sample rates. This must be done *before* trying to synchronize the videos using skelly_synchronize.
 
 
 # How to run from source
 
 First clone this repository and pip install the `requirements.txt` file.
 
 Synchronize your videos by setting the path to your folder of raw videos and the file types of your videos into `skelly_synchronize.py`, lines 343-344, then run the file.
```

