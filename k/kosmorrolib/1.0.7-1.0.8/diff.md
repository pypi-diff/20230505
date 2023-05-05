# Comparing `tmp/kosmorrolib-1.0.7.tar.gz` & `tmp/kosmorrolib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kosmorrolib-1.0.7.tar", max compression
+gzip compressed data, was "kosmorrolib-1.0.8.tar", max compression
```

## Comparing `kosmorrolib-1.0.7.tar` & `kosmorrolib-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    32089 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/LICENSE.md
--rw-r--r--   0        0        0     1401 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/README.md
--rw-r--r--   0        0        0     1007 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/__init__.py
--rw-r--r--   0        0        0     1125 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/__version__.py
--rw-r--r--   0        0        0     1481 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/core.py
--rw-r--r--   0        0        0     2548 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/dateutil.py
--rw-r--r--   0        0        0     1977 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/enum.py
--rw-r--r--   0        0        0    18595 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/ephemerides.py
--rw-r--r--   0        0        0    19523 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/events.py
--rw-r--r--   0        0        0     1236 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/exceptions.py
--rw-r--r--   0        0        0    11579 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/kosmorrolib/model.py
--rw-r--r--   0        0        0     1008 2022-11-11 09:04:30.924674 kosmorrolib-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 kosmorrolib-1.0.7/setup.py
--rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 kosmorrolib-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    32089 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/LICENSE.md
+-rw-r--r--   0        0        0     1401 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/README.md
+-rw-r--r--   0        0        0     1007 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/__init__.py
+-rw-r--r--   0        0        0     1125 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/__version__.py
+-rw-r--r--   0        0        0     1481 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/core.py
+-rw-r--r--   0        0        0     2548 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/dateutil.py
+-rw-r--r--   0        0        0     1977 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/enum.py
+-rw-r--r--   0        0        0    18595 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/ephemerides.py
+-rw-r--r--   0        0        0    19468 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/events.py
+-rw-r--r--   0        0        0     1236 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/exceptions.py
+-rw-r--r--   0        0        0    11579 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/kosmorrolib/model.py
+-rw-r--r--   0        0        0     1014 2023-05-05 11:44:02.011213 kosmorrolib-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 kosmorrolib-1.0.8/PKG-INFO
```

### Comparing `kosmorrolib-1.0.7/LICENSE.md` & `kosmorrolib-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/README.md` & `kosmorrolib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/__init__.py` & `kosmorrolib-1.0.8/kosmorrolib/__init__.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/__version__.py` & `kosmorrolib-1.0.8/kosmorrolib/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 #
 #    You should have received a copy of the GNU Affero General Public License
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 __title__ = "kosmorrolib"
 __description__ = "A library to compute your ephemerides"
 __url__ = "http://kosmorro.space/lib"
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 __author__ = "Jérôme Deuchnord"
 __author_email__ = "jerome@deuchnord.fr"
 __license__ = "AGPL-v3"
 __copyright__ = "2021 - Jérôme Deuchnord"
