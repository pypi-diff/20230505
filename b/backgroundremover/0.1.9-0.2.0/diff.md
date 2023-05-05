# Comparing `tmp/backgroundremover-0.1.9.tar.gz` & `tmp/backgroundremover-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backgroundremover-0.1.9.tar", last modified: Fri Aug 13 15:32:56 2021, max compression
+gzip compressed data, was "dist/backgroundremover-0.2.0.tar", last modified: Fri May  5 19:23:18 2023, max compression
```

## Comparing `backgroundremover-0.1.9.tar` & `backgroundremover-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,26 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/
--rw-rw-r--   0 john      (1000) john      (1000)      183 2021-04-24 21:14:16.000000 backgroundremover-0.1.9/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)      230 2021-04-24 21:14:16.000000 backgroundremover-0.1.9/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)     6481 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)       78 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     4721 2021-08-13 14:30:46.000000 backgroundremover-0.1.9/README.md
--rw-rw-r--   0 john      (1000) john      (1000)      364 2021-07-30 22:27:39.000000 backgroundremover-0.1.9/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2021-05-24 03:18:01.000000 backgroundremover-0.1.9/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)     1058 2021-08-13 15:31:50.000000 backgroundremover-0.1.9/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)       70 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      364 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     6481 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      718 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover.egg-info/dependency_links.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)     7904 2021-08-13 15:30:16.000000 backgroundremover-0.1.9/src/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2021-04-24 21:14:16.000000 backgroundremover-0.1.9/src/backgroundremover/cmd/server.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-04-24 21:14:16.000000 backgroundremover-0.1.9/src/backgroundremover/cmd/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2021-08-13 15:32:56.000000 backgroundremover-0.1.9/src/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2021-04-24 21:14:16.000000 backgroundremover-0.1.9/src/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)     4357 2021-08-13 14:21:03.000000 backgroundremover-0.1.9/src/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2021-05-24 03:21:24.000000 backgroundremover-0.1.9/src/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-04-24 21:14:16.000000 backgroundremover-0.1.9/src/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     6923 2021-08-13 15:27:54.000000 backgroundremover-0.1.9/src/backgroundremover/bg.py
--rw-rw-r--   0 john      (1000) john      (1000)    10781 2021-08-13 15:29:14.000000 backgroundremover-0.1.9/src/backgroundremover/utilities.py
--rw-rw-r--   0 john      (1000) john      (1000)      173 2021-08-13 15:31:50.000000 backgroundremover-0.1.9/src/backgroundremover/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.0/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.0/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     6149 2023-05-05 19:20:58.000000 backgroundremover-0.2.0/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      677 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      364 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/cmd/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.0/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.0/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      364 2023-04-30 21:22:20.000000 backgroundremover-0.2.0/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-05 19:23:18.000000 backgroundremover-0.2.0/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1086 2023-05-05 19:23:15.000000 backgroundremover-0.2.0/setup.py
```

### Comparing `backgroundremover-0.1.9/PKG-INFO` & `backgroundremover-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.1.9
+Version: 0.2.0
 Summary: Background remover from image and video
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
-        
-        BackgroundRemover is a command line tool to remove background from [video](https://backgroundremover.app/video)
-        and [image](https://backgroundremover.app/image), brought to you
-        by [https://BackgroundRemover.app](https://backgroundremover.app) which is an app made by [nadermx](https://john.nader.mx) powered by this tool
-        
-        <img alt="background remover image" src="https://backgroundremover.app/static/backgroundremoverexample.png" height="200" />
-        <img alt="background remover video" src="/examplegif/backgroundremoverprocessed.gif" height="200" />
+        ![Background Remover](/examplefiles/backgroundremoverexample.png)
+        <img alt="background remover video" src="/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
+        BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video), made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
         
         
         ### Requirements
         
-        * python <= 3.6
+        * python >= 3.6
         * python3.6-dev #or what ever version of python you using
         * torch and torchvision stable version (https://pytorch.org)
         * ffmpeg 4.4+
         
         #### How to install torch and fmpeg
         
         Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
@@ -41,51 +37,66 @@
         
         ```
         sudo apt install ffmpeg python3.6-dev
         ```
         
         ### Installation
         
+        To run code without installation:
+        
+        ```bash
+        python -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
+        ```
+        and for windows
+        ```bash
+        python.exe -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
+        ```
+        ### Installation
+        
         To Install backgroundremover, install it from pypi
         
         ```bash
         pip install --upgrade pip
         pip install backgroundremover
         ```
-        
+        Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will get them from u2net's google drive, as they say too [here](https://github.com/xuebinqin/U-2-Net#usage-for-salient-object-detection), and in this repo the code that pulls it is [here](https://github.com/nadermx/backgroundremover/blob/main/src/backgroundremover/utilities.py#L289)
         # Usage as a cli
         ## Image
         
         Remove the background from a local file image
         
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -o "output.png"
         ```
         
         ### Advance usage for image background removal
         
         Sometimes it is possible to achieve better results by turning on alpha matting. Example:
         
         ```bash
-        backgroundremover -i "/path/to/image.jpeg" a -ae 15 -o "output.png"
+        backgroundremover -i "/path/to/image.jpeg" -a -ae 15 -o "output.png"
         ```
         change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -m "u2net_human_seg" -o "output.png"
         ```
         ## Video
         
         ### remove background from video and make transparent mov
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -tv -o "output.mov"
         ```
         ### remove background from local video and overlay it over other video
         ```bash
-        backgroundremover -i "/path/to/video.mp4" -tov -tv "/path/to/videtobeoverlayed.mp4" -o "output.mov"
+        backgroundremover -i "/path/to/video.mp4" -tov "/path/to/videtobeoverlayed.mp4" -o "output.mov"
+        ```
+        ### remove background from local video and overlay it over an image
+        ```bash
+        backgroundremover -i "/path/to/video.mp4" -toi "/path/to/videtobeoverlayed.mp4" -o "output.mov"
         ```
         
         ### remove background from video and make transparent gif
         
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -tg -o "output.gif"
@@ -102,44 +113,57 @@
         
         Change the framerate of the video (default is set to 30)
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -fr 30 -tv -o "output.mov"
         ```
         
+        Set total number of frames of the video (default is set to -1, ie the remove background from full video)
+        
+        ```bash
+        backgroundremover -i "/path/to/video.mp4" -fl 150 -tv -o "output.mov"
+        ```
+        
         Change the gpu batch size of the video (default is set to 1)
         
         ```bash
-        backgroundremover -i "/path/to/video.mp4" -gp 4 -tv -o "output.mov"
+        backgroundremover -i "/path/to/video.mp4" -gb 4 -tv -o "output.mov"
         ```
         
         Change the number of workers working on video (default is set to 1)
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
         ```
-        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
+        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
         ```bash
-        backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg"-tv -o "output.mov"
+        backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
         ```
         
         ## Todo
         
         - convert logic from video to image to utilize more GPU on image removal
         - clean up documentation a bit more
         - add ability to adjust and give feedback images or videos to datasets
+        - add ability to realtime background removal for videos, for streaming
+        - finish flask server api
+        - add ability to use other models than u2net, ie your own.
         - other
         
         ### Pull requests
         
         Accepted
         
         ### If you like this library
         
-        Give a link to our project [BackgroundRemover.app](https://backgroundremover.app) or this git, telling people that you like it or use it.
+        Give a link to our project [BackgroundRemoverAI.com](https://backgroundremoverai.com) or this git, telling people that you like it or use it.
+        #### bitcoin
+        <a href="bitcoin:BC1Q80PSHGQGQR7WN3KAX59XWVMGQ9FTVWLA7DEW7W?label=backgroundremover&message=BackgroundRemover">bc1q80pshgqgqr7wn3kax59xwvmgq9ftvwla7dew7w</a>
+        
+        
         
         ### Reason for project
         
         We made it our own package after merging together parts of others, adding in a few features of our own via posting parts as bounty questions on superuser, etc.  As well as asked on hackernews earlier to open source the image part, so decided to add in video, and a bit more.
```

### Comparing `backgroundremover-0.1.9/README.md` & `backgroundremover-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # BackgroundRemover
-
-BackgroundRemover is a command line tool to remove background from [video](https://backgroundremover.app/video)
-and [image](https://backgroundremover.app/image), brought to you
-by [https://BackgroundRemover.app](https://backgroundremover.app) which is an app made by [nadermx](https://john.nader.mx) powered by this tool
-
-<img alt="background remover image" src="https://backgroundremover.app/static/backgroundremoverexample.png" height="200" />
-<img alt="background remover video" src="/examplegif/backgroundremoverprocessed.gif" height="200" />
+![Background Remover](/examplefiles/backgroundremoverexample.png)
+<img alt="background remover video" src="/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
+BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video), made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
 
 
 ### Requirements
 
-* python <= 3.6
+* python >= 3.6
 * python3.6-dev #or what ever version of python you using
 * torch and torchvision stable version (https://pytorch.org)
 * ffmpeg 4.4+
 
 #### How to install torch and fmpeg
 
 Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
@@ -33,51 +29,66 @@
 
 ```
 sudo apt install ffmpeg python3.6-dev
 ```
 
 ### Installation
 
+To run code without installation:
+
+```bash
+python -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
+```
+and for windows
+```bash
+python.exe -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
+```
+### Installation
+
 To Install backgroundremover, install it from pypi
 
 ```bash
 pip install --upgrade pip
 pip install backgroundremover
 ```
-
+Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will get them from u2net's google drive, as they say too [here](https://github.com/xuebinqin/U-2-Net#usage-for-salient-object-detection), and in this repo the code that pulls it is [here](https://github.com/nadermx/backgroundremover/blob/main/src/backgroundremover/utilities.py#L289)
 # Usage as a cli
 ## Image
 
 Remove the background from a local file image
 
 ```bash
 backgroundremover -i "/path/to/image.jpeg" -o "output.png"
 ```
 
 ### Advance usage for image background removal
 
 Sometimes it is possible to achieve better results by turning on alpha matting. Example:
 
 ```bash
-backgroundremover -i "/path/to/image.jpeg" a -ae 15 -o "output.png"
+backgroundremover -i "/path/to/image.jpeg" -a -ae 15 -o "output.png"
 ```
 change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
 ```bash
 backgroundremover -i "/path/to/image.jpeg" -m "u2net_human_seg" -o "output.png"
 ```
 ## Video
 
 ### remove background from video and make transparent mov
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -tv -o "output.mov"
 ```
 ### remove background from local video and overlay it over other video
 ```bash
-backgroundremover -i "/path/to/video.mp4" -tov -tv "/path/to/videtobeoverlayed.mp4" -o "output.mov"
+backgroundremover -i "/path/to/video.mp4" -tov "/path/to/videtobeoverlayed.mp4" -o "output.mov"
+```
+### remove background from local video and overlay it over an image
+```bash
+backgroundremover -i "/path/to/video.mp4" -toi "/path/to/videtobeoverlayed.mp4" -o "output.mov"
 ```
 
 ### remove background from video and make transparent gif
 
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -tg -o "output.gif"
@@ -94,44 +105,57 @@
 
 Change the framerate of the video (default is set to 30)
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -fr 30 -tv -o "output.mov"
 ```
 
+Set total number of frames of the video (default is set to -1, ie the remove background from full video)
+
+```bash
+backgroundremover -i "/path/to/video.mp4" -fl 150 -tv -o "output.mov"
+```
+
 Change the gpu batch size of the video (default is set to 1)
 
 ```bash
-backgroundremover -i "/path/to/video.mp4" -gp 4 -tv -o "output.mov"
+backgroundremover -i "/path/to/video.mp4" -gb 4 -tv -o "output.mov"
 ```
 
 Change the number of workers working on video (default is set to 1)
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
 ```
-change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
+change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
 ```bash
-backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg"-tv -o "output.mov"
+backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
 ```
 
 ## Todo
 
 - convert logic from video to image to utilize more GPU on image removal
 - clean up documentation a bit more
 - add ability to adjust and give feedback images or videos to datasets
+- add ability to realtime background removal for videos, for streaming
+- finish flask server api
+- add ability to use other models than u2net, ie your own.
 - other
 
 ### Pull requests
 
 Accepted
 
 ### If you like this library
 
-Give a link to our project [BackgroundRemover.app](https://backgroundremover.app) or this git, telling people that you like it or use it.
+Give a link to our project [BackgroundRemoverAI.com](https://backgroundremoverai.com) or this git, telling people that you like it or use it.
+#### bitcoin
+<a href="bitcoin:BC1Q80PSHGQGQR7WN3KAX59XWVMGQ9FTVWLA7DEW7W?label=backgroundremover&message=BackgroundRemover">bc1q80pshgqgqr7wn3kax59xwvmgq9ftvwla7dew7w</a>
+
+
 
 ### Reason for project
 
 We made it our own package after merging together parts of others, adding in a few features of our own via posting parts as bounty questions on superuser, etc.  As well as asked on hackernews earlier to open source the image part, so decided to add in video, and a bit more.
```

### Comparing `backgroundremover-0.1.9/LICENSE.txt` & `backgroundremover-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.1.9/setup.py` & `backgroundremover-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.1.9",
+    version="0.2.0",
     description="Background remover from image and video",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="remove, background, u2net, remove background, background remover",
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    package_dir={"": "backgroundremover"},
+    packages=find_packages(where="backgroundremover"),
     python_requires=">=3.6, <4",
     install_requires=requireds,
     entry_points={
         "console_scripts": [
             "backgroundremover=backgroundremover.cmd.cli:main",
         ],
     },
```

### Comparing `backgroundremover-0.1.9/src/backgroundremover.egg-info/PKG-INFO` & `backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.1.9
+Version: 0.2.0
 Summary: Background remover from image and video
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
-        
-        BackgroundRemover is a command line tool to remove background from [video](https://backgroundremover.app/video)
-        and [image](https://backgroundremover.app/image), brought to you
-        by [https://BackgroundRemover.app](https://backgroundremover.app) which is an app made by [nadermx](https://john.nader.mx) powered by this tool
-        
-        <img alt="background remover image" src="https://backgroundremover.app/static/backgroundremoverexample.png" height="200" />
-        <img alt="background remover video" src="/examplegif/backgroundremoverprocessed.gif" height="200" />
+        ![Background Remover](/examplefiles/backgroundremoverexample.png)
+        <img alt="background remover video" src="/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
+        BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video), made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
         
         
         ### Requirements
         
-        * python <= 3.6
+        * python >= 3.6
         * python3.6-dev #or what ever version of python you using
         * torch and torchvision stable version (https://pytorch.org)
         * ffmpeg 4.4+
         
         #### How to install torch and fmpeg
         
         Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
@@ -41,51 +37,66 @@
         
         ```
         sudo apt install ffmpeg python3.6-dev
         ```
         
         ### Installation
         
+        To run code without installation:
+        
+        ```bash
+        python -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
+        ```
+        and for windows
+        ```bash
+        python.exe -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
+        ```
+        ### Installation
+        
         To Install backgroundremover, install it from pypi
         
         ```bash
         pip install --upgrade pip
         pip install backgroundremover
         ```
-        
+        Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will get them from u2net's google drive, as they say too [here](https://github.com/xuebinqin/U-2-Net#usage-for-salient-object-detection), and in this repo the code that pulls it is [here](https://github.com/nadermx/backgroundremover/blob/main/src/backgroundremover/utilities.py#L289)
         # Usage as a cli
         ## Image
         
         Remove the background from a local file image
         
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -o "output.png"
         ```
         
         ### Advance usage for image background removal
         
         Sometimes it is possible to achieve better results by turning on alpha matting. Example:
         
         ```bash
-        backgroundremover -i "/path/to/image.jpeg" a -ae 15 -o "output.png"
+        backgroundremover -i "/path/to/image.jpeg" -a -ae 15 -o "output.png"
         ```
         change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -m "u2net_human_seg" -o "output.png"
         ```
         ## Video
         
         ### remove background from video and make transparent mov
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -tv -o "output.mov"
         ```
         ### remove background from local video and overlay it over other video
         ```bash
-        backgroundremover -i "/path/to/video.mp4" -tov -tv "/path/to/videtobeoverlayed.mp4" -o "output.mov"
+        backgroundremover -i "/path/to/video.mp4" -tov "/path/to/videtobeoverlayed.mp4" -o "output.mov"
+        ```
+        ### remove background from local video and overlay it over an image
+        ```bash
+        backgroundremover -i "/path/to/video.mp4" -toi "/path/to/videtobeoverlayed.mp4" -o "output.mov"
         ```
         
         ### remove background from video and make transparent gif
         
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -tg -o "output.gif"
@@ -102,44 +113,57 @@
         
         Change the framerate of the video (default is set to 30)
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -fr 30 -tv -o "output.mov"
         ```
         
+        Set total number of frames of the video (default is set to -1, ie the remove background from full video)
+        
+        ```bash
+        backgroundremover -i "/path/to/video.mp4" -fl 150 -tv -o "output.mov"
+        ```
+        
         Change the gpu batch size of the video (default is set to 1)
         
         ```bash
-        backgroundremover -i "/path/to/video.mp4" -gp 4 -tv -o "output.mov"
+        backgroundremover -i "/path/to/video.mp4" -gb 4 -tv -o "output.mov"
         ```
         
         Change the number of workers working on video (default is set to 1)
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
         ```
-        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
+        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
         ```bash
-        backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg"-tv -o "output.mov"
+        backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
         ```
         
         ## Todo
         
         - convert logic from video to image to utilize more GPU on image removal
         - clean up documentation a bit more
         - add ability to adjust and give feedback images or videos to datasets
+        - add ability to realtime background removal for videos, for streaming
+        - finish flask server api
+        - add ability to use other models than u2net, ie your own.
         - other
         
         ### Pull requests
         
         Accepted
         
         ### If you like this library
         
-        Give a link to our project [BackgroundRemover.app](https://backgroundremover.app) or this git, telling people that you like it or use it.
+        Give a link to our project [BackgroundRemoverAI.com](https://backgroundremoverai.com) or this git, telling people that you like it or use it.
+        #### bitcoin
+        <a href="bitcoin:BC1Q80PSHGQGQR7WN3KAX59XWVMGQ9FTVWLA7DEW7W?label=backgroundremover&message=BackgroundRemover">bc1q80pshgqgqr7wn3kax59xwvmgq9ftvwla7dew7w</a>
+        
+        
         
         ### Reason for project
         
         We made it our own package after merging together parts of others, adding in a few features of our own via posting parts as bounty questions on superuser, etc.  As well as asked on hackernews earlier to open source the image part, so decided to add in video, and a bit more.
```

### Comparing `backgroundremover-0.1.9/src/backgroundremover.egg-info/SOURCES.txt` & `backgroundremover-0.2.0/backgroundremover/backgroundremover.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
-src/backgroundremover/__init__.py
-src/backgroundremover/bg.py
-src/backgroundremover/utilities.py
-src/backgroundremover.egg-info/PKG-INFO
-src/backgroundremover.egg-info/SOURCES.txt
-src/backgroundremover.egg-info/dependency_links.txt
-src/backgroundremover.egg-info/entry_points.txt
-src/backgroundremover.egg-info/requires.txt
-src/backgroundremover.egg-info/top_level.txt
-src/backgroundremover/cmd/__init__.py
-src/backgroundremover/cmd/cli.py
-src/backgroundremover/cmd/server.py
-src/backgroundremover/u2net/__init__.py
-src/backgroundremover/u2net/data_loader.py
-src/backgroundremover/u2net/detect.py
-src/backgroundremover/u2net/u2net.py
+backgroundremover/backgroundremover.egg-info/PKG-INFO
+backgroundremover/backgroundremover.egg-info/SOURCES.txt
+backgroundremover/backgroundremover.egg-info/dependency_links.txt
+backgroundremover/backgroundremover.egg-info/entry_points.txt
+backgroundremover/backgroundremover.egg-info/requires.txt
+backgroundremover/backgroundremover.egg-info/top_level.txt
+backgroundremover/cmd/__init__.py
+backgroundremover/cmd/cli.py
+backgroundremover/cmd/server.py
+backgroundremover/u2net/__init__.py
+backgroundremover/u2net/data_loader.py
+backgroundremover/u2net/detect.py
+backgroundremover/u2net/u2net.py
```

### Comparing `backgroundremover-0.1.9/src/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.0/backgroundremover/cmd/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import argparse
-import glob
 import os
 from distutils.util import strtobool
 from .. import utilities
 from ..bg import remove
-import torch
 
 
 def main():
     model_choices = ["u2net", "u2net_human_seg", "u2netp"]
 
     ap = argparse.ArgumentParser()
 
@@ -124,15 +122,15 @@
     ap.add_argument(
         "-toi",
         "--transparentvideooverimage",
         nargs="?",
         const=True,
         default=False,
         type=lambda x: bool(strtobool(x)),
-        help="Overlay transparent video over another video",
+        help="Overlay transparent video over another image",
     )
     ap.add_argument(
         "-tg",
         "--transparentgif",
         nargs="?",
         const=True,
         default=False,
@@ -185,56 +183,56 @@
         help="Path to the output",
     )
 
     args = ap.parse_args()
     if args.input.name.rsplit('.', 1)[1] in ['mp4', 'mov', 'webm', 'ogg', 'gif']:
         if args.mattekey:
             utilities.matte_key(os.path.abspath(args.output.name), os.path.abspath(args.input.name),
-                      worker_nodes=args.workernodes,
-                      gpu_batchsize=args.gpubatchsize,
-                      model_name=args.model,
-                      frame_limit=args.framelimit,
-                      framerate=args.framerate)
+                                worker_nodes=args.workernodes,
+                                gpu_batchsize=args.gpubatchsize,
+                                model_name=args.model,
+                                frame_limit=args.framelimit,
+                                framerate=args.framerate)
         elif args.transparentvideo:
             utilities.transparentvideo(os.path.abspath(args.output.name), os.path.abspath(args.input.name),
-                             worker_nodes=args.workernodes,
-                             gpu_batchsize=args.gpubatchsize,
-                             model_name=args.model,
-                             frame_limit=args.framelimit,
-                             framerate=args.framerate)
+                                       worker_nodes=args.workernodes,
+                                       gpu_batchsize=args.gpubatchsize,
+                                       model_name=args.model,
+                                       frame_limit=args.framelimit,
+                                       framerate=args.framerate)
         elif args.transparentvideoovervideo:
             utilities.transparentvideoovervideo(os.path.abspath(args.output.name), os.path.abspath(args.backgroundvideo.name),
-                                 os.path.abspath(args.input.name),
-                                 worker_nodes=args.workernodes,
-                                 gpu_batchsize=args.gpubatchsize,
-                                 model_name=args.model,
-                                 frame_limit=args.framelimit,
-                                 framerate=args.framerate)
+                                                os.path.abspath(args.input.name),
+                                                worker_nodes=args.workernodes,
+                                                gpu_batchsize=args.gpubatchsize,
+                                                model_name=args.model,
+                                                frame_limit=args.framelimit,
+                                                framerate=args.framerate)
         elif args.transparentvideooverimage:
             utilities.transparentvideooverimage(os.path.abspath(args.output.name), os.path.abspath(args.backgroundimage.name),
-                                 os.path.abspath(args.input.name),
-                                 worker_nodes=args.workernodes,
-                                 gpu_batchsize=args.gpubatchsize,
-                                 model_name=args.model,
-                                 frame_limit=args.framelimit,
-                                 framerate=args.framerate)
+                                                os.path.abspath(args.input.name),
+                                                worker_nodes=args.workernodes,
+                                                gpu_batchsize=args.gpubatchsize,
+                                                model_name=args.model,
+                                                frame_limit=args.framelimit,
+                                                framerate=args.framerate)
         elif args.transparentgif:
             utilities.transparentgif(os.path.abspath(args.output.name), os.path.abspath(args.input.name),
-                           worker_nodes=args.workernodes,
-                           gpu_batchsize=args.gpubatchsize,
-                           model_name=args.model,
-                           frame_limit=args.framelimit,
-                           framerate=args.framerate)
+                                     worker_nodes=args.workernodes,
+                                     gpu_batchsize=args.gpubatchsize,
+                                     model_name=args.model,
+                                     frame_limit=args.framelimit,
+                                     framerate=args.framerate)
         elif args.transparentgifwithbackground:
             utilities.transparentgifwithbackground(os.path.abspath(args.output.name), os.path.abspath(args.backgroundimage.name), os.path.abspath(args.input.name),
-                              worker_nodes=args.workernodes,
-                              gpu_batchsize=args.gpubatchsize,
-                              model_name=args.model,
-                              frame_limit=args.framelimit,
-                              framerate=args.framerate)
+                                                   worker_nodes=args.workernodes,
+                                                   gpu_batchsize=args.gpubatchsize,
+                                                   model_name=args.model,
+                                                   frame_limit=args.framelimit,
+                                                   framerate=args.framerate)
 
     else:
         print(args.output.name)
         r = lambda i: i.buffer.read() if hasattr(i, "buffer") else i.read()
         w = lambda o, data: o.buffer.write(data) if hasattr(o, "buffer") else o.write(data)
         w(
             args.output,
```

### Comparing `backgroundremover-0.1.9/src/backgroundremover/cmd/server.py` & `backgroundremover-0.2.0/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.1.9/src/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.0/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.1.9/src/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.0/backgroundremover/u2net/detect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import errno
 import os
 import sys
-import gdown
 import numpy as np
-import requests
 import torch
 from hsh.library.hash import Hasher
 from PIL import Image
 from torchvision import transforms
-from tqdm import tqdm
 
 from . import data_loader, u2net
 from .. import utilities
 
 def load_model(model_name: str = "u2net"):
     hasher = Hasher()
 
@@ -35,47 +32,48 @@
         net = u2net.U2NETP(3, 1)
         path = os.environ.get(
             "U2NETP_PATH",
             os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
         )
         if (
             not os.path.exists(path)
-            or hasher.md5(path) != "e4f636406ca4e2af789941e7f139ee2e"
+            #or hasher.md5(path) != "e4f636406ca4e2af789941e7f139ee2e"
         ):
-            utilities.download_file_from_google_drive(
-                model, path,
+            utilities.download_files_from_github(
+                path, model_name
             )
 
     elif model_name == "u2net":
         net = u2net.U2NET(3, 1)
         path = os.environ.get(
             "U2NET_PATH",
             os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
         )
         if (
             not os.path.exists(path)
-            or hasher.md5(path) != "09fb4e49b7f785c9f855baf94916840a"
+            #or hasher.md5(path) != "09fb4e49b7f785c9f855baf94916840a"
         ):
-            utilities.download_file_from_google_drive(
-                model, path,
+            utilities.download_files_from_github(
+                path, model_name
             )
 
     elif model_name == "u2net_human_seg":
         net = u2net.U2NET(3, 1)
         path = os.environ.get(
             "U2NET_PATH",
             os.path.expanduser(os.path.join("~", ".u2net", model_name + ".pth")),
         )
         if (
             not os.path.exists(path)
-            or hasher.md5(path) != "347c3d51b01528e5c6c071e3cff1cb55"
+            #or hasher.md5(path) != "347c3d51b01528e5c6c071e3cff1cb55"
         ):
-            utilities.download_file_from_google_drive(
-                model, path,
+            utilities.download_files_from_github(
+                path, model_name
             )
+
     else:
         print("Choose between u2net, u2net_human_seg or u2netp", file=sys.stderr)
 
     try:
         if torch.cuda.is_available():
             net.load_state_dict(torch.load(path))
             net.to(torch.device("cuda"))
```

### Comparing `backgroundremover-0.1.9/src/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.0/backgroundremover/u2net/data_loader.py`

 * *Files identical despite different names*

