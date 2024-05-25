# Comparing `tmp/aurum_hikari-0.1.5.3.tar.gz` & `tmp/aurum_hikari-0.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.5.3.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.5.4.tar", max compression
```

## Comparing `aurum_hikari-0.1.5.3.tar` & `aurum_hikari-0.1.5.4.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1080 2024-05-22 10:56:33.061764 aurum_hikari-0.1.5.3/LICENSE
--rw-r--r--   0        0        0     3510 2024-05-22 10:56:33.061764 aurum_hikari-0.1.5.3/README.md
--rw-r--r--   0        0        0      598 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/__init__.py
--rw-r--r--   0        0        0      430 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/_about.py
--rw-r--r--   0        0        0      183 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/client/__init__.py
--rw-r--r--   0        0        0     9303 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/client/client.py
--rw-r--r--   0        0        0      309 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/client/integration.py
--rw-r--r--   0        0        0      366 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     2324 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/message_command.py
--rw-r--r--   0        0        0     5767 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     2720 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/sub_command.py
--rw-r--r--   0        0        0     2402 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/enum/__init__.py
--rw-r--r--   0        0        0      423 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/ext/__init__.py
--rw-r--r--   0        0        0      312 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/ext/plugins/plugin.py
--rw-r--r--   0        0        0     1720 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/ext/plugins/plugin_integration.py
--rw-r--r--   0        0        0     3457 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/ext/plugins/plugin_manager.py
--rw-r--r--   0        0        0      292 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     8344 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3035 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     5738 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1937 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       75 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      456 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/internal/utils/commands.py
--rw-r--r--   0        0        0      360 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/l10n/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      255 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/l10n/localized.py
--rw-r--r--   0        0        0      479 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/l10n/pass_localization_provider.py
--rw-r--r--   0        0        0      207 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/options/__init__.py
--rw-r--r--   0        0        0      299 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/options/choice.py
--rw-r--r--   0        0        0     1715 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/py.typed
--rw-r--r--   0        0        0      147 2024-05-22 10:56:33.065764 aurum_hikari-0.1.5.3/aurum/types.py
--rw-r--r--   0        0        0     2047 2024-05-22 10:56:42.957793 aurum_hikari-0.1.5.3/pyproject.toml
--rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/LICENSE
+-rw-r--r--   0        0        0     3510 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/README.md
+-rw-r--r--   0        0        0      584 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/__main__.py
+-rw-r--r--   0        0        0      563 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/_about.py
+-rw-r--r--   0        0        0      183 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/client/__init__.py
+-rw-r--r--   0        0        0     9439 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/client/client.py
+-rw-r--r--   0        0        0      720 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/client/integration.py
+-rw-r--r--   0        0        0      366 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2324 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     5767 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     2720 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2402 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4226 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     1724 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_integration.py
+-rw-r--r--   0        0        0     3462 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      292 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/includable.py
+-rw-r--r--   0        0        0      220 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     5738 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1937 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/utils/commands.py
+-rw-r--r--   0        0        0      226 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/version.py
+-rw-r--r--   0        0        0      360 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      479 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/options/choice.py
+-rw-r--r--   0        0        0     1715 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/py.typed
+-rw-r--r--   0        0        0      147 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/types.py
+-rw-r--r--   0        0        0     2360 2024-05-25 23:35:30.857595 aurum_hikari-0.1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.4/PKG-INFO
```

### Comparing `aurum_hikari-0.1.5.3/LICENSE` & `aurum_hikari-0.1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/README.md` & `aurum_hikari-0.1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/__init__.py` & `aurum_hikari-0.1.5.4/aurum/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 __all__: Sequence[str] = (
     "Client",
     "MessageCommand",
     "SlashCommand",
     "UserCommand",
     "InteractionContext",
     "LocalizationProviderInterface",
-    "Locale",
     "Localized",
     "LocalizedOr",
     "Option",
     "Choice",
 )
 
 import typing
```

### Comparing `aurum_hikari-0.1.5.3/aurum/client/client.py` & `aurum_hikari-0.1.5.4/aurum/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     from logging import Logger
 
     from hikari.interactions import (
         CommandInteractionOption,
         PartialInteraction,
     )
 
+    from aurum.ext.plugins import PluginManager
     from aurum.includable import Includable
     from aurum.l10n import LocalizationProviderInterface
     from aurum.types import BotT
 
 
 class Client:
     """A wrapper class for the main bot class, designed to work with the Aurum framework and its features.
@@ -82,14 +83,15 @@
                 "or create your own implementation based on the LocalizationProviderInterface."
             )
         else:
             self.add_starting_task(self.l10n.start())
 
         self.bot: BotT = bot
         self.commands: CommandHandler = CommandHandler(bot, self.l10n)
+        self.plugins: PluginManager | None = None
 
         for integration in integrations:
             integration.install(self)
             self.__logger.debug(f"installed integration: {type(integration).__qualname__}")
 
         for event, callback in {
             StartingEvent: self._on_starting,
@@ -118,14 +120,15 @@
         Args:
             coro (Coroutine[None, None, typing.Any]): Any coroutine.
         """
         self._starting_tasks.append(coro)
         self.__logger.debug(f"add starting task: {coro.__qualname__}")
 
     def include(self, includable: typing.Type[Includable]) -> None:
