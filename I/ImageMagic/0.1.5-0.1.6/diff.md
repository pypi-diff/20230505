# Comparing `tmp/ImageMagic-0.1.5.tar.gz` & `tmp/ImageMagic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.1.5.tar", last modified: Thu May  4 13:03:12 2023, max compression
+gzip compressed data, was "ImageMagic-0.1.6.tar", last modified: Fri May  5 10:55:03 2023, max compression
```

## Comparing `ImageMagic-0.1.5.tar` & `ImageMagic-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/ImageMagic/
--rw-rw-rw-   0        0        0     6184 2023-05-04 12:40:18.000000 ImageMagic-0.1.5/ImageMagic/Aocr.py
--rw-rw-rw-   0        0        0    10110 2023-05-04 09:07:20.000000 ImageMagic-0.1.5/ImageMagic/Image.py
--rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.5/ImageMagic/_Atesseract.py
--rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.5/ImageMagic/__init__.py
--rw-rw-rw-   0        0        0       85 2023-05-04 09:25:12.000000 ImageMagic-0.1.5/ImageMagic/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0      245 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      245 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2023-05-04 09:42:24.000000 ImageMagic-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-05-04 13:03:00.000000 ImageMagic-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-05-05 10:55:03.091027 ImageMagic-0.1.6/ImageMagic/
+-rw-rw-rw-   0        0        0     6184 2023-05-04 12:40:18.000000 ImageMagic-0.1.6/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    11530 2023-05-05 10:43:04.000000 ImageMagic-0.1.6/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.6/ImageMagic/_Atesseract.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.6/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-05 10:54:35.000000 ImageMagic-0.1.6/ImageMagic/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-05 10:55:03.000000 ImageMagic-0.1.6/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 10:55:02.000000 ImageMagic-0.1.6/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      500 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1096 2023-05-05 10:54:35.000000 ImageMagic-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 10:55:03.106652 ImageMagic-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      778 2023-05-05 10:53:04.000000 ImageMagic-0.1.6/setup.py
```

### Comparing `ImageMagic-0.1.5/ImageMagic/Aocr.py` & `ImageMagic-0.1.6/ImageMagic/Aocr.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.5/ImageMagic/Image.py` & `ImageMagic-0.1.6/ImageMagic/Image.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,14 +103,62 @@
         None
     """
 
     image = PILImage.open(originFilePath).convert(mode=mode)
     image.save(savePath,format=format)
 
 
+def equal_scale_image(filePath,savePath,multiple=1):
+
+    """
+    Change your image in equal proportions
+    Args:
+        filePath: Original file path
+        savePath: The path to the save
+        multiple: The multiplier of the change
+
+    Returns:
+        None
+    """
+
+    img = PILImage.open(filePath)
+    width = img.size[0]
+    height = img.size[1]
+    img = img.resize((int(width * multiple), int(height * multiple)), PILImage.Resampling.LANCZOS)
+    img.save(savePath)
+
+
+def customize_image(filePath,savePath,new_width=None,new_height=None):
+
+    """
+    Custom image size (if no input is used, the original parameter will be used)
+    Args:
+        filePath: Original file path
+        savePath: The path to the save
+        new_width: width
+        new_height: height
+
+    Returns:
+        None
+    """
+
+    img = PILImage.open(filePath)
+    width = img.size[0]
+    height = img.size[1]
+    if new_width is None:
+        img = img.resize((int(width), int(new_height)), PILImage.Resampling.LANCZOS)
+    if new_height is None:
+        img = img.resize((int(new_width,int(height)),PILImage.Resampling.LANCZOS))
+    if new_width is None and new_height is None:
+        img = img.resize((int(width),int(height)),PILImage.Resampling.LANCZOS)
+    else:
+        img = img.resize((int(new_width),int(new_height)),PILImage.Resampling.LANCZOS)
+    img.save(savePath)
+
+
 def categorize_image(filePath):
 
     """
     Categorize your images, support jpg, jpeg, png, webp, bmp, tif, tiff, gif, svg, wmf
     Args:
         filePath: Your folder path
 
@@ -172,14 +220,15 @@
         else:
             try:
                 os.makedirs(f'{filePath}/another')
             except FileExistsError as error:
                 pass
             shutil.copy(os.path.join(filePath,filename),f'{filePath}/another')
 
+
 class Audio:
 
     """
     You need to pass in the appid, secret-key, and path to the audio file
     """
 
     def __init__(self,appid,key,upload_file_path):
```

### Comparing `ImageMagic-0.1.5/ImageMagic/_Atesseract.py` & `ImageMagic-0.1.6/ImageMagic/_Atesseract.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.5/LICENSE` & `ImageMagic-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.5/README.md` & `ImageMagic-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <div align="center">
   <img src="https://i.328888.xyz/2023/05/04/iPlOg8.png" width="500" height="450"><br>
 </div>
 
+[DOCS in English](https://github.com/asxez/ImageMagic/blob/master/README_EN.md)
+
 # ImageMagic:一个简洁的图像（包括但不限于）处理库
-[![Pypi](https://img.shields.io/badge/pypi-0.1.3-blue)]()
-[![License](https://img.shields.io/badge/license-MIT-yellow)]()
+[![Pypi](https://img.shields.io/badge/pypi-0.1.6-blue)]()
+[![License](https://img.shields.io/badge/license-GPL3.0-yellow)]()
 [![]()]()
 
 # 这是什么？
 ImageMagic是Python的一个包，提供简洁的图像（包括但不限于）处理功能，主要体现为简洁二字。
 
 # 获取
 1. 使用pip下载
@@ -22,11 +24,11 @@
   - [PIL](https://github.com/python-pillow/Pillow)
   - [Tesseract-OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
   - [numpy](https://github.com/numpy/numpy)
   - [pandas](https://github.com/pandas-dev/pandas)
   - ……
 
 # 许可证
-GNU GPL
+GNU GPL 3.0
 
 # 为ImageMagic做贡献
 欢迎所有贡献、错误报告、错误修复以及功能增强和想法。
```

