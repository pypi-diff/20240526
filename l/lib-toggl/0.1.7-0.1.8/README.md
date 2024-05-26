# Comparing `tmp/lib_toggl-0.1.7.tar.gz` & `tmp/lib_toggl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_toggl-0.1.7.tar", max compression
+gzip compressed data, was "lib_toggl-0.1.8.tar", max compression
```

## Comparing `lib_toggl-0.1.7.tar` & `lib_toggl-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-12-26 19:39:10.972800 lib_toggl-0.1.7/LICENSE
--rw-r--r--   0        0        0     3112 2024-05-22 17:50:45.128033 lib_toggl-0.1.7/README.md
--rw-r--r--   0        0        0      168 2024-05-23 17:27:54.569197 lib_toggl-0.1.7/lib_toggl/__init__.py
--rw-r--r--   0        0        0      918 2024-05-23 17:03:38.968701 lib_toggl-0.1.7/lib_toggl/account.py
--rw-r--r--   0        0        0    29593 2024-05-23 17:26:48.940856 lib_toggl-0.1.7/lib_toggl/client.py
--rw-r--r--   0        0        0      372 2024-05-23 17:03:38.968701 lib_toggl-0.1.7/lib_toggl/const.py
--rw-r--r--   0        0        0      582 2024-05-23 17:03:38.968701 lib_toggl-0.1.7/lib_toggl/organization.py
--rw-r--r--   0        0        0     1776 2024-05-23 17:03:38.968701 lib_toggl-0.1.7/lib_toggl/tags.py
--rw-r--r--   0        0        0     9362 2024-05-23 17:03:38.968701 lib_toggl-0.1.7/lib_toggl/time_entries.py
--rw-r--r--   0        0        0     5857 2024-05-23 17:03:38.972034 lib_toggl-0.1.7/lib_toggl/workspace.py
--rw-r--r--   0        0        0      628 2024-05-23 17:27:49.512657 lib_toggl-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 lib_toggl-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-12-26 19:39:10.972800 lib_toggl-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3112 2024-05-26 19:06:55.781060 lib_toggl-0.1.8/README.md
+-rw-r--r--   0        0        0      168 2024-05-26 19:14:32.237855 lib_toggl-0.1.8/lib_toggl/__init__.py
+-rw-r--r--   0        0        0      918 2024-05-23 17:03:38.968701 lib_toggl-0.1.8/lib_toggl/account.py
+-rw-r--r--   0        0        0    29648 2024-05-26 19:11:09.975901 lib_toggl-0.1.8/lib_toggl/client.py
+-rw-r--r--   0        0        0      372 2024-05-23 17:03:38.968701 lib_toggl-0.1.8/lib_toggl/const.py
+-rw-r--r--   0        0        0      582 2024-05-23 17:03:38.968701 lib_toggl-0.1.8/lib_toggl/organization.py
+-rw-r--r--   0        0        0     1776 2024-05-23 17:03:38.968701 lib_toggl-0.1.8/lib_toggl/tags.py
+-rw-r--r--   0        0        0     8278 2024-05-26 19:14:17.984560 lib_toggl-0.1.8/lib_toggl/time_entries.py
+-rw-r--r--   0        0        0     5857 2024-05-23 17:03:38.972034 lib_toggl-0.1.8/lib_toggl/workspace.py
+-rw-r--r--   0        0        0      628 2024-05-26 19:14:40.024504 lib_toggl-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 lib_toggl-0.1.8/PKG-INFO
```

### Comparing `lib_toggl-0.1.7/LICENSE` & `lib_toggl-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.7/README.md` & `lib_toggl-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.7/lib_toggl/account.py` & `lib_toggl-0.1.8/lib_toggl/account.py`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.7/lib_toggl/client.py` & `lib_toggl-0.1.8/lib_toggl/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,38 +427,39 @@
         _url = TIME_ENTRY_CREATE_ENDPOINT(te.workspace_id)
 
         if not te.start:
             te.start = datetime.now(UTC)
             log.debug("te.start was not set, setting to %s", te.start)
 
         # Render out to JSON, exclude the things that user didn't set
-        # In testing, it looks like tag_ids will override tags.
+        # In testing, it looks like tag_ids will override tags; the list of strings is virtually meaningless!
         # If tags is set to a list of strings but tag_action is not set or tag_ids is an empty list, the server will NOT
         #   set the tags and will create a new time track entry with the empty list of tags.
         # So, we default both tags and tag_ids to None and let the user pick which to set.
         # TODO: i'll want to do more sophisticated validation / coercion to handle this case.
         #   e.g: tag_action should remain None unless tags is a list with at least one string, then default to add
+        ##
         data = te.json(exclude_none=True)
         log.debug("create_new_time_entry. To make: %s", data)
         d = await self.do_post_request(_url, data_as_json_str=data)
         # As of now, not a ton of error handling in the do_*_request functions.
         # We do basic checking here to make sure pylance is happy.
         if d is None:
             return None
         return TimeEntry(**d)
 
     async def _persist_time_entry(self, te: TimeEntry) -> TimeEntry | None:
-        """Lower level level API that attemmpts to update state for an existing Time Entry.
+        """Lower level level API that attempts to update state for an existing Time Entry.
         Can be used directly, is meant to be used by higher level API functions like edit_time_entry().
 
         Args:
             te (TimeEntry): Object representing the desired state.
 
         Returns:
-            TimeEntry | None: Object representing the presisted state or None on failure.
+            TimeEntry | None: Object representing the persisted state or None on failure.
         """
         # If user creates a TimeEntry directly and tries to use _persist_time_entry instead of create()
         validate_workspace_id(te.workspace_id)
         validate_time_entry_id(te.id)
 
         _url = TIME_ENTRY_EDIT_ENDPOINT(
             te.workspace_id, te.id  # pyright: ignore reportArgumentType
@@ -469,29 +470,29 @@
         # As of now, not a ton of error handling in the do_*_request functions.
         # We do basic checking here to make sure pylance is happy.
         if d is None:
             return None
         return TimeEntry(**d)
 
     async def edit_time_entry(self, local_te: TimeEntry) -> TimeEntry | None:
-        """High level API that attemmpts to update state for an existing Time Entry.
+        """High level API that attempts to update state for an existing Time Entry.
 
         Modifying some aspects of a Time Entry are trivial, such as the description.
         Tags are a bit more convoluted. Depending on the passed time entry and the desired state
             several API calls may be needed.
         This is abstracted away in the update_tags() function which is called by this function.
         That function is meant to be relatively cheap to call if the user ends up passing in a desired set of tags
             that perfectly overlaps with the current set of tags on the Time Entry.
         In that case, we'll just move on to updating the description for the Time Entry
 
         Args:
             local_te (TimeEntry): Object representing the desired state.
 
         Returns:
-            TimeEntry | None: Object representing the presisted state or None on failure.
+            TimeEntry | None: Object representing the persisted state or None on failure.
         """
         log.debug("edit_time_entry is alive. Starting with %s", local_te)
 
         # To determine if we have any tags to update, we first need to ask the server what IT thinks the passed in TE looks like
         remote_te = await self.get_time_entry_by_id(
             local_te.id  # pyright: ignore reportArgumentType
         )
```

