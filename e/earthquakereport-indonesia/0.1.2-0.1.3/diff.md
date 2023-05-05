# Comparing `tmp/earthquakereport-indonesia-0.1.2.tar.gz` & `tmp/earthquakereport-indonesia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthquakereport-indonesia-0.1.2.tar", last modified: Thu May  4 09:26:12 2023, max compression
+gzip compressed data, was "earthquakereport-indonesia-0.1.3.tar", last modified: Fri May  5 09:12:15 2023, max compression
```

## Comparing `earthquakereport-indonesia-0.1.2.tar` & `earthquakereport-indonesia-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:26:12.165985 earthquakereport-indonesia-0.1.2/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.2/LICENSE
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-04 09:26:12.165684 earthquakereport-indonesia-0.1.2/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      596 2023-05-04 09:24:44.000000 earthquakereport-indonesia-0.1.2/README.md
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:26:12.164465 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/SOURCES.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/dependency_links.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-04 09:26:12.000000 earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/top_level.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-04 09:26:12.166107 earthquakereport-indonesia-0.1.2/setup.cfg
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-04 09:25:39.000000 earthquakereport-indonesia-0.1.2/setup.py
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-04 09:26:12.164967 earthquakereport-indonesia-0.1.2/updateGempa/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2392 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.2/updateGempa/__init__.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-05 09:12:15.842114 earthquakereport-indonesia-0.1.3/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.3/LICENSE
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-05 09:12:15.841737 earthquakereport-indonesia-0.1.3/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      596 2023-05-04 09:24:44.000000 earthquakereport-indonesia-0.1.3/README.md
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-05 09:12:15.839984 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/top_level.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-05 09:12:15.842225 earthquakereport-indonesia-0.1.3/setup.cfg
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-05 07:53:04.000000 earthquakereport-indonesia-0.1.3/setup.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-05 09:12:15.840650 earthquakereport-indonesia-0.1.3/updateGempa/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2540 2023-05-05 07:41:53.000000 earthquakereport-indonesia-0.1.3/updateGempa/__init__.py
```

### Comparing `earthquakereport-indonesia-0.1.2/LICENSE` & `earthquakereport-indonesia-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `earthquakereport-indonesia-0.1.2/PKG-INFO` & `earthquakereport-indonesia-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakereport-indonesia
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 Home-page: https://github.com/ganirh0612/indonesiaEarthquakeReport
 Author: Hasan Gani
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `earthquakereport-indonesia-0.1.2/README.md` & `earthquakereport-indonesia-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `earthquakereport-indonesia-0.1.2/earthquakereport_indonesia.egg-info/PKG-INFO` & `earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakereport-indonesia
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 Home-page: https://github.com/ganirh0612/indonesiaEarthquakeReport
 Author: Hasan Gani
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `earthquakereport-indonesia-0.1.2/setup.py` & `earthquakereport-indonesia-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="earthquakereport-indonesia",
-    version="0.1.2",
+    version="0.1.3",
     author="Hasan Gani",
     author_email="ganirh0612@gmail.com",
     description="This package will provide the most update of Indonesian bureau of Forecast (BMKG)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ganirh0612/indonesiaEarthquakeReport",
     project_urls={
```

### Comparing `earthquakereport-indonesia-0.1.2/updateGempa/__init__.py` & `earthquakereport-indonesia-0.1.3/updateGempa/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import bs4
 import requests
 
+description = 'To get the latest earthquake in Indonesia from Bureau website https: www.bmkg.go.id'
+
 def ekstraksi_data():
     """
     Tanggal     : 01 Mei 2023
     Waktu       : 10:20:12 WIB
     Magnitude   : 3.8
     Kedalaman   : 10 km
     Lokasi      : LS = 4.01 BT = 136.07
@@ -77,9 +79,10 @@
     print(f"Magnitude {result['magnitude']}")
     print(f"Kedalaman {result['kedalaman']}")
     print(f"Koordinat: LS =  {result['koordinat']['ls']}, BT =  {result['koordinat']['bt']}")
     print(f"Lokasi {result['lokasi']}")
     print(f"{result['dirasakan']}")
 
 if __name__ == '__main__':
+    print('Deskription Package:', description)
     result = ekstraksi_data()
     tampilkan_data(result)
```

