# Comparing `tmp/pypomes_core-1.0.7.tar.gz` & `tmp/pypomes_core-1.0.8.tar.gz`

## Comparing `pypomes_core-1.0.7.tar` & `pypomes_core-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.8/PKG-INFO
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.8/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/src/pypomes_core/__init__.py` & `pypomes_core-1.0.8/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/datetime_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,18 @@
 
     :param dt_str: the date to convert
     :param to_format: the format for the conversion
     :param kwargs: optional arguments for the parser in python-dateutil
     :return:  the converted date
     """
     result: str | None = None
-    ts: datetime = parser.parse(dt_str, **kwargs)
+    ts: datetime = parser.parse(timestr=dt_str,
+                                **kwargs)
     if ts:
-        result = datetime.strftime(ts, to_format)
+        result = ts.strftime(format=to_format)
 
     return result
 
 
 def date_parse(dt_str: str,
                **kwargs: any) -> date:
     """
@@ -55,15 +56,16 @@
 
     :param dt_str: the date, in a supported format
     :param kwargs: optional arguments for the parser in python-dateutil
     :return: the corresponding date object, or None
     """
     result: date | None = None
     if dt_str:
-        result = parser.parse(dt_str, **kwargs).date()
+        result = parser.parse(timestr=dt_str,
+                              **kwargs).date()
 
     return result
 
 
 def datetime_parse(dt_str: str,
                    **kwargs: any) -> datetime:
     """
@@ -76,10 +78,11 @@
 
     :param dt_str: the date, in a supported format
     :param kwargs: optional arguments for the parser in python-dateutil
     :return: the corresponding datetime object, or None
     """
     result: datetime | None = None
     if dt_str:
-        result = parser.parse(dt_str, **kwargs)
+        result = parser.parse(timestr=dt_str,
+                              **kwargs)
 
     return result
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/dict_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     if len(key_chain) == 1:
         # yes, use the provided dict
         parent = source
 
     # does the key chain contain more than 1 element ?
     elif len(key_chain) > 1:
         # yes, obtain the parent element of the last key in the chain
-        parent = dict_get_value(source, key_chain[:-1])
+        parent = dict_get_value(source=source,
+                                key_chain=key_chain[:-1])
 
     # is the parent element a dict ?
     if isinstance(parent, dict):
         # yes, proceed
         key = key_chain[-1]
 
         # is the element denoted by the last key in the chain a list ?
@@ -193,15 +194,16 @@
     if len(key_chain) == 1:
         # yes, use the provided dict
         parent = target
 
     # does the key chain contain more than 1 element ?
     elif len(key_chain) > 1:
         # yes, retrieve the parent element of the last key in the chain
-        parent = dict_get_value(target, key_chain[:-1])
+        parent = dict_get_value(source=target,
+                                key_chain=key_chain[:-1])
 
     # is the parent element a dict ?
     if isinstance(parent, dict):
         # yes, proceed
         key: str = key_chain[-1]
 
         # does the last key un the chain refer to a list element ?
@@ -231,45 +233,55 @@
     """
     Replace, in *target*, all occurrences of *old_value* with *new_value*.
 
     :param target: the reference dict
     :param old_value: the value to be replaced
     :param new_value: the new value
     """
-    def list_replace_value(items: list[any], old_val: any, new_val: any) -> None:
+    def list_replace_value(items: list[any],
+                           old_val: any,
+                           new_val: any) -> None:
         # traverse the list
         for item in items:
 
             # is 'item' a dict ?
             if isinstance(item, dict):
                 # yes, process it recursively
-                dict_replace_value(item, old_val, new_val)
+                dict_replace_value(target=item,
+                                   old_value=old_val,
+                                   new_value=new_val)
 
             # is 'item' a list ?
             elif isinstance(item, list):
                 # yes, process it recursively
-                list_replace_value(item, old_val, new_val)
+                list_replace_value(items=item,
+                                   old_val=old_val,
+                                   new_val=new_val)
 
     # traverse the dict
     for curr_key, curr_value in target.items():
 
         # is 'curr_value' the value to be replaced ?
         if curr_value == old_value:
             # yes, replace it
             target[curr_key] = new_value
 
         # is 'curr_value' a dict ?
         elif isinstance(curr_value, dict):
             # yes, process it recursively
-            dict_replace_value(curr_value, old_value, new_value)
+            dict_replace_value(target=curr_value,
+                               old_value=old_value,
+                               new_value=new_value)
 
         # is 'curr_value' a list ?
         elif isinstance(curr_value, list):
             # yes, process it recursively
-            list_replace_value(curr_value, old_value, new_value)
+            list_replace_value(items=curr_value,
+                               old_val=old_value,
+                               new_val=new_value)
 
 
 def dict_get_key(source: dict,
                  value: any) -> any:
     """
     Return the key in *source*, mapping the first occurrence of *value* found.
 
