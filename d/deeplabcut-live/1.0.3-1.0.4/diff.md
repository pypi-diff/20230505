# Comparing `tmp/deeplabcut_live-1.0.3.tar.gz` & `tmp/deeplabcut_live-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplabcut_live-1.0.3.tar", max compression
+gzip compressed data, was "deeplabcut_live-1.0.4.tar", max compression
```

## Comparing `deeplabcut_live-1.0.3.tar` & `deeplabcut_live-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0    34775 2022-06-21 11:22:48.969606 deeplabcut_live-1.0.3/LICENSE
--rw-r--r--   0        0        0    12537 2023-01-27 18:21:22.067708 deeplabcut_live-1.0.3/README.md
--rw-r--r--   0        0        0      334 2022-06-21 11:22:48.976717 deeplabcut_live-1.0.3/dlclive/__init__.py
--rw-r--r--   0        0        0    25227 2022-06-21 11:22:48.976913 deeplabcut_live-1.0.3/dlclive/benchmark.py
--rwxr-xr-x   0        0        0     2755 2023-01-27 18:21:22.068262 deeplabcut_live-1.0.3/dlclive/check_install/check_install.py
--rw-r--r--   0        0        0     3357 2022-06-21 11:22:48.977188 deeplabcut_live-1.0.3/dlclive/display.py
--rw-r--r--   0        0        0    16072 2022-06-21 11:22:48.977341 deeplabcut_live-1.0.3/dlclive/dlclive.py
--rw-r--r--   0        0        0      345 2022-06-21 11:22:48.977425 deeplabcut_live-1.0.3/dlclive/exceptions.py
--rw-r--r--   0        0        0     3276 2022-06-21 11:22:48.977522 deeplabcut_live-1.0.3/dlclive/graph.py
--rw-r--r--   0        0        0     3259 2022-06-21 11:22:48.977634 deeplabcut_live-1.0.3/dlclive/pose.py
--rw-r--r--   0        0        0     1749 2022-06-21 11:22:48.977766 deeplabcut_live-1.0.3/dlclive/processor/README.md
--rw-r--r--   0        0        0      238 2022-06-21 11:22:48.977857 deeplabcut_live-1.0.3/dlclive/processor/__init__.py
--rw-r--r--   0        0        0     4263 2022-06-21 11:22:48.977971 deeplabcut_live-1.0.3/dlclive/processor/kalmanfilter.py
--rw-r--r--   0        0        0      559 2022-06-21 11:22:48.978058 deeplabcut_live-1.0.3/dlclive/processor/processor.py
--rw-r--r--   0        0        0     4802 2022-06-21 11:22:48.978187 deeplabcut_live-1.0.3/dlclive/utils.py
--rw-r--r--   0        0        0      194 2023-01-27 18:22:28.708112 deeplabcut_live-1.0.3/dlclive/version.py
--rw-r--r--   0        0        0     1407 2023-01-27 18:22:06.384284 deeplabcut_live-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 deeplabcut_live-1.0.3/setup.py
--rw-r--r--   0        0        0    14024 1970-01-01 00:00:00.000000 deeplabcut_live-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34775 2023-05-05 17:26:40.321495 deeplabcut_live-1.0.4/LICENSE
+-rw-r--r--   0        0        0    12537 2023-05-05 17:26:40.321495 deeplabcut_live-1.0.4/README.md
+-rw-r--r--   0        0        0      334 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/__init__.py
+-rw-r--r--   0        0        0    25227 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/benchmark.py
+-rwxr-xr-x   0        0        0     2882 2023-05-05 17:38:49.898075 deeplabcut_live-1.0.4/dlclive/check_install/check_install.py
+-rw-r--r--   0        0        0     3357 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/display.py
+-rw-r--r--   0        0        0    16072 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/dlclive.py
+-rw-r--r--   0        0        0      345 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/exceptions.py
+-rw-r--r--   0        0        0     3276 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/graph.py
+-rw-r--r--   0        0        0     3259 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/pose.py
+-rw-r--r--   0        0        0     1749 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/processor/README.md
+-rw-r--r--   0        0        0      238 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/processor/__init__.py
+-rw-r--r--   0        0        0     4263 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/processor/kalmanfilter.py
+-rw-r--r--   0        0        0      559 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/processor/processor.py
+-rw-r--r--   0        0        0     4802 2023-05-05 17:26:40.333495 deeplabcut_live-1.0.4/dlclive/utils.py
+-rw-r--r--   0        0        0      194 2023-05-05 17:40:01.134671 deeplabcut_live-1.0.4/dlclive/version.py
+-rw-r--r--   0        0        0     1407 2023-05-05 17:40:55.067132 deeplabcut_live-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    14024 1970-01-01 00:00:00.000000 deeplabcut_live-1.0.4/PKG-INFO
```

### Comparing `deeplabcut_live-1.0.3/LICENSE` & `deeplabcut_live-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/README.md` & `deeplabcut_live-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/benchmark.py` & `deeplabcut_live-1.0.4/dlclive/benchmark.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/check_install/check_install.py` & `deeplabcut_live-1.0.4/dlclive/check_install/check_install.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,74 +15,71 @@
 import argparse
 from pathlib import Path
 from dlclibrary.dlcmodelzoo.modelzoo_download import (
     download_huggingface_model,
 )
 
 
+MODEL_NAME = "superanimal_quadruped"
+SNAPSHOT_NAME = "snapshot-700000.pb"
+
+
 def urllib_pbar(count, blockSize, totalSize):
     percent = int(count * blockSize * 100 / totalSize)
     outstr = f"{round(percent)}%"
     sys.stdout.write(outstr)
     sys.stdout.write("\b"*len(outstr))
     sys.stdout.flush()
 
 
-def main(display:bool=None):
+def main():
     parser = argparse.ArgumentParser(
         description="Test DLC-Live installation by downloading and evaluating a demo DLC project!")
     parser.add_argument('--nodisplay', action='store_false', help="Run the test without displaying tracking")
     args = parser.parse_args()
-
-    if display is None:
-        display = args.nodisplay
+    display = args.nodisplay
 
     if not display:
         print('Running without displaying video')
 
     # make temporary directory in $HOME
+    # TODO: why create this temp directory in $HOME?
     print("\nCreating temporary directory...\n")
     tmp_dir = Path().home() / 'dlc-live-tmp'
     tmp_dir.mkdir(mode=0o775,exist_ok=True)
 
     video_file = str(tmp_dir / 'dog_clip.avi')
     model_dir = tmp_dir / 'DLC_Dog_resnet_50_iteration-0_shuffle-0'
 
     # download dog test video from github:
+    # TODO: Should check if the video's already there before downloading it (should have been cloned with the files)
     print(f"Downloading Video to {video_file}")
     url_link = "https://github.com/DeepLabCut/DeepLabCut-live/blob/master/check_install/dog_clip.avi?raw=True"
     urllib.request.urlretrieve(url_link, video_file, reporthook=urllib_pbar)
 
