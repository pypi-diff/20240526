# Comparing `tmp/wireup-0.7.2.tar.gz` & `tmp/wireup-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireup-0.7.2.tar", max compression
+gzip compressed data, was "wireup-0.8.0.tar", max compression
```

## Comparing `wireup-0.7.2.tar` & `wireup-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     3510 2024-04-07 19:43:59.695910 wireup-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3327 2024-04-07 19:40:26.353780 wireup-0.7.2/readme.md
--rw-r--r--   0        0        0      745 2024-04-06 10:38:15.863651 wireup-0.7.2/wireup/__init__.py
--rw-r--r--   0        0        0     2720 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/annotation/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/errors.py
--rw-r--r--   0        0        0     2961 2024-03-29 14:28:28.443108 wireup-0.7.2/wireup/import_util.py
--rw-r--r--   0        0        0        0 2024-03-29 14:24:37.869539 wireup-0.7.2/wireup/integration/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-02 21:36:05.205145 wireup-0.7.2/wireup/integration/fastapi_integration.py
--rw-r--r--   0        0        0     1901 2024-03-29 14:24:37.869539 wireup-0.7.2/wireup/integration/flask_integration.py
--rw-r--r--   0        0        0      722 2024-03-29 14:24:37.869539 wireup-0.7.2/wireup/integration/util.py
--rw-r--r--   0        0        0        0 2023-09-14 21:08:33.059327 wireup-0.7.2/wireup/ioc/__init__.py
--rw-r--r--   0        0        0    15862 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/ioc/dependency_container.py
--rw-r--r--   0        0        0     2589 2024-03-29 14:24:37.873539 wireup-0.7.2/wireup/ioc/initialization_context.py
--rw-r--r--   0        0        0     3049 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/ioc/override_manager.py
--rw-r--r--   0        0        0     3740 2024-04-06 10:38:15.863651 wireup-0.7.2/wireup/ioc/parameter.py
--rw-r--r--   0        0        0     1884 2024-03-29 14:24:37.873539 wireup-0.7.2/wireup/ioc/proxy.py
--rw-r--r--   0        0        0     6746 2024-03-29 14:28:28.443108 wireup-0.7.2/wireup/ioc/service_registry.py
--rw-r--r--   0        0        0     3897 2024-04-02 20:58:05.389534 wireup-0.7.2/wireup/ioc/types.py
--rw-r--r--   0        0        0     1992 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/ioc/util.py
--rw-r--r--   0        0        0        0 2023-10-22 19:11:24.510952 wireup-0.7.2/wireup/py.typed
--rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 wireup-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     3573 2024-05-26 20:21:38.593926 wireup-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4059 2024-05-26 20:17:19.484440 wireup-0.8.0/readme.md
+-rw-r--r--   0        0        0      866 2024-05-26 14:53:53.805340 wireup-0.8.0/wireup/__init__.py
+-rw-r--r--   0        0        0     5208 2024-05-26 20:07:30.073408 wireup-0.8.0/wireup/annotation/__init__.py
+-rw-r--r--   0        0        0     3899 2024-05-26 20:07:30.073408 wireup-0.8.0/wireup/errors.py
+-rw-r--r--   0        0        0     5101 2024-05-25 13:00:17.719229 wireup-0.8.0/wireup/import_util.py
+-rw-r--r--   0        0        0        0 2024-05-18 13:21:01.278641 wireup-0.8.0/wireup/integration/__init__.py
+-rw-r--r--   0        0        0      378 2024-05-19 17:56:51.012767 wireup-0.8.0/wireup/integration/django/__init__.py
+-rw-r--r--   0        0        0      908 2024-05-26 20:08:58.592671 wireup-0.8.0/wireup/integration/django/apps.py
+-rw-r--r--   0        0        0     1537 2024-05-19 17:56:40.184883 wireup-0.8.0/wireup/integration/fastapi_integration.py
+-rw-r--r--   0        0        0     1901 2024-05-19 17:56:49.208786 wireup-0.8.0/wireup/integration/flask_integration.py
+-rw-r--r--   0        0        0      619 2024-05-19 17:56:44.696835 wireup-0.8.0/wireup/integration/util.py
+-rw-r--r--   0        0        0        0 2023-09-14 21:08:33.059327 wireup-0.8.0/wireup/ioc/__init__.py
+-rw-r--r--   0        0        0    15712 2024-05-26 20:07:30.073408 wireup-0.8.0/wireup/ioc/dependency_container.py
+-rw-r--r--   0        0        0     2589 2024-05-19 17:55:36.121569 wireup-0.8.0/wireup/ioc/initialization_context.py
+-rw-r--r--   0        0        0     2956 2024-05-26 20:07:30.073408 wireup-0.8.0/wireup/ioc/override_manager.py
+-rw-r--r--   0        0        0     3740 2024-05-19 17:56:37.468912 wireup-0.8.0/wireup/ioc/parameter.py
+-rw-r--r--   0        0        0     1884 2024-05-19 17:54:24.222342 wireup-0.8.0/wireup/ioc/proxy.py
+-rw-r--r--   0        0        0     7012 2024-05-26 20:07:30.073408 wireup-0.8.0/wireup/ioc/service_registry.py
+-rw-r--r--   0        0        0     3862 2024-05-26 20:07:30.073408 wireup-0.8.0/wireup/ioc/types.py
+-rw-r--r--   0        0        0     2415 2024-05-19 17:55:53.281385 wireup-0.8.0/wireup/ioc/util.py
+-rw-r--r--   0        0        0        0 2023-10-22 19:11:24.510952 wireup-0.8.0/wireup/py.typed
+-rw-r--r--   0        0        0     5431 1970-01-01 00:00:00.000000 wireup-0.8.0/PKG-INFO
```

### Comparing `wireup-0.7.2/pyproject.toml` & `wireup-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [tool.poetry]
 name = "wireup"
