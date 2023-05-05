# Comparing `tmp/aij-webcam-1.1.1.tar.gz` & `tmp/aij-webcam-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.1.1.tar", last modified: Fri May  5 12:52:13 2023, max compression
+gzip compressed data, was "aij-webcam-1.1.2.tar", last modified: Fri May  5 13:14:29 2023, max compression
```

## Comparing `aij-webcam-1.1.1.tar` & `aij-webcam-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.1/README.md
--rw-rw-rw-   0        0        0     6368 2023-05-05 12:52:02.000000 aij-webcam-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      175 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.1/src/news/__init__.py
--rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.1/src/news/core.py
--rw-rw-rw-   0        0        0     3663 2023-05-05 12:51:30.000000 aij-webcam-1.1.1/src/news/publisher.py
--rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.1/src/news/subscriber.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:52:14.000000 aij-webcam-1.1.1/src/webcam/
--rw-rw-rw-   0        0        0    16936 2023-05-05 12:22:56.000000 aij-webcam-1.1.1/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.2/README.md
+-rw-rw-rw-   0        0        0     6368 2023-05-05 13:14:18.000000 aij-webcam-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      175 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.2/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.2/src/news/core.py
+-rw-rw-rw-   0        0        0     3663 2023-05-05 12:51:30.000000 aij-webcam-1.1.2/src/news/publisher.py
+-rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.2/src/news/subscriber.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:30.000000 aij-webcam-1.1.2/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-05 13:14:12.000000 aij-webcam-1.1.2/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.1.1/LICENSE.txt` & `aij-webcam-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.1/PKG-INFO` & `aij-webcam-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.1
+Version: 1.1.2
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.1/README.md` & `aij-webcam-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.1/pyproject.toml` & `aij-webcam-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.1"
+version = "1.1.2"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.1.1/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.1.2/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.1
+Version: 1.1.2
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.1/src/news/__init__.py` & `aij-webcam-1.1.2/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.1/src/news/core.py` & `aij-webcam-1.1.2/src/news/core.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.1/src/news/publisher.py` & `aij-webcam-1.1.2/src/news/publisher.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.1/src/news/subscriber.py` & `aij-webcam-1.1.2/src/news/subscriber.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.1/src/webcam/__init__.py` & `aij-webcam-1.1.2/src/webcam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,26 @@
     api_key = os.environ['WEATHERAPI_COM']
     region = os.environ['WEATHERAPI_COM_REGION']
     response = requests.get(
         f'http://api.weatherapi.com/v1/current.json?key={api_key}&q={region}&aqi=no'
     )
     return response.json()
 
+def get_weather_temp_c(weather):
+    """
+    Get the temperature in Celsius
+    """
+    return weather['current']['temp_c']
+
+def get_weather_temp_f(weather):
+    """
+    Get the temperature in Fahrenheit
+    """
+    return weather['current']['temp_f']
+
 def get_weather_to_df(weather):
     """
     Convert the weather to a dataframe
     """
     # map all the articles to a list
     current = weather['current']
 
@@ -159,15 +171,15 @@
     weather_df = pd.DataFrame()
     weather_df['temp_c'] = [0]
     weather_df['temp_f'] = [0]
     weather_df['condition'] = ['']
 
 
 titles = news_df['title'].str.cat(sep=' ') + ' ... |'
-weather = f"{weather_df['temp_c'][0]}°C | {weather_df['temp_f'][0]}°F | {weather_df['condition'][0]}"
+weather = f"{weather_df['temp_c'][0]}c"
 
 # Using OpenCV to display the image
 cap = cv2.VideoCapture(0)
 cap.set(cv2.CAP_PROP_FRAME_WIDTH, SCREEN_WIDTH)
 cap.set(cv2.CAP_PROP_FRAME_HEIGHT, SCREEN_HEIGHT)
 cap.set(cv2.CAP_PROP_FPS, SCREEN_FPS)
 
@@ -258,20 +270,31 @@
     mixer.music.forward()
 
 
 def draw_text(image, x, y, text, color):
     """
     Draw text on the image
     """
+    # draw a black rectangle on the image
+    cv2.rectangle(
+        image,
+        (x, y - 25),
+        # until the end of screen width
+        (x + image.shape[1], y),
+        (0, 0, 0),
+        -1
+    )
+
+    # draw the text on the image
     cv2.putText(
         image,
         text,
         (x, y),
         cv2.FONT_HERSHEY_SIMPLEX,
-        font_size,
+        font_size / 12,
         color,
         2,
         cv2.LINE_AA
     )
 
 
 def draw_box(image, x, y, color):
@@ -430,19 +453,20 @@
             titles = titles[1:] + titles[0]
         elif direction == 1:
             titles = titles[-1] + titles[:-1]
         elif direction == 2:
             pass
 
         # draw the text
-        draw_text(image, 0, 40, titles, color)
+        draw_text(image, 2, image.shape[0] - 10, titles, color)
 
         # draw the weather on the image if the weather is available
         if weather_df['temp_c'][0] != 0:
-            draw_text(image, 0, 20, weather, color)
+            # set the position of the weather to the right top corner
+            draw_text(image, image.shape[1] - 250, 30, weather, color)
 
         # if there is a logo then draw it
         if os.path.exists(logo_abs):
             logo = cv2.imread(logo_abs)
             # Resize the logo to match the height of the main image and keep the aspect ratio
             # resize the logo to 100px height and keep the aspect ratio
             logo_resized = cv2.resize(logo, (100, 100), interpolation=cv2.INTER_AREA)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