@@ -326,15 +338,16 @@
         if skey in target:
             # yes, proceed
             tvalue: any = target.get(skey)
 
             # are both elements dictionaries  ?
             if isinstance(svalue, dict) and isinstance(tvalue, dict):
                 # yes, recursively process them
-                dict_merge(tvalue, svalue)
+                dict_merge(target=tvalue,
+                           source=svalue)
 
             # are both elements lists ?
             elif isinstance(svalue, list) and isinstance(tvalue, list):
                 # yes, add the missing elements
                 for item in svalue:
                     if item not in tvalue:
                         tvalue.append(item)
@@ -370,15 +383,16 @@
         in_list: list[any] = curr_dict.get(key)
         if isinstance(in_list, list):
             # yes, recursively invoke the coalescing of the dictionaries in the list
             for in_dict in in_list:
                 # is 'in_dict' a dictionary ?
                 if isinstance(in_dict, dict):
                     # yes, recursively coaslesce it
-                    dict_coalesce(in_dict, key_chain[inx + 1:])
+                    dict_coalesce(target=in_dict,
+                                  key_chain=key_chain[inx + 1:])
             # finalize the operation
             curr_dict = None
             break
 
         # proceed, with the value associated to 'key'
         curr_dict = curr_dict.get(key)
 
@@ -467,15 +481,16 @@
             in_list: list[any] = curr_dict.get(key)
             if isinstance(in_list, list):
                 # sim, invoque recursivamente a redução dos dicionários da lista
                 for in_dict in in_list:
                     # o item da lista é um dicionário ?
                     if isinstance(in_dict, dict):
                         # sim, reduza-o recursivamente
-                        dict_reduce(in_dict, key_chain[inx + 1:])
+                        dict_reduce(target=in_dict,
+                                    key_chain=key_chain[inx + 1:])
                 # termine a operação
                 curr_dict = None
                 break
 
             # prossiga com o valor associado a key
             curr_dict = curr_dict.get(key)
 
@@ -501,15 +516,16 @@
     :return: the 'dict' wanted, or 'None' if not found
     """
     # initialize the return variable
     result: dict | None = None
 
     for item in source:
         if isinstance(item, dict) and \
-           value == dict_get_value(item, key_chain):
+           value == dict_get_value(source=item,
+                                   key_chain=key_chain):
             result = item
             break
 
     return result
 
 
 def dict_from_object(source: object) -> dict:
@@ -521,15 +537,15 @@
     :param source: the reference object
     :return: 'dict' structurally similar to the reference object
     """
     # initialize the return variable
     result: dict = {}
 
     # obtain the object's source module
-    source_module: types.ModuleType = inspect.getmodule(source)
+    source_module: types.ModuleType = inspect.getmodule(object=source)
     # obtain the source module's dictionary
     source_dict: dict = source.__dict__
     # traverse it
     for key, value in source_dict.items():
         # is 'value' None or an empty list ?
         if not (value is None or (isinstance(value, list) and len(value) == 0)):
             # no, proceed
@@ -537,25 +553,25 @@
 
             # is 'value' a list ?
             if isinstance(value, list):
                 # es, traverse it
                 result[name] = []
                 for list_item in value:
                     # is 'list_item' an object of the same module ?
