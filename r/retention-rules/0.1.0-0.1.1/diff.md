# Comparing `tmp/retention-rules-0.1.0.tar.gz` & `tmp/retention-rules-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retention-rules-0.1.0.tar", last modified: Fri May  5 04:29:43 2023, max compression
+gzip compressed data, was "retention-rules-0.1.1.tar", last modified: Fri May  5 19:33:10 2023, max compression
```

## Comparing `retention-rules-0.1.0.tar` & `retention-rules-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2023-05-05 04:29:43.459826 retention-rules-0.1.0/
--rw-r--r--   0 matt      (1000) matt      (1000)     1071 2023-05-05 04:03:32.000000 retention-rules-0.1.0/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)     8055 2023-05-05 04:29:43.459826 retention-rules-0.1.0/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     7561 2023-05-05 04:03:32.000000 retention-rules-0.1.0/README.md
--rw-r--r--   0 matt      (1000) matt      (1000)      542 2023-05-05 04:15:53.000000 retention-rules-0.1.0/pyproject.toml
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2023-05-05 04:29:43.459826 retention-rules-0.1.0/retention_rules/
--rw-r--r--   0 matt      (1000) matt      (1000)       72 2023-05-05 04:03:32.000000 retention-rules-0.1.0/retention_rules/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1958 2023-05-05 04:03:32.000000 retention-rules-0.1.0/retention_rules/builder.py
--rw-r--r--   0 matt      (1000) matt      (1000)     5112 2023-05-05 04:06:45.000000 retention-rules-0.1.0/retention_rules/periods.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2666 2023-05-05 04:03:32.000000 retention-rules-0.1.0/retention_rules/policy.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2023-05-05 04:29:43.459826 retention-rules-0.1.0/retention_rules.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     8055 2023-05-05 04:29:43.000000 retention-rules-0.1.0/retention_rules.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      403 2023-05-05 04:29:43.000000 retention-rules-0.1.0/retention_rules.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2023-05-05 04:29:43.000000 retention-rules-0.1.0/retention_rules.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       16 2023-05-05 04:29:43.000000 retention-rules-0.1.0/retention_rules.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       38 2023-05-05 04:29:43.459826 retention-rules-0.1.0/setup.cfg
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2023-05-05 04:29:43.459826 retention-rules-0.1.0/tests/
--rw-r--r--   0 matt      (1000) matt      (1000)     2644 2023-05-05 04:03:32.000000 retention-rules-0.1.0/tests/test_build.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4873 2023-05-05 04:07:17.000000 retention-rules-0.1.0/tests/test_period_advancement.py
--rw-r--r--   0 matt      (1000) matt      (1000)     3458 2023-05-05 04:03:32.000000 retention-rules-0.1.0/tests/test_period_start_times.py
--rw-r--r--   0 matt      (1000) matt      (1000)     3188 2023-05-05 04:03:32.000000 retention-rules-0.1.0/tests/test_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:33:10.411959 retention-rules-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 19:32:58.000000 retention-rules-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18608 2023-05-05 19:33:10.411959 retention-rules-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-05 19:32:58.000000 retention-rules-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-05 19:32:58.000000 retention-rules-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:33:10.411959 retention-rules-0.1.1/retention_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 19:32:58.000000 retention-rules-0.1.1/retention_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-05 19:32:58.000000 retention-rules-0.1.1/retention_rules/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-05 19:32:58.000000 retention-rules-0.1.1/retention_rules/periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-05 19:32:58.000000 retention-rules-0.1.1/retention_rules/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:33:10.411959 retention-rules-0.1.1/retention_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18608 2023-05-05 19:33:10.000000 retention-rules-0.1.1/retention_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 19:33:10.000000 retention-rules-0.1.1/retention_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:33:10.000000 retention-rules-0.1.1/retention_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 19:33:10.000000 retention-rules-0.1.1/retention_rules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:33:10.411959 retention-rules-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:33:10.411959 retention-rules-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-05 19:32:58.000000 retention-rules-0.1.1/tests/test_build_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-05 19:32:58.000000 retention-rules-0.1.1/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-05 19:32:58.000000 retention-rules-0.1.1/tests/test_period_advancement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-05 19:32:58.000000 retention-rules-0.1.1/tests/test_period_start_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-05-05 19:32:58.000000 retention-rules-0.1.1/tests/test_policy.py
```

### Comparing `retention-rules-0.1.0/LICENSE` & `retention-rules-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `retention-rules-0.1.0/pyproject.toml` & `retention-rules-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.7.2", "wheel"]
 
 [project]
 name = "retention-rules"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Matt Jarvis"},
 ]
 description = "A library to calculate period-based retention rules for timestamps"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `retention-rules-0.1.0/retention_rules/builder.py` & `retention-rules-0.1.1/retention_rules/builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,64 +7,78 @@
         "rules": [
             {"applies_for": "3D", "retain_every": "H/4"},
             {"applies_for": "2W", "retain_every": "H"},
             {"applies_for": "M", "retain_every": "D/2"},
             {"applies_for": "6M", "retain_every": "W/2"},
             {"applies_for": "Y", "retain_every": "W"},
             {"applies_for": "10Y", "retain_every": "M"},
-        ]
+        ],
+        "retain": "oldest",
+        "reuse": True
     }
 
 """
 
 import re
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Callable
 
-from .policy import RetentionPolicy
+from .policy import RetentionPolicy, RetainStrategy
 from .periods import *
 
 
-def build_policy(policy_dict: Dict) -> RetentionPolicy:
-    policy = RetentionPolicy()
-    rule_items = policy_dict.get("rules", [])
-    if not rule_items:
-        raise ValueError("Policy must contain at least one rule in the 'rules' key")
-
-    for rule in rule_items:
-        applies, count = parse_period_text(rule["applies_for"])
-        retain_every, rcount = parse_period_text(rule["retain_every"])
-        if rcount != 1:
-            raise ValueError(f"Retain-every does not currently support a count")
+class PolicyBuilder:
+    def __init__(self, **kwargs):
+        self.keys: Dict[str, Callable[[], Period]] = kwargs.get("keys", _by_key)
 
-        policy.add_rule(applies, count, retain_every)
-    return policy
+    def build(self, policy_dict: Dict) -> RetentionPolicy:
+        retain = RetainStrategy(policy_dict.get("retain", "oldest"))
+        reuse = policy_dict.get("reuse", False)
+        policy = RetentionPolicy(retain_strategy=retain, reuse_in_group=reuse)
 
+        rule_items = policy_dict.get("rules", [])
+        if not rule_items:
+            raise ValueError("Policy must contain at least one rule in the 'rules' key")
 
-_key_pattern = re.compile(r"^(\d+)?(Y|M|W|D|H|MIN|S)(/\d+)?$")
+        for rule in rule_items:
+            applies_text = rule["applies_for"]
+            retain_text = rule["retain_every"]
+
+            applies, count = self._parse_key_text(applies_text)
+            retain_every, rcount = self._parse_key_text(retain_text)
+            if rcount != 1:
+                raise ValueError(f"Retain-every does not currently support a count")
+
+            note = rule.get("note", None) or f"{applies_text} retain {retain_text}"
+            policy.add_rule(applies, count, retain_every, note)
+
+        return policy
+
+    def _parse_key_text(self, text: str):
+        match = _key_pattern.match(text)
+        if not match:
+            raise ValueError(f"Invalid specifier: {text}")
+
+        count = int(match.group(1) or 1)
+        unit_key = match.group(2)
+        sub_div = match.group(3)
+
+        period_cls = self.keys.get(unit_key, None)
+        if not period_cls:
+            raise ValueError(f"PolicyBuilder could not find a period associated with the key: {unit_key}")
+
+        period = period_cls()
+        if sub_div:
+            period = SubdividedPeriod(period, int(sub_div[1:]))
+
+        return period, count
+
+
+_key_pattern = re.compile(r"^(\d+)?(\w+)(/\d+)?$")
 
 _by_key = {
     "Y": Year,
     "M": Month,
     "W": Week,
     "D": Day,
     "H": Hour,
     "MIN": Minute,
 }
-
-
-def parse_period_text(text: str) -> Tuple[Period, int]:
-    match = _key_pattern.match(text)
-    if not match:
-        raise ValueError(f"Invalid period: {text}")
-
-    count = int(match.group(1) or 1)
-    unit = match.group(2)
-    sub_div = match.group(3)
-
-    period_cls = _by_key.get(unit, None)
-    if not period_cls:
-        raise ValueError(f"Could not find period for unit: {unit}")
-
-    period = period_cls()
-    if sub_div:
-        period = SubdividedPeriod(period, int(sub_div[1:]))
-    return period, count
```

### Comparing `retention-rules-0.1.0/retention_rules/periods.py` & `retention-rules-0.1.1/retention_rules/periods.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     incrementing the integer by one and the previous period can be found by decrementing it by one.  The easiest
     example of this is a "year", which is simply the year associated with the date.  There is a difference between
     specifying that one wants to retain data from each year, vs specifying that one wants to retain data from increments
     of time backwards from the present we usually associate with a year.
 
 """
 
