# Comparing `tmp/shadowsocks_manager-0.1.8.tar.gz` & `tmp/shadowsocks_manager-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowsocks_manager-0.1.8.tar", last modified: Sun May 12 10:48:26 2024, max compression
+gzip compressed data, was "shadowsocks_manager-0.1.9.tar", last modified: Sat May 25 22:30:24 2024, max compression
```

## Comparing `shadowsocks_manager-0.1.8.tar` & `shadowsocks_manager-0.1.9.tar`

### file list

```diff
@@ -1,126 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.991607 shadowsocks_manager-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-05-12 10:48:26.991607 shadowsocks_manager-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.971607 shadowsocks_manager-0.1.8/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/bin/ssm-dev-start
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/bin/ssm-dev-stop
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/bin/ssm-setup
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/bin/ssm-test
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-12 10:48:23.000000 shadowsocks_manager-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-12 10:48:26.991607 shadowsocks_manager-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.971607 shadowsocks_manager-0.1.8/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.975607 shadowsocks_manager-0.1.8/shadowsocks_manager/args_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/args_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/args_formatter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.975607 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.975607 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/fixtures/nameserver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.975607 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.975607 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.975607 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.979607 shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/auth.group.json
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/sites.site.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.979607 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.979607 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/template-txt-to-json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/template.json
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.979607 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/notification/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.979607 shadowsocks_manager-0.1.8/shadowsocks_manager/retry/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/retry/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/fixtures/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36237 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.983607 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.987607 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.987607 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.987607 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/createsuperuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/uwsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-12 10:48:13.000000 shadowsocks_manager-0.1.8/shadowsocks_manager/utils/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:48:26.987607 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-05-12 10:48:26.000000 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-12 10:48:26.000000 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:48:26.000000 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 10:48:26.000000 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 10:48:26.000000 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 10:48:26.000000 shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.586996 shadowsocks_manager-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-05-25 22:30:24.586996 shadowsocks_manager-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.570996 shadowsocks_manager-0.1.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/bin/ssm-dev-start
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/bin/ssm-dev-stop
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/bin/ssm-setup
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/bin/ssm-test
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-25 22:30:20.000000 shadowsocks_manager-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-25 22:30:24.586996 shadowsocks_manager-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.570996 shadowsocks_manager-0.1.9/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.570996 shadowsocks_manager-0.1.9/shadowsocks_manager/args_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/args_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/args_formatter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.570996 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/commands/domain_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/commands/domain_nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/management/commands/domain_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11689 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/auth.group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/django_celery_beat.intervalschedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/sites.site.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      940 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.574996 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/template-txt-to-json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/notification/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/retry/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/fixtures/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36283 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21088 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.578996 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.582996 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.582996 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.582996 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.582996 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.582996 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/createsuperuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/uwsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-25 22:30:09.000000 shadowsocks_manager-0.1.9/shadowsocks_manager/utils/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:30:24.582996 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-05-25 22:30:24.000000 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-25 22:30:24.000000 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:30:24.000000 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 22:30:24.000000 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-25 22:30:24.000000 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 22:30:24.000000 shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/top_level.txt
```

### Comparing `shadowsocks_manager-0.1.8/LICENSE` & `shadowsocks_manager-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/PKG-INFO` & `shadowsocks_manager-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.8
+Version: 0.1.9
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -70,23 +70,26 @@
 Requires-Dist: django-celery-results; python_version > "2.7"
 Requires-Dist: django-enumfield<3.0; python_version <= "2.7"
 Requires-Dist: django-enumfield; python_version > "2.7"
 Requires-Dist: django-filter~=1.1; python_version <= "2.7"
 Requires-Dist: django-filter; python_version > "2.7"
 Requires-Dist: django-import-export
 Requires-Dist: djangorestframework
+Requires-Dist: dns-lexicon[full]
+Requires-Dist: dnspython
 Requires-Dist: docopt
 Requires-Dist: ipaddress; python_version < "3.3"
 Requires-Dist: psutil
 Requires-Dist: python-crontab==2.6.0; python_version <= "2.7"
 Requires-Dist: python-crontab; python_version > "2.7"
 Requires-Dist: python-decouple
 Requires-Dist: python-memcached==1.59
 Requires-Dist: pytz
 Requires-Dist: requests
+Requires-Dist: tldextract
 Requires-Dist: uWSGI
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: codecov-cli; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -367,35 +370,35 @@
     # run memcached, used by django cache
     docker run -d -p 11211:11211 --name ssm-dev-memcached memcached
 
     # run rabbitmq, used by celery
     docker run -d -p 5672:5672 --name ssm-dev-rabbitmq rabbitmq
 
     # run shadowsocks-libev, simulate localhost node
-    MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    MGR_PORT=6001 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
     docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP \
         -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
 
     # get the private IP address of the host, double check the result, it might not be correct
     PRIVATE_IP=$(ipconfig getifaddr en0 2>/dev/null || hostname -i | awk '{print $1}' 2>/dev/null)
     echo "PRIVATE_IP=$PRIVATE_IP"
 
     # run shadowsocks-libev, simulate private IP node
-    MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    MGR_PORT=6002 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
     docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
         -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-private shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         
     # run shadowsocks-libev, simulate public IP node
-    MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+    MGR_PORT=6003 SS_PORTS=8385 ENCRYPT=aes-256-cfb
     docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
         -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-public shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
     ```
 
@@ -435,16 +438,16 @@
 1. Test the Django code
 
     Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
 
     ```sh
     ssm-test -t
 
-    # or use the django test command directly for more options
-    ssm-manage test --no-input -v 2
+    # or use the django test command directly for more options, use the `-t .` for the Python 2.7 compatibility
+    ssm-manage test --no-input -v 2 -t .
     ```
 
 1. Test the Django code with coverage
 
     ```sh
     pip install coverage
     ssm-test -c
@@ -502,15 +505,18 @@
     # --use-pep517 is used together to make sure the PEP 517 is tested
     pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
-    docker build -t alexzhangs/shadowsocks-manager .
+    docker build -t alexzhangs/shadowsocks-manager -f docker/debian/Dockerfile .
+
+    # or use:
+    bash docker/docker-build-and-run.sh
     ```
 
 ### 8.2. CI/CD
 
 Github Actions is currently used for the CI/CD.
 Travis CI is removed due to the limitation of the free plan.
 
@@ -520,47 +526,71 @@
 * ci-testpypi.yml: Build and upload the package to TestPyPI.
 * ci-pypi.yml: Build and upload the package to PyPI. It can be triggered by the tag: `ci-pypi` or `ci-pypi-(major|minor|patch|suffx)`.
 * ci-docker.yml: Build and push the docker image to Docker Hub. It can be triggered by the Github release.
 
 
 ## 9. Troubleshooting
 
-1. Check the logs
+1. Docker
 
     ```
-    # supervisor
-    cat /var/log/supervisor/supervisord.log
+    # containers
+    docker ps -a
+
+    # network
+    docker network ls
+
+    # logs
+    docker logs <container_id>
+    ```
+
+1. Check the logs (inside container)
+
+    ```
+    # supervisor (debian)
+    cat /var/log/supervisor/supervisord.log 
+
+    # supervisor (alpine)
+    cat /var/log/supervisord.log
 
     # uWSGI
     cat /var/log/ssm-uwsgi.log
 
     # Celery
     cat /var/log/ssm-cerlery*
     ```
 
-1. Check the services
+1. Check the services (inside container)
 
     ```
     # nginx