### Comparing `lib_toggl-0.1.7/lib_toggl/organization.py` & `lib_toggl-0.1.8/lib_toggl/organization.py`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.7/lib_toggl/tags.py` & `lib_toggl-0.1.8/lib_toggl/tags.py`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.7/lib_toggl/time_entries.py` & `lib_toggl-0.1.8/lib_toggl/time_entries.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import logging
 from datetime import datetime
 from typing import Any, List, Optional
 
 try:
     # Pydantic v2 ships a copy of v1.
-    from pydantic.v1 import BaseModel, Field, validator
+    from pydantic.v1 import BaseModel, Field
 except ImportError:
     # Home Assistant does not yet support v2.
-    from pydantic import BaseModel, Field, validator
+    from pydantic import BaseModel, Field
 
 from pyrfc3339 import generate
 
 from .const import BASE, DEFAULT_CREATED_BY
 
 log = logging.getLogger(__name__)
 
@@ -78,15 +78,15 @@
 # pylint: disable=invalid-name
 def EXPLICIT_ENDPOINT(time_entry_id: int) -> str:
     """Returns the endpoint for editing specific time entry in the specified workspace"""
     validate_time_entry_id(time_entry_id)
     return f"{BASE}/me/time_entries/{time_entry_id}"
 
 
-class TimeEntry(BaseModel):
+class TimeEntry(BaseModel):  # pyright: ignore reportGeneralTypeIssues
     """Class representing the Toggl organization object.
     Leverages dataclass to cut down on boilerplate code.
     See: https://developers.track.toggl.com/docs/api/time_entries#200
     """
 
     # For Pydantic v1, a sub `config` class holds the custom serialization config.
     # See: https://docs.pydantic.dev/1.10/usage/exporting_models/#json_encoders