-from abc import ABC, abstractmethod
+from abc import ABC
 from datetime import datetime as DateTime, timedelta as TimeDelta
 
 _reference_date = DateTime(1970, 1, 1)
 
 
 def _year(time_stamp: DateTime) -> int:
     return time_stamp.year - _reference_date.year
@@ -59,25 +59,31 @@
         internal_start = self._sub_period.period_start(p)
         internal_next = self._sub_period.period_start(p + 1)
         return internal_start + (internal_next - internal_start) * (period % self._sub_div) / self._sub_div
 
     def max_duration(self) -> TimeDelta:
         return self._sub_period.max_duration() / self._sub_div
 
+    def __repr__(self):
+        return f"{self._sub_period}/{self._sub_div}"
+
 
 class Year(Period):
     def to_period(self, time_stamp: DateTime) -> int:
         return _year(time_stamp)
 
     def max_duration(self) -> TimeDelta:
         return TimeDelta(days=366)
 
     def period_start(self, period: int) -> DateTime:
         return DateTime(_reference_date.year + period, 1, 1)
 
+    def __repr__(self):
+        return "Year"
+
 
 class Month(Period):
     def to_period(self, time_stamp: DateTime) -> int:
         return _year(time_stamp) * 12 + time_stamp.month
 
     def max_duration(self) -> TimeDelta:
         return TimeDelta(days=31)
