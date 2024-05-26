# Comparing `tmp/RecoLul-1.8.0.tar.gz` & `tmp/RecoLul-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecoLul-1.8.0.tar", last modified: Mon May 15 02:02:39 2023, max compression
+gzip compressed data, was "RecoLul-1.9.0.tar", last modified: Tue Aug 15 09:32:38 2023, max compression
```

## Comparing `RecoLul-1.8.0.tar` & `RecoLul-1.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.462144 RecoLul-1.8.0/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1069 2022-10-28 02:03:59.000000 RecoLul-1.8.0/LICENSE
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-05-15 02:02:39.462144 RecoLul-1.8.0/PKG-INFO
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      643 2023-02-06 08:29:19.000000 RecoLul-1.8.0/README.md
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.458144 RecoLul-1.8.0/RecoLul.egg-info/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/PKG-INFO
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      434 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/SOURCES.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        1 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/dependency_links.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       45 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/entry_points.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       81 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/requires.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        8 2023-05-15 02:02:39.000000 RecoLul-1.8.0/RecoLul.egg-info/top_level.txt
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      100 2022-10-19 06:32:10.000000 RecoLul-1.8.0/pyproject.toml
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.462144 RecoLul-1.8.0/recolul/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       22 2023-05-15 02:01:29.000000 RecoLul-1.8.0/recolul/__init__.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     4020 2023-04-07 06:25:37.000000 RecoLul-1.8.0/recolul/cli.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1325 2023-02-06 04:58:11.000000 RecoLul-1.8.0/recolul/config.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1237 2023-02-06 07:38:04.000000 RecoLul-1.8.0/recolul/duration.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      924 2023-02-09 07:26:16.000000 RecoLul-1.8.0/recolul/plotting.py
-drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-05-15 02:02:39.462144 RecoLul-1.8.0/recolul/recoru/
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        0 2023-02-22 01:29:18.000000 RecoLul-1.8.0/recolul/recoru/__init__.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2516 2023-05-15 01:53:12.000000 RecoLul-1.8.0/recolul/recoru/attendance_chart.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1723 2023-02-22 02:34:58.000000 RecoLul-1.8.0/recolul/recoru/recoru_session.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2416 2023-05-15 01:57:40.000000 RecoLul-1.8.0/recolul/time.py
--rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      739 2023-05-15 02:02:39.462144 RecoLul-1.8.0/setup.cfg
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-08-15 09:32:38.951150 RecoLul-1.9.0/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1069 2022-10-28 02:03:59.000000 RecoLul-1.9.0/LICENSE
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-08-15 09:32:38.951150 RecoLul-1.9.0/PKG-INFO
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      643 2023-02-06 08:29:19.000000 RecoLul-1.9.0/README.md
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-08-15 09:32:38.951150 RecoLul-1.9.0/RecoLul.egg-info/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1051 2023-08-15 09:32:38.000000 RecoLul-1.9.0/RecoLul.egg-info/PKG-INFO
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      434 2023-08-15 09:32:38.000000 RecoLul-1.9.0/RecoLul.egg-info/SOURCES.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        1 2023-08-15 09:32:38.000000 RecoLul-1.9.0/RecoLul.egg-info/dependency_links.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       45 2023-08-15 09:32:38.000000 RecoLul-1.9.0/RecoLul.egg-info/entry_points.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       81 2023-08-15 09:32:38.000000 RecoLul-1.9.0/RecoLul.egg-info/requires.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        8 2023-08-15 09:32:38.000000 RecoLul-1.9.0/RecoLul.egg-info/top_level.txt
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      100 2022-10-19 06:32:10.000000 RecoLul-1.9.0/pyproject.toml
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-08-15 09:32:38.951150 RecoLul-1.9.0/recolul/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)       22 2023-08-15 09:31:20.000000 RecoLul-1.9.0/recolul/__init__.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     4062 2023-08-15 09:25:04.000000 RecoLul-1.9.0/recolul/cli.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1325 2023-02-06 04:58:11.000000 RecoLul-1.9.0/recolul/config.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1294 2023-08-15 08:50:34.000000 RecoLul-1.9.0/recolul/duration.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      924 2023-02-09 07:26:16.000000 RecoLul-1.9.0/recolul/plotting.py
+drwxrwxr-x   0 jean-loup  (1000) jean-loup  (1000)        0 2023-08-15 09:32:38.951150 RecoLul-1.9.0/recolul/recoru/
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)        0 2023-02-22 01:29:18.000000 RecoLul-1.9.0/recolul/recoru/__init__.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     2516 2023-05-15 01:53:12.000000 RecoLul-1.9.0/recolul/recoru/attendance_chart.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     1723 2023-02-22 02:34:58.000000 RecoLul-1.9.0/recolul/recoru/recoru_session.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)     3039 2023-08-15 09:21:05.000000 RecoLul-1.9.0/recolul/time.py
+-rw-rw-r--   0 jean-loup  (1000) jean-loup  (1000)      739 2023-08-15 09:32:38.951150 RecoLul-1.9.0/setup.cfg
```

### Comparing `RecoLul-1.8.0/LICENSE` & `RecoLul-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RecoLul-1.8.0/PKG-INFO` & `RecoLul-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecoLul
-Version: 1.8.0
+Version: 1.9.0
 Summary: Overtime management for RecoRu
 Home-page: https://github.com/Maerig/recolul
 Author: Jean-Loup Roussel-Clouet
 Author-email: jean-loup@cryptact.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `RecoLul-1.8.0/README.md` & `RecoLul-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `RecoLul-1.8.0/RecoLul.egg-info/PKG-INFO` & `RecoLul-1.9.0/RecoLul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecoLul
-Version: 1.8.0
+Version: 1.9.0
 Summary: Overtime management for RecoRu
 Home-page: https://github.com/Maerig/recolul
 Author: Jean-Loup Roussel-Clouet
 Author-email: jean-loup@cryptact.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `RecoLul-1.8.0/recolul/cli.py` & `RecoLul-1.9.0/recolul/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import argparse
 import sys
-from datetime import datetime
 from getpass import getpass
 
 from recolul import plotting, time
 from recolul.config import Config
 from recolul.duration import Duration
 from recolul.recoru.attendance_chart import AttendanceChart
 from recolul.recoru.recoru_session import RecoruSession
-from recolul.time import get_work_time
+from recolul.time import get_work_time, until_today
 
 
 def balance(exclude_last_day: bool) -> None:
-    attendance_chart = _get_attendance_chart()
-    month = attendance_chart[:-1] if exclude_last_day else attendance_chart
-    overtime_balance, total_workplace_times = time.get_overtime_balance(month)
+    full_attendance_chart = _get_attendance_chart()
+    attendance_chart = until_today(full_attendance_chart)
+    if exclude_last_day and len(attendance_chart) > 1:
+        attendance_chart = attendance_chart[:-1]
+    overtime_balance, total_workplace_times = time.get_overtime_balance(attendance_chart)
     print(f"Monthly overtime balance: {overtime_balance}")
     print(f"Total time per workplace:")
     for workplace, total_work_time in total_workplace_times.items():
         print(f"  {workplace}: {total_work_time}")
+    print(f"Maximum WFH time this month: {Duration(60) * time.count_working_days(full_attendance_chart)}")
 
     if exclude_last_day:
         return
 
     last_day = attendance_chart[-1]
     print(f"\nLast day {last_day.day.text}")
     print(f"  Clock-in: {last_day.clock_in_time}")
     print(f"  Working hours: {get_work_time(last_day)}")
 
 
 def when_to_leave() -> None:
-    attendance_chart = _get_attendance_chart()
+    attendance_chart = until_today(_get_attendance_chart())
     leave_time, includes_break = time.get_leave_time(attendance_chart)
     current_time = Duration.now()
     if leave_time <= current_time:
         print("Leave today as early as you like.")
         return
 
     break_msg = "(includes a 1-hour break)" if includes_break else "(break time not included)"
@@ -51,15 +53,15 @@
         recoru_auth_id=recoru_auth_id,
         recoru_password=recoru_password
     )
     config.save()
 
 
 def graph(exclude_last_day: bool) -> None:
-    attendance_chart = _get_attendance_chart()
+    attendance_chart = until_today(_get_attendance_chart())
     if exclude_last_day and len(attendance_chart) > 1:
         attendance_chart = attendance_chart[:-1]
     days, history, _ = time.get_overtime_history(attendance_chart)
     plotting.plot_overtime_balance_history(days, history)
 
 
 def main() -> None:
@@ -104,17 +106,12 @@
     with RecoruSession(
         contract_id=config.recoru_contract_id,
         auth_id=config.recoru_auth_id,
         password=config.recoru_password
     ) as recoru_session:
         attendance_chart = recoru_session.get_attendance_chart()
 
-    # Exclude rows which date is in the future
-    current_day_of_month = datetime.now().day
-    return [
-        row for row in attendance_chart
-        if row.day_of_month <= current_day_of_month
-    ]
+    return attendance_chart
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `RecoLul-1.8.0/recolul/config.py` & `RecoLul-1.9.0/recolul/config.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.8.0/recolul/duration.py` & `RecoLul-1.9.0/recolul/duration.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,7 +41,10 @@
         return self.minutes <= other.minutes
 
     def __ge__(self, other):
         return self.minutes >= other.minutes
 
     def __abs__(self):
         return Duration(abs(self.minutes))
