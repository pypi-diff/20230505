# Comparing `tmp/html2info-0.1.8.tar.gz` & `tmp/html2info-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2info-0.1.8.tar", last modified: Thu May  4 19:16:16 2023, max compression
+gzip compressed data, was "html2info-0.1.9.tar", last modified: Fri May  5 19:17:15 2023, max compression
```

## Comparing `html2info-0.1.8.tar` & `html2info-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-04 19:16:16.553869 html2info-0.1.8/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-04 19:16:16.553869 html2info-0.1.8/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.8/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-04 19:16:16.553869 html2info-0.1.8/html2info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.8/html2info/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5191 2023-05-04 19:14:11.000000 html2info-0.1.8/html2info/linkedin.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.8/html2info/types.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.8/html2info/utils.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-04 19:16:16.553869 html2info-0.1.8/html2info.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-05-04 19:16:16.000000 html2info-0.1.8/html2info.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.8/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-04 19:16:16.553869 html2info-0.1.8/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-05-04 19:15:27.000000 html2info-0.1.8/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-05 19:17:15.536865 html2info-0.1.9/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-05 19:17:15.536865 html2info-0.1.9/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5278 2023-04-20 20:54:37.000000 html2info-0.1.9/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-05 19:17:15.536865 html2info-0.1.9/html2info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-04-19 18:56:39.000000 html2info-0.1.9/html2info/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6157 2023-05-05 19:14:12.000000 html2info-0.1.9/html2info/linkedin.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      439 2023-04-23 00:43:09.000000 html2info-0.1.9/html2info/types.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      190 2023-04-19 19:16:29.000000 html2info-0.1.9/html2info/utils.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-05-05 19:17:15.536865 html2info-0.1.9/html2info.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6013 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      279 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       23 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       10 2023-05-05 19:17:15.000000 html2info-0.1.9/html2info.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1475 2023-04-23 00:41:00.000000 html2info-0.1.9/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-05-05 19:17:15.536865 html2info-0.1.9/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1360 2023-05-05 19:16:44.000000 html2info-0.1.9/setup.py
```

### Comparing `html2info-0.1.8/PKG-INFO` & `html2info-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.8/README.md` & `html2info-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `html2info-0.1.8/html2info/linkedin.py` & `html2info-0.1.9/html2info/linkedin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import re
 from typing import Optional
 
 from bs4 import BeautifulSoup
 
 from html2info.types import EducationType, ExperienceType
 
 
 class Person:
-    def __init__(self, linkein_url: str, raw_html: str) -> None:
+    def __init__(self, linkedin_url: str, raw_html: str) -> None:
         self.soup = BeautifulSoup(raw_html, "html.parser")
-        self.linkedin_url = linkein_url
+        self.linkedin_url = linkedin_url.strip().rstrip("/")
 
         self.name = None
         self.title = None
         self.location = None
         self.profile_photo_link = None
         self.about = None
         self.experience: list[ExperienceType] = []
@@ -30,14 +31,36 @@
         )
 
         self.profile_photo_link = profile_photo["src"] if profile_photo else None
 
         self.parse_about()
         self.parse_experience()
         self.parse_education()
+        self.parse_profile_link()
+
+    def parse_profile_link(self) -> None:
+        links = self.soup.find_all("a", href=True)
+        # Regular expression pattern to match the desired links
+
+        pattern = r"https:\/\/www\.linkedin\.com\/in\/[^/]+\/recent-activity\/(?:[^/]*)"
+
+        extracted_links = []
+
+        for link in links:
+            href = link["href"]
+            if match := re.match(pattern, href):
+                temp_extracted_links = match[0].split("/")[:5]
+                extracted_link = "/".join(temp_extracted_links)
+                # Remove the trailing slash if it exists
+                extracted_link = extracted_link.rstrip("/")
+                if extracted_link not in extracted_links:
+                    extracted_links.append(extracted_link)
+
+        if len(set(extracted_links)) != 1 or self.linkedin_url not in extracted_links:
+            raise ValueError("Could not find the profile link")
 
     def find_section_by_id(self, section_name: str) -> Optional[BeautifulSoup]:
         div = self.soup.find("div", {"id": section_name})
         return None if div is None else div.find_parent("section")
 
     def parse_about(self):
         # Find the span containing the text
```

### Comparing `html2info-0.1.8/html2info.egg-info/PKG-INFO` & `html2info-0.1.9/html2info.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2info
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to parse raw HTML and return structured information.
 Author: Vladimir Iglovikov
 Author-email: iglovikov@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2info-0.1.8/pyproject.toml` & `html2info-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html2info-0.1.8/setup.py` & `html2info-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="html2info",  # Replace with your package name
-    version="0.1.8",  # Replace with your package version
+    version="0.1.9",  # Replace with your package version
     author="Vladimir Iglovikov",  # Replace with your name
     author_email="iglovikov@gmail.com",  # Replace with your email
     description="A package to parse raw HTML and return structured information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=[
```

