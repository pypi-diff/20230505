# Comparing `tmp/pix_framework-0.7.0.tar.gz` & `tmp/pix_framework-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.7.0.tar", max compression
+gzip compressed data, was "pix_framework-0.7.1.tar", max compression
```

## Comparing `pix_framework-0.7.0.tar` & `pix_framework-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-05-05 15:07:18.334761 pix_framework-0.7.0/LICENSE
--rw-r--r--   0        0        0      549 2023-05-05 15:07:18.334761 pix_framework-0.7.0/README.md
--rw-r--r--   0        0        0      638 2023-05-05 15:07:18.334761 pix_framework-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0    10717 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0       27 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/input.py
--rw-r--r--   0        0        0     2639 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13043 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      969 2023-05-05 15:07:18.334761 pix_framework-0.7.0/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 pix_framework-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-05 16:18:53.563943 pix_framework-0.7.1/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-05 16:18:53.563943 pix_framework-0.7.1/README.md
+-rw-r--r--   0        0        0      744 2023-05-05 16:18:53.563943 pix_framework-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0    11236 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5444 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2498 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/input.py
+-rw-r--r--   0        0        0     2058 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4414 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    13047 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-05-05 16:18:53.563943 pix_framework-0.7.1/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 pix_framework-0.7.1/PKG-INFO
```

### Comparing `pix_framework-0.7.0/LICENSE` & `pix_framework-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.0/README.md` & `pix_framework-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.0/pyproject.toml` & `pix_framework-0.7.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.7.0"
+version = "0.7.1"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>", "Ihar Suvorau <ihar.suvorau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "pix_framework", from = "src" },
 ]
 
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
-pandas = "^2.0.0"
+pandas = "^2.0.1"
 scipy = "^1.10.1"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+markers = [
+    "unit",
+    "integration",
+    "smoke",
+]
```

### Comparing `pix_framework-0.7.0/src/pix_framework/calendar/resource_calendar.py` & `pix_framework-0.7.1/src/pix_framework/calendar/resource_calendar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-# -------------------- Calendar class and utils ------------------- #
-# The main structures have been copied and simplified from Prosimos #
-# project (https://github.com/AutomatedProcessImprovement/Prosimos/blob/main/bpdfr_simulation_engine/resource_calendar.py).
-# ----------------------------------------------------------------- #
+"""
+The main structures have been copied and simplified from Prosimos project
+(https://github.com/AutomatedProcessImprovement/Prosimos/blob/main/bpdfr_simulation_engine/resource_calendar.py).
+"""
 from dataclasses import dataclass
 from typing import List
 
 import pandas as pd
 import pytz
 
-str_week_days = {"MONDAY": 0, "TUESDAY": 1, "WEDNESDAY": 2, "THURSDAY": 3, "FRIDAY": 4, "SATURDAY": 5, "SUNDAY": 6}
-int_week_days = {0: "MONDAY", 1: "TUESDAY", 2: "WEDNESDAY", 3: "THURSDAY", 4: "FRIDAY", 5: "SATURDAY", 6: "SUNDAY"}
+str_week_days = {
+    "MONDAY": 0,
+    "TUESDAY": 1,
+    "WEDNESDAY": 2,
+    "THURSDAY": 3,
+    "FRIDAY": 4,
+    "SATURDAY": 5,
+    "SUNDAY": 6,
+}
+int_week_days = {
+    0: "MONDAY",
+    1: "TUESDAY",
+    2: "WEDNESDAY",
+    3: "THURSDAY",
+    4: "FRIDAY",
+    5: "SATURDAY",
+    6: "SUNDAY",
+}
 
 conversion_table = {
-    'WEEKS': 604800,
-    'DAYS': 86400,
-    'HOURS': 3600,
-    'MINUTES': 60,
-    'SECONDS': 1
+    "WEEKS": 604800,
+    "DAYS": 86400,
+    "HOURS": 3600,
+    "MINUTES": 60,
+    "SECONDS": 1,
 }
 
 
 @dataclass
 class Interval:
     def __init__(self, start: pd.Timestamp, end: pd.Timestamp):
         self.start = start
@@ -31,15 +47,15 @@
 
     def __eq__(self, other):
         if isinstance(other, Interval):
             return self.start == other.start and self.end == other.end
         else:
             return False
 