-    # download exported dog model from DeepLabCut Model Zoo
-    if Path(model_dir / 'snapshot-75000.pb').exists():
+    # download model from the DeepLabCut Model Zoo
+    if Path(model_dir / SNAPSHOT_NAME).exists():
         print('Model already downloaded, using cached version')
     else:
         print("Downloading full_dog model from the DeepLabCut Model Zoo...")
-        download_huggingface_model("full_dog", model_dir)
+        download_huggingface_model(MODEL_NAME, model_dir)
 
     # assert these things exist so we can give informative error messages
-    assert Path(video_file).exists()
-    assert Path(model_dir / 'snapshot-75000.pb').exists()
+    assert Path(video_file).exists(), f"Missing video file {video_file}"
+    assert Path(model_dir / SNAPSHOT_NAME).exists(), f"Missing model file {model_dir / SNAPSHOT_NAME}"
 
     # run benchmark videos
     print("\n Running inference...\n")
-    # model_dir = "DLC_Dog_resnet_50_iteration-0_shuffle-0"
-    # print(video_file)
     benchmark_videos(str(model_dir), video_file, display=display, resize=0.5, pcutoff=0.25)
 
     # deleting temporary files
     print("\n Deleting temporary files...\n")
     try:
         shutil.rmtree(tmp_dir)
     except PermissionError:
         warnings.warn(f'Could not delete temporary directory {str(tmp_dir)} due to a permissions error, but otherwise dlc-live seems to be working fine!')
 
     print("\nDone!\n")
 
 
 if __name__ == "__main__":
-
-
-    display = args.nodisplay
-
-
-    main(display=args.nodisplay)
+    main()
```

### Comparing `deeplabcut_live-1.0.3/dlclive/display.py` & `deeplabcut_live-1.0.4/dlclive/display.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/dlclive.py` & `deeplabcut_live-1.0.4/dlclive/dlclive.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/graph.py` & `deeplabcut_live-1.0.4/dlclive/graph.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/pose.py` & `deeplabcut_live-1.0.4/dlclive/pose.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/processor/README.md` & `deeplabcut_live-1.0.4/dlclive/processor/README.md`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/processor/kalmanfilter.py` & `deeplabcut_live-1.0.4/dlclive/processor/kalmanfilter.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/processor/processor.py` & `deeplabcut_live-1.0.4/dlclive/processor/processor.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/dlclive/utils.py` & `deeplabcut_live-1.0.4/dlclive/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut_live-1.0.3/pyproject.toml` & `deeplabcut_live-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deeplabcut-live"
-version = "1.0.3"
+version = "1.0.4"
 description = "Class to load exported DeepLabCut networks and perform pose estimation on single frames (from a camera feed)"
 authors = ["A. & M. Mathis Labs <admin@deeplabcut.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/DeepLabCut/DeepLabCut-live"
 repository = "https://github.com/DeepLabCut/DeepLabCut-live"
 classifiers = [
```