-    service nginx {status|start|stop|reload}
+    nginx -s {stop|quit|reopen|reload}
 
     # supervisor
-    service supervisord {status|start|stop|restart}
     supervisorctl reload
     supervisorctl start all
 
     # uWSGI
     supervisorctl start ssm-uwsgi
 
     # Celery
     supervisorctl start ssm-celery-worker
     supervisorctl start ssm-celery-beat
 
-    # Docker
-    docker ps
+    # acme.sh
+    acme.sh --list
+    crontab -l
+    ls -l /root/.acme.sh
+
+    # volume data
+    ls -la /var/local/ssm
+
+    # setup done files
+    ls -la /var/local/ssm/.*done
+    ls -la /root/.*done
     ```
 
 1. Check the listening ports and processes (Linux)
 
     ```
     # TCP
     netstat -tanp
```

### Comparing `shadowsocks_manager-0.1.8/README.md` & `shadowsocks_manager-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -272,35 +272,35 @@
     # run memcached, used by django cache
     docker run -d -p 11211:11211 --name ssm-dev-memcached memcached
 
     # run rabbitmq, used by celery
     docker run -d -p 5672:5672 --name ssm-dev-rabbitmq rabbitmq
 
     # run shadowsocks-libev, simulate localhost node
-    MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    MGR_PORT=6001 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
     docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP \
         -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
 
     # get the private IP address of the host, double check the result, it might not be correct
     PRIVATE_IP=$(ipconfig getifaddr en0 2>/dev/null || hostname -i | awk '{print $1}' 2>/dev/null)
     echo "PRIVATE_IP=$PRIVATE_IP"
 
     # run shadowsocks-libev, simulate private IP node
-    MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    MGR_PORT=6002 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
     docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
         -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-private shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         
     # run shadowsocks-libev, simulate public IP node
-    MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+    MGR_PORT=6003 SS_PORTS=8385 ENCRYPT=aes-256-cfb
     docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
         -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-public shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
     ```
 
@@ -340,16 +340,16 @@
 1. Test the Django code
 
     Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
 
     ```sh
     ssm-test -t
 
-    # or use the django test command directly for more options
-    ssm-manage test --no-input -v 2
+    # or use the django test command directly for more options, use the `-t .` for the Python 2.7 compatibility
+    ssm-manage test --no-input -v 2 -t .
     ```
 
 1. Test the Django code with coverage
 
     ```sh
     pip install coverage
     ssm-test -c
@@ -407,15 +407,18 @@
     # --use-pep517 is used together to make sure the PEP 517 is tested
     pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
-    docker build -t alexzhangs/shadowsocks-manager .
+    docker build -t alexzhangs/shadowsocks-manager -f docker/debian/Dockerfile .
+
+    # or use:
+    bash docker/docker-build-and-run.sh
     ```
 
 ### 8.2. CI/CD
 
 Github Actions is currently used for the CI/CD.
 Travis CI is removed due to the limitation of the free plan.
 
@@ -425,47 +428,71 @@
 * ci-testpypi.yml: Build and upload the package to TestPyPI.
 * ci-pypi.yml: Build and upload the package to PyPI. It can be triggered by the tag: `ci-pypi` or `ci-pypi-(major|minor|patch|suffx)`.
 * ci-docker.yml: Build and push the docker image to Docker Hub. It can be triggered by the Github release.
 
 
 ## 9. Troubleshooting
 
-1. Check the logs
+1. Docker
 
     ```
-    # supervisor
-    cat /var/log/supervisor/supervisord.log
+    # containers
+    docker ps -a
+
+    # network
+    docker network ls
+
+    # logs
+    docker logs <container_id>
+    ```
+
+1. Check the logs (inside container)
+
+    ```
+    # supervisor (debian)
+    cat /var/log/supervisor/supervisord.log 
+
+    # supervisor (alpine)
+    cat /var/log/supervisord.log
 
     # uWSGI
     cat /var/log/ssm-uwsgi.log
 
     # Celery
     cat /var/log/ssm-cerlery*
     ```
 
-1. Check the services
+1. Check the services (inside container)
 
     ```
     # nginx
-    service nginx {status|start|stop|reload}
+    nginx -s {stop|quit|reopen|reload}
 
     # supervisor
-    service supervisord {status|start|stop|restart}
     supervisorctl reload
     supervisorctl start all
 
     # uWSGI
     supervisorctl start ssm-uwsgi
 
     # Celery
     supervisorctl start ssm-celery-worker
     supervisorctl start ssm-celery-beat
 
-    # Docker
-    docker ps
+    # acme.sh
+    acme.sh --list
+    crontab -l
+    ls -l /root/.acme.sh
+
+    # volume data
+    ls -la /var/local/ssm
+
+    # setup done files
+    ls -la /var/local/ssm/.*done
+    ls -la /root/.*done
     ```
 
 1. Check the listening ports and processes (Linux)
 
     ```
     # TCP
     netstat -tanp
```

### Comparing `shadowsocks_manager-0.1.8/bin/ssm-dev-start` & `shadowsocks_manager-0.1.9/bin/ssm-dev-start`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/bin/ssm-test` & `shadowsocks_manager-0.1.9/bin/ssm-test`

 * *Files 6% similar despite different names*

```diff
@@ -73,32 +73,33 @@
                 outfile_opt=(-o "$OPTARG")
                 ;;
             u)
                 upload=1
                 ;;
             *)
                 usage
-                exit 255
+                return 255
                 ;;
         esac
     done
 
     if [[ $# -eq 0 ]]; then
         usage
-        exit 255
+        return 255
     fi
 
     # run the test
     if [[ ${test} -eq 1 ]]; then
-        ssm-manage test --no-input -v 2
+        # use `-t .` for the Python 2.7 compatibility
+        ssm-manage test --no-input -v 2 -t .
     fi
 
     # run the test with coverage
     if [[ ${coverage} -eq 1 ]]; then
-        ssm coverage run manage.py test --no-input -v 2
+        ssm coverage run manage.py test --no-input -v 2 -t .
     fi
 
     # generate coverage report
     if [[ ${report} -eq 1 ]]; then
         ssm coverage xml "${outfile_opt[@]}"
     fi
```

