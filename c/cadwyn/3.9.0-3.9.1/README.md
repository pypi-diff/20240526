# Comparing `tmp/cadwyn-3.9.0.tar.gz` & `tmp/cadwyn-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadwyn-3.9.0.tar", max compression
+gzip compressed data, was "cadwyn-3.9.1.tar", max compression
```

## Comparing `cadwyn-3.9.0.tar` & `cadwyn-3.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1072 2024-03-01 08:27:46.274066 cadwyn-3.9.0/LICENSE
--rw-r--r--   0        0        0     2379 2024-03-01 08:27:46.274066 cadwyn-3.9.0/README.md
--rw-r--r--   0        0        0      495 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/__init__.py
--rw-r--r--   0        0        0     4423 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/__main__.py
--rw-r--r--   0        0        0    10138 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/_asts.py
--rw-r--r--   0        0        0     5408 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/_compat.py
--rw-r--r--   0        0        0     1443 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/_package_utils.py
--rw-r--r--   0        0        0     4861 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/_utils.py
--rw-r--r--   0        0        0    12326 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/applications.py
--rw-r--r--   0        0        0     1047 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/README.md
--rw-r--r--   0        0        0      355 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/__init__.py
--rw-r--r--   0        0        0     5916 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_common.py
--rw-r--r--   0        0        0     9312 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_main.py
--rw-r--r--   0        0        0        0 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/__init__.py
--rw-r--r--   0        0        0    20111 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/class_migrations.py
--rw-r--r--   0        0        0     3695 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/class_rebuilding.py
--rw-r--r--   0        0        0     1843 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/class_renaming.py
--rw-r--r--   0        0        0     2613 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/import_auto_adding.py
--rw-r--r--   0        0        0     3946 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/latest_version_aliasing.py
--rw-r--r--   0        0        0      722 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/codegen/_plugins/module_migrations.py
--rw-r--r--   0        0        0     1442 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/exceptions.py
--rw-r--r--   0        0        0      218 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/main.py
--rw-r--r--   0        0        0     3372 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/middleware.py
--rw-r--r--   0        0        0        0 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/py.typed
--rw-r--r--   0        0        0    35460 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/route_generation.py
--rw-r--r--   0        0        0     6378 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/routing.py
--rw-r--r--   0        0        0        0 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/static/__init__.py
--rw-r--r--   0        0        0     3455 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/static/docs.html
--rw-r--r--   0        0        0      661 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/__init__.py
--rw-r--r--   0        0        0      269 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/common.py
--rw-r--r--   0        0        0     7128 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/data.py
--rw-r--r--   0        0        0     5627 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/endpoints.py
--rw-r--r--   0        0        0      954 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/enums.py
--rw-r--r--   0        0        0     1268 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/modules.py
--rw-r--r--   0        0        0     8802 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/schemas.py
--rw-r--r--   0        0        0    33289 2024-03-01 08:27:46.274066 cadwyn-3.9.0/cadwyn/structure/versions.py
--rw-r--r--   0        0        0     8098 2024-03-01 08:27:46.282065 cadwyn-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 cadwyn-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-02 13:06:31.299193 cadwyn-3.9.1/LICENSE
+-rw-r--r--   0        0        0     2395 2024-03-02 13:06:31.299193 cadwyn-3.9.1/README.md
+-rw-r--r--   0        0        0      495 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/__init__.py
+-rw-r--r--   0        0        0     4423 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/__main__.py
+-rw-r--r--   0        0        0    10138 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/_asts.py
+-rw-r--r--   0        0        0     5408 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/_compat.py
+-rw-r--r--   0        0        0     1443 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/_package_utils.py
+-rw-r--r--   0        0        0     4861 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/_utils.py
+-rw-r--r--   0        0        0    12326 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/applications.py
+-rw-r--r--   0        0        0     1047 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/README.md
+-rw-r--r--   0        0        0      355 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/__init__.py
+-rw-r--r--   0        0        0     5916 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_common.py
+-rw-r--r--   0        0        0     9312 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_main.py
+-rw-r--r--   0        0        0        0 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/__init__.py
+-rw-r--r--   0        0        0    20111 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/class_migrations.py
+-rw-r--r--   0        0        0     3695 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/class_rebuilding.py
+-rw-r--r--   0        0        0     1843 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/class_renaming.py
+-rw-r--r--   0        0        0     2613 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/import_auto_adding.py
+-rw-r--r--   0        0        0     3946 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/latest_version_aliasing.py
+-rw-r--r--   0        0        0      722 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/codegen/_plugins/module_migrations.py
+-rw-r--r--   0        0        0     1442 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/exceptions.py
+-rw-r--r--   0        0        0      218 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/main.py
+-rw-r--r--   0        0        0     3372 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/middleware.py
+-rw-r--r--   0        0        0        0 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/py.typed
+-rw-r--r--   0        0        0    35460 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/route_generation.py
+-rw-r--r--   0        0        0     6378 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/routing.py
+-rw-r--r--   0        0        0        0 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/static/__init__.py
+-rw-r--r--   0        0        0     3455 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/static/docs.html
+-rw-r--r--   0        0        0      661 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/__init__.py
+-rw-r--r--   0        0        0      269 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/common.py
+-rw-r--r--   0        0        0     7128 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/data.py
+-rw-r--r--   0        0        0     5627 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/endpoints.py
+-rw-r--r--   0        0        0      954 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/enums.py
+-rw-r--r--   0        0        0     1268 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/modules.py
+-rw-r--r--   0        0        0     8802 2024-03-02 13:06:31.299193 cadwyn-3.9.1/cadwyn/structure/schemas.py
+-rw-r--r--   0        0        0    33289 2024-03-02 13:06:31.303192 cadwyn-3.9.1/cadwyn/structure/versions.py
+-rw-r--r--   0        0        0     8149 2024-03-02 13:06:31.307192 cadwyn-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4359 1970-01-01 00:00:00.000000 cadwyn-3.9.1/PKG-INFO
```

### Comparing `cadwyn-3.9.0/LICENSE` & `cadwyn-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/README.md` & `cadwyn-3.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 </a>
 </p>
 
 ## Who is this for?
 
 Cadwyn allows you to support a single version of your code while auto-generating the schemas and routes for older versions. You keep API versioning encapsulated in small and independent "version change" modules while your business logic stays simple and knows nothing about versioning.
 
