# Comparing `tmp/PyMouseKey-1.0.2.tar.gz` & `tmp/PyMouseKey-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMouseKey-1.0.2.tar", last modified: Thu May  4 00:46:14 2023, max compression
+gzip compressed data, was "PyMouseKey-1.0.3.tar", last modified: Fri May  5 03:14:38 2023, max compression
```

## Comparing `PyMouseKey-1.0.2.tar` & `PyMouseKey-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 00:46:14.208606 PyMouseKey-1.0.2/
--rw-rw-rw-   0        0        0      434 2023-05-04 00:46:14.202652 PyMouseKey-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 00:46:14.196206 PyMouseKey-1.0.2/PyMouseKey.egg-info/
--rw-rw-rw-   0        0        0      434 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 00:46:14.000000 PyMouseKey-1.0.2/PyMouseKey.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 00:46:14.198190 PyMouseKey-1.0.2/pymousekey/
--rw-rw-rw-   0        0        0    17498 2023-05-04 00:44:56.000000 PyMouseKey-1.0.2/pymousekey/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 00:46:14.208606 PyMouseKey-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-05-04 00:29:46.000000 PyMouseKey-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:14:38.908499 PyMouseKey-1.0.3/
+-rw-rw-rw-   0        0        0      434 2023-05-05 03:14:38.902207 PyMouseKey-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 03:14:38.888221 PyMouseKey-1.0.3/PyMouseKey.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-05 03:14:38.000000 PyMouseKey-1.0.3/PyMouseKey.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-05 03:14:38.000000 PyMouseKey-1.0.3/PyMouseKey.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 03:14:38.000000 PyMouseKey-1.0.3/PyMouseKey.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 03:14:38.000000 PyMouseKey-1.0.3/PyMouseKey.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 03:14:38.891195 PyMouseKey-1.0.3/pymousekey/
+-rw-rw-rw-   0        0        0    17820 2023-05-04 22:18:12.000000 PyMouseKey-1.0.3/pymousekey/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 03:14:38.908997 PyMouseKey-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-05-05 03:14:31.000000 PyMouseKey-1.0.3/setup.py
```

### Comparing `PyMouseKey-1.0.2/pymousekey/__init__.py` & `PyMouseKey-1.0.3/pymousekey/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -330,23 +330,26 @@
 
 def dragTo(x=None, y=None, duration=0.0, _pause=True):
     """
     Performs a drag (mouse movement with mouse button down) to coordinates on screen\n
     
     x,y(int): are the coordinates your going to drag to from your current cursor position\n
     
-    Duration(int/float): is the time inbetween each mouse movement towards the new x & y coordinates, if 0 it moves instantly
+    Duration(int/float): is the time inbetween each mouse movement towards the new x & y coordinates, if 0 it moves almost instantly\n
+    
+    _pause is the sleep after every function call
     """
 
     start_x, start_y = getPos()
     duration = duration / 100
 
     distance = math.hypot(x - start_x, y - start_y)
 
     ii_ = Input_I()
+    
     ii_.mi = MouseInput(0, 0, 0, MOUSEEVENTF_LEFTDOWN, 0, ctypes.pointer(ctypes.c_ulong(0)))
     xx = Input(ctypes.c_ulong(0), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(xx), ctypes.sizeof(xx))
     if _pause:
         time.sleep(PAUSE)
 
     for i in range(1, int(distance)+1):
@@ -365,34 +368,47 @@
     if _pause:
         time.sleep(PAUSE)
 
 
 def moveTo(x=None, y=None, _pause=True):
     """
     Moves the mouse to the specified x and y coordinates\n
-    x,y(int): x,y(int): The coordinates your going to move to\n
-    _pause is the sleep after every keypress _pause=False to disable the pause
+    x,y(int): The coordinates your going to move to\n
+    _pause is the sleep after every function call
     
     """
     ii_ = Input_I()
     ii_.mi = MouseInput(int(65535 * x / screen_width), int(65535 * y / screen_height), 0, MOUSEEVENTF_MOVE | MOUSEEVENTF_ABSOLUTE, 0, ctypes.pointer(ctypes.c_ulong(0)))
     xx = Input(ctypes.c_ulong(0), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(xx), ctypes.sizeof(xx))
     if _pause:
         time.sleep(PAUSE)
 
 
+def moveRel(offsetX=0, offsetY=0, _pause=True):
+    """
+    Moves the mouse by a certain amount based off the x and y offsets\n
+    offsetX,offsetY(int): The amount of pixels your going to move\n
+    _pause is the sleep after every function call
+    
+    """
+
+    x, y = getPos()
+    moveTo(offsetX + x, offsetY + y, _pause)
+
+
 def click(x=None, y=None, interval=0.0, clicks=1, button=LEFT, _pause=True):
     """
     Performs a mouse click at the specified x and y coordinates\n
     If no x and y coordinates are specified perform a mouse click at your mouse location\n
     x,y(int): The coordinates your going to move to\n
     interval(float): The sleep after the mouse key has been pressed so you can set your own intervals per call\n
-    clicks(int): The amount of clicks you want to perform
-
+    clicks(int): The amount of clicks you want to perform\n
+    _pause is the sleep after every function call
+    
     """
     if x and y:
         moveTo(x,y)
 
     if button == LEFT:
         event = MOUSEEVENTF_LEFTCLICK
     elif button == RIGHT:
