# Comparing `tmp/sdss_hal-1.1.9.tar.gz` & `tmp/sdss_hal-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_hal-1.1.9.tar", max compression
+gzip compressed data, was "sdss_hal-1.2.0.tar", max compression
```

## Comparing `sdss_hal-1.1.9.tar` & `sdss_hal-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1504 2024-04-26 15:49:31.607083 sdss_hal-1.1.9/LICENSE.md
--rw-r--r--   0        0        0      816 2024-04-26 15:49:31.607083 sdss_hal-1.1.9/README.md
--rw-r--r--   0        0        0     2672 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/pyproject.toml
--rw-r--r--   0        0        0      483 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/__init__.py
--rw-r--r--   0        0        0     1761 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/__main__.py
--rw-r--r--   0        0        0      356 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/__init__.py
--rw-r--r--   0        0        0     3070 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/actor.py
--rw-r--r--   0        0        0     2939 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/__init__.py
--rw-r--r--   0        0        0     3761 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/auto.py
--rw-r--r--   0        0        0     1593 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/bypass.py
--rw-r--r--   0        0        0      844 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/calibrations.py
--rw-r--r--   0        0        0     7973 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/expose.py
--rw-r--r--   0        0        0     1669 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/goto.py
--rw-r--r--   0        0        0     4434 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/goto_field.py
--rw-r--r--   0        0        0     2455 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/script.py
--rw-r--r--   0        0        0     1419 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/status.py
--rw-r--r--   0        0        0      687 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/actor/commands/test.py
--rw-r--r--   0        0        0     3356 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/hal.yml
--rw-r--r--   0        0        0     2189 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/schema.json
--rw-r--r--   0        0        0      346 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/apo/cartchange.inp
--rw-r--r--   0        0        0     1161 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/apo/eveningcals.inp
--rw-r--r--   0        0        0      161 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/apo/example.inp
--rw-r--r--   0        0        0     1616 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/apo/morningcals.inp
--rw-r--r--   0        0        0       35 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/apo/test.inp
--rw-r--r--   0        0        0      346 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/lco/cartchange.inp
--rw-r--r--   0        0        0     1056 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/lco/eveningcals.inp
--rw-r--r--   0        0        0     1450 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/etc/scripts/lco/morningcals.inp
--rw-r--r--   0        0        0     1180 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/exceptions.py
--rw-r--r--   0        0        0     2373 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/__init__.py
--rw-r--r--   0        0        0    10224 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/apogee.py
--rw-r--r--   0        0        0     6825 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/boss.py
--rw-r--r--   0        0        0     6514 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/cherno.py
--rw-r--r--   0        0        0     1769 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/ffs.py
--rw-r--r--   0        0        0     6715 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/jaeger.py
--rw-r--r--   0        0        0    10429 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/lamps.py
--rw-r--r--   0        0        0     4732 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/overhead.py
--rw-r--r--   0        0        0     4671 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/scripts.py
--rw-r--r--   0        0        0    13441 2024-04-26 15:49:31.611083 sdss_hal-1.1.9/src/hal/helpers/tcc.py
--rw-r--r--   0        0        0     1385 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/apogee_dome_flat.py
--rw-r--r--   0        0        0     7706 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/auto.py
--rw-r--r--   0        0        0    21007 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/expose.py
--rw-r--r--   0        0        0    23656 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/goto_field.py
--rw-r--r--   0        0        0    18518 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/macro.py
--rw-r--r--   0        0        0     1263 2024-04-26 15:49:31.615083 sdss_hal-1.1.9/src/hal/macros/test_macro.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 sdss_hal-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-26 20:09:52.901536 sdss_hal-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0      816 2024-05-26 20:09:52.901536 sdss_hal-1.2.0/README.md
+-rw-r--r--   0        0        0     2708 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      483 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/__init__.py
+-rw-r--r--   0        0        0     1761 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/__main__.py
+-rw-r--r--   0        0        0      356 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/__init__.py
+-rw-r--r--   0        0        0     3024 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/actor.py
+-rw-r--r--   0        0        0     3326 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3940 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/auto_pilot.py
+-rw-r--r--   0        0        0     1593 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/bypass.py
+-rw-r--r--   0        0        0      844 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/calibrations.py
+-rw-r--r--   0        0        0     8082 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/expose.py
+-rw-r--r--   0        0        0     1669 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/goto.py
+-rw-r--r--   0        0        0     3498 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/goto_field.py
+-rw-r--r--   0        0        0     2537 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/script.py
+-rw-r--r--   0        0        0     1419 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/status.py
+-rw-r--r--   0        0        0      687 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/test.py
+-rw-r--r--   0        0        0     3362 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/hal.yml
+-rw-r--r--   0        0        0     2190 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/schema.json
+-rw-r--r--   0        0        0      346 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/cartchange.inp
+-rw-r--r--   0        0        0     1161 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/eveningcals.inp
+-rw-r--r--   0        0        0      161 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/example.inp
+-rw-r--r--   0        0        0     1616 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/morningcals.inp
+-rw-r--r--   0        0        0       35 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/test.inp
+-rw-r--r--   0        0        0      346 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/lco/cartchange.inp
+-rw-r--r--   0        0        0     1056 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/lco/eveningcals.inp
+-rw-r--r--   0        0        0     1450 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/lco/morningcals.inp
+-rw-r--r--   0        0        0     1180 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/exceptions.py
+-rw-r--r--   0        0        0     3502 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/__init__.py
+-rw-r--r--   0        0        0    10610 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/apogee.py
+-rw-r--r--   0        0        0     7101 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/boss.py
+-rw-r--r--   0        0        0     6514 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/cherno.py
+-rw-r--r--   0        0        0     1769 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/ffs.py
+-rw-r--r--   0        0        0     8270 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/jaeger.py
+-rw-r--r--   0        0        0    10429 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/lamps.py
+-rw-r--r--   0        0        0     4732 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/overhead.py
+-rw-r--r--   0        0        0     4671 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/scripts.py
+-rw-r--r--   0        0        0    13441 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/tcc.py
+-rw-r--r--   0        0        0     1399 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/apogee_dome_flat.py
+-rw-r--r--   0        0        0    12278 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/auto_pilot.py
+-rw-r--r--   0        0        0    21544 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/expose.py
+-rw-r--r--   0        0        0    23929 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/goto_field.py
+-rw-r--r--   0        0        0    18881 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/macro.py
+-rw-r--r--   0        0        0     1263 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/test_macro.py
+-rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.2.0/PKG-INFO
```

### Comparing `sdss_hal-1.1.9/LICENSE.md` & `sdss_hal-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/README.md` & `sdss_hal-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/pyproject.toml` & `sdss_hal-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-hal"
-version = "1.1.9"
+version = "1.2.0"
 description = "High-level observing tool for SDSS-V (replaces SOP)"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/hal"
 repository = "https://github.com/sdss/hal"
 documentation = "https://sdss-hal.readthedocs.org"
