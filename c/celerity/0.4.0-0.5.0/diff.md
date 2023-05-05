# Comparing `tmp/celerity-0.4.0.tar.gz` & `tmp/celerity-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celerity-0.4.0.tar", max compression
+gzip compressed data, was "celerity-0.5.0.tar", max compression
```

## Comparing `celerity-0.4.0.tar` & `celerity-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-05-04 16:36:03.625378 celerity-0.4.0/LICENSE
--rw-r--r--   0        0        0     4346 2023-05-04 16:36:03.625378 celerity-0.4.0/README.md
--rw-r--r--   0        0        0     1830 2023-05-04 16:36:03.625378 celerity-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/__init__.py
--rw-r--r--   0        0        0     1752 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/astrometry.py
--rw-r--r--   0        0        0      240 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/common.py
--rw-r--r--   0        0        0      997 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/constants.py
--rw-r--r--   0        0        0     1650 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/coordinates.py
--rw-r--r--   0        0        0     2092 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/seeing.py
--rw-r--r--   0        0        0     3771 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/temporal.py
--rw-r--r--   0        0        0      961 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/utilities.py
--rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 celerity-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-05 16:10:40.668348 celerity-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4346 2023-05-05 16:10:40.668348 celerity-0.5.0/README.md
+-rw-r--r--   0        0        0     1830 2023-05-05 16:10:40.668348 celerity-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/__init__.py
+-rw-r--r--   0        0        0     2501 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/astrometry.py
+-rw-r--r--   0        0        0      240 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/common.py
+-rw-r--r--   0        0        0      997 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/constants.py
+-rw-r--r--   0        0        0     1650 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/coordinates.py
+-rw-r--r--   0        0        0      468 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/epoch.py
+-rw-r--r--   0        0        0     2092 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/seeing.py
+-rw-r--r--   0        0        0     4129 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/temporal.py
+-rw-r--r--   0        0        0      961 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/utilities.py
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 celerity-0.5.0/PKG-INFO
```

### Comparing `celerity-0.4.0/LICENSE` & `celerity-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celerity-0.4.0/README.md` & `celerity-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `celerity-0.4.0/pyproject.toml` & `celerity-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celerity"
-version = "0.4.0"
+version = "0.5.0"
 description = "Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations."
 authors = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
 maintainers = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
```

### Comparing `celerity-0.4.0/src/celerity/astrometry.py` & `celerity-0.5.0/src/celerity/astrometry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 from datetime import datetime
 
 from .common import EquatorialCoordinate, GeographicCoordinate
-from .temporal import get_local_sidereal_time
+from .temporal import get_julian_date, get_local_sidereal_time
 
 
 def get_hour_angle(date: datetime, ra: float, longitude: float) -> float:
     """
     Gets the hour angle for a particular object for a particular observer at a given datetime
 
     :param date: The datetime object to convert.
@@ -21,14 +21,37 @@
     # If the hour angle is less than zero, ensure we rotate by 2π radians (360 degrees)
     if ha < 0:
         ha += 360
 
     return ha
 
 
+def get_obliquity_of_the_ecliptic(date: datetime) -> float:
+    """
+    Gets the obliquity of the ecliptic for a particular datetime
+
+    The obliquity of the ecliptic is the angle between the ecliptic and the celestial equator, and is used to
+    convert between ecliptic and equatorial coordinates.
+
+    :param date: The datetime object to convert.
+    :return The obliquity of the ecliptic in degrees.
+    """
+    # Get the Julian date:
+    JD = get_julian_date(date)
+
+    # Calculate the number of centuries since J2000.0:
+    T = (JD - 2451545.0) / 36525
+
+    # Calculate the obliquity of the ecliptic:
+    return (
+        23.439292
+        - (46.845 * T + 0.00059 * math.pow(T, 2) + 0.001813 * math.pow(T, 3)) / 3600
+    )
+
+
 def get_parallactic_angle(
     date: datetime,
     observer: GeographicCoordinate,
     target: EquatorialCoordinate,
 ) -> float:
     """
     Gets the parallactic angle for a particular object for a particular observer at a given datetime
```

### Comparing `celerity-0.4.0/src/celerity/constants.py` & `celerity-0.5.0/src/celerity/constants.py`

 * *Files identical despite different names*

### Comparing `celerity-0.4.0/src/celerity/coordinates.py` & `celerity-0.5.0/src/celerity/coordinates.py`

 * *Files identical despite different names*

### Comparing `celerity-0.4.0/src/celerity/seeing.py` & `celerity-0.5.0/src/celerity/seeing.py`

 * *Files identical despite different names*

### Comparing `celerity-0.4.0/src/celerity/temporal.py` & `celerity-0.5.0/src/celerity/temporal.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,25 @@
             ).total_seconds()
             * 1000
         )
         / 86400000.0
     ) + 2440587.5
 
 
+def get_modified_julian_date(date: datetime) -> float:
+    """
+    The Modified Julian Date (MJD) is the number of fractional days since midnight
+    on November 17, 1858.
+
+    :param date: The datetime object to convert.
+    :return: The Modified Julian Date (MJD) of the given date normalised to UTC.
+    """
+    return get_julian_date(date) - 2400000.5
+
+
 def get_greenwhich_sidereal_time(date: datetime) -> float:
     """
     The Greenwich Sidereal Time (GST) is the hour angle of the vernal
     equinox, the ascending node of the ecliptic on the celestial equator.
 
     :param date: The datetime object to convert.
     :return: The Greenwich Sidereal Time (GST) of the given date normalised to UTC.
```

### Comparing `celerity-0.4.0/src/celerity/utilities.py` & `celerity-0.5.0/src/celerity/utilities.py`

 * *Files identical despite different names*

### Comparing `celerity-0.4.0/PKG-INFO` & `celerity-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celerity
-Version: 0.4.0
+Version: 0.5.0
 Summary: Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations.
 Home-page: https://github.com/michaelroberts/celerity
 Keywords: astronomy,astrometry,ephemeris
 Author: Michael J. Roberts
 Author-email: michael@observerly.com
 Maintainer: Michael J. Roberts
 Maintainer-email: michael@observerly.com
```