-version = "0.7.2"
+version = "0.8.0"
 description = "Python Dependency Injection Library"
 authors = ["Aldo Mateli <aldo.mateli@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/maldoinc/wireup"
-packages = [
-    { include = "wireup" }
-]
+packages = [{ include = "wireup" }]
 keywords = [
     "flask",
     "django",
     "injector",
     "dependency injection",
     "dependency injection container",
-    "dependency injector"
+    "dependency injector",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -42,15 +40,15 @@
 [project.urls]
 Repository = "https://github.com/maldoinc/wireup"
 Documentation = "https://maldoinc.github.io/wireup/"
 Changelog = "https://github.com/maldoinc/wireup/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-graphlib2 = {version="^0.4.7", python=">=3.8,<3.9"}
+graphlib2 = { version = "^0.4.7", python = ">=3.8,<3.9" }
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.3.4"
 setuptools = "^68.0.0"
 mkdocs = "^1.5.2"
 mkdocs-material = "^9.4.14"
 mkdocstrings-python = "^1.6.2"
@@ -65,31 +63,44 @@
 target-version = "py38"
 line-length = 120
 src = ["wireup"]
 lint.fixable = ["ALL"]
 lint.select = ["ALL"]
 lint.ignore = [
     "ANN401", # Allow returning any. Parameter bag has to store/retrieve arbitraty types.
-    "PT009", # Prefer using assertEqual instead of plain asserts
+    "PT009",  # Prefer using assertEqual instead of plain asserts
     "ANN101", # Exclude self from type hint requirement,
-    "TD003", # Exclude "missing issue link for todos",
+    "TD003",  # Exclude "missing issue link for todos",
     "FIX002", # Disable "Line contains to do, consider resolving the issue". It will be done, in due time.
-    "D100", # Disable undocumented public module. The definitions themselves will be documented
-    "D104", # Same as above, disable missing docstring in public package,
-    "D203", # Ignore "one blank line before class". Using "no blank lines before class rule".
-    "D213", # Disable "Summary must go into next line"
-    "D107", # Disable required docs for __init. Can be redundant if class also has them.
-    "A003", # Disable "shadows builtin". OverrideManager.set was flagged by this
+    "D100",   # Disable undocumented public module. The definitions themselves will be documented
+    "D104",   # Same as above, disable missing docstring in public package,
+    "D203",   # Ignore "one blank line before class". Using "no blank lines before class rule".
+    "D213",   # Disable "Summary must go into next line"
+    "D107",   # Disable required docs for __init. Can be redundant if class also has them.
+    "A003",   # Disable "shadows builtin". OverrideManager.set was flagged by this
 
     # Disable as they may cause conflicts with ruff formatter
     "COM812",
-    "ISC001"
+    "ISC001",
 ]
 [tool.ruff.lint.per-file-ignores]
-"test/*" = ["D", "ANN", "PT", "SLF001", "T201", "EM101", "TRY", "FA100", "B008", "RUF009", "F401", "SIM117"]
+"test/*" = [
+    "D",
+    "ANN",
+    "PT",
+    "SLF001",
+    "T201",
+    "EM101",
+    "TRY",
+    "FA100",
+    "B008",
+    "RUF009",
+    "F401",
+    "SIM117",
+]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Taken from https://coverage.readthedocs.io/en/latest/excluding.html
@@ -102,11 +113,11 @@
     "raise AssertionError",
     "raise NotImplementedError",
     "if 0:",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
-    ]
+]
 
 [tool.mypy]
 exclude = "wireup.integration"
```

### Comparing `wireup-0.7.2/wireup/__init__.py` & `wireup-0.8.0/wireup/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from wireup.annotation import ParameterEnum, Wire, wire
-from wireup.import_util import load_module, register_all_in_module, warmup_container
+from wireup.annotation import Inject, ParameterEnum, Wire, abstract, service, wire
+from wireup.import_util import initialize_container, load_module, register_all_in_module, warmup_container
 from wireup.ioc.dependency_container import DependencyContainer
 from wireup.ioc.parameter import ParameterBag
 from wireup.ioc.types import ParameterReference, ServiceLifetime, ServiceOverride
 
 container = DependencyContainer(ParameterBag())
 """Singleton DI container instance.
 
 Use when your application only needs one container.
 """
 
-
 __all__ = [
     "DependencyContainer",
+    "Inject",
     "ParameterBag",
     "ParameterEnum",
     "ParameterReference",
     "ServiceLifetime",
     "ServiceOverride",
     "Wire",
+    "abstract",
     "container",
+    "load_module",
     "register_all_in_module",
+    "service",
     "warmup_container",
-    "load_module",
+    "initialize_container",
     "wire",
 ]
```

### Comparing `wireup-0.7.2/wireup/errors.py` & `wireup-0.8.0/wireup/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
-    from wireup.ioc.types import ContainerProxyQualifierValue
+    from wireup.ioc.types import Qualifier
 
 
 class WireupError(Exception):
     """Base type for all exceptions raised by wrireup."""
 
 
 class DuplicateServiceRegistrationError(WireupError):
     """Raised when attempting to register a service with the same qualifier twice."""
 