@@ -26,19 +26,20 @@
 
 [tool.poetry.scripts]
 hal = "hal.__main__:hal"
 
 [tool.poetry.dependencies]
 python = "^3.10,<4.0"
 sdsstools = "^1.0.0"
-sdss-clu = "^2.0.0"
+sdss-clu = "^2.2.7"
 click-default-group = "^1.2.2"
 numpy = "^1.22.1"
 sdssdb = ">=0.8.3"
 peewee = "^3.17.0"
+typing-extensions = "^4.11.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=8.0.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.23.4"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
@@ -55,20 +56,20 @@
 myst-parser = ">=0.15.2"
 nox = ">=2021.6.12"
 sphinx-autobuild = ">=2021.3.14"
 ruff = ">=0.0.291"
 
 [tool.black]
 line-length = 88
-target-version = ['py311']
+target-version = ['py312']
 fast = true
 
 [tool.ruff]
 line-length = 88
-target-version = 'py311'
+target-version = 'py312'
 exclude = ["typings/"]
 
 [ruff.lint]
 select = ["E", "F", "I"]
 unfixable = ["F841"]
 
 [tool.ruff.lint.per-file-ignores]
@@ -87,15 +88,15 @@
 addopts = "--cov hal --cov-report xml --cov-report html --cov-report term -W ignore"
 asyncio_mode = "auto"
 
 [tool.coverage.run]
 branch = true
 include = ["src/hal/*"]
 omit = [
-    "*/__init__.py",
+    "src/hal/__init__.py",
     "src/hal/__main__.py",
     "src/hal/exceptions.py",
     "src/hal/macros/test_macro.py",
     "src/hal/actor/commands/test.py"
 ]
 
 [tool.coverage.report]
```

### Comparing `sdss_hal-1.1.9/src/hal/__main__.py` & `sdss_hal-1.2.0/src/hal/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/actor/actor.py` & `sdss_hal-1.2.0/src/hal/actor/actor.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,25 @@
 # @Filename: actor.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import os
 