### Comparing `shadowsocks_manager-0.1.8/pyproject.toml` & `shadowsocks_manager-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shadowsocks-manager"
-version = "0.1.8"
+version = "0.1.9"
 requires-python = ">=2.7"
 dependencies = [
     "future",
     "six",
     "boto3",
     "celery",
     "Django<4",
@@ -34,14 +34,16 @@
     # 20210314 - py2.7 - workaround for: SyntaxError: invalid syntax: File python2.7/site-packages/django_filters/filterset.py, line 184
     # https://github.com/carltongibson/django-filter/issues/954
     "django-filter~=1.1; python_version <= '2.7'",
     "django-filter; python_version > '2.7'",
 
     "django-import-export",
     "djangorestframework",
+    "dns-lexicon[full]",
+    "dnspython",
     "docopt",
 
     # ipaddress is available since Python 3.3
     "ipaddress; python_version < '3.3'",
 
     "psutil",
 
@@ -61,14 +63,15 @@
 
     # 20240430 - removed. the installation of Shadowsocks service should be handled outside of this project.
     # 20240417 - workaround for: AttributeError: dlsym(0x8c358790, EVP_CIPHER_CTX_cleanup): symbol not found: File python3.12/site-packages/shadowsocks/crypto/openssl.py, line 52
     # 20240417 - py3.10+ - workaround for: AttributeError: module 'collections' has no attribute 'MutableMapping': File python3.12/site-packages/shadowsocks/lru_cache.py, line 34
     # "shadowsocks",
     # "shadowsocks-alexforks",
 
+    "tldextract",
     "uWSGI",
 ]
 authors = [{name = "Alex", email = "alexzhangs@gmail.com"}]
 maintainers = []
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A shadowsocks manager for multi-user and traffic statistics"
@@ -136,15 +139,15 @@
 [tool.setuptools.package-data]
 shadowsocks_manager = ["fixtures/*", "**/fixtures/*"]
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.bumpversion]
-current_version = "0.1.8"
+current_version = "0.1.9"
 parse = """
     (?P<major>\\d+)\\.
     (?P<minor>\\d+)\\.
     (?P<patch>\\d+)
     (
         \\-                         # separator
         (?P<suffix>[0-9]\\d*)       # suffix Number
```

### Comparing `shadowsocks_manager-0.1.8/setup.cfg` & `shadowsocks_manager-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shadowsocks-manager
-version = 0.1.8
+version = 0.1.9
 description = A shadowsocks manager for multi-user and traffic statistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Alex
 author_email = alexzhangs@gmail.com
 url = https://github.com/alexzhangs/shadowsocks-manager
 license = MIT
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/__main__.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/args_formatter/__init__.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/args_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/args_formatter/tests.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/args_formatter/tests.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/domain/admin.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/domain/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,48 +9,48 @@
 from .models import NameServer, Domain, Record
 
 
 # Register your models here.
 
 @admin.register(NameServer)
 class NameServerAdmin(admin.ModelAdmin):
-    fields = ('name', 'api_cls_name', 'user', 'credential',
+    fields = ('name', 'env',
                   'dt_created', 'dt_updated')
 
     readonly_fields = ('dt_created', 'dt_updated')
 
-    list_display = ('name', 'api_cls_name', 'user', 'is_api_accessible',
+    list_display = ('name', 'env',
                         'dt_created', 'dt_updated')
 
-    def is_api_accessible(self, obj):
-        return obj.is_api_accessible
-
-    is_api_accessible.boolean = True
-    is_api_accessible.short_description = 'API'
-
 
 @admin.register(Domain)
 class DomainAdmin(admin.ModelAdmin):
     fields = ('name', 'nameserver',
                   'dt_created', 'dt_updated')
 
     readonly_fields = ('dt_created', 'dt_updated')
 
-    list_display = ('name', 'nameserver',
+    list_display = ('name', 'nameserver', 'is_api_accessible',
                         'dt_created', 'dt_updated')
 
+    def is_api_accessible(self, obj):
+        return obj.is_api_accessible
+
+    is_api_accessible.boolean = True
+    is_api_accessible.short_description = 'API'
+
 
 @admin.register(Record)
 class RecordAdmin(admin.ModelAdmin):
     fields = ('host', 'domain', 'type', 'answer', 'site',
                   'dt_created', 'dt_updated')
 
     readonly_fields = ('dt_created', 'dt_updated')
 
-    list_display = ('host', 'domain', 'type', 'answer', 'answer_from_dns_api', 'is_matching_dns_api',
+    list_display = ('fqdn', 'host', 'domain', 'type', 'answer', 'answer_from_dns_api', 'is_matching_dns_api',
                         'answer_from_dns_query', 'is_matching_dns_query', 'site',
                         'dt_created', 'dt_updated')
 
     def answer_from_dns_api(self, obj):
         return list(obj.answer_from_dns_api) if obj.answer_from_dns_api is not None else obj.answer_from_dns_api
 
     def answer_from_dns_query(self, obj):
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/domain/models.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/domain/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,164 +1,227 @@
 # -*- coding: utf-8 -*-
 
 # py2.7 and py3 compatibility imports
 from __future__ import unicode_literals
 
+import os
+import re
 import logging
-import socket, requests, json
+import dns.resolver, tldextract
+import lexicon
 from collections import defaultdict
 from django.db import models
 from django.db.models.signals import post_save, post_delete
 from django.dispatch import receiver
 from django.contrib.sites.models import Site
 from django.conf import settings
 
 
 logger = logging.getLogger(__name__)
 
 
 # Create your models here.
 
+def get_host_name(domain):
+    """
+    Return the part before the root domain name or the delegated subdomain name.
+    e.g.:
+        foo.bar.example.co.uk           -> foo.bar
+        foo.zone2.zone1.example.co.uk   -> foo
+        example.co.uk                   -> ''
+        zone2.zone1.example.co.uk       -> ''
+    """
+    if domain:
+        zone = get_zone_name(domain)
+        return re.sub('([.]|^)' + zone + '$', '', domain) if zone else None
+
+def get_zone_name(domain):
+    """
+    Return the root domain name or the delegated subdomain name.
+    If the domain is not resolvable, fallback to use the root domain name.
+    e.g.:
+        foo.bar.example.co.uk           -> example.co.uk
+        foo.zone2.zone1.example.co.uk   -> zone2.zone1.example.co.uk
+        example.co.uk                   -> example.co.uk
+        zone2.zone1.example.co.uk       -> zone2.zone1.example.co.uk
+    """
+    if domain:
+        extract = tldextract.TLDExtract()
+        # deal with py2 and py3 compatibility
+        compat_method = extract.extract if hasattr(extract, 'extract') else extract
+        result = compat_method(domain)
+
+        # get the root domain name
+        root = result.registered_domain
+        if domain == root:
+            # no need to resolve the domain
+            return domain
+
+        zone = dns.resolver.zone_for_name(domain).to_text(omit_final_dot=True)
+        # get the tld from the domain
+        tld = result.suffix
+        if zone == tld:
+            # the domain is not resolvable, fallback to use the root domain
+            zone = root
+        return zone
+
+
 class Site(Site):
 
     class Meta:
         proxy = True
 
     def __str__(self):
         return self.name
 
 
-class BaseNsApi(object):
-
-    def __init__(self, user, credential, *args, **kwargs):
-        super(BaseNsApi, self).__init__(*args, **kwargs)
-        self.user = user
-        self.credential = credential
-
-    def call_api(self, url, method='get', data=None):
-        if not self.user or not self.credential:
-            logger.error('{0}: User and Credential are required.'.format(self.__class__.__name__))
-            return
-
-        response = getattr(requests, method)(
-            url,
-            auth=(self.user, self.credential),
-            json=data,
-            timeout=30
-        )
-        return response.json()
-
-    def create_record(self, *args, **kwargs):
-        pass
-
-    def list_records(self, *args, **kwargs):
-        pass
-
-    def delete_records(self, *args, **kwargs):
-        pass
-
-
-class NameNsApi(BaseNsApi):
-
-    api_base_url = 'https://api.name.com/v4'
-
-    def create_record(self, domain, type, host, answer, ttl=300):
-        url = "/".join([self.api_base_url, 'domains', domain, 'records'])
-        data = {"host": host, "type": type, "answer": answer, "ttl": ttl}
+class DnsApi:
+    """
+    https://dns-lexicon.readthedocs.io/en/latest/provider_conventions.html
+    """
+    def __init__(self, env, domain):
+        self.config = lexicon.config.ConfigResolver()
+
+        # export the environment variables
+        for item in env.split(','):
+            # split with only the first '=', ignore the rest
+            key, value = item.split('=', 1)
+            os.environ[key] = value
+
+        self.config.with_env().with_dict({
+            'domain': domain,
+        })
 
-        return self.call_api(url, method='post', data=data)
-
-    def list_records(self, domain, type, host):
-        url = "/".join([self.api_base_url, 'domains', domain, 'records'])
-
-        records = self.call_api(url, method='get') or {}
-        return [item for item in records.get('records', [])
-                   if item.get('type') == type and item.get('host') == host]
+    def call(self, method, *args):
+        try:
+            with lexicon.client.Client(self.config) as operations:
+                return getattr(operations, method)(*args)
+        except Exception as e:
+            logger.error(e)
+            return None
+    
+    def list_records(self, type, name=None, content=None):
+        return self.call('list_records', type, name, content)
 
-    def delete_records(self, domain, type, host):
-        records = self.list_records(domain, type, host)
+    def create_record(self, type, name, content):
+        return self.call('create_record', type, name, content)
 
-        for item in records:
-            url = "/".join([self.api_base_url, 'domains', domain, 'records', str(item.get('id'))])
-            self.call_api(url, method='delete')
+    def update_record(self, type, name, content):
+        return self.call('update_record', None, type, name, content)
 
-        return records
+    def delete_record(self, type, name, content=None):
+        return self.call('delete_record', None, type, name, content)
 
     @property
     def is_accessible(self):
         try:
-            url = "/".join([self.api_base_url, 'hello'])
-            return self.call_api(url, method='get').get('username') == self.user
-        except:
+            return self.list_records('A', 'whatever') is not None
+        except Exception as e:
+            logger.error(e)
             return False
 
 
 class NameServer(models.Model):
-    API_CLASS_NAME = [
-        ('NameNsApi', 'NameNsApi')
-    ]
-
     name = models.CharField(unique=True, max_length=64,
-        help_text='The name for the Nameserver, name it as your wish. Example: name.com.')
-    api_cls_name = models.CharField('API Class', max_length=32, choices=API_CLASS_NAME,
-        help_text='Select the API class name for the Nameserver.')
-    user = models.CharField(max_length=64, null=True, blank=True,
-        help_text='User identity for the Nameserver API service.')
-    credential = models.CharField(max_length=128, null=True, blank=True,
-        help_text='User credential/token for the Nameserver API service.')
+        help_text='The name for the Nameserver, name it as your wish. Example: `name.com`.')
+    env = models.CharField(max_length=512, null=True, blank=True,
+        help_text='Environment variables required to use the DNS API service.<br>'
+            'Syntax: `LEXICON_PROVIDER_NAME={dns_provider},LEXICON_{DNS_PROVIDER}_{OPTION}={value}[,...]`<br>'
+            'The Python library `dns-lexicon` is leveraged to parse the DNS_ENV and access the DNS API.<br>'
+            'The required {OPTION} depends on the {dns_provider} that you use.<br>'
+            'Sample: `LEXICON_PROVIDER_NAME=namecom,LEXICON_NAMECOM_AUTH_USERNAME=your_username,LEXICON_NAMECOM_AUTH_TOKEN=your_token`<br>'
+            'Link: https://dns-lexicon.readthedocs.io/en/latest/configuration_reference.html')
     dt_created = models.DateTimeField('Created', auto_now_add=True)
     dt_updated = models.DateTimeField('Updated', auto_now=True)
 
     def __str__(self):
         return self.name
 
-    def __init__(self, *args, **kwargs):
-        super(NameServer, self).__init__(*args, **kwargs)
-
-        self.api_cls = globals().get(self.api_cls_name)
-
-    @property
-    def api(self):
-        if self.api_cls and self.user and self.credential:
-            return self.api_cls(self.user, self.credential)
-
-    @property
-    def is_api_accessible(self):
-        return self.api.is_accessible if self.api else None
 
+class DomainManager(models.Manager):
+    def resolve_name(self, kwargs):
+        if 'name' in kwargs:
+            kwargs['name'] = get_zone_name(kwargs['name'])
+        return kwargs
+
+    def get(self, *args, **kwargs):
+        kwargs = self.resolve_name(kwargs)
+        return super(DomainManager, self).get(*args, **kwargs)
+
+    def filter(self, *args, **kwargs):
+        kwargs = self.resolve_name(kwargs)
+        return super(DomainManager, self).filter(*args, **kwargs)
+
+    def get_or_create(self, *args, **kwargs):
+        kwargs = self.resolve_name(kwargs)
+        return super(DomainManager, self).get_or_create(*args, **kwargs)
+
+    def update_or_create(self, *args, **kwargs):
+        kwargs = self.resolve_name(kwargs)
+        return super(DomainManager, self).update_or_create(*args, **kwargs)
+    
 
 class Domain(models.Model):
     name = models.CharField(unique=True, max_length=64,
-        help_text='Root domain name. Example: yourdomain.com.')
+        help_text='Domain name. Example: `example.com`. '
+        'If the domain name is not root domain name, the zone name will be resolved automatically. ')
     nameserver = models.ForeignKey(NameServer, null=True, blank=True, on_delete=models.SET_NULL)
     dt_created = models.DateTimeField('Created', auto_now_add=True)
     dt_updated = models.DateTimeField('Updated', auto_now=True)
 
+    objects = DomainManager()
+
     def __str__(self):
         return self.name
 
+    def __init__(self, *args, **kwargs):
+        super(Domain, self).__init__(*args, **kwargs)
+
+        self.api = None
+        if self.nameserver and self.nameserver.env:
+            try:
+                self.api = DnsApi(self.nameserver.env, self.name)
+            except Exception as e:
+                logger.error('DnsApi: domain ({0}), env ({1}): {2}'.format(self.name, self.nameserver.env, e))
+
+    def save(self, *args, **kwargs):
+        self.auto_resolve()
+
+        super(Domain, self).save(*args, **kwargs)
+
+    def auto_resolve(self):
+        """
+        Resolve the root domain name or the delegated subdomain name from the domain name.
+        """
+        if self.name:
+            self.name = get_zone_name(self.name)
+
     @property
-    def ns_api(self):
-        return self.nameserver.api if self.nameserver else None
+    def is_api_accessible(self):
+        return self.api.is_accessible if self.api else None
 
 
 class Record(models.Model):
     TYPE = [
         ('A', 'A'),
         ('MX', 'MX'),
         ('CNAME', 'CNAME'),
         ('TXT', 'TXT'),
         ('SRV', 'SRV'),
         ('AAAA', 'AAAA'),
         ('NS', 'NS'),
         ('ANAME', 'ANAME'),
     ]
 
+    fqdn = models.CharField(unique=True, max_length=128,
+        help_text='Fully Qualified Domain Name. Example: `vpn.yourdomain.com`. '
+        'The `host` and `domain` (zone name) will be automatically resolved. '
+        'if both `host` and `domain` are set, this field will be ignored.')
     host = models.CharField(max_length=64,
-        help_text='Host name. Example: vpn.')
+        help_text='Host name without domain name. Example: `vpn`.')
     domain = models.ForeignKey(Domain, on_delete=models.PROTECT)
     type = models.CharField(max_length=8, null=True, blank=True, choices=TYPE)
     answer = models.CharField(max_length=512, null=True, blank=True,
         help_text='Answer for the host name, comma "," is the delimiter for multiple answers.')
     site = models.ForeignKey(Site, null=True, blank=True, on_delete=models.SET_NULL, related_name='records',
         help_text="The record with a site will be dynamically added to Django's ALLOWED_HOSTS.")
     dt_created = models.DateTimeField('Created', auto_now_add=True)
@@ -167,23 +230,34 @@
     class Meta:
         unique_together = ('host', 'domain')
 
     def __str__(self):
         return self.fqdn
 
     def save(self, *args, **kwargs):
+        self.auto_resolve()
+
         super(Record, self).save(*args, **kwargs)
+
+        # update the site domain
         if self.site:
             self.site.domain = self.fqdn
             self.site.save()
             settings.ALLOWED_HOSTS.update_cache()
 
-    @property
-    def fqdn(self):
-        return '.'.join([self.host, self.domain.name])
+    def auto_resolve(self):
+        """
+        Resolve the host and domain from the fqdn if they are not set.
+        Resolve the fqdn from the host and domain if it is not set.
+        """
+        if self.host and self.domain:
+            self.fqdn = '.'.join([self.host, self.domain.name])
+        elif self.fqdn:
+            self.host = get_host_name(self.fqdn)
+            self.domain = Domain.objects.get(name=get_zone_name(self.fqdn))
 
     @property
     def answers(self):
         """
         Return the record.answer in lowercase and split as Set.
         """
         return {
@@ -192,36 +266,36 @@
         }
 
     @property
     def answer_from_dns_api(self):
         """
         Return the answers from DNS API, in lowercase and as Set.
         """
-        if self.domain.ns_api:
+        if self.domain.api:
             return {
-                record.get('answer').lower()
-                for record in self.domain.ns_api.list_records(
-                    self.domain.name, self.type, self.host
-                )
+                record.get('content').lower()
+                for record in self.domain.api.list_records(self.type, self.host) or []
             }
 
     @property
     def answer_from_dns_query(self):
         """
         Return the answers from DNS query, in lowercase and as Set.
         """
-        ips = []
         try:
-            truename, alias, ips = socket.gethostbyname_ex(self.fqdn)
-        except socket.gaierror:
+            # deal with py2 and py3 compatibility
+            compat_method = dns.resolver.query if hasattr(dns.resolver, 'query') else dns.resolver.resolve
+            answers = compat_method(self.fqdn, self.type)
+
+            return {item.to_text().lower() for item in answers}
+        except dns.resolver.NXDOMAIN:
             # not found the host
-            pass
+            return {}
         except Exception as e:
             logger.error(e)
-        return {item.lower() for item in ips}
 
     @property
     def is_matching_dns_api(self):
         """
         Test if the record.answer matches the DNS API query.
         """
         return self.answers == self.answer_from_dns_api
@@ -234,34 +308,33 @@
         return self.answers == self.answer_from_dns_query
 
     def sync_to_dns(self):
         """
         Sync the record to DNS server through DNS API.
         """
         ret = defaultdict(list)
-        if self.domain.ns_api:
+        if self.domain.api:
             if self.is_matching_dns_api:
                 ret['message'] = 'No need to synchronize.'
                 return ret
 
             ret['deleted'] = self.delete_from_dns()
             for answer in (self.answer or '').split(','):
-                ret['created'].append(
-                    self.domain.ns_api.create_record(self.domain.name, self.type, self.host, answer))
+                ret['created'].append(self.domain.api.create_record(self.type, self.host, answer))
         else:
-            ret['message'] = 'Please configure Nameserver and its User and Credential for the domain first.'
+            ret['message'] = 'Please configure Nameserver properly for the domain first.'
 
         return ret
 
     def delete_from_dns(self):
         """
         Delete the record from DNS server through DNS API.
         """
-        if self.domain.ns_api:
-            return self.domain.ns_api.delete_records(self.domain.name, self.type, self.host)
+        if self.domain.api:
+            return self.domain.api.delete_record(self.type, self.host)
 
 
 @receiver(post_save, sender=Record)
 def record_sync_to_dns(sender, instance, **kwargs):
     instance.sync_to_dns()
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/domain/tests.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/domain/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from abc import abstractmethod
 from django.test import TestCase
 
 from domain import models, serializers
 
 
 import logging
-# Get a logger for this module
-logger = logging.getLogger(__name__)
+# Get a logger for this django app
+logger = logging.getLogger(__name__.split('.')[0])
 # Set the logging level to make the output clean
-logger.setLevel(logging.ERROR)
+logger.setLevel(logging.CRITICAL)
 
 
 class BaseTestCase(TestCase):
     """
     A base test case for current app.
     This class is inherited from Django TestCase class, and provides the following features:
 
