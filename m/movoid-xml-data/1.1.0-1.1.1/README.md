# Comparing `tmp/movoid_xml_data-1.1.0.tar.gz` & `tmp/movoid_xml_data-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_xml_data-1.1.0.tar", last modified: Thu May 23 18:15:29 2024, max compression
+gzip compressed data, was "movoid_xml_data-1.1.1.tar", last modified: Sun May 26 12:22:10 2024, max compression
```

## Comparing `movoid_xml_data-1.1.0.tar` & `movoid_xml_data-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:29.700469 movoid_xml_data-1.1.0/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_xml_data-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      234 2024-05-23 18:15:29.699469 movoid_xml_data-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_xml_data-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:29.690467 movoid_xml_data-1.1.0/movoid_xml_data/
--rw-rw-rw-   0        0        0      214 2024-05-23 18:13:26.000000 movoid_xml_data-1.1.0/movoid_xml_data/__init__.py
--rw-rw-rw-   0        0        0    15905 2024-05-23 18:13:26.000000 movoid_xml_data-1.1.0/movoid_xml_data/label_data.py
--rw-rw-rw-   0        0        0     7862 2024-05-19 17:52:01.000000 movoid_xml_data-1.1.0/movoid_xml_data/tag_data.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:29.698469 movoid_xml_data-1.1.0/movoid_xml_data.egg-info/
--rw-rw-rw-   0        0        0      234 2024-05-23 18:15:29.000000 movoid_xml_data-1.1.0/movoid_xml_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-23 18:15:29.000000 movoid_xml_data-1.1.0/movoid_xml_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:15:29.000000 movoid_xml_data-1.1.0/movoid_xml_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 18:15:29.000000 movoid_xml_data-1.1.0/movoid_xml_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-23 18:15:29.000000 movoid_xml_data-1.1.0/movoid_xml_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 18:15:29.700469 movoid_xml_data-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      484 2024-05-23 18:14:57.000000 movoid_xml_data-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:22:10.062281 movoid_xml_data-1.1.1/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_xml_data-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      260 2024-05-26 12:22:10.061251 movoid_xml_data-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_xml_data-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 12:22:10.051731 movoid_xml_data-1.1.1/movoid_xml_data/
+-rw-rw-rw-   0        0        0      214 2024-05-23 18:13:26.000000 movoid_xml_data-1.1.1/movoid_xml_data/__init__.py
+-rw-rw-rw-   0        0        0    16612 2024-05-26 12:16:24.000000 movoid_xml_data-1.1.1/movoid_xml_data/label_data.py
+-rw-rw-rw-   0        0        0     7862 2024-05-19 17:52:01.000000 movoid_xml_data-1.1.1/movoid_xml_data/tag_data.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:22:10.060237 movoid_xml_data-1.1.1/movoid_xml_data.egg-info/
+-rw-rw-rw-   0        0        0      260 2024-05-26 12:22:10.000000 movoid_xml_data-1.1.1/movoid_xml_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-26 12:22:10.000000 movoid_xml_data-1.1.1/movoid_xml_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 12:22:10.000000 movoid_xml_data-1.1.1/movoid_xml_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-26 12:22:10.000000 movoid_xml_data-1.1.1/movoid_xml_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-26 12:22:10.000000 movoid_xml_data-1.1.1/movoid_xml_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 12:22:10.062281 movoid_xml_data-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      506 2024-05-26 12:21:37.000000 movoid_xml_data-1.1.1/setup.py
```

### Comparing `movoid_xml_data-1.1.0/movoid_xml_data/label_data.py` & `movoid_xml_data-1.1.1/movoid_xml_data/label_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,93 +181,96 @@
                 else:
                     return self._son[index]
             elif isinstance(self._son, dict):
                 return self._son.get(son_key)
             else:
                 return None
 
+    def has_son(self):
+        return self._type in self.__kw_type or self._type in self.__v_type
+
     @property
     def value(self):
         if self._type in self.__kw_type:
             return {k: v.value for k, v in self._son.items()}
         elif self._type in self.__v_type:
             return [_.value for _ in self._son]
         else:
             return self._value
 
-    def items(self):
+    def items(self, value=False):
         if self._type in self.__kw_type:
-            return self._son.items()
+            return [(k, (v.value if value else v)) for k, v in self._son.items()]
         elif self._type in self.__v_type:
-            return enumerate(self._son)
+            return [(k, (v.value if value else v)) for k, v in enumerate(self._son)]
         else:
-            return [['', self._value]]
+            return [['', (self.value if value else self)]]
 
     def keys(self):
         if self._type in self.__kw_type:
             return self._son.keys()
         elif self._type in self.__v_type:
             return range(len(self._son))
         else:
             return ['']
 
