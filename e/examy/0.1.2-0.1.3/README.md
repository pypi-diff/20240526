# Comparing `tmp/examy-0.1.2.tar.gz` & `tmp/examy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examy-0.1.2.tar", max compression
+gzip compressed data, was "examy-0.1.3.tar", max compression
```

## Comparing `examy-0.1.2.tar` & `examy-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    18092 2024-05-25 16:01:42.024616 examy-0.1.2/LICENSE
--rw-r--r--   0        0        0        8 2024-05-25 16:01:42.024616 examy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-25 16:01:42.024616 examy-0.1.2/examy/__init__.py
--rw-r--r--   0        0        0     1050 2024-05-25 16:01:42.024616 examy-0.1.2/examy/fetchers/new_web_layout/optimized.py
--rw-r--r--   0        0        0     1573 2024-05-25 16:01:42.024616 examy-0.1.2/examy/fetchers/new_web_layout/utils/process_html.py
--rw-r--r--   0        0        0     4000 2024-05-25 16:01:42.024616 examy-0.1.2/examy/fetchers/new_web_layout/utils/webpage_actions.py
--rw-r--r--   0        0        0      253 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/ExamDescriptor.py
--rw-r--r--   0        0        0     1884 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/ExamReport.py
--rw-r--r--   0        0        0      716 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/Ranking.py
--rw-r--r--   0        0        0     1604 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/Student.py
--rw-r--r--   0        0        0      127 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/Test.py
--rw-r--r--   0        0        0      535 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/TestResult.py
--rw-r--r--   0        0        0      191 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/exceptions.py
--rw-r--r--   0        0        0     1459 2024-05-25 16:01:42.024616 examy-0.1.2/examy/models/fetcher.py
--rw-r--r--   0        0        0      635 2024-05-25 16:01:42.024616 examy-0.1.2/examy/utils/__init__.py
--rw-r--r--   0        0        0     4759 2024-05-25 16:01:42.024616 examy-0.1.2/examy/utils/export.py
--rw-r--r--   0        0        0     4183 2024-05-25 16:01:42.024616 examy-0.1.2/examy/utils/manager.py
--rw-r--r--   0        0        0     1152 2024-05-25 16:01:42.024616 examy-0.1.2/examy/utils/stgroup.py
--rw-r--r--   0        0        0      552 2024-05-25 16:01:42.024616 examy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 examy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-05-26 10:23:05.693760 examy-0.1.3/LICENSE
+-rw-r--r--   0        0        0        8 2024-05-26 10:23:05.693760 examy-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 10:23:05.693760 examy-0.1.3/examy/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-26 10:23:05.697761 examy-0.1.3/examy/fetchers/new_web_layout/optimized.py
+-rw-r--r--   0        0        0     1573 2024-05-26 10:23:05.697761 examy-0.1.3/examy/fetchers/new_web_layout/utils/process_html.py
+-rw-r--r--   0        0        0     4000 2024-05-26 10:23:05.697761 examy-0.1.3/examy/fetchers/new_web_layout/utils/webpage_actions.py
+-rw-r--r--   0        0        0      253 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/ExamDescriptor.py
+-rw-r--r--   0        0        0     1884 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/ExamReport.py
+-rw-r--r--   0        0        0      716 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/Ranking.py
+-rw-r--r--   0        0        0     1604 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/Student.py
+-rw-r--r--   0        0        0      127 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/Test.py
+-rw-r--r--   0        0        0      535 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/TestResult.py
+-rw-r--r--   0        0        0      191 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/exceptions.py
+-rw-r--r--   0        0        0     2095 2024-05-26 10:23:05.697761 examy-0.1.3/examy/models/fetcher.py
+-rw-r--r--   0        0        0      635 2024-05-26 10:23:05.697761 examy-0.1.3/examy/utils/__init__.py
+-rw-r--r--   0        0        0     4872 2024-05-26 10:23:05.697761 examy-0.1.3/examy/utils/export.py
+-rw-r--r--   0        0        0     4234 2024-05-26 10:23:05.697761 examy-0.1.3/examy/utils/manager.py
+-rw-r--r--   0        0        0     1152 2024-05-26 10:23:05.697761 examy-0.1.3/examy/utils/stgroup.py
+-rw-r--r--   0        0        0      552 2024-05-26 10:23:05.697761 examy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 examy-0.1.3/PKG-INFO
```

### Comparing `examy-0.1.2/LICENSE` & `examy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/fetchers/new_web_layout/optimized.py` & `examy-0.1.3/examy/fetchers/new_web_layout/optimized.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class OptimizedNewTypeFetcher(SeleniumCompatibleFetcher):
     result_page_layout = "new"
     fetcher_codename = "optimized"
 
     @SeleniumCompatibleFetcher.requires_driver
