# Comparing `tmp/prodia-python-2.1.tar.gz` & `tmp/prodia-python-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodia-python-2.1.tar", last modified: Thu May  4 11:25:10 2023, max compression
+gzip compressed data, was "prodia-python-2.2.tar", last modified: Fri May  5 14:29:49 2023, max compression
```

## Comparing `prodia-python-2.1.tar` & `prodia-python-2.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 11:25:10.723214 prodia-python-2.1/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-2.1/LICENSE
--rw-rw-rw-   0        0        0     2010 2023-05-04 11:25:10.722539 prodia-python-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1784 2023-05-04 11:03:56.000000 prodia-python-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 11:25:10.707355 prodia-python-2.1/prodia/
--rw-rw-rw-   0        0        0       76 2023-05-04 10:55:14.000000 prodia-python-2.1/prodia/__init__.py
--rw-rw-rw-   0        0        0     4782 2023-05-04 10:55:14.000000 prodia-python-2.1/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:25:10.721336 prodia-python-2.1/prodia_python.egg-info/
--rw-rw-rw-   0        0        0     2010 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 11:25:10.000000 prodia-python-2.1/prodia_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 11:25:10.723214 prodia-python-2.1/setup.cfg
--rw-rw-rw-   0        0        0      401 2023-05-04 11:24:52.000000 prodia-python-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:29:49.383146 prodia-python-2.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-2.2/LICENSE
+-rw-rw-rw-   0        0        0     2354 2023-05-05 14:29:49.382596 prodia-python-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2128 2023-05-05 12:19:03.000000 prodia-python-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 14:29:49.372146 prodia-python-2.2/prodia/
+-rw-rw-rw-   0        0        0       95 2023-05-05 14:08:13.000000 prodia-python-2.2/prodia/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-05-05 10:09:12.000000 prodia-python-2.2/prodia/data.py
+-rw-rw-rw-   0        0        0     5249 2023-05-05 11:51:07.000000 prodia-python-2.2/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:29:49.381147 prodia-python-2.2/prodia_python.egg-info/
+-rw-rw-rw-   0        0        0     2354 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:29:49.383146 prodia-python-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-05-05 12:19:48.000000 prodia-python-2.2/setup.py
```

### Comparing `prodia-python-2.1/LICENSE` & `prodia-python-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prodia-python-2.1/PKG-INFO` & `prodia-python-2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 2.1
+Version: 2.2
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodia-python==2.0
+pip install prodia-python==2.2
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-image = prodia.txt2img(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+prodia.Client(api_key=key)
+
+image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 ### Example of img2img usage
 ```python
 import prodia
 
 key = 'your-prodia-key'
 
+prodia.Client(api_key=key)
+
 image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
 
-image = prodia.img2img(key=key, imageUrl=image_url, prompt="winter nature wallpaper")
+image = prodia.img2img(imageUrl=image_url, prompt="winter nature wallpaper")
 
 print(image)
 ```
 
 ### Additional info
-prodia.run() have arguments:
-- `key` - string Prodia API key(required)
-- `prompt` - string prompt for image(default is "kittens on cloud")
-- `negative_prompt` - string for negative tags(default is "badly drawn")
-- `model` - string(you can check full list of available models on https://docs.prodia.com/reference/generate, default is deliberate_v2.safetensors [10ec4b29])
-- `aspect_ratio` - string(square, portrait, landscape, default is square)
-- `steps` - integer, 1-50, default is 25
-- `cfg_scale` - integer, 1-20, default is 7
-- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Heun)
-- `seed` - integer(default -1, it generates images with random seed)
-- `upscale` - boolean of 2x upscaling(default False)
+
+All available arguments for txt2img():
+- prompt:str(required)
+- negative_prompt:str
+- model:str check all available models on https://docs.prodia.com/reference/generate
+- sampler:str check all available samplers on https://docs.prodia.com/reference/generate
+- steps:int from 1 to 50
+- cfg_scale:int from 1 to 20
+- seed:int leave blank for random(or use -1 for random)
+- upscale:bool Enable/Disable 2x upscaling of image
+- aspect_ratio:str available: "square", "landscape", "portrait"
+
+All available arguments for img2img():
+- imageUrl:str(required)
+- model:str check all available models on https://docs.prodia.com/reference/generate
+- sampler:str check all available samplers on https://docs.prodia.com/reference/generate
+- prompt:str(required)
+- denoising_strength:float default is 0.7
+- negative_prompt:str
+- steps:int from 1 to 50
+- cfg_scale:int from 1 to 20
+- seed:int leave blank for random(or use -1 for random)
+- upscale:bool Enable/Disable 2x upscaling of image
+
+Feel free to join out [Discord server](https://discord.gg/eAcrtqaE) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodia-python-2.1/README.md` & `prodia-python-2.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,67 @@
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodia-python==2.0
+pip install prodia-python==2.2
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-image = prodia.txt2img(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+prodia.Client(api_key=key)
+
+image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 ### Example of img2img usage
 ```python
 import prodia
 
 key = 'your-prodia-key'
 
+prodia.Client(api_key=key)
+
 image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
 
-image = prodia.img2img(key=key, imageUrl=image_url, prompt="winter nature wallpaper")
+image = prodia.img2img(imageUrl=image_url, prompt="winter nature wallpaper")
 
 print(image)
 ```
 
 ### Additional info
-prodia.run() have arguments:
-- `key` - string Prodia API key(required)
-- `prompt` - string prompt for image(default is "kittens on cloud")
-- `negative_prompt` - string for negative tags(default is "badly drawn")
-- `model` - string(you can check full list of available models on https://docs.prodia.com/reference/generate, default is deliberate_v2.safetensors [10ec4b29])
-- `aspect_ratio` - string(square, portrait, landscape, default is square)
-- `steps` - integer, 1-50, default is 25
-- `cfg_scale` - integer, 1-20, default is 7
-- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Heun)
-- `seed` - integer(default -1, it generates images with random seed)
-- `upscale` - boolean of 2x upscaling(default False)
+
+All available arguments for txt2img():
+- prompt:str(required)
+- negative_prompt:str
+- model:str check all available models on https://docs.prodia.com/reference/generate
+- sampler:str check all available samplers on https://docs.prodia.com/reference/generate
+- steps:int from 1 to 50
+- cfg_scale:int from 1 to 20
+- seed:int leave blank for random(or use -1 for random)
+- upscale:bool Enable/Disable 2x upscaling of image
+- aspect_ratio:str available: "square", "landscape", "portrait"
+
+All available arguments for img2img():
+- imageUrl:str(required)
+- model:str check all available models on https://docs.prodia.com/reference/generate
+- sampler:str check all available samplers on https://docs.prodia.com/reference/generate
+- prompt:str(required)
+- denoising_strength:float default is 0.7
+- negative_prompt:str
+- steps:int from 1 to 50
+- cfg_scale:int from 1 to 20
+- seed:int leave blank for random(or use -1 for random)
+- upscale:bool Enable/Disable 2x upscaling of image
+
+Feel free to join out [Discord server](https://discord.gg/eAcrtqaE) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodia-python-2.1/prodia/main.py` & `prodia-python-2.2/prodia/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import requests
 import time
 import os
 
+
+api_key = None
+log=True
+
+def Client(api_key:str=None):
+    if api_key is None:
+        print("No API key provided")
+        return
+    else:
+        global key
+        key = api_key
+
+
 def txt2img(
-        key:str=None,
         prompt:str="kittens on cloud",
         negative_prompt:str="bad drawn, low quality, low detailed, ugly, mutated, blurry, watermark",
         model:str="deliberate_v2.safetensors [10ec4b29]",
         sampler:str="Heun",
         aspect_ratio:str="square",
         steps:int=25,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False):
     if key is None:
-        print("API key cant be None, get your API kay at https://app.prodia.com/api")
+        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
     else:
         if prompt == "kittens on cloud":
-            print("Prompt wasnt not defined, used default (kittens on cloud)")
+            print("LOG: Prompt was not defined, used default (kittens on cloud)" if log is True else "")
         url = "https://api.prodia.com/v1/job"
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
@@ -35,58 +47,59 @@
             "content-type": "application/json",
             "X-Prodia-Key": key
         }
         headersrecieve = {
             "accept": "application/json",
             "X-Prodia-Key": key
         }
-        print(f"txt2img image with params:\n{payload}")
+        print(f"LOG: txt2img image with params:\n{payload}" if log is True else "")
         response = requests.post(url, json=payload, headers=headers)
         job_id = response.json()['job']
-        time.sleep(5)
+        time.sleep(3)
 
         rec_url = f'https://api.prodia.com/v1/job/{job_id}'
         stt = True
         while stt is True:
             rec = requests.get(rec_url, headers=headersrecieve)
             status = rec.json()['status']
             if status == "succeeded":
-                print(f"Image {job_id} generated!")
+                print(f"Image {job_id} generated!" if log is True else "")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
-                time.sleep(5)
+                time.sleep(2)
             elif status == "generating":
                 print("Still working...")
-                time.sleep(5)
+                time.sleep(2)
             else:
-                print(f"Something went wrong! Please try later, error: {status}")
+                print(f"ERROR: Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
+
 def img2img(
-        key:str=None,
         imageUrl:str=None,
         model:str="deliberate_v2.safetensors [10ec4b29]",
         prompt:str=None,
         denoising_strength:float=0.7,
         negative_prompt:str="badly drawn, low detailed, ugly, mutated, unralistic",
         steps:int=25,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False,
         sampler:str="Heun"):
+
     if key is None:
-        print("API key cant be None, get your API kay at https://app.prodia.com/api")
+        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
     elif imageUrl is None:
-        print("Image URL is required and cannot be empty")
+        print("ERROR: Image URL is required and cannot be empty")
     elif prompt is None:
-        print("Prompt is required and cannot be empty")
+        print("ERROR: Prompt is required and cannot be empty")
     else:
         url = "https://api.prodia.com/v1/transform"
 
         payload = {
             "steps": steps,
             "sampler": sampler,
             "imageUrl": imageUrl,
@@ -103,35 +116,35 @@
             "content-type": "application/json",
             "X-Prodia-Key": key
         }
         headersrecieve = {
             "accept": "application/json",
             "X-Prodia-Key": key
         }
-        print(f"img2img image with params:\n{payload}")
+        print(f"LOG: img2img image with params:\n{payload}" if log is True else "")
         response = requests.post(url, json=payload, headers=headers)
         job_id = response.json()['job']
         time.sleep(5)
 
         rec_url = f'https://api.prodia.com/v1/job/{job_id}'
         stt = True
         while stt is True:
             rec = requests.get(rec_url, headers=headersrecieve)
             status = rec.json()['status']
             if status == "succeeded":
-                print(f"Image {job_id} generated!")
+                print(f"LOG: Image {job_id} generated!" if log is True else "")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
                 time.sleep(5)
             elif status == "generating":
                 print("Still working...")
                 time.sleep(5)
             else:
-                print(f"Something went wrong! Please try later, error: {status}")
+                print(f"ERROR: Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
```

### Comparing `prodia-python-2.1/prodia_python.egg-info/PKG-INFO` & `prodia-python-2.2/prodia_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 2.1
+Version: 2.2
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodia-python==2.0
+pip install prodia-python==2.2
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-image = prodia.txt2img(key=key, prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
+prodia.Client(api_key=key)
+
+image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 ### Example of img2img usage
 ```python
 import prodia
 
 key = 'your-prodia-key'
 
+prodia.Client(api_key=key)
+
 image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
 
-image = prodia.img2img(key=key, imageUrl=image_url, prompt="winter nature wallpaper")
+image = prodia.img2img(imageUrl=image_url, prompt="winter nature wallpaper")
 
 print(image)
 ```
 
 ### Additional info
-prodia.run() have arguments:
-- `key` - string Prodia API key(required)
-- `prompt` - string prompt for image(default is "kittens on cloud")
-- `negative_prompt` - string for negative tags(default is "badly drawn")
-- `model` - string(you can check full list of available models on https://docs.prodia.com/reference/generate, default is deliberate_v2.safetensors [10ec4b29])
-- `aspect_ratio` - string(square, portrait, landscape, default is square)
-- `steps` - integer, 1-50, default is 25
-- `cfg_scale` - integer, 1-20, default is 7
-- `sampler` - string(you can see all available samplers on https://docs.prodia.com/reference/generate, default is Heun)
-- `seed` - integer(default -1, it generates images with random seed)
-- `upscale` - boolean of 2x upscaling(default False)
+
+All available arguments for txt2img():
+- prompt:str(required)
+- negative_prompt:str
+- model:str check all available models on https://docs.prodia.com/reference/generate
+- sampler:str check all available samplers on https://docs.prodia.com/reference/generate
+- steps:int from 1 to 50
+- cfg_scale:int from 1 to 20
+- seed:int leave blank for random(or use -1 for random)
+- upscale:bool Enable/Disable 2x upscaling of image
+- aspect_ratio:str available: "square", "landscape", "portrait"
+
+All available arguments for img2img():
+- imageUrl:str(required)
+- model:str check all available models on https://docs.prodia.com/reference/generate
+- sampler:str check all available samplers on https://docs.prodia.com/reference/generate
+- prompt:str(required)
+- denoising_strength:float default is 0.7
+- negative_prompt:str
+- steps:int from 1 to 50
+- cfg_scale:int from 1 to 20
+- seed:int leave blank for random(or use -1 for random)
+- upscale:bool Enable/Disable 2x upscaling of image
+
+Feel free to join out [Discord server](https://discord.gg/eAcrtqaE) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

