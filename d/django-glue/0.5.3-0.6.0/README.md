# Comparing `tmp/django_glue-0.5.3.tar.gz` & `tmp/django_glue-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_glue-0.5.3.tar", last modified: Thu Apr 25 19:54:19 2024, max compression
+gzip compressed data, was "django_glue-0.6.0.tar", last modified: Sun May 26 15:59:40 2024, max compression
```

## Comparing `django_glue-0.5.3.tar` & `django_glue-0.6.0.tar`

### file list

```diff
@@ -1,146 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-25 19:54:10.000000 django_glue-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-25 19:54:10.000000 django_glue-0.5.3/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 19:54:10.000000 django_glue-0.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-25 19:54:10.000000 django_glue-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 19:54:19.139330 django_glue-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 19:54:10.000000 django_glue-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/access.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/access/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.123330 django_glue-0.5.3/django_glue/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/base_entity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.127330 django_glue-0.5.3/django_glue/entities/function/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/post_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/function/session_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.127330 django_glue-0.5.3/django_glue/entities/model_object/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/model_object/session_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/post_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/entities/query_set/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/post_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/query_set/session_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/entities/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/post_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/entities/template/session_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/form/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/form/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/glue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/handler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/body_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.131330 django_glue-0.5.3/django_glue/response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/response/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/session/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/glue_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/keep_alive_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/session/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.119330 django_glue-0.5.3/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.119330 django_glue-0.5.3/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_function.js
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.119330 django_glue-0.5.3/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.135330 django_glue-0.5.3/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-25 19:54:10.000000 django_glue-0.5.3/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:54:19.000000 django_glue-0.5.3/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 19:54:10.000000 django_glue-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 19:54:19.139330 django_glue-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 19:54:10.000000 django_glue-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:19.139330 django_glue-0.5.3/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 19:54:10.000000 django_glue-0.5.3/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.011024 django_glue-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-26 15:59:31.000000 django_glue-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-26 15:59:31.000000 django_glue-0.6.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-26 15:59:31.000000 django_glue-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-26 15:59:31.000000 django_glue-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-26 15:59:40.011024 django_glue-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-26 15:59:31.000000 django_glue-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.983024 django_glue-0.6.0/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.983024 django_glue-0.6.0/django_glue/access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/access/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/access/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/access/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.983024 django_glue-0.6.0/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.983024 django_glue-0.6.0/django_glue/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/base_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.987024 django_glue-0.6.0/django_glue/entities/function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/post_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/function/session_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.987024 django_glue-0.6.0/django_glue/entities/model_object/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.987024 django_glue-0.6.0/django_glue/entities/model_object/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/fields/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/fields/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/fields/seralizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/fields/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/model_object/session_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/post_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.991024 django_glue-0.6.0/django_glue/entities/query_set/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/post_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/query_set/session_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.991024 django_glue-0.6.0/django_glue/entities/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/post_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/entities/template/session_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.991024 django_glue-0.6.0/django_glue/form/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/form/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/form/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/form/html_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/form/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/form/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/glue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.995024 django_glue-0.6.0/django_glue/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/handler/body_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/handler/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/handler/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/handler/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.995024 django_glue-0.6.0/django_glue/response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/response/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/response/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/response/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.995024 django_glue-0.6.0/django_glue/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/session/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/session/glue_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/session/keep_alive_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/session/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.975024 django_glue-0.6.0/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.975024 django_glue-0.6.0/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.995024 django_glue-0.6.0/django_glue/static/django_glue/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   232802 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.999024 django_glue-0.6.0/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    44523 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/alpine.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_function.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.999024 django_glue-0.6.0/django_glue/static/django_glue/js/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/forms/django_glue_form_field_binder.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/static/django_glue/js/forms/django_glue_form_fields.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.979024 django_glue-0.6.0/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.999024 django_glue-0.6.0/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/django_glue.html
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/django_glue_alpine_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/django_glue_bootstrap_css.html
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/django_glue_bootstrap_js.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:39.979024 django_glue-0.6.0/django_glue/templates/django_glue/form/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.003024 django_glue-0.6.0/django_glue/templates/django_glue/form/field/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/base_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/char_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/checkbox_select.html
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/decimal_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/email_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/input_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/number_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/password_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/telephone_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/field/text_field.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.003024 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/base_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/char_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/checkbox_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/color_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/date_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/datetime_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/email_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/input_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/number_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/password_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/radio_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/range_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/select_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/telephone_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/text_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templates/django_glue/form/glue_field/time_field.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.003024 django_glue-0.6.0/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-26 15:59:31.000000 django_glue-0.6.0/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.007024 django_glue-0.6.0/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-26 15:59:39.000000 django_glue-0.6.0/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-26 15:59:39.000000 django_glue-0.6.0/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:59:39.000000 django_glue-0.6.0/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:59:39.000000 django_glue-0.6.0/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 15:59:39.000000 django_glue-0.6.0/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 15:59:39.000000 django_glue-0.6.0/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-26 15:59:31.000000 django_glue-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-26 15:59:40.011024 django_glue-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-26 15:59:31.000000 django_glue-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.007024 django_glue-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/context_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:40.007024 django_glue-0.6.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/migrations/0003_testmodel_email_testmodel_personality_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/migrations/0004_testmodel_likes_to_party_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/migrations/0005_testmodel_bed_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-26 15:59:31.000000 django_glue-0.6.0/tests/wsgi.py
```

### Comparing `django_glue-0.5.3/CHANGELOG.md` & `django_glue-0.6.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog for Django Glue
 