-    def merge_interval(self, n_interval: 'Interval'):
+    def merge_interval(self, n_interval: "Interval"):
         self.start = min(n_interval.start, self.start)
         self.end = max(n_interval.end, self.end)
         self.duration = (self.end - self.start).total_seconds()
 
 
 class RCalendar:
     def __init__(self, calendar_id: str):
@@ -50,20 +66,22 @@
     def to_json(self) -> list:
         # Create empty list
         items = []
         # Insert calendar for each week day
         for i in range(0, 7):
             if len(self.work_intervals[i]) > 0:
                 for interval in self.work_intervals[i]:
-                    items.append({
-                        'from': int_week_days[i],
-                        'to': int_week_days[i],
-                        "beginTime": str(interval.start.time()),
-                        "endTime": str(interval.end.time())
-                    })
+                    items.append(
+                        {
+                            "from": int_week_days[i],
+                            "to": int_week_days[i],
+                            "beginTime": str(interval.start.time()),
+                            "endTime": str(interval.end.time()),
+                        }
+                    )
         # Return list with working schedule
         return items
 
     def _add_interval(self, w_day: str, interval: Interval):
         i = 0
         for to_merge in self.work_intervals[w_day]:
             if to_merge.end < interval.start:
@@ -79,33 +97,41 @@
                         break
                     if next_i.start <= to_merge.end < next_i.end:
                         to_merge.merge_interval(next_i)
                     del self.work_intervals[w_day][i]
                 return
         self.work_intervals[w_day].insert(i, interval)
 
-    def add_calendar_item(self, from_day: str, to_day: str, begin_time: str, end_time: str):
+    def add_calendar_item(
+        self, from_day: str, to_day: str, begin_time: str, end_time: str
+    ):
         if from_day.upper() in str_week_days and to_day.upper() in str_week_days:
             try:
                 t_interval = Interval(
-                    start=pd.Timestamp.combine(self.default_date, pd.Timestamp(begin_time).time()),
-                    end=pd.Timestamp.combine(self.default_date, pd.Timestamp(end_time).time())
+                    start=pd.Timestamp.combine(
+                        self.default_date, pd.Timestamp(begin_time).time()
+                    ),
+                    end=pd.Timestamp.combine(
+                        self.default_date, pd.Timestamp(end_time).time()
+                    ),
                 )
                 d_s = str_week_days[from_day.upper()]
                 d_e = str_week_days[to_day.upper()]
                 while True:
                     self._add_interval(d_s % 7, t_interval)
                     if d_s % 7 == d_e:
                         break
                     d_s += 1
             except ValueError:
                 return
 
 
