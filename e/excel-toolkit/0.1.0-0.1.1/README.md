# Comparing `tmp/excel_toolkit-0.1.0.tar.gz` & `tmp/excel_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel_toolkit-0.1.0.tar", last modified: Mon Apr 29 07:27:31 2024, max compression
+gzip compressed data, was "excel_toolkit-0.1.1.tar", last modified: Sun May 26 03:50:48 2024, max compression
```

## Comparing `excel_toolkit-0.1.0.tar` & `excel_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:27:31.322041 excel_toolkit-0.1.0/
--rw-rw-rw-   0        0        0      207 2024-04-29 07:27:31.322041 excel_toolkit-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 07:27:31.309810 excel_toolkit-0.1.0/excel_toolkit/
--rw-rw-rw-   0        0        0      174 2024-04-29 07:07:05.000000 excel_toolkit-0.1.0/excel_toolkit/All_Module.py
--rw-rw-rw-   0        0        0     6899 2024-04-06 04:37:01.000000 excel_toolkit-0.1.0/excel_toolkit/Emblem01.py
--rw-rw-rw-   0        0        0     6907 2023-06-01 06:28:59.000000 excel_toolkit-0.1.0/excel_toolkit/EmblemV01.py
--rw-rw-rw-   0        0        0    10390 2023-06-01 06:16:26.000000 excel_toolkit-0.1.0/excel_toolkit/FromWorkPC.py
--rw-rw-rw-   0        0        0     6822 2023-06-01 06:20:40.000000 excel_toolkit-0.1.0/excel_toolkit/LibPortableV01.py
--rw-rw-rw-   0        0        0     3753 2024-03-03 10:30:32.000000 excel_toolkit-0.1.0/excel_toolkit/M01_String.py
--rw-rw-rw-   0        0        0      154 2024-04-17 03:20:50.000000 excel_toolkit-0.1.0/excel_toolkit/__init__.py
--rw-rw-rw-   0        0        0      494 2023-05-24 08:06:41.000000 excel_toolkit-0.1.0/excel_toolkit/learn01.py
--rw-rw-rw-   0        0        0      553 2023-05-24 08:52:48.000000 excel_toolkit-0.1.0/excel_toolkit/other.py
--rw-rw-rw-   0        0        0     6749 2024-04-17 04:06:54.000000 excel_toolkit-0.1.0/excel_toolkit/range.py
--rw-rw-rw-   0        0        0      974 2024-04-06 03:21:38.000000 excel_toolkit-0.1.0/excel_toolkit/scratch01.py
--rw-rw-rw-   0        0        0     5561 2024-04-06 05:01:05.000000 excel_toolkit-0.1.0/excel_toolkit/test_xlwings02.py
--rw-rw-rw-   0        0        0      251 2024-04-06 04:44:28.000000 excel_toolkit-0.1.0/excel_toolkit/workbook.py
--rw-rw-rw-   0        0        0     1106 2024-04-06 04:44:39.000000 excel_toolkit-0.1.0/excel_toolkit/worksheet.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:27:31.320997 excel_toolkit-0.1.0/excel_toolkit.egg-info/
--rw-rw-rw-   0        0        0      207 2024-04-29 07:27:31.000000 excel_toolkit-0.1.0/excel_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-04-29 07:27:31.000000 excel_toolkit-0.1.0/excel_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:27:31.000000 excel_toolkit-0.1.0/excel_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 07:27:31.000000 excel_toolkit-0.1.0/excel_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 07:27:31.000000 excel_toolkit-0.1.0/excel_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 07:27:31.322041 excel_toolkit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      297 2024-04-29 07:27:17.000000 excel_toolkit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:50:48.421474 excel_toolkit-0.1.1/
+-rw-rw-rw-   0        0        0      155 2024-05-26 03:50:48.412207 excel_toolkit-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 03:50:48.382930 excel_toolkit-0.1.1/excel_toolkit/
+-rw-rw-rw-   0        0        0      174 2024-04-29 07:07:05.000000 excel_toolkit-0.1.1/excel_toolkit/All_Module.py
+-rw-rw-rw-   0        0        0    10390 2023-06-01 06:16:26.000000 excel_toolkit-0.1.1/excel_toolkit/FromWorkPC.py
+-rw-rw-rw-   0        0        0     6822 2023-06-01 06:20:40.000000 excel_toolkit-0.1.1/excel_toolkit/LibPortableV01.py
+-rw-rw-rw-   0        0        0      154 2024-05-26 03:49:33.000000 excel_toolkit-0.1.1/excel_toolkit/__init__.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:07.000000 excel_toolkit-0.1.1/excel_toolkit/cant_use_xt.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:00.000000 excel_toolkit-0.1.1/excel_toolkit/fix_bug_xt.py
+-rw-rw-rw-   0        0        0     6772 2024-05-25 04:34:07.000000 excel_toolkit-0.1.1/excel_toolkit/range.py
+-rw-rw-rw-   0        0        0      974 2024-04-06 03:21:38.000000 excel_toolkit-0.1.1/excel_toolkit/scratch01.py
+-rw-rw-rw-   0        0        0      253 2024-05-25 02:47:24.000000 excel_toolkit-0.1.1/excel_toolkit/workbook.py
+-rw-rw-rw-   0        0        0     1106 2024-04-06 04:44:39.000000 excel_toolkit-0.1.1/excel_toolkit/worksheet.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:50:48.405226 excel_toolkit-0.1.1/excel_toolkit.egg-info/
+-rw-rw-rw-   0        0        0      155 2024-05-26 03:50:48.000000 excel_toolkit-0.1.1/excel_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-26 03:50:48.000000 excel_toolkit-0.1.1/excel_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 03:50:48.000000 excel_toolkit-0.1.1/excel_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-26 03:50:48.000000 excel_toolkit-0.1.1/excel_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 03:50:48.000000 excel_toolkit-0.1.1/excel_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 03:50:48.423269 excel_toolkit-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      376 2024-05-26 03:49:40.000000 excel_toolkit-0.1.1/setup.py
```

### Comparing `excel_toolkit-0.1.0/excel_toolkit/FromWorkPC.py` & `excel_toolkit-0.1.1/excel_toolkit/FromWorkPC.py`

 * *Files identical despite different names*

### Comparing `excel_toolkit-0.1.0/excel_toolkit/LibPortableV01.py` & `excel_toolkit-0.1.1/excel_toolkit/LibPortableV01.py`

 * *Files identical despite different names*

### Comparing `excel_toolkit-0.1.0/excel_toolkit/range.py` & `excel_toolkit-0.1.1/excel_toolkit/range.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import xlwings as xw
 from excel_tool.worksheet import ws_at_WB
 from excel_tool.M01_String import St_ContainsNum
 from excel_tool.other import D_OffsetVal
 
 