-    def __init__(self, klass: type[Any], qualifier: ContainerProxyQualifierValue) -> None:
+    def __init__(self, klass: type[Any], qualifier: Qualifier | None) -> None:
         self.klass = klass
         self.qualifier = qualifier
 
         msg = f"Cannot register type {klass} with qualifier '{qualifier}' as it already exists."
         super().__init__(msg)
 
 
 class DuplicateQualifierForInterfaceError(WireupError):
     """Raised when registering an impl for an interface using a qualifier that is already known."""
 
-    def __init__(self, klass: type[Any], qualifier: ContainerProxyQualifierValue) -> None:
+    def __init__(self, klass: type[Any], qualifier: Qualifier | None) -> None:
         super().__init__(
             f"Cannot register implementation class {klass} for {klass.__base__} "
             f"with qualifier '{qualifier}' as it already exists",
         )
 
 
 class UnknownParameterError(WireupError):
@@ -45,30 +45,30 @@
     def __init__(self) -> None:
         super().__init__("Factory functions must specify a return type denoting the type of dependency it can create.")
 
 
 class FactoryDuplicateServiceRegistrationError(WireupError):
     """Raised when a factory function declares that it produces a type which is already known."""
 
-    def __init__(self, return_type: type[Any], qualifier: ContainerProxyQualifierValue = None) -> None:
+    def __init__(self, return_type: type[Any], qualifier: Qualifier | None = None) -> None:
         self.return_type = return_type
         super().__init__(
             f"A function is already registered as a factory for dependency type {return_type} "
             f"with qualifier {qualifier}."
         )
 
 
 class UnknownQualifiedServiceRequestedError(WireupError):
     """Raised when requesting a type which exists but using an unknown qualifier."""
 
     def __init__(
         self,
         klass: type[Any],
-        qualifier: ContainerProxyQualifierValue,
-        available_qualifiers: set[ContainerProxyQualifierValue],
+        qualifier: Qualifier | None,
+        available_qualifiers: set[Qualifier | None],
     ) -> None:
         self.klass = klass
         self.qualifier = qualifier
 
         super().__init__(
             f"Cannot instantiate concrete class for {klass} as qualifier '{qualifier}' is unknown. "
             f"Available qualifiers: {available_qualifiers}",
@@ -83,23 +83,23 @@
             f"Cannot wire unknown class {klass}. Use @Container.{{register,abstract}} to enable autowiring",
         )
 
 
 class UsageOfQualifierOnUnknownObjectError(WireupError):
     """Raised when using a qualifier on an unknown type that is not managed by the container."""
 
-    def __init__(self, qualifier_value: ContainerProxyQualifierValue) -> None:
+    def __init__(self, qualifier_value: Qualifier | None) -> None:
         super().__init__(f"Cannot use qualifier {qualifier_value} on a type that is not managed by the container.")
 
 
 class InvalidRegistrationTypeError(WireupError):
     """Raised when attempting to call @container.register with an invalid argument."""
 
     def __init__(self, attempted: Any) -> None:
         super().__init__(f"Cannot register {attempted} with the container. Allowed types are callables and types")
 
 
 class UnknownOverrideRequestedError(WireupError):
     """Raised when attempting to override a service which does not exist."""
 
-    def __init__(self, klass: type, qualifier: ContainerProxyQualifierValue) -> None:
+    def __init__(self, klass: type, qualifier: Qualifier | None) -> None:
         super().__init__(f"Cannot override unknown {klass} with qualifier '{qualifier}'.")
```

### Comparing `wireup-0.7.2/wireup/integration/fastapi_integration.py` & `wireup-0.8.0/wireup/integration/fastapi_integration.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.2/wireup/integration/flask_integration.py` & `wireup-0.8.0/wireup/integration/flask_integration.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.2/wireup/integration/util.py` & `wireup-0.8.0/wireup/integration/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import inspect
 from typing import Any, Callable
 
 from wireup import DependencyContainer
-from wireup.ioc.types import InjectableType
-from wireup.ioc.util import parameter_get_type_and_annotation
+from wireup.ioc.util import param_get_annotation
 
 
 def is_view_using_container(dependency_container: DependencyContainer, view: Callable[..., Any]) -> bool:
     """Determine whether the view is using the given dependency container."""
     for dep in inspect.signature(view).parameters.values():
-        param = parameter_get_type_and_annotation(dep)
+        if param := param_get_annotation(dep):
+            is_known_type = param.klass and dependency_container.is_type_known(param.klass)
 
-        is_requesting_injection = isinstance(param.annotation, InjectableType)
-        if is_requesting_injection or (param.klass and dependency_container.is_type_known(param.klass)):
-            return True
+            if param.annotation or is_known_type:
+                return True
 
     return False
```

### Comparing `wireup-0.7.2/wireup/ioc/dependency_container.py` & `wireup-0.8.0/wireup/ioc/dependency_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 import sys
-from typing import TYPE_CHECKING, Any, Callable, Tuple, TypeVar, overload
+from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, TypeVar, overload
 
 from .override_manager import OverrideManager
 
 if sys.version_info[:2] > (3, 8):
     from graphlib import TopologicalSorter
 else:
     from graphlib2 import TopologicalSorter