-                    if source_module == inspect.getmodule(list_item):
+                    if source_module == inspect.getmodule(object=list_item):
                         # yes, proceed recursively
-                        result[name].append(dict_from_object(list_item))
+                        result[name].append(dict_from_object(source=list_item))
                     else:
                         # no, proceed linearly
                         result[name].append(list_item)
 
             # is 'value' an object of the same module ?
-            elif source_module == inspect.getmodule(value):
+            elif source_module == inspect.getmodule(object=value):
                 # yes, proceed recursively
-                result[name] = dict_from_object(value)
+                result[name] = dict_from_object(source=value)
             else:
                 # no, proceed linearly
                 result[name] = value
 
     return result
 
 
@@ -593,37 +609,46 @@
         # define a cadeia de chaves de origem
         if prefix_from:
             from_keys: str = f"{prefix_from}.{key}"
         else:
             from_keys: str = key
 
         # obtem a cadeia de chaves de destino
-        to_keys: str = list_find_coupled(from_to_keys, from_keys)
+        to_keys: str = list_find_coupled(coupled_elements=from_to_keys,
+                                         primary_element=from_keys)
 
         # o destino foi definido ?
         if to_keys:
             # sim, obtenha o valor de destino
             if isinstance(value, dict):
                 # valor é um dicionário, transforme-o
-                to_value: dict = dict_transform(value, from_to_keys, from_keys, to_keys)
+                to_value: dict = dict_transform(source=value,
+                                                from_to_keys=from_to_keys,
+                                                prefix_from=from_keys,
+                                                prefix_to=to_keys)
             elif isinstance(value, list):
                 # valor é uma lista, transforme-a
-                to_value: list = list_transform(value, from_to_keys, from_keys, to_keys)
+                to_value: list = list_transform(source=value,
+                                                from_to_keys=from_to_keys,
+                                                prefix_from=from_keys,
+                                                prefix_to=to_keys)
             else:
                 # valor não é dicionário ou lista
                 to_value: any = value
 
             # o prefixo de destino foi definido e ocorre na cadeia de destino ?
             if prefix_to and to_keys.startswith(prefix_to):
                 # sim, remova o prefixo
                 to_keys = to_keys[len(prefix_to)+1:]
-            to_keys_deep: list[str] = list_unflatten(to_keys)
+            to_keys_deep: list[str] = list_unflatten(source=to_keys)
 
             # atribui o valor transformado ao resultado
-            dict_set_value(result, to_keys_deep, to_value)
+            dict_set_value(target=result,
+                           key_chain=to_keys_deep,
+                           value=to_value)
 
     return result
 
 
 def dict_clone(source: dict,
                from_to_keys: list) -> dict:
     """
@@ -647,15 +672,16 @@
     # inicialize the return variable
     result: dict = {}
 
     # traverse the list of elements and add to the target dict
     for elem in from_to_keys:
         from_key: str = elem[0] if isinstance(elem, tuple) else elem
         to_key: str = (elem[1] if isinstance(elem, tuple) and len(elem) > 1 else None) or from_key
-        result[to_key] = dict_get_value(source, list_unflatten(from_key))
+        result[to_key] = dict_get_value(source=source,
+                                        key_chain=list_unflatten(from_key))
 
     return result
 
 
 def dict_listify(target: dict,
                  key_chain: list[str]) -> None:
     """
@@ -671,29 +697,32 @@
                       in_keys: list[str]) -> None:
 
         # traverse the list
         for in_target in in_targets:
             # is the element a dictionary ?
             if isinstance(in_target, dict):
                 # yes, process it
-                dict_listify(in_target, in_keys)
+                dict_listify(target=in_target,
+                             key_chain=in_keys)
             # is the element a list ?
             elif isinstance(in_target, list):
                 # yes, recursively process it
                 # (key chain is also applicable to lists directly nested in lists)
-                items_listify(in_target, in_keys)
+                items_listify(in_targets=in_target,
+                              in_keys=in_keys)
 
     parent: any = target
     # traverse the chain up to its penultimate key
     for inx, key in enumerate(key_chain[:-1]):
         parent = parent.get(key)
         # is the item a list ?
         if isinstance(parent, list):
             # yess, process it and close the operation