@@ -86,52 +92,67 @@
         year = _reference_date.year + (period // 12)
         month = period % 12
         if month == 0:
             month = 12
             year -= 1
         return DateTime(year, month, 1)
 
+    def __repr__(self):
+        return "Month"
+
 
 class Week(Period):
     def to_period(self, time_stamp: DateTime) -> int:
         # This is easier than dealing with the years that have 53 weeks
         days = _day(time_stamp) - _reference_date.isocalendar()[2]
         return days // 7
 
     def max_duration(self) -> TimeDelta:
         return TimeDelta(days=7)
 
     def period_start(self, period: int) -> DateTime:
         return _reference_date + TimeDelta(days=(period * 7) + _reference_date.isocalendar()[2])
 
+    def __repr__(self):
+        return "Week"
+
 
 class Day(Period):
     def to_period(self, time_stamp: DateTime) -> int:
         return _day(time_stamp)
 
     def max_duration(self) -> TimeDelta:
         return TimeDelta(hours=24)
 
     def period_start(self, period: int) -> DateTime:
         return _reference_date + TimeDelta(days=period)
 
+    def __repr__(self):
+        return "Day"
+
 
 class Hour(Period):
     def to_period(self, time_stamp: DateTime) -> int:
         return _day(time_stamp) * 24 + time_stamp.hour
 
     def max_duration(self) -> TimeDelta:
         return TimeDelta(minutes=60)
 
     def period_start(self, period: int) -> DateTime:
         return _reference_date + TimeDelta(hours=period)
 
+    def __repr__(self):
+        return "Hour"
+
 
 class Minute(Period):
     def to_period(self, time_stamp: DateTime) -> int:
         return (_day(time_stamp) * 24 + time_stamp.hour) * 60 + time_stamp.minute
 
     def max_duration(self) -> TimeDelta:
         return TimeDelta(seconds=60)
 
     def period_start(self, period: int) -> DateTime:
         return _reference_date + TimeDelta(minutes=period)
+
+    def __repr__(self):
+        return "Minute"
```

### Comparing `retention-rules-0.1.0/tests/test_build.py` & `retention-rules-0.1.1/tests/test_build_parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Tests to check the policy building
 """
 from typing import Tuple
 
-from retention_rules.builder import build_policy, parse_period_text
+from retention_rules.builder import PolicyBuilder
 from retention_rules.periods import Period, Year, Month, Week, Day, Hour, Minute, SubdividedPeriod
 
 
 def test_parse_simple():
     assert parse_period_text("Y") == _Check(Year(), 1)
     assert parse_period_text("M") == _Check(Month(), 1)
     assert parse_period_text("W") == _Check(Week(), 1)
@@ -39,14 +39,19 @@
     assert parse_period_text("3M/2") == _Check(SubdividedPeriod(Month(), 2), 3)
     assert parse_period_text("3W/2") == _Check(SubdividedPeriod(Week(), 2), 3)
     assert parse_period_text("3D/2") == _Check(SubdividedPeriod(Day(), 2), 3)
     assert parse_period_text("3H/2") == _Check(SubdividedPeriod(Hour(), 2), 3)
     assert parse_period_text("3MIN/2") == _Check(SubdividedPeriod(Minute(), 2), 3)
 
 
+def parse_period_text(text: str):
+    b = PolicyBuilder()
+    return b._parse_key_text(text)
+
+
 class _Check:
     def __init__(self, period, count: int):
         self.period = period
         self.count = count
 
     def __eq__(self, other: Tuple[Period, int]):
         if isinstance(other[0], SubdividedPeriod):
```

### Comparing `retention-rules-0.1.0/tests/test_period_advancement.py` & `retention-rules-0.1.1/tests/test_period_advancement.py`

 * *Files identical despite different names*

### Comparing `retention-rules-0.1.0/tests/test_period_start_times.py` & `retention-rules-0.1.1/tests/test_period_start_times.py`

 * *Files identical despite different names*