+## 0.6.0
+### Changes
+- System to build form field attributes from model fields. 
+- HTML form fields (input, select, check radio).
+- Glue js field objects bind to HTML form fields to set attributes and expose values.
+- Ability to have full control over reactivity in forms in js that work with or without glue model objects.
+ 
+
 
 ## 0.5.3
 ### Changes
 - Created an extendable structure using glue entities as the base objects.
 - Removed meta and context keys from session data. 
 - Handler map based on action called from glue js objects to process response.
 - Dataclass structure for Response, Session and Post data.
```

### Comparing `django_glue-0.5.3/LICENSE.md` & `django_glue-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/PKG-INFO` & `django_glue-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.5.3
+Version: 0.6.0
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_glue-0.5.3/README.md` & `django_glue-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/access/access.py` & `django_glue-0.6.0/django_glue/access/access.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/core/decorators.py` & `django_glue-0.6.0/django_glue/core/decorators.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/base_entity.py` & `django_glue-0.6.0/django_glue/entities/base_entity.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/function/entities.py` & `django_glue-0.6.0/django_glue/entities/function/entities.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/function/handlers.py` & `django_glue-0.6.0/django_glue/entities/function/handlers.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/model_object/actions.py` & `django_glue-0.6.0/django_glue/entities/model_object/actions.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/model_object/entities.py` & `django_glue-0.6.0/django_glue/entities/model_object/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Union, Any
 
 from django.db.models import Model
 
 from django_glue.access.access import GlueAccess
 from django_glue.entities.base_entity import GlueEntity
