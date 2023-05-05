# Comparing `tmp/styledlogger-0.0.4.tar.gz` & `tmp/styledlogger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styledlogger-0.0.4.tar", last modified: Sat Apr 22 11:39:24 2023, max compression
+gzip compressed data, was "styledlogger-0.0.5.tar", last modified: Fri May  5 15:21:54 2023, max compression
```

## Comparing `styledlogger-0.0.4.tar` & `styledlogger-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-22 11:39:14.000000 styledlogger-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-22 11:39:24.119378 styledlogger-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-22 11:39:14.000000 styledlogger-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 11:39:24.119378 styledlogger-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 11:39:14.000000 styledlogger-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/styledlogger/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/styledlogger/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/printcolors.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/printtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/classes/styleconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-22 11:39:14.000000 styledlogger-0.0.4/styledlogger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:39:24.119378 styledlogger-0.0.4/styledlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 11:39:24.000000 styledlogger-0.0.4/styledlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 15:21:41.000000 styledlogger-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-05 15:21:54.656999 styledlogger-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 15:21:41.000000 styledlogger-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:21:54.656999 styledlogger-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-05 15:21:41.000000 styledlogger-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/styledlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/styledlogger/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/printcolors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/printtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/classes/styleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-05 15:21:41.000000 styledlogger-0.0.5/styledlogger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:21:54.656999 styledlogger-0.0.5/styledlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 15:21:54.000000 styledlogger-0.0.5/styledlogger.egg-info/top_level.txt
```

### Comparing `styledlogger-0.0.4/LICENSE` & `styledlogger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.4/PKG-INFO` & `styledlogger-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -14,33 +14,35 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # StyledLogger
 
 ### A simple - yet beautiful logging library for Python 🐍 > 3.7
 
-To use, simply do `pip install styledlogger`
+To use, simply install via `pip install styledlogger`
 
-Then you can import `StyledLogger` from the package and initialize it.
+Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
 
 >>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug
+>>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
 
 >>> logger.debug("This is just a test print")
 9:55:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
+
 >>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+
 >>> logger.warn("CPU usage exceeding 90%")
 (22/04/2023 10:01) | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.4/README.md` & `styledlogger-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # StyledLogger
 
 ### A simple - yet beautiful logging library for Python 🐍 > 3.7
 
-To use, simply do `pip install styledlogger`
+To use, simply install via `pip install styledlogger`
 
-Then you can import `StyledLogger` from the package and initialize it.
+Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
 
 >>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug
+>>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
 
 >>> logger.debug("This is just a test print")
 9:55:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
+
 >>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+
 >>> logger.warn("CPU usage exceeding 90%")
 (22/04/2023 10:01) | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

### Comparing `styledlogger-0.0.4/setup.py` & `styledlogger-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     # Basics
     name='styledlogger',
-    version='0.0.4',
+    version='0.0.5',
     description='A simple, styled logging library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    
+
     # Author
     author='ImAlek (splayzdk)',
     author_email='alek@imalek.me',
