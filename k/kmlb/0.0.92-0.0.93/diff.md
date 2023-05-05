# Comparing `tmp/kmlb-0.0.92.tar.gz` & `tmp/kmlb-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmlb-0.0.92.tar", last modified: Thu May  4 21:22:46 2023, max compression
+gzip compressed data, was "kmlb-0.0.93.tar", last modified: Fri May  5 03:52:41 2023, max compression
```

## Comparing `kmlb-0.0.92.tar` & `kmlb-0.0.93.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 21:22:46.059504 kmlb-0.0.92/
--rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.92/LICENSE.md
--rw-rw-rw-   0        0        0    38527 2023-05-04 21:22:46.058053 kmlb-0.0.92/PKG-INFO
--rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.92/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 21:22:46.034390 kmlb-0.0.92/kmlb/
--rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.92/kmlb/__init__.py
--rw-rw-rw-   0        0        0    43022 2023-05-04 21:17:54.000000 kmlb-0.0.92/kmlb/base.py
--rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.92/kmlb/gis_basics.py
--rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.92/kmlb/shapes.py
-drwxrwxrwx   0        0        0        0 2023-05-04 21:22:46.058053 kmlb-0.0.92/kmlb.egg-info/
--rw-rw-rw-   0        0        0    38527 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-04 21:22:45.000000 kmlb-0.0.92/kmlb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 21:22:46.059504 kmlb-0.0.92/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-05-04 21:15:06.000000 kmlb-0.0.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:52:41.290742 kmlb-0.0.93/
+-rw-rw-rw-   0        0        0    35817 2023-04-07 16:36:25.000000 kmlb-0.0.93/LICENSE.md
+-rw-rw-rw-   0        0        0    38527 2023-05-05 03:52:41.290742 kmlb-0.0.93/PKG-INFO
+-rw-rw-rw-   0        0        0    38044 2023-04-25 14:31:02.000000 kmlb-0.0.93/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 03:52:41.270417 kmlb-0.0.93/kmlb/
+-rw-rw-rw-   0        0        0       65 2023-04-07 16:36:25.000000 kmlb-0.0.93/kmlb/__init__.py
+-rw-rw-rw-   0        0        0    43400 2023-05-05 03:51:08.000000 kmlb-0.0.93/kmlb/base.py
+-rw-rw-rw-   0        0        0    10618 2023-04-07 16:36:25.000000 kmlb-0.0.93/kmlb/gis_basics.py
+-rw-rw-rw-   0        0        0     6922 2023-04-26 16:09:29.000000 kmlb-0.0.93/kmlb/shapes.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:52:41.289736 kmlb-0.0.93/kmlb.egg-info/
+-rw-rw-rw-   0        0        0    38527 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-05 03:52:41.000000 kmlb-0.0.93/kmlb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 03:52:41.290742 kmlb-0.0.93/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-05 03:51:36.000000 kmlb-0.0.93/setup.py
```

### Comparing `kmlb-0.0.92/LICENSE.md` & `kmlb-0.0.93/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.92/PKG-INFO` & `kmlb-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.92
+Version: 0.0.93
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.92/README.md` & `kmlb-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.92/kmlb/base.py` & `kmlb-0.0.93/kmlb/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1037,15 +1037,15 @@
             f.write(kml_string)
     else:
         pass
 
     return kml_string
 
 
-def network_link(name, link_path, description='', refresh_interval=None, folder_type=1, collapsed=True, camera=None):
+def network_link(name, link_path, description='', refresh_interval=None, folder_type=1, hidden=False, collapsed=True, camera=None):
     """
        Creates a NetworkLink element.
 
        OVERVIEW:
            Creates an XML element that defines a network link. This string element can be added to kml and folders.
 
        INPUTS:
@@ -1056,14 +1056,16 @@
            description (String) [Optional]:
                 A small body of descriptive text for the NetworkLink element.
            refresh_interval (Int) [Optional]:
                 Number of seconds between file refreshes. (Default = None)
             folder_type (Integer):
                 Can be any of the following values:
                 1 = check, 2 = radioFolder, 3 = checkOffOnly, 4 = checkHideChildren
+            hidden (Bool) [Optional]:
+                A value of 'True' or 'False' where 'False' means the network link will be visible (Default = 'False').
            collapsed (Bool) [Optional]:
                 True = Root folder is collapsed.
                 False = Root folder is open/expanded.
             camera (Element) [Optional]:
                 A KML 'LookAt' element that defines the default camera angle to the kml.
 
        OUTPUT:
@@ -1074,28 +1076,36 @@
        ----------
        name : str
        link_path : str
        description : str, optional
        refresh_interval : int, optional
        folder_type : int, optional
        collapsed : bool, optional
+       hidden : bool, optional
        camera : element, optional
 
        Returns
        -------
        network_link : element
 
        """
 
     network_link = ET.Element("NetworkLink")
     ET.SubElement(network_link, "name").text = str(name)
     ET.SubElement(network_link, "description").text = str(description)
     collapsed = 0 if collapsed is True else 1
     ET.SubElement(network_link, "open").text = str(collapsed)
 
+    # Set 'visibility' value
+    visibility = 0
+    if hidden is False:
+        visibility = 1
+
+    ET.SubElement(network_link, 'visibility').text = str(visibility)
+
     style = ET.SubElement(network_link, "Style")
     list_style = ET.SubElement(style, "ListStyle")
     if folder_type == 1:
         folder_type = 'check'
     elif folder_type == 2:
         folder_type = 'radioFolder'
     elif folder_type == 3:
```

### Comparing `kmlb-0.0.92/kmlb/gis_basics.py` & `kmlb-0.0.93/kmlb/gis_basics.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.92/kmlb/shapes.py` & `kmlb-0.0.93/kmlb/shapes.py`

 * *Files identical despite different names*

### Comparing `kmlb-0.0.92/kmlb.egg-info/PKG-INFO` & `kmlb-0.0.93/kmlb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmlb
-Version: 0.0.92
+Version: 0.0.93
 Summary: A Straightforward Google Earth KML Builder
 Home-page: https://github.com/HFM3/kmlb
 Author: HFM3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kmlb-0.0.92/setup.py` & `kmlb-0.0.93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kmlb",
-    version="0.0.92",
+    version="0.0.93",
     author="HFM3",
     description="A Straightforward Google Earth KML Builder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HFM3/kmlb",
     packages=setuptools.find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "images", "art"]),
     classifiers=[
```