-def get_last_available_timestamp(start: pd.Timestamp, end: pd.Timestamp, schedule: RCalendar) -> pd.Timestamp:
+def get_last_available_timestamp(
+    start: pd.Timestamp, end: pd.Timestamp, schedule: RCalendar
+) -> pd.Timestamp:
     """
     Get the timestamp [last_available] within the interval from [start] to [end] (i.e. [start] <= [last_available] <= [end]) such that
     the interval from [last_available] to [end] is the largest and all of it is in the working hours in the calendar [schedule].
 
     For example, for [start] = 09:30, [end] = 14:00, and a [schedule] of every week day from 06:00 to 09:00, and from 10:00 to 16:00. The
     [last_available] would be 10:00.
 
@@ -120,69 +146,77 @@
     last_available = end
     found = False
     while not found:
         day_intervals = schedule.work_intervals[last_available.weekday()]
         for interval in reversed(day_intervals):
             # Move interval to current day
             interval_start = interval.start.replace(
-                day=last_available.day, month=last_available.month, year=last_available.year, tzinfo=pytz.timezone('UTC')
+                day=last_available.day,
+                month=last_available.month,
+                year=last_available.year,
+                tzinfo=pytz.timezone("UTC"),
             )
             interval_end = interval.end.replace(
-                day=last_available.day, month=last_available.month, year=last_available.year, tzinfo=pytz.timezone('UTC')
+                day=last_available.day,
+                month=last_available.month,
+                year=last_available.year,
+                tzinfo=pytz.timezone("UTC"),
             )
             if interval_end < last_available:
                 # The last available is later than the end of the current working interval
                 if (last_available - interval_end) > pd.Timedelta(seconds=2):
                     # Non-working time gap previous to last_available, search finished
                     found = True
                     # Correct jump to previous day if needed
                     if (
-                            last_available.hour == 23 and
-                            last_available.minute == 59 and
-                            last_available.second == 59 and
-                            last_available.microsecond == 999999
+                        last_available.hour == 23
+                        and last_available.minute == 59
+                        and last_available.second == 59
+                        and last_available.microsecond == 999999
                     ):
                         last_available = last_available + pd.Timedelta(microseconds=1)
                 else:
                     # No non-working time gap, move to the start of this working interval and continue
                     last_available = last_available.replace(
                         hour=interval_start.hour,
                         minute=interval_start.minute,
                         second=interval_start.second,
-                        microsecond=interval_start.microsecond
+                        microsecond=interval_start.microsecond,
                     )
             elif interval_start <= last_available <= interval_end:
                 # The last available timestamp is within the current interval
                 last_available = last_available.replace(
                     hour=interval_start.hour,
                     minute=interval_start.minute,
                     second=interval_start.second,
-                    microsecond=interval_start.microsecond
+                    microsecond=interval_start.microsecond,
                 )
         if not found:
-            start_of_day = last_available.replace(hour=00, minute=00, second=00, microsecond=0)
+            start_of_day = last_available.replace(
+                hour=00, minute=00, second=00, microsecond=0
+            )
             if (last_available - start_of_day) > pd.Timedelta(seconds=2):
                 # Non-working interval between last_available and the start of the day
                 found = True
             else:
                 # Move to previous day at 23:59:59.999999
-                last_available = (last_available - pd.Timedelta(days=1)).replace(hour=23, minute=59, second=59, microsecond=999999)
+                last_available = (last_available - pd.Timedelta(days=1)).replace(
+                    hour=23, minute=59, second=59, microsecond=999999
+                )
         # If last_available moved previously to the start of the queried interval
         if last_available <= start:
             # Stop and set to the start of the queried interval
             found = True
             last_available = start
     # Return last available timestamp
     return last_available
 
 
 def absolute_unavailability_intervals_within(
-        start: pd.Timestamp,
-        end: pd.Timestamp,
-        schedule: RCalendar
+    start: pd.Timestamp, end: pd.Timestamp, schedule: RCalendar
 ) -> List[Interval]:
     """
     Compute the list of intervals (in absolute timestamps) from [start] to [end] where, based on the working intervals in [schedule], the
     resource is not working.
 
     :param start:       Start of the interval to get the non-working periods from.
     :param end:         End of the interval to get the non-working periods from.
@@ -196,25 +230,39 @@
         current_instant = start
         while current_instant < end:
             # Go over the working intervals of the current weekday, storing the non-working periods
             day_intervals = schedule.work_intervals[current_instant.weekday()]
             for interval in day_intervals:
                 # Move interval to current day
                 interval_start = interval.start.replace(
-                    day=current_instant.day, month=current_instant.month, year=current_instant.year, tzinfo=pytz.timezone('UTC')
+                    day=current_instant.day,
+                    month=current_instant.month,
+                    year=current_instant.year,
+                    tzinfo=pytz.timezone("UTC"),
                 )
                 interval_end = interval.end.replace(
-                    day=current_instant.day, month=current_instant.month, year=current_instant.year, tzinfo=pytz.timezone('UTC')
+                    day=current_instant.day,
+                    month=current_instant.month,
+                    year=current_instant.year,
+                    tzinfo=pytz.timezone("UTC"),
                 )
                 if current_instant < interval_end:
                     if current_instant < interval_start:
                         # Non-working time gap between [current_instant] and the start of the current working interval, save it
-                        non_working_intervals += [Interval(current_instant, min(interval_start, end))]
+                        non_working_intervals += [
+                            Interval(current_instant, min(interval_start, end))
+                        ]
                     # Advance [current_instant] to the end of the working interval
                     current_instant = min(interval_end, end)
             # Current day finished, add non-working interval from current instant to end of day and advance
-            end_of_day = current_instant.replace(hour=23, minute=59, second=59, microsecond=0) + pd.Timedelta(microseconds=999999)
+            end_of_day = current_instant.replace(
+                hour=23, minute=59, second=59, microsecond=0
+            ) + pd.Timedelta(microseconds=999999)
             if current_instant < end:
-                non_working_intervals += [Interval(current_instant, min(end_of_day, end))]
-                current_instant = (current_instant + pd.Timedelta(days=1)).replace(hour=0, minute=0, second=0, microsecond=0)
+                non_working_intervals += [
+                    Interval(current_instant, min(end_of_day, end))
+                ]
+                current_instant = (current_instant + pd.Timedelta(days=1)).replace(
+                    hour=0, minute=0, second=0, microsecond=0
+                )
     # Return found non-working intervals
     return non_working_intervals
```

### Comparing `pix_framework-0.7.0/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.7.1/src/pix_framework/filesystem/file_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 import os
 import shutil
 import uuid
 from pathlib import Path
 
 
-def get_random_folder_id(prefix: str = '') -> str:
-    return f'{prefix}{get_random_id()}'
+def get_random_folder_id(prefix: str = "") -> str:
+    return f"{prefix}{get_random_id()}"
 
 
-def get_random_file_id(extension: str, prefix: str = '') -> str:
-    return f'{prefix}{get_random_id()}.{extension}'
+def get_random_file_id(extension: str, prefix: str = "") -> str:
+    return f"{prefix}{get_random_id()}.{extension}"
 
 
 def get_random_id() -> str:
     return f'{datetime.datetime.today().strftime("%Y%m%d_%H%M%S")}_{str(uuid.uuid4()).upper().replace("-", "_")}'
 
 
 def create_folder(path: Path) -> bool:
```

### Comparing `pix_framework-0.7.0/src/pix_framework/input.py` & `pix_framework-0.7.1/src/pix_framework/input.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.0/src/pix_framework/log_ids.py` & `pix_framework-0.7.1/src/pix_framework/log_ids.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 from dataclasses import dataclass, fields
 
 
 @dataclass
 class EventLogIDs:
     # General
-    case: str = 'case'  # Case ID
-    activity: str = 'activity'  # Activity label
-    resource: str = 'resource'  # Resource who performed this activity instance
-    start_time: str = 'start_time'  # Start time of the activity instance
-    end_time: str = 'end_time'  # End time of the activity instance
+    case: str = "case"  # Case ID
+    activity: str = "activity"  # Activity label
+    resource: str = "resource"  # Resource who performed this activity instance
+    start_time: str = "start_time"  # Start time of the activity instance
+    end_time: str = "end_time"  # End time of the activity instance
     # Start time estimator
-    enabled_time: str = 'enabled_time'  # Enablement time of the activity instance
-    enabling_activity: str = 'enabling_activity'  # Label of the activity instance enabling the current one
-    available_time: str = 'available_time'  # Last availability time of the resource who performed this activity instance
-    estimated_start_time: str = 'estimated_start_time'  # Estimated start time of the activity instance
+    enabled_time: str = "enabled_time"  # Enablement time of the activity instance
+    enabling_activity: str = (
+        "enabling_activity"  # Label of the activity instance enabling the current one
+    )
+    available_time: str = "available_time"  # Last availability time of the resource who performed this activity instance
+    estimated_start_time: str = (
+        "estimated_start_time"  # Estimated start time of the activity instance
+    )
 
     @staticmethod
-    def from_dict(config: dict) -> 'EventLogIDs':
+    def from_dict(config: dict) -> "EventLogIDs":
         return EventLogIDs(**config)
 
     def to_dict(self) -> dict:
-        return {
-            attr.name: getattr(self, attr.name)
-            for attr in fields(self.__class__)
-        }
-
-
-DEFAULT_CSV_IDS = EventLogIDs(case='case_id',
-                              activity='Activity',
-                              enabled_time='enabled_time',
-                              start_time='start_time',
-                              end_time='end_time',
-                              available_time='available_time',
-                              estimated_start_time='estimated_start_time',
-                              resource='Resource')
-
-DEFAULT_XES_IDS = EventLogIDs(case='case:concept:name',
-                              activity='concept:name',
-                              enabled_time='time:enabled',
-                              start_time='start_timestamp',  # Compatibility with PM4PY
-                              end_time='time:timestamp',
-                              available_time='time:available',
-                              estimated_start_time='time:estimated_start',
-                              resource='org:resource')
-
-APROMORE_LOG_IDS = EventLogIDs(case='Case_ID',
-                               activity='Activity',
-                               start_time='Start_Time',
-                               end_time='End_Time',
-                               resource='Resource')
-
-PROSIMOS_LOG_IDS = EventLogIDs(case='case_id',
-                               activity='activity',
-                               enabled_time='enabled_time',
-                               start_time='start_time',
-                               end_time='end_time',
-                               resource='resource')
+        return {attr.name: getattr(self, attr.name) for attr in fields(self.__class__)}
+
+
+DEFAULT_CSV_IDS = EventLogIDs(
+    case="case_id",
+    activity="Activity",
+    enabled_time="enabled_time",
+    start_time="start_time",
+    end_time="end_time",
+    available_time="available_time",
+    estimated_start_time="estimated_start_time",
+    resource="Resource",
+)
+
+DEFAULT_XES_IDS = EventLogIDs(
+    case="case:concept:name",
+    activity="concept:name",
+    enabled_time="time:enabled",
+    start_time="start_timestamp",  # Compatibility with PM4PY
+    end_time="time:timestamp",
+    available_time="time:available",
+    estimated_start_time="time:estimated_start",
+    resource="org:resource",
+)
+
+APROMORE_LOG_IDS = EventLogIDs(
+    case="Case_ID",
+    activity="Activity",
+    start_time="Start_Time",
+    end_time="End_Time",
+    resource="Resource",
+)
+
+PROSIMOS_LOG_IDS = EventLogIDs(
+    case="case_id",
+    activity="activity",
+    enabled_time="enabled_time",
+    start_time="start_time",
+    end_time="end_time",
+    resource="resource",
+)
```

### Comparing `pix_framework-0.7.0/src/pix_framework/log_split/log_split.py` & `pix_framework-0.7.1/src/pix_framework/log_split/log_split.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.7.0/src/pix_framework/statistics/distribution.py` & `pix_framework-0.7.1/src/pix_framework/statistics/distribution.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     TRIANGULAR = "triang"
     EXPONENTIAL = "expon"
     LOG_NORMAL = "lognorm"
     GAMMA = "gamma"
     FIXED = "fix"
 
     @staticmethod
-    def from_string(value: str) -> 'DistributionType':
+    def from_string(value: str) -> "DistributionType":
         name = value.lower()
         if name == "uniform":
             return DistributionType.UNIFORM
         elif name in ("norm", "normal"):
             return DistributionType.NORMAL
         elif name in ("triang", "triangular"):
             return DistributionType.TRIANGULAR
@@ -49,20 +49,27 @@
     arg1: str = "NaN"
     arg2: str = "NaN"
     unit: str = "seconds"  # This is the unit to show in the interface by transforming the values in seconds
 
 
 class DurationDistribution:
     def __init__(
-            self,
-            name: Union[str, DistributionType] = "fix",  # supported 'fix', 'expon', 'norm', 'uniform', 'lognorm', and 'gamma'
-            mean: float = 0.0, var: float = 0.0, std: float = 0.0,
-            minimum: float = 0.0, maximum: float = 0.0,
+        self,
+        name: Union[
+            str, DistributionType
+        ] = "fix",  # supported 'fix', 'expon', 'norm', 'uniform', 'lognorm', and 'gamma'
+        mean: float = 0.0,
+        var: float = 0.0,
+        std: float = 0.0,
+        minimum: float = 0.0,
+        maximum: float = 0.0,
     ):
-        self.type = DistributionType.from_string(name) if isinstance(name, str) else name
+        self.type = (
+            DistributionType.from_string(name) if isinstance(name, str) else name
+        )
         self.mean = mean
         self.var = var
         self.std = std
         self.min = minimum
         self.max = maximum
 
     def generate_sample(self, size: int) -> list:
@@ -78,184 +85,182 @@
             sample = st.uniform.rvs(loc=self.min, scale=self.max - self.min, size=size)
         elif self.type == DistributionType.LOG_NORMAL:
             # If the distribution corresponds to a 'lognorm' with loc!=0, the estimation is done wrong
             # dunno how to take that into account
             pow_mean = pow(self.mean, 2)
             phi = math.sqrt(self.var + pow_mean)
             mu = math.log(pow_mean / phi)
-            sigma = math.sqrt(math.log(phi ** 2 / pow_mean))
+            sigma = math.sqrt(math.log(phi**2 / pow_mean))
             sample = st.lognorm.rvs(sigma, loc=0, scale=math.exp(mu), size=size)
         elif self.type == DistributionType.GAMMA:
             # If the distribution corresponds to a 'gamma' with loc!=0, the estimation is done wrong
             # dunno how to take that into account