-            items_listify(parent, key_chain[inx+1:])
+            items_listify(in_targets=parent,
+                          in_keys=key_chain[inx+1:])
             parent = None
 
         # is it possible to proceed ?
         if not isinstance(parent, dict):
             # no, exit the loop
             break
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/email_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,23 @@
     email_msg = EmailMessage()
     email_msg.set_content(content)
     email_msg["Subject"] = subject
     email_msg["From"] = EMAIL_ACCOUNT
     email_msg["To"] = user_email
 
     # instanciate the email server
-    server = SMTP(host=EMAIL_SERVER, port=EMAIL_PORT)
+    server = SMTP(host=EMAIL_SERVER,
+                  port=EMAIL_PORT)
     server.starttls()
-    server.login(user=EMAIL_ACCOUNT, password=EMAIL_PWD)
+    server.login(user=EMAIL_ACCOUNT,
+                 password=EMAIL_PWD)
 
     # send the message
     try:
-        server.send_message(email_msg)
+        server.send_message(msg=email_msg)
         server.quit()
         if logger:
             logger.debug(f"Sent email {subject} to {user_email}")
     except Exception as e:
         # the operatin raised an exception
         err_msg: str = f"Error sending the email: {exc_format(e, sys.exc_info())}"
         if logger:
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/env_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,16 @@
     """
     Retrieve and return the string value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The str value associated with the key
     """
-    result: str
-    try:
-        result = os.environ[key]
-    except (KeyError, TypeError):
+    result: str = os.environ.get(key)
+    if result is None:
         result = def_value
 
     return result
 
 
 def env_get_bool(key: str,
                  def_value: bool = None) -> bool:
@@ -67,15 +65,15 @@
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The float value associated with the key
     """
     result: float
     try:
-        result = int(os.environ[key])
+        result = float(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_path(key: str,
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/json_pomes.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         - all other types are left unchanged
     HAZARD: depending on the type of object contained in *source*, the final result may not be serializable.
 
     :param source: the dict to be made serializable
     """
     for key, value in source.items():
         if isinstance(value, dict):
-            json_normalize_dict(value)
+            json_normalize_dict(source=value)
         elif isinstance(value, bytes | bytearray):
             source[key] = base64.b64encode(value).decode()
         elif isinstance(value, Iterable) and not isinstance(value, str):
-            source[key] = json_normalize_iterable(value)
+            source[key] = json_normalize_iterable(source=value)
 
 
 def json_normalize_iterable(source: Iterable) -> list[any]:
     """
     Return in a *list* the values in *source* that can be serialized to JSON, thus avoiding *TypeError*.
 
     Possible operations:
@@ -40,12 +40,12 @@
     for value in source:
         if isinstance(value, dict):
             json_normalize_dict(value)
             result.append(value)
         elif isinstance(value, bytes | bytearray):
             result.append(base64.b64encode(value).decode())
         elif isinstance(value, Iterable) and not isinstance(value, str):
-            result.append(json_normalize_iterable(value))
+            result.append(json_normalize_iterable(source=value))
         else:
             result.append(value)
 
     return result
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/list_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,17 +130,23 @@
         if prefix_from is None:
             from_keys: None = None
         else:
             from_keys: str = f"{prefix_from}[{inx}]"
 
         # obtain the target value
         if isinstance(value, dict):
-            to_value: dict = dict_transform(value, from_to_keys, from_keys, prefix_to)
+            to_value: dict = dict_transform(source=value,
+                                            from_to_keys=from_to_keys,
+                                            prefix_from=from_keys,
+                                            prefix_to=prefix_to)
         elif isinstance(value, list):
-            to_value: list = list_transform(value, from_to_keys, from_keys, prefix_to)
+            to_value: list = list_transform(source=value,
+                                            from_to_keys=from_to_keys,
+                                            prefix_from=from_keys,
+                                            prefix_to=prefix_to)
         else:
             to_value: any = value
 
         # added the value transformed to 'result'
         result.append(to_value)
 
     return result
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/str_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any
 
 
 def str_as_list(source: str | Any,
                 separator: str = ",") -> list[any]:
     """