+    @SeleniumCompatibleFetcher.check_fetch_arguments
     def fetch(self, student, exam_descriptor, *args, **kwargs):
         from examy.fetchers.new_web_layout.utils.webpage_actions import (
             login,
             get_result_page_address,
             logout,
         )
         from examy.fetchers.new_web_layout.utils.process_html import process_result_html
```

### Comparing `examy-0.1.2/examy/fetchers/new_web_layout/utils/process_html.py` & `examy-0.1.3/examy/fetchers/new_web_layout/utils/process_html.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/fetchers/new_web_layout/utils/webpage_actions.py` & `examy-0.1.3/examy/fetchers/new_web_layout/utils/webpage_actions.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/models/ExamReport.py` & `examy-0.1.3/examy/models/ExamReport.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/models/Ranking.py` & `examy-0.1.3/examy/models/Ranking.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/models/Student.py` & `examy-0.1.3/examy/models/Student.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/models/TestResult.py` & `examy-0.1.3/examy/models/TestResult.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/models/fetcher.py` & `examy-0.1.3/examy/models/fetcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,28 @@
 
 class ExamFetcher(ABC):
     """Base class for fetchers"""
 
     result_page_layout: str
     fetcher_codename: str
 
+    @staticmethod
+    def check_fetch_arguments(func):
+        @wraps(func)
+        def wrapper(self: "ExamFetcher", student: Student, exam_descriptor: ExamDescriptor, *args, **kwargs):
+            if exam_descriptor.result_page_layout != self.result_page_layout:
+                raise ValueError(
+                    f"Expected result page layout '{self.result_page_layout}', "
+                    f"got '{exam_descriptor.result_page_layout}' instead."
+                )
+            return func(self, student, exam_descriptor, *args, **kwargs)
+
+        return wrapper
+
+    @check_fetch_arguments
     @abstractmethod
     def fetch(self, student: Student, exam_descriptor: ExamDescriptor, *args, **kwargs) -> ExamReport:
         pass
 
 
 class SeleniumCompatibleFetcher(ExamFetcher, ABC):
     _driver: WebDriver
@@ -43,10 +57,11 @@
                     "Attempted to execute an action with selenium without configuring any driver for " "the process"
                 )
             return func(self, *args, **kwargs)
 
         return wrapper
 
     @requires_driver
+    @ExamFetcher.check_fetch_arguments
     @abstractmethod
     def fetch(self, student, exam_descriptor, *args, **kwargs):
         pass
```

### Comparing `examy-0.1.2/examy/utils/__init__.py` & `examy-0.1.3/examy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/examy/utils/export.py` & `examy-0.1.3/examy/utils/export.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,121 @@
-from collections import OrderedDict
 from typing import Iterator
 
 from examy.models.ExamDescriptor import ExamDescriptor
 from examy.models.ExamReport import ExamReport
 from examy.models.Student import Student
 
 
 class ResultExporter(object):
