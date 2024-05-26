# Comparing `tmp/recodex-cli-0.0.8.tar.gz` & `tmp/recodex-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\recodex-cli-0.0.8.tar", last modified: Fri Aug  3 16:01:42 2018, max compression
+gzip compressed data, was "dist\recodex-cli-0.0.9.tar", last modified: Sat Sep  7 21:13:51 2019, max compression
```

## Comparing `recodex-cli-0.0.8.tar` & `recodex-cli-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/
--rw-rw-rw-   0        0        0      709 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/
--rw-rw-rw-   0        0        0     7277 2018-07-30 15:01:42.000000 recodex-cli-0.0.8/recodex/api.py
--rw-rw-rw-   0        0        0     2822 2018-04-15 18:25:31.000000 recodex-cli-0.0.8/recodex/cli.py
--rw-rw-rw-   0        0        0     1670 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/config.py
--rw-rw-rw-   0        0        0      919 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/decorators.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/assignments/
--rw-rw-rw-   0        0        0     2358 2018-04-26 22:39:28.000000 recodex-cli-0.0.8/recodex/plugins/assignments/cli.py
--rw-rw-rw-   0        0        0        0 2018-04-26 22:39:28.000000 recodex-cli-0.0.8/recodex/plugins/assignments/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/caslogin/
--rw-rw-rw-   0        0        0     1515 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/caslogin/cli.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/caslogin/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/codex/
--rw-rw-rw-   0        0        0     8611 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/codex/cli.py
--rw-rw-rw-   0        0        0     8410 2018-04-26 22:39:28.000000 recodex-cli-0.0.8/recodex/plugins/codex/codex_config.py
--rw-rw-rw-   0        0        0      728 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/codex/plugin_config.py
--rw-rw-rw-   0        0        0     9361 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/codex/utils.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/codex/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/exercises/
--rw-rw-rw-   0        0        0     3446 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/exercises/cli.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/exercises/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/login/
--rw-rw-rw-   0        0        0      609 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/login/cli.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/login/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/takeover/
--rw-rw-rw-   0        0        0      472 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/takeover/cli.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/takeover/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex/plugins/users/
--rw-rw-rw-   0        0        0     3752 2018-07-30 15:01:42.000000 recodex-cli-0.0.8/recodex/plugins/users/cli.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/users/__init__.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/plugins/__init__.py
--rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.8/recodex/__init__.py
-drwxrwxrwx   0        0        0        0 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/
--rw-rw-rw-   0        0        0        1 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      366 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      709 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       60 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0      919 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2018-08-03 16:01:41.000000 recodex-cli-0.0.8/recodex_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2018-08-03 16:01:42.000000 recodex-cli-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1528 2018-08-03 16:01:29.000000 recodex-cli-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/
+-rw-rw-rw-   0        0        0      709 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/
+-rw-rw-rw-   0        0        0     8458 2019-09-05 22:33:40.000000 recodex-cli-0.0.9/recodex/api.py
+-rw-rw-rw-   0        0        0     2822 2018-04-15 18:25:31.000000 recodex-cli-0.0.9/recodex/cli.py
+-rw-rw-rw-   0        0        0     1670 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/config.py
+-rw-rw-rw-   0        0        0      919 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/decorators.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/assignments/
+-rw-rw-rw-   0        0        0     2930 2019-09-05 21:20:05.000000 recodex-cli-0.0.9/recodex/plugins/assignments/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-26 22:39:28.000000 recodex-cli-0.0.9/recodex/plugins/assignments/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/caslogin/
+-rw-rw-rw-   0        0        0     1515 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/caslogin/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/caslogin/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/codex/
+-rw-rw-rw-   0        0        0     8611 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/codex/cli.py
+-rw-rw-rw-   0        0        0     8410 2018-04-26 22:39:28.000000 recodex-cli-0.0.9/recodex/plugins/codex/codex_config.py
+-rw-rw-rw-   0        0        0      728 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/codex/plugin_config.py
+-rw-rw-rw-   0        0        0     9361 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/codex/utils.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/codex/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/exercises/
+-rw-rw-rw-   0        0        0     7654 2018-11-24 10:16:25.000000 recodex-cli-0.0.9/recodex/plugins/exercises/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/exercises/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/groups/
+-rw-rw-rw-   0        0        0     1172 2019-09-05 22:01:44.000000 recodex-cli-0.0.9/recodex/plugins/groups/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/groups/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/login/
+-rw-rw-rw-   0        0        0      609 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/login/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/login/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/takeover/
+-rw-rw-rw-   0        0        0      472 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/takeover/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/takeover/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex/plugins/users/
+-rw-rw-rw-   0        0        0     4346 2019-09-05 22:34:44.000000 recodex-cli-0.0.9/recodex/plugins/users/cli.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/users/__init__.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/plugins/__init__.py
+-rw-rw-rw-   0        0        0        0 2018-04-13 10:57:02.000000 recodex-cli-0.0.9/recodex/__init__.py
+drwxrwxrwx   0        0        0        0 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      406 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      709 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      984 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/recodex_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2019-09-07 21:13:51.000000 recodex-cli-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2019-09-07 21:13:18.000000 recodex-cli-0.0.9/setup.py
```

### Comparing `recodex-cli-0.0.8/PKG-INFO` & `recodex-cli-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: recodex-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: ReCodEx CLI
 Home-page: https://github.com/ReCodEx/cli
 Author: ReCodEx team
 Author-email: UNKNOWN
 License: MIT
 Description: A command line frontend to the ReCodEx programmer evaluation system
 Keywords: recodex
