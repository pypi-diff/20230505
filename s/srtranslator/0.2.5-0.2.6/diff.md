# Comparing `tmp/srtranslator-0.2.5.tar.gz` & `tmp/srtranslator-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtranslator-0.2.5.tar", last modified: Fri May  5 15:01:18 2023, max compression
+gzip compressed data, was "srtranslator-0.2.6.tar", last modified: Fri May  5 15:16:18 2023, max compression
```

## Comparing `srtranslator-0.2.5.tar` & `srtranslator-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:01:18.573966 srtranslator-0.2.5/
--rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.5/LICENSE.md
--rw-rw-rw-   0        0        0     2891 2023-05-05 15:01:18.573966 srtranslator-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2486 2023-04-23 15:51:51.000000 srtranslator-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 15:01:18.573966 srtranslator-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-05-05 14:59:56.000000 srtranslator-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:01:18.567961 srtranslator-0.2.5/srtranslator/
--rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.5/srtranslator/__init__.py
--rw-rw-rw-   0        0        0     2382 2023-05-04 18:24:01.000000 srtranslator-0.2.5/srtranslator/__main__.py
--rw-rw-rw-   0        0        0     6026 2023-05-05 15:00:20.000000 srtranslator-0.2.5/srtranslator/srt_file.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:01:18.572965 srtranslator-0.2.5/srtranslator/translators/
--rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.5/srtranslator/translators/__init__.py
--rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.5/srtranslator/translators/base.py
--rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.5/srtranslator/translators/deepl_api.py
--rw-rw-rw-   0        0        0     4572 2023-04-03 17:46:29.000000 srtranslator-0.2.5/srtranslator/translators/deepl_scrap.py
--rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.5/srtranslator/translators/selenium_utils.py
--rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.5/srtranslator/translators/translatepy.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:01:18.569962 srtranslator-0.2.5/srtranslator.egg-info/
--rw-rw-rw-   0        0        0     2891 2023-05-05 15:01:18.000000 srtranslator-0.2.5/srtranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-05-05 15:01:18.000000 srtranslator-0.2.5/srtranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:01:18.000000 srtranslator-0.2.5/srtranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      657 2023-05-05 15:01:18.000000 srtranslator-0.2.5/srtranslator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 15:01:18.000000 srtranslator-0.2.5/srtranslator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 15:16:18.365011 srtranslator-0.2.6/
+-rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.6/LICENSE.md
+-rw-rw-rw-   0        0        0     2891 2023-05-05 15:16:18.365011 srtranslator-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2486 2023-04-23 15:51:51.000000 srtranslator-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:16:18.366011 srtranslator-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-05-05 15:15:58.000000 srtranslator-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:16:18.358004 srtranslator-0.2.6/srtranslator/
+-rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.6/srtranslator/__init__.py
+-rw-rw-rw-   0        0        0     2382 2023-05-04 18:24:01.000000 srtranslator-0.2.6/srtranslator/__main__.py
+-rw-rw-rw-   0        0        0     6026 2023-05-05 15:00:20.000000 srtranslator-0.2.6/srtranslator/srt_file.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:16:18.364010 srtranslator-0.2.6/srtranslator/translators/
+-rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.6/srtranslator/translators/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.6/srtranslator/translators/base.py
+-rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.6/srtranslator/translators/deepl_api.py
+-rw-rw-rw-   0        0        0     4698 2023-05-05 15:15:53.000000 srtranslator-0.2.6/srtranslator/translators/deepl_scrap.py
+-rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.6/srtranslator/translators/selenium_utils.py
+-rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.6/srtranslator/translators/translatepy.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:16:18.361007 srtranslator-0.2.6/srtranslator.egg-info/
+-rw-rw-rw-   0        0        0     2891 2023-05-05 15:16:18.000000 srtranslator-0.2.6/srtranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-05-05 15:16:18.000000 srtranslator-0.2.6/srtranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:16:18.000000 srtranslator-0.2.6/srtranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      657 2023-05-05 15:16:18.000000 srtranslator-0.2.6/srtranslator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 15:16:18.000000 srtranslator-0.2.6/srtranslator.egg-info/top_level.txt
```

### Comparing `srtranslator-0.2.5/PKG-INFO` & `srtranslator-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtranslator
-Version: 0.2.5
+Version: 0.2.6
 Summary: Traslate a .SRT file using any custom translator
 Home-page: https://github.com/sinedie/SRTranslator
 Author: EAR
 Author-email: sinedie@protonmail.com
 License: FREE
 Keywords: python,srt,languages,translator,subtitles
 Platform: UNKNOWN