-    export_dict_student: OrderedDict = {
+    export_dict_student = {
         "name": ["Student", "name"],
         "number": ["Student", "number"],
         "class": ["Student", "class_"],
         "class_rank": ["Ranking", "class_rank"],
         "school_rank": ["Ranking", "school_rank"],
         "district_rank": ["Ranking", "district_rank"],
         "province_rank": ["Ranking", "province_rank"],
         "global_rank": ["Ranking", "global_rank"],
         "score": ["Report", "score"],
         "true_count": ["Report", "true_count"],
         "false_count": ["Report", "false_count"],
         "empty_count": ["Report", "empty_count"],
         "net": ["Report", "net"],
-        "{short_test_name}_true": ["TestResult", "true_count"],
-        "{short_test_name}_false": ["TestResult", "false_count"],
-        "{short_test_name}_empty": ["TestResult", "empty_count"],
-        "{short_test_name}_net": ["TestResult", "net"],
+        "group1": [
+            "group",
+            {
+                "{short_test_name}_true": ["TestResult", "true_count"],
+                "{short_test_name}_false": ["TestResult", "false_count"],
+                "{short_test_name}_empty": ["TestResult", "empty_count"],
+                "{short_test_name}_net": ["TestResult", "net"],
+            },
+        ],
     }
 
-    export_dict_common: OrderedDict = {
+    export_dict_common = {
         "school_attendance": ["Ranking", "school_attendance"],
         "district_attendance": ["Ranking", "district_attendance"],
         "province_attendance": ["Ranking", "province_attendance"],
         "global_attendance": ["Ranking", "global_attendance"],
         "question_count": ["Report", "question_count"],
-        "{short_test_name}_question_count": ["Test", "question_count"],
+        "group1": [
+            "group",
+            {
+                "{short_test_name}_question_count": ["Test", "question_count"],
+            },
+        ],
     }
 
     def __init__(self):
         self.student_export = []
         self.student_export_headers = []
         self.common_export = []
         self.common_export_headers = []
 
     def clear(self):
         self.student_export = []
         self.common_export = []
 
     @staticmethod
-    def _make_export(st: Student, desc: ExamDescriptor, report: ExamReport, export_scheme: OrderedDict) -> list:
+    def _make_export(st: Student, desc: ExamDescriptor, report: ExamReport, export_scheme: dict) -> list:
         export = []
 
         for k, v in export_scheme.items():
             obj, attrib = v
             match obj:
-                case "Test" | "TestResult":
+                case "group":
                     for td, tr in report.iter_tests():
-                        if obj == "Test":
-                            export.append(td.__getattribute__(attrib))
-                        else:
-                            export.append(tr.__getattribute__(attrib))
-                case other:
-                    match other:
-                        case "Student":
-                            export.append(st.__getattribute__(attrib))
-                        case "Report":
-                            export.append(report.__getattribute__(attrib))
-                        case "Ranking":
-                            export.append(report.ranks.__getattribute__(attrib))
+                        for k2, (obj2, attrib2) in attrib.items():
+                            if obj2 == "Test":
+                                export.append(td.__getattribute__(attrib2))
+                            else:
+                                export.append(tr.__getattribute__(attrib2))
+                case "Student":
+                    export.append(st.__getattribute__(attrib))
+                case "Report":
+                    export.append(report.__getattribute__(attrib))
+                case "Ranking":
+                    export.append(report.ranks.__getattribute__(attrib))
         return export
 
     @staticmethod
-    def _make_headers(st: Student, desc: ExamDescriptor, report: ExamReport, export_scheme: OrderedDict) -> list:
+    def _make_headers(st: Student, desc: ExamDescriptor, report: ExamReport, export_scheme: dict) -> list:
         headers = []
         for k, v in export_scheme.items():
             obj, attrib = v
             match obj:
-                case "Test" | "TestResult":
+                case "group":
                     for td, tr in report.iter_tests():
-                        headers.append(k.format(short_test_name = td.short_name))
+                        for k2, _ in attrib.items():
+                            headers.append(k2.format(short_test_name=td.short_name))
                 case _:
                     headers.append(k)
         return headers
 
     def create_export_from_students(self, st_gen: Iterator[Student], desc: ExamDescriptor):
         commons_set = False
         for st in st_gen:
             report = st.get_report(desc.exam_name, soft_return=True)
             if report is None:
                 continue
-            self.student_export.append(
-                self._make_export(st,desc,report,self.export_dict_student)
-            )
+            self.student_export.append(self._make_export(st, desc, report, self.export_dict_student))
             if not commons_set:
                 commons_set = True
-                self.student_export_headers = self._make_headers(st,desc,report,self.export_dict_student)
+                self.student_export_headers = self._make_headers(st, desc, report, self.export_dict_student)
 
-                self.common_export_headers = self._make_headers(st,desc,report,self.export_dict_common)
-                self.common_export = self._make_export(st,desc,report, self.export_dict_common)
+                self.common_export_headers = self._make_headers(st, desc, report, self.export_dict_common)
+                self.common_export = self._make_export(st, desc, report, self.export_dict_common)
 
     def sort(self, by: str, reverse: bool = False):
         index = self.student_export_headers.index(by)
         self.student_export.sort(key=lambda x: x[index], reverse=reverse)
 
     def to_csv(self, student_path: str, common_path: str):
         import csv
+
         with open(student_path, "w", newline="") as f:
             writer = csv.writer(f)
             writer.writerow(self.student_export_headers)
             writer.writerows(self.student_export)
         with open(common_path, "w", newline="") as f:
             writer = csv.writer(f)
             writer.writerow(self.common_export_headers)
```

### Comparing `examy-0.1.2/examy/utils/manager.py` & `examy-0.1.3/examy/utils/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from examy.utils.stgroup import StudentGroup
 
 logger = logging.getLogger(__name__)
 
 
 class Manager(object):
     def __init__(self, webdriver_generator: Callable[[], WebDriver] | None = None):
-        self.errored_students: dict[str,list[Student]] = {}
+        self.errored_students: dict[str, list[Student]] = {}
         self.errored_students_lock = threading.Lock()
         self._groups: list[StudentGroup] = []
         self.webdriver_generator = webdriver_generator
 
         self._drivers: dict = {}
         self._exam_descriptor: ExamDescriptor | None = None
         self._fetcher_type: type[ExamFetcher] | None = None
@@ -60,15 +60,18 @@
             fetcher.driver = self._drivers[threading.current_thread().name]
 
         err_list = self.errored_students[self._exam_descriptor.exam_name]
 
         try:
             fetcher.fetch(st, self._exam_descriptor)
             res = st.reports[-1]
-            logger.info(f"Get: {st.name}: ok; score={res.score}, net={res.net}, class_rank={res.ranks.class_rank}, school_rank={res.ranks.school_rank}")
+            logger.info(
+                f"Get: {st.name}: ok; score={res.score}, net={res.net}, "
+                f"class_rank={res.ranks.class_rank}, school_rank={res.ranks.school_rank}"
+            )
             with self.errored_students_lock:
                 if st in err_list:
                     err_list.remove(st)
         except StudentDidNotTakeExam:
             logger.info(f"{st.name} did not take the exam named '{self._exam_descriptor.exam_name}'")
         except:
             with self.errored_students_lock:
```

### Comparing `examy-0.1.2/examy/utils/stgroup.py` & `examy-0.1.3/examy/utils/stgroup.py`

 * *Files identical despite different names*

### Comparing `examy-0.1.2/pyproject.toml` & `examy-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "examy"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Eren Akgün <iobthedev@outlook.com>"]
 readme = "README.md"
 license = "GPL-2.0-only"
 repository = "https://github.com/insanolanbiri/examy"
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `examy-0.1.2/PKG-INFO` & `examy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: examy
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/insanolanbiri/examy
 License: GPL-2.0-only
 Author: Eren Akgün
 Author-email: iobthedev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

