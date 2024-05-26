# Comparing `tmp/django_debug_toolbar-4.2.0.tar.gz` & `tmp/django_debug_toolbar-4.3.0.tar.gz`

## Comparing `django_debug_toolbar-4.2.0.tar` & `django_debug_toolbar-4.3.0.tar`

### file list

```diff
@@ -1,199 +1,200 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.editorconfig
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.eslintrc.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/Makefile
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/requirements_dev.txt
--rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/setup.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tox.ini
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.tx/config
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/_stubs.py
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/apps.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/decorators.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/forms.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/middleware.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/settings.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/toolbar.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/urls.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/utils.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/views.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/management/commands/__init__.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/management/commands/debugsqlshell.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/__init__.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/cache.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/headers.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/profiling.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/redirects.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/request.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/settings.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/signals.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/staticfiles.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/timer.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/versions.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/history/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/history/forms.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/history/panel.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/history/views.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/forms.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/panel.py
--rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/tracking.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/utils.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/views.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/templates/__init__.py
--rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/templates/panel.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/panels/templates/views.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/css/print.css
--rw-r--r--   0        0        0    12621 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/css/toolbar.css
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/history.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/redirect.js
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/timer.js
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/toolbar.js
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/utils.js
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/base.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/redirect.html
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/cache.html
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/headers.html
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/history.html
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/request.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/settings.html
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/signals.html
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql.html
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/template_source.html
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/templates.html
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/timer.html
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/versions.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/debug_toolbar/templatetags/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/Makefile
--rw-r--r--   0        0        0    25690 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/changes.rst
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/checks.rst
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/commands.rst
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/conf.py
--rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/configuration.rst
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/contributing.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/index.rst
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/installation.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/make.bat
--rw-r--r--   0        0        0    12827 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/panels.rst
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/docs/tips.rst
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/__init__.py
--rw-r--r--   0        0        0    84160 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/django-debug-toolbar.png
--rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/example.db
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/manage.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/screenshot.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/settings.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/urls.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/views.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/wsgi.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/static/test.css
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/templates/index.html
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/templates/htmx/boost.html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/templates/jquery/index.html
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/templates/mootools/index.html
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/templates/prototype/index.html
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/example/templates/turbo/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/base.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/context_processors.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/forms.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/loaders.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/middleware.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/models.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/settings.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/sync.py
--rw-r--r--   0        0        0    10081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/test_checks.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/test_decorators.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/test_forms.py
--rw-r--r--   0        0        0    30273 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/test_integration.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/urls.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/urls_invalid.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/urls_use_package_urls.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/views.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/additional_static/base.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/commands/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/commands/test_debugsqlshell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_cache.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_custom.py
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_history.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_profiling.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_redirects.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_request.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_settings.py
--rw-r--r--   0        0        0    29916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_sql.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_staticfiles.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_template.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/panels/test_versions.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/base.html
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/basic.html
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/jinja2/basic.jinja
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/registration/login.html
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/sql/flat.html
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/sql/included.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/tests/templates/sql/nested.html
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/LICENSE
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/README.rst
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 django_debug_toolbar-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.eslintrc.js
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/Makefile
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/requirements_dev.txt
+-rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/setup.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tox.ini
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.tx/config
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/_stubs.py
+-rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/apps.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/decorators.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/forms.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/middleware.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/settings.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/toolbar.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/urls.py
+-rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/utils.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/views.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/management/commands/__init__.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/management/commands/debugsqlshell.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/__init__.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/cache.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/headers.py
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/profiling.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/redirects.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/request.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/settings.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/signals.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/staticfiles.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/timer.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/versions.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/forms.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/panel.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/views.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/forms.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/panel.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/tracking.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/utils.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/views.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/__init__.py
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/panel.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/views.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/css/print.css
+-rw-r--r--   0        0        0    12621 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/css/toolbar.css
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/history.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/redirect.js
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/timer.js
+-rw-r--r--   0        0        0    13578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/toolbar.js
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/utils.js
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/base.html
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/redirect.html
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/cache.html
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/headers.html
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history.html
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/settings.html
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/signals.html
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql.html
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/template_source.html
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/templates.html
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/timer.html
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/versions.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templatetags/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/Makefile
+-rw-r--r--   0        0        0    26588 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/changes.rst
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/checks.rst
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/commands.rst
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/conf.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/configuration.rst
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/contributing.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/index.rst
+-rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/installation.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/make.bat
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/panels.rst
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/tips.rst
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/__init__.py
+-rw-r--r--   0        0        0    84160 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/django-debug-toolbar.png
+-rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/example.db
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/manage.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/screenshot.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/settings.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/urls.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/views.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/wsgi.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/static/test.css
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/index.html
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/htmx/boost.html
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/jquery/index.html
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/mootools/index.html
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/prototype/index.html
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/turbo/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/base.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/context_processors.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/forms.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/loaders.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/middleware.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/models.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/settings.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/sync.py
+-rw-r--r--   0        0        0    10081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_checks.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_decorators.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_forms.py
+-rw-r--r--   0        0        0    31235 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_integration.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/urls.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/urls_invalid.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/urls_use_package_urls.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/views.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/additional_static/base.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/commands/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/commands/test_debugsqlshell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_cache.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_custom.py
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_history.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_profiling.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_redirects.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_request.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_settings.py
+-rw-r--r--   0        0        0    29916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_sql.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_staticfiles.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_template.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_versions.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/base.html
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/basic.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/ajax/ajax.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/jinja2/basic.jinja
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/registration/login.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/sql/flat.html
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/sql/included.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/sql/nested.html
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/LICENSE
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/README.rst
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/PKG-INFO
```

### Comparing `django_debug_toolbar-4.2.0/.pre-commit-config.yaml` & `django_debug_toolbar-4.3.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
     -   id: check-toml
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
     -   id: mixed-line-ending
     -   id: file-contents-sorter
         files: docs/spelling_wordlist.txt
 -   repo: https://github.com/pycqa/doc8
     rev: v1.1.1
     hooks:
     -   id: doc8
 -   repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.14.0
+    rev: 1.15.0
     hooks:
     -   id: django-upgrade
         args: [--target-version, "3.2"]
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
     -   id: rst-backticks
     -   id: rst-directive-colons
 -   repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.1
+    rev: v4.0.0-alpha.8
     hooks:
     -   id: prettier
+        entry: env PRETTIER_LEGACY_CLI=1 prettier
         types_or: [javascript, css]
         args:
-        -  --trailing-comma=es5
+        - --trailing-comma=es5
 -   repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.46.0
+    rev: v8.56.0
     hooks:
     -   id: eslint
         files: \.js?$
         types: [file]
         args:
         - --fix
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.0.282'
+    rev: 'v0.1.11'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
--   repo: https://github.com/psf/black
-    rev: 23.7.0
-    hooks:
-    -   id: black
-        language_version: python3
-        entry: black --target-version=py38
+      - id: ruff-format
 -   repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.13.0
+    rev: 1.5.3
     hooks:
       - id: pyproject-fmt
 -   repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.13
+    rev: v0.15
     hooks:
       - id: validate-pyproject
```

### Comparing `django_debug_toolbar-4.2.0/CODE_OF_CONDUCT.md` & `django_debug_toolbar-4.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/Makefile` & `django_debug_toolbar-4.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/setup.py` & `django_debug_toolbar-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tox.ini` & `django_debug_toolbar-4.3.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tox]
 isolated_build = true
 envlist =
     docs
     packaging
     py{38,39,310}-dj32-{sqlite,postgresql,postgis,mysql}
-    py310-dj40-sqlite
     py{310,311}-dj41-{sqlite,postgresql,postgis,mysql}
-    py{310,311}-dj{42,main}-{sqlite,postgresql,psycopg3,postgis,mysql}
+    py{310,311,312}-dj{42,50,main}-{sqlite,postgresql,psycopg3,postgis,mysql}
 
 [testenv]
 deps =
     dj32: django~=3.2.9
-    dj40: django~=4.0.0
     dj41: django~=4.1.3
     dj42: django~=4.2.1
+    dj50: django~=5.0a1
     djmain: https://github.com/django/django/archive/main.tar.gz
     postgresql: psycopg2-binary
     psycopg3: psycopg[binary]
     postgis: psycopg2-binary
     mysql: mysqlclient
     coverage[toml]
     Jinja2
@@ -45,33 +44,37 @@
     DB_HOST = {env:DB_HOST:localhost}
     DB_PASSWORD =  {env:DB_PASSWORD:debug_toolbar}
     DJANGO_SETTINGS_MODULE = tests.settings
 allowlist_externals = make
 pip_pre = True
 commands = python -b -W always -m coverage run -m django test -v2 {posargs:tests}
 
-[testenv:py{38,39,310,311}-dj{32,40,41,42,main}-{postgresql,psycopg3}]
+
+[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-{postgresql,psycopg3}]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = postgresql
     DB_PORT = {env:DB_PORT:5432}
 
-[testenv:py{38,39,310,311}-dj{32,40,41,42,main}-postgis]
+
+[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-postgis]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = postgis
     DB_PORT = {env:DB_PORT:5432}
 
-[testenv:py{38,39,310,311}-dj{32,40,41,42,main}-mysql]
+
+[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-mysql]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = mysql
     DB_PORT = {env:DB_PORT:3306}
 
-[testenv:py{38,39,310,311}-dj{32,40,41,42,main}-sqlite]
+
+[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-sqlite]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = sqlite3
     DB_NAME = ":memory:"
 
 [testenv:docs]
 commands = make -C {toxinidir}/docs {posargs:spelling}
@@ -91,14 +94,15 @@
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
+    3.12: py312
 
 [gh-actions:env]
 DB_BACKEND =
     mysql: mysql
     postgresql: postgresql
     psycopg3: psycopg3
     postgis: postgis
```

### Comparing `django_debug_toolbar-4.2.0/.github/workflows/release.yml` & `django_debug_toolbar-4.3.0/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 jobs:
   build:
     if: github.repository == 'jazzband/django-debug-toolbar'
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U build hatchling twine
```

### Comparing `django_debug_toolbar-4.2.0/.github/workflows/test.yml` & `django_debug_toolbar-4.3.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   mysql:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     services:
       mariadb:
         image: mariadb
         env:
           MARIADB_ROOT_PASSWORD: debug_toolbar
         options: >-
@@ -26,20 +26,21 @@
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
         ports:
         - 3306:3306
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        allow-prereleases: true
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
@@ -73,22 +74,24 @@
 
   postgres:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
         database: [postgresql, postgis]
-        # Add psycopg3 to our matrix for 3.10 and 3.11
+        # Add psycopg3 to our matrix for modern python versions
         include:
             - python-version: '3.10'
               database: psycopg3
             - python-version: '3.11'
               database: psycopg3
+            - python-version: '3.12'
+              database: psycopg3
 
     services:
       postgres:
         image: postgis/postgis:14-3.1
         env:
           POSTGRES_DB: debug_toolbar
           POSTGRES_USER: debug_toolbar
@@ -98,20 +101,21 @@
         options: >-
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        allow-prereleases: true
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
@@ -148,23 +152,24 @@
 
   sqlite:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        allow-prereleases: true
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
@@ -194,15 +199,15 @@
         path: ".coverage.*"
 
   coverage:
     name: Check coverage.
     runs-on: "ubuntu-latest"
     needs: [sqlite, mysql, postgres]
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           # Use latest, so it understands all syntax.
           python-version: "3.11"
 
       - run: python -m pip install --upgrade coverage[toml]
 
@@ -226,15 +231,15 @@
 
   lint:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Get pip cache dir
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/_stubs.py` & `django_debug_toolbar-4.3.0/debug_toolbar/_stubs.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/apps.py` & `django_debug_toolbar-4.3.0/debug_toolbar/apps.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/decorators.py` & `django_debug_toolbar-4.3.0/debug_toolbar/decorators.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/forms.py` & `django_debug_toolbar-4.3.0/debug_toolbar/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/middleware.py` & `django_debug_toolbar-4.3.0/debug_toolbar/middleware.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/settings.py` & `django_debug_toolbar-4.3.0/debug_toolbar/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "PROFILER_MAX_DEPTH": 10,
     "PROFILER_THRESHOLD_RATIO": 8,
     "SHOW_TEMPLATE_CONTEXT": True,
     "SKIP_TEMPLATE_PREFIXES": ("django/forms/widgets/", "admin/widgets/"),
     "SQL_WARNING_THRESHOLD": 500,  # milliseconds
     "OBSERVE_REQUEST_CALLBACK": "debug_toolbar.toolbar.observe_request",
     "TOOLBAR_LANGUAGE": None,