-from typing import ClassVar, TypeVar
+from typing import ClassVar
 
 from clu.legacy import LegacyActor
 
 from hal import __version__
 from hal.actor.commands import hal_command_parser
 
 
 __all__ = ["HALActor", "ActorHelpers"]
 
 
-T = TypeVar("T", bound="HALActor")
-
-
 class HALActor(LegacyActor):
     """HAL actor."""
 
     _instance: ClassVar[HALActor | None] = None
     parser = hal_command_parser
 
     def __init__(self, *args, **kwargs):
```

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/__init__.py` & `sdss_hal-1.2.0/src/hal/actor/commands/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 # @Date: 2022-12-26
 # @Filename: __init__.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import functools
+from re import L
 
 from typing import TYPE_CHECKING
 
 import click
 
 from clu import Command
 from clu.parsers.click import command_parser, coro_helper
 
 from hal.macros.macro import StageType, flatten
 
 
 if TYPE_CHECKING:
-    from hal.actor.actor import HALActor
+    from hal.actor import HALActor, HALCommandType
 
 
 hal_command_parser = command_parser
 
 
 def stages(macro_name: str, reset: bool = True):
     """A decorator that adds ``--stages`` and ``--list-stages`` options.
@@ -89,15 +90,27 @@
                 return await coro_helper(f, command, macro, stages, *args, **kwargs)
 
         return functools.update_wrapper(wrapper, f)
 
     return decorator
 
 
-from .auto import *
+def fail_if_running_macro(command: HALCommandType):
+    """Fails a command if a macro is already running."""
+
+    macros = command.actor.helpers.macros
+    running_macros = [macro for macro in macros if macros[macro].running]
+    if any(running_macros):
+        command.fail("An expose macro is already running.")
+        return False
+
+    return True
+
+
+from .auto_pilot import *
 from .bypass import *
 from .calibrations import *
 from .expose import *
 from .goto import *
 from .goto_field import *
 from .script import *
 from .status import *
```

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/auto.py` & `sdss_hal-1.2.0/src/hal/actor/commands/auto_pilot.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from . import hal_command_parser
 
 
 if TYPE_CHECKING:
     from .. import HALCommandType
 
 
-__all__ = ["auto"]
+__all__ = ["auto_pilot"]
 
 
-@hal_command_parser.command(name="auto")
+@hal_command_parser.command(name="auto-pilot", aliases=["auto"])
 @click.option(
     "--stop",
     is_flag=True,
     help="Stops the auto mode loop after the next stage completes. "
     "For an immediate stop use with --now.",
 )
 @click.option(
@@ -61,36 +61,36 @@
 )
 @click.option(
     "--preload-ahead",
     type=float,
     default=None,
     help="Preload the next design this many seconds before the exposure completes.",
 )