@@ -20,26 +20,26 @@
 )
 
 from .proxy import ContainerProxy
 from .service_registry import _ServiceRegistry
 from .types import (
     AnnotatedParameter,
     AnyCallable,
-    ContainerProxyQualifierValue,
     EmptyContainerInjectionRequest,
     ParameterWrapper,
+    Qualifier,
     ServiceLifetime,
 )
 
 if TYPE_CHECKING:
     from .initialization_context import InitializationContext
     from .parameter import ParameterBag
 
 __T = TypeVar("__T")
-__ObjectIdentifier = Tuple[type, ContainerProxyQualifierValue]
+__ObjectIdentifier = Tuple[type, Optional[Qualifier]]
 
 
 class DependencyContainer:
     """Dependency Injection and Service Locator container registry.
 
     This contains all the necessary information to initialize registered classes.
     Objects instantiated by the container are lazily loaded and initialized only on first use.
@@ -72,15 +72,15 @@
         self.__initialized_proxies: dict[__ObjectIdentifier, ContainerProxy[Any]] = {}
         self.__buildable_types: set[type] = set()
         self.__params: ParameterBag = parameter_bag
         self.__override_manager: OverrideManager = OverrideManager(
             self.__active_overrides, self.__service_registry.is_type_with_qualifier_known
         )
 
-    def get(self, klass: type[__T], qualifier: ContainerProxyQualifierValue = None) -> __T:
+    def get(self, klass: type[__T], qualifier: Qualifier | None = None) -> __T:
         """Get an instance of the requested type.
 
         Use this to locate services by their type but strongly prefer using injection instead.
 
         :param qualifier: Qualifier for the class if it was registered with one.
         :param klass: Class of the dependency already registered in the container.
         :return: An instance of the requested object. Always returns an existing instance when one is available.
@@ -107,34 +107,34 @@
         return klass
 
     @overload
     def register(
         self,
         obj: None = None,
         *,
-        qualifier: ContainerProxyQualifierValue | None = None,
+        qualifier: Qualifier | None = None,
         lifetime: ServiceLifetime = ServiceLifetime.SINGLETON,
     ) -> Callable[[__T], __T]:
         pass
 
     @overload
     def register(
         self,
         obj: __T,
         *,
-        qualifier: ContainerProxyQualifierValue | None = None,
+        qualifier: Qualifier | None = None,
         lifetime: ServiceLifetime = ServiceLifetime.SINGLETON,
     ) -> __T:
         pass
 
     def register(
         self,
         obj: __T | None = None,
         *,
-        qualifier: ContainerProxyQualifierValue | None = None,
+        qualifier: Qualifier | None = None,
         lifetime: ServiceLifetime = ServiceLifetime.SINGLETON,
     ) -> __T | Callable[[__T], __T]:
         """Register a dependency in the container. Dependency must be either a class or a factory function.
 
         * Use as a decorator without parameters @container.register on a factory function or class to register it.
         * Use as a decorator with parameters to specify qualifier and lifetime, @container.register(qualifier=...).
         * Call it directly with @container.register(some_class_or_factory, qualifier=..., lifetime=...).
@@ -171,15 +171,15 @@
     def clear_initialized_objects(self) -> None:
         """Drop references to initialized singleton objects.
 
         Calling this will cause the container to drop references to initialized singletons
         and cause it to create new instances when they are requested to be injected.
 
         This can be useful in tests in a `unittest.TestCase.setUp` method or pytest autouse=True fixture,
-        allowing you to have a fresh copy of the container with no previously intitialized instances
+        allowing you to have a fresh copy of the container with no previously initialized instances
         to make test cases independent of each-other.
         """
         self.__initialized_objects.clear()
 
     def autowire(self, fn: AnyCallable) -> AnyCallable:
         """Automatically inject resources from the container to the decorated methods.
 
@@ -251,15 +251,15 @@
         # If autowiring, the container is assumed to be final, so unnecessary entries can be removed
         # from the context in order to speed up the autowiring process.
         if names_to_remove:
             self.context.remove_dependencies(fn, names_to_remove)
 
         return values_from_parameters
 
-    def __create_instance(self, klass: type, qualifier: ContainerProxyQualifierValue) -> Any:
+    def __create_instance(self, klass: type, qualifier: Qualifier | None) -> Any:
         """Create the real instances of dependencies. Additional dependencies they may have will be lazily created."""
         self.__assert_dependency_exists(klass, qualifier)
         obj_id = klass, qualifier
 
         if self.__service_registry.is_interface_known(klass):
             klass = self.__resolve_impl(klass, qualifier)
 
@@ -310,17 +310,15 @@
         # We don't actually want that to happen as the value is used only for hinting the container
         # and all values should be supplied.
         if qualifier_value:
             raise UsageOfQualifierOnUnknownObjectError(qualifier_value)
 
         return None
 
-    def __get_instance_or_proxy(
-        self, klass: type, qualifier: ContainerProxyQualifierValue
-    ) -> ContainerProxy[Any] | Any:
+    def __get_instance_or_proxy(self, klass: type, qualifier: Qualifier | None) -> ContainerProxy[Any] | Any:
         """Return a container proxy or an instance of the requested singleton class if one has been initialized."""
         obj_id = klass, qualifier
 
         # If there's an existing instance return that directly without having to proxy it
         if instance := self.__initialized_objects.get(obj_id):
             return instance
 
@@ -335,25 +333,25 @@
             return proxy
 
         proxy = ContainerProxy(lambda: self.__create_instance(klass, qualifier))
         self.__initialized_proxies[obj_id] = proxy
 
         return proxy
 