+    "UPDATE_ON_FETCH": False,
 }
 
 
 @lru_cache(maxsize=None)
 def get_config():
     USER_CONFIG = getattr(settings, "DEBUG_TOOLBAR_CONFIG", {})
     CONFIG = CONFIG_DEFAULTS.copy()
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/toolbar.py` & `django_debug_toolbar-4.3.0/debug_toolbar/toolbar.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/utils.py` & `django_debug_toolbar-4.3.0/debug_toolbar/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,21 +158,23 @@
     line = exception_info["line"]
     source_lines = exception_info["source_lines"]
     name = exception_info["name"]
     return line, source_lines, name
 
 
 def get_name_from_obj(obj: Any) -> str:
-    name = obj.__name__ if hasattr(obj, "__name__") else obj.__class__.__name__
-
-    if hasattr(obj, "__module__"):
-        module = obj.__module__
-        name = f"{module}.{name}"
-
-    return name
+    """Get the best name as `str` from a view or a object."""
+    # This is essentially a rewrite of the `django.contrib.admindocs.utils.get_view_name`
+    # https://github.com/django/django/blob/9a22d1769b042a88741f0ff3087f10d94f325d86/django/contrib/admindocs/utils.py#L26-L32
+    if hasattr(obj, "view_class"):
+        klass = obj.view_class
+        return f"{klass.__module__}.{klass.__qualname__}"
+    mod_name = obj.__module__
+    view_name = getattr(obj, "__qualname__", obj.__class__.__name__)
+    return mod_name + "." + view_name
 
 
 def getframeinfo(frame: Any, context: int = 1) -> inspect.Traceback:
     """
     Get information about a frame or traceback object.
 
     A tuple of five things is returned: the filename, the line number of
@@ -207,15 +209,15 @@
     else:
         lines = index = None
 
     return inspect.Traceback(filename, lineno, frame.f_code.co_name, lines, index)
 
 
 def get_sorted_request_variable(
-    variable: Union[Dict[str, Any], QueryDict]
+    variable: Union[Dict[str, Any], QueryDict],
 ) -> Dict[str, Union[List[Tuple[str, Any]], Any]]:
     """
     Get a data structure for showing a sorted list of variables from the
     request data.
     """
     try:
         if isinstance(variable, dict):
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/views.py` & `django_debug_toolbar-4.3.0/debug_toolbar/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/de/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/en/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/es/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/he/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/id/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/it/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po` & `django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/management/commands/debugsqlshell.py` & `django_debug_toolbar-4.3.0/debug_toolbar/management/commands/debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/__init__.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/cache.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/headers.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/profiling.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/profiling.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,18 +38,22 @@
         Check if the function is from the project code.
 
         Project code is identified by the BASE_DIR setting
         which is used in Django projects by default.
         """
         if hasattr(settings, "BASE_DIR"):
             file_name, _, _ = self.func
-            return (
-                str(settings.BASE_DIR) in file_name
-                and "/site-packages/" not in file_name
-                and "/dist-packages/" not in file_name
+            base_dir = str(settings.BASE_DIR)
+
+            file_name = os.path.normpath(file_name)
+            base_dir = os.path.normpath(base_dir)
+
+            return file_name.startswith(base_dir) and not any(
+                directory in file_name.split(os.path.sep)
+                for directory in ["site-packages", "dist-packages"]
             )
         return None
 
     def func_std_string(self):  # match what old profile produced
         func_name = self.func
         if func_name[:2] == ("~", 0):
             # special case for built-in functions
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/redirects.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/request.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/settings.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/signals.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/signals.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/staticfiles.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/staticfiles.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/timer.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/versions.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/history/panel.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/history/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/history/views.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/history/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/forms.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/panel.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/tracking.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/tracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,29 +105,14 @@
 
 
 class NormalCursorMixin(DjDTCursorWrapperMixin):
     """
     Wraps a cursor and logs queries.
     """
 
-    def _quote_expr(self, element):
-        if isinstance(element, str):
-            return "'%s'" % element.replace("'", "''")
-        else:
-            return repr(element)
-
-    def _quote_params(self, params):
-        if not params:
-            return params
-        if isinstance(params, dict):
-            return {key: self._quote_expr(value) for key, value in params.items()}
-        if isinstance(params, tuple):
-            return tuple(self._quote_expr(p) for p in params)
-        return [self._quote_expr(p) for p in params]
-
     def _decode(self, param):
         if PostgresJson and isinstance(param, PostgresJson):
             # psycopg3
             if hasattr(param, "obj"):
                 return param.dumps(param.obj)
             # psycopg2
             if hasattr(param, "adapted"):
@@ -153,17 +138,15 @@
         # Django's psycopg3 backend creates a new cursor in its implementation of the
         # .last_executed_query() method.  To avoid wrapping that cursor, temporarily set
         # the DatabaseWrapper's ._djdt_logger attribute to None.  This will cause the
         # monkey-patched .cursor() and .chunked_cursor() methods to skip the wrapping
         # process during the .last_executed_query() call.
         self.db._djdt_logger = None
         try:
-            return self.db.ops.last_executed_query(
-                self.cursor, sql, self._quote_params(params)
-            )
+            return self.db.ops.last_executed_query(self.cursor, sql, params)
         finally:
             self.db._djdt_logger = self.logger
 
     def _record(self, method, sql, params):
         alias = self.db.alias
         vendor = self.db.vendor
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/utils.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/sql/views.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/templates/panel.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,66 +79,19 @@
             or template.name.startswith(
                 tuple(self.toolbar.config["SKIP_TEMPLATE_PREFIXES"])
             )
         )
         if is_debug_toolbar_template:
             return
 