+
+    def __bool__(self):
+        return self.minutes > 0
```

### Comparing `RecoLul-1.8.0/recolul/plotting.py` & `RecoLul-1.9.0/recolul/plotting.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.8.0/recolul/recoru/attendance_chart.py` & `RecoLul-1.9.0/recolul/recoru/attendance_chart.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.8.0/recolul/recoru/recoru_session.py` & `RecoLul-1.9.0/recolul/recoru/recoru_session.py`

 * *Files identical despite different names*

### Comparing `RecoLul-1.8.0/recolul/time.py` & `RecoLul-1.9.0/recolul/time.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 from collections import defaultdict
+from datetime import datetime
 
 from recolul.duration import Duration
 from recolul.recoru.attendance_chart import AttendanceChart, ChartRow
 
 _MIN_HOURS_FOR_MANDATORY_BREAK = Duration(6 * 60)
 
 
+def until_today(attendance_chart: AttendanceChart) -> AttendanceChart:
+    """Return a slice of the attendance chart that only contains rows until today"""
+    current_day_of_month = datetime.now().day
+    return [
+        row for row in attendance_chart
+        if row.day_of_month <= current_day_of_month
+    ]
+
+
 def get_work_time(chart_row: ChartRow) -> Duration:
     """
     Get work time from the column if available,
     else calculate it from clock-in time and current time
     """
     if work_time := chart_row.work_time:
         return Duration.parse(work_time)
 
-    clock_in_time = Duration.parse(chart_row.clock_in_time)
+    if not (raw_clock_in_time := chart_row.clock_in_time):
+        return Duration(0)
+    clock_in_time = Duration.parse(raw_clock_in_time)
     current_work_time = Duration.now() - clock_in_time
     break_time = (
         Duration(60) if current_work_time >= _MIN_HOURS_FOR_MANDATORY_BREAK
         else Duration(0)
     )
     return current_work_time - break_time
 
 
 def get_overtime_history(attendance_chart: AttendanceChart) -> tuple[list[str], list[Duration], dict[str, Duration]]:
     days = []
     overtime_history = []
     total_workplace_times = defaultdict(Duration)
     for row in attendance_chart:
-        if not row.clock_in_time:
-            continue
-
-        day = row.day
-        if not day.text:
-            continue
-
-        days.append(day.text)
-        if day.color in ["blue", "red"] and "swap day" not in row.memo.lower():
+        if not _is_working_day(row):
             required_time = Duration(0)
         else:
             required_time = Duration(8 * 60)
         work_time = get_work_time(row)
+        if not (required_time or work_time):
+            continue
         overtime_history.append(work_time - required_time)
         total_workplace_times[row.workplace.text] += work_time
+        days.append(row.day.text)
 
     return days, overtime_history, total_workplace_times
 
 
 def get_overtime_balance(attendance_chart: AttendanceChart) -> tuple[Duration, dict[str, Duration]]:
     _, history, total_workplace_times = get_overtime_history(attendance_chart)
     return sum(history, Duration()), total_workplace_times
@@ -63,7 +70,19 @@
     # add a mandatory 1-hour break time.
     required_today = day_base_hours - overtime_balance
     if required_today > _MIN_HOURS_FOR_MANDATORY_BREAK:
         leave_time += Duration(60)
         return leave_time, True
 
     return leave_time, False
+
+
+def count_working_days(attendance_chart: AttendanceChart) -> int:
+    return sum(
+        1
+        for row in attendance_chart
+        if _is_working_day(row)
+    )
+
+
+def _is_working_day(row: ChartRow) -> bool:
+    return row.day.color not in ["blue", "red"] or "swap day" in row.memo.lower()
```

### Comparing `RecoLul-1.8.0/setup.cfg` & `RecoLul-1.9.0/setup.cfg`

 * *Files identical despite different names*

