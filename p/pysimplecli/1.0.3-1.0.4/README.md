# Comparing `tmp/pysimplecli-1.0.3.tar.gz` & `tmp/pysimplecli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimplecli-1.0.3.tar", max compression
+gzip compressed data, was "pysimplecli-1.0.4.tar", max compression
```

## Comparing `pysimplecli-1.0.3.tar` & `pysimplecli-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5940 2024-05-19 20:48:42.974579 pysimplecli-1.0.3/README.md
--rw-r--r--   0        0        0     2410 2024-05-19 21:02:16.079271 pysimplecli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       64 2024-04-29 23:39:55.371531 pysimplecli-1.0.3/simplecli/__init__.py
--rw-r--r--   0        0        0    15063 2024-05-19 20:48:42.974899 pysimplecli-1.0.3/simplecli/simplecli.py
--rw-r--r--   0        0        0     6432 1970-01-01 00:00:00.000000 pysimplecli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     5940 2024-05-19 20:48:42.974579 pysimplecli-1.0.4/README.md
+-rw-r--r--   0        0        0     2410 2024-05-26 15:56:41.590623 pysimplecli-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-29 23:39:55.371531 pysimplecli-1.0.4/simplecli/__init__.py
+-rw-r--r--   0        0        0    16492 2024-05-26 15:54:20.550713 pysimplecli-1.0.4/simplecli/simplecli.py
+-rw-r--r--   0        0        0     6432 1970-01-01 00:00:00.000000 pysimplecli-1.0.4/PKG-INFO
```

### Comparing `pysimplecli-1.0.3/README.md` & `pysimplecli-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysimplecli-1.0.3/pyproject.toml` & `pysimplecli-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 shell = """
     poetry run coverage run \
     && poetry run coverage html \
     && open htmlcov/index.html
 """
 [tool.poetry]
 name = "pysimplecli"
-version = "1.0.3"  # Placeholder
+version = "1.0.4"  # Placeholder
 description = "Easily turn functions into command line utilities"
 authors = ["Clif Bratcher <cebratcher@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "simplecli"}
 ]
```

### Comparing `pysimplecli-1.0.3/simplecli/simplecli.py` & `pysimplecli-1.0.4/simplecli/simplecli.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing import (
     Any,
     Callable,
     Union,
     get_args,
     get_origin,
 )
+from types import GenericAlias
 
 try:
     from types import UnionType
 except ImportError:  # pragma: no cover - coverage is generated via py3.12
     # Adapted from cpython/Lib/types.py which defines it as `int | str`.
     # This is ok because if UnionType is not imported, it is not supported.
     UnionType = Union[int, str]  # type: ignore
@@ -38,18 +39,23 @@
     pass
 
 
 class DefaultIfBool:
     pass
 
 
+class UnsupportedType(TypeError):
+    pass
+
+
 _wrapped = False
 ValueType = Union[type[DefaultIfBool], type[Empty], bool, float, int, str]
 ArgDict = dict[str, ValueType]
 ArgList = list[str]
+valid_origins = (Union, UnionType, list, set)
 
 
 class Param(inspect.Parameter):
     internal_only: bool  # Do not pass to wrapped function
     _required: bool  # Exit if a value is not present
     _optional: Union[bool, None] = None  # Mirrors `Optional` type
 
@@ -61,22 +67,14 @@
         )
         # Allow 'name' as a positional parameter
         if "name" not in kwargs:
             if len(argv) == 0:
                 raise TypeError("needs 'name' argument")
             kwargs["name"] = argv[0]
             argv = ()
-        if kwargs["annotation"] not in get_args(ValueType):
-            if get_origin(kwargs["annotation"]) not in (Union, UnionType):
-                if kwargs["annotation"] is not Empty:
-                    raise ValueError(
-                        "annotation type "
-                        f"'{type(kwargs['annotation']).__name__}' "
-                        "is not currently supported!"
-                    )
         param_description = str(kwargs.pop("description", ""))
         param_line = str(kwargs.pop("line", ""))
         param_value = kwargs.pop("value", Empty)
         param_internal_only = bool(kwargs.pop("internal_only", False))
         param_optional = kwargs.pop("optional", None)
         param_required = bool(kwargs.pop("required", True))
         super().__init__(*argv, **kwargs)
@@ -86,14 +84,33 @@
         self._optional = (
             bool(param_optional) if param_optional is not None else None
         )
         self._required = param_required
         # Overrides required as these values are generally unused
         if not self.description:
             self.parse_or_prepend(param_line)