```

### Comparing `recodex-cli-0.0.8/recodex/api.py` & `recodex-cli-0.0.9/recodex/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
     def get_pipelines(self):
         return self.get("/pipelines")
 
     def get_exercise(self, exercise_id):
         return self.get("/exercises/{}".format(exercise_id))
 
-    def get_exercises(self):
-        return self.get("/exercises")
+    def get_exercises(self, offset=0, limit=0):
+        return self.get("/exercises?offset={}&limit={}".format(offset, limit))["items"]
 
     def get_reference_solutions(self, exercise_id):
         return self.get("/reference-solutions/exercise/{}".format(exercise_id))
 
     def get_reference_solution_evaluations(self, solution_id):
         return self.get("/reference-solutions/{}/evaluations".format(solution_id))
 
@@ -90,22 +90,28 @@
 
     def update_exercise(self, exercise_id, details):
         self.post('/exercises/{}'.format(exercise_id), data=details)
 
     def delete_exercise(self, exercise_id):
         self.delete('/exercises/{}'.format(exercise_id))
 
+    def delete_reference_solution_evaluation(self, evaluation_id):
+        self.delete('/reference-solutions/evaluation/{}'.format(evaluation_id))
+
     def create_reference_solution(self, exercise_id, data):
         return self.post('/reference-solutions/exercise/{}/submit'.format(exercise_id), data=data)
 
     def update_environment_configs(self, exercise_id, configs):
         self.post("/exercises/{}/environment-configs".format(exercise_id), data={
             "environmentConfigs": configs
         })
 
+    def get_exercise_config(self, exercise_id):
+        return self.get("/exercises/{}/config".format(exercise_id))
+
     def update_exercise_config(self, exercise_id, config):
         self.post("/exercises/{}/config".format(exercise_id), data={"config": config})
 
     def set_exercise_tests(self, exercise_id, tests):
         self.post("/exercises/{}/tests".format(exercise_id), data={"tests": tests})
 
     def get_exercise_tests(self, exercise_id):
@@ -114,14 +120,17 @@
     def update_limits(self, exercise_id, environment_id, hwgroup_id, limits):
         self.post("/exercises/{}/environment/{}/hwgroup/{}/limits".format(exercise_id, environment_id, hwgroup_id),
                   data={"limits": limits})
 
     def evaluate_reference_solutions(self, exercise_id):
         self.post("/reference-solutions/exercise/{}/evaluate".format(exercise_id), data={})
 
+    def resubmit_reference_solution(self, ref_solution_id, debug=False):
+        return self.post("/reference-solutions/{}/resubmit".format(ref_solution_id), data={"debug": debug})
+
     def get_hwgroups(self):
         return self.get("/hardware-groups")
 
     # Authentication
 
     def login(self, username, password):
         return self.post("/login", data={
@@ -155,19 +164,34 @@
             'firstName': first_name,
             'lastName': last_name,
             'password': password,
             'passwordConfirm': password,
             'instanceId': instance_id
         })
 
+    def delete_user(self, user_id):
+        return self.delete("/users/{}".format(user_id))
+
+    def set_allow_user(self, user_id, allow):
+        return self.post("/users/{}/allowed".format(user_id), data={"isAllowed": allow})
+
     # Groups
 
     def group_add_student(self, group_id, user_id):
         return self.post("/groups/{}/students/{}".format(group_id, user_id))
 
+    def group_remove_student(self, group_id, user_id):
+        return self.delete("/groups/{}/students/{}".format(group_id, user_id))
+
+    def group_attach_exercise(self, group_id, exercise_id):
+        return self.post("/exercises/{}/groups/{}".format(exercise_id, group_id))
+
+    def group_detach_exercise(self, group_id, exercise_id):
+        return self.delete("/exercises/{}/groups/{}".format(exercise_id, group_id))
+
     # Assignments
 
     def get_assignment(self, assignment_id):
         return self.get("/exercise-assignments/{}".format(assignment_id))
 
     def get_assignment_best_solutions(self, assignment_id):
         return self.get("/exercise-assignments/{}/best-solutions".format(assignment_id))
@@ -189,10 +213,10 @@
             json = response.json()
         except JSONDecodeError:
             logging.error("Loading JSON response failed, see full response below:")
             logging.error(response.text)
             raise RuntimeError("Loading JSON response failed")
 
         if not json["success"]:
-            raise RuntimeError("Received error from API: " + json["msg"])
+            raise RuntimeError("Received error from API: " + json["error"]["message"])
 
         return json["payload"]