+        """Decorator to include an includable object to client"""
         if issubclass(includable, AppCommand):
             try:
                 instance: AppCommand = includable()  # type: ignore
             except TypeError:
                 raise AurumException("`__init__` of base includable wasn't overrided")
             self.commands.commands[instance.name] = instance
 
@@ -174,23 +177,23 @@
                             )
                 for option in options or ():
                     arguments[option.name] = context.resolve_command_argument(option)
             callback: Callable[..., Coroutine[None, None, typing.Any]] = getattr(
                 command, "callback"
             )
             if isinstance(command, SlashCommand):
-                return await callback(context, **arguments)
-            return await callback(parent_command, context, **arguments)
+                await callback(context, **arguments)
+            await callback(parent_command, context, **arguments)
         if interaction.command_type is CommandType.MESSAGE:
             assert isinstance(command, MessageCommand)
             assert interaction.resolved
-            return await command.callback(
+            await command.callback(
                 context,
                 list(interaction.resolved.messages.values())[0],
             )
         if interaction.command_type is CommandType.USER:
             assert isinstance(command, UserCommand)
             assert interaction.resolved
-            return await command.callback(
+            await command.callback(
                 context,
                 list(interaction.resolved.users.values())[0],
             )
```

### Comparing `aurum_hikari-0.1.5.3/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.5.4/aurum/commands/decorators/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/commands/message_command.py` & `aurum_hikari-0.1.5.4/aurum/commands/message_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/commands/slash_command.py` & `aurum_hikari-0.1.5.4/aurum/commands/slash_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/commands/sub_command.py` & `aurum_hikari-0.1.5.4/aurum/commands/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/commands/user_command.py` & `aurum_hikari-0.1.5.4/aurum/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/ext/plugins/plugin.py` & `aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/ext/plugins/plugin_integration.py` & `aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,10 +43,10 @@
         *,
         base_directory: PathLike[str] | None = None,
     ):
         self.plugin_manager: typing.Type[PluginManager] = plugin_manager
         self.base_directory: Path | None = Path(base_directory) if base_directory else None
 
     def install(self, client: Client) -> None:
-        self.plugins = self.plugin_manager(client.bot, client)
+        client.plugins = self.plugin_manager(client.bot, client)
         if self.base_directory:
-            client.add_starting_task(self.plugins.load_folder(self.base_directory))
+            client.add_starting_task(client.plugins.load_folder(self.base_directory))
```

### Comparing `aurum_hikari-0.1.5.3/aurum/ext/plugins/plugin_manager.py` & `aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         except Exception as exception:
             self.__logger.error(
                 "couldn't load module %s due error", module_name, exc_info=exception
             )
             return None
         return None
 
-    async def load_folder(self, directory: PathLike) -> None:
+    async def load_folder(self, directory: PathLike[str]) -> None:
         """Load plugins from folder"""
         loaded: typing.List[Plugin] = []
         for file in Path(directory).rglob("*.py"):
             plugin: Plugin | None = self.load_plugin_from_file(file)
             if not plugin:
                 return
             plugin.bot = self.bot
```

### Comparing `aurum_hikari-0.1.5.3/aurum/interactions/interaction_context.py` & `aurum_hikari-0.1.5.4/aurum/interactions/interaction_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,46 +12,56 @@
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
 
     from hikari.api import ComponentBuilder
     from hikari.embeds import Embed
     from hikari.files import Resourceish
     from hikari.guilds import PartialRole
-    from hikari.impl import GatewayBot
     from hikari.interactions import (
         CommandInteraction,
         CommandInteractionOption,
         ComponentInteraction,
+        InteractionMember,
     )
     from hikari.messages import Message
     from hikari.snowflakes import SnowflakeishSequence
     from hikari.undefined import UndefinedOr
     from hikari.users import PartialUser
 
     from aurum.client import Client
-    from aurum.l10n import Locale
+    from aurum.types import BotT
 
 
 @dataclass(slots=True, kw_only=True)
 class InteractionContext:
     """Represents a interaction context.
 
     Attributes:
         interaction (CommandInteraction | ComponentInteraction): The interaction.
-        bot (GatewayBot): The instance of the bot.
+        bot (BotT): The instance of the bot.
         client (Client): The client.
-        locale (Locale | None): An Aurum locale for the interaction.
+        locale (typing.Any): An any locale object for the interaction.
     """
 
     interaction: CommandInteraction | ComponentInteraction
 
-    bot: GatewayBot
+    bot: BotT
     client: Client
 
-    locale: Locale | None
+    locale: typing.Any
+
+    @property
+    def user(self) -> PartialUser | None:
+        """User of the interaction"""
+        return self.interaction.user
+
+    @property
+    def member(self) -> InteractionMember | None:
+        """Member of the interaction"""
+        return self.interaction.member
 
     async def defer(
         self, flags: MessageFlag = MessageFlag.NONE, *, ephemeral: bool = False
     ) -> None:
         """Create a deferred response to the interaction.
 
         Note:
@@ -192,7 +202,9 @@
             case OptionType.MENTIONABLE:
                 return self.interaction.resolved.members.get(
                     option.value,
                     self.interaction.resolved.roles.get(option.value),
                 )
             case OptionType.ATTACHMENT:
                 return self.interaction.resolved.attachments.get(option.value)
+            case _:
+                return None
```

### Comparing `aurum_hikari-0.1.5.3/aurum/internal/commands/app_command.py` & `aurum_hikari-0.1.5.4/aurum/internal/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.5.4/aurum/internal/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.5.4/aurum/internal/commands/context_menu_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/internal/utils/commands.py` & `aurum_hikari-0.1.5.4/aurum/internal/utils/commands.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/l10n/localization_provider_interface.py` & `aurum_hikari-0.1.5.4/aurum/l10n/localization_provider_interface.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/aurum/options/option.py` & `aurum_hikari-0.1.5.4/aurum/options/option.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.3/pyproject.toml` & `aurum_hikari-0.1.5.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,14 @@
-# Package
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-
-# Package information
 [tool.poetry]
-packages = [{ include = "aurum" }]
+version = "v0.1.5.4"
 name = "aurum-hikari"
-version = "v0.1.5.3"
-license = "MIT"
-authors = ["stefanlight <64615032+stefanlight8@users.noreply.github.com>"]
+authors = ["stefanlight8 <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible framework for handling commands and components with integrations."
-keywords = [
-    "discord",
-    "hikari",
-    "commands",
-    "components",
-    "command-handler",
-    "component-handler",
-    "integrations",
-]
+readme = "README.md"
+license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -32,44 +16,74 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Communications :: Chat",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-readme = "README.md"
-
+keywords = [
+    "discord",
+    "hikari",
+    "commands",
+    "components",
+    "command-handler",
+    "component-handler",
+    "integrations",
+]
+packages = [{ include = "aurum" }]
+include = ["./VERSION"]
 
 [tool.poetry.urls]
 repository = "https://github.com/ShinshiDevs/aurum-hikari"
 documentation = "https://shinshidevs.github.io/aurum-hikari/"
 "Issue Tracker" = "https://github.com/ShinshiDevs/aurum-hikari/issues"
-# TODO: Add discord later
-
 
-# Package dependencies
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
-hikari = ">2.0.0.dev122"
-
+hikari = ">=2.0.0.dev122"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = ">=1.5.3,<1.7"
-mkdocstrings-python = ">=1.8.0,<1.11"
+
 mkdocs-material = { version = "^9.5.23", extras = ["imaging"] }
-griffe-inherited-docstrings = "^1.0.0"
 mkdocs-material-extensions = "^1.3.1"
 
+mkdocstrings-python = ">=1.8.0,<1.11"
+griffe-inherited-docstrings = "^1.0.0"
 
-# Developers stuff 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.10.0"
 ruff = "^0.4.3"
-
-# Developers stuff: Ruff settings
+black = "^24.4.2"
+pyright = "^1.1.364"
 
 [tool.ruff]
 line-length = 100
 target-version = "py310"
 
-[tool.ruff.lint.per-file-ignores] # borrowed from hikari-lightbulb
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "F405"]
+
+[tool.mypy]
+python_version = "3.10"
+strict = true
+warn_unused_configs = true
+warn_return_any = true
+warn_redundant_casts = true
+namespace_packages = true
+
+[tool.pyright]
+include = ["aurum", "examples"]
+exclude = ["tests"]
+pythonVersion = "3.10"
+typeCheckingMode = "strict"
+reportPrivateUsage = false
+reportImportCycles = false
+
+[tool.black]
+line-length = 100
+target-version = ['py310']
+skip-magic-trailing-comma = true
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `aurum_hikari-0.1.5.3/PKG-INFO` & `aurum_hikari-0.1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: aurum-hikari
-Version: 0.1.5.3
+Version: 0.1.5.4
 Summary: A flexible framework for handling commands and components with integrations.
 License: MIT
 Keywords: discord,hikari,commands,components,command-handler,component-handler,integrations
-Author: stefanlight
+Author: stefanlight8
 Author-email: 64615032+stefanlight8@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: hikari (>2.0.0.dev122)
+Requires-Dist: hikari (>=2.0.0.dev122)
 Project-URL: Issue Tracker, https://github.com/ShinshiDevs/aurum-hikari/issues
 Project-URL: documentation, https://shinshidevs.github.io/aurum-hikari/
 Project-URL: repository, https://github.com/ShinshiDevs/aurum-hikari
 Description-Content-Type: text/markdown
 
 <div align="center">
     <div>
```