### Comparing `deeplabcut_live-1.0.3/setup.py` & `deeplabcut_live-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,188 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['dlclive', 'dlclive.check_install', 'dlclive.processor']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Pillow>=8.0.0',
- 'colorcet>=3.0.0,<4.0.0',
- 'dlclibrary>=0.0.2',
- 'numpy>=1.20,<2.0',
- 'opencv-python-headless>=4.5,<5.0',
- 'pandas>=1.3,<2.0',
- 'py-cpuinfo>=5.0.0',
- 'ruamel.yaml>=0.17.20,<0.18.0',
- 'tables>=3.6,<4.0',
- 'tensorflow>=2.7.0,<=2.10',
- 'tqdm>=4.62.3,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['dlc-live-benchmark = dlclive.benchmark:main',
-                     'dlc-live-test = '
-                     'dlclive.check_install.check_install:main']}
-
-setup_kwargs = {
-    'name': 'deeplabcut-live',
-    'version': '1.0.3',
-    'description': 'Class to load exported DeepLabCut networks and perform pose estimation on single frames (from a camera feed)',
-    'long_description': '# DeepLabCut-live! SDK<img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1606082050387-M8M1CFI5DFUZCBAAUI0W/ke17ZwdGBToddI8pDm48kLuMKy7Ws6mFofiFehYynfdZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpzp2tFVMcEgqZM8QO7VXXQogrsLnYKC4n4YnYuHC1HMRWygQlqMNAoTF9HaycikLeg/DLClive.png?format=750w" width="350" title="DLC-live" alt="DLC LIVE!" align="right" vspace = "50">\n\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n![PyPI - Python Version](https://img.shields.io/pypi/v/deeplabcut-live)\n[![Downloads](https://pepy.tech/badge/deeplabcut-live)](https://pepy.tech/project/deeplabcut-live)\n[![Downloads](https://pepy.tech/badge/deeplabcut-live/month)](https://pepy.tech/project/deeplabcut-live)\n![Python package](https://github.com/DeepLabCut/DeepLabCut-live/workflows/Python%20package/badge.svg)\n[![GitHub stars](https://img.shields.io/github/stars/DeepLabCut/DeepLabCut-live.svg?style=social&label=Star)](https://github.com/DeepLabCut/DeepLabCut-live)\n[![GitHub forks](https://img.shields.io/github/forks/DeepLabCut/DeepLabCut-live.svg?style=social&label=Fork)](https://github.com/DeepLabCut/DeepLabCut-live)\n[![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&amp;url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fdeeplabcut.json&amp;query=%24.topic_list.tags.0.topic_count&amp;colorB=brightgreen&amp;&amp;suffix=%20topics&amp;logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/deeplabcut)\n[![Gitter](https://badges.gitter.im/DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)\n[![Twitter Follow](https://img.shields.io/twitter/follow/DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)\n\nThis package contains a [DeepLabCut](http://www.mousemotorlab.org/deeplabcut) inference pipeline for real-time applications that has minimal (software) dependencies. Thus, it is as easy to install as possible (in particular, on atypical systems like [NVIDIA Jetson boards](https://developer.nvidia.com/buy-jetson)).\n\n**Performance:** If you would like to see estimates on how your model should perform given different video sizes, neural network type, and hardware, please see: https://deeplabcut.github.io/DLC-inferencespeed-benchmark/\n\nIf you have different hardware, please consider submitting your results too! https://github.com/DeepLabCut/DLC-inferencespeed-benchmark\n\n**What this SDK provides:** This package provides a `DLCLive` class which enables pose estimation online to provide feedback. This object loads and prepares a DeepLabCut network for inference, and will return the predicted pose for single images. \n\nTo perform processing on poses (such as predicting the future pose of an animal given it\'s current pose, or to trigger external hardware like send TTL pulses to a laser for optogenetic stimulation), this object takes in a `Processor` object. Processor objects must contain two methods: process and save.\n\n- The `process` method takes in a pose, performs some processing, and returns processed pose.\n- The `save` method saves any valuable data created by or used by the processor\n\nFor more details and examples, see documentation [here](dlclive/processor/README.md).\n\n###### 🔥🔥🔥🔥🔥 Note :: alone, this object does not record video or capture images from a camera. This must be done separately, i.e. see our [DeepLabCut-live GUI](https://github.com/gkane26/DeepLabCut-live-GUI).🔥🔥🔥\n\n### News! \n- March 2022: DeepLabCut-Live! 1.0.2 supports poetry installation `poetry install deeplabcut-live`, thanks to PR #60.\n- March 2021: DeepLabCut-Live! [**version 1.0** is released](https://pypi.org/project/deeplabcut-live/), with support for tensorflow 1 and tensorflow 2!\n- Feb 2021: DeepLabCut-Live! was featured in **Nature Methods**: ["Real-time behavioral analysis"](https://www.nature.com/articles/s41592-021-01072-z)\n- Jan 2021: full **eLife** paper is published: ["Real-time, low-latency closed-loop feedback using markerless posture tracking"](https://elifesciences.org/articles/61909)\n- Dec 2020: we talked to **RTS Suisse Radio** about DLC-Live!: ["Capture animal movements in real time"](https://www.rts.ch/play/radio/cqfd/audio/capturer-les-mouvements-des-animaux-en-temps-reel?id=11782529)\n\n\n### Installation:\n\nPlease see our instruction manual to install on a [Windows or Linux machine](docs/install_desktop.md) or on a [NVIDIA Jetson Development Board](docs/install_jetson.md). Note, this code works with tensorflow (TF) 1 or TF 2 models, but TF requires that whatever version you exported your model with, you must import with the same version (i.e., export with TF1.13, then use TF1.13 with DlC-Live; export with TF2.3, then use TF2.3 with DLC-live).\n\n- available on pypi as: `pip install deeplabcut-live`\n\nNote, you can then test your installation by running:\n\n`dlc-live-test`\n\nIf installed properly, this script will i) create a temporary folder ii) download the full_dog model from the [DeepLabCut Model Zoo](http://www.mousemotorlab.org/dlc-modelzoo), iii) download a short video clip of a dog, and iv) run inference while displaying keypoints. v) remove the temporary folder.\n\n<img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1606081086014-TG9GWH63ZGGOO7K779G3/ke17ZwdGBToddI8pDm48kHiSoSToKfKUI9t99vKErWoUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYxCRW4BPu10St3TBAUQYVKcOoIGycwr1shdgJWzLuxyzjLbSRGBFFxjYMBr42yCvRK5HHsLZWtMlAHzDU294nCd/dlclivetest.png?format=1000w" width="650" title="DLC-live-test" alt="DLC LIVE TEST" align="center" vspace = "50">\n\n### Quick Start: instructions for use:\n\n1. Initialize `Processor` (if desired)\n2. Initialize the `DLCLive` object\n3. Perform pose estimation!\n\n```python\nfrom dlclive import DLCLive, Processor\ndlc_proc = Processor()\ndlc_live = DLCLive(<path to exported model directory>, processor=dlc_proc)\ndlc_live.init_inference(<your image>)\ndlc_live.get_pose(<your image>)\n```\n\n`DLCLive` **parameters:**\n\n  - `path` = string; full path to the exported DLC model directory\n  - `model_type` = string; the type of model to use for inference. Types include:\n      - `base` = the base DeepLabCut model\n      - `tensorrt` = apply [tensor-rt](https://developer.nvidia.com/tensorrt) optimizations to model\n      - `tflite` = use [tensorflow lite](https://www.tensorflow.org/lite) inference (in progress...)\n  - `cropping` = list of int, optional; cropping parameters in pixel number: [x1, x2, y1, y2]\n  - `dynamic` = tuple, optional; defines parameters for dynamic cropping of images\n      - `index 0` = use dynamic cropping, bool\n      - `index 1` = detection threshold, float\n      - `index 2` = margin (in pixels) around identified points, int\n  - `resize` = float, optional; factor by which to resize image (resize=0.5 downsizes both width and height of image by half). Can be used to downsize large images for faster inference\n  - `processor` = dlc pose processor object, optional\n  - `display` = bool, optional; display processed image with DeepLabCut points? Can be used to troubleshoot cropping and resizing parameters, but is very slow\n\n`DLCLive` **inputs:**\n\n  - `<path to exported model directory>` = path to the folder that has the `.pb` files that you acquire after running `deeplabcut.export_model`\n  - `<your image>` = is a numpy array of each frame\n\n\n### Benchmarking/Analyzing your exported DeepLabCut models\n\nDeepLabCut-live offers some analysis tools that allow users to peform the following operations on videos, from python or from the command line:\n\n1. Test inference speed across a range of image sizes, downsizing images by specifying the `resize` or `pixels` parameter. Using the `pixels` parameter will resize images to the desired number of `pixels`, without changing the aspect ratio. Results will be saved (along with system info) to a pickle file if you specify an output directory.\n##### python\n```python\ndlclive.benchmark_videos(\'/path/to/exported/model\', [\'/path/to/video1\', \'/path/to/video2\'], output=\'/path/to/output\', resize=[1.0, 0.75, \'0.5\'])\n```\n##### command line\n```\ndlc-live-benchmark /path/to/exported/model /path/to/video1 /path/to/video2 -o /path/to/output -r 1.0 0.75 0.5\n```\n\n2. Display keypoints to visually inspect the accuracy of exported models on different image sizes (note, this is slow and only for testing purposes):\n\n##### python\n```python\ndlclive.benchmark_videos(\'/path/to/exported/model\', \'/path/to/video\', resize=0.5, display=True, pcutoff=0.5, display_radius=4, cmap=\'bmy\')\n```\n##### command line\n```\ndlc-live-benchmark /path/to/exported/model /path/to/video -r 0.5 --display --pcutoff 0.5 --display-radius 4 --cmap bmy\n```\n\n3. Analyze and create a labeled video using the exported model and desired resize parameters. This option functions similar to `deeplabcut.benchmark_videos` and `deeplabcut.create_labeled_video` (note, this is slow and only for testing purposes).\n\n##### python\n```python\ndlclive.benchmark_videos(\'/path/to/exported/model\', \'/path/to/video\', resize=[1.0, 0.75, 0.5], pcutoff=0.5, display_radius=4, cmap=\'bmy\', save_poses=True, save_video=True)\n```\n##### command line\n```\ndlc-live-benchmark /path/to/exported/model /path/to/video -r 0.5 --pcutoff 0.5 --display-radius 4 --cmap bmy --save-poses --save-video\n```\n\n## License:\n\nThis project is licensed under the GNU AGPLv3. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, we ask that you please cite us! This software is available for licensing via the EPFL Technology Transfer Office (https://tto.epfl.ch/, info.tto@epfl.ch).\n\n## Community Support, Developers, & Help:\n\nThis is an actively developed package and we welcome community development and involvement.\n\n- If you want to contribute to the code, please read our guide [here](https://github.com/DeepLabCut/DeepLabCut/blob/master/CONTRIBUTING.md), which is provided at the main repository of DeepLabCut.\n\n- We are a community partner on the [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&amp;url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fdeeplabcut.json&amp;query=%24.topic_list.tags.0.topic_count&amp;colorB=brightgreen&amp;&amp;suffix=%20topics&amp;logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/deeplabcut). Please post help and support questions on the forum with the tag DeepLabCut. Check out their mission statement [Scientific Community Image Forum: A discussion forum for scientific image software](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3000340).\n\n- If you encounter a previously unreported bug/code issue, please post here (we encourage you to search issues first): https://github.com/DeepLabCut/DeepLabCut-live/issues\n\n- For quick discussions here: [![Gitter](https://badges.gitter.im/DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)\n\n### Reference:\n\nIf you utilize our tool, please [cite Kane et al, eLife 2020](https://elifesciences.org/articles/61909). The preprint is available here: https://www.biorxiv.org/content/10.1101/2020.08.04.236422v2\n\n```\n@Article{Kane2020dlclive,\n  author    = {Kane, Gary and Lopes, Gonçalo and Sanders, Jonny and Mathis, Alexander and Mathis, Mackenzie},\n  title     = {Real-time, low-latency closed-loop feedback using markerless posture tracking},\n  journal   = {eLife},\n  year      = {2020},\n}\n```\n\n',
-    'author': 'A. & M. Mathis Labs',
-    'author_email': 'admin@deeplabcut.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DeepLabCut/DeepLabCut-live',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
+Metadata-Version: 2.1
+Name: deeplabcut-live
+Version: 1.0.4
+Summary: Class to load exported DeepLabCut networks and perform pose estimation on single frames (from a camera feed)
+Home-page: https://github.com/DeepLabCut/DeepLabCut-live
+License: AGPL-3.0-or-later
+Author: A. & M. Mathis Labs
+Author-email: admin@deeplabcut.org
+Requires-Python: >=3.7.1,<3.11
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: Pillow (>=8.0.0)
+Requires-Dist: colorcet (>=3.0.0,<4.0.0)
+Requires-Dist: dlclibrary (>=0.0.2)
+Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: opencv-python-headless (>=4.5,<5.0)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: py-cpuinfo (>=5.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.20,<0.18.0)
+Requires-Dist: tables (>=3.6,<4.0)
+Requires-Dist: tensorflow (>=2.7.0,<=2.10)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Project-URL: Repository, https://github.com/DeepLabCut/DeepLabCut-live
+Description-Content-Type: text/markdown
+
+# DeepLabCut-live! SDK<img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1606082050387-M8M1CFI5DFUZCBAAUI0W/ke17ZwdGBToddI8pDm48kLuMKy7Ws6mFofiFehYynfdZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpzp2tFVMcEgqZM8QO7VXXQogrsLnYKC4n4YnYuHC1HMRWygQlqMNAoTF9HaycikLeg/DLClive.png?format=750w" width="350" title="DLC-live" alt="DLC LIVE!" align="right" vspace = "50">
+
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+![PyPI - Python Version](https://img.shields.io/pypi/v/deeplabcut-live)
+[![Downloads](https://pepy.tech/badge/deeplabcut-live)](https://pepy.tech/project/deeplabcut-live)
+[![Downloads](https://pepy.tech/badge/deeplabcut-live/month)](https://pepy.tech/project/deeplabcut-live)
+![Python package](https://github.com/DeepLabCut/DeepLabCut-live/workflows/Python%20package/badge.svg)
+[![GitHub stars](https://img.shields.io/github/stars/DeepLabCut/DeepLabCut-live.svg?style=social&label=Star)](https://github.com/DeepLabCut/DeepLabCut-live)
+[![GitHub forks](https://img.shields.io/github/forks/DeepLabCut/DeepLabCut-live.svg?style=social&label=Fork)](https://github.com/DeepLabCut/DeepLabCut-live)
+[![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&amp;url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fdeeplabcut.json&amp;query=%24.topic_list.tags.0.topic_count&amp;colorB=brightgreen&amp;&amp;suffix=%20topics&amp;logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/deeplabcut)
+[![Gitter](https://badges.gitter.im/DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![Twitter Follow](https://img.shields.io/twitter/follow/DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)
+
+This package contains a [DeepLabCut](http://www.mousemotorlab.org/deeplabcut) inference pipeline for real-time applications that has minimal (software) dependencies. Thus, it is as easy to install as possible (in particular, on atypical systems like [NVIDIA Jetson boards](https://developer.nvidia.com/buy-jetson)).
+
+**Performance:** If you would like to see estimates on how your model should perform given different video sizes, neural network type, and hardware, please see: https://deeplabcut.github.io/DLC-inferencespeed-benchmark/
+
+If you have different hardware, please consider submitting your results too! https://github.com/DeepLabCut/DLC-inferencespeed-benchmark
+
+**What this SDK provides:** This package provides a `DLCLive` class which enables pose estimation online to provide feedback. This object loads and prepares a DeepLabCut network for inference, and will return the predicted pose for single images. 
+
+To perform processing on poses (such as predicting the future pose of an animal given it's current pose, or to trigger external hardware like send TTL pulses to a laser for optogenetic stimulation), this object takes in a `Processor` object. Processor objects must contain two methods: process and save.
+
+- The `process` method takes in a pose, performs some processing, and returns processed pose.
+- The `save` method saves any valuable data created by or used by the processor
+
+For more details and examples, see documentation [here](dlclive/processor/README.md).
+
+###### 🔥🔥🔥🔥🔥 Note :: alone, this object does not record video or capture images from a camera. This must be done separately, i.e. see our [DeepLabCut-live GUI](https://github.com/gkane26/DeepLabCut-live-GUI).🔥🔥🔥
+
+### News! 
+- March 2022: DeepLabCut-Live! 1.0.2 supports poetry installation `poetry install deeplabcut-live`, thanks to PR #60.
+- March 2021: DeepLabCut-Live! [**version 1.0** is released](https://pypi.org/project/deeplabcut-live/), with support for tensorflow 1 and tensorflow 2!
+- Feb 2021: DeepLabCut-Live! was featured in **Nature Methods**: ["Real-time behavioral analysis"](https://www.nature.com/articles/s41592-021-01072-z)
+- Jan 2021: full **eLife** paper is published: ["Real-time, low-latency closed-loop feedback using markerless posture tracking"](https://elifesciences.org/articles/61909)
+- Dec 2020: we talked to **RTS Suisse Radio** about DLC-Live!: ["Capture animal movements in real time"](https://www.rts.ch/play/radio/cqfd/audio/capturer-les-mouvements-des-animaux-en-temps-reel?id=11782529)
+
+
+### Installation:
+
+Please see our instruction manual to install on a [Windows or Linux machine](docs/install_desktop.md) or on a [NVIDIA Jetson Development Board](docs/install_jetson.md). Note, this code works with tensorflow (TF) 1 or TF 2 models, but TF requires that whatever version you exported your model with, you must import with the same version (i.e., export with TF1.13, then use TF1.13 with DlC-Live; export with TF2.3, then use TF2.3 with DLC-live).
+
+- available on pypi as: `pip install deeplabcut-live`
+
+Note, you can then test your installation by running:
+
+`dlc-live-test`
+
+If installed properly, this script will i) create a temporary folder ii) download the full_dog model from the [DeepLabCut Model Zoo](http://www.mousemotorlab.org/dlc-modelzoo), iii) download a short video clip of a dog, and iv) run inference while displaying keypoints. v) remove the temporary folder.
+
+<img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1606081086014-TG9GWH63ZGGOO7K779G3/ke17ZwdGBToddI8pDm48kHiSoSToKfKUI9t99vKErWoUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYxCRW4BPu10St3TBAUQYVKcOoIGycwr1shdgJWzLuxyzjLbSRGBFFxjYMBr42yCvRK5HHsLZWtMlAHzDU294nCd/dlclivetest.png?format=1000w" width="650" title="DLC-live-test" alt="DLC LIVE TEST" align="center" vspace = "50">
+
+### Quick Start: instructions for use:
+
+1. Initialize `Processor` (if desired)
+2. Initialize the `DLCLive` object
+3. Perform pose estimation!
+
+```python
+from dlclive import DLCLive, Processor
+dlc_proc = Processor()
+dlc_live = DLCLive(<path to exported model directory>, processor=dlc_proc)
+dlc_live.init_inference(<your image>)
+dlc_live.get_pose(<your image>)
+```
+
+`DLCLive` **parameters:**
+
+  - `path` = string; full path to the exported DLC model directory
+  - `model_type` = string; the type of model to use for inference. Types include:
+      - `base` = the base DeepLabCut model
+      - `tensorrt` = apply [tensor-rt](https://developer.nvidia.com/tensorrt) optimizations to model
+      - `tflite` = use [tensorflow lite](https://www.tensorflow.org/lite) inference (in progress...)
+  - `cropping` = list of int, optional; cropping parameters in pixel number: [x1, x2, y1, y2]
+  - `dynamic` = tuple, optional; defines parameters for dynamic cropping of images
+      - `index 0` = use dynamic cropping, bool
+      - `index 1` = detection threshold, float
+      - `index 2` = margin (in pixels) around identified points, int
+  - `resize` = float, optional; factor by which to resize image (resize=0.5 downsizes both width and height of image by half). Can be used to downsize large images for faster inference
+  - `processor` = dlc pose processor object, optional
+  - `display` = bool, optional; display processed image with DeepLabCut points? Can be used to troubleshoot cropping and resizing parameters, but is very slow
+
+`DLCLive` **inputs:**
+
+  - `<path to exported model directory>` = path to the folder that has the `.pb` files that you acquire after running `deeplabcut.export_model`
+  - `<your image>` = is a numpy array of each frame
+
+
+### Benchmarking/Analyzing your exported DeepLabCut models
+
+DeepLabCut-live offers some analysis tools that allow users to peform the following operations on videos, from python or from the command line:
+
+1. Test inference speed across a range of image sizes, downsizing images by specifying the `resize` or `pixels` parameter. Using the `pixels` parameter will resize images to the desired number of `pixels`, without changing the aspect ratio. Results will be saved (along with system info) to a pickle file if you specify an output directory.
+##### python
+```python
+dlclive.benchmark_videos('/path/to/exported/model', ['/path/to/video1', '/path/to/video2'], output='/path/to/output', resize=[1.0, 0.75, '0.5'])
+```
+##### command line
+```
+dlc-live-benchmark /path/to/exported/model /path/to/video1 /path/to/video2 -o /path/to/output -r 1.0 0.75 0.5
+```
+
+2. Display keypoints to visually inspect the accuracy of exported models on different image sizes (note, this is slow and only for testing purposes):
+
+##### python
+```python
+dlclive.benchmark_videos('/path/to/exported/model', '/path/to/video', resize=0.5, display=True, pcutoff=0.5, display_radius=4, cmap='bmy')
+```
+##### command line
+```
+dlc-live-benchmark /path/to/exported/model /path/to/video -r 0.5 --display --pcutoff 0.5 --display-radius 4 --cmap bmy
+```
+
+3. Analyze and create a labeled video using the exported model and desired resize parameters. This option functions similar to `deeplabcut.benchmark_videos` and `deeplabcut.create_labeled_video` (note, this is slow and only for testing purposes).
+
+##### python
+```python
+dlclive.benchmark_videos('/path/to/exported/model', '/path/to/video', resize=[1.0, 0.75, 0.5], pcutoff=0.5, display_radius=4, cmap='bmy', save_poses=True, save_video=True)
+```
+##### command line
+```
+dlc-live-benchmark /path/to/exported/model /path/to/video -r 0.5 --pcutoff 0.5 --display-radius 4 --cmap bmy --save-poses --save-video
+```
+
+## License:
+
+This project is licensed under the GNU AGPLv3. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, we ask that you please cite us! This software is available for licensing via the EPFL Technology Transfer Office (https://tto.epfl.ch/, info.tto@epfl.ch).
+
+## Community Support, Developers, & Help:
+
+This is an actively developed package and we welcome community development and involvement.
+
+- If you want to contribute to the code, please read our guide [here](https://github.com/DeepLabCut/DeepLabCut/blob/master/CONTRIBUTING.md), which is provided at the main repository of DeepLabCut.
+
+- We are a community partner on the [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&amp;url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fdeeplabcut.json&amp;query=%24.topic_list.tags.0.topic_count&amp;colorB=brightgreen&amp;&amp;suffix=%20topics&amp;logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tags/deeplabcut). Please post help and support questions on the forum with the tag DeepLabCut. Check out their mission statement [Scientific Community Image Forum: A discussion forum for scientific image software](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3000340).
+
+- If you encounter a previously unreported bug/code issue, please post here (we encourage you to search issues first): https://github.com/DeepLabCut/DeepLabCut-live/issues
+
+- For quick discussions here: [![Gitter](https://badges.gitter.im/DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+
+### Reference:
+
+If you utilize our tool, please [cite Kane et al, eLife 2020](https://elifesciences.org/articles/61909). The preprint is available here: https://www.biorxiv.org/content/10.1101/2020.08.04.236422v2
+
+```
+@Article{Kane2020dlclive,
+  author    = {Kane, Gary and Lopes, Gonçalo and Sanders, Jonny and Mathis, Alexander and Mathis, Mackenzie},
+  title     = {Real-time, low-latency closed-loop feedback using markerless posture tracking},
+  journal   = {eLife},
+  year      = {2020},
 }
+```
 
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,166 +1,165 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['dlclive',
-'dlclive.check_install', 'dlclive.processor'] package_data = \ {'': ['*']}
-install_requires = \ ['Pillow>=8.0.0', 'colorcet>=3.0.0,<4.0.0',
-'dlclibrary>=0.0.2', 'numpy>=1.20,<2.0', 'opencv-python-headless>=4.5,<5.0',
-'pandas>=1.3,<2.0', 'py-cpuinfo>=5.0.0', 'ruamel.yaml>=0.17.20,<0.18.0',
-'tables>=3.6,<4.0', 'tensorflow>=2.7.0,<=2.10', 'tqdm>=4.62.3,<5.0.0']
-entry_points = \ {'console_scripts': ['dlc-live-benchmark = dlclive.benchmark:
-main', 'dlc-live-test = ' 'dlclive.check_install.check_install:main']}
-setup_kwargs = { 'name': 'deeplabcut-live', 'version': '1.0.3', 'description':
-'Class to load exported DeepLabCut networks and perform pose estimation on
-single frames (from a camera feed)', 'long_description': '# DeepLabCut-live!
-SDK[DLC LIVE!]\n\n[Code_style:_black]\n![PyPI - Python Version](https://
-img.shields.io/pypi/v/deeplabcut-live)\n[![Downloads](https://pepy.tech/badge/
-deeplabcut-live)](https://pepy.tech/project/deeplabcut-live)\n[![Downloads]
+Metadata-Version: 2.1 Name: deeplabcut-live Version: 1.0.4 Summary: Class to
+load exported DeepLabCut networks and perform pose estimation on single frames
+(from a camera feed) Home-page: https://github.com/DeepLabCut/DeepLabCut-live
+License: AGPL-3.0-or-later Author: A. & M. Mathis Labs Author-email:
+admin@deeplabcut.org Requires-Python: >=3.7.1,<3.11 Classifier: License :: OSI
+Approved :: GNU Affero General Public License v3 or later (AGPLv3+) Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: Pillow (>=8.0.0) Requires-Dist:
+colorcet (>=3.0.0,<4.0.0) Requires-Dist: dlclibrary (>=0.0.2) Requires-Dist:
+numpy (>=1.20,<2.0) Requires-Dist: opencv-python-headless (>=4.5,<5.0)
+Requires-Dist: pandas (>=1.3,<2.0) Requires-Dist: py-cpuinfo (>=5.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.20,<0.18.0) Requires-Dist: tables
+(>=3.6,<4.0) Requires-Dist: tensorflow (>=2.7.0,<=2.10) Requires-Dist: tqdm
+(>=4.62.3,<5.0.0) Project-URL: Repository, https://github.com/DeepLabCut/
+DeepLabCut-live Description-Content-Type: text/markdown # DeepLabCut-live! SDK
+[DLC LIVE!] [Code_style:_black] ![PyPI - Python Version](https://
+img.shields.io/pypi/v/deeplabcut-live) [![Downloads](https://pepy.tech/badge/
+deeplabcut-live)](https://pepy.tech/project/deeplabcut-live) [![Downloads]
 (https://pepy.tech/badge/deeplabcut-live/month)](https://pepy.tech/project/
-deeplabcut-live)\n![Python package](https://github.com/DeepLabCut/DeepLabCut-
-live/workflows/Python%20package/badge.svg)\n[![GitHub stars](https://
+deeplabcut-live) ![Python package](https://github.com/DeepLabCut/DeepLabCut-
+live/workflows/Python%20package/badge.svg) [![GitHub stars](https://
 img.shields.io/github/stars/DeepLabCut/DeepLabCut-
 live.svg?style=social&label=Star)](https://github.com/DeepLabCut/DeepLabCut-
-live)\n[![GitHub forks](https://img.shields.io/github/forks/DeepLabCut/
+live) [![GitHub forks](https://img.shields.io/github/forks/DeepLabCut/
 DeepLabCut-live.svg?style=social&label=Fork)](https://github.com/DeepLabCut/
-DeepLabCut-live)\n[![Image.sc forum](https://img.shields.io/badge/dynamic/
+DeepLabCut-live) [![Image.sc forum](https://img.shields.io/badge/dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
-forum.image.sc/tags/deeplabcut)\n[![Gitter](https://badges.gitter.im/
-DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)\n[![Twitter
+forum.image.sc/tags/deeplabcut) [![Gitter](https://badges.gitter.im/DeepLabCut/
+community.svg)](https://gitter.im/DeepLabCut/
+community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) [![Twitter
 Follow](https://img.shields.io/twitter/follow/
-DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/
-DeepLabCut)\n\nThis package contains a [DeepLabCut](http://
-www.mousemotorlab.org/deeplabcut) inference pipeline for real-time applications
-that has minimal (software) dependencies. Thus, it is as easy to install as
-possible (in particular, on atypical systems like [NVIDIA Jetson boards](https:
-//developer.nvidia.com/buy-jetson)).\n\n**Performance:** If you would like to
-see estimates on how your model should perform given different video sizes,
-neural network type, and hardware, please see: https://deeplabcut.github.io/
-DLC-inferencespeed-benchmark/\n\nIf you have different hardware, please
-consider submitting your results too! https://github.com/DeepLabCut/DLC-
-inferencespeed-benchmark\n\n**What this SDK provides:** This package provides a
-`DLCLive` class which enables pose estimation online to provide feedback. This
-object loads and prepares a DeepLabCut network for inference, and will return
-the predicted pose for single images. \n\nTo perform processing on poses (such
-as predicting the future pose of an animal given it\'s current pose, or to
-trigger external hardware like send TTL pulses to a laser for optogenetic
-stimulation), this object takes in a `Processor` object. Processor objects must
-contain two methods: process and save.\n\n- The `process` method takes in a
-pose, performs some processing, and returns processed pose.\n- The `save`
-method saves any valuable data created by or used by the processor\n\nFor more
-details and examples, see documentation [here](dlclive/processor/
-README.md).\n\n###### ð¥ð¥ð¥ð¥ð¥ Note :: alone, this object does not
+DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)
+This package contains a [DeepLabCut](http://www.mousemotorlab.org/deeplabcut)
+inference pipeline for real-time applications that has minimal (software)
+dependencies. Thus, it is as easy to install as possible (in particular, on
+atypical systems like [NVIDIA Jetson boards](https://developer.nvidia.com/buy-
+jetson)). **Performance:** If you would like to see estimates on how your model
+should perform given different video sizes, neural network type, and hardware,
+please see: https://deeplabcut.github.io/DLC-inferencespeed-benchmark/ If you
+have different hardware, please consider submitting your results too! https://
+github.com/DeepLabCut/DLC-inferencespeed-benchmark **What this SDK provides:**
+This package provides a `DLCLive` class which enables pose estimation online to
+provide feedback. This object loads and prepares a DeepLabCut network for
+inference, and will return the predicted pose for single images. To perform
+processing on poses (such as predicting the future pose of an animal given it's
+current pose, or to trigger external hardware like send TTL pulses to a laser
+for optogenetic stimulation), this object takes in a `Processor` object.
+Processor objects must contain two methods: process and save. - The `process`
+method takes in a pose, performs some processing, and returns processed pose. -
+The `save` method saves any valuable data created by or used by the processor
+For more details and examples, see documentation [here](dlclive/processor/
+README.md). ###### ð¥ð¥ð¥ð¥ð¥ Note :: alone, this object does not
 record video or capture images from a camera. This must be done separately,
 i.e. see our [DeepLabCut-live GUI](https://github.com/gkane26/DeepLabCut-live-
-GUI).ð¥ð¥ð¥\n\n### News! \n- March 2022: DeepLabCut-Live! 1.0.2 supports
-poetry installation `poetry install deeplabcut-live`, thanks to PR #60.\n-
-March 2021: DeepLabCut-Live! [**version 1.0** is released](https://pypi.org/
-project/deeplabcut-live/), with support for tensorflow 1 and tensorflow 2!\n-
-Feb 2021: DeepLabCut-Live! was featured in **Nature Methods**: ["Real-time
-behavioral analysis"](https://www.nature.com/articles/s41592-021-01072-z)\n-
-Jan 2021: full **eLife** paper is published: ["Real-time, low-latency closed-
-loop feedback using markerless posture tracking"](https://elifesciences.org/
-articles/61909)\n- Dec 2020: we talked to **RTS Suisse Radio** about DLC-Live!:
-["Capture animal movements in real time"](https://www.rts.ch/play/radio/cqfd/
-audio/capturer-les-mouvements-des-animaux-en-temps-reel?id=11782529)\n\n\n###
-Installation:\n\nPlease see our instruction manual to install on a [Windows or
-Linux machine](docs/install_desktop.md) or on a [NVIDIA Jetson Development
-Board](docs/install_jetson.md). Note, this code works with tensorflow (TF) 1 or
-TF 2 models, but TF requires that whatever version you exported your model
-with, you must import with the same version (i.e., export with TF1.13, then use
-TF1.13 with DlC-Live; export with TF2.3, then use TF2.3 with DLC-live).\n\n-
-available on pypi as: `pip install deeplabcut-live`\n\nNote, you can then test
-your installation by running:\n\n`dlc-live-test`\n\nIf installed properly, this
-script will i) create a temporary folder ii) download the full_dog model from
-the [DeepLabCut Model Zoo](http://www.mousemotorlab.org/dlc-modelzoo), iii)
+GUI).ð¥ð¥ð¥ ### News! - March 2022: DeepLabCut-Live! 1.0.2 supports
+poetry installation `poetry install deeplabcut-live`, thanks to PR #60. - March
+2021: DeepLabCut-Live! [**version 1.0** is released](https://pypi.org/project/
+deeplabcut-live/), with support for tensorflow 1 and tensorflow 2! - Feb 2021:
+DeepLabCut-Live! was featured in **Nature Methods**: ["Real-time behavioral
+analysis"](https://www.nature.com/articles/s41592-021-01072-z) - Jan 2021: full
+**eLife** paper is published: ["Real-time, low-latency closed-loop feedback
+using markerless posture tracking"](https://elifesciences.org/articles/61909) -
+Dec 2020: we talked to **RTS Suisse Radio** about DLC-Live!: ["Capture animal
+movements in real time"](https://www.rts.ch/play/radio/cqfd/audio/capturer-les-
+mouvements-des-animaux-en-temps-reel?id=11782529) ### Installation: Please see
+our instruction manual to install on a [Windows or Linux machine](docs/
+install_desktop.md) or on a [NVIDIA Jetson Development Board](docs/
+install_jetson.md). Note, this code works with tensorflow (TF) 1 or TF 2
+models, but TF requires that whatever version you exported your model with, you
+must import with the same version (i.e., export with TF1.13, then use TF1.13
+with DlC-Live; export with TF2.3, then use TF2.3 with DLC-live). - available on
+pypi as: `pip install deeplabcut-live` Note, you can then test your
+installation by running: `dlc-live-test` If installed properly, this script
+will i) create a temporary folder ii) download the full_dog model from the
+[DeepLabCut Model Zoo](http://www.mousemotorlab.org/dlc-modelzoo), iii)
 download a short video clip of a dog, and iv) run inference while displaying
-keypoints. v) remove the temporary folder.\n\n[DLC LIVE TEST]\n\n### Quick
-Start: instructions for use:\n\n1. Initialize `Processor` (if desired)\n2.
-Initialize the `DLCLive` object\n3. Perform pose estimation!\n\n```python\nfrom
-dlclive import DLCLive, Processor\ndlc_proc = Processor()\ndlc_live = DLCLive(,
-processor=dlc_proc)\ndlc_live.init_inference()\ndlc_live.get_pose
-()\n```\n\n`DLCLive` **parameters:**\n\n - `path` = string; full path to the
-exported DLC model directory\n - `model_type` = string; the type of model to
-use for inference. Types include:\n - `base` = the base DeepLabCut model\n -
-`tensorrt` = apply [tensor-rt](https://developer.nvidia.com/tensorrt)
-optimizations to model\n - `tflite` = use [tensorflow lite](https://
-www.tensorflow.org/lite) inference (in progress...)\n - `cropping` = list of
-int, optional; cropping parameters in pixel number: [x1, x2, y1, y2]\n -
-`dynamic` = tuple, optional; defines parameters for dynamic cropping of
-images\n - `index 0` = use dynamic cropping, bool\n - `index 1` = detection
-threshold, float\n - `index 2` = margin (in pixels) around identified points,
-int\n - `resize` = float, optional; factor by which to resize image (resize=0.5
-downsizes both width and height of image by half). Can be used to downsize
-large images for faster inference\n - `processor` = dlc pose processor object,
-optional\n - `display` = bool, optional; display processed image with
+keypoints. v) remove the temporary folder. [DLC LIVE TEST] ### Quick Start:
+instructions for use: 1. Initialize `Processor` (if desired) 2. Initialize the
+`DLCLive` object 3. Perform pose estimation! ```python from dlclive import
+DLCLive, Processor dlc_proc = Processor() dlc_live = DLCLive(,
+processor=dlc_proc) dlc_live.init_inference() dlc_live.get_pose() ``` `DLCLive`
+**parameters:** - `path` = string; full path to the exported DLC model
+directory - `model_type` = string; the type of model to use for inference.
+Types include: - `base` = the base DeepLabCut model - `tensorrt` = apply
+[tensor-rt](https://developer.nvidia.com/tensorrt) optimizations to model -
+`tflite` = use [tensorflow lite](https://www.tensorflow.org/lite) inference (in
+progress...) - `cropping` = list of int, optional; cropping parameters in pixel
+number: [x1, x2, y1, y2] - `dynamic` = tuple, optional; defines parameters for
+dynamic cropping of images - `index 0` = use dynamic cropping, bool - `index 1`
+= detection threshold, float - `index 2` = margin (in pixels) around identified
+points, int - `resize` = float, optional; factor by which to resize image
+(resize=0.5 downsizes both width and height of image by half). Can be used to
+downsize large images for faster inference - `processor` = dlc pose processor
+object, optional - `display` = bool, optional; display processed image with
 DeepLabCut points? Can be used to troubleshoot cropping and resizing
-parameters, but is very slow\n\n`DLCLive` **inputs:**\n\n - `` = path to the
-folder that has the `.pb` files that you acquire after running
-`deeplabcut.export_model`\n - `` = is a numpy array of each frame\n\n\n###
-Benchmarking/Analyzing your exported DeepLabCut models\n\nDeepLabCut-live
-offers some analysis tools that allow users to peform the following operations
-on videos, from python or from the command line:\n\n1. Test inference speed
-across a range of image sizes, downsizing images by specifying the `resize` or
-`pixels` parameter. Using the `pixels` parameter will resize images to the
-desired number of `pixels`, without changing the aspect ratio. Results will be
-saved (along with system info) to a pickle file if you specify an output
-directory.\n##### python\n```python\ndlclive.benchmark_videos(\'/path/to/
-exported/model\', [\'/path/to/video1\', \'/path/to/video2\'], output=\'/path/
-to/output\', resize=[1.0, 0.75, \'0.5\'])\n```\n##### command line\n```\ndlc-
-live-benchmark /path/to/exported/model /path/to/video1 /path/to/video2 -o /
-path/to/output -r 1.0 0.75 0.5\n```\n\n2. Display keypoints to visually inspect
-the accuracy of exported models on different image sizes (note, this is slow
-and only for testing purposes):\n\n#####
-python\n```python\ndlclive.benchmark_videos(\'/path/to/exported/model\', \'/
-path/to/video\', resize=0.5, display=True, pcutoff=0.5, display_radius=4,
-cmap=\'bmy\')\n```\n##### command line\n```\ndlc-live-benchmark /path/to/
-exported/model /path/to/video -r 0.5 --display --pcutoff 0.5 --display-radius 4
---cmap bmy\n```\n\n3. Analyze and create a labeled video using the exported
-model and desired resize parameters. This option functions similar to
-`deeplabcut.benchmark_videos` and `deeplabcut.create_labeled_video` (note, this
-is slow and only for testing purposes).\n\n#####
-python\n```python\ndlclive.benchmark_videos(\'/path/to/exported/model\', \'/
-path/to/video\', resize=[1.0, 0.75, 0.5], pcutoff=0.5, display_radius=4,
-cmap=\'bmy\', save_poses=True, save_video=True)\n```\n##### command
-line\n```\ndlc-live-benchmark /path/to/exported/model /path/to/video -r 0.5 --
-pcutoff 0.5 --display-radius 4 --cmap bmy --save-poses --save-video\n```\n\n##
-License:\n\nThis project is licensed under the GNU AGPLv3. Note that the
+parameters, but is very slow `DLCLive` **inputs:** - `` = path to the folder
+that has the `.pb` files that you acquire after running
+`deeplabcut.export_model` - `` = is a numpy array of each frame ###
+Benchmarking/Analyzing your exported DeepLabCut models DeepLabCut-live offers
+some analysis tools that allow users to peform the following operations on
+videos, from python or from the command line: 1. Test inference speed across a
+range of image sizes, downsizing images by specifying the `resize` or `pixels`
+parameter. Using the `pixels` parameter will resize images to the desired
+number of `pixels`, without changing the aspect ratio. Results will be saved
+(along with system info) to a pickle file if you specify an output directory.
+##### python ```python dlclive.benchmark_videos('/path/to/exported/model', ['/
+path/to/video1', '/path/to/video2'], output='/path/to/output', resize=[1.0,
+0.75, '0.5']) ``` ##### command line ``` dlc-live-benchmark /path/to/exported/
+model /path/to/video1 /path/to/video2 -o /path/to/output -r 1.0 0.75 0.5 ``` 2.
+Display keypoints to visually inspect the accuracy of exported models on
+different image sizes (note, this is slow and only for testing purposes): #####
+python ```python dlclive.benchmark_videos('/path/to/exported/model', '/path/to/
+video', resize=0.5, display=True, pcutoff=0.5, display_radius=4, cmap='bmy')
+``` ##### command line ``` dlc-live-benchmark /path/to/exported/model /path/to/
+video -r 0.5 --display --pcutoff 0.5 --display-radius 4 --cmap bmy ``` 3.
+Analyze and create a labeled video using the exported model and desired resize
+parameters. This option functions similar to `deeplabcut.benchmark_videos` and
+`deeplabcut.create_labeled_video` (note, this is slow and only for testing
+purposes). ##### python ```python dlclive.benchmark_videos('/path/to/exported/
+model', '/path/to/video', resize=[1.0, 0.75, 0.5], pcutoff=0.5,
+display_radius=4, cmap='bmy', save_poses=True, save_video=True) ``` #####
+command line ``` dlc-live-benchmark /path/to/exported/model /path/to/video -
+r 0.5 --pcutoff 0.5 --display-radius 4 --cmap bmy --save-poses --save-video ```
+## License: This project is licensed under the GNU AGPLv3. Note that the
 software is provided "as is", without warranty of any kind, express or implied.
 If you use the code or data, we ask that you please cite us! This software is
 available for licensing via the EPFL Technology Transfer Office (https://
-tto.epfl.ch/, info.tto@epfl.ch).\n\n## Community Support, Developers, & Help:
-\n\nThis is an actively developed package and we welcome community development
-and involvement.\n\n- If you want to contribute to the code, please read our
-guide [here](https://github.com/DeepLabCut/DeepLabCut/blob/master/
-CONTRIBUTING.md), which is provided at the main repository of DeepLabCut.\n\n-
-We are a community partner on the [![Image.sc forum](https://img.shields.io/
-badge/dynamic/
+tto.epfl.ch/, info.tto@epfl.ch). ## Community Support, Developers, & Help: This
+is an actively developed package and we welcome community development and
+involvement. - If you want to contribute to the code, please read our guide
+[here](https://github.com/DeepLabCut/DeepLabCut/blob/master/CONTRIBUTING.md),
+which is provided at the main repository of DeepLabCut. - We are a community
+partner on the [![Image.sc forum](https://img.shields.io/badge/dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftags%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
 forum.image.sc/tags/deeplabcut). Please post help and support questions on the
 forum with the tag DeepLabCut. Check out their mission statement [Scientific
 Community Image Forum: A discussion forum for scientific image software](https:
-//journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3000340).\n\n-
-If you encounter a previously unreported bug/code issue, please post here (we
+//journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3000340). - If
+you encounter a previously unreported bug/code issue, please post here (we
 encourage you to search issues first): https://github.com/DeepLabCut/
-DeepLabCut-live/issues\n\n- For quick discussions here: [![Gitter](https://
+DeepLabCut-live/issues - For quick discussions here: [![Gitter](https://
 badges.gitter.im/DeepLabCut/community.svg)](https://gitter.im/DeepLabCut/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)\n\n###
-Reference:\n\nIf you utilize our tool, please [cite Kane et al, eLife 2020]
-(https://elifesciences.org/articles/61909). The preprint is available here:
-https://www.biorxiv.org/content/10.1101/2020.08.04.236422v2\n\n```\n@Article
-{Kane2020dlclive,\n author = {Kane, Gary and Lopes, GonÃ§alo and Sanders, Jonny
-and Mathis, Alexander and Mathis, Mackenzie},\n title = {Real-time, low-latency
-closed-loop feedback using markerless posture tracking},\n journal = {eLife},\n
-year = {2020},\n}\n```\n\n', 'author': 'A. & M. Mathis Labs', 'author_email':
-'admin@deeplabcut.org', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/DeepLabCut/DeepLabCut-live', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7.1,<3.11', } setup
-(**setup_kwargs)
+community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) ###
+Reference: If you utilize our tool, please [cite Kane et al, eLife 2020](https:
+//elifesciences.org/articles/61909). The preprint is available here: https://
+www.biorxiv.org/content/10.1101/2020.08.04.236422v2 ``` @Article
+{Kane2020dlclive, author = {Kane, Gary and Lopes, GonÃ§alo and Sanders, Jonny
+and Mathis, Alexander and Mathis, Mackenzie}, title = {Real-time, low-latency
+closed-loop feedback using markerless posture tracking}, journal = {eLife},
+year = {2020}, } ```
```