```

### Comparing `recodex-cli-0.0.8/recodex/cli.py` & `recodex-cli-0.0.9/recodex/cli.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/config.py` & `recodex-cli-0.0.9/recodex/config.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/decorators.py` & `recodex-cli-0.0.9/recodex/decorators.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/plugins/assignments/cli.py` & `recodex-cli-0.0.9/recodex/plugins/assignments/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,28 @@
         return -1
     evaluation = submission["evaluation"]
     if evaluation is None:
         return -1
     return evaluation["points"] + solution["bonusPoints"]
 
 
+def getAssignmentName(assignment):
+    if "localizedTexts" not in assignment or len(assignment["localizedTexts"]) == 0:
+        # There is no "localizedTexts" key or empty array :(
+        return "unknown"
+    known_languages = ("en", "cs")
+    # Try known languages (in given order)
+    for lang in known_languages:
+        for item in assignment["localizedTexts"]:
+            if item["locale"] == lang:
+                return item["name"]
+    # Something weird happened, return first name we got
+    return assignment["localizedTexts"][0]["name"]
+
+
 @click.group()
 def cli():
     """
     Tools for working with assignments (exercise instances)
     """
 
 
@@ -44,15 +58,16 @@
         return
 
     # Get assignment metadata and best solution for each student ...
     assignment = api.get_assignment(assignment_id)
     if assignment is None:
         click.echo("Assignment not found.")
         return
-    click.echo("Downloading best solutions of '{}' to '{}' ...".format(assignment["name"], download_dir))
+    click.echo("Downloading best solutions of '{}' to '{}' ...".format(
+        getAssignmentName(assignment), download_dir))
     best_solutions = api.get_assignment_best_solutions(assignment_id)
 
     # Iterate over students
     for student in api.get_group_students(assignment["groupId"]):
         # Try to find best solution for the student
         best = best_solutions[student["id"]]
         if best:
```

### Comparing `recodex-cli-0.0.8/recodex/plugins/caslogin/cli.py` & `recodex-cli-0.0.9/recodex/plugins/caslogin/cli.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/plugins/codex/cli.py` & `recodex-cli-0.0.9/recodex/plugins/codex/cli.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/plugins/codex/codex_config.py` & `recodex-cli-0.0.9/recodex/plugins/codex/codex_config.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/plugins/codex/plugin_config.py` & `recodex-cli-0.0.9/recodex/plugins/codex/plugin_config.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/plugins/codex/utils.py` & `recodex-cli-0.0.9/recodex/plugins/codex/utils.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex/plugins/login/cli.py` & `recodex-cli-0.0.9/recodex/plugins/login/cli.py`

 * *Files identical despite different names*

### Comparing `recodex-cli-0.0.8/recodex_cli.egg-info/PKG-INFO` & `recodex-cli-0.0.9/recodex_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: recodex-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: ReCodEx CLI
 Home-page: https://github.com/ReCodEx/cli
 Author: ReCodEx team
 Author-email: UNKNOWN
 License: MIT
 Description: A command line frontend to the ReCodEx programmer evaluation system
 Keywords: recodex
```

### Comparing `recodex-cli-0.0.8/recodex_cli.egg-info/SOURCES.txt` & `recodex-cli-0.0.9/recodex_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 recodex/plugins/codex/__init__.py
 recodex/plugins/codex/cli.py
 recodex/plugins/codex/codex_config.py
 recodex/plugins/codex/plugin_config.py
 recodex/plugins/codex/utils.py
 recodex/plugins/exercises/__init__.py
 recodex/plugins/exercises/cli.py
+recodex/plugins/groups/__init__.py
+recodex/plugins/groups/cli.py
 recodex/plugins/login/__init__.py
 recodex/plugins/login/cli.py
 recodex/plugins/takeover/__init__.py
 recodex/plugins/takeover/cli.py
 recodex/plugins/users/__init__.py
 recodex/plugins/users/cli.py
 recodex_cli.egg-info/PKG-INFO
```

### Comparing `recodex-cli-0.0.8/setup.py` & `recodex-cli-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='recodex-cli',
-      version='0.0.8',
+      version='0.0.9',
       description='ReCodEx CLI',
       long_description='A command line frontend to the ReCodEx programmer evaluation system',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Intended Audience :: Education',
@@ -25,14 +25,15 @@
       entry_points={
           'console_scripts':
               ['recodex = recodex.cli:cli'],
           'recodex': [
               'assignments = recodex.plugins.assignments.cli:cli',
               'codex = recodex.plugins.codex.cli:cli',
               'exercises = recodex.plugins.exercises.cli:cli',
+              'groups = recodex.plugins.groups.cli:cli',
               'caslogin = recodex.plugins.caslogin.cli:caslogin',
               'login = recodex.plugins.login.cli:login',
               'takeover = recodex.plugins.takeover.cli:takeover',
               'users = recodex.plugins.users.cli:cli'
           ]
       }
 )
```

