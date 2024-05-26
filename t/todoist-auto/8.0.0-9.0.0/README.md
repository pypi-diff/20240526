# Comparing `tmp/todoist_auto-8.0.0.tar.gz` & `tmp/todoist_auto-9.0.0.tar.gz`

## Comparing `todoist_auto-8.0.0.tar` & `todoist_auto-9.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/src/todoist_auto/__init__.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/src/todoist_auto/models.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/src/todoist_auto/rm_empty_sections.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/src/todoist_auto/routine.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/src/todoist_auto/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/LICENSE
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/README.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 todoist_auto-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/src/todoist_auto/__init__.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/src/todoist_auto/models.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/src/todoist_auto/rm_empty_sections.py
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/src/todoist_auto/routine.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/src/todoist_auto/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/LICENSE
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/README.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 todoist_auto-9.0.0/PKG-INFO
```

### Comparing `todoist_auto-8.0.0/.github/workflows/publish-on-pip.yml` & `todoist_auto-9.0.0/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `todoist_auto-8.0.0/src/todoist_auto/models.py` & `todoist_auto-9.0.0/src/todoist_auto/models.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-8.0.0/src/todoist_auto/rm_empty_sections.py` & `todoist_auto-9.0.0/src/todoist_auto/rm_empty_sections.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-8.0.0/src/todoist_auto/routine.py` & `todoist_auto-9.0.0/src/todoist_auto/routine.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 from functools import partial
 from pathlib import Path
 
 import pandas as pd
 import requests
 from todoist_api.api import TodoistAPI
 
-from .models import ColName
-from .models import Notion
-from .models import Todoist
-from .models import TodoistProject
-from .models import TodoistSection
-from .models import TodoistTask
-from .models import Types
-from .util import del_sections
-from .util import get_all_sections
-from .util import get_all_tasks
-from .util import Params
-from .util import ret_not_special_items_of_a_class as rnsioac
+from todoist_auto.models import ColName
+from todoist_auto.models import Notion
+from todoist_auto.models import Todoist
+from todoist_auto.models import TodoistProject
+from todoist_auto.models import TodoistSection
+from todoist_auto.models import TodoistTask
+from todoist_auto.models import Types
+from todoist_auto.util import del_sections
+from todoist_auto.util import get_all_sections
+from todoist_auto.util import get_all_tasks
+from todoist_auto.util import Params
+from todoist_auto.util import ret_not_special_items_of_a_class as rnsioac
 
-warnings.filterwarnings('ignore')
 
 c = ColName()
 ty = Types()
 ts = TodoistSection()
 tsk = TodoistTask()
 tsd = rnsioac(TodoistSection)
 tp = TodoistProject()
@@ -220,28 +219,35 @@
 
     # keep only sections in the day routine project
     msk = df[ts.project_id].eq(pa.routine_proj_id)
     df = df[msk]
 
     del_sections(df[ts.id])
 
-def get_the_routine_fr_notion() :
+def get_routine_from_notion_db() :
+    pass
 
+    ##
     proxies = {
-            'http'  : '172.31.0.235:8080' ,
-            'https' : '172.31.0.235:8080' ,
+            'http'  : '172.31.0.221:8080' ,
+            'https' : '172.31.0.221:8080' ,
             }
 
     if False :
         pass
 
+        ##
+
         r = requests.post(no.db_url , headers = no.hdrs , proxies = proxies)
 
+    ##
     r = requests.post(no.db_url , headers = no.hdrs)
 
+    ##
+
     secs = r.json()['results']
     df = pd.DataFrame(secs)
 
     df = df[['id']]
     df['id'] = df['id'].str.replace('-' , '')
     df[c.url] = no.pg_url + df['id']
 
@@ -315,18 +321,18 @@
     ##
     move_all_tasks_out_of_sections()
 
     ##
     rm_all_sections_in_the_routine_proj()
 
     ##
-    df_a = get_the_routine_fr_notion()
+    dfa = get_routine_from_notion_db()
 
     ##
-    df = get_all_pages_in_routine_db_from_notion(df_a)
+    df = get_all_pages_in_routine_db_from_notion(dfa)
 
     ##
     df = format_page_properties(df)
 
     ##
     df = split_section_order_and_section_name(df)
 
@@ -353,8 +359,7 @@
         df = make_tasks_with_the_indent(df , indnt)
 
 ##
 
 
 if __name__ == "__main__" :
     main()
-    print(f'{Path(__file__).name} Done!')
```

### Comparing `todoist_auto-8.0.0/src/todoist_auto/util.py` & `todoist_auto-9.0.0/src/todoist_auto/util.py`

 * *Files identical despite different names*

### Comparing `todoist_auto-8.0.0/.gitignore` & `todoist_auto-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `todoist_auto-8.0.0/LICENSE` & `todoist_auto-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `todoist_auto-8.0.0/PKG-INFO` & `todoist_auto-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todoist_auto
-Version: 8.0.0
+Version: 9.0.0
 Summary: Automating My Todoist
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