-async def auto(
+async def auto_pilot(
     command: HALCommandType,
     stop: bool = False,
     now: bool = False,
     modify: bool = False,
     pause: bool = False,
     resume: bool = False,
     count: int = 1,
     preload_ahead: float | None = None,
 ):
-    """Starts the auto mode."""
+    """Starts the auto-pilot mode."""
 
     assert command.actor
 
     expose_macro = command.actor.helpers.macros["expose"]
     assert isinstance(expose_macro, ExposeMacro)
 
-    macro = command.actor.helpers.macros["auto"]
+    macro = command.actor.helpers.macros["auto_pilot"]
 
     if (stop or modify or pause or resume) and not macro.running:
         return command.fail(
-            "I'm afraid I cannot do that Dave. The auto mode is not running."
+            "I'm afraid I cannot do that Dave. The auto pilot mode is not running."
         )
 
     if pause and resume:
         return command.fail("--pause and --resume are incompatible Dave.")
 
     if pause:
         await expose_macro._pause()
@@ -98,18 +98,18 @@
 
     if resume:
         await expose_macro._resume()
         return command.finish()
 
     if stop is True:
         if now is True:
-            command.warning(auto_mode_message="Cancelling auto mode NOW.")
+            command.warning(auto_pilot_message="Stopping auto-pilot mode NOW.")
             macro.cancel(now=True)
         else:
-            command.warning(auto_mode_message="Cancelling auto after stage completes.")
+            command.warning(auto_pilot_message="Stopping auto-pilot after this stage.")
             macro.cancel(now=False)
 
         return command.finish()
 
     if modify is True:
         # For now the only option we can modify is the count of exposures.
         macro.config["count"] = count
@@ -126,18 +126,22 @@
 
     # From this point on this is a new macro, so it should not be already running.
     if macro.running:
         return command.fail(
             "I'm afraid I cannot do that Dave. The auto mode is already running."
         )
 
+    macro.reset(command, count=count, preload_ahead_time=preload_ahead)
+
     result: bool = True
     while True:
+        # Reset the macro (stages and such) but keep the current config.
+        macro.reset(command, reset_config=False)
+
         # Run the auto loop until the command is cancelled.
-        macro.reset(command, count=count, preload_ahead_time=preload_ahead)
         if not await macro.run():
             result = False
             break
 
         await asyncio.sleep(0.1)
 
         if macro.cancelled:
```

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/bypass.py` & `sdss_hal-1.2.0/src/hal/actor/commands/bypass.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/calibrations.py` & `sdss_hal-1.2.0/src/hal/actor/commands/calibrations.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/expose.py` & `sdss_hal-1.2.0/src/hal/actor/commands/expose.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import click
 
 from hal import config
 from hal.helpers import get_default_exposure_time
 from hal.macros.macro import StageType, flatten
 
-from . import hal_command_parser, stages
+from . import fail_if_running_macro, hal_command_parser, stages
 
 
 if TYPE_CHECKING:
     from hal.macros.expose import ExposeMacro
 
     from .. import HALCommandType
 
@@ -156,16 +156,20 @@
     reads: int | None = None,
     initial_apogee_dither: str | None = None,
     with_fpi: bool = True,
     disable_readout_matching: bool = False,
 ):
     """Take science exposures."""
 
-    if (stop or modify or pause or resume) and not macro.running:
-        return command.fail("No expose macro currently running.")
+    if stop or modify or pause or resume:
+        if not macro.running:
+            return command.fail("No expose macro currently running.")
+    else:
+        if not fail_if_running_macro(command):
+            return
 
     # Check incompatible options.
     if exposure_time and (boss_exposure_time or apogee_exposure_time or reads):
         return command.fail(
             "--exposure-time cannot be used with "
             "--apogee-exposure-time, --boss-exposure-time or --reads."
         )
```

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/goto.py` & `sdss_hal-1.2.0/src/hal/actor/commands/goto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/script.py` & `sdss_hal-1.2.0/src/hal/actor/commands/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import click
 
-from . import hal_command_parser
+from . import fail_if_running_macro, hal_command_parser
 
 
 if TYPE_CHECKING:
     from . import HALCommandType
 
 
 __all__ = ["script"]
@@ -65,14 +65,17 @@
 
 
 @script.command()
 @click.argument("SCRIPT", type=str)
 async def run(command: HALCommandType, script: str):
     """Runs a script."""
 
+    if not fail_if_running_macro(command):
+        return
+
     try:
         result = await command.actor.helpers.scripts.run(script, command)
     except Exception as err:
         return command.fail(error=err)
 
     if result is True:
         return command.finish(text=f"Script {script} has been successfully executed.")
```

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/status.py` & `sdss_hal-1.2.0/src/hal/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/actor/commands/test.py` & `sdss_hal-1.2.0/src/hal/actor/commands/test.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/etc/hal.yml` & `sdss_hal-1.2.0/src/hal/etc/hal.yml`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
       count: 1
       exptime:
         default: 900
         bright_design_mode:
           APO: 730
           LCO: 900
 
-  auto:
+  auto_pilot:
     guider_time: 15
     min_rms: 3.0
     count: 1
     preload_ahead_time: 300
 
 goto:
   stow:
```

### Comparing `sdss_hal-1.1.9/src/hal/etc/schema.json` & `sdss_hal-1.2.0/src/hal/etc/schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'properties'": "{'auto_pilot_message': OrderedDict([('type', 'string')]), delete: "*

 * *                 "['auto_mode_message']}"}*

```diff
@@ -5,15 +5,15 @@
         "all_stages": {
             "items": {
                 "type": "string"
             },
             "minLength": 2,
             "type": "array"
         },
-        "auto_mode_message": {
+        "auto_pilot_message": {
             "type": "string"
         },
         "available_scripts": {
             "items": {
                 "type": "string"
             },
             "type": "array"
```

### Comparing `sdss_hal-1.1.9/src/hal/etc/scripts/apo/eveningcals.inp` & `sdss_hal-1.2.0/src/hal/etc/scripts/apo/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/etc/scripts/apo/morningcals.inp` & `sdss_hal-1.2.0/src/hal/etc/scripts/apo/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/etc/scripts/lco/eveningcals.inp` & `sdss_hal-1.2.0/src/hal/etc/scripts/lco/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/etc/scripts/lco/morningcals.inp` & `sdss_hal-1.2.0/src/hal/etc/scripts/lco/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/exceptions.py` & `sdss_hal-1.2.0/src/hal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/helpers/apogee.py` & `sdss_hal-1.2.0/src/hal/helpers/apogee.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2021-12-16
 # @Filename: apogee.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
+import asyncio
 import enum
 
 from typing import TYPE_CHECKING
 
+from sdsstools.utils import cancel_task
+
 from hal import config
 from hal.exceptions import HALError
 
-from . import HALHelper
+from . import SpectrographHelper
 
 
 if TYPE_CHECKING:
     from hal.actor import HALActor, HALCommandType
 
 
 __all__ = ["APOGEEHelper"]
 
 
-class APOGEEHelper(HALHelper):
+class APOGEEHelper(SpectrographHelper):
     """APOGEE instrument helper."""
 
     name = "apogee"
 
     def __init__(self, actor: HALActor):
         super().__init__(actor)
 
@@ -194,30 +197,35 @@
         )
 
         return dither_command
 
     def is_exposing(self):
         """Returns `True` if APOGEE is exposing or stopping."""
 
