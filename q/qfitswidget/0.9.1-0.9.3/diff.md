# Comparing `tmp/qfitswidget-0.9.1.tar.gz` & `tmp/qfitswidget-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfitswidget-0.9.1.tar", max compression
+gzip compressed data, was "qfitswidget-0.9.3.tar", max compression
```

## Comparing `qfitswidget-0.9.1.tar` & `qfitswidget-0.9.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1074 2022-07-28 12:42:03.417246 qfitswidget-0.9.1/LICENSE
--rw-r--r--   0        0        0      548 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       37 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/__init__.py
--rw-r--r--   0        0        0     2262 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/navigationtoolbar.py
--rw-r--r--   0        0        0     1549 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/norm.py
--rw-r--r--   0        0        0    24139 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qfitswidget.py
--rw-r--r--   0        0        0        0 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/__init__.py
--rw-r--r--   0        0        0     6960 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/fitswidget.py
--rw-r--r--   0        0        0     8226 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/fitswidget.ui
--rw-r--r--   0        0        0      765 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/resources/image-solid.svg
--rw-r--r--   0        0        0     4689 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/resources.py
--rw-r--r--   0        0        0       95 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/resources.rc
--rw-r--r--   0        0        0     8268 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/settings.py
--rw-r--r--   0        0        0     5685 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/qt/settings.ui
--rw-r--r--   0        0        0     3934 2022-07-28 12:42:03.421247 qfitswidget-0.9.1/qfitswidget/settings.py
--rw-r--r--   0        0        0      769 2022-07-28 12:42:12.135778 qfitswidget-0.9.1/setup.py
--rw-r--r--   0        0        0      567 2022-07-28 12:42:12.136182 qfitswidget-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-05 09:54:54.159167 qfitswidget-0.9.3/LICENSE
+-rw-r--r--   0        0        0      559 2023-05-05 09:54:54.159167 qfitswidget-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-05-05 09:54:54.159167 qfitswidget-0.9.3/qfitswidget/__init__.py
+-rw-r--r--   0        0        0     2262 2023-05-05 09:54:54.159167 qfitswidget-0.9.3/qfitswidget/navigationtoolbar.py
+-rw-r--r--   0        0        0     1549 2023-05-05 09:54:54.159167 qfitswidget-0.9.3/qfitswidget/norm.py
+-rw-r--r--   0        0        0    24157 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qfitswidget.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/__init__.py
+-rw-r--r--   0        0        0     6960 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/fitswidget.py
+-rw-r--r--   0        0        0     8226 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/fitswidget.ui
+-rw-r--r--   0        0        0      765 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/resources/image-solid.svg
+-rw-r--r--   0        0        0     4689 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/resources.py
+-rw-r--r--   0        0        0       95 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/resources.rc
+-rw-r--r--   0        0        0     8268 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/settings.py
+-rw-r--r--   0        0        0     5685 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/qt/settings.ui
+-rw-r--r--   0        0        0     3934 2023-05-05 09:54:54.163167 qfitswidget-0.9.3/qfitswidget/settings.py
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 qfitswidget-0.9.3/PKG-INFO
```

### Comparing `qfitswidget-0.9.1/LICENSE` & `qfitswidget-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/navigationtoolbar.py` & `qfitswidget-0.9.3/qfitswidget/navigationtoolbar.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/norm.py` & `qfitswidget-0.9.3/qfitswidget/norm.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/qfitswidget.py` & `qfitswidget-0.9.3/qfitswidget/qfitswidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def run(self) -> None:
         # convert to RA/Dec and show it
         try:
             coord = pixel_to_skycoord(self.x, self.y, self.wcs)
             ra = coord.ra.to_string(u.hour, precision=1)
             dec = coord.dec.to_string(precision=1)
-        except ValueError:
+        except (ValueError, AttributeError):
             ra, dec = "", ""
 
         # value
         iy, ix = int(self.y), int(self.x)
         value = self.data[iy, ix, :] if len(self.data.shape) == 3 else np.array([self.data[iy, ix]])
 
         # mean / max
```

### Comparing `qfitswidget-0.9.1/qfitswidget/qt/fitswidget.py` & `qfitswidget-0.9.3/qfitswidget/qt/fitswidget.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/qt/fitswidget.ui` & `qfitswidget-0.9.3/qfitswidget/qt/fitswidget.ui`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/qt/resources/image-solid.svg` & `qfitswidget-0.9.3/qfitswidget/qt/resources/image-solid.svg`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/qt/resources.py` & `qfitswidget-0.9.3/qfitswidget/qt/resources.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/qt/settings.py` & `qfitswidget-0.9.3/qfitswidget/qt/settings.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/qt/settings.ui` & `qfitswidget-0.9.3/qfitswidget/qt/settings.ui`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/qfitswidget/settings.py` & `qfitswidget-0.9.3/qfitswidget/settings.py`

 * *Files identical despite different names*

### Comparing `qfitswidget-0.9.1/PKG-INFO` & `qfitswidget-0.9.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: qfitswidget
-Version: 0.9.1
+Version: 0.9.3
 Summary: PyQt widget for displaying FITS files
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyQt5 (>=5.15.7,<6.0.0)
-Requires-Dist: astropy (>=5.1,<6.0)
-Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyQt5 (>=5.15.9,<6.0.0)
+Requires-Dist: astropy (>=5.2.2,<6.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
```