```

### Comparing `srtranslator-0.2.5/README.md` & `srtranslator-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.5/setup.py` & `srtranslator-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name="srtranslator",
     description="Traslate a .SRT file using any custom translator",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/sinedie/SRTranslator",
-    version="0.2.5",
+    version="0.2.6",
     author="EAR",
     author_email="sinedie@protonmail.com",
     license="FREE",
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages(),
     keywords=["python", "srt", "languages", "translator", "subtitles"],
```

### Comparing `srtranslator-0.2.5/srtranslator/__main__.py` & `srtranslator-0.2.6/srtranslator/__main__.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.5/srtranslator/srt_file.py` & `srtranslator-0.2.6/srtranslator/srt_file.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.5/srtranslator/translators/deepl_scrap.py` & `srtranslator-0.2.6/srtranslator/translators/deepl_scrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,17 @@
         self.target_lang = language
 
     def _set_language(self, language: str, dropdown_class: str) -> None:
         # Click the languages dropdown button
         Button(self.driver, "CLASS_NAME", dropdown_class).click()
 
         # Get the language button to click based on is dl-test property or the text in the button
-        xpath_by_property = f"//button[@data-testid='translator-lang-option-{language}']"
+        xpath_by_property = (
+            f"//button[@data-testid='translator-lang-option-{language}']"
+        )
         x_path_by_text = f"//button[text()='{self.languages[language]}']"
         xpath = f"{xpath_by_property} | {x_path_by_text}"
 
         # Click the wanted language button
         Button(self.driver, "XPATH", xpath).click()
 
     def _is_translated(self, original: str, translation: str) -> bool:
@@ -122,14 +124,16 @@
         self.input_lang_from.write((clean_text))
 
         # Maximun number of iterations 60 seconds
         for _ in range(60):
             translation = self.input_destination_language.value
 
             if self._is_translated(clean_text, translation):
+                time.sleep(1)
+                translation = self.input_destination_language.value
                 return translation.replace("@[.]@", "[...]")
             time.sleep(1)
 
         self.quit()
         raise TimeOutException("Translation timed out")
 
     def quit(self):
```

### Comparing `srtranslator-0.2.5/srtranslator/translators/selenium_utils.py` & `srtranslator-0.2.6/srtranslator/translators/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.5/srtranslator/translators/translatepy.py` & `srtranslator-0.2.6/srtranslator/translators/translatepy.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.5/srtranslator.egg-info/PKG-INFO` & `srtranslator-0.2.6/srtranslator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtranslator
-Version: 0.2.5
+Version: 0.2.6
 Summary: Traslate a .SRT file using any custom translator
 Home-page: https://github.com/sinedie/SRTranslator
 Author: EAR
 Author-email: sinedie@protonmail.com
 License: FREE
 Keywords: python,srt,languages,translator,subtitles
 Platform: UNKNOWN
```

### Comparing `srtranslator-0.2.5/srtranslator.egg-info/SOURCES.txt` & `srtranslator-0.2.6/srtranslator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.5/srtranslator.egg-info/requires.txt` & `srtranslator-0.2.6/srtranslator.egg-info/requires.txt`

 * *Files identical despite different names*