@@ -70,54 +70,50 @@
         """
         for testcase in [globals().get(name) for name in cls.testcases]:
             method = getattr(testcase or {}, 'down', None)
             if method: method()
 
 
 class AppTestCase(BaseTestCase):
-    fixtures = ['nameserver.json']
+    fixtures = []
     testcases = ['NameServerTestCase', 'DomainTestCase', 'RecordTestCase']
 
 
 class NameServerTestCase(AppTestCase):
     @classmethod
     def up(cls):
-        # add mock username and credential to nameserver
-        for obj in models.NameServer.objects.all():
-            if not obj.user:
-                obj.user = 'mock-user'
-            if not obj.credential:
-                obj.credential = 'mock-credential'
-            obj.save()
+        # add nameserver
+        obj = models.NameServer(name='mocknameserver', env='PROVIDER=mockprovider,LEXICON_PROVIDER_NAME=mockprovider,LEXICON_MOCKPROVIDER_MOCKUSER=mockuser,LEXICON_MOCKPROVIDER_MOCKTOKEN=mocktoken')
+        obj.save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
 
-    def test_nameserver_is_api_accessible_negative(self):
-        for obj in models.NameServer.objects.all():
-            self.assertFalse(obj.is_api_accessible)
-
     def test_nameserver_serializer(self):
         obj = serializers.NameServerSerializer()
         json.loads(json.dumps(obj.to_representation(models.NameServer.objects.first())))
 
 
 class DomainTestCase(AppTestCase):
     @classmethod
     def up(cls):
         # add mock domain
         for ns in models.NameServer.objects.all():
-            obj = models.Domain(name='mock-example-{}.com'.format(ns.pk), nameserver=ns)
+            obj = models.Domain(name='mock-{}.example.com'.format(ns.pk), nameserver=ns)
             obj.save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
 
+    def test_domain_is_api_accessible_negative(self):
+        for obj in models.Domain.objects.all():
+            self.assertFalse(obj.is_api_accessible)
+
     def test_domain_serializer(self):
         obj = serializers.DomainSerializer()
         json.loads(json.dumps(obj.to_representation(models.Domain.objects.first())))
 
 
 class RecordTestCase(AppTestCase):
     @classmethod
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/domain/views.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 # -*- coding: utf-8 -*-
 
 # py2.7 and py3 compatibility imports
 from __future__ import unicode_literals
 from __future__ import absolute_import
 
-from shadowsocks_manager.utils.viewsets import CompatModelViewSet
+from utils.viewsets import CompatModelViewSet
 
 from . import models, serializers
 
 
 # Create your views here.
 
-class NameServerViewSet(CompatModelViewSet):
+class ConfigViewSet(CompatModelViewSet):
     """
     This viewset automatically provides `list` and `detail` actions.
     """
-    queryset = models.NameServer.objects.all()
-    serializer_class = serializers.NameServerSerializer
-    filter_fields = ['name', 'api_cls_name', 'user']
+    queryset = models.Config.objects.all()
+    serializer_class = serializers.ConfigSerializer
 
 
-class DomainViewSet(CompatModelViewSet):
+class AccountViewSet(CompatModelViewSet):
     """
     This viewset automatically provides `list` and `detail` actions.
     """
-    queryset = models.Domain.objects.all()
-    serializer_class = serializers.DomainSerializer
-    filter_fields = ['name', 'nameserver', 'nameserver__name']
+    queryset = models.Account.objects.all()
+    serializer_class = serializers.AccountSerializer
 
 
-class RecordViewSet(CompatModelViewSet):
+class NodeViewSet(CompatModelViewSet):
     """
     This viewset automatically provides `list` and `detail` actions.
     """
-    queryset = models.Record.objects.all()
-    serializer_class = serializers.RecordSerializer
-    filter_fields = ['host', 'domain', 'domain__name', 'type', 'answer', 'site', 'site__name', 'site__domain']
+    queryset = models.Node.objects.all()
+    serializer_class = serializers.NodeSerializer
+    filter_fields = ['name']
+
+
+class NodeAccountViewSet(CompatModelViewSet):
+    """
+    This viewset automatically provides `list` and `detail` actions.
+    """
+    queryset = models.NodeAccount.objects.all()
+    serializer_class = serializers.NodeAccountSerializer
+
+
+class SSManagerViewSet(CompatModelViewSet):
+    """
+    This viewset automatically provides `list` and `detail` actions.
+    """
+    queryset = models.SSManager.objects.all()
+    serializer_class = serializers.SSManagerSerializer
+    filter_fields = ['node', 'node__name', 'server_edition', 'is_v2ray_enabled']
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/dynamicmethod/models.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/dynamicmethod/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json` & `shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/django_celery_beat.crontabschedule.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json` & `shadowsocks_manager-0.1.9/shadowsocks_manager/fixtures/django_celery_beat.periodictask.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/manage.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/template-txt-to-json.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/template-txt-to-json.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/template.json` & `shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/template.json`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/notification/fixtures/template.txt` & `shadowsocks_manager-0.1.9/shadowsocks_manager/notification/fixtures/template.txt`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/notification/models.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/notification/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/notification/tests.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/notification/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from abc import abstractmethod
 from django.test import TestCase
 
 from notification import models, serializers
 
 
 import logging
-# Get a logger for this module
-logger = logging.getLogger(__name__)
+# Get a logger for this django app
+logger = logging.getLogger(__name__.split('.')[0])
 # Set the logging level to make the output clean
 logger.setLevel(logging.ERROR)
 
 
 class BaseTestCase(TestCase):
     """
     A base test case for current app.
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/retry/__init__.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/admin.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/management/commands/shadowsocks_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from django.core.management.base import BaseCommand
 from shadowsocks.models import Config
 
 class Command(BaseCommand):