-from django_glue.entities.model_object.fields import model_object_fields_from_model
-from django_glue.entities.model_object.response_data import GlueModelObjectJsonData, GlueModelFields
+from django_glue.entities.model_object.fields.entities import GlueModelFields
+from django_glue.entities.model_object.fields.factories import model_object_fields_from_model
+from django_glue.entities.model_object.fields.utils import get_field_value_from_model_object
 from django_glue.entities.model_object.session_data import GlueModelObjectSessionData
 from django_glue.handler.enums import GlueConnection
 from django_glue.utils import check_valid_method_kwargs, type_set_method_kwargs
 
 
 class GlueModelObject(GlueEntity):
     def __init__(
@@ -40,19 +41,24 @@
                 type_set_kwargs = type_set_method_kwargs(method, method_kwargs)
 
                 return method(**type_set_kwargs)
 
         return None
 
     def generate_field_data(self, include_values: bool = True) -> GlueModelFields:
-        glue_model_fields = model_object_fields_from_model(self.model, self.included_fields, self.excluded_fields)
+
+        glue_model_fields = model_object_fields_from_model(
+            model=self.model,
+            included_fields=self.included_fields,
+            excluded_fields=self.excluded_fields
+        )
 
         if include_values:
             for field in glue_model_fields:
-                field.value = getattr(self.model_object, field.name)
+                field.value = get_field_value_from_model_object(self.model_object, field)
 
         return glue_model_fields
 
     def generate_method_data(self):
         methods_list = list()
 
         for method in self.included_methods:
```

### Comparing `django_glue-0.5.3/django_glue/entities/model_object/factories.py` & `django_glue-0.6.0/django_glue/entities/model_object/factories.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/model_object/handlers.py` & `django_glue-0.6.0/django_glue/entities/model_object/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django_glue.access.decorators import check_access
 from django_glue.entities.model_object.actions import GlueModelObjectAction
-from django_glue.entities.post_data import UpdatePostData, MethodPostData, GetPostData
+from django_glue.entities.post_data import UpdatePostData, MethodPostData
 from django_glue.entities.model_object.factories import glue_model_object_from_glue_session
 from django_glue.entities.model_object.response_data import MethodGlueModelObjectJsonData, GlueModelObjectJsonData
 from django_glue.entities.model_object.session_data import GlueModelObjectSessionData
 from django_glue.handler.handlers import GlueRequestHandler
 from django_glue.response.data import GlueJsonResponseData
 from django_glue.response.responses import generate_json_200_response_data
```

### Comparing `django_glue-0.5.3/django_glue/entities/model_object/response_data.py` & `django_glue-0.6.0/django_glue/entities/model_object/response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import Any
 
-
-from django_glue.entities.model_object.fields import GlueModelFields
+from django_glue.entities.model_object.fields.entities import GlueModelFields
 from django_glue.response.data import GlueJsonData
 
 
 @dataclass
 class GlueModelObjectJsonData(GlueJsonData):  # This is a little duplicated but allows us to send more response data.
     fields: GlueModelFields
```

### Comparing `django_glue-0.5.3/django_glue/entities/post_data.py` & `django_glue-0.6.0/django_glue/entities/post_data.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/query_set/entities.py` & `django_glue-0.6.0/django_glue/entities/query_set/entities.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import pickle
 from typing import Union
 
 from django.db.models import QuerySet
 
 from django_glue.access.access import GlueAccess
 from django_glue.entities.base_entity import GlueEntity
-from django_glue.entities.model_object.entities import GlueModelObject
-from django_glue.entities.model_object.fields import model_object_fields_from_model
-from django_glue.entities.query_set.response_data import GlueQuerySetJsonData
+from django_glue.entities.model_object.fields.factories import model_object_fields_from_model
 from django_glue.entities.query_set.session_data import GlueQuerySetSessionData
 from django_glue.handler.enums import GlueConnection
 
 
 class GlueQuerySet(GlueEntity):
     def __init__(
             self,
```

### Comparing `django_glue-0.5.3/django_glue/entities/query_set/factories.py` & `django_glue-0.6.0/django_glue/entities/query_set/factories.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/query_set/handlers.py` & `django_glue-0.6.0/django_glue/entities/query_set/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,30 @@
         return generate_json_200_response_data(
             message_title='Success',
             message_body='Successfully retrieved model object!',
             data=GlueQuerySetJsonData([GlueModelObjectJsonData(glue_model_object.fields)])
         )
 
 
+class NullObjectGlueQuerySetHandler(GlueRequestHandler):
+    action = GlueQuerySetAction.NULL_OBJECT
+    _session_data_class = GlueQuerySetSessionData
+
+    @check_access
+    def process_response_data(self) -> GlueJsonResponseData:
+        glue_query_set = glue_query_set_from_session_data(self.session_data)
+        glue_model_object = glue_model_object_from_glue_query_set_session(glue_query_set.model(), self.session_data)
+
+        return generate_json_200_response_data(
+            message_title='Success',
+            message_body='Successfully retrieved model object!',
+            data=GlueQuerySetJsonData([GlueModelObjectJsonData(glue_model_object.fields)])
+        )
+
+
 class UpdateGlueQuerySetHandler(GlueRequestHandler):
     action = GlueQuerySetAction.UPDATE
     _session_data_class = GlueQuerySetSessionData
     _post_data_class = UpdatePostData
 
     @check_access
     def process_response_data(self) -> GlueJsonResponseData:
```

### Comparing `django_glue-0.5.3/django_glue/entities/query_set/maps.py` & `django_glue-0.6.0/django_glue/entities/query_set/maps.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,11 +2,12 @@
 from django_glue.entities.query_set import handlers
 
 
 GLUE_QUERY_SET_HANDLER_MAP = {
     GlueQuerySetAction.ALL: handlers.AllGlueQuerySetHandler,
     GlueQuerySetAction.FILTER: handlers.FilterGlueQuerySetHandler,
     GlueQuerySetAction.GET: handlers.GetGlueQuerySetHandler,
+    GlueQuerySetAction.NULL_OBJECT: handlers.NullObjectGlueQuerySetHandler,
     GlueQuerySetAction.UPDATE: handlers.UpdateGlueQuerySetHandler,
     GlueQuerySetAction.DELETE: handlers.DeleteGlueQuerySetHandler,
     GlueQuerySetAction.METHOD: handlers.MethodGlueQuerySetHandler,
 }
```

### Comparing `django_glue-0.5.3/django_glue/entities/query_set/response_data.py` & `django_glue-0.6.0/django_glue/entities/query_set/response_data.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/template/entities.py` & `django_glue-0.6.0/django_glue/entities/template/entities.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/entities/template/handlers.py` & `django_glue-0.6.0/django_glue/entities/template/handlers.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/glue.py` & `django_glue-0.6.0/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/handler/handlers.py` & `django_glue-0.6.0/django_glue/handler/handlers.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/handler/maps.py` & `django_glue-0.6.0/django_glue/handler/maps.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/handler/utils.py` & `django_glue-0.6.0/django_glue/handler/utils.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/middleware.py` & `django_glue-0.6.0/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/response/data.py` & `django_glue-0.6.0/django_glue/response/data.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/response/responses.py` & `django_glue-0.6.0/django_glue/response/responses.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/session/glue_session.py` & `django_glue-0.6.0/django_glue/session/glue_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import json
+
+from django.core.serializers.json import DjangoJSONEncoder
+
 from django_glue.conf import settings
 
 from django_glue.session.data import GlueSessionData
 from django_glue.session.session import Session
 
 
 class GlueSession(Session):
@@ -36,7 +40,10 @@
         self.set_modified()
 
     def purge_unique_name(self, unique_name):
         self.session.pop(unique_name)
 
     def set_modified(self):
         self.request.session.modified = True
+
+    def to_json(self):
+        return json.dumps(self.session, cls=DjangoJSONEncoder)
```

### Comparing `django_glue-0.5.3/django_glue/session/keep_alive_session.py` & `django_glue-0.6.0/django_glue/session/keep_alive_session.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_ajax.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_event.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_event.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_function.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_function.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_model_object.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -2,46 +2,54 @@
 
     constructor(glue_unique_name) {
         // We are encoding the unique name twice when
         this.glue_unique_name = glue_unique_name
         this.glue_encoded_unique_name = encodeUniqueName(glue_unique_name)
         this.glue_fields_set = false
 
-        // this['html_attr'] = {}
+        this['fields'] = {}
         if (this.glue_encoded_unique_name in window.glue_session_data) {
             this.set_fields(window.glue_session_data[this.glue_encoded_unique_name].fields)
         }
 
         window.glue_keep_live.add_unique_name(this.glue_encoded_unique_name)
     }
 
     delete() {
         glue_ajax_request(
             this.glue_encoded_unique_name,
             'delete', {
                 'id': this.id
             }
         ).then((response) => {
-            console.log(response)
+            // console.log(response)
             glue_dispatch_response_event(response)
         }).catch((error) => {
             glue_dispatch_object_delete_error_event(error)
         })
     }
 
+    duplicate() {
+        let model_object = new GlueModelObject(this.glue_unique_name)
+        console.log(this.get_properties())
+        model_object.set_properties(this.get_properties())
+        return model_object
+    }
+
     // Todo: Change this to load values.
     async get() {
         await glue_ajax_request(
             this.glue_encoded_unique_name,
             'get', {
                 'id': this.id,
             }
         ).then((response) => {
             glue_dispatch_response_event(response)
-            this.set_properties(JSON.parse(response.data))
+            // console.log(response.data)
+            this._set_properties(JSON.parse(response.data))
         }).catch((error) => {
             glue_dispatch_object_get_error_event(error)
         })
     }
 
     async method(method, kwargs = {}) {
         let data = {
@@ -67,47 +75,64 @@
             this.glue_encoded_unique_name,
             'update', {
                 'fields': this.get_properties(),
                 'id': this.id
             }
         ).then((response) => {
             glue_dispatch_response_event(response)
-            console.log(response)
             glue_dispatch_response_event(response)
-            this.set_properties(JSON.parse(response.data))
+            this._set_properties(JSON.parse(response.data))
 
         }).catch((error) => {
             glue_dispatch_object_update_error_event(error)
         })
     }
 
     get_properties() {
         let properties = {}
         Object.entries(this).forEach(([key, value]) => {
             properties[key] = value
         });
         return properties
     }
 
-    set_properties(fields) {
-        // Only sets properties that are already initialized on the glue object model.
+    _set_properties(fields) {
+        // Used to set fields internally on model object.
         if (!this.glue_fields_set) {
             this.set_fields(fields)
         }
+
         let simple_fields = simplify_model_fields(fields)
         for (let key in simple_fields) {
             if (key in this) {
                 this[key] = simple_fields[key]
             }
         }
     }
 
+    set_properties(simple_fields) {
+        // Used to set initial data to the glue object model after load.
+        // Send django context data and it will parse it into an object.
+
+        if (typeof simple_fields === 'string') {
+            simple_fields = parse_json_data(simple_fields)
+        }
+
+        for (let key in simple_fields) {
+            if (key in this) {
+                this[key] = simple_fields[key]
+            }
+        }
+    }
+
     set_fields(fields) {
+        // Fields are set on initialization if data is in the session.
+        // Else we have to set the field data on retrieval of object
         for (let key in fields) {
             this[key] = ''
-            // this['form_fields'][key] = window.glue_session_data['context'][this.glue_encoded_unique_name].fields[key]
+            this['fields'][key] = glue_model_field_from_field_attrs(fields[key].field_attrs)
         }
         this.glue_fields_set = true
 
     }
 
 }
```

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_query_set.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -19,29 +19,21 @@
                 'all': true
             })
             .then((response) => {
                 glue_dispatch_response_event(response)
                 let glue_query_set = JSON.parse(response.data)
                 for (let object in glue_query_set) {
                     let model_object = new GlueModelObject(this.glue_unique_name);
-                    model_object.set_properties(glue_query_set[object])
+                    model_object._set_properties(glue_query_set[object])
                     model_object_list.push(model_object)
                 }
                 return model_object_list
             });
     }
 
-    async bulk_create(query_model_object_list) {
-
-    }
-
-    async bulk_update(query_model_object_list) {
-
-    }
-
     delete(id) {
         glue_ajax_request(
             this.glue_encoded_unique_name,
             'delete', {
                 'id': id
             }
         ).then((response) => {
@@ -58,15 +50,15 @@
             })
             .then((response) => {
                 console.log(response)
                 let glue_query_set = JSON.parse(response.data)
                 glue_dispatch_response_event(response)
                 for (let object in glue_query_set) {
                     let model_object = new GlueModelObject(this.glue_unique_name)
-                    model_object.set_properties(glue_query_set[object])
+                    model_object._set_properties(glue_query_set[object])
                     model_object_list.push(model_object)
                 }
 
                 return model_object_list
             });
     }
 
@@ -75,15 +67,15 @@
         return await glue_ajax_request(this.glue_encoded_unique_name, 'get', {
                 'id': id
             })
             .then((response) => {
                 glue_dispatch_response_event(response)
                 model_object = new GlueModelObject(this.glue_unique_name);
                 let glue_query_set = JSON.parse(response.data)
-                model_object.set_properties(glue_query_set[0])
+                model_object._set_properties(glue_query_set[0])
                 return model_object
             });
     }
 
     async method(id, method, kwargs = {}) {
         // Todo: Should query sets be able to call methods?
         let data = {
@@ -98,14 +90,30 @@
         ).then((response) => {
             console.log(response)
             glue_dispatch_response_event(response)
             return JSON.parse(response.data).method_return
         })
     }
 
+    async null_object() {
+        console.log('null object')
+        let data = {}
+        return await glue_ajax_request(
+            this.glue_encoded_unique_name,
+            'null_object',
+            data
+        ).then((response) => {
+            glue_dispatch_response_event(response)
+            console.log(response)
+            let glue_query_set = JSON.parse(response.data)
+            let model_object = new GlueModelObject(this.glue_unique_name)
+            model_object._set_properties(glue_query_set[0])
+            return model_object
+        })
+    }
 
     update(query_model_object, field = null) {
         // Todo: Update on queryset should take fields and update all the objects fields to that value.
         // Todo: Should only be able to update fields on the main table.
         // Todo: Be aware that it does not call the save method.
 
         let data = {}
```

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_template.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/static/django_glue/js/django_glue_view.js` & `django_glue-0.6.0/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue/templates/django_glue/django_glue.html` & `django_glue-0.6.0/django_glue/templates/django_glue/django_glue.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 <script type="application/javascript">
     const DJANGO_DEBUG = {% if debug %}true{% else %}false{% endif %}
     const DJANGO_GLUE_AJAX_URL = '{% url 'django_glue:django_glue_data_handler' %}'
     const DJANGO_GLUE_KEEP_LIVE_URL = '{% url 'django_glue:django_glue_keep_live_handler' %}'
     const DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS = parseInt({{ DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS }})
 
-
     window.glue_keep_live = new GlueKeepLive()
     window.glue_session_data = {{ GLUE_SESSION_DATA|safe }}
 
     setInterval(() => {
         window.glue_keep_live.update(DJANGO_GLUE_KEEP_LIVE_URL)
     }, DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS)
 
 </script>
-
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_csrf.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_ajax.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_event.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
+<script type="application/javascript" src="{% static 'django_glue/js/forms/django_glue_form_fields.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
+<script type="application/javascript" src="{% static 'django_glue/js/forms/django_glue_form_field_binder.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_function.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_response.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_message.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_model_object.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_query_set.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_template.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_view.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
```

### Comparing `django_glue-0.5.3/django_glue/views.py` & `django_glue-0.6.0/django_glue/views.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/django_glue.egg-info/PKG-INFO` & `django_glue-0.6.0/django_glue.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.5.3
+Version: 0.6.0
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django_glue-0.5.3/setup.py` & `django_glue-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/forms.py` & `django_glue-0.6.0/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/manage.py` & `django_glue-0.6.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/migrations/0001_initial.py` & `django_glue-0.6.0/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py` & `django_glue-0.6.0/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/settings.py` & `django_glue-0.6.0/tests/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 }
 
 ROOT_URLCONF = 'tests.urls'
 
 SECRET_KEY = 'django_glue_secret_key_of_secrets'
 
 USE_TZ = True
+TIME_ZONE = 'America/Edmonton'
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [
             os.path.join(BASE_DIR, 'templates'),
         ],
@@ -70,9 +71,7 @@
             ],
             'debug': DEBUG,
         },
     },
 ]
 
 STATIC_URL = '/static/'