-        exposure_state = self.actor.models["apogee"]["exposureState"]
-
-        if exposure_state.value is None or None in exposure_state.value:
-            raise ValueError("Unknown APOGEE exposure state.")
+        state = self.get_exposure_state()
 
-        state = exposure_state.value[0].lower()
         if state in ["exposing", "stopping"]:
             return True
         else:
             return False
 
+    def get_exposure_state(self) -> str | None:
+
+        exposure_state = self.actor.models["apogee"]["exposureState"]
+
+        if exposure_state.value is None or None in exposure_state.value:
+            raise ValueError("Unknown APOGEE exposure state.")
+
+        return exposure_state.value[0].lower()
+
     async def expose(
         self,
         command: HALCommandType,
         exp_time: float,
-        exp_type: str = "dark",
+        exp_type: str = "object",
         dither_position: str | None = None,
     ):
         """Exposes APOGEE.
 
         Parameters
         ----------
         command
@@ -278,22 +286,27 @@
             dither_sequence = current.upper()
             dither_sequence = "AB" if dither_sequence == "A" else "BA"
         else:
             dither_sequence = dither_sequence.upper()
             if dither_sequence not in ["AB", "BA", "AA", "BB"]:
                 raise HALError(f"Invalid dither sequence {dither_sequence}.")
 
+        self._exposure_time_remaining = exp_time * len(dither_sequence)
+        self._exposure_time_remaining_timer = asyncio.create_task(self._timer())
+
         for dither_position in dither_sequence:
             await self.expose(
                 command,
                 exp_time,
                 exp_type=exp_type,
                 dither_position=dither_position,
             )
 
+        await cancel_task(self._exposure_time_remaining_timer)
+
 
 class APOGEEGangHelper:
     """Helper for the APOGEE gang connector."""
 
     def __init__(self, actor: HALActor):
         self.actor = actor
         self.flag: APOGEEGang = APOGEEGang.UNKNWON
```

### Comparing `sdss_hal-1.1.9/src/hal/helpers/boss.py` & `sdss_hal-1.2.0/src/hal/helpers/boss.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 
 from __future__ import annotations
 
 import asyncio
 
 from typing import TYPE_CHECKING
 
+from sdsstools.utils import cancel_task
+
 from hal import config
 from hal.exceptions import HALError
 
-from . import HALHelper
+from . import SpectrographHelper
 
 
 if TYPE_CHECKING:
     from hal.actor import HALActor, HALCommandType
 
 
 __all__ = ["BOSSHelper"]
 
 
-class BOSSHelper(HALHelper):
+class BOSSHelper(SpectrographHelper):
     """Control for BOSS spectrograph."""
 
     __readout_pending: bool = False
     __readout_task: asyncio.Task | None = None
 
     name = "boss"
 
@@ -104,19 +106,22 @@
         exp_time: float = 0.0,
         exp_type: str = "science",
         readout: bool = True,
         read_async: bool = False,
     ):
         """Exposes BOSS. If ``readout=False``, does not read the exposure."""
 
-        if self.readout_pending is not False:
+        if self.readout_pending is not False or self.is_exposing():
             raise HALError(
                 "Cannot expose. The camera is exposing or a readout is pending."
             )
 
+        self._exposure_time_remaining = exp_time
+        self._exposure_time_remaining_timer = asyncio.create_task(self._timer())
+
         if self.actor.observatory == "APO":
             await self._expose_boss_icc(
                 command,
                 exp_time=exp_time,
                 exp_type=exp_type,
                 readout=readout,
                 read_async=read_async,
@@ -126,14 +131,16 @@
                 command,
                 exp_time=exp_time,
                 exp_type=exp_type,
                 readout=readout,
                 read_async=read_async,
             )
 
+        await cancel_task(self._exposure_time_remaining_timer)
+
     async def _expose_boss_icc(
         self,
         command: HALCommandType,
         exp_time: float = 0.0,
         exp_type: str = "science",
         readout: bool = True,
         read_async: bool = False,
```

### Comparing `sdss_hal-1.1.9/src/hal/helpers/cherno.py` & `sdss_hal-1.2.0/src/hal/helpers/cherno.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/helpers/ffs.py` & `sdss_hal-1.2.0/src/hal/helpers/ffs.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/helpers/jaeger.py` & `sdss_hal-1.2.0/src/hal/helpers/jaeger.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from collections import deque
 from dataclasses import dataclass
 
 from typing import TYPE_CHECKING
 
 from sdssdb.peewee.sdss5db import targetdb
 
+from hal import config
 from hal.helpers import HALHelper
 
 
 if TYPE_CHECKING:
     from hal.actor import HALActor, HALCommandType
 
 
@@ -32,27 +33,30 @@
 
     actor: HALActor
     design_id: int
     configuration_id: int | None = None
     field_id: int | None = None
     cloned: bool = False
     preloaded: bool = False
+    loaded: bool = False
     is_rm_field: bool = False
     new_field: bool = True
     observed: bool = False
     goto_complete: bool = False
     design_mode: str | None = None
 
     def __post_init__(self):
         if self.design_id is None or self.design_id < 0:
             return
 
         if self.check_db():
             self.set_field_id()
 
+        assert self.loaded or self.preloaded
+
     def warn(self, message: str):
         """Warns users."""
 
         assert self.actor
         self.actor.write("w", error=message)
 
     def check_db(self):
@@ -94,14 +98,31 @@
             elif self.design_mode in ["dark_monit", "dark_rm"]:
                 self.is_rm_field = True
         except Exception as err:
             self.warn(f"Failed determining RM/AQMES: {err}")
 
         return
 
+    def get_goto_field_stages(self):
+        """Returns the list of goto-field stages depending on the design mode."""
+
+        observatory = self.actor.observatory
+        goto_auto_mode_stages = config["macros"]["goto_field"]["auto_mode"]
+
+        if self.cloned is True:
+            stages = goto_auto_mode_stages["cloned_stages"][observatory]
+        elif self.new_field is False:
+            stages = goto_auto_mode_stages["repeat_field_stages"][observatory]
+        elif self.is_rm_field is True:
+            stages = goto_auto_mode_stages["rm_field_stages"][observatory]
+        else:
+            stages = goto_auto_mode_stages["new_field_stages"][observatory]
+
+        return stages
+
 
 class JaegerHelper(HALHelper):
     """Helper to interact with jaeger."""
 
     name = "jaeger"
 
     def __init__(self, actor: HALActor):
@@ -119,24 +140,55 @@
         self.model["design_preloaded"].register_callback(self._design_preloaded)
 
     def warn(self, message: str):
         """Warns users."""
 
         self.actor.write("w", error=message)
 
+    async def is_folded(self, command: HALCommandType):
+        """Checks whether the FPS is folded."""
+
+        cmd = await self._send_command(
+            command,
+            "jaeger",
+            "unwind --status",
+            raise_on_fail=True,
+        )
+
+        return cmd.replies.get("folded")[0]
+
+    async def unwind(self, command: HALCommandType):
+        """Unwinds the FPS."""
+
+        cmd = await self._send_command(
+            command,
+            "jaeger",
+            "unwind",
+            raise_on_fail=False,
+        )
+
+        if cmd.status.did_fail:
+            self.warn("Failed unwinding the FPS.")
+            return False
+
+        return True
+
     async def load_from_queue(
         self,
         command: HALCommandType,
         preload: bool = False,
         extra_epoch_delay: float = 0.0,
     ):
         """(Pre-)Loads a design from the queue."""
 
         verb = "preload" if preload else "load"
 
+        if extra_epoch_delay < 0:
+            extra_epoch_delay = 0
+
         cmd = await self._send_command(
             command,
             "jaeger",
             f"configuration {verb} --extra-epoch-delay {extra_epoch_delay}",
             raise_on_fail=False,
         )
 
@@ -172,29 +224,29 @@
         is_cloned = key.value[9]
 
         # First check if we had already preloaded this design.
         if self.preloaded and self.preloaded.design_id == design_id:
             new = self.preloaded
 
             new.preloaded = False
+            new.loaded = True
             new.configuration_id = configuration_id
             new.cloned = is_cloned
         else:
             new = Configuration(
                 self.actor,
                 design_id,
                 configuration_id=configuration_id,
                 field_id=field_id,
                 cloned=is_cloned,
                 preloaded=False,
+                loaded=True,
             )
 
-        user_message = (
-            f"Found configuration with design_id={design_id}, field_id={field_id}."
-        )
+        user_message = f"New configuration: design_id={design_id}, field_id={field_id}."
 
         if current:
             if current.goto_complete and current.field_id == new.field_id:
                 new.new_field = False
                 user_message += " This is a repeat field design."
 
             self._previous.append(current)
```

### Comparing `sdss_hal-1.1.9/src/hal/helpers/lamps.py` & `sdss_hal-1.2.0/src/hal/helpers/lamps.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/helpers/overhead.py` & `sdss_hal-1.2.0/src/hal/helpers/overhead.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/helpers/scripts.py` & `sdss_hal-1.2.0/src/hal/helpers/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/helpers/tcc.py` & `sdss_hal-1.2.0/src/hal/helpers/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/macros/__init__.py` & `sdss_hal-1.2.0/src/hal/macros/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,12 +41,13 @@
 
             obj = getattr(mod, objname)
             if inspect.isclass(obj) and issubclass(obj, Macro) and obj != Macro:
                 all_macros.append(obj())
                 locals().update({objname: obj})
 
     except Exception as ee:
+        raise
         warnings.warn(f"cannot import file {f_}: {ee}", HALUserWarning)
 
 os.chdir(cwd)
 
 __all__ = ["all_macros", "Macro"]
```

### Comparing `sdss_hal-1.1.9/src/hal/macros/apogee_dome_flat.py` & `sdss_hal-1.2.0/src/hal/macros/apogee_dome_flat.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/src/hal/macros/expose.py` & `sdss_hal-1.2.0/src/hal/macros/expose.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         # Information about each exposure to take.
         self.apogee_exps: list[ApogeeExposure] = []
         self.boss_exps: list[BossExposure] = []
 
         self._apogee_exp_start_time: float = 0
         self._boss_exp_start_time: float = 0
 
+        self.etr: float = 0.0
+
         self.interval: float = 10
         self._monitor_task: asyncio.Task | None = None
 
         self.params: ExposeParameters = ExposeParameters()
         self.update_params(**opts)
 
         self.refresh()
@@ -409,14 +411,16 @@
                 etr -= exp_elapsed
                 if etr < 0:
                     etr = 0
             state_boss["etr"] = int(round(etr))
 
             self.macro.command.debug(exposure_state_boss=list(state_boss.values()))
 
+        self.etr = max(state_apogee["etr"], state_boss["etr"])
+
 
 class ExposeMacro(Macro):
     """Takes a science exposure with APOGEE and/or BOSS."""
 
     name = "expose"
 
     __PRECONDITIONS__ = ["prepare"]
@@ -504,14 +508,19 @@
                         open=True,
                         shutter="fpi",
                     )
                 )
 
         await asyncio.gather(*tasks)
 
+        # If we are about to expose that means the goto-field is done, so let's mark it.
+        # This is useful in cases where the goto failed and it was manually completed.
+        if self.helpers.jaeger.configuration:
+            self.helpers.jaeger.configuration.goto_complete = True
+
         # Tell the helper that we're about to start exposing.
         await self.expose_helper.start()
 
     async def expose_boss(self):
         """Exposes BOSS."""
 
         # Just in case there's a readout pending from some previous error. Although
@@ -588,14 +597,17 @@
 
         if self.helpers.boss.is_exposing():
             if self.helpers.boss.is_reading():
                 self.command.info("BOSS is reading.")
             else:
                 self.command.warning("BOSS exposure is running. Not cancelling it.")
 
+        if not self.failed and not self.cancelled and self.helpers.jaeger.configuration:
+            self.helpers.jaeger.configuration.observed = True
+
     async def _pause(self):
         """Pauses the execution of the macro."""
 
         if self._pause_event.is_set():
             self._pause_event.clear()
             self.command.warning("Pausing execution of the expose macro.")
             self.command.debug(expose_is_paused=True)
```

### Comparing `sdss_hal-1.1.9/src/hal/macros/goto_field.py` & `sdss_hal-1.2.0/src/hal/macros/goto_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,22 @@
         raise NotImplementedError()
 
     async def reconfigure(self):
         """Reconfigures the FPS."""
 
         self.command.info("Reconfiguring FPS array.")
 
-        # This is always safe. If it's already folded jaeger will return immediately.
-        await self.send_command("jaeger", "configuration reverse")
+        if not (await self.helpers.jaeger.is_folded(self.command)):
+            try:
+                await self.send_command("jaeger", "configuration reverse")
+            except MacroError:
+                self.command.warning("Reverse trajectory failed. Will try to unwind.")
+
+                if not (await self.helpers.jaeger.unwind(self.command)):
+                    raise MacroError("Failed unwindind the FPS array.")
 
         await self.send_command("jaeger", "configuration execute")
 
     async def fvc(self):
         """Run the FVC loop."""
 
         if "slew" in self.flat_stages and self.observatory == "APO":
@@ -389,15 +395,15 @@
         The stage at which we mark the configuration as ``goto_complete`` depends
         on what stages we are running, but it is always after the last stage
         before acquisition.
 
         """
 
         for stage in self.flat_stages:
-            if stage == "acquire" or stage == "guide":
+            if stage in ["acquire", "guide", "cleanup"]:
                 continue
             if not self.is_stage_done(stage):
                 return False
 
         return True
 
     async def _close_ffs(self, wait: bool = True):
```

### Comparing `sdss_hal-1.1.9/src/hal/macros/macro.py` & `sdss_hal-1.2.0/src/hal/macros/macro.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,26 +117,27 @@
 
         self._running_task: asyncio.Task | None = None
         self._running_event = asyncio.Event()
         self._running_event.set()  # Won't unset until the macro is actually running.
 
     def __repr__(self):
         stages = flatten(self.stages)
-        return f"<{self.__class__.__name__} (name={self.name}, stages={stages})>"
+        return f"<{self.__class__.__name__} (name={self.name!r}, stages={stages})>"
 
     def _reset_internal(self, **opts):
         """Internal reset method that can be overridden by the subclasses."""
 
         pass
 
     def reset(
         self,
         command: HALCommandType,
         reset_stages: Optional[list[StageType]] = None,
         force: bool = False,
+        reset_config: bool = True,
         **opts,
     ):
         """Resets stage status.
 
         ``reset_stages`` is a list of stages to be executed when calling `.run`.
         If ``reset_stages`` is a list of string and ``force=False``, the reset
         stages are rearranged according to the original ``__STAGES__`` order,
@@ -189,15 +190,17 @@
 
         if len(self.stages) == 0:
             raise MacroError("No stages found.")
 
         self.flat_stages = flatten(self.stages)
 
         # Reload the config and update it with custom options for this run.
-        self.config = defaultdict(lambda: None, self._base_config.copy())
+        if reset_config:
+            self.config = defaultdict(lambda: None, self._base_config.copy())
+
         self.config.update(
             {k: v for k, v in opts.items() if k not in self.config or v is not None}
         )
 
         self.failed = False
         self.cancelled = False
 
@@ -255,14 +258,25 @@
         if is_running:
             if not self._running_event.is_set():
                 self._running_event.set()
             self._running_event.clear()
         else:
             self._running_event.set()
 
+    def is_cancelling(self):
+        """Returns ``True`` if the macro is cancelling."""
+
+        if not self.running or (self.cancelled or self.failed):
+            return False
+
+        if self.has_status(self.flat_stages, StageStatus.CANCELLING):
+            return True
+
+        return False
+
     def set_stage_status(
         self,
         stages: StageType,
         status: StageStatus,
         output: bool = True,
     ):
         """Set the stage status and inform the actor."""
```

### Comparing `sdss_hal-1.1.9/src/hal/macros/test_macro.py` & `sdss_hal-1.2.0/src/hal/macros/test_macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.9/PKG-INFO` & `sdss_hal-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-hal
-Version: 1.1.9
+Version: 1.2.0
 Summary: High-level observing tool for SDSS-V (replaces SOP)
 Home-page: https://github.com/sdss/hal
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
@@ -20,17 +20,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: numpy (>=1.22.1,<2.0.0)
 Requires-Dist: peewee (>=3.17.0,<4.0.0)
-Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
+Requires-Dist: sdss-clu (>=2.2.7,<3.0.0)
 Requires-Dist: sdssdb (>=0.8.3)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Project-URL: Documentation, https://sdss-hal.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/hal
 Description-Content-Type: text/markdown
 
 # HAL
 
 ![Versions](https://img.shields.io/badge/python->3.9-blue)
```