-    def values(self):
+    def values(self, value=False):
         if self._type in self.__kw_type:
-            return self._son.values()
+            return [(v.value if value else v) for k, v in self._son.items()]
         elif self._type in self.__v_type:
-            return self._son
+            return [(v.value if value else v) for v in self._son]
         else:
-            return [self._value]
+            return [(self.value if value else self)]
 
     def pure_keys(self, header=''):
         re_list = []
         if self._type in self.__kw_type + self.__v_type:
             for k, v in self._son.items():
                 re_list += v.pure_keys(f'{header} {k}' if header else k)
         else:
             re_list = [header] if header else []
         return re_list
 
-    def pure_values(self, header=''):
+    def pure_values(self, value=False, header=''):
         re_list = []
         if self._type in self.__kw_type + self.__v_type:
             for k, v in self._son.items():
-                re_list += v.pure_keys(f'{header} {k}' if header else k)
+                re_list += v.pure_keys(value, f'{header} {k}' if header else k)
         else:
-            re_list = [self._value] if header else []
+            re_list = [(self.value if value else self)] if header else []
         return re_list
 
-    def pure_items(self, header=''):
+    def pure_items(self, value=False, header=''):
         re_list = []
         if self._type in self.__kw_type + self.__v_type:
             for k, v in self._son.items():
-                re_list += v.pure_items(f'{header} {k}' if header else k)
+                re_list += v.pure_items(value, f'{header} {k}' if header else k)
         else:
-            re_list = [[header, self._value]] if header else []
+            re_list = [[header, (self.value if value else self)]] if header else []
         return re_list
 
     def all_keys(self, header=''):
         re_list = [header] if header else []
         if self._type in self.__kw_type + self.__v_type:
             for k, v in self._son.items():
                 re_list += v.all_keys(f'{header} {k}' if header else k)
         return re_list
 
-    def all_values(self, header=''):
-        re_list = [self._value] if header else []
+    def all_values(self, value=False, header=''):
+        re_list = [(self.value if value else self)] if header else []
         if self._type in self.__kw_type + self.__v_type:
             for k, v in self._son.items():
-                re_list += v.all_keys(f'{header} {k}' if header else k)
+                re_list += v.all_keys(value, f'{header} {k}' if header else k)
         return re_list
 
-    def all_items(self, header=''):
-        re_list = [[header, self._value]] if header else []
+    def all_items(self, value=False, header=''):
+        re_list = [[header, (self.value if value else self)]] if header else []
         if self._type in self.__kw_type + self.__v_type:
             for k, v in self._son.items():
-                re_list += v.all_keys(f'{header} {k}' if header else k)
+                re_list += v.all_keys(value, f'{header} {k}' if header else k)
         return re_list
 
     def to_xml(self, parent_root=None, tag_name='var', **kwargs):
         if parent_root is None:
             root = etree.Element(tag_name)
         else:
             root = etree.SubElement(parent_root, tag_name)
@@ -303,20 +306,20 @@
     def clear(self):
         self._son.clear()
 
     def setdefault(self, key, value):
         if key not in self:
             self[key] = value
 
-    def get(self, key, default=None, *args, __analyse=True, **kwargs):
+    def get(self, key, __default=None, *args, __value=True, __analyse=True, **kwargs):
         try:
-            temp_value = self[key].value
+            temp_value = self[key].value if __value else self[key]
         except KeyError:
-            temp_value = default
-        else:
+            temp_value = __default
+        finally:
             if __analyse and isinstance(temp_value, str):
                 temp_value = self.analyse(temp_value, *args, **kwargs)
         return temp_value
 
     def analyse(self, ori_text, *args, **kwargs):
         temp_str = ori_text
         while True:
@@ -414,17 +417,20 @@
             self._now.clear()
             self.use_labels(self._label_list)
 
     def use_labels(self, labels, clear_now=False):
         labels = [labels] if isinstance(labels, str) else list(labels)
         self.clear_now(clear_now)
         for label in labels:
-            if label in self._body:
+            if label in self._label:
+                label_list = self._label[label].value
                 self._label_list.append(label)
-                self._now += self._body[label]
+                for body_label in label_list:
+                    if body_label in self._body:
+                        self._now += self._body[body_label]
 
     def read(self, file_name, replace=True, reuse_label=True, reuse_label_clear=True, error=False):
         file_path = pathlib.Path(file_name)
         if file_path.is_file():
             if replace:
                 self._label.clear()
                 self._body.clear()
```

### Comparing `movoid_xml_data-1.1.0/movoid_xml_data/tag_data.py` & `movoid_xml_data-1.1.1/movoid_xml_data/tag_data.py`

 * *Files identical despite different names*