@@ -163,20 +163,20 @@
     description: Optional[str] = Field(
         default=None, description="Time entry description, optional"
     )
 
     tag_action: Optional[str] = Field(pattern=r"^(add|delete)$", default="add")
 
     tags: Optional[List[str]] = Field(
-        default=[],
+        default=None,
         description="Tag names",
     )
 
     tag_ids: Optional[List[int]] = Field(
-        default=[],
+        default=None,
         description="Tag IDs.",
     )
 
     # This field is deprecated for GET endpoints where the value will always be true.
     duronly: Optional[bool] = Field(
         exclude=True,
         default=False,
@@ -209,33 +209,7 @@
     pid: Optional[int] = Field(
         exclude=True, default=None, repr=False, description="Project ID, legacy field"
     )
 
     tid: Optional[int] = Field(
         exclude=True, default=None, repr=False, description="Task ID, legacy field"
     )
-
-    # The Toggl API continues to "amaze".
-    # It is absolutely possible to get a reply that looks like this:
-    #       "tags":null,"tag_ids":[]
-    # Which when parsed as json results in tags = None, tag_ids = []
-    # Internally, Pydantic's Optional[] is a Union of the type and None.
-    # This means that we technically are allowed to pass None as a value for tags and tag_ids.
-    # This makes things simple if the user wants to create a TimeEntry with no tags, for example.
-    # But internally, we do not want to expose `None` to the user as a valid value for tags.
-    # The list of tags/tags_ids should always be a list, even if it's an empty list.
-    ##
-    # pylint: disable=no-self-argument
-    @validator("tags", "tag_ids", always=True)
-    def tags_must_not_be_null(cls, v):
-        """Ensures that tag/tag_ids is always an empty list not None
-
-        Args:
-            v (_type_): Value of the field to be validated
-
-        Returns:
-            _type_: `v` if `v` is not None, else an empty list
-        """
-        if v is None:
-            return []
-        else:
-            return v
```

### Comparing `lib_toggl-0.1.7/lib_toggl/workspace.py` & `lib_toggl-0.1.8/lib_toggl/workspace.py`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.7/pyproject.toml` & `lib_toggl-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-toggl"
-version = "0.1.7"
+version = "0.1.8"
 description = "Asynchronous Python library for the Toggl API."
 authors = ["Karl Quinsalnd <karl@karlquinsland.com>"]
 readme = "README.md"
 packages = [{ include = "lib_toggl" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lib_toggl-0.1.7/PKG-INFO` & `lib_toggl-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: lib-toggl
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asynchronous Python library for the Toggl API.
 Author: Karl Quinsalnd
 Author-email: karl@karlquinsland.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiodns (>=3.1.1,<4.0.0)
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: certifi (>=2023.11.17,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.2,<3.0.0)
 Requires-Dist: pyrfc3339 (>=1.1,<2.0)
 Description-Content-Type: text/markdown
```