-    help = 'Set shadowsocks config parameters'
+    help = 'Set shadowsocks.models.Config parameters'
     django_default_options = ('verbosity', 'settings', 'pythonpath', 'traceback', 'no_color', 
                        'force_color', 'skip_checks')
 
     def add_arguments(self, parser):
         parser.add_argument('--port-begin', type=int, nargs='?')
         parser.add_argument('--port-end', type=int, nargs='?')
         parser.add_argument('--timeout-remote', type=float, nargs='?')
         parser.add_argument('--timeout-local', type=float, nargs='?')
         parser.add_argument('--cache-timeout', type=float, nargs='?')
 
     def handle(self, *args, **options):
-        for key, value in options.items():
-            if key in self.django_default_options:
-                # skip django default options
-                continue
-
+        for key, value in self.get_fields(options).items():
             if value is not None:
                 Config.objects.update(**{key: value})
-                self.stdout.write(self.style.SUCCESS(f'Successfully set shadowsocks.config.{key} to {value}'))
+                self.stdout.write(self.style.SUCCESS(f'Successfully set shadowsocks.models.Config: {key} to {value}'))
+
+    @classmethod
+    def get_fields(cls, options):
+        return {key: value for key, value in options.items() if key not in cls.django_default_options}
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/models.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             kwargs['node_accounts'].append(d)
             d['node'] = na.node
             d['account'] = na.account
         kwargs['sender'] = sender
 
         message = template.render(kwargs)
 