-        context_list = []
-        for context_layer in context.dicts:
-            if hasattr(context_layer, "items") and context_layer:
-                # Check if the layer is in the cache.
-                pformatted = None
-                for key_values, _pformatted in self.pformat_layers:
-                    if key_values == context_layer:
-                        pformatted = _pformatted
-                        break
-
-                if pformatted is None:
-                    temp_layer = {}
-                    for key, value in context_layer.items():
-                        # Replace any request elements - they have a large
-                        # Unicode representation and the request data is
-                        # already made available from the Request panel.
-                        if isinstance(value, http.HttpRequest):
-                            temp_layer[key] = "<<request>>"
-                        # Replace the debugging sql_queries element. The SQL
-                        # data is already made available from the SQL panel.
-                        elif key == "sql_queries" and isinstance(value, list):
-                            temp_layer[key] = "<<sql_queries>>"
-                        # Replace LANGUAGES, which is available in i18n context
-                        # processor
-                        elif key == "LANGUAGES" and isinstance(value, tuple):
-                            temp_layer[key] = "<<languages>>"
-                        # QuerySet would trigger the database: user can run the
-                        # query from SQL Panel
-                        elif isinstance(value, (QuerySet, RawQuerySet)):
-                            temp_layer[key] = "<<{} of {}>>".format(
-                                value.__class__.__name__.lower(),
-                                value.model._meta.label,
-                            )
-                        else:
-                            token = allow_sql.set(False)  # noqa: FBT003
-                            try:
-                                saferepr(value)  # this MAY trigger a db query
-                            except SQLQueryTriggered:
-                                temp_layer[key] = "<<triggers database query>>"
-                            except UnicodeEncodeError:
-                                temp_layer[key] = "<<Unicode encode error>>"
-                            except Exception:
-                                temp_layer[key] = "<<unhandled exception>>"
-                            else:
-                                temp_layer[key] = value
-                            finally:
-                                allow_sql.reset(token)
-                    pformatted = pformat(temp_layer)
-                    self.pformat_layers.append((context_layer, pformatted))
-                context_list.append(pformatted)
-
-        kwargs["context"] = context_list
+        kwargs["context"] = [
+            context_layer
+            for context_layer in context.dicts
+            if hasattr(context_layer, "items") and context_layer
+        ]
         kwargs["context_processors"] = getattr(context, "context_processors", None)
         self.templates.append(kwargs)
 
     # Implement the Panel API
 
     nav_title = _("Templates")
 
@@ -163,14 +116,71 @@
 
     def enable_instrumentation(self):
         template_rendered.connect(self._store_template_info)
 
     def disable_instrumentation(self):
         template_rendered.disconnect(self._store_template_info)
 
+    def process_context_list(self, context_layers):
+        context_list = []
+        for context_layer in context_layers:
+            # Check if the layer is in the cache.
+            pformatted = None
+            for key_values, _pformatted in self.pformat_layers:
+                if key_values == context_layer:
+                    pformatted = _pformatted
+                    break
+
+            if pformatted is None:
+                temp_layer = {}
+                for key, value in context_layer.items():
+                    # Do not force evaluating LazyObject
+                    if hasattr(value, "_wrapped"):
+                        # SimpleLazyObject has __repr__ which includes actual value
+                        # if it has been already evaluated
+                        temp_layer[key] = repr(value)
+                    # Replace any request elements - they have a large
+                    # Unicode representation and the request data is
+                    # already made available from the Request panel.
+                    elif isinstance(value, http.HttpRequest):
+                        temp_layer[key] = "<<request>>"
+                    # Replace the debugging sql_queries element. The SQL
+                    # data is already made available from the SQL panel.
+                    elif key == "sql_queries" and isinstance(value, list):
+                        temp_layer[key] = "<<sql_queries>>"
+                    # Replace LANGUAGES, which is available in i18n context
+                    # processor
+                    elif key == "LANGUAGES" and isinstance(value, tuple):
+                        temp_layer[key] = "<<languages>>"
+                    # QuerySet would trigger the database: user can run the
+                    # query from SQL Panel
+                    elif isinstance(value, (QuerySet, RawQuerySet)):
+                        temp_layer[
+                            key
+                        ] = f"<<{value.__class__.__name__.lower()} of {value.model._meta.label}>>"
+                    else:
+                        token = allow_sql.set(False)  # noqa: FBT003
+                        try:
+                            saferepr(value)  # this MAY trigger a db query
+                        except SQLQueryTriggered:
+                            temp_layer[key] = "<<triggers database query>>"
+                        except UnicodeEncodeError:
+                            temp_layer[key] = "<<Unicode encode error>>"
+                        except Exception:
+                            temp_layer[key] = "<<unhandled exception>>"
+                        else:
+                            temp_layer[key] = value
+                        finally:
+                            allow_sql.reset(token)
+                pformatted = pformat(temp_layer)
+                self.pformat_layers.append((context_layer, pformatted))
+            context_list.append(pformatted)
+
+        return context_list
+
     def generate_stats(self, request, response):
         template_context = []
         for template_data in self.templates:
             info = {}
             # Clean up some info about templates
             template = template_data["template"]
             if hasattr(template, "origin") and template.origin and template.origin.name:
@@ -178,16 +188,19 @@
                 template.origin_hash = signing.dumps(template.origin.name)
             else:
                 template.origin_name = _("No origin")
                 template.origin_hash = ""
             info["template"] = template
             # Clean up context for better readability
             if self.toolbar.config["SHOW_TEMPLATE_CONTEXT"]:
-                context_list = template_data.get("context", [])
-                info["context"] = "\n".join(context_list)
+                if "context_list" not in template_data:
+                    template_data["context_list"] = self.process_context_list(
+                        template_data.get("context", [])
+                    )
+                info["context"] = "\n".join(template_data["context_list"])
             template_context.append(info)
 
         # Fetch context_processors/template_dirs from any template
         if self.templates:
             context_processors = self.templates[0]["context_processors"]
             template = self.templates[0]["template"]
             # django templates have the 'engine' attribute, while jinja
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/panels/templates/views.py` & `django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/css/toolbar.css` & `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/css/toolbar.css`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/history.js` & `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/history.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -103,8 +103,11 @@
     event.preventDefault();
     switchHistory(this.dataset.storeId);
 });
 
 $$.on(djDebug, "click", ".refreshHistory", function(event) {
     event.preventDefault();
     refreshHistory();
-});
+});
+// We don't refresh the whole toolbar each fetch or ajax request,
+// so we need to refresh the history when we open the panel
+$$.onPanelRender(djDebug, "HistoryPanel", refreshHistory);
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/timer.js` & `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/timer.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/toolbar.js` & `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/toolbar.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -18,16 +18,18 @@
     // to the element should be avoided because the entire DOM could
     // be reloaded such as via HTMX boosting.
     return document.getElementById("djDebug");
 }
 
 const djdt = {
     handleDragged: false,
+    needUpdateOnFetch: false,
     init() {
         const djDebug = getDebugElement();
+        djdt.needUpdateOnFetch = djDebug.dataset.updateOnFetch === "True";
         $$.on(djDebug, "click", "#djDebugPanelList li a", function(event) {
             event.preventDefault();
             if (!this.className) {
                 return;
             }
             const panelId = this.className;
             const current = document.getElementById(panelId);
@@ -232,15 +234,15 @@
             e.classList.remove("djdt-active");
         });
     },
     ensureHandleVisibility() {
         const handle = document.getElementById("djDebugToolbarHandle");
         // set handle position
         const handleTop = Math.min(
-            localStorage.getItem("djdt.top") || 0,
+            localStorage.getItem("djdt.top") || 265,
             window.innerHeight - handle.offsetWidth
         );
         handle.style.top = handleTop + "px";
     },
     hideToolbar() {
         djdt.hidePanels();
 
@@ -280,15 +282,17 @@
             document.getElementById("djDebug").dataset.sidebarUrl;
         const slowjax = debounce(ajax, 200);
 
         function handleAjaxResponse(storeId) {
             storeId = encodeURIComponent(storeId);
             const dest = `${sidebarUrl}?store_id=${storeId}`;
             slowjax(dest).then(function(data) {
-                replaceToolbarState(storeId, data);
+                if (djdt.needUpdateOnFetch) {
+                    replaceToolbarState(storeId, data);
+                }
             });
         }
 
         // Patch XHR / traditional AJAX requests
         const origOpen = XMLHttpRequest.prototype.open;
         XMLHttpRequest.prototype.open = function() {
             this.addEventListener("load", function() {
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/static/debug_toolbar/js/utils.js` & `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/utils.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/base.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
      data-render-panel-url="{% url 'djdt:render_panel' %}"
      {% endif %}
      {% url 'djdt:history_sidebar' as history_url %}
      {% if history_url %}
      data-sidebar-url="{{ history_url }}"
      {% endif %}
      data-default-show="{% if toolbar.config.SHOW_COLLAPSED %}false{% else %}true{% endif %}"
-     {{ toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }}>
+     {{ toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }}  data-update-on-fetch="{{ toolbar.config.UPDATE_ON_FETCH }}">
   <div class="djdt-hidden" id="djDebugToolbar">
     <ul id="djDebugPanelList">
       <li><a id="djHideToolBarButton" href="#" title="{% trans 'Hide toolbar' %}">{% trans "Hide" %} »</a></li>
       {% for panel in toolbar.panels %}
         {% include "debug_toolbar/includes/panel_button.html" %}
       {% endfor %}
     </ul>
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 {% endblock %} {% block js %}
 {% endblock %}
 % if not toolbar.should_render_panels %} data-store-id="{{ toolbar.store_id }}"
 data-render-panel-url="{% url 'djdt:render_panel' %}" {% endif %} {% url 'djdt:
 history_sidebar' as history_url %} {% if history_url %} data-sidebar-url="{
 { history_url }}" {% endif %} data-default-show="{% if
 toolbar.config.SHOW_COLLAPSED %}false{% else %}true{% endif %}" {
-{ toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }}>
+{ toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }} data-update-on-fetch="{
+{ toolbar.config.UPDATE_ON_FETCH }}">
     * _{_%_ _t_r_a_n_s_ _"_H_i_d_e_"_ _%_}_ _Â_»
     * {% for panel in toolbar.panels %} {% include "debug_toolbar/includes/
       panel_button.html" %} {% endfor %}
 DJDT
 {% for panel in toolbar.panels %} {% include "debug_toolbar/includes/
 panel_content.html" %} {% endfor %}
```

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/redirect.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/redirect.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/cache.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/cache.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/headers.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/headers.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/history.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/request.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/templates.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/templates.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/debug_toolbar/templates/debug_toolbar/panels/timer.html` & `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/timer.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/docs/Makefile` & `django_debug_toolbar-4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/docs/changes.rst` & `django_debug_toolbar-4.3.0/docs/changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 Change log
 ==========
 
 Pending
 -------
 
+4.3.0 (2024-02-01)
+------------------
+
+* Dropped support for Django 4.0.
+* Added Python 3.12 to test matrix.
+* Removed outdated third-party panels from the list.
+* Avoided the unnecessary work of recursively quoting SQL parameters.
+* Postponed context process in templates panel to include lazy evaluated
+  content.
+* Fixed template panel to avoid evaluating ``LazyObject`` when not already
+  evaluated.
+* Added support for Django 5.0.
+* Refactor the ``utils.get_name_from_obj`` to simulate the behavior of
+  ``django.contrib.admindocs.utils.get_view_name``.
+* Switched from black to the `ruff formatter
+  <https://astral.sh/blog/the-ruff-formatter>`__.
+* Changed the default position of the toolbar from top to the upper top
+  position.
+* Added the setting, ``UPDATE_ON_FETCH`` to control whether the
+  toolbar automatically updates to the latest AJAX request or not.
+  It defaults to ``False``.
+
 4.2.0 (2023-08-10)
 ------------------
 
 * Adjusted app directories system check to allow for nested template loaders.
 * Switched from flake8, isort and pyupgrade to `ruff
   <https://beta.ruff.rs/>`__.
 * Converted cookie keys to lowercase. Fixed the ``samesite`` argument to
```

### Comparing `django_debug_toolbar-4.2.0/docs/checks.rst` & `django_debug_toolbar-4.3.0/docs/checks.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/docs/commands.rst` & `django_debug_toolbar-4.3.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/docs/conf.py` & `django_debug_toolbar-4.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "Django Debug Toolbar"
 copyright = "{}, Django Debug Toolbar developers and contributors"
 copyright = copyright.format(datetime.date.today().year)
 
 # The full version, including alpha/beta/rc tags
-release = "4.2.0"
+release = "4.3.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `django_debug_toolbar-4.2.0/docs/configuration.rst` & `django_debug_toolbar-4.3.0/docs/configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,24 @@
   The language used to render the toolbar. If no value is supplied, then the
   application's current language will be used. This setting can be used to
   render the toolbar in a different language than what the application is
   rendered in. For example, if you wish to use English for development,
   but want to render your application in French, you would set this to
   ``"en-us"`` and :setting:`LANGUAGE_CODE` to ``"fr"``.
 
+.. _UPDATE_ON_FETCH:
+
+* ``UPDATE_ON_FETCH``
+
+  Default: ``False``
+
+  This controls whether the toolbar should update to the latest AJAX
+  request when it occurs. This is especially useful when using htmx
+  boosting or similar JavaScript techniques.
+
 Panel options
 ~~~~~~~~~~~~~
 
 * ``EXTRA_SIGNALS``
 
   Default: ``[]``
```

### Comparing `django_debug_toolbar-4.2.0/docs/contributing.rst` & `django_debug_toolbar-4.3.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/docs/installation.rst` & `django_debug_toolbar-4.3.0/docs/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 Process
 -------
 
 Each of the following steps needs to be configured for the Debug Toolbar to be
 fully functional.
 