-
-DJANGO_GLUE_URL = 'django_glue/'
```

### Comparing `django_glue-0.5.3/tests/test_views.py` & `django_glue-0.6.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/urls.py` & `django_glue-0.6.0/tests/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     path("no_glue/", TemplateView.as_view(template_name='page/no_glue_page.html'), name="no_glue"),
     path("benchmark/", views.benchmark_view, name="benchmark"),
     path("django_glue/", include('django_glue.urls', namespace='django_glue')),
     path("template/", views.template_view, name="template"),
     path("view/", views.view_view, name="view"),
     path("view/card/", views.view_card_view, name="view_card"),
     path("function/", views.function_view, name="function"),
+    path("form/fields/", views.form_field_view, name="form_fields"),
     path("complex_form/", views.complex_form_view, name="complex_form"),
     path("complex_model_form/", views.complex_model_form_view, name="complex_model_form"),
 ]
 
 urlpatterns += [
     path('admin/', admin.site.urls),
 ]
```

### Comparing `django_glue-0.5.3/tests/utils.py` & `django_glue-0.6.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_glue-0.5.3/tests/views.py` & `django_glue-0.6.0/tests/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,54 @@
 from django.shortcuts import render
 from django.template.response import TemplateResponse
 from django.views.generic import TemplateView
 
 from tests.models import TestModel, BigTestModel
 from tests.processors import get_complex_form_processor
 from tests.utils import generate_randomized_test_model, generate_big_test_model