@@ -421,14 +437,15 @@
     click(x, y, interval, 3, button, _pause)
 
 
 def scroll(scrollAmount=1):
     """
     Sends a scroll input\n
     scrollAmount(int)\n
+    _pause is the sleep after every function call
     Positive numbers scroll upwards, negative numbers scroll downwards\n
 
     Sometimes games dont take the scroll data thats sent and just takes thes scroll input to scroll at a fixed amount so it may not work for some games
     
     """
     ii_ = Input_I()
     ii_.mi = MouseInput(0,0, scrollAmount*120, MOUSEEVENTF_WHEEL, 0, ctypes.pointer(ctypes.c_ulong(0)))
@@ -437,14 +454,15 @@
 
 
 def press(key, interval=0.0, _pause=True):
     """
     Performs a keypress, also supports side mouse buttons (xbutton1 and xbutton2)\n
     Key(string): The key/mouse button expected to be pressed\n
     interval(float): The sleep after the key has been pressed so you can set your own intervals per call\n
+    _pause is the sleep after every function call\n
     pymousekey.KEYS for the dict of keys
 
     """
     if not key.lower() in KEYS or KEYS[key.lower()] is None:
         return
     ii_ = Input_I()
     
@@ -455,16 +473,16 @@
         return
     
     if str(key).isupper():
         ii_.ki = KeyBdInput(0, KEYS['shift'], KEYEVENTF_SCANCODE, 0, ctypes.pointer(ctypes.c_ulong(0)))
         x = Input(ctypes.c_ulong(1), ii_)
         ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
     
-    keyDown(key.lower())
-    keyUp(key.lower())
+    keyDown(key)
+    keyUp(key)
     
     if str(key).isupper():
         ii_.ki = KeyBdInput(0, KEYS['shift'], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
         x = Input(ctypes.c_ulong(1), ii_)
         ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
     
     time.sleep(interval)
@@ -473,65 +491,60 @@
 
 
 def keyDown(key):
     if not key.lower() in KEYS or KEYS[key.lower()] is None:
         return
 
     ii_ = Input_I()
-    ii_.ki = KeyBdInput(0, KEYS[key], KEYEVENTF_SCANCODE, 0, ctypes.pointer(ctypes.c_ulong(0)))
+    ii_.ki = KeyBdInput(0, KEYS[key.lower()], KEYEVENTF_SCANCODE, 0, ctypes.pointer(ctypes.c_ulong(0)))
     x = Input(ctypes.c_ulong(1), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
 
 
 def keyUp(key):
     if not key.lower() in KEYS or KEYS[key.lower()] is None:
         return
 
     ii_ = Input_I()
-    ii_.ki = KeyBdInput(0, KEYS[key], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
+    ii_.ki = KeyBdInput(0, KEYS[key.lower()], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
     x = Input(ctypes.c_ulong(1), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
 
 
 def typeWrite(message, interval=0.0, _pause=True):
     """
     Types out a given message, letters suppors lowercase and uppercase letters\n
     message(str): The message you want typed out\n
     interval(float): The sleep after the key has been pressed so you can set your own intervals per call\n
-    _pause(bool): The sleep inbetween each keypress, True for pauses False for no pauses
+    _pause is the sleep after every function call
 
     """
     for i in message:
-        if i.isupper():
-            press(i, interval, _pause)
-        elif i.islower():
-            press(i, interval, _pause)
-        elif i == ' ':
-            press(i, interval, _pause)
+        press(i, interval, _pause)
 
 
 def getPixelColor(x=None, y=None):
     """
-    Gets the color from the specified x and y coordinates, if no coordinates are specified grab the color at your mouse coordinates\n
+    Gets the color from the specified coordinates, if no coordinates are specified grab the color from your mouse coordinates\n
     Returns:
     ----
     hexColor & rgbColor
     
     """
     dc = ctypes.windll.user32.GetDC(None)
     if not (x and y):
         x,y = getPos()
         color = ctypes.windll.gdi32.GetPixel(dc, x, y)
     else:
         color = ctypes.windll.gdi32.GetPixel(dc, x, y)
 
+    ctypes.windll.user32.ReleaseDC(None,dc)
     red = color & 0xff
     green = (color >> 8) & 0xff
     blue = (color >> 16) & 0xff
-    ctypes.windll.user32.ReleaseDC(None,dc)
     hexColor = '#{:02x}{:02x}{:02x}'.format(red,green,blue)
     rgbColor = red, green, blue
     return hexColor, rgbColor
 
 
 def controlSend(key=None, className=None, windowTitle=None, lparam=None):
     """
@@ -575,10 +588,8 @@
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONDOWN, MK_RBUTTON, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_RBUTTONUP, MK_RBUTTON, lparam)
 
     elif button == 'middle':
         ctypes.windll.user32.PostMessageW(handle, WM_NCHITTEST, 0, lparam)
         ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONDOWN, MK_MBUTTON, lparam)
-        ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
-
-
+        ctypes.windll.user32.PostMessageW(handle, WM_MBUTTONUP, MK_MBUTTON, lparam)
```

### Comparing `PyMouseKey-1.0.2/setup.py` & `PyMouseKey-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'A python package for sending keyboard and mouse inputs'
 LONG_DESCRIPTION = 'pymousekey is made for sending keyboard and mouse inputs simular to how pyautogui does but using the ctypes module only\nKeep in mid their is no failsafe wrapper for any function so use with caution\nNo extra dependencies are needed to use this module'
 
 
 setuptools.setup(
     name="PyMouseKey",
     version=VERSION,
```