+        self.validate_annotation(kwargs["name"], kwargs["annotation"])
+
+    def validate_annotation(self, name: str, annotation: object) -> None:
+        if annotation in get_args(ValueType):
+            return
+        if get_origin(annotation) in valid_origins:
+            return
+        if annotation is Empty:
+            return
+
+        pretty_annotation = (
+            annotation
+            if (
+                type(annotation) is type
+                or isinstance(annotation, GenericAlias)
+            )
+            else annotation.__class__.__name__
+        )
+        raise UnsupportedType(name, pretty_annotation)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Param):
             return NotImplemented
         return (
             self.name == other.name
             and self.description == other.description
@@ -144,15 +161,15 @@
 
     @property
     def help_name(self) -> str:
         return self.name.replace("_", "-")
 
     @property
     def help_type(self) -> str:
-        if get_origin(self.annotation) in (Union, UnionType):
+        if get_origin(self.annotation) in valid_origins:
             typelist = ", ".join([a.__name__ for a in self.datatypes])
             return f"[{typelist}]"
         return self.annotation.__name__
 
     @property
     def value(self) -> ValueType:
         if self._value is not Empty:
@@ -194,14 +211,17 @@
     def datatypes(self) -> list[type]:
         args = get_args(self.annotation)
         if args:
             return list(args)
         return [self.annotation]
 
     def validate(self, value: ValueType) -> bool:
+        # Recurse for list handling
+        if isinstance(value, list):
+            return all(self.validate(v) for v in value)
         passed = False
         for expected_type in self.datatypes:
             if expected_type is type(None):
                 continue
             try:
                 expected_type(value)
                 return True
@@ -213,15 +233,16 @@
         result = value
         if self.validate(value) is False:
             raise ValueError(
                 f"'{self.help_name}' must be of type {self.help_type}"
             )
         # Handle datatypes
         args = get_args(self.annotation)
-        if args:
+        origin = get_origin(self.annotation)
+        if origin in (Union, UnionType):
             for type_arg in args:
                 with (
                     contextlib.suppress(TypeError),
                     contextlib.suppress(ValueError),
                 ):
                     self._value = type_arg(value)
             return
@@ -229,14 +250,27 @@
             if bool not in self.datatypes:
                 raise ValueError(f"'{self.help_name}' requires a value")
             result = self.default if self.default is not Empty else True
         elif bool in self.datatypes and self.default is Empty:
             result = value
         self._value = self.annotation(result)
 
+    def set_value_as_seq(self, values: ArgList) -> None:
+        args = get_args(self.annotation)
+        origin = get_origin(self.annotation)
+        self._value = []
+        temp_value = []
+        for value in values:
+            if self.validate(value) is False:
+                raise ValueError(
+                    f"'{self.help_name}' must be of type {self.help_type}"
+                )
+            temp_value.append(args[0](value))
+        self._value = origin(temp_value)
+
 
 def tokenize_string(string: str) -> Generator[TokenInfo, None, None]:
     return generate_tokens(io.StringIO(string).readline)
 
 
 def help_text(
     filename: str,
@@ -307,29 +341,27 @@
     params: list[Param],
     pos_args: ArgList,
     kw_args: ArgDict,
 ) -> ArgDict:
     missing_params = []
     try:
         for param in params:
+            kw_value = kw_args.get(param.name)
+            if get_origin(param.annotation) in (list, set):
+                # Consume ALL pos_args if list or set
+                param.set_value_as_seq(pos_args)
+                pos_args.clear()
             # Positional arguments take precedence
-            if pos_args:
+            elif pos_args:
                 param.set_value(pos_args.pop(0))
-            elif param.name in kw_args:
-                if kw_args[param.name] is DefaultIfBool:
-                    # Invert the default value
-                    param.set_value(
-                        True if param.default is Empty else not param.default
-                    )
-                    continue
-                param.set_value(kw_args[param.name])
+            elif kw_value:
+                param.set_value(kw_value)
                 continue
             elif param.required:
                 missing_params.append(param)
-                continue
     except ValueError as e:
         exit(e.args[0])
 
     if pos_args:
         raise TypeError("Too many positional arguments!")
 
     if missing_params:
@@ -372,15 +404,29 @@
         return func
     global _wrapped
     if _wrapped:
         exit("Error, sorry only ONE `@wrap` decorator allowed!")
     _wrapped = True
     filename = sys.argv[0]
     argv = sys.argv[1:]
-    params = extract_code_params(code=func)
+    try:
+        params = extract_code_params(code=func)
+    except UnsupportedType as e:
+        source = inspect.findsource(func)
+        offset = source[1] + 1
+        offset += [
+            index
+            for index, line in enumerate(source[0][source[1] :])
+            if re.search(rf"[\(\s]{e.args[0]}:", line)
+        ][0]
+        exit(
+            f"File \x22{filename}\x22, line {offset}\n"
+            f"{source[0][offset - 1].rstrip()}\n"
+            f"UnsupportedType: {e.args[1]}"
+        )
     pos_args, kw_args = clean_args(argv)
     params.append(
         Param("help", description="Show this message", internal_only=True)
     )
     version = func.__globals__.get("__version__", "")
     if version:
         params.append(
@@ -406,27 +452,26 @@
         exit("\n".join(e.args))
 
     return func(**kwargs)
 
 
 def code_to_ordered_params(code: Callable[..., Any]) -> OrderedDict:
     signature = inspect.signature(code)
-    empty = inspect._empty
-    return OrderedDict(
-        (
-            k,
-            Param(
-                name=v.name,
-                default=Empty if v.default is empty else v.default,
-                annotation=Empty if v.annotation is empty else v.annotation,
-                kind=v.kind,
-            ),
+    result = OrderedDict()
+
+    for k, v in signature.parameters.items():
+        if v.annotation is inspect._empty:
+            exit("ERROR: All wrapped function parameters need type hints!")
+        result[k] = Param(
+            name=v.name,
+            default=Empty if v.default is inspect._empty else v.default,
+            annotation=v.annotation,
+            kind=v.kind,
         )
-        for k, v in signature.parameters.items()
-    )
+    return result
 
 
 def process_comment(
     param: Param | None,
     params: list[Param],
     token: TokenInfo,
 ) -> str:
```

### Comparing `pysimplecli-1.0.3/PKG-INFO` & `pysimplecli-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysimplecli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Easily turn functions into command line utilities
 Author: Clif Bratcher
 Author-email: cebratcher@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