-            sample = st.gamma.rvs(pow(self.mean, 2) / self.var, loc=0, scale=self.var / self.mean, size=size)
+            sample = st.gamma.rvs(
+                pow(self.mean, 2) / self.var,
+                loc=0,
+                scale=self.var / self.mean,
+                size=size,
+            )
         # Return generated sample
         return sample
 
-    def scale_distribution(self, alpha: float) -> 'DurationDistribution':
+    def scale_distribution(self, alpha: float) -> "DurationDistribution":
         return DurationDistribution(
             name=self.type,
             mean=self.mean * alpha,  # Mean: scaled by multiplying by [alpha]
-            var=self.var * alpha * alpha,  # Variance: scaled by multiplying by [alpha]^2
+            var=self.var
+            * alpha
+            * alpha,  # Variance: scaled by multiplying by [alpha]^2
             std=self.std * alpha,  # STD: scaled by multiplying by [alpha]
             minimum=self.min * alpha,  # Min: scaled by multiplying by [alpha]
-            maximum=self.max * alpha  # Max: scaled by multiplying by [alpha]
+            maximum=self.max * alpha,  # Max: scaled by multiplying by [alpha]
         )
 
     def to_prosimos_distribution(self) -> dict:
         # Initialize empty list of params
         distribution_params = []
         # Add specific params depending on distribution
         if self.type == DistributionType.FIXED:
-            distribution_params += [
-                {'value': self.mean}  # fixed value
-            ]
+            distribution_params += [{"value": self.mean}]  # fixed value
         elif self.type == DistributionType.EXPONENTIAL:
             distribution_params += [
-                {'value': self.min},  # loc
-                {'value': self.mean - self.min},  # scale
-                {'value': self.min},  # min
-                {'value': self.max}  # max
+                {"value": self.min},  # loc
+                {"value": self.mean - self.min},  # scale
+                {"value": self.min},  # min
+                {"value": self.max},  # max
             ]
         elif self.type == DistributionType.NORMAL:
             distribution_params += [
-                {'value': self.mean},  # loc
-                {'value': self.std},  # scale
-                {'value': self.min},  # min
-                {'value': self.max}  # max
+                {"value": self.mean},  # loc
+                {"value": self.std},  # scale
+                {"value": self.min},  # min
+                {"value": self.max},  # max
             ]
         elif self.type == DistributionType.UNIFORM:
             distribution_params += [
-                {'value': self.min},  # loc
-                {'value': self.max - self.min},  # scale
-                {'value': self.min},  # min
-                {'value': self.max}  # max
+                {"value": self.min},  # loc
+                {"value": self.max - self.min},  # scale
+                {"value": self.min},  # min
+                {"value": self.max},  # max
             ]
         elif self.type == DistributionType.LOG_NORMAL:
             # If the distribution corresponds to a 'lognorm' with loc!=0, the estimation is done wrong
             # dunno how to take that into account
             pow_mean = pow(self.mean, 2)
             phi = math.sqrt(self.var + pow_mean)
             mu = math.log(pow_mean / phi)
-            sigma = math.sqrt(math.log(phi ** 2 / pow_mean))
+            sigma = math.sqrt(math.log(phi**2 / pow_mean))
             distribution_params += [
-                {'value': sigma},  # sigma
-                {'value': 0},  # loc
-                {'value': math.exp(mu)},  # scale
-                {'value': self.min},  # min
-                {'value': self.max}  # max
+                {"value": sigma},  # sigma
+                {"value": 0},  # loc
+                {"value": math.exp(mu)},  # scale
+                {"value": self.min},  # min
+                {"value": self.max},  # max
             ]
         elif self.type == DistributionType.GAMMA:
             # If the distribution corresponds to a 'gamma' with loc!=0, the estimation is done wrong
             # dunno how to take that into account
             distribution_params += [
-                {'value': pow(self.mean, 2) / self.var},  # a
-                {'value': 0},  # loc
-                {'value': self.var / self.mean},  # scale
-                {'value': self.min},  # min
-                {'value': self.max}  # max
+                {"value": pow(self.mean, 2) / self.var},  # a
+                {"value": 0},  # loc
+                {"value": self.var / self.mean},  # scale
+                {"value": self.min},  # min
+                {"value": self.max},  # max
             ]
         else:
             raise ValueError(f"Unsupported distribution: {self}")
         # Return dict with the distribution data as expected by PROSIMOS