-    Return *source* as a *list*, by splitting its comma-separated contents.
+    Return *source* as a *list*, by splitting its contents separated by *separator*.
 
     If *source* is not a *str*, then it is itself returned.
 
     :param source: the source value to be worked on
     :param separator: the separator (defaults to ",")
     :return: a list built from the contents of the source parameter, or that parameter itself, if is not string
     """
     result: str | list[Any]
     if isinstance(source, str):
-        result = str.split(separator)
+        result = source.split(sep=separator)
     else:
         result = source
 
     return result
 
 
 def str_sanitize(target_str: str) -> str:
@@ -132,15 +132,18 @@
         result = list_dest[pos]
     except (ValueError, IndexError):
         result = None
 
     return result
 
 
-def str_rreplace(source: str, old: str, new: str, count: int = 1) -> str:
+def str_rreplace(source: str,
+                 old: str,
+                 new: str,
+                 count: int = 1) -> str:
     """
     Replace at most *count* occurrences of substring *old* with string *new* in *source*, in reverse order.
 
     :param source: the string to have a substring replaced
     :param old: the substring to replace
     :param new: the string replacement
     :param count: the maximum number of replacements (defaults to 1)
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.8/src/pypomes_core/validation_msgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 __ERR_MSGS: Final[dict] = {
     101: {
         "en": "Error accessing the DB {} in {}: {}",
         "pt": "Erro na interação com o BD {} em {}: {}",
     },
     102: {
-        "en": "No record found on DB {}, in {} for {}",
-        "pt": "Nenhum registro encontrado no BD {}, em {} para {}",
+        "en": "No record found on DB in {}, for {}",
+        "pt": "Nenhum registro encontrado no BD, em {} para {}",
     },
     103: {
         "en": "Error accessing the object store: {}",
         "pt": "Erro na interação com o armazenador de objetos: {}",
     },
     104: {
         "en": "Unexpected error: {}",
```

### Comparing `pypomes_core-1.0.7/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.8/src/pypomes_core/xml_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Final
 from xmltodict3 import XmlTextToDict
 
 from .file_pomes import file_get_data
 
 XML_FILE_HEADER: Final[str] = '<?xml version="1.0" encoding="UTF-8" ?>'
 
@@ -46,27 +47,27 @@
                 result[curr_key] = curr_value
             else:
                 result[curr_key[pos+1:]] = curr_value
 
     return result
 
 
-def xml_to_dict(file_data: bytes | str) -> dict:
+def xml_to_dict(file_data: Path | str | bytes) -> dict:
     """
     Convert the XML into a *dict*, by removing namespaces, and keys prefixed with "@" e "#".
 
     O XML de entrada deve estar em *file_data* (tipo *bytes*),
-    ou em arquivo do sistema com o caminho especificado por *file_data* (tipo *str*).
+    ou em arquivo do sistema com o caminho especificado por *file_data* (tipo *Path* ou *str*).
 
     :param file_data: XML a ser convertido
     :return: dict normalizado
     """
     # obtain the file data
-    file_bytes: bytes = file_get_data(file_data)
+    file_bytes: bytes = file_get_data(file_data=file_data)
 
-    # converte o XML em dict
+    # convert XML to dict
     xml_data = XmlTextToDict(xml_text=file_bytes.decode(),
                              ignore_namespace=True)
     result: dict = xml_data.get_dict()
 
-    # normalize the dict, removing namespaces, and prefixos '@' e '#' from the key names
-    return xml_normalize_keys(result)
+    # normalize the dict, removing namespaces and prefixes '@' e '#' from the key names
+    return xml_normalize_keys(source=result)
```

### Comparing `pypomes_core-1.0.7/LICENSE` & `pypomes_core-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.7/pyproject.toml` & `pypomes_core-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.7/PKG-INFO` & `pypomes_core-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.7
+Version: 1.0.8
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