-Its [approach](https://docs.cadwyn.dev/theory/#ii-migration-based-response-building) will be useful if you want to:
+Its [approach](https://docs.cadwyn.dev/theory/how_we_got_here/#ii-migration-based-response-building) will be useful if you want to:
 
 1. Support many API versions for a long time
 2. Effortlessly backport features and bugfixes to older API versions
 
 Whether you are a newbie in API versioning, a pro looking for a sophisticated tool, an experimenter looking to build a similar framework, or even someone who just wants to learn about all approaches to API versioning -- Cadwyn has the functionality, theory, and documentation to cover all the mentioned use cases.
 
 ## Get started
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
 # Cadwyn Production-ready community-driven modern [Stripe-like](https://
 stripe.com/blog/api-versioning) API versioning in FastAPI ---
           _[_T_e_s_t_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_D_i_s_c_o_r_d_]
 ## Who is this for? Cadwyn allows you to support a single version of your code
 while auto-generating the schemas and routes for older versions. You keep API
 versioning encapsulated in small and independent "version change" modules while
 your business logic stays simple and knows nothing about versioning. Its
-[approach](https://docs.cadwyn.dev/theory/#ii-migration-based-response-
-building) will be useful if you want to: 1. Support many API versions for a
-long time 2. Effortlessly backport features and bugfixes to older API versions
-Whether you are a newbie in API versioning, a pro looking for a sophisticated
-tool, an experimenter looking to build a similar framework, or even someone who
-just wants to learn about all approaches to API versioning -- Cadwyn has the
-functionality, theory, and documentation to cover all the mentioned use cases.
-## Get started The [documentation](https://docs.cadwyn.dev) has everything you
-need to succeed. ## Sponsors These are our gorgeous sponsors. They are using
-Cadwyn and are sponsoring it through various means. Contact [me](https://
-github.com/zmievsa) if you would like to become one too! [![Monite](https://
-docs.cadwyn.dev/img/sponsor_logos/monite.png)](https://docs.monite.com/)
+[approach](https://docs.cadwyn.dev/theory/how_we_got_here/#ii-migration-based-
+response-building) will be useful if you want to: 1. Support many API versions
+for a long time 2. Effortlessly backport features and bugfixes to older API
+versions Whether you are a newbie in API versioning, a pro looking for a
+sophisticated tool, an experimenter looking to build a similar framework, or
+even someone who just wants to learn about all approaches to API versioning -
+- Cadwyn has the functionality, theory, and documentation to cover all the
+mentioned use cases. ## Get started The [documentation](https://
+docs.cadwyn.dev) has everything you need to succeed. ## Sponsors These are our
+gorgeous sponsors. They are using Cadwyn and are sponsoring it through various
+means. Contact [me](https://github.com/zmievsa) if you would like to become one
+too! [![Monite](https://docs.cadwyn.dev/img/sponsor_logos/monite.png)](https://
+docs.monite.com/)
```

### Comparing `cadwyn-3.9.0/cadwyn/__main__.py` & `cadwyn-3.9.1/cadwyn/__main__.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/_asts.py` & `cadwyn-3.9.1/cadwyn/_asts.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/_compat.py` & `cadwyn-3.9.1/cadwyn/_compat.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/_package_utils.py` & `cadwyn-3.9.1/cadwyn/_package_utils.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/_utils.py` & `cadwyn-3.9.1/cadwyn/_utils.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/applications.py` & `cadwyn-3.9.1/cadwyn/applications.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/README.md` & `cadwyn-3.9.1/cadwyn/codegen/README.md`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_common.py` & `cadwyn-3.9.1/cadwyn/codegen/_common.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_main.py` & `cadwyn-3.9.1/cadwyn/codegen/_main.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_plugins/class_migrations.py` & `cadwyn-3.9.1/cadwyn/codegen/_plugins/class_migrations.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_plugins/class_rebuilding.py` & `cadwyn-3.9.1/cadwyn/codegen/_plugins/class_rebuilding.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_plugins/class_renaming.py` & `cadwyn-3.9.1/cadwyn/codegen/_plugins/class_renaming.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_plugins/import_auto_adding.py` & `cadwyn-3.9.1/cadwyn/codegen/_plugins/import_auto_adding.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_plugins/latest_version_aliasing.py` & `cadwyn-3.9.1/cadwyn/codegen/_plugins/latest_version_aliasing.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/codegen/_plugins/module_migrations.py` & `cadwyn-3.9.1/cadwyn/codegen/_plugins/module_migrations.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/exceptions.py` & `cadwyn-3.9.1/cadwyn/exceptions.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/middleware.py` & `cadwyn-3.9.1/cadwyn/middleware.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/route_generation.py` & `cadwyn-3.9.1/cadwyn/route_generation.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/routing.py` & `cadwyn-3.9.1/cadwyn/routing.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/static/docs.html` & `cadwyn-3.9.1/cadwyn/static/docs.html`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/__init__.py` & `cadwyn-3.9.1/cadwyn/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/data.py` & `cadwyn-3.9.1/cadwyn/structure/data.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/endpoints.py` & `cadwyn-3.9.1/cadwyn/structure/endpoints.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/enums.py` & `cadwyn-3.9.1/cadwyn/structure/enums.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/modules.py` & `cadwyn-3.9.1/cadwyn/structure/modules.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/schemas.py` & `cadwyn-3.9.1/cadwyn/structure/schemas.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/cadwyn/structure/versions.py` & `cadwyn-3.9.1/cadwyn/structure/versions.py`

 * *Files identical despite different names*

### Comparing `cadwyn-3.9.0/pyproject.toml` & `cadwyn-3.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cadwyn"
-version = "3.9.0"
+version = "3.9.1"
 description = "Production-ready community-driven modern Stripe-like API versioning in FastAPI"
 authors = ["Stanislav Zmiev <zmievsa@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zmievsa/cadwyn"
 documentation = "https://docs.cadwyn.dev"
 keywords = [
@@ -105,15 +105,15 @@
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
     "@(abc\\.)?abstractmethod",
     "@(typing\\.)?overload",
     "__rich_repr__",
     "__repr__",
 ]
-omit = ["./docs/plugin.py", "./site/plugin.py", "./tests/_data/_temp/**/*", "tests/tutorial/data/**/*"]
+omit = ["./docs/plugin.py", "./site/plugin.py", "./tests/_data/_temp/**/*", "tests/tutorial/data/**/*", "scripts/*.py"]
 
 [tool.pyright]
 reportMissingImports = true
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
 reportPropertyTypeMismatch = true
@@ -133,14 +133,15 @@
 reportFunctionMemberAccess = false
 reportCircularImports = true
 
 
 [tool.ruff]
 target-version = "py310"
 line-length = 120
+extend-exclude = ["scripts/*.py"]
 
 [tool.ruff.lint]
 select = [
     "F",       # pyflakes
     "E",       # pycodestyle errors
     "W",       # pycodestyle warnings
     "C90",     # mccabe
@@ -211,14 +212,15 @@
     "Q001",  # Checks for multiline strings that use single quotes or double quotes
     "Q002",  # Checks for docstrings that use single quotes or double quotes
     "Q003",  # Checks for strings that include escaped quotes
     "COM812",  # Checks for the absence of trailing commas
     "COM819",  # Checks for the presence of prohibited trailing commas
 ]
 
+
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "S",      # ignore bandit security issues in tests
     "B018",   # ignore useless expressions in tests
     "PT012",  # ignore complex with pytest.raises clauses
     "RUF012", # ignore mutable class attributes ClassVar typehint requirement
     "ANN001", # Missing type annotation for function argument
```

### Comparing `cadwyn-3.9.0/PKG-INFO` & `cadwyn-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadwyn
-Version: 3.9.0
+Version: 3.9.1
 Summary: Production-ready community-driven modern Stripe-like API versioning in FastAPI
 Home-page: https://github.com/zmievsa/cadwyn
 License: MIT
 Keywords: python,api,json-schema,stripe,versioning,code-generation,hints,api-versioning,pydantic,fastapi,python310,python311,python312
 Author: Stanislav Zmiev
 Author-email: zmievsa@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -67,15 +67,15 @@
 </a>
 </p>
 
 ## Who is this for?
 
 Cadwyn allows you to support a single version of your code while auto-generating the schemas and routes for older versions. You keep API versioning encapsulated in small and independent "version change" modules while your business logic stays simple and knows nothing about versioning.
 
-Its [approach](https://docs.cadwyn.dev/theory/#ii-migration-based-response-building) will be useful if you want to:
+Its [approach](https://docs.cadwyn.dev/theory/how_we_got_here/#ii-migration-based-response-building) will be useful if you want to:
 
 1. Support many API versions for a long time
 2. Effortlessly backport features and bugfixes to older API versions
 
 Whether you are a newbie in API versioning, a pro looking for a sophisticated tool, an experimenter looking to build a similar framework, or even someone who just wants to learn about all approaches to API versioning -- Cadwyn has the functionality, theory, and documentation to cover all the mentioned use cases.
 
 ## Get started
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cadwyn Version: 3.9.0 Summary: Production-ready
+Metadata-Version: 2.1 Name: cadwyn Version: 3.9.1 Summary: Production-ready
 community-driven modern Stripe-like API versioning in FastAPI Home-page: https:
 //github.com/zmievsa/cadwyn License: MIT Keywords: python,api,json-
 schema,stripe,versioning,code-generation,hints,api-
 versioning,pydantic,fastapi,python310,python311,python312 Author: Stanislav
 Zmiev Author-email: zmievsa@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: FastAPI
@@ -27,19 +27,20 @@
 text/markdown # Cadwyn Production-ready community-driven modern [Stripe-like]
 (https://stripe.com/blog/api-versioning) API versioning in FastAPI ---
           _[_T_e_s_t_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_D_i_s_c_o_r_d_]
 ## Who is this for? Cadwyn allows you to support a single version of your code
 while auto-generating the schemas and routes for older versions. You keep API
 versioning encapsulated in small and independent "version change" modules while
 your business logic stays simple and knows nothing about versioning. Its
-[approach](https://docs.cadwyn.dev/theory/#ii-migration-based-response-
-building) will be useful if you want to: 1. Support many API versions for a
-long time 2. Effortlessly backport features and bugfixes to older API versions
-Whether you are a newbie in API versioning, a pro looking for a sophisticated
-tool, an experimenter looking to build a similar framework, or even someone who
-just wants to learn about all approaches to API versioning -- Cadwyn has the
-functionality, theory, and documentation to cover all the mentioned use cases.
-## Get started The [documentation](https://docs.cadwyn.dev) has everything you
-need to succeed. ## Sponsors These are our gorgeous sponsors. They are using
-Cadwyn and are sponsoring it through various means. Contact [me](https://
-github.com/zmievsa) if you would like to become one too! [![Monite](https://
-docs.cadwyn.dev/img/sponsor_logos/monite.png)](https://docs.monite.com/)
+[approach](https://docs.cadwyn.dev/theory/how_we_got_here/#ii-migration-based-
+response-building) will be useful if you want to: 1. Support many API versions
+for a long time 2. Effortlessly backport features and bugfixes to older API
+versions Whether you are a newbie in API versioning, a pro looking for a
+sophisticated tool, an experimenter looking to build a similar framework, or
+even someone who just wants to learn about all approaches to API versioning -
+- Cadwyn has the functionality, theory, and documentation to cover all the
+mentioned use cases. ## Get started The [documentation](https://
+docs.cadwyn.dev) has everything you need to succeed. ## Sponsors These are our
+gorgeous sponsors. They are using Cadwyn and are sponsoring it through various
+means. Contact [me](https://github.com/zmievsa) if you would like to become one
+too! [![Monite](https://docs.cadwyn.dev/img/sponsor_logos/monite.png)](https://
+docs.monite.com/)
```