-    def __resolve_impl(self, klass: type, qualifier: ContainerProxyQualifierValue) -> type:
+    def __resolve_impl(self, klass: type, qualifier: Qualifier | None) -> type:
         impls = self.__service_registry.known_interfaces.get(klass, {})
 
         if qualifier in impls:
             return impls[qualifier]
 
         # We have to raise here otherwise if we have a default hinting the qualifier for an unknown type
         # which will result in the value of the parameter being ContainerProxyQualifier.
         raise UnknownQualifiedServiceRequestedError(klass, qualifier, set(impls.keys()))
 
     def is_type_known(self, klass: type) -> bool:
         """Given a class type return True if's registered in the container as a service or interface."""
         return self.__service_registry.is_impl_known(klass) or self.__service_registry.is_interface_known(klass)
 
-    def __assert_dependency_exists(self, klass: type, qualifier: ContainerProxyQualifierValue) -> None:
+    def __assert_dependency_exists(self, klass: type, qualifier: Qualifier | None) -> None:
         """Assert that there exists an impl with that qualifier or an interface with an impl and the same qualifier."""
         if not self.__service_registry.is_type_with_qualifier_known(klass, qualifier):
             raise UnknownServiceRequestedError(klass)
```

### Comparing `wireup-0.7.2/wireup/ioc/initialization_context.py` & `wireup-0.8.0/wireup/ioc/initialization_context.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.2/wireup/ioc/override_manager.py` & `wireup-0.8.0/wireup/ioc/override_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 from typing import TYPE_CHECKING, Any, Iterator
 
 from wireup.errors import UnknownOverrideRequestedError
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
-    from wireup.ioc.types import ContainerProxyQualifierValue, ServiceOverride
+    from wireup.ioc.types import Qualifier, ServiceOverride
 
 
 class OverrideManager:
     """Enables overriding of services registered with the container."""
 
     def __init__(
         self,
-        active_overrides: dict[tuple[type, ContainerProxyQualifierValue], Any],
-        is_valid_override: Callable[[type, ContainerProxyQualifierValue], bool],
+        active_overrides: dict[tuple[type, Qualifier], Any],
+        is_valid_override: Callable[[type, Qualifier], bool],
     ) -> None:
         self.__is_valid_override = is_valid_override
         self.__active_overrides = active_overrides
 
-    def set(self, target: type, new: Any, qualifier: ContainerProxyQualifierValue = None) -> None:
+    def set(self, target: type, new: Any, qualifier: Qualifier | None = None) -> None:
         """Override the `target` service with `new`.
 
         Subsequent autowire calls to `target` will result in `new` being injected.
 
         :param target: The target service to override.
         :param qualifier: The qualifier of the service to override. Set this if service is registered
         with the qualifier parameter set to a value.
         :param new: The new object to be injected instead of `target`.
         """
         if not self.__is_valid_override(target, qualifier):
             raise UnknownOverrideRequestedError(klass=target, qualifier=qualifier)
 
         self.__active_overrides[target, qualifier] = new
 
-    def delete(self, target: type, qualifier: ContainerProxyQualifierValue = None) -> None:
+    def delete(self, target: type, qualifier: Qualifier | None = None) -> None:
         """Clear active override for the `target` service."""
         if (target, qualifier) in self.__active_overrides:
             del self.__active_overrides[target, qualifier]
 
     def clear(self) -> None:
         """Clear active service overrides."""
         self.__active_overrides.clear()
 
     @contextmanager
