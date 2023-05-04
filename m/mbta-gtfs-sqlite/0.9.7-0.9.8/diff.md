# Comparing `tmp/mbta-gtfs-sqlite-0.9.7.tar.gz` & `tmp/mbta-gtfs-sqlite-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.9.7.tar", max compression
+gzip compressed data, was "mbta-gtfs-sqlite-0.9.8.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.9.7.tar` & `mbta-gtfs-sqlite-0.9.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/build.py
--rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0     4369 2023-05-04 15:02:00.233311 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6281 2023-05-03 21:20:38.555719 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     1970 2023-05-02 13:18:10.062598 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/utils/indexes.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      454 2023-05-04 15:02:39.694427 mbta-gtfs-sqlite-0.9.7/pyproject.toml
--rw-r--r--   0        0        0      742 2023-05-04 15:03:14.000921 mbta-gtfs-sqlite-0.9.7/setup.py
--rw-r--r--   0        0        0      494 2023-05-04 15:03:14.001154 mbta-gtfs-sqlite-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     4369 2023-05-04 15:02:00.233311 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6333 2023-05-04 22:19:23.539885 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-04-30 02:22:10.347470 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     2005 2023-05-04 22:18:43.022321 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-05-04 22:22:42.864670 mbta-gtfs-sqlite-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-05-04 22:23:04.506645 mbta-gtfs-sqlite-0.9.8/setup.py
+-rw-r--r--   0        0        0      494 2023-05-04 22:23:04.506902 mbta-gtfs-sqlite-0.9.8/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/archive.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/build.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/build.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/feed.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/feed.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/ingest.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
             stop_times_by_trip_id[trip_row["trip_id"]],
             key=lambda stop_time: int(stop_time["stop_sequence"]),
         )
         yield {
             **trip_row,
             "start_time": stop_times_for_trip[0]["arrival_time"],
             "end_time": stop_times_for_trip[-1]["arrival_time"],
+            "stop_count": len(stop_times_for_trip),
         }
 
 
 def ingest_feed_info(
     session: Session,
     download: GtfsFeedDownloadResult,
     reader: GtfsReader,
```

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/base.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/calendar.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/feed_info.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/lines.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/routes.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/stop_times.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/stops.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/transfers.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/transfers.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/models/trips.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/models/trips.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,11 +51,12 @@
     )
     trip_route_type: Mapped[TRouteType] = mapped_column(gtfs_enum_type(RouteType))
     route_pattern_id: Mapped[str] = mapped_column(String, nullable=True)
     bikes_allowed: Mapped[TBikesAllowed] = mapped_column(
         gtfs_enum_type(BikesAllowed),
         nullable=True,
     )
-    # start_time and end_time are not part of GTFS but they're useful information to have
+    # These are not part of GTFS but they're useful information to have
     # in smaller versions of the database without StopTimes
     start_time: Mapped[int] = mapped_column(Integer)
     end_time: Mapped[int] = mapped_column(Integer)
+    stop_count: Mapped[int] = mapped_column(Integer)
```

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/reader.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/utils/indexes.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/mbta_gtfs_sqlite/utils/time.py` & `mbta-gtfs-sqlite-0.9.8/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.7/setup.py` & `mbta-gtfs-sqlite-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['SQLAlchemy>=2.0.7,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'mbta-gtfs-sqlite',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': "Query the MBTA's static GTFS feeds using sqlite",
     'long_description': None,
     'author': 'Ian Reynolds',
     'author_email': 'ireynolds@transitmatters.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

