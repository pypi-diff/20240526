# Comparing `tmp/alita_tools-0.0.8.tar.gz` & `tmp/alita_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_tools-0.0.8.tar", last modified: Fri Apr 12 16:14:02 2024, max compression
+gzip compressed data, was "alita_tools-0.0.9.tar", last modified: Wed Apr 24 11:04:34 2024, max compression
```

## Comparing `alita_tools-0.0.8.tar` & `alita_tools-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.060000 alita_tools-0.0.8/
--rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.8/LICENSE
--rwx------   0 arozumenko   (501) staff       (20)     1007 2024-04-12 16:14:02.290000 alita_tools-0.0.8/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.8/README.md
--rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-12 16:13:53.000000 alita_tools-0.0.8/pyproject.toml
--rwx------   0 arozumenko   (501) staff       (20)      162 2024-04-12 11:51:15.000000 alita_tools-0.0.8/requirements.txt
--rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-12 16:14:02.290000 alita_tools-0.0.8/setup.cfg
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.080000 alita_tools-0.0.8/src/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.8/src/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.100000 alita_tools-0.0.8/src/alita_tools/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.8/src/alita_tools/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.150000 alita_tools-0.0.8/src/alita_tools/base/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.8/src/alita_tools/base/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.8/src/alita_tools/base/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.170000 alita_tools-0.0.8/src/alita_tools/confluence/
--rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.8/src/alita_tools/confluence/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.8/src/alita_tools/confluence/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.190000 alita_tools-0.0.8/src/alita_tools/github/
--rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.8/src/alita_tools/github/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    15406 2024-04-04 06:35:17.000000 alita_tools-0.0.8/src/alita_tools/github/api_wrapper.py
--rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.8/src/alita_tools/github/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.220000 alita_tools-0.0.8/src/alita_tools/jira/
--rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.8/src/alita_tools/jira/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    11532 2024-04-09 08:08:34.000000 alita_tools-0.0.8/src/alita_tools/jira/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.240000 alita_tools-0.0.8/src/alita_tools/openapi/
--rwx------   0 arozumenko   (501) staff       (20)     1747 2024-04-12 14:21:33.000000 alita_tools-0.0.8/src/alita_tools/openapi/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-12 16:14:02.130000 alita_tools-0.0.8/src/alita_tools.egg-info/
--rwx------   0 arozumenko   (501) staff       (20)     1007 2024-04-12 16:14:02.000000 alita_tools-0.0.8/src/alita_tools.egg-info/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      639 2024-04-12 16:14:02.000000 alita_tools-0.0.8/src/alita_tools.egg-info/SOURCES.txt
--rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-12 16:14:02.000000 alita_tools-0.0.8/src/alita_tools.egg-info/dependency_links.txt
--rwx------   0 arozumenko   (501) staff       (20)      163 2024-04-12 16:14:02.000000 alita_tools-0.0.8/src/alita_tools.egg-info/requires.txt
--rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-12 16:14:02.000000 alita_tools-0.0.8/src/alita_tools.egg-info/top_level.txt
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.420000 alita_tools-0.0.9/
+-rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.9/LICENSE
+-rwx------   0 arozumenko   (501) staff       (20)     1007 2024-04-24 11:04:34.670000 alita_tools-0.0.9/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.9/README.md
+-rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-24 11:04:19.000000 alita_tools-0.0.9/pyproject.toml
+-rwx------   0 arozumenko   (501) staff       (20)      162 2024-04-12 11:51:15.000000 alita_tools-0.0.9/requirements.txt
+-rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-24 11:04:34.670000 alita_tools-0.0.9/setup.cfg
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.440000 alita_tools-0.0.9/src/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.9/src/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.460000 alita_tools-0.0.9/src/alita_tools/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.9/src/alita_tools/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.510000 alita_tools-0.0.9/src/alita_tools/base/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.9/src/alita_tools/base/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.9/src/alita_tools/base/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.530000 alita_tools-0.0.9/src/alita_tools/confluence/
+-rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.9/src/alita_tools/confluence/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.9/src/alita_tools/confluence/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.550000 alita_tools-0.0.9/src/alita_tools/github/
+-rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.9/src/alita_tools/github/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    15406 2024-04-04 06:35:17.000000 alita_tools-0.0.9/src/alita_tools/github/api_wrapper.py
+-rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.9/src/alita_tools/github/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.580000 alita_tools-0.0.9/src/alita_tools/jira/
+-rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.9/src/alita_tools/jira/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    11546 2024-04-23 08:44:35.000000 alita_tools-0.0.9/src/alita_tools/jira/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.600000 alita_tools-0.0.9/src/alita_tools/openapi/
+-rwx------   0 arozumenko   (501) staff       (20)     1747 2024-04-12 14:21:33.000000 alita_tools-0.0.9/src/alita_tools/openapi/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-24 11:04:34.490000 alita_tools-0.0.9/src/alita_tools.egg-info/
+-rwx------   0 arozumenko   (501) staff       (20)     1007 2024-04-24 11:04:34.000000 alita_tools-0.0.9/src/alita_tools.egg-info/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      639 2024-04-24 11:04:34.000000 alita_tools-0.0.9/src/alita_tools.egg-info/SOURCES.txt
+-rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-24 11:04:34.000000 alita_tools-0.0.9/src/alita_tools.egg-info/dependency_links.txt
+-rwx------   0 arozumenko   (501) staff       (20)      163 2024-04-24 11:04:34.000000 alita_tools-0.0.9/src/alita_tools.egg-info/requires.txt
+-rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-24 11:04:34.000000 alita_tools-0.0.9/src/alita_tools.egg-info/top_level.txt
```

### Comparing `alita_tools-0.0.8/LICENSE` & `alita_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/PKG-INFO` & `alita_tools-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_tools-0.0.8/pyproject.toml` & `alita_tools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_tools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Artem Rozumenko", email="support@projectalita.ai" },
   { name="Vadym Vlasenko", email="vadym_vlasenko@epam.com"}
 ]
 description = "Default set of tools and toolkits available within ProjectAlita and CodeMie applications."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `alita_tools-0.0.8/src/alita_tools/base/tool.py` & `alita_tools-0.0.9/src/alita_tools/base/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/confluence/__init__.py` & `alita_tools-0.0.9/src/alita_tools/confluence/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/confluence/api_wrapper.py` & `alita_tools-0.0.9/src/alita_tools/confluence/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/github/__init__.py` & `alita_tools-0.0.9/src/alita_tools/github/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/github/api_wrapper.py` & `alita_tools-0.0.9/src/alita_tools/github/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/github/tool.py` & `alita_tools-0.0.9/src/alita_tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/jira/__init__.py` & `alita_tools-0.0.9/src/alita_tools/jira/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools/jira/api_wrapper.py` & `alita_tools-0.0.9/src/alita_tools/jira/api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 logger = logging.getLogger(__name__)
 
 
 class JiraSearch(BaseModel):
     jql: str = Field(..., description="Jira Query Language (JQL) query string")
     
 class JiraCreateIssue(BaseModel):
-    issue_json: dict = Field(..., description="""JSON of body to create an issue for JIRA. You must follow the atlassian-python-api's Jira `issue_create` function's input format.
+    issue_json: str = Field(..., description="""JSON of body to create an issue for JIRA. You must follow the atlassian-python-api's Jira `issue_create` function's input format.
 For example, to create a low priority task called "test issue" with description "test description", you would pass in the following STRING dictionary:
-{"fields: {"project": {"key": "project_key"}, "summary": "test issue", "description": "test description", "issuetype": {"name": "Task"}, "priority": {"name": "Major"}}}}
+{"fields": {"project": {"key": "project_key"}, "summary": "test issue", "description": "test description", "issuetype": {"name": "Task"}, "priority": {"name": "Major"}}}
 """)
     
 class JiraUpdateIssue(BaseModel):
     issue_json: str = Field(
         description="""You must follow the atlassian-python-api's Jira `update_issue` function's input format. 
 For example, to update a task with key XXX-123 with new summary, description and custom field, you would pass in the following STRING dictionary: 
 {"key": "issue key", "fields": {"summary": "updated issue", "description": "updated description", "customfield_xxx": "updated custom field"}}
@@ -130,40 +130,41 @@
 
     
     def create_issue_validate(self, params: Dict[str, Any]):
         if params.get("fields") is None:
             raise ToolException("""
             Jira fields are provided in a wrong way.
             For example, to create a low priority task called "test issue" with description "test description", you would pass in the following STRING dictionary:
-            {{"fields: {{{{"project": {{"key": "project_key"}}, "summary": "test issue", "description": "test description", "issuetype": {{"name": "Task"}}, "priority": {{"name": "Major"}}}}}}
+            {"fields": {"project": {"key": "project_key"}, "summary": "test issue", "description": "test description", "issuetype": {"name": "Task"}, "priority": {"name": "Major"}}}
             """)
         if params["fields"].get("project") is None:
             raise ToolException("Jira project key is required to create an issue. Ask user to provide it.")
     
     def update_issue_validate(self, params: Dict[str, Any]):
         if params.get("key") is None:
             raise ToolException("Jira issue key is required to update an issue. Ask user to provide it.")
         if params.get("fields") is None:
             raise ToolException("""
         Jira fields are provided in a wrong way.
         For example, to update a task with key XXX-123 with new summary, description and custom field, you would pass in the following STRING dictionary: 
-        {{"key": "issue key", "fields": {{"summary": "updated issue", "description": "updated description", "customfield_xxx": "updated custom field"}}}}
+        {"key": "issue key", "fields": {"summary": "updated issue", "description": "updated description", "customfield_xxx": "updated custom field"}}
         """)
 
 
     def search_using_jql(self, jql: str):
         """ Search for Jira issues using JQL."""
         parsed = self._parse_issues(self.client.jql(jql))
         if len(parsed) == 0:
             return "No Jira issues found"
         return "Found " + str(len(parsed)) + " Jira issues:\n" + str(parsed)
 
     def create_issue(self, issue_json: str):
         """ Create an issue in Jira."""
         try:
+            print(issue_json)
             params = json.loads(issue_json)
             self.create_issue_validate(params)
             issue = self.client.issue_create(fields=dict(params["fields"]))
             issue_url = f"{self.client.url}browse/{issue['key']}"
             logger.info(f"issue is created: {issue}")
             return f"Done. Issue {issue['key']} is created successfully. You can view it at {issue_url}. Details: {str(issue)}"
         except ToolException as e:
```

### Comparing `alita_tools-0.0.8/src/alita_tools/openapi/__init__.py` & `alita_tools-0.0.9/src/alita_tools/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.8/src/alita_tools.egg-info/PKG-INFO` & `alita_tools-0.0.9/src/alita_tools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_tools-0.0.8/src/alita_tools.egg-info/SOURCES.txt` & `alita_tools-0.0.9/src/alita_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

