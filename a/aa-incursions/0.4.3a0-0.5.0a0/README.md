# Comparing `tmp/aa_incursions-0.4.3a0.tar.gz` & `tmp/aa_incursions-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_incursions-0.4.3a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_incursions-0.5.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_incursions-0.4.3a0.tar` & `aa_incursions-0.5.0a0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1069 2024-05-21 05:29:40.029332 aa_incursions-0.4.3a0/LICENSE
--rw-r--r--   0        0        0     2530 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/README.md
--rw-r--r--   0        0        0       85 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/incursions/__init__.py
--rw-r--r--   0        0        0     1200 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/incursions/admin.py
--rw-r--r--   0        0        0      382 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/incursions/app_settings.py
--rw-r--r--   0        0        0      299 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/incursions/apps.py
--rw-r--r--   0        0        0      133 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/incursions/auth_hooks.py
--rw-r--r--   0        0        0     4775 2024-05-21 05:29:40.030332 aa_incursions-0.4.3a0/incursions/cogs/incursions.py
--rw-r--r--   0        0        0  1705544 2024-05-21 05:29:40.033332 aa_incursions-0.4.3a0/incursions/data.everef.net/incursions/history/backfills/eve-incursions-de-2023-10-12.json.xz
--rw-r--r--   0        0        0      903 2024-05-21 05:29:40.034332 aa_incursions-0.4.3a0/incursions/data.everef.net/readme.md
--rw-r--r--   0        0        0     5677 2024-05-21 05:29:40.034332 aa_incursions-0.4.3a0/incursions/everef.py
--rw-r--r--   0        0        0    59780 2024-05-21 05:29:40.034332 aa_incursions-0.4.3a0/incursions/fixtures/Incursion.json.xz
--rw-r--r--   0        0        0  1444644 2024-05-21 05:29:40.037332 aa_incursions-0.4.3a0/incursions/fixtures/IncursionInfluence.json.xz
--rw-r--r--   0        0        0     9653 2024-05-21 05:29:40.037332 aa_incursions-0.4.3a0/incursions/helpers.py
--rw-r--r--   0        0        0      400 2024-05-21 05:29:40.037332 aa_incursions-0.4.3a0/incursions/locale/da_DK/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2596 2024-05-21 05:29:40.037332 aa_incursions-0.4.3a0/incursions/locale/da_DK/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      384 2024-05-21 05:29:40.037332 aa_incursions-0.4.3a0/incursions/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2580 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2884 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      424 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2620 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2646 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2634 2024-05-21 05:29:40.038332 aa_incursions-0.4.3a0/incursions/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2575 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2587 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      523 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2719 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2805 2024-05-21 05:29:40.039332 aa_incursions-0.4.3a0/incursions/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      399 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2595 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4033 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0001_initial.py
--rw-r--r--   0        0        0     1944 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0002_remove_incursion_influence_and_more.py
--rw-r--r--   0        0        0      831 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0003_focus.py
--rw-r--r--   0        0        0      523 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0004_alter_focus_incursion.py
--rw-r--r--   0        0        0      458 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0005_incursioninfluence_uniqueincursioninfluencelogtimestamp.py
--rw-r--r--   0        0        0      902 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0006_alter_incursion_infested_solar_systems_and_more.py
--rw-r--r--   0        0        0      455 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/migrations/0007_alter_focus_options.py
--rw-r--r--   0        0        0        0 2024-05-21 05:29:40.081332 aa_incursions-0.4.3a0/incursions/migrations/__init__.py
--rw-r--r--   0        0        0     6621 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/models.py
--rw-r--r--   0        0        0      652 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/providers.py
--rw-r--r--   0        0        0     1462 2024-05-21 05:29:40.040332 aa_incursions-0.4.3a0/incursions/signals.py
--rw-r--r--   0        0        0    87001 2024-05-21 05:29:40.041332 aa_incursions-0.4.3a0/incursions/static_data.py
--rw-r--r--   0        0        0   881823 2024-05-21 05:29:40.043332 aa_incursions-0.4.3a0/incursions/swagger.json
--rw-r--r--   0        0        0     5492 2024-05-21 05:29:40.044332 aa_incursions-0.4.3a0/incursions/tasks.py
--rw-r--r--   0        0        0     2195 2024-05-21 05:29:40.044332 aa_incursions-0.4.3a0/pyproject.toml
--rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 aa_incursions-0.4.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-26 11:40:05.508489 aa_incursions-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     2530 2024-05-26 11:40:05.508489 aa_incursions-0.5.0a0/README.md
+-rw-r--r--   0        0        0       85 2024-05-26 11:40:05.508489 aa_incursions-0.5.0a0/incursions/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-26 11:40:05.509489 aa_incursions-0.5.0a0/incursions/admin.py
+-rw-r--r--   0        0        0      382 2024-05-26 11:40:05.509489 aa_incursions-0.5.0a0/incursions/app_settings.py
+-rw-r--r--   0        0        0      299 2024-05-26 11:40:05.509489 aa_incursions-0.5.0a0/incursions/apps.py
+-rw-r--r--   0        0        0      133 2024-05-26 11:40:05.509489 aa_incursions-0.5.0a0/incursions/auth_hooks.py
+-rw-r--r--   0        0        0     4801 2024-05-26 11:40:05.509489 aa_incursions-0.5.0a0/incursions/cogs/incursions.py
+-rw-r--r--   0        0        0  1705544 2024-05-26 11:40:05.513489 aa_incursions-0.5.0a0/incursions/data.everef.net/incursions/history/backfills/eve-incursions-de-2023-10-12.json.xz
+-rw-r--r--   0        0        0      903 2024-05-26 11:40:05.513489 aa_incursions-0.5.0a0/incursions/data.everef.net/readme.md
+-rw-r--r--   0        0        0     5677 2024-05-26 11:40:05.513489 aa_incursions-0.5.0a0/incursions/everef.py
+-rw-r--r--   0        0        0    59780 2024-05-26 11:40:05.514489 aa_incursions-0.5.0a0/incursions/fixtures/Incursion.json.xz
+-rw-r--r--   0        0        0  1444644 2024-05-26 11:40:05.516489 aa_incursions-0.5.0a0/incursions/fixtures/IncursionInfluence.json.xz
+-rw-r--r--   0        0        0    10043 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/helpers.py
+-rw-r--r--   0        0        0      400 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/locale/da_DK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2596 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/locale/da_DK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      384 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2580 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2884 2024-05-26 11:40:05.517489 aa_incursions-0.5.0a0/incursions/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      424 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2620 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2646 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2634 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2575 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2024-05-26 11:40:05.518489 aa_incursions-0.5.0a0/incursions/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2587 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      523 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2719 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2805 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      399 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2595 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4033 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1944 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py
+-rw-r--r--   0        0        0      831 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/migrations/0003_focus.py
+-rw-r--r--   0        0        0      523 2024-05-26 11:40:05.519489 aa_incursions-0.5.0a0/incursions/migrations/0004_alter_focus_incursion.py
+-rw-r--r--   0        0        0      458 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/migrations/0005_incursioninfluence_uniqueincursioninfluencelogtimestamp.py
+-rw-r--r--   0        0        0      902 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/migrations/0006_alter_incursion_infested_solar_systems_and_more.py
+-rw-r--r--   0        0        0      455 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/migrations/0007_alter_focus_options.py
+-rw-r--r--   0        0        0        0 2024-05-26 11:40:05.553488 aa_incursions-0.5.0a0/incursions/migrations/__init__.py
+-rw-r--r--   0        0        0     6605 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/models.py
+-rw-r--r--   0        0        0      652 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/providers.py
+-rw-r--r--   0        0        0     1462 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/signals.py
+-rw-r--r--   0        0        0    87001 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/static_data.py
+-rw-r--r--   0        0        0     6748 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/incursions/tasks.py
+-rw-r--r--   0        0        0     2195 2024-05-26 11:40:05.520489 aa_incursions-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 aa_incursions-0.5.0a0/PKG-INFO
```

### Comparing `aa_incursions-0.4.3a0/LICENSE` & `aa_incursions-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/README.md` & `aa_incursions-0.5.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/admin.py` & `aa_incursions-0.5.0a0/incursions/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 @admin.register(IncursionsConfig)
 class IncursionsConfigAdmin(admin.ModelAdmin):
     filter_horizontal = ["status_webhooks", ]
 
 
 @admin.register(Incursion)
 class IncursionAdmin(admin.ModelAdmin):