-    def service(self, target: type, new: Any, qualifier: ContainerProxyQualifierValue = None) -> Iterator[None]:
+    def service(self, target: type, new: Any, qualifier: Qualifier | None = None) -> Iterator[None]:
         """Override the `target` service with `new` for the duration of the context manager.
 
         Subsequent autowire calls to `target` will result in `new` being injected.
 
         :param target: The target service to override.
         :param qualifier: The qualifier of the service to override. Set this if service is registered
         with the qualifier parameter set to a value.
```

### Comparing `wireup-0.7.2/wireup/ioc/parameter.py` & `wireup-0.8.0/wireup/ioc/parameter.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.2/wireup/ioc/proxy.py` & `wireup-0.8.0/wireup/ioc/proxy.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.2/wireup/ioc/service_registry.py` & `wireup-0.8.0/wireup/ioc/service_registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,37 +8,39 @@
 from wireup.errors import (
     DuplicateQualifierForInterfaceError,
     DuplicateServiceRegistrationError,
     FactoryDuplicateServiceRegistrationError,
     FactoryReturnTypeIsEmptyError,
 )
 from wireup.ioc.initialization_context import InitializationContext
-from wireup.ioc.types import AutowireTarget, InjectableType, ServiceLifetime
-from wireup.ioc.util import is_type_autowireable, parameter_get_type_and_annotation
+from wireup.ioc.types import AnnotatedParameter, AutowireTarget, ServiceLifetime
+from wireup.ioc.util import is_type_autowireable, param_get_annotation
 
 if TYPE_CHECKING:
+    from collections.abc import Iterable
+
     from wireup.ioc.types import (
-        ContainerProxyQualifierValue,
+        Qualifier,
     )
 
 
 class _ServiceRegistry:
     __slots__ = ("known_interfaces", "known_impls", "factory_functions", "context")
 
     def __init__(self) -> None:
-        self.known_interfaces: dict[type, dict[ContainerProxyQualifierValue, type]] = {}
-        self.known_impls: dict[type, set[ContainerProxyQualifierValue]] = defaultdict(set)
-        self.factory_functions: dict[tuple[type, ContainerProxyQualifierValue], Callable[..., Any]] = {}
+        self.known_interfaces: dict[type, dict[Qualifier, type]] = {}
+        self.known_impls: dict[type, set[Qualifier]] = defaultdict(set)
+        self.factory_functions: dict[tuple[type, Qualifier], Callable[..., Any]] = {}
 
         self.context = InitializationContext()
 
     def register_service(
         self,
         klass: type,
-        qualifier: ContainerProxyQualifierValue,
+        qualifier: Qualifier | None,
         lifetime: ServiceLifetime,
     ) -> None:
         if self.is_type_with_qualifier_known(klass, qualifier):
             raise DuplicateServiceRegistrationError(klass, qualifier)
 
         if klass.__base__ and self.is_interface_known(klass.__base__):
             if qualifier in self.known_interfaces[klass.__base__]:
@@ -49,15 +51,15 @@
         self.known_impls[klass].add(qualifier)
         self.target_init_context(klass, lifetime)
 
     def register_abstract(self, klass: type) -> None:
         self.known_interfaces[klass] = defaultdict()
 
     def register_factory(
-        self, fn: Callable[..., Any], lifetime: ServiceLifetime, qualifier: ContainerProxyQualifierValue = None
+        self, fn: Callable[..., Any], lifetime: ServiceLifetime, qualifier: Qualifier | None = None
     ) -> None:
         return_type = inspect.signature(fn).return_annotation
 
         if return_type is Parameter.empty:
             raise FactoryReturnTypeIsEmptyError
 
         if self.is_impl_known_from_factory(return_type, qualifier):
@@ -76,85 +78,87 @@
 
     def target_init_context(self, target: AutowireTarget, lifetime: ServiceLifetime | None = None) -> None:
         """Init and collect all the necessary dependencies to initialize the specified target."""
         if not self.context.init_target(target, lifetime):
             return
 
         for name, parameter in inspect.signature(target).parameters.items():
-            annotated_param = parameter_get_type_and_annotation(parameter)
+            annotated_param = param_get_annotation(parameter)
 
-            if not (annotated_param.klass or annotated_param.annotation):
+            if not annotated_param:
                 continue
 
             # Add to the context only if it's something we can inject
             # or if it is a class that's not one of the builtins: int str dict etc.
             # This is the case for services which are only typed and do not require an annotation.
-            if isinstance(annotated_param.annotation, InjectableType) or is_type_autowireable(annotated_param.klass):
+            if annotated_param.annotation or is_type_autowireable(annotated_param.klass):
                 self.context.add_dependency(target, name, annotated_param)
 
     def get_dependency_graph(self) -> dict[type, set[type]]:
         """Return a dependency graph for the current set of registered services.
 
         This is based on the context's but with the following changes
         * Transient services are removed
         * Objects depending on interfaces will instead depend on all implementations of that interface.
         * Factories are replaced with the thing they produce.
         """
-        factory_to_type = {v: k[0] for k, v in self.factory_functions.items()}
-        res: dict[type, set[type]] = {}
+        factory_to_type: dict[Callable[..., Any], type[Any]] = {v: k[0] for k, v in self.factory_functions.items()}
+        types_created_by_factories = set(factory_to_type.values())
+        res: dict[type, set[type[Any]]] = {}
+
         for target, dependencies in self.context.dependencies.items():
-            if not isinstance(target, type):
+            # If this type is being created by a factory then do not process the current entry
+            # as the dependency graph for it will be processed through the factory.
+            if target in types_created_by_factories:
                 continue
 
-            klass = factory_to_type.get(target, target)
+            klass: type[Any] = factory_to_type.get(target, target)  # type: ignore[arg-type]
 
             if not self.is_impl_singleton(klass):
                 continue
 
-            res[klass] = set()
-            current_deps: list[type] = []
-
-            for annotated_param in dependencies.values():
-                if annotated_param.is_parameter or not annotated_param.klass:
-                    continue
-
-                dependency = annotated_param.klass
-
-                if self.is_interface_known(dependency):
-                    current_deps.extend(self.known_interfaces.get(dependency, {}).values())
-                else:
-                    current_deps.append(dependency)
-
-            for dep in current_deps:
-                if self.is_impl_singleton(dep):
-                    res[klass].add(dep)
+            res[klass] = {cls for cls in self._get_class_deps(dependencies.values()) if self.is_impl_singleton(cls)}
 
         return res
 
+    def _get_class_deps(self, dependencies: Iterable[AnnotatedParameter]) -> set[type[Any]]:
+        """Return a set with non-parameter dependencies from the given annotated parameter list."""
+        current_deps: set[type[Any]] = set()
+
+        for annotated_param in dependencies:
+            if annotated_param.is_parameter or not annotated_param.klass:
+                continue
+
+            if self.is_interface_known(annotated_param.klass):
+                current_deps.update(self.known_interfaces.get(annotated_param.klass, {}).values())
+            else:
+                current_deps.add(annotated_param.klass)
+        return current_deps
+
     def is_impl_known(self, klass: type) -> bool:
         return klass in self.known_impls
 
-    def is_impl_with_qualifier_known(self, klass: type, qualifier_value: ContainerProxyQualifierValue) -> bool:
+    def is_impl_with_qualifier_known(self, klass: type, qualifier_value: Qualifier | None) -> bool:
         return klass in self.known_impls and qualifier_value in self.known_impls[klass]
 
-    def is_type_with_qualifier_known(self, klass: type, qualifier: ContainerProxyQualifierValue) -> bool:
+    def is_type_with_qualifier_known(self, klass: type, qualifier: Qualifier | None) -> bool:
         is_known_impl = self.is_impl_with_qualifier_known(klass, qualifier)
         is_known_intf = self.__is_interface_with_qualifier_known(klass, qualifier)
         is_known_from_factory = self.is_impl_known_from_factory(klass, qualifier)
 
         return is_known_impl or is_known_intf or is_known_from_factory
 
     def __is_interface_with_qualifier_known(
         self,
         klass: type,
-        qualifier: ContainerProxyQualifierValue,
+        qualifier: Qualifier | None,
     ) -> bool:
         return klass in self.known_interfaces and qualifier in self.known_interfaces[klass]
 
-    def is_impl_known_from_factory(self, klass: type, qualifier: ContainerProxyQualifierValue) -> bool:
+    def is_impl_known_from_factory(self, klass: type, qualifier: Qualifier | None) -> bool:
         return (klass, qualifier) in self.factory_functions
 
     def is_impl_singleton(self, klass: type) -> bool:
         return self.context.lifetime.get(klass) == ServiceLifetime.SINGLETON
 
     def is_interface_known(self, klass: type) -> bool:
         return klass in self.known_interfaces
```

### Comparing `wireup-0.7.2/wireup/ioc/types.py` & `wireup-0.8.0/wireup/ioc/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+from collections.abc import Hashable
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Union
 
 AnyCallable = Callable[..., Any]
 AutowireTarget = Union[AnyCallable, type]
 """Represents types that can be targets for autowiring.
 
 This is any method where autowire decorator is used or any class which is registered in the container
 where autowiring happens automatically.