-    
+
     # Package
     packages=find_packages(),
     url='https://github.com/SpLayzDK/StyledLogger/',
 
     # License
     license='BSL 1.0',
     classifiers = [
```

### Comparing `styledlogger-0.0.4/styledlogger/classes/printcolors.py` & `styledlogger-0.0.5/styledlogger/classes/printcolors.py`

 * *Files identical despite different names*

### Comparing `styledlogger-0.0.4/styledlogger/classes/styleconfig.py` & `styledlogger-0.0.5/styledlogger/classes/styleconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .printcolors import Colors
 from arrow import now
 
-from .printtypes import Debug, Info, Warn, Error, Fatal, PrintType
+from .printtypes import Debug, Info, Warn, Error, Fatal, System, PrintType
 
 
 class StyleConfig:
     """
     The style configuration for the logger.
 
     :param time_format: The format of the time.
@@ -24,26 +24,28 @@
         name_color: str = "reset",
         text_color: str | None = None,
         debug_color: str = "yellow",
         info_color: str = "green",
         warn_color: str = "brown",
         error_color: str = "red",
         fatal_color: str = "purple",
+        system_color: str = "cyan",
     ) -> None:
         self.text_format = text_format
         self.time_format = time_format
         self.time_color = self._validate_color(time_color)
         self.name_color = self._validate_color(name_color)
         self.text_color = self._validate_color(text_color) if text_color else Colors.RESET
 
         self.debug_color = self._validate_color(debug_color)
         self.info_color = self._validate_color(info_color)
         self.warn_color = self._validate_color(warn_color)
         self.error_color = self._validate_color(error_color)
         self.fatal_color = self._validate_color(fatal_color)
+        self.system_color = self._validate_color(system_color)
 
         self.reset = Colors.RESET
 
     def _validate_color(self, color: str) -> None:
         try:
             color = getattr(Colors, color.upper())
 
@@ -70,14 +72,16 @@
             type_color = self.info_color
         elif print_type == Warn:
             type_color = self.warn_color
         elif print_type == Error:
             type_color = self.error_color
         elif print_type == Fatal:
             type_color = self.fatal_color
+        elif print_type == System:
+            type_color = self.system_color
 
         format_blueprint = self.text_format
 
         replacemap = {
             "%name%": self.name_color + logger_name + self.reset,
             "%time%": self.time_color + now().format(self.time_format) + self.reset,
             "%type%": type_color + str(print_type.display) + self.reset,
```

### Comparing `styledlogger-0.0.4/styledlogger/logger.py` & `styledlogger-0.0.5/styledlogger/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from colorama import (
     just_fix_windows_console,
 )
 
 from .classes.styleconfig import StyleConfig
-from .classes.printtypes import Debug, Info, Warn, Error, Fatal
+from .classes.printtypes import Debug, Info, Warn, Error, Fatal, System
 
 just_fix_windows_console()
 
 
 class Logger:
     """
     The main object for logging.
@@ -22,68 +22,74 @@
         self.level = level
         self.is_muted = False
         self.file = file # TODO: Implement file logging
         self.style_config = StyleConfig() 
 
     def set_level(self, level):
         """
-        Set the log level
+        Set the log level. 0 = debug, 1 = info, 2 = warn, 3 = error, 4 = fatal. All prints lower than the level will be ignored.
         """
         self.level = level
 
     def debug(self, message):
         """
-        Log an info message
+        Log a debug message
         """
         if self.level <= 0:
             self._log(self.style_config.style_text(self.name, Debug, message))
 
     def info(self, message):
         """
         Log an info message
         """
         if self.level <= 1:
             self._log(self.style_config.style_text(self.name, Info, message))
 
     def warn(self, message):
         """
-        Log an info message
+        Log a warning message
         """
         if self.level <= 2:
             self._log(self.style_config.style_text(self.name, Warn, message))
 
     def error(self, message):
         """
-        Log an info message
+        Log an error message
         """
         if self.level <= 3:
             self._log(self.style_config.style_text(self.name, Error, message))
     
     def fatal(self, message):
         """
-        Log an info message
+        Log a fatal message
         """
         if self.level <= 4:
             self._log(self.style_config.style_text(self.name, Fatal, message))
 
+    def system(self, message):
+        """
+        Log a system message
+        """
+        self._log(self.style_config.style_text(self.name, System, message))
+
     def _log(self, message):
         if self.is_muted:
             return
         print(message)
 
     def set_style(self, style_config: StyleConfig):
         """
         Change the style config of the logger.
         """
         self.style_config = style_config
 
     def mute(self):
         """
-        Mute the logger
+        Mute the logger.
         """
         self.is_muted = True
 
     def unmute(self):
         """
-        Unmute the logger
+        Unmute the logger.
         """
         self.is_muted = False
```

### Comparing `styledlogger-0.0.4/styledlogger.egg-info/PKG-INFO` & `styledlogger-0.0.5/styledlogger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styledlogger
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple, styled logging library.
 Home-page: https://github.com/SpLayzDK/StyledLogger/
 Author: ImAlek (splayzdk)
 Author-email: alek@imalek.me
 License: BSL 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)
@@ -14,33 +14,35 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # StyledLogger
 
 ### A simple - yet beautiful logging library for Python 🐍 > 3.7
 
-To use, simply do `pip install styledlogger`
+To use, simply install via `pip install styledlogger`
 
-Then you can import `StyledLogger` from the package and initialize it.
+Then you can import the `StyledLogger class` from the `styledlogger` package, and initialize it.
 
 Simple example using a logger:
 
 ```py
 >>> from styledlogger import StyledLogger
 
 >>> logger = StyledLogger(name="Main") # Initialize a logger named "Main"
->>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug
+>>> logger.set_level(0) # Enable debug - default level is 1, which means every log type except debug. Setting the level to 0 enables the debug logs.
 
 >>> logger.debug("This is just a test print")
 9:55:30 :: DEBU @ Main - This is just a test print
 
 >>> logger.error("Could not fetch url 'https://example.com'")
 10:15:14 :: ERRO @ Main - Could not fetch url 'https://example.com'
 
 >>> from styledlogger import StyleConfig
+
 >>> logger.set_style(StyleConfig( text_format="(%time%) | %type% - %msg%", time_format='DD/MM/YYYY hh:mm' )) # Change the text format and time format in the logs. Placeholders you can use are: %name%, %time%, %type% and %msg%.
+
 >>> logger.warn("CPU usage exceeding 90%")
 (22/04/2023 10:01) | WARN - CPU usage exceeding 90%
 ```
 
 Check out the GitHub: https://github.com/SpLayzDK/StyledLogger
 Contact me at mail: alek@imalek.me
```