-    list_display = ["constellation", "state", "established_timestamp"]
-    list_filter = ["state", ]
+    list_display = ["constellation", "state", "established_timestamp",
+                    "mobilizing_timestamp", "withdrawing_timestamp", "ended_timestamp"]
+    list_filter = ["state", "has_boss"]
     filter_horizontal = ["infested_solar_systems", ]
 
 
 @admin.register(Webhook)
 class WebhookAdmin(admin.ModelAdmin):
     list_display = ("name", "url")
```

### Comparing `aa_incursions-0.4.3a0/incursions/cogs/incursions.py` & `aa_incursions-0.5.0a0/incursions/cogs/incursions.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,16 @@
 
     @incursion_commands.command(name="set_focus", description="Set the current Focus", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def focus_set(
         self, ctx,
         incursion=Option(str, "Constellation", autocomplete=search_incursion_active),
     ):
         focus = Focus.get_solo()
-        focus.incursion_id = Incursion.objects.exclude(state=Incursion.States.ENDED).get(constellation__name__icontains=incursion)
+        focus.incursion_id = Incursion.objects.exclude(
+            state=Incursion.States.ENDED).get(constellation__name__icontains=incursion)
         focus.save()
         return await ctx.respond("Focus Set")
 
     @incursion_commands.command(name="incursions", description="List active incursions", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def incursions(
         self, ctx,
     ):
@@ -90,15 +91,16 @@
         return await ctx.respond(incursion_string)
 
     @incursion_commands.command(name="incursion_detail", description="Status of a specific incursion", guild_ids=[int(settings.DISCORD_GUILD_ID)])
     async def incursion_detail(
         self, ctx,
         incursion=Option(str, "Constellation", autocomplete=search_incursion_active),
     ):
-        incursion_obj = Incursion.objects.exclude(state=Incursion.States.ENDED).get(constellation__name__icontains=incursion)
+        incursion_obj = Incursion.objects.exclude(state=Incursion.States.ENDED).get(
+            constellation__name__icontains=incursion)
         incursion_detail_string = f"""
             {incursion_obj.constellation.name} ({incursion_obj.state})
             Established: {incursion_obj.established_timestamp}
             Mobilized: {incursion_obj.mobilizing_timestamp}
             Withdrawing:{incursion_obj.withdrawing_timestamp}
             Boss Spotted: {incursion_obj.has_boss}
             Influence: {incursion_obj.influence}
```

### Comparing `aa_incursions-0.4.3a0/incursions/data.everef.net/incursions/history/backfills/eve-incursions-de-2023-10-12.json.xz` & `aa_incursions-0.5.0a0/incursions/data.everef.net/incursions/history/backfills/eve-incursions-de-2023-10-12.json.xz`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/data.everef.net/readme.md` & `aa_incursions-0.5.0a0/incursions/data.everef.net/readme.md`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/everef.py` & `aa_incursions-0.5.0a0/incursions/everef.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/fixtures/Incursion.json.xz` & `aa_incursions-0.5.0a0/incursions/fixtures/Incursion.json.xz`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/fixtures/IncursionInfluence.json.xz` & `aa_incursions-0.5.0a0/incursions/fixtures/IncursionInfluence.json.xz`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/helpers.py` & `aa_incursions-0.5.0a0/incursions/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     embed.timestamp = datetime.now()
     return embed
 
 
 def embed_established(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.green()
-    embed.title = f"New {incursion.security_string}: {incursion.constellation.name}"
+    embed.title = f"New {incursion.security_string}: {incursion.constellation.eve_region.name}/{incursion.constellation.name}"
     embed.description = "PSA: Create and use an Insta-Dock Bookmark when warping to the new dockup. Scout the route ahead including the dockup station."
     embed.add_field(
         name="Region",
         value=f"[{incursion.constellation.eve_region.name}]({incursion.constellation.eve_region.profile_url})",
         inline=True)
     embed.add_field(
         name="Constellation",
@@ -52,30 +52,34 @@
         value="".join(incursion_constellations[incursion.constellation.name]["Vanguards"]),
         inline=True)
     # newline
     embed.add_field(name="Stations in HQ",
                     value=f"{ EveSolarSystem.objects.get(name=incursion_constellations[incursion.constellation.name]['Headquarter']).eve_stations.count() }", inline=True)
     embed.add_field(name="HS Island?",
                     value=f"{incursion.is_island}", inline=True)
-    embed.add_field(name="Jumps from last HQ",
-                    value=f"{route_length(incursion.staging_solar_system.id, Focus.get_solo().incursion.staging_solar_system.id)}", inline=True)
+    try:
+        embed.add_field(name=f"Jumps from last HQ {Focus.get_solo().incursion.staging_solar_system.name}",
+                        value=f"{route_length(incursion.staging_solar_system.id, Focus.get_solo().incursion.staging_solar_system.id)}", inline=True)
+    except AttributeError:
+        # Focus isnt Set, dont stress
+        pass
     # newline
     embed.add_field(name="Suggested Dockup",
                     value="Not Implemented", inline=True)
     embed.add_field(name="Edencom In Spawn",
                     value="Not Implemented", inline=True)
     embed.add_field(name="Trigs In Spawn",
                     value="Not Implemented", inline=True)
     return embed
 
 
 def embed_established_addendum(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.blue()
-    embed.title = f"{incursion.constellation.name}"
+    embed.title = f"{incursion.security_string}: {incursion.constellation.eve_region.name}/{incursion.constellation.name}"
     embed.add_field(name="Spawn Time",
                     value=f"<t:{ int(incursion.established_timestamp.timestamp()) }:R>", inline=True)
     embed.add_field(name="Despawn Window Starts",
                     value=f"<t:{ int((incursion.established_timestamp + timedelta(days=4)).timestamp()) }:R>", inline=True)
     embed.add_field(name="Despawn Window Ends",
                     value=f"<t:{ int((incursion.established_timestamp + timedelta(days=8)).timestamp()) }:R>", inline=True)
     # newline
@@ -106,15 +110,15 @@
         pass
     return embed
 
 
 def embed_mobilizing(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.yellow()
-    embed.title = f"Mobilizing {incursion.security_string}: {incursion.constellation.name}"
+    embed.title = f"Mobilizing {incursion.security_string}: {incursion.constellation.eve_region.name}/{incursion.constellation.name}"
     embed.add_field(name="Estimated Withdrawing Time",
                     value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=2)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Despawn Time",
                     value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3)).timestamp()) }:R>", inline=False)
     try:
         embed.add_field(name="Max Spawn Stats",
                         value=f'''
@@ -145,15 +149,15 @@
     # Estimated Respawn Window Closes
     # Monday, 26 June 2023 09:37 (in 4 days)
 
 
 def embed_withdrawing(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.red()
-    embed.title = f"Withdrawing {incursion.security_string}: {incursion.constellation.name}"
+    embed.title = f"Withdrawing {incursion.security_string}: {incursion.constellation.eve_region.name}/{incursion.constellation.name}"
     embed.add_field(name="Despawn Before",
                     value=f"<t:{ int((incursion.withdrawing_timestamp + timedelta(days=1)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Respawn Window Opens",
                     value=f"<t:{ int((incursion.withdrawing_timestamp + timedelta(days=1, hours=12)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Respawn Window Closes",
                     value=f"<t:{ int((incursion.withdrawing_timestamp + timedelta(days=1, hours=36)).timestamp()) }:R>", inline=False)
     return embed
@@ -168,15 +172,15 @@
     # Monday, 26 June 2023 09:40 (2 hours ago)
 
 
 def embed_ended(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.red()
     embed.description = "The next spawn will occur in 12-36 hours."
-    embed.title = f"Ended {incursion.security_string}: {incursion.constellation.name}"
+    embed.title = f"Ended {incursion.security_string}: {incursion.constellation.eve_region.name}/{incursion.constellation.name}"
     embed.add_field(name="Spawn Window Opens",
                     value=f"<t:{ int((incursion.ended_timestamp + timedelta(days=1)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Spawn Window Closes",
                     value=f"<t:{ int((incursion.ended_timestamp + timedelta(days=1, hours=12)).timestamp()) }:R>", inline=False)
     try:
         embed.add_field(name="Max Spawn Stats",
                         value=f'''
```

### Comparing `aa_incursions-0.4.3a0/incursions/locale/da_DK/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/da_DK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/de/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/en/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/es/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/fr_FR/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/it_IT/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/ja/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/ko_KR/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/ru/LC_MESSAGES/django.mo` & `aa_incursions-0.5.0a0/incursions/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/ru/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/uk/LC_MESSAGES/django.mo` & `aa_incursions-0.5.0a0/incursions/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/uk/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_incursions-0.5.0a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/migrations/0001_initial.py` & `aa_incursions-0.5.0a0/incursions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/migrations/0002_remove_incursion_influence_and_more.py` & `aa_incursions-0.5.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/migrations/0003_focus.py` & `aa_incursions-0.5.0a0/incursions/migrations/0003_focus.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/migrations/0004_alter_focus_incursion.py` & `aa_incursions-0.5.0a0/incursions/migrations/0004_alter_focus_incursion.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/migrations/0006_alter_incursion_infested_solar_systems_and_more.py` & `aa_incursions-0.5.0a0/incursions/migrations/0006_alter_incursion_infested_solar_systems_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/models.py` & `aa_incursions-0.5.0a0/incursions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         I Think this used to be used for Trig Incursions etc, leaving the option in place to expand it later
         """
         INCURSION = 'Incursion', _("Sansha Incursion")
 
     constellation = models.ForeignKey(EveConstellation, verbose_name=_(
         "The constellation id in which this incursion takes place"), on_delete=models.CASCADE)
     faction = models.ForeignKey(EveFactionInfo, verbose_name=_(
-        "The attacking faction’s id"), on_delete=models.CASCADE)
+        "The attacking Faction"), on_delete=models.CASCADE)
     has_boss = models.BooleanField(_("Whether the final encounter has boss or not"), default=False)
     infested_solar_systems = models.ManyToManyField(EveSolarSystem, verbose_name=_(
         "A list of infested solar system ids that are a part of this incursion"), related_name="+")
     staging_solar_system = models.ForeignKey(EveSolarSystem, verbose_name=_(
         "Staging solar system for this incursion"), on_delete=models.CASCADE, related_name="+")
     state = models.CharField(
         _("The state of this incursion"),
@@ -96,15 +96,15 @@
         except Exception:
             # wtf
             return True  # WHY NOT
 
     @property
     def influence(self) -> float:
         try:
-            IncursionInfluence.objects.filter(incursion=self).order_by("timestamp").last().influence
+            IncursionInfluence.objects.filter(incursion=self).latest("timestamp").influence
         except Exception:
             return float(0)
 
 
 class IncursionInfluence(models.Model):
     incursion = models.ForeignKey(Incursion, verbose_name=_("Incursion"), on_delete=models.CASCADE)
     timestamp = models.DateTimeField(_("Timestamp"), auto_now=False, auto_now_add=False)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_incursions-0.4.3a0/incursions/providers.py` & `aa_incursions-0.5.0a0/incursions/providers.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/signals.py` & `aa_incursions-0.5.0a0/incursions/signals.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/incursions/static_data.py` & `aa_incursions-0.5.0a0/incursions/static_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
     "Miennue": {"Staging": "X-M9ON", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Minotaur": {"Staging": "PXF-RF", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "MK7-AO": {"Staging": "A-3ES3", "Vanguards": ["6-U2M8", "617I-I", "DP34-U", "I0AB-R", "MXYS-8", "XS-XAY"], "Assaults": ["35-RK9", "IIRH-G", "VV-VCR"], "Headquarter": "5-75MB"},
     "MPJW-6": {"Staging": "N-M1A3", "Vanguards": ["3-JCJT", "49-U6U", "5V-BJI", "8QT-H4", "M1BZ-2"], "Assaults": ["4-GJT1", "L3-I3K", "W-IIYI"], "Headquarter": "AO-N1P"},
     "MRC-29": {"Staging": "PKN-NJ", "Vanguards": ["LQ-01M", "NG-M8K", "RV5-TT"], "Assaults": ["K85Y-6"], "Headquarter": "8OYE-Z"},
     "MW49-U": {"Staging": "RXTY-4", "Vanguards": ["2FL-5W", "HG-YEQ", "QSCO-D", "RSE-PT"], "Assaults": ["6A-FUY", "863P-X"], "Headquarter": "ZO-YJZ"},
     "MY-HQD": {"Staging": "QRH-BF", "Vanguards": ["M-NP5O", "WIW-X8", "X-KHRZ"], "Assaults": ["L-EUY2"], "Headquarter": "JL-ZUQ"},
-    "MY-QQI": {"Staging": "Z8-81T", "Vanguards": ["DY-P7Q", "H-RXNZ" ,"XVV-21"], "Assaults": ["ZBP-TP"], "Headquarter": "XD-JW7"},
+    "MY-QQI": {"Staging": "Z8-81T", "Vanguards": ["DY-P7Q", "H-RXNZ", "XVV-21"], "Assaults": ["ZBP-TP"], "Headquarter": "XD-JW7"},
     "MZ-PA2": {"Staging": "52CW-6", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "N-39FI": {"Staging": "UR-E46", "Vanguards": ["VYO-68", "TCAG-3", "TPAR-G"], "Assaults": ["CW9-1Y"], "Headquarter": "MG0-RD"},
     "N-APJ8": {"Staging": "4LJ6-Q", "Vanguards": ["G-QTSD", "MF-PGF", "SAH-AD"], "Assaults": ["KGT3-6"], "Headquarter": "L-ZJLN"},
     "N-K4Q0": {"Staging": "OEY-OR", "Vanguards": ["O1-FTD", "2E-ZR5", "SR-KBB"], "Assaults": ["FDZ4-A", "MR4-MY"], "Headquarter": "Roua"},
     "N-LY4R": {"Staging": "LVL-GZ", "Vanguards": ["FN0-QS", "TTP-2B", "X0-6LH"], "Assaults": ["N7-BIY"], "Headquarter": "F3-8X2"},
     "N-OGI1": {"Staging": "2J-WJY", "Vanguards": ["6-K738", "9-8GBA", "ZXIC-7"], "Assaults": ["KDF-GY", "QBQ-RF"], "Headquarter": "QSM-LM"},
     "N-U2LX": {"Staging": "N-TFXK", "Vanguards": ["33RB-O", "3OAT-Q", "DKUK-G"], "Assaults": ["X-Z4DA"], "Headquarter": "C7Y-7Z"},
```

### Comparing `aa_incursions-0.4.3a0/incursions/tasks.py` & `aa_incursions-0.5.0a0/incursions/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,55 +19,71 @@
 def update_incursions():
     incursions, response = get_incursions_incursions()
     actives = []
     for incursion in incursions:
         actives.append(incursion['constellation_id'])
         try:
             # Get, because i need to do more steps than an update_or_create would let me
+            # This chunk is purely for when incursions change states.
             # Also incursions have no unique id.... wtf ccp
             i = Incursion.objects.get(
                 constellation=EveConstellation.objects.get_or_create_esi(id=incursion['constellation_id'])[0],
                 ended_timestamp__isnull=True)
             if incursion['state'] == "established":
                 # This is still just an established incursion, nothing to act on
                 pass
             elif incursion['state'] == "mobilizing" and i.state != Incursion.States.MOBILIZING:
                 i.mobilizing_timestamp = datetime.datetime.strptime(
                     str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
                 i.state = Incursion.States.MOBILIZING
                 i.save(update_fields=["mobilizing_timestamp", "state"])
-            elif incursion['state'] == "withdrawing " and i.state != Incursion.States.WITHDRAWING:
+            elif incursion['state'] == "withdrawing" and i.state != Incursion.States.WITHDRAWING:
                 i.withdrawing_timestamp = datetime.datetime.strptime(
                     str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
                 i.state = Incursion.States.WITHDRAWING
                 i.save(update_fields=["withdrawing_timestamp", "state"])
             else:
                 # ????
                 pass
-            IncursionInfluence.objects.create(
-                incursion=i,
-                influence=incursion['influence'],
-                timestamp=datetime.datetime.strptime(
-                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
-            )
+            try:
+                IncursionInfluence.objects.create(
+                    incursion=i,
+                    influence=incursion['influence'],
+                    timestamp=datetime.datetime.strptime(
+                        str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc))
+            except IntegrityError:
+                # If we call this task too often cache will return the same influence
+                pass
         except Incursion.DoesNotExist:
-            # Create an Incursion
+            # Create an Incursion, It does not exist.
             i = Incursion.objects.create(
                 constellation=EveConstellation.objects.get_or_create_esi(
                     id=incursion['constellation_id'])[0],
                 faction=EveFactionInfo.objects.get_or_create(
                     faction_id=incursion['faction_id'])[0],
                 has_boss=incursion['has_boss'],
                 staging_solar_system=EveSolarSystem.objects.get_or_create_esi(
                     id=incursion['staging_solar_system_id'])[0],
                 state=incursion['state'],
                 type=incursion['type'],
                 established_timestamp=datetime.datetime.strptime(
                     str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
             )
+            # We need to also set the mobilizing and withdrawing state here
+            # This is purely for new installs, bcoz partially complete incursions
+            if incursion['state'] == "mobilizing":
+                i.mobilizing_timestamp = datetime.datetime.strptime(
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
+                i.save(update_fields=["mobilizing_timestamp"])
+            elif incursion['state'] == "withdrawing ":
+                i.mobilizing_timestamp = datetime.datetime.strptime(
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
+                i.withdrawing_timestamp = datetime.datetime.strptime(
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
+                i.save(update_fields=["withdrawing_timestamp", "mobilizing_timestamp"])
             try:
                 IncursionInfluence.objects.create(
                     incursion=i,
                     influence=incursion['influence'],
                     timestamp=datetime.datetime.strptime(
                         str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc))
             except IntegrityError:
```

### Comparing `aa_incursions-0.4.3a0/pyproject.toml` & `aa_incursions-0.5.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.4.3a0/PKG-INFO` & `aa_incursions-0.5.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-incursions
-Version: 0.4.3a0
+Version: 0.5.0a0
 Summary: AllianceAuth Incursion Tools
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
```