-def findAllRange2(str_list, ws, wb=None, as_list=True, search_rng=None, caseSensitive=False) -> list:
+def find_all_range(str_list, ws, wb=None, as_list=True, search_rng=None, caseSensitive=False) -> list:
     #  supposed to run much faster than Rg_FindAllRange as it use .api
     
     #  medium tested through get_interaction_grouping
     # Rg_FindAllRange2... seems like this function can run as fast as my VBA Rg_FindAllRange now
     
     
     #  about 2 hrs to write 
@@ -71,22 +71,22 @@
     if as_list:
         return out_list
     else:
         # If needed, implement logic to return a unified range (not directly supported by xlwings)
         return None  # Placeholder: xlwings does not directly support Range union like Excel VBA
 
 
-def pickTilEnd(rng, direction) -> xw.main.Range:
+def pick_til_end(rng, direction) -> xw.main.Range:
         # direction => 'left','right','up','down' as text is shorter
     ws = rng.sheet
     end_address = rng.end(direction).address
     outRng = ws.range(rng.address, end_address)
     return outRng
 
-def findAllRange(str_list,ws,wb=None,as_list=True,search_rng=None,caseSensitive=False) -> xw.main.Range :
+def find_all_range_slow(str_list,ws,wb=None,as_list=True,search_rng=None,caseSensitive=False) -> xw.main.Range :
     # still slow
     ws01 = ws_at_WB(ws,wb)
     out_list = []
     outRng = None
 
     if search_rng:
         search_area = search_rng
@@ -129,40 +129,40 @@
     if as_list:
         return out_list
     else:
         
         return outRng
 
 
-def nextTextCell(rng, direction = "down",cut_off = 100):
+def next_text_cell(rng, direction = "down",cut_off = 100):
     return_text = "No Next Text Cell"
     func = lambda x: not x is None
-    ans = nextCell(rng,direction,func,True,return_text,cut_off)
+    ans = next_cell(rng,direction,func,True,return_text,cut_off)
     return ans
 
-def nextNoTextCell(rng, direction = "down",cut_off = 100):
+def next_no_text_cell(rng, direction = "down",cut_off = 100):
     return_text = "No Next Empty Cell"
     func = lambda x: x is None
-    ans = nextCell(rng,direction,func,True,return_text,cut_off)
+    ans = next_cell(rng,direction,func,True,return_text,cut_off)
     return ans
 
-def nextContainNum(rng, direction = "down",cut_off = 100):
+def next_contain_num(rng, direction = "down",cut_off = 100):
     return_text = "No Next Cell that contains number"
     func = St_ContainsNum
-    ans = nextCell(rng,direction,func,True,return_text,cut_off)
+    ans = next_cell(rng,direction,func,True,return_text,cut_off)
     return ans
 
-def nextNumeric(rng, direction = "down",cut_off = 100):
+def next_numeric(rng, direction = "down",cut_off = 100):
     return_text = "No Next Cell that is Number"
     func = lambda x: isinstance(x,(int,float))
-    ans = nextCell(rng,direction,func,True,return_text,cut_off)
+    ans = next_cell(rng,direction,func,True,return_text,cut_off)
     return ans
 
 
-def nextCell(rng, direction,func_bool,on_value=True,return_text="No Next Cell Found",cut_off = 100):
+def next_cell(rng, direction,func_bool,on_value=True,return_text="No Next Cell Found",cut_off = 100):
     # direction => 'left','right','up','down' as text is shorter
     # func_bool should return only True or False
     # on_value = True func_bool will work on rng.value, otherwise it will work directly on rng
     nextCell = rng
     row_offset, col_offset = D_OffsetVal(direction)
     nextCell = nextCell.offset(row_offset,col_offset)
     try:
```

### Comparing `excel_toolkit-0.1.0/excel_toolkit/scratch01.py` & `excel_toolkit-0.1.1/excel_toolkit/scratch01.py`

 * *Files identical despite different names*

### Comparing `excel_toolkit-0.1.0/excel_toolkit/worksheet.py` & `excel_toolkit-0.1.1/excel_toolkit/worksheet.py`

 * *Files identical despite different names*