@@ -18,15 +19,15 @@
 
 
 @dataclass(frozen=True)
 class TemplatedString:
     """Wrapper for strings which contain values that must be interpolated by the parameter bag.
 
     Use this with the special ${param_name} syntax to reference a parameter in a string similar to python f-string.
-    Strings in .wire(expr="") calls are automatically wrapped.
+    Strings in Inject(expr="") calls are automatically wrapped.
     """
 
     __slots__ = ("value",)
 
     value: str
 
 
@@ -37,28 +38,28 @@
 class ParameterWrapper(InjectableType):
     """Wrapper for parameter values. This indicates to the container registry that this argument is a parameter."""
 
     __slots__ = ("param",)
     param: ParameterReference
 
 
-ContainerProxyQualifierValue = Optional[Any]
+Qualifier = Hashable
 
 
 @dataclass(frozen=True)
-class ContainerProxyQualifier(InjectableType):
+class ServiceQualifier(InjectableType):
     """Hint the container registry which dependency to load when there are multiple ones registered with the same type.
 
     Use in case of interfaces where there are multiple dependencies that inherit it, but the type of the parameter
     is that of the base class acting as an interface.
     """
 
     __slots__ = ("qualifier",)
 
-    qualifier: ContainerProxyQualifierValue
+    qualifier: Qualifier | None
 
 
 class EmptyContainerInjectionRequest(InjectableType):
     """Serves as hint for the container that it must always perform injection for this parameter.
 
     Instead of skipping, this would force it to throw if dependency is unknown
     """
@@ -77,29 +78,27 @@
 class AnnotatedParameter:
     """Represent an annotated dependency parameter."""
 
     __slots__ = ("klass", "annotation", "qualifier_value", "is_parameter")
 
     def __init__(
         self,
-        klass: type | None = None,
-        annotation: Any | None = None,
+        klass: type[Any] | None = None,
+        annotation: InjectableType | None = None,
     ) -> None:
         """Create a new AnnotatedParameter.
 
         If the annotation is a ContainerProxyQualifier, `qualifier_value` will be set to its value.
 
         :param klass: The type of the dependency
-        :param annotation: Any annotation passed along. Such as Wire(param=...) calls
+        :param annotation: Any annotation passed along. Such as Inject(param=...) calls
         """
         self.klass = klass
         self.annotation = annotation