+from tests.context_data import django_glue_context_data
+
 from django_glue.glue import glue_model, glue_query_set, glue_template, glue_function
 
 
 def big_model_object_view(request):
-    big_model = BigTestModel.objects.first()
+    big_model = generate_big_test_model()
     glue_model(request, 'big_model', big_model, 'delete', fields=('foreign_key',))
     glue_query_set(request, 'big_model_query', BigTestModel.objects.all(), 'delete', fields=('foreign_key',))
 
     return TemplateResponse(request, template='page/big_model_object_page.html')
 
 
 class ModelObjectView(TemplateView):
     template_name = 'page/model_object_page.html'
 
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
+        context_data.update(django_glue_context_data(self.request))
 
         test_model_object = generate_randomized_test_model()
 
         glue_model(self.request, 'test_model_1', test_model_object, 'delete', exclude=('birth_date', 'anniversary_datetime'), methods=['is_lighter_than', 'get_full_name'])
-        glue_model(self.request, 'test_model_2', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime'))
-        glue_model(self.request, 'test_model_3', test_model_object, 'delete', exclude=('birth_date', 'anniversary_datetime'))
-        glue_model(self.request, 'test_model_4', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime'))
+        # glue_model(self.request, 'test_model_2', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime'))
+        # glue_model(self.request, 'test_model_3', test_model_object, 'delete', exclude=('birth_date', 'anniversary_datetime'))
+        # glue_model(self.request, 'test_model_4', test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime'))
 
         big_test_model_object = generate_big_test_model()
 
         return context_data
 
 
 class QuerySetView(TemplateView):
     template_name = 'page/query_set_page.html'
 
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
+        context_data.update(django_glue_context_data(self.request))
+
         glue_query_set(self.request, 'test_query_1', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'delete', exclude=('anniversary_datetime', 'birth_date'), methods=['is_lighter_than', 'get_full_name'])
         glue_query_set(self.request, 'test_query_3', TestModel.objects.filter(id__gte=1).filter(id__lte=10000), 'change', exclude=('birth_date', 'anniversary_datetime'))
 
         context_data['model_object_id'] = TestModel.objects.filter(id__gte=1).filter(id__lte=10000).first().id
         return context_data
 
 
@@ -56,17 +61,20 @@
         request,
         template='page/query_set_list_page.html'
     )
 
 
 class OtherView(TemplateView):
     template_name = 'page/other_glue_page.html'
+
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
+        context_data.update(django_glue_context_data(self.request))
+
         other_test_model_object = generate_randomized_test_model()
 
         logging.warning(f'Added Other TestModel object.')
 
         glue_model(self.request, 'other_test_model_1', other_test_model_object, 'change', exclude=('birth_date', 'anniversary_datetime',))
 
         logging.warning('Added model object glue for Other TestModel Object in write mode')
@@ -156,14 +164,20 @@
 
 
 def function_view(request):
     glue_function(request, 'function_1', 'tests.utils.test_glue_function')
     return TemplateResponse(request, 'page/function_page.html')
 
 
+def form_field_view(request):
+    person = generate_randomized_test_model()
+    glue_model(request, 'person', person)
+    return TemplateResponse(request, 'page/form_fields_page.html')
+
+
 def complex_form_view(request):
     LOCATION_CHOICES = [
         {'key': 'NYC', 'value': 'New York'},
         {'key': 'CHI', 'value': 'Chicago'},
     ]
 
     context_data = {
```