+.. warning::
+
+    The Debug Toolbar does not currently support `Django's asynchronous views <https://docs.djangoproject.com/en/dev/topics/async/>`_.
+
 1. Install the Package
 ^^^^^^^^^^^^^^^^^^^^^^
 
 The recommended way to install the Debug Toolbar is via pip_:
 
 .. code-block:: console
```

### Comparing `django_debug_toolbar-4.2.0/docs/make.bat` & `django_debug_toolbar-4.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/docs/panels.rst` & `django_debug_toolbar-4.3.0/docs/panels.rst`

 * *Files 3% similar despite different names*

```diff
@@ -148,35 +148,14 @@
 Path: ``pyflame.djdt.panel.FlamegraphPanel``
 
 Displays a flame graph for visualizing the performance profile of the request,
 using Brendan Gregg's `flamegraph.pl script
 <https://github.com/brendangregg/FlameGraph/flamegraph.pl>`_ to perform the
 heavy lifting.
 
-HTML Tidy/Validator
-~~~~~~~~~~~~~~~~~~~
-
-URL: https://github.com/joymax/django-dtpanel-htmltidy
-
-Path: ``debug_toolbar_htmltidy.panels.HTMLTidyDebugPanel``
-
-HTML Tidy or HTML Validator is a custom panel that validates your HTML and
-displays warnings and errors.
-
-Inspector
-~~~~~~~~~
-
-URL: https://github.com/santiagobasulto/debug-inspector-panel
-
-Path: ``inspector_panel.panels.inspector.InspectorPanel``
-
-Retrieves and displays information you specify using the ``debug`` statement.
-Inspector panel also logs to the console by default, but may be instructed not
-to.
-
 LDAP Tracing
 ~~~~~~~~~~~~
 
 URL: https://github.com/danyi1212/django-windowsauth
 
 Path: ``windows_auth.panels.LDAPPanel``
 
@@ -272,26 +251,14 @@
 
 URL: https://github.com/marceltschoppch/django-requests-debug-toolbar
 
 Path: ``requests_panel.panel.RequestsDebugPanel``
 
 Lists HTTP requests made with the popular `requests <https://requests.readthedocs.io/>`_ library.
 
-Sites
-~~~~~
-
-URL: https://github.com/elvard/django-sites-toolbar
-
-Path: ``sites_toolbar.panels.SitesDebugPanel``
-
-Browse Sites registered in ``django.contrib.sites`` and switch between them.
-Useful to debug project when you use `django-dynamicsites
-<https://bitbucket.org/uysrc/django-dynamicsites/src>`_ which sets SITE_ID
-dynamically.
-
 Template Profiler
 ~~~~~~~~~~~~~~~~~
 
 URL: https://github.com/node13h/django-debug-toolbar-template-profiler
 
 Path: ``template_profiler_panel.panels.template.TemplateProfilerPanel``
 
@@ -304,23 +271,14 @@
 
 URL: https://github.com/orf/django-debug-toolbar-template-timings
 
 Path: ``template_timings_panel.panels.TemplateTimings.TemplateTimings``
 
 Displays template rendering times for your Django application.
 
-User
-~~~~
-
-URL: https://github.com/playfire/django-debug-toolbar-user-panel
-
-Path: ``debug_toolbar_user_panel.panels.UserPanel``
-
-Easily switch between logged in users, see properties of current user.
-
 VCS Info
 ~~~~~~~~
 
 URL: https://github.com/giginet/django-debug-toolbar-vcs-info
 
 Path: ``vcs_info_panel.panels.GitInfoPanel``
```

### Comparing `django_debug_toolbar-4.2.0/docs/tips.rst` & `django_debug_toolbar-4.3.0/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/README.rst` & `django_debug_toolbar-4.3.0/example/README.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/django-debug-toolbar.png` & `django_debug_toolbar-4.3.0/example/django-debug-toolbar.png`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/example.db` & `django_debug_toolbar-4.3.0/example/example.db`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/screenshot.py` & `django_debug_toolbar-4.3.0/example/screenshot.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/settings.py` & `django_debug_toolbar-4.3.0/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/urls.py` & `django_debug_toolbar-4.3.0/example/urls.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/templates/index.html` & `django_debug_toolbar-4.3.0/example/templates/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/templates/htmx/boost.html` & `django_debug_toolbar-4.3.0/example/templates/htmx/boost.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/templates/jquery/index.html` & `django_debug_toolbar-4.3.0/example/templates/jquery/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/templates/mootools/index.html` & `django_debug_toolbar-4.3.0/example/templates/mootools/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/templates/prototype/index.html` & `django_debug_toolbar-4.3.0/example/templates/prototype/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/example/templates/turbo/index.html` & `django_debug_toolbar-4.3.0/example/templates/turbo/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/base.py` & `django_debug_toolbar-4.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/models.py` & `django_debug_toolbar-4.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/settings.py` & `django_debug_toolbar-4.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/sync.py` & `django_debug_toolbar-4.3.0/tests/sync.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/test_checks.py` & `django_debug_toolbar-4.3.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/test_decorators.py` & `django_debug_toolbar-4.3.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/test_forms.py` & `django_debug_toolbar-4.3.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/test_integration.py` & `django_debug_toolbar-4.3.0/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import time
 import unittest
 
 import html5lib
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
 from django.core import signing
 from django.core.cache import cache
 from django.db import connection
@@ -745,7 +746,28 @@
         self.selenium.find_element(By.CLASS_NAME, "SQLPanel").click()
 
         table = self.wait.until(
             lambda selenium: sql_panel.find_element(By.TAG_NAME, "table")
         )
         self.assertIn("Query", table.text)
         self.assertIn("Action", table.text)
+
+    def test_ajax_dont_refresh(self):
+        self.get("/ajax/")
+        make_ajax = self.selenium.find_element(By.ID, "click_for_ajax")
+        make_ajax.click()
+        history_panel = self.selenium.find_element(By.ID, "djdt-HistoryPanel")
+        self.assertIn("/ajax/", history_panel.text)
+        self.assertNotIn("/json_view/", history_panel.text)
+
+    @override_settings(DEBUG_TOOLBAR_CONFIG={"UPDATE_ON_FETCH": True})
+    def test_ajax_refresh(self):
+        self.get("/ajax/")
+        make_ajax = self.selenium.find_element(By.ID, "click_for_ajax")
+        make_ajax.click()
+        # Need to wait until the ajax request is over and json_view is displayed on the toolbar
+        time.sleep(2)
+        history_panel = self.wait.until(
+            lambda selenium: self.selenium.find_element(By.ID, "djdt-HistoryPanel")
+        )
+        self.assertNotIn("/ajax/", history_panel.text)
+        self.assertIn("/json_view/", history_panel.text)
```

### Comparing `django_debug_toolbar-4.2.0/tests/test_utils.py` & `django_debug_toolbar-4.3.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,32 @@
 
 class GetNameFromObjTestCase(unittest.TestCase):
     def test_func(self):
         def x():
             return 1
 
         res = get_name_from_obj(x)