-        self.qualifier_value = (
-            self.annotation.qualifier if isinstance(self.annotation, ContainerProxyQualifier) else None
-        )
+        self.qualifier_value = self.annotation.qualifier if isinstance(self.annotation, ServiceQualifier) else None
         self.is_parameter = isinstance(self.annotation, ParameterWrapper)
 
     def __eq__(self, other: object) -> bool:
         """Check if two things are equal."""
         return (
             isinstance(other, AnnotatedParameter)
             and self.klass == other.klass
@@ -113,10 +112,10 @@
         return hash((self.klass, self.annotation, self.qualifier_value, self.is_parameter))
 
 
 @dataclass(frozen=True, eq=True)
 class ServiceOverride:
     """Data class to represent a service override. Target type will be replaced with the new type by the container."""
 
-    target: type
-    qualifier: ContainerProxyQualifierValue
+    target: type[Any]
+    qualifier: Qualifier | None
     new: Any
```

### Comparing `wireup-0.7.2/PKG-INFO` & `wireup-0.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wireup
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python Dependency Injection Library
 Home-page: https://github.com/maldoinc/wireup
 License: MIT
 Keywords: flask,django,injector,dependency injection,dependency injection container,dependency injector
 Author: Aldo Mateli
 Author-email: aldo.mateli@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -29,88 +29,107 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: graphlib2 (>=0.4.7,<0.5.0) ; python_version >= "3.8" and python_version < "3.9"
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1>Wireup</h1>
-<p>Dependency Injection Container with a focus on developer experience, type safety and ease of use.</p>
+<p>Modern Dependency Injection for Python.</p>
 
 [![GitHub](https://img.shields.io/github/license/maldoinc/wireup)](https://github.com/maldoinc/wireup)
 [![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/maldoinc/wireup/run_all.yml)](https://github.com/maldoinc/wireup)
 [![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability/maldoinc/wireup?label=Code+Climate)](https://codeclimate.com/github/maldoinc/wireup)
 [![Coverage](https://img.shields.io/codeclimate/coverage/maldoinc/wireup?label=Coverage)](https://codeclimate.com/github/maldoinc/wireup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wireup)](https://pypi.org/project/wireup/)
 [![PyPI - Version](https://img.shields.io/pypi/v/wireup)](https://pypi.org/project/wireup/)
-</div>
 
-> [!TIP]
->    Simplify Dependency injection for Flask using the new
-[Flask integration](https://maldoinc.github.io/wireup/latest/integrations/flask)!
->
->    * Automatically inject dependencies without having to manually call autowire.
->    * Expose flask application configuration in the container.
+<p>Wireup is a performant, concise, and easy-to-use dependency injection container for Python 3.8+.</p>
+</div>
 
 ---
 
 ## ⚡ Key Features
-* Inject Services and Configuration
-* Interfaces / Abstract classes
-* Multiple Containers 
-* Static factories
-* Singleton/Transient dependencies
-* Framework Agnostic
-* Simplified usage in 
-[Flask](https://maldoinc.github.io/wireup/latest/integrations/flask/) 
-and [FastApi](https://maldoinc.github.io/wireup/latest/integrations/fastapi/) using the first-party integrations.
+* Effortlessly Inject services and configuration.
+* Support for interfaces and abstract classes.
+* Factory pattern.
+* Singleton and transient dependencies.
+* Truly declrative container.
+* Framework-agnostic.
+* Simplified integration with [Django](https://maldoinc.github.io/wireup/latest/integrations/django/),
+[Flask](https://maldoinc.github.io/wireup/latest/integrations/flask/), and 
+[FastAPI](https://maldoinc.github.io/wireup/latest/integrations/fastapi/).
 
 ## 📋 Quickstart
 
-Example showing a Database service, a repository and a web view which uses the repository to fetch all posts 
-from a fictional blog db.
+Example showcasing a Redis wrapper and a weather service that calls an external API and caches results as needed.
 
-**1. Register dependencies**
+**1. Set up**
 
 ```python
-from wireup import container
+from wireup import container, initialize_container
+def create_app():
+    app = ...
+    
+    # ⬇️ Expose configuration by populating container.params.
+    container.params.put("redis_url", os.environ["APP_REDIS_URL"])
+    container.params.put("weather_api_key", os.environ["APP_WEATHER_API_KEY"])
+
+    # Bulk update is possible via the "update" method.
+    container.params.update(Settings().model_dump())
+    
+    # Start the container: This registers and initializes services.
+    # `service_modules` contains top-level modules containing registrations.
+    # ⬇️
+    initialize_container(container, service_modules=[services])
+
+    return app
+```
+
+**2. Register services**
 
-# Optionally wire parameters, they serve as configuration for services. 
-# Think of a database url or environment name.
-container.params.update(app.config.items())
-
-
-# Register a class as a service in the container.
-@container.register 
-class DatabaseService:
-    # connection_url will contain the value of the parameter 
-    # with the given name in the annotation.
-    def __init__(self, connection_url: Annotated[str, Wire(param="db_connection_url")]):
-        self.engine = create_engine(connection_url)
-
-        
-# Initializer injection is supported for regular classes as well as dataclasses.
-@container.register
+Use a declarative syntax to describe services, and let the container handle the rest.
+
+```python
+from wireup import service, Inject
+
+@service # ⬅️ Decorator tells the container this is a service.
+class KeyValueStore:
+                                           # This tells the container to inject the value
+                                           # of the parameter during creation.
+                                           # ⬇️ 
+    def __init__(self, dsn: Annotated[str, Inject(param="redis_url")]):
+        self.client = redis.from_url(dsn)
+
+    def get(self, key: str) -> Any: ...
+    def set(self, key: str, value: Any): ...
+
+
+@service
 @dataclass
-class PostRepository:
-    db: DatabaseService 
+class WeatherService:
+    # Inject the value of the parameter to this field. ⬇️
+    api_key: Annotated[str, Inject(param="weather_api_key")]
+    kv_store: KeyValueStore # ⬅️ This will be injected automatically without additional metadata.
 
-    def find_all(self) -> list[Post]:
-        return self.db.query...
+    def get_forecast(self, lat: float, lon: float) -> WeatherForecast:
+        ...
 ```
 
-**2. Inject**
+**3. Inject**
+
+Decorate targets where the library should perform injection.
 
 ```python
-@app.get("/posts")
-@container.autowire 
-# Decorate all targets where the library must perform injection, such as views in an Api.
-# Services are automatically injected based on annotated type.
-# Optional for views when using flask or fastapi integration.
-def get_posts(post_repository: PostRepository):
-    return post_repository.find_all()
+from wireup import container
+
+@app.get("/weather/forecast")
+# ⬇️ Decorating views with autowire enables the container to inject services/parameters.
+@container.autowire
+def get_weather_forecast_view(weather_service: WeatherService, request):
+    return weather_service.get_forecast(request.lat, request.lon)
 ```
 
 **Installation**
 
 ```bash
 # Install using poetry:
 poetry add wireup
```