-        return {'distribution_name': self.type.value, 'distribution_params': distribution_params}
+        return {
+            "distribution_name": self.type.value,
+            "distribution_params": distribution_params,
+        }
 
     def to_qbp_distribution(self) -> QBPDurationDistribution:
         # Initialize empty distribution
         qbp_distribution = None
         # Parse distribution
         if self.type == DistributionType.FIXED:
             qbp_distribution = QBPDurationDistribution(
-                type="FIXED",
-                mean=str(self.mean),
-                arg1="0",
-                arg2="0"
+                type="FIXED", mean=str(self.mean), arg1="0", arg2="0"
             )
         elif self.type == DistributionType.EXPONENTIAL:
             # For the XML mean=0 and arg2=0
             qbp_distribution = QBPDurationDistribution(
-                type="EXPONENTIAL",
-                mean="0",
-                arg1=str(self.mean),
-                arg2="0"
+                type="EXPONENTIAL", mean="0", arg1=str(self.mean), arg2="0"
             )
         elif self.type == DistributionType.NORMAL:
             # For the XML arg1=std and arg2=0
             qbp_distribution = QBPDurationDistribution(
-                type="NORMAL",
-                mean=str(self.mean),
-                arg1=str(self.std),
-                arg2="0"
+                type="NORMAL", mean=str(self.mean), arg1=str(self.std), arg2="0"
             )
         elif self.type == DistributionType.UNIFORM:
             # For the XML the mean is always 3600, arg1=min and arg2=max
             qbp_distribution = QBPDurationDistribution(
-                type="UNIFORM",
-                mean="3600",
-                arg1=str(self.min),
-                arg2=str(self.max)
+                type="UNIFORM", mean="3600", arg1=str(self.min), arg2=str(self.max)
             )
         elif self.type == DistributionType.LOG_NORMAL:
             # For the XML arg1=var and arg2=0
             qbp_distribution = QBPDurationDistribution(
-                type="LOGNORMAL",
-                mean=str(self.mean),
-                arg1=str(self.var),
-                arg2="0"
+                type="LOGNORMAL", mean=str(self.mean), arg1=str(self.var), arg2="0"
             )
         elif self.type == DistributionType.GAMMA:
             # For the XML arg1=var and arg2=0
             qbp_distribution = QBPDurationDistribution(
-                type="GAMMA",
-                mean=str(self.mean),
-                arg1=str(self.var),
-                arg2="0"
+                type="GAMMA", mean=str(self.mean), arg1=str(self.var), arg2="0"
             )
         # Return parsed distribution
         return qbp_distribution
 
     def __str__(self):
         return "DurationDistribution(name: {}, mean: {}, var: {}, std: {}, min: {}, max: {})".format(
             self.type.value, self.mean, self.var, self.std, self.min, self.max
         )
 
 
-def get_best_fitting_distribution(data: list, filter_outliers: bool = False) -> DurationDistribution:
+def get_best_fitting_distribution(
+    data: list, filter_outliers: bool = False
+) -> DurationDistribution:
     """
     Discover the distribution (exponential, normal, uniform, log-normal, and gamma) that best fits the values in [data].
 
     :param data:            Values to fit a distribution for.
     :param filter_outliers: If true, remove outliers from the sample.
 
     :return: the best fitting distribution.
     """
     # Filter outliers
     filtered_data = remove_outliers(data) if filter_outliers else data
     # Check for fixed value
     fix_value = _check_fix(filtered_data)
     if fix_value is not None:
         # If it is a fixed value, infer distribution
-        distribution = DurationDistribution("fix", fix_value, 0.0, 0.0, fix_value, fix_value)
+        distribution = DurationDistribution(
+            "fix", fix_value, 0.0, 0.0, fix_value, fix_value
+        )
     else:
         # Otherwise, compute basic statistics and try with other distributions
         mean = np.mean(filtered_data)
         var = np.var(filtered_data)
         std = np.std(filtered_data)
         d_min = min(filtered_data)
         d_max = max(filtered_data)
         # Create distribution candidates
         dist_candidates = [
             DurationDistribution("expon", mean, var, std, d_min, d_max),
             DurationDistribution("norm", mean, var, std, d_min, d_max),
-            DurationDistribution("uniform", mean, var, std, d_min, d_max)
+            DurationDistribution("uniform", mean, var, std, d_min, d_max),
         ]
         if mean != 0:
-            dist_candidates += [DurationDistribution("lognorm", mean, var, std, d_min, d_max)]
+            dist_candidates += [
+                DurationDistribution("lognorm", mean, var, std, d_min, d_max)
+            ]
             if var != 0:
-                dist_candidates += [DurationDistribution("gamma", mean, var, std, d_min, d_max)]
+                dist_candidates += [
+                    DurationDistribution("gamma", mean, var, std, d_min, d_max)
+                ]
         # Search for the best one within the candidates
         best_distribution = None
         best_emd = sys.float_info.max
         for distribution_candidate in dist_candidates:
             # Generate a list of observations from the distribution
             generated_data = distribution_candidate.generate_sample(len(filtered_data))
             # Compute its distance with the observed data
@@ -266,30 +271,34 @@
                 best_distribution = distribution_candidate
         # Set the best distribution as the one to return
         distribution = best_distribution
     # Return best distribution
     return distribution
 
 
-def _check_fix(data:list, delta=5):
+def _check_fix(data: list, delta=5):
     value = None
     counter = Counter(data)
     counter[None] = 0
     for d1 in counter:
-        if (counter[d1] > counter[value]) and (sum([abs(d1 - d2) < delta for d2 in data]) / len(data) > 0.95):
+        if (counter[d1] > counter[value]) and (
+            sum([abs(d1 - d2) < delta for d2 in data]) / len(data) > 0.95
+        ):
             # If the value [d1] is more frequent than the current fixed one [value]
             # and
             # the ratio of values similar (or with a difference lower than [delta]) to [d1] is more than 90%
             # update value
             value = d1
     # Return fixed value with more apparitions
     return value
 
 
-def get_observations_histogram(data: list, num_bins: int = 20, filter_outliers: bool = False) -> dict:
+def get_observations_histogram(
+    data: list, num_bins: int = 20, filter_outliers: bool = False
+) -> dict:
     """
     Build a histogram with the values in [data], with [num_bins] bins. It builds the histogram, computes the CDF and the values of each
     bin of the CDF.
 
     :param data:            Data to build the histogram.
     :param num_bins:        Number of bins to use in the histogram.
     :param filter_outliers: If true, remove outliers from the sample.
@@ -299,13 +308,13 @@
     filtered_durations = remove_outliers(data) if filter_outliers else data
     bins = np.linspace(min(filtered_durations), max(filtered_durations), num_bins + 1)
     hist, _ = np.histogram(filtered_durations, bins=bins)
     cdf = np.cumsum(hist)
     cdf = cdf / cdf[-1]
     bin_midpoints = (bins[:-1] + bins[1:]) / 2
     return {
-        'distribution_name': "histogram_sampling",
-        'histogram_data': {
-            'cdf': [float(num) for num in cdf],
-            'bin_midpoints': [float(num) for num in bin_midpoints]
-        }
+        "distribution_name": "histogram_sampling",
+        "histogram_data": {
+            "cdf": [float(num) for num in cdf],
+            "bin_midpoints": [float(num) for num in bin_midpoints],
+        },
     }
```

### Comparing `pix_framework-0.7.0/src/pix_framework/statistics/utils.py` & `pix_framework-0.7.1/src/pix_framework/statistics/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-def remove_outliers(data: list, m=5.) -> list:
+def remove_outliers(data: list, m=5.0) -> list:
     """
     Remove outliers from a list of values following the approach presented in https://stackoverflow.com/a/16562028.
     :param data: list of values.
     :param m: maximum ratio between the difference (value - median) and the median of these differences, to NOT be
     considered an outlier. Decreasing the [m] ratio increases the number of detected outliers (observations closer
     to the median are considered as outliers).
     :return: the received list of values without the outliers.
```

### Comparing `pix_framework-0.7.0/PKG-INFO` & `pix_framework-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.7.0
+Version: 0.7.1
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PIX Framework
 
 ![pix-framework](https://github.com/AutomatedProcessImprovement/pix-framework/actions/workflows/build.yaml/badge.svg)
 ![version](https://img.shields.io/github/v/tag/AutomatedProcessImprovement/pix-framework)
```