-        self.assertEqual(res, "tests.test_utils.x")
+        self.assertEqual(
+            res, "tests.test_utils.GetNameFromObjTestCase.test_func.<locals>.x"
+        )
 
     def test_lambda(self):
         res = get_name_from_obj(lambda: 1)
-        self.assertEqual(res, "tests.test_utils.<lambda>")
+        self.assertEqual(
+            res, "tests.test_utils.GetNameFromObjTestCase.test_lambda.<locals>.<lambda>"
+        )
 
     def test_class(self):
         class A:
             pass
 
         res = get_name_from_obj(A)
-        self.assertEqual(res, "tests.test_utils.A")
+        self.assertEqual(
+            res, "tests.test_utils.GetNameFromObjTestCase.test_class.<locals>.A"
+        )
 
 
 class RenderStacktraceTestCase(unittest.TestCase):
     def test_importlib_path_issue_1612(self):
         trace = [
             ("/server/app.py", 1, "foo", ["code line 1", "code line 2"], {"foo": "bar"})
         ]
```

### Comparing `django_debug_toolbar-4.2.0/tests/urls.py` & `django_debug_toolbar-4.3.0/tests/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,11 +17,12 @@
     path("non_ascii_request/", views.regular_view, {"title": NonAsciiRepr()}),
     path("new_user/", views.new_user),
     path("execute_sql/", views.execute_sql),
     path("cached_view/", views.cached_view),
     path("cached_low_level_view/", views.cached_low_level_view),
     path("json_view/", views.json_view),
     path("redirect/", views.redirect_view),
+    path("ajax/", views.ajax_view),
     path("login_without_redirect/", LoginView.as_view(redirect_field_name=None)),
     path("admin/", admin.site.urls),
     path("__debug__/", include("debug_toolbar.urls")),
 ]
```

### Comparing `django_debug_toolbar-4.2.0/tests/views.py` & `django_debug_toolbar-4.3.0/tests/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,7 +54,11 @@
 def listcomp_view(request):
     lst = [i for i in range(50000) if i % 2 == 0]
     return render(request, "basic.html", {"title": "List comprehension", "lst": lst})
 
 
 def redirect_view(request):
     return HttpResponseRedirect("/regular/redirect/")
+
+
+def ajax_view(request):
+    return render(request, "ajax/ajax.html")
```

### Comparing `django_debug_toolbar-4.2.0/tests/commands/test_debugsqlshell.py` & `django_debug_toolbar-4.3.0/tests/commands/test_debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_cache.py` & `django_debug_toolbar-4.3.0/tests/panels/test_cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_custom.py` & `django_debug_toolbar-4.3.0/tests/panels/test_custom.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_history.py` & `django_debug_toolbar-4.3.0/tests/panels/test_history.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_profiling.py` & `django_debug_toolbar-4.3.0/tests/panels/test_profiling.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import sys
+import unittest
+
 from django.contrib.auth.models import User
 from django.db import IntegrityError, transaction
 from django.http import HttpResponse
 from django.test.utils import override_settings
 
 from ..base import BaseTestCase, IntegrationTestCase
 from ..views import listcomp_view, regular_view
@@ -46,14 +49,18 @@
         self.panel.generate_stats(self.request, response)
         # ensure the panel renders but doesn't include our function.
         content = self.panel.content
         self.assertIn("regular_view", content)
         self.assertNotIn("render", content)
         self.assertValidHTML(content)
 
+    @unittest.skipUnless(
+        sys.version_info < (3, 12, 0),
+        "Python 3.12 no longer contains a frame for list comprehensions.",
+    )
     def test_listcomp_escaped(self):
         self._get_response = lambda request: listcomp_view(request)
         response = self.panel.process_request(self.request)
         self.panel.generate_stats(self.request, response)
         content = self.panel.content
         self.assertNotIn('<span class="djdt-func"><listcomp></span>', content)
         self.assertIn('<span class="djdt-func">&lt;listcomp&gt;</span>', content)
```

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_redirects.py` & `django_debug_toolbar-4.3.0/tests/panels/test_redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_request.py` & `django_debug_toolbar-4.3.0/tests/panels/test_request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_settings.py` & `django_debug_toolbar-4.3.0/tests/panels/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_sql.py` & `django_debug_toolbar-4.3.0/tests/panels/test_sql.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_staticfiles.py` & `django_debug_toolbar-4.3.0/tests/panels/test_staticfiles.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_template.py` & `django_debug_toolbar-4.3.0/tests/panels/test_template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import django
 from django.contrib.auth.models import User
 from django.template import Context, RequestContext, Template
 from django.test import override_settings
+from django.utils.functional import SimpleLazyObject
 
 from ..base import BaseTestCase, IntegrationTestCase
 from ..forms import TemplateReprForm
 from ..models import NonAsciiRepr
 
 
 class TemplatesPanelTestCase(BaseTestCase):
@@ -17,28 +18,30 @@
         self.sql_panel.enable_instrumentation()
 
     def tearDown(self):
         self.sql_panel.disable_instrumentation()
         super().tearDown()
 
     def test_queryset_hook(self):
+        response = self.panel.process_request(self.request)
         t = Template("No context variables here!")
         c = Context(
             {
                 "queryset": User.objects.all(),
                 "deep_queryset": {"queryset": User.objects.all()},
             }
         )
         t.render(c)
+        self.panel.generate_stats(self.request, response)
 
         # ensure the query was NOT logged
         self.assertEqual(len(self.sql_panel._queries), 0)
 
         self.assertEqual(
-            self.panel.templates[0]["context"],
+            self.panel.templates[0]["context_list"],
             [
                 "{'False': False, 'None': None, 'True': True}",
                 "{'deep_queryset': '<<triggers database query>>',\n"
                 " 'queryset': '<<queryset of auth.User>>'}",
             ],
         )
 
@@ -95,24 +98,42 @@
     def test_disabled(self):
         config = {"DISABLE_PANELS": {"debug_toolbar.panels.templates.TemplatesPanel"}}
         self.assertTrue(self.panel.enabled)
         with self.settings(DEBUG_TOOLBAR_CONFIG=config):
             self.assertFalse(self.panel.enabled)
 
     def test_empty_context(self):
+        response = self.panel.process_request(self.request)
         t = Template("")
         c = Context({})
         t.render(c)
+        self.panel.generate_stats(self.request, response)
 
         # Includes the builtin context but not the empty one.
         self.assertEqual(
-            self.panel.templates[0]["context"],
+            self.panel.templates[0]["context_list"],
             ["{'False': False, 'None': None, 'True': True}"],
         )
 
+    def test_lazyobject(self):
+        response = self.panel.process_request(self.request)
+        t = Template("")
+        c = Context({"lazy": SimpleLazyObject(lambda: "lazy_value")})
+        t.render(c)
+        self.panel.generate_stats(self.request, response)
+        self.assertNotIn("lazy_value", self.panel.content)
+
+    def test_lazyobject_eval(self):
+        response = self.panel.process_request(self.request)
+        t = Template("{{lazy}}")
+        c = Context({"lazy": SimpleLazyObject(lambda: "lazy_value")})
+        self.assertEqual(t.render(c), "lazy_value")
+        self.panel.generate_stats(self.request, response)
+        self.assertIn("lazy_value", self.panel.content)
+
 
 @override_settings(
     DEBUG=True, DEBUG_TOOLBAR_PANELS=["debug_toolbar.panels.templates.TemplatesPanel"]
 )
 class JinjaTemplateTestCase(IntegrationTestCase):
     def test_django_jinja2(self):
         r = self.client.get("/regular_jinja/foobar/")
```