-        logger.info("Sending VPN account Email to %s(%s) on port %s" % (self.email, \
+        logger.info("Sending VPN account Email to %s(%s) on port %s" % (self.email,
             self.get_full_name(), self.username))
         return Notify.sendmail(message, sender.get_full_name(), sender.email)
 
     def on_update(self):
         for na in self.nodes_ref.all():
             if self._original_username != self.username: # port is changed
                 na.on_delete(original=True)
@@ -261,15 +261,15 @@
             if ip_address(ip).is_private:
                 s.settimeout(Config.load().timeout_local) # seconds
             else:
                 s.settimeout(Config.load().timeout_remote) # seconds
             s.connect((ip, int(port)))
             s.shutdown(socket.SHUT_RDWR)
             return True
-        except:
+        except Exception:
             return False
         finally:
             s.close()
 
     @property
     def is_matching_dns_query(self):
         """
@@ -480,29 +480,29 @@
             return
 
         if self.is_active:
             if self.node.ssmanager.is_accessible:
                 self.node.ssmanager.add(port=self.account.username, password=self.account.password)
                 self.clear_cache()
             else:
-                logger.error('%s: creation eror: ssmanager %s currently is not available.' \
+                logger.error('%s: creation eror: ssmanager %s currently is not available.'
                     % (self, self.node.ssmanager))
         else:
             self.on_delete()
 
     def on_delete(self, original=False):
         if not self.node.ssmanager:
             return
 
         port = '_original_username' if original else 'username'
         if self.node.ssmanager.is_accessible:
             self.node.ssmanager.remove(port=getattr(self.account, port))
             self.clear_cache()
         else:
-            logger.error('%s: deletion eror: ssmanager %s currently is not available.' % (self, \
+            logger.error('%s: deletion eror: ssmanager %s currently is not available.' % (self,
                 self.node.ssmanager))
 
     @classmethod
     def heartbeat(cls):
         """
         Heartbeat once on all the nodeaccounts.
         Create the active ones and delete the inactive ones on the corresponding nodes.
@@ -903,15 +903,15 @@
         Return the Shadowsocks process's pid and status.
         """
         try:
             with open(self.pidfile(), 'r') as f:
                 pid = int(f.read())
             p = psutil.Process(pid=pid).as_dict(['pid', 'status'])
             return '{status}({pid})'.format(**p)
-        except:
+        except (FileNotFoundError, psutil.NoSuchProcess):
             pass
 
     '''
     def install(self):
         """
         Install Shadowsocks python edition.
         Skip if already installed.
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/serializers.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/tests.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # -*- coding: utf-8 -*-
 
 # py2.7 and py3 compatibility imports
 from __future__ import unicode_literals
 from __future__ import absolute_import
 
 import json
-import re
 from abc import abstractmethod
 from django.test import TestCase
 from django.core.exceptions import ValidationError
 
 from domain.models import Record
 from domain.tests import AppTestCase as DomainAppTestCase
 from notification.tests import AppTestCase as NotificationAppTestCase
 from shadowsocks import models, serializers
 
 
 import logging
-# Get a logger for this module
-logger = logging.getLogger(__name__)
+# Get a logger for this django app
+logger = logging.getLogger(__name__.split('.')[0])
 # Set the logging level to make the output clean
 logger.setLevel(logging.ERROR)
 
 
 import socket
 def get_local_ip():
     """
     Get the local ip address.
     https://github.com/mayermakes/Get_IP
     """
-    ip = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
-        ip.connect(('10.255.255.255', 1))
-        IP = ip.getsockname()[0]
-    except:
-        raise
+        s.connect(('10.255.255.255', 1))
+        IP = s.getsockname()[0]
     finally:
-        ip.close()
+        s.close()
     return IP
 local_ip = get_local_ip()
 
 
 """
 Feature matrix for methods in unittest.TestCase class:
 +-------------+------------------+---------------------+----------------+----------------------------------+---------------------------+
@@ -138,14 +135,15 @@
     testcases = ['ConfigTestCase', 'AccountTestCase', 'NodeTestCase', 'SSManagerTestCase', 'NodeAccountTestCase']
 
 
 class ConfigTestCase(AppTestCase):
     @classmethod
     def up(cls):
         obj = models.Config.load()
+        obj.port_end=8385
         obj.timeout_local=0.3
         obj.timeout_remote=1  # minimal the waiting time with mock public ip address
         obj.save()
 
     @classmethod
     def setUpTestData(cls):
         cls.allup()
@@ -158,14 +156,15 @@
         json.loads(json.dumps(obj.to_representation(models.Config.objects.first())))
 
 
 class AccountTestCase(AppTestCase):
     @classmethod
     def up(cls):
         config = models.Config.load()
+        config.port_end=8385
 
         # generate 2 accounts
         for port in [config.port_begin, config.port_end]:
             models.Account(
                 username=port,
                 password='mock-password',
                 email='mock@mock-example.com',
@@ -429,15 +428,15 @@
 
 class SSManagerTestCase(AppTestCase):
     @classmethod
     def up(cls):
         # Add a libev edition manager to the localhost node
         # Make sure this manager is running and accessible at localhost before the test.
         # Example command:
-        # MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+        # MGR_PORT=6001 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
         # docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
         #   --name ssm-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
         #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
 
         models.SSManager(
             node=models.Node.objects.get(name='ss-libev-localhost'),
             interface=models.InterfaceList.LOCALHOST,
@@ -446,15 +445,15 @@
             server_edition=models.ServerEditionList.LIBEV,
             is_v2ray_enabled=False,
         ).save()
 
         # Add a libev edition manager to the private node
         # Make sure this manager is running and accessible at private ip before the test.
         # Example command:
-        # MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+        # MGR_PORT=6002 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
         # docker run -d -p <private_ip>:$MGR_PORT:$MGR_PORT/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS \
         #   --name ssm-ss-libev-private shadowsocks/shadowsocks-libev:edge \
         #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         models.SSManager(
             node=models.Node.objects.get(name='ss-libev-private'),
             interface=models.InterfaceList.PRIVATE,
             port=6002,
@@ -462,15 +461,15 @@
             server_edition=models.ServerEditionList.LIBEV,
             is_v2ray_enabled=False,
         ).save()
 
         # Add a libev edition manager to the public node
         # Make sure this manager is running and accessible at private ip before the test.
         # Example command:
-        # MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+        # MGR_PORT=6003 SS_PORTS=8385 ENCRYPT=aes-256-cfb
         # docker run -d -p <private_ip>:$MGR_PORT:$MGR_PORT/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS/UDP -p <private_ip>:$SS_PORTS:$SS_PORTS \
         #   --name ssm-ss-libev-public shadowsocks/shadowsocks-libev:edge \
         #   ss-manager --manager-address 0.0.0.0:$MGR_PORT --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         models.SSManager(
             node=models.Node.objects.get(name='ss-libev-public'),
             interface=models.InterfaceList.PUBLIC,
             port=6003,
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks/urls.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/celery.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/settings.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     'import_export',
     'rest_framework',
     'django_filters',
     'shadowsocks',
     'statistic',
     'notification',
     'domain',
+    'utils',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/shadowsocks_manager/urls.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/shadowsocks_manager/urls.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/singleton/models.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/singleton/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/admin.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/admin.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/models.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/models.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/serializers.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/serializers.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/statistic/tests.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/statistic/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from django.test import TestCase
 
 from shadowsocks.tests import AppTestCase as shadowsocksAppTestCase
 from statistic import models, serializers
 
 
 import logging
-# Get a logger for this module
-logger = logging.getLogger(__name__)
+# Get a logger for this django app
+logger = logging.getLogger(__name__.split('.')[0])
 # Set the logging level to make the output clean
 logger.setLevel(logging.ERROR)
 
 
 class BaseTestCase(TestCase):
     """
     A base test case for current app.
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/utils/celery.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/utils/celery.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/utils/createsuperuser.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/utils/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/utils/dotenv.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/utils/manage.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/utils/manage.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager/utils/viewsets.py` & `shadowsocks_manager-0.1.9/shadowsocks_manager/utils/viewsets.py`

 * *Files identical despite different names*

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/PKG-INFO` & `shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowsocks-manager
-Version: 0.1.8
+Version: 0.1.9
 Summary: A shadowsocks manager for multi-user and traffic statistics
 Home-page: https://github.com/alexzhangs/shadowsocks-manager
 Author: Alex
 Author-email: Alex <alexzhangs@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Alex Zhang
@@ -70,23 +70,26 @@
 Requires-Dist: django-celery-results; python_version > "2.7"
 Requires-Dist: django-enumfield<3.0; python_version <= "2.7"
 Requires-Dist: django-enumfield; python_version > "2.7"
 Requires-Dist: django-filter~=1.1; python_version <= "2.7"
 Requires-Dist: django-filter; python_version > "2.7"
 Requires-Dist: django-import-export
 Requires-Dist: djangorestframework
+Requires-Dist: dns-lexicon[full]
+Requires-Dist: dnspython
 Requires-Dist: docopt
 Requires-Dist: ipaddress; python_version < "3.3"
 Requires-Dist: psutil
 Requires-Dist: python-crontab==2.6.0; python_version <= "2.7"
 Requires-Dist: python-crontab; python_version > "2.7"
 Requires-Dist: python-decouple
 Requires-Dist: python-memcached==1.59
 Requires-Dist: pytz
 Requires-Dist: requests
+Requires-Dist: tldextract
 Requires-Dist: uWSGI
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: codecov-cli; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -367,35 +370,35 @@
     # run memcached, used by django cache
     docker run -d -p 11211:11211 --name ssm-dev-memcached memcached
 
     # run rabbitmq, used by celery
     docker run -d -p 5672:5672 --name ssm-dev-rabbitmq rabbitmq
 
     # run shadowsocks-libev, simulate localhost node
-    MGR_PORT=6001 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    MGR_PORT=6001 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
     docker run -d -p 127.0.0.1:$MGR_PORT:$MGR_PORT/UDP \
         -p 127.0.0.1:$SS_PORTS:$SS_PORTS/UDP -p 127.0.0.1:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-localhost shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
 
     # get the private IP address of the host, double check the result, it might not be correct
     PRIVATE_IP=$(ipconfig getifaddr en0 2>/dev/null || hostname -i | awk '{print $1}' 2>/dev/null)
     echo "PRIVATE_IP=$PRIVATE_IP"
 
     # run shadowsocks-libev, simulate private IP node
-    MGR_PORT=6002 SS_PORTS=8381-8479 ENCRYPT=aes-256-cfb
+    MGR_PORT=6002 SS_PORTS=8381-8384 ENCRYPT=aes-256-cfb
     docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
         -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-private shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
         
     # run shadowsocks-libev, simulate public IP node
-    MGR_PORT=6003 SS_PORTS=8480 ENCRYPT=aes-256-cfb
+    MGR_PORT=6003 SS_PORTS=8385 ENCRYPT=aes-256-cfb
     docker run -d -p $PRIVATE_IP:$MGR_PORT:$MGR_PORT/UDP \
         -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS/UDP -p $PRIVATE_IP:$SS_PORTS:$SS_PORTS \
         --name ssm-dev-ss-libev-public shadowsocks/shadowsocks-libev:edge \
         ss-manager --manager-address 0.0.0.0:$MGR_PORT \
         --executable /usr/local/bin/ss-server -m $ENCRYPT -s 0.0.0.0 -u
     ```
 
@@ -435,16 +438,16 @@
 1. Test the Django code
 
     Make sure the memcached and rabbitmq are running, and also the 3 shadowsocks-libev node are running.
 
     ```sh
     ssm-test -t
 
-    # or use the django test command directly for more options
-    ssm-manage test --no-input -v 2
+    # or use the django test command directly for more options, use the `-t .` for the Python 2.7 compatibility
+    ssm-manage test --no-input -v 2 -t .
     ```
 
 1. Test the Django code with coverage
 
     ```sh
     pip install coverage
     ssm-test -c
@@ -502,15 +505,18 @@
     # --use-pep517 is used together to make sure the PEP 517 is tested
     pip install --no-binary shadowsocks-manager --use-pep517 shadowsocks-manager
     ```
 
 1. Build the docker image
 
     ```sh
-    docker build -t alexzhangs/shadowsocks-manager .
+    docker build -t alexzhangs/shadowsocks-manager -f docker/debian/Dockerfile .
+
+    # or use:
+    bash docker/docker-build-and-run.sh
     ```
 
 ### 8.2. CI/CD
 
 Github Actions is currently used for the CI/CD.
 Travis CI is removed due to the limitation of the free plan.
 
@@ -520,47 +526,71 @@
 * ci-testpypi.yml: Build and upload the package to TestPyPI.
 * ci-pypi.yml: Build and upload the package to PyPI. It can be triggered by the tag: `ci-pypi` or `ci-pypi-(major|minor|patch|suffx)`.
 * ci-docker.yml: Build and push the docker image to Docker Hub. It can be triggered by the Github release.
 
 
 ## 9. Troubleshooting
 
-1. Check the logs
+1. Docker
 
     ```
-    # supervisor
-    cat /var/log/supervisor/supervisord.log
+    # containers
+    docker ps -a
+
+    # network
+    docker network ls
+
+    # logs
+    docker logs <container_id>
+    ```
+
+1. Check the logs (inside container)
+
+    ```
+    # supervisor (debian)
+    cat /var/log/supervisor/supervisord.log 
+
+    # supervisor (alpine)
+    cat /var/log/supervisord.log
 
     # uWSGI
     cat /var/log/ssm-uwsgi.log
 
     # Celery
     cat /var/log/ssm-cerlery*
     ```
 
-1. Check the services
+1. Check the services (inside container)
 
     ```
     # nginx
-    service nginx {status|start|stop|reload}
+    nginx -s {stop|quit|reopen|reload}
 
     # supervisor
-    service supervisord {status|start|stop|restart}
     supervisorctl reload
     supervisorctl start all
 
     # uWSGI
     supervisorctl start ssm-uwsgi
 
     # Celery
     supervisorctl start ssm-celery-worker
     supervisorctl start ssm-celery-beat
 
-    # Docker
-    docker ps
+    # acme.sh
+    acme.sh --list
+    crontab -l
+    ls -l /root/.acme.sh
+
+    # volume data
+    ls -la /var/local/ssm
+
+    # setup done files
+    ls -la /var/local/ssm/.*done
+    ls -la /root/.*done
     ```
 
 1. Check the listening ports and processes (Linux)
 
     ```
     # TCP
     netstat -tanp
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/SOURCES.txt` & `shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 shadowsocks_manager/domain/admin.py
 shadowsocks_manager/domain/apps.py
 shadowsocks_manager/domain/models.py
 shadowsocks_manager/domain/serializers.py
 shadowsocks_manager/domain/tests.py
 shadowsocks_manager/domain/urls.py
 shadowsocks_manager/domain/views.py
-shadowsocks_manager/domain/fixtures/nameserver.json
+shadowsocks_manager/domain/management/__init__.py
+shadowsocks_manager/domain/management/commands/__init__.py
+shadowsocks_manager/domain/management/commands/domain_domain.py
+shadowsocks_manager/domain/management/commands/domain_nameserver.py
+shadowsocks_manager/domain/management/commands/domain_record.py
 shadowsocks_manager/domain/migrations/__init__.py
 shadowsocks_manager/dynamicmethod/__init__.py
 shadowsocks_manager/dynamicmethod/admin.py
 shadowsocks_manager/dynamicmethod/apps.py
 shadowsocks_manager/dynamicmethod/models.py
 shadowsocks_manager/dynamicmethod/tests.py
 shadowsocks_manager/dynamicmethod/views.py
```

### Comparing `shadowsocks_manager-0.1.8/shadowsocks_manager.egg-info/requires.txt` & `shadowsocks_manager-0.1.9/shadowsocks_manager.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 boto3
 celery
 Django<4
 django-allowedsites-dynamic
 django-cache-lock
 django-import-export
 djangorestframework
+dns-lexicon[full]
+dnspython
 docopt
 psutil
 python-decouple
 python-memcached==1.59
 pytz
 requests
+tldextract
 uWSGI
 
 [:python_version < "3.3"]
 ipaddress
 
 [:python_version <= "2.7"]
 django-celery-beat==1.6.0
```