```

### Comparing `kosmorrolib-1.0.7/kosmorrolib/core.py` & `kosmorrolib-1.0.8/kosmorrolib/core.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/dateutil.py` & `kosmorrolib-1.0.8/kosmorrolib/dateutil.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/enum.py` & `kosmorrolib-1.0.8/kosmorrolib/enum.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/ephemerides.py` & `kosmorrolib-1.0.8/kosmorrolib/ephemerides.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/events.py` & `kosmorrolib-1.0.8/kosmorrolib/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,24 +387,22 @@
 
 
 def _search_lunar_eclipse(start_time: Time, end_time: Time, timezone: int) -> [Event]:
     """Function to detect lunar eclipses.
 
     **Warning:** this is an internal function, not intended for use by end-developers.
 
-    Will return a total lunar eclipse for 2021-05-26:
-
     >>> _search_lunar_eclipse(get_timescale().utc(2021, 5, 26), get_timescale().utc(2021, 5, 27), 0)
-    [<Event type=LUNAR_ECLIPSE objects=[<Object type=SATELLITE name=MOON />] start=2021-05-26 08:47:54.795821+00:00 end=2021-05-26 13:49:34.353411+00:00 details={'type': <LunarEclipseType.TOTAL: 2>, 'maximum': datetime.datetime(2021, 5, 26, 11, 18, 42, 328842, tzinfo=datetime.timezone.utc)} />]
+    [<Event type=LUNAR_ECLIPSE objects=[<Object type=SATELLITE name=MOON />] start=2021-05-26 08:49:13.314888+00:00 end=2021-05-26 13:48:15.757096+00:00 details={'type': <LunarEclipseType.TOTAL: 2>, 'maximum': datetime.datetime(2021, 5, 26, 11, 18, 42, 328842, tzinfo=datetime.timezone.utc)} />]
 
     >>> _search_lunar_eclipse(get_timescale().utc(2019, 7, 16), get_timescale().utc(2019, 7, 17), 0)
-    [<Event type=LUNAR_ECLIPSE objects=[<Object type=SATELLITE name=MOON />] start=2019-07-16 18:39:53.391337+00:00 end=2019-07-17 00:21:51.378940+00:00 details={'type': <LunarEclipseType.PARTIAL: 1>, 'maximum': datetime.datetime(2019, 7, 16, 21, 30, 44, 170096, tzinfo=datetime.timezone.utc)} />]
+    [<Event type=LUNAR_ECLIPSE objects=[<Object type=SATELLITE name=MOON />] start=2019-07-16 18:41:24.400419+00:00 end=2019-07-17 00:20:20.079536+00:00 details={'type': <LunarEclipseType.PARTIAL: 1>, 'maximum': datetime.datetime(2019, 7, 16, 21, 30, 44, 170096, tzinfo=datetime.timezone.utc)} />]
 
     >>> _search_lunar_eclipse(get_timescale().utc(2017, 2, 11), get_timescale().utc(2017, 2, 12), 0)
-    [<Event type=LUNAR_ECLIPSE objects=[<Object type=SATELLITE name=MOON />] start=2017-02-10 22:02:59.016572+00:00 end=2017-02-11 03:25:07.627886+00:00 details={'type': <LunarEclipseType.PENUMBRAL: 0>, 'maximum': datetime.datetime(2017, 2, 11, 0, 43, 51, 793786, tzinfo=datetime.timezone.utc)} />]
+    [<Event type=LUNAR_ECLIPSE objects=[<Object type=SATELLITE name=MOON />] start=2017-02-10 22:04:24.192412+00:00 end=2017-02-11 03:23:42.046415+00:00 details={'type': <LunarEclipseType.PENUMBRAL: 0>, 'maximum': datetime.datetime(2017, 2, 11, 0, 43, 51, 793786, tzinfo=datetime.timezone.utc)} />]
     """
     moon = get_aster(ObjectIdentifier.MOON)
     events = []
     t, y, details = eclipselib.lunar_eclipses(start_time, end_time, get_skf_objects())
 
     for ti, yi in zip(t, y):
         penumbra_radius = Angle(radians=details["penumbra_radius_radians"][0])
```

### Comparing `kosmorrolib-1.0.7/kosmorrolib/exceptions.py` & `kosmorrolib-1.0.8/kosmorrolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/kosmorrolib/model.py` & `kosmorrolib-1.0.8/kosmorrolib/model.py`

 * *Files identical despite different names*

### Comparing `kosmorrolib-1.0.7/pyproject.toml` & `kosmorrolib-1.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kosmorrolib"
-version = "1.0.7"
+version = "1.0.8"
 authors = ["Jérôme Deuchnord <jerome@deuchnord.fr>"]
 homepage = "https://kosmorro.space/lib"
 repository = "https://github.com/Kosmorro/lib"
 documentation = "https://kosmorro.space/lib/doc"
 keywords = ["kosmorro", "astronomy", "ephemerides", "ephemeris"]
 license = "AGPL-3.0-or-later"
 description = "A library to computes the ephemerides."
@@ -17,19 +17,19 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 skyfield = "^1.21"
-skyfield-data = ">=3,<5"
+skyfield-data = ">=3,<6"
 python-dateutil = "^2.8"
 
-[tool.poetry.dev-dependencies]
-black = "^22.1"
-parameterized = "^0.8.1"
+[tool.poetry.group.dev.dependencies]
+black = "^23.1"
+parameterized = "^0.9.0"
 coverage = "^6.1.2"
 coveralls = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kosmorrolib-1.0.7/PKG-INFO` & `kosmorrolib-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kosmorrolib
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library to computes the ephemerides.
 Home-page: https://kosmorro.space/lib
 License: AGPL-3.0-or-later
 Keywords: kosmorro,astronomy,ephemerides,ephemeris
 Author: Jérôme Deuchnord
 Author-email: jerome@deuchnord.fr
 Requires-Python: >=3.8,<3.12
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: skyfield (>=1.21,<2.0)
-Requires-Dist: skyfield-data (>=3,<5)
+Requires-Dist: skyfield-data (>=3,<6)
 Project-URL: Documentation, https://kosmorro.space/lib/doc
 Project-URL: Repository, https://github.com/Kosmorro/lib
 Description-Content-Type: text/markdown
 
 # ![Kosmorrolib](https://raw.githubusercontent.com/Kosmorro/logos/main/kosmorrolib/kosmorrolib-artwork.jpg)
 
 [![Coverage Status](https://coveralls.io/repos/github/Kosmorro/lib/badge.svg?branch=main)](https://coveralls.io/github/Kosmorro/lib?branch=main) [![Version on PyPI](https://img.shields.io/pypi/v/kosmorrolib)](https://pypi.org/project/kosmorrolib)  [![IRC: #kosmorro on Libera.Chat](https://img.shields.io/badge/Libera.Chat-%23kosmorro-blueviolet)](https://web.libera.chat/?nick=Astronaut?#kosmorro)
```