### Comparing `django_debug_toolbar-4.2.0/tests/panels/test_versions.py` & `django_debug_toolbar-4.3.0/tests/panels/test_versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/LICENSE` & `django_debug_toolbar-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.2.0/README.rst` & `django_debug_toolbar-4.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
 The current stable version of the Debug Toolbar is 4.1.0. It works on
 Django ≥ 3.2.4.
 
+The Debug Toolbar does not currently support `Django's asynchronous views
+<https://docs.djangoproject.com/en/dev/topics/async/>`_.
+
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
 
 The Django Debug Toolbar is released under the BSD license, like Django
 itself. If you like it, please consider contributing!
 
 The Django Debug Toolbar was originally created by Rob Hudson <rob@cogit8.org>
```

### Comparing `django_debug_toolbar-4.2.0/pyproject.toml` & `django_debug_toolbar-4.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
+  "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "Django>=3.2.4",
@@ -47,69 +48,51 @@
 packages = ["debug_toolbar"]
 
 [tool.hatch.version]
 path = "debug_toolbar/__init__.py"
 
 [tool.ruff]
 extend-select = [
-  # pyflakes, pycodestyle
-  "F", "E", "W",
-  # mmcabe
-  # "C90",
-  # isort
-  "I",
-  # pep8-naming
-  # "N",
-  # pyupgrade
-  "UP",
-  # flake8-2020
-  # "YTT",
-  # flake8-boolean-trap
-  "FBT",
-  # flake8-bugbear
-  "B",
-  # flake8-comprehensions
-  "C4",
-  # flake8-django
-  "DJ",
-  # flake8-pie
-  "PIE",
-  # flake8-simplify
-  "SIM",
-  # flake8-gettext
-  "INT",
-  # pygrep-hooks
-  "PGH",
-  # pylint
-  # "PL",
-  # unused noqa
-  "RUF100",
+  "ASYNC",  # flake8-async
+  "B",      # flake8-bugbear
+  "C4",     # flake8-comprehensions
+  "C90",    # McCabe cyclomatic complexity
+  "DJ",     # flake8-django
+  "E",      # pycodestyle errors
+  "F",      # Pyflakes
+  "FBT",    # flake8-boolean-trap
+  "I",      # isort
+  "INT",    # flake8-gettext
+  "PGH",    # pygrep-hooks
+  "PIE",    # flake8-pie
+  "RUF100", # Unused noqa directive
+  "SIM",    # flake8-simplify
+  "SLOT",   # flake8-slots
+  "UP",     # pyupgrade
+  "W",      # pycodestyle warnings
 ]
 extend-ignore = [
-  # Allow zip() without strict=
-  "B905",
-  # No line length errors
-  "E501",
+  "B905",   # Allow zip() without strict=
+  "E501",   # Ignore line length violations
+  "SIM108", # Use ternary operator instead of if-else-block
 ]
 fix = true
 show-fixes = true
 target-version = "py38"
 
 [tool.ruff.isort]
 combine-as-imports = true
 
 [tool.ruff.mccabe]
-max-complexity = 15
+max-complexity = 16
 
 [tool.ruff.per-file-ignores]
 "*/migrat*/*" = [
-  # Allow using PascalCase model names in migrations
-  "N806",
-  # Ignore the fact that migration files are invalid module names
-  "N999",
+  "N806",  # Allow using PascalCase model names in migrations
+  "N999",  # Ignore the fact that migration files are invalid module names
 ]
 
 [tool.coverage.html]
 skip_covered = true
 skip_empty = true
 
 [tool.coverage.run]
```

### Comparing `django_debug_toolbar-4.2.0/PKG-INFO` & `django_debug_toolbar-4.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: django-debug-toolbar
-Version: 4.2.0
+Version: 4.3.0
 Summary: A configurable set of panels that display various debug information about the current request/response.
 Project-URL: Download, https://pypi.org/project/django-debug-toolbar/
 Project-URL: Homepage, https://github.com/jazzband/django-debug-toolbar
 Author: Rob Hudson
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: django>=3.2.4
 Requires-Dist: sqlparse>=0.2
 Description-Content-Type: text/x-rst
 
 =====================================
@@ -74,14 +75,17 @@
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
 The current stable version of the Debug Toolbar is 4.1.0. It works on
 Django ≥ 3.2.4.
 
+The Debug Toolbar does not currently support `Django's asynchronous views
+<https://docs.djangoproject.com/en/dev/topics/async/>`_.
+
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
 
 The Django Debug Toolbar is released under the BSD license, like Django
 itself. If you like it, please consider contributing!
 
 The Django Debug Toolbar was originally created by Rob Hudson <rob@cogit8.org>
```

