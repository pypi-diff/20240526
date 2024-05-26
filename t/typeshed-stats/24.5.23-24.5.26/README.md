# Comparing `tmp/typeshed_stats-24.5.23.tar.gz` & `tmp/typeshed_stats-24.5.26.tar.gz`

## Comparing `typeshed_stats-24.5.23.tar` & `typeshed_stats-24.5.26.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.editorconfig
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.gitattributes
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.markdownlint.yaml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/mkdocs.yml
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/website_macros.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/renovate.json5
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/workflows/check-requirements.yml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/workflows/regen-examples-and-docs.yml
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/workflows/test-website.yml
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/workflows/test.yml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.github/workflows/typecheck.yml
--rw-r--r--   0        0        0    31441 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/examples/example.csv
--rw-r--r--   0        0        0   170880 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/examples/example.json
--rw-r--r--   0        0        0   286080 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/examples/example.md
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/scripts/regenerate.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/scripts/runtests.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/__init__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/__main__.py
--rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/_cli.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/_markdown_template.md.jinja
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/_version.py
--rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/gather.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/py.typed
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/src/typeshed_stats/serialize.py
--rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/big_logo.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/cli.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/gather.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/index.md
--rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/logo.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/serialize.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/stats-csv.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/stats.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/.snippets/links.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/.snippets/refs.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/javascripts/filtertable.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/stats_website/javascripts/tablesort.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/__init__.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/conftest.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/test___all__.py
--rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/test__cli.py
--rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/test_gather.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/test_running_from_command_line.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/tests/test_serialize.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/LICENSE
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/README.md
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/pyproject.toml
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 typeshed_stats-24.5.23/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.editorconfig
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.gitattributes
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.markdownlint.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/mkdocs.yml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/website_macros.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/renovate.json5
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/check-requirements.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/regen-examples-and-docs.yml
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/test-website.yml
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.github/workflows/typecheck.yml
+-rw-r--r--   0        0        0    31422 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/examples/example.csv
+-rw-r--r--   0        0        0   170862 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/examples/example.json
+-rw-r--r--   0        0        0   286082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/examples/example.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/scripts/regenerate.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/scripts/runtests.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/__main__.py
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/_cli.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/_markdown_template.md.jinja
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/_version.py
+-rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/gather.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/py.typed
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/src/typeshed_stats/serialize.py
+-rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/big_logo.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/cli.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/gather.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/index.md
+-rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/logo.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/serialize.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/stats-csv.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/stats.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/.snippets/links.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/.snippets/refs.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/javascripts/filtertable.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/stats_website/javascripts/tablesort.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/__init__.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/conftest.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test___all__.py
+-rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test__cli.py
+-rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test_gather.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test_running_from_command_line.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/tests/test_serialize.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/LICENSE
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/README.md
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/pyproject.toml
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 typeshed_stats-24.5.26/PKG-INFO
```

### Comparing `typeshed_stats-24.5.23/.pre-commit-config.yaml` & `typeshed_stats-24.5.26/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/mkdocs.yml` & `typeshed_stats-24.5.26/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/website_macros.py` & `typeshed_stats-24.5.26/website_macros.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.github/renovate.json5` & `typeshed_stats-24.5.26/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.github/workflows/check-requirements.yml` & `typeshed_stats-24.5.26/.github/workflows/check-requirements.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.github/workflows/publish.yml` & `typeshed_stats-24.5.26/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 name: Publish Python distributions to PyPI
 
 on:
   push:
   workflow_dispatch:
   schedule:
-    - cron: "0 0 * * *"
+    - cron: "0 0 * * 0"
 
 permissions:
   contents: read
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
```

### Comparing `typeshed_stats-24.5.23/.github/workflows/regen-examples-and-docs.yml` & `typeshed_stats-24.5.26/.github/workflows/regen-examples-and-docs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.github/workflows/test-website.yml` & `typeshed_stats-24.5.26/.github/workflows/test-website.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.github/workflows/test.yml` & `typeshed_stats-24.5.26/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.github/workflows/typecheck.yml` & `typeshed_stats-24.5.26/.github/workflows/typecheck.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/examples/example.csv` & `typeshed_stats-24.5.26/examples/example.csv`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Flask-Cors,types-Flask-Cors,https://github.com/corydolphin/flask-cors,PARTIAL,-,126,UP_TO_DATE,UPLOADED,STRICT,63,0,24,0,0,0,7,2,30,1,0,2,0,0,MISSING_STUBS_IGNORED,linux,0
 Flask-Migrate,types-Flask-Migrate,https://github.com/miguelgrinberg/Flask-Migrate,COMPLETE,-,130,UP_TO_DATE,UPLOADED,STRICT,86,0,24,0,0,0,0,0,7,0,0,3,0,0,ERROR_ON_MISSING_STUB,linux,1
 Flask-SocketIO,types-Flask-SocketIO,https://github.com/miguelgrinberg/flask-socketio,COMPLETE,-,233,UP_TO_DATE,UPLOADED,NOT_STRICT,138,36,37,15,17,1,2,0,3,1,0,8,0,0,ERROR_ON_MISSING_STUB,linux,3
 JACK-Client,types-JACK-Client,https://github.com/spatialaudio/jackclient-python,COMPLETE,-,311,UP_TO_DATE,UPLOADED,STRICT,107,0,152,0,0,0,0,2,46,0,0,15,0,0,ERROR_ON_MISSING_STUB,linux,0
 Markdown,types-Markdown,https://github.com/Python-Markdown/markdown,PARTIAL,-,695,UP_TO_DATE,UPLOADED,NOT_STRICT,256,30,198,2,0,0,15,3,217,15,0,102,0,0,MISSING_STUBS_IGNORED,linux,0
 Pillow,types-Pillow,https://github.com/python-pillow/Pillow,COMPLETE,-,3266,OBSOLETE,UPLOADED,NOT_STRICT,777,584,588,319,55,2,7,5,766,5,305,226,3,1,ERROR_ON_MISSING_STUB,linux;win32,18
 PyAutoGUI,types-PyAutoGUI,https://github.com/asweigart/pyautogui,COMPLETE,-,234,UP_TO_DATE,UPLOADED,STRICT,145,0,38,0,0,0,0,0,22,0,0,5,0,0,ERROR_ON_MISSING_STUB,linux,1
-PyMySQL,types-PyMySQL,https://github.com/PyMySQL/PyMySQL,PARTIAL,-,1045,UP_TO_DATE,UPLOADED,NOT_STRICT,142,52,101,37,28,0,10,18,734,60,0,24,0,0,MISSING_STUBS_IGNORED,linux,11
+PyMySQL,types-PyMySQL,https://github.com/PyMySQL/PyMySQL,PARTIAL,-,1051,UP_TO_DATE,UPLOADED,NOT_STRICT,143,52,101,37,28,0,10,18,736,60,0,24,0,0,MISSING_STUBS_IGNORED,linux,11
 PyScreeze,types-PyScreeze,https://github.com/asweigart/pyscreeze,COMPLETE,-,193,UP_TO_DATE,UPLOADED,STRICT,102,0,21,0,0,0,0,0,17,0,0,5,0,0,ERROR_ON_MISSING_STUB,linux;win32,2
 PyYAML,types-PyYAML,https://github.com/yaml/pyyaml,COMPLETE,-,1298,UP_TO_DATE,UPLOADED,NOT_STRICT,516,282,222,172,12,0,44,12,220,160,2,91,0,0,ERROR_ON_MISSING_STUB,linux,3
 Pygments,types-Pygments,https://github.com/pygments/pygments,PARTIAL,-,845,UP_TO_DATE,UPLOADED,NOT_STRICT,116,156,108,75,17,5,7,2,376,169,24,94,0,1,MISSING_STUBS_IGNORED,linux,4
 RPi.GPIO,types-RPi.GPIO,https://sourceforge.net/p/raspberry-gpio-python/code/,COMPLETE,-,56,UP_TO_DATE,UPLOADED,STRICT,28,0,18,0,0,0,0,0,26,0,0,2,0,0,SKIPPED,None,0
 Send2Trash,types-Send2Trash,https://github.com/arsenetar/send2trash,COMPLETE,-,15,UP_TO_DATE,UPLOADED,STRICT,4,0,4,0,0,0,3,0,0,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,2
 WTForms,types-WTForms,https://github.com/wtforms/wtforms,COMPLETE,-,1069,UP_TO_DATE,UPLOADED,STRICT,531,0,185,0,0,0,71,15,139,28,0,100,0,0,ERROR_ON_MISSING_STUB,linux,21
 WebOb,types-WebOb,https://github.com/Pylons/webob,COMPLETE,-,1796,UP_TO_DATE,UPLOADED,STRICT,808,0,606,0,0,0,91,13,246,15,0,149,0,0,ERROR_ON_MISSING_STUB,linux,100
@@ -35,15 +35,15 @@
 colorama,types-colorama,https://github.com/tartley/colorama,COMPLETE,-,201,UP_TO_DATE,UPLOADED,STRICT,89,0,60,0,0,0,3,1,85,0,0,11,0,0,ERROR_ON_MISSING_STUB,linux;win32,44
 commonmark,types-commonmark,https://github.com/rtfd/commonmark.py,PARTIAL,-,370,UP_TO_DATE,UPLOADED,NOT_STRICT,63,158,84,76,55,0,0,0,133,86,0,18,0,0,MISSING_STUBS_IGNORED,linux,0
 console-menu,types-console-menu,https://github.com/aegirhall/console-menu,COMPLETE,-,711,UP_TO_DATE,UPLOADED,STRICT,217,0,278,0,0,0,7,1,58,3,1,39,0,0,ERROR_ON_MISSING_STUB,linux,0
 croniter,types-croniter,https://github.com/kiorky/croniter,COMPLETE,-,151,UP_TO_DATE,UPLOADED,STRICT,69,0,24,0,0,0,0,8,29,0,0,8,1,0,ERROR_ON_MISSING_STUB,linux,0
 dateparser,types-dateparser,https://github.com/scrapinghub/dateparser,COMPLETE,-,473,UP_TO_DATE,UPLOADED,NOT_STRICT,126,130,74,69,21,0,4,6,135,76,0,34,0,0,ERROR_ON_MISSING_STUB,linux,6
 decorator,types-decorator,https://github.com/micheles/decorator,COMPLETE,-,66,UP_TO_DATE,UPLOADED,STRICT,36,0,13,0,0,0,19,6,15,3,0,2,0,0,ERROR_ON_MISSING_STUB,linux,10
 defusedxml,types-defusedxml,https://github.com/tiran/defusedxml,PARTIAL,-,234,UP_TO_DATE,UPLOADED,NOT_STRICT,81,97,38,13,13,0,0,1,37,0,19,12,0,0,MISSING_STUBS_IGNORED,linux,0
-docker,types-docker,https://github.com/docker/docker-py,COMPLETE,-,1886,UP_TO_DATE,UPLOADED,NOT_STRICT,775,379,290,270,315,7,19,25,206,2,83,127,2,24,ERROR_ON_MISSING_STUB,linux,7
+docker,types-docker,https://github.com/docker/docker-py,COMPLETE,-,1899,OUT_OF_DATE,UPLOADED,NOT_STRICT,782,376,292,270,315,7,19,25,206,2,83,128,2,24,ERROR_ON_MISSING_STUB,linux,7
 dockerfile-parse,types-dockerfile-parse,https://github.com/containerbuildsystem/dockerfile-parse,COMPLETE,-,113,UP_TO_DATE,UPLOADED,STRICT,46,0,24,0,0,0,0,0,39,0,0,8,0,0,ERROR_ON_MISSING_STUB,linux,0
 docopt,types-docopt,https://github.com/docopt/docopt,COMPLETE,-,14,UP_TO_DATE,UPLOADED,STRICT,7,0,3,0,1,0,0,1,2,0,0,2,0,0,ERROR_ON_MISSING_STUB,linux,0
 docutils,types-docutils,https://sourceforge.net/p/docutils/code,PARTIAL,-,1493,UP_TO_DATE,UPLOADED,NOT_STRICT,762,51,448,7,51,33,39,19,250,20,1,222,1,0,MISSING_STUBS_IGNORED,linux,18
 editdistance,types-editdistance,https://github.com/roy-ht/editdistance,COMPLETE,-,5,UP_TO_DATE,UPLOADED,STRICT,10,0,4,0,0,0,0,0,0,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,1
 entrypoints,types-entrypoints,https://github.com/takluyver/entrypoints,COMPLETE,-,41,UP_TO_DATE,UPLOADED,STRICT,23,0,12,0,0,0,0,1,12,0,0,5,0,0,ERROR_ON_MISSING_STUB,linux,1
 fanstatic,types-fanstatic,https://github.com/zopefoundation/fanstatic,COMPLETE,-,530,UP_TO_DATE,UPLOADED,STRICT,167,0,133,0,0,0,8,3,128,0,0,49,0,0,ERROR_ON_MISSING_STUB,linux,40
 first,types-first,https://github.com/hynek/first,COMPLETE,-,14,UP_TO_DATE,UPLOADED,STRICT,8,0,4,0,0,0,2,0,2,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,0
@@ -92,15 +92,15 @@
 peewee,types-peewee,https://github.com/coleifer/peewee,PARTIAL,-,1693,OUT_OF_DATE,UPLOADED,NOT_STRICT,425,669,346,438,216,5,0,0,420,0,348,168,0,0,ERROR_ON_MISSING_STUB,linux,11
 pep8-naming,types-pep8-naming,https://github.com/PyCQA/pep8-naming,PARTIAL,-,26,UP_TO_DATE,UPLOADED,STRICT,10,0,8,0,0,2,1,1,10,3,0,1,0,0,MISSING_STUBS_IGNORED,linux,2
 pexpect,types-pexpect,https://github.com/pexpect/pexpect,COMPLETE,-,673,UP_TO_DATE,UPLOADED,NOT_STRICT,234,120,181,33,8,0,0,0,160,0,24,22,0,0,ERROR_ON_MISSING_STUB,linux,1
 pika,types-pika-ts,https://github.com/pika/pika,COMPLETE,"The `types-pika` package contains alternate, more complete type stubs, that are maintained outside of typeshed.",2235,UP_TO_DATE,UPLOADED,NOT_STRICT,618,383,413,347,141,24,4,0,464,0,258,222,0,0,ERROR_ON_MISSING_STUB,linux,9
 playsound,types-playsound,https://github.com/TaylorSMarks/playsound,COMPLETE,-,5,UP_TO_DATE,UPLOADED,STRICT,2,0,1,0,0,0,0,0,1,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,0
 polib,types-polib,https://github.com/izimobil/polib,COMPLETE,-,143,UP_TO_DATE,UPLOADED,STRICT,61,0,75,0,0,0,18,0,45,0,0,8,0,0,ERROR_ON_MISSING_STUB,linux,0
 portpicker,types-portpicker,https://github.com/google/python_portpicker,COMPLETE,-,16,UP_TO_DATE,UPLOADED,STRICT,10,0,6,0,0,0,0,0,0,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,0
-protobuf,types-protobuf,https://github.com/protocolbuffers/protobuf,PARTIAL,Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1),4825,UP_TO_DATE,UPLOADED,NOT_STRICT,785,254,530,75,14,0,17,4,921,123,1,185,0,0,MISSING_STUBS_IGNORED,linux,11
+protobuf,types-protobuf,https://github.com/protocolbuffers/protobuf,PARTIAL,Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1),4825,OUT_OF_DATE,UPLOADED,NOT_STRICT,785,254,530,75,14,0,17,4,921,123,1,185,0,0,MISSING_STUBS_IGNORED,linux,11
 psutil,types-psutil,https://github.com/giampaolo/psutil,COMPLETE,-,1565,UP_TO_DATE,UPLOADED,NOT_STRICT,125,310,194,355,28,0,0,47,592,198,99,89,3,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,14
 psycopg2,types-psycopg2,https://github.com/psycopg/psycopg2,COMPLETE,-,1731,UP_TO_DATE,UPLOADED,NOT_STRICT,337,152,314,75,29,5,14,21,517,60,3,331,2,0,ERROR_ON_MISSING_STUB,linux,2
 pyOpenSSL,types-pyOpenSSL,https://github.com/pyca/pyopenssl,PARTIAL,-,363,UP_TO_DATE,UPLOADED,STRICT,148,0,179,0,1,1,2,2,125,1,0,22,0,0,MISSING_STUBS_IGNORED,linux,1
 pyRFC3339,types-pyRFC3339,https://github.com/kurtraschke/pyRFC3339,COMPLETE,-,17,UP_TO_DATE,UPLOADED,STRICT,15,0,9,0,0,0,1,0,0,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,0
 pyasn1,types-pyasn1,https://github.com/pyasn1/pyasn1,COMPLETE,-,1502,UP_TO_DATE,UPLOADED,NOT_STRICT,209,533,118,425,39,9,0,0,251,0,1,178,0,0,ERROR_ON_MISSING_STUB,linux,8
 pyaudio,types-pyaudio,-,COMPLETE,-,165,UP_TO_DATE,UPLOADED,STRICT,51,0,37,0,0,0,0,0,72,0,0,3,0,0,ERROR_ON_MISSING_STUB,darwin;linux,0
 pycocotools,types-pycocotools,https://github.com/ppwwyyxx/cocoapi,COMPLETE,-,183,UP_TO_DATE,UPLOADED,STRICT,51,0,35,0,0,0,0,1,70,0,1,12,0,0,ERROR_ON_MISSING_STUB,linux,0
@@ -110,41 +110,41 @@
 pygit2,types-pygit2,https://github.com/libgit2/pygit2,COMPLETE,-,1928,UP_TO_DATE,UPLOADED,STRICT,674,0,503,0,0,0,3,0,474,0,1,119,0,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,11
 pyinstaller,types-pyinstaller,https://github.com/pyinstaller/pyinstaller,COMPLETE,-,703,OUT_OF_DATE,UPLOADED,STRICT,274,0,149,0,6,0,1,2,195,0,15,26,0,0,ERROR_ON_MISSING_STUB,linux,49
 pyjks,types-pyjks,https://github.com/kurtbrose/pyjks,COMPLETE,-,377,UP_TO_DATE,UPLOADED,STRICT,132,0,59,0,0,0,0,0,73,0,0,31,0,0,ERROR_ON_MISSING_STUB,linux,38
 pynput,types-pynput,https://github.com/moses-palmer/pynput,COMPLETE,-,324,OUT_OF_DATE,UPLOADED,STRICT,81,0,71,0,0,0,11,0,58,1,0,24,2,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,12
 pyserial,types-pyserial,https://github.com/pyserial/pyserial,COMPLETE,-,1079,UP_TO_DATE,UPLOADED,STRICT,223,0,270,0,0,0,2,4,466,7,65,66,0,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,64
 pysftp,types-pysftp,https://bitbucket.org/dundeemt/pysftp,COMPLETE,-,166,UP_TO_DATE,UPLOADED,STRICT,109,0,70,0,0,0,0,0,6,0,0,6,0,0,ERROR_ON_MISSING_STUB,linux,0
 pytest-lazy-fixture,types-pytest-lazy-fixture,https://github.com/tvorog/pytest-lazy-fixture,COMPLETE,-,12,UP_TO_DATE,UPLOADED,STRICT,5,0,5,0,0,0,0,1,1,0,0,1,0,0,ERROR_ON_MISSING_STUB,linux,8
-python-crontab,types-python-crontab,https://gitlab.com/doctormo/python-crontab,COMPLETE,-,328,OUT_OF_DATE,UPLOADED,NOT_STRICT,174,2,146,4,1,0,17,0,72,1,1,18,0,1,ERROR_ON_MISSING_STUB,linux,2
+python-crontab,types-python-crontab,https://gitlab.com/doctormo/python-crontab,COMPLETE,-,329,UP_TO_DATE,UPLOADED,NOT_STRICT,176,2,147,4,1,0,17,0,72,1,1,18,0,1,ERROR_ON_MISSING_STUB,linux,2
 python-datemath,types-python-datemath,https://github.com/nickmaccarthy/python-datemath,PARTIAL,-,16,UP_TO_DATE,UPLOADED,STRICT,16,0,4,0,0,1,0,0,0,0,0,1,0,0,MISSING_STUBS_IGNORED,linux,0
 python-dateutil,types-python-dateutil,https://github.com/dateutil/dateutil,PARTIAL,-,439,UP_TO_DATE,UPLOADED,NOT_STRICT,172,65,112,42,5,0,0,0,89,0,4,29,0,0,MISSING_STUBS_IGNORED,linux,11
 python-gflags,types-python-gflags,https://github.com/google/python-gflags,COMPLETE,-,251,UP_TO_DATE,UPLOADED,STRICT,186,0,98,0,0,0,39,9,19,2,0,27,0,0,ERROR_ON_MISSING_STUB,linux,1
 python-jose,types-python-jose,https://github.com/mpdavis/python-jose,COMPLETE,-,357,UP_TO_DATE,UPLOADED,NOT_STRICT,86,39,64,26,4,0,14,12,117,30,0,26,0,0,ERROR_ON_MISSING_STUB,linux,6
 python-nmap,types-python-nmap,https://bitbucket.org/xael/python-nmap,COMPLETE,-,119,UP_TO_DATE,UPLOADED,STRICT,44,0,44,0,0,0,0,0,31,0,0,14,1,0,ERROR_ON_MISSING_STUB,linux,1
 python-slugify,types-python-slugify,https://github.com/un33k/python-slugify,COMPLETE,-,45,OBSOLETE,UPLOADED,STRICT,19,0,3,0,0,0,0,0,12,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,1
 python-xlib,types-python-xlib,https://github.com/python-xlib/python-xlib,COMPLETE,-,5421,UP_TO_DATE,UPLOADED,STRICT,1334,0,583,0,0,0,15,8,3519,5,0,425,0,0,ERROR_ON_MISSING_STUB,linux,10
 pytz,types-pytz,https://github.com/stub42/pytz,COMPLETE,-,133,UP_TO_DATE,UPLOADED,STRICT,69,0,51,0,2,0,2,0,29,0,0,16,0,0,ERROR_ON_MISSING_STUB,linux,4
 pywin32,types-pywin32,https://github.com/mhammond/pywin32,COMPLETE,-,34801,UP_TO_DATE,UPLOADED,NOT_STRICT,3800,3558,3865,1987,419,288,1,1,25095,0,2824,724,0,0,ERROR_ON_MISSING_STUB,win32,46
 pyxdg,types-pyxdg,https://github.com/takluyver/pyxdg,COMPLETE,-,860,UP_TO_DATE,UPLOADED,NOT_STRICT,511,1,297,0,2,0,0,0,165,0,1,31,0,0,ERROR_ON_MISSING_STUB,linux,2
 qrbill,types-qrbill,https://github.com/claudep/swiss-qr-bill,COMPLETE,-,172,UP_TO_DATE,UPLOADED,STRICT,96,0,31,0,0,0,0,4,33,0,0,4,0,0,ERROR_ON_MISSING_STUB,linux,2
 qrcode,types-qrcode,https://github.com/lincolnloop/python-qrcode,COMPLETE,-,524,UP_TO_DATE,UPLOADED,NOT_STRICT,109,174,109,60,14,2,2,1,166,0,91,40,0,0,ERROR_ON_MISSING_STUB,linux,8
 redis,types-redis,https://github.com/redis/redis-py,PARTIAL,"Note: Redis-py 5.0.0 added a py.typed file, but the inline annotations are incomplete. Continuing to use `types-redis` for the time being may lead to superior results.",6165,OUT_OF_DATE,UPLOADED,NOT_STRICT,3945,1223,1379,607,352,5,92,330,618,158,34,215,0,2,MISSING_STUBS_IGNORED,linux,67
 regex,types-regex,https://github.com/mrabarnett/mrab-regex,COMPLETE,-,750,UP_TO_DATE,UPLOADED,STRICT,431,0,114,0,0,0,25,16,4,0,0,7,0,0,ERROR_ON_MISSING_STUB,linux,13
-requests,types-requests,https://github.com/psf/requests,COMPLETE,"Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.",1001,UP_TO_DATE,UPLOADED,NOT_STRICT,373,134,129,69,19,0,9,5,116,39,0,51,0,0,ERROR_ON_MISSING_STUB,linux,4
+reportlab,types-reportlab,-,COMPLETE,-,7731,UP_TO_DATE,UPLOADED,NOT_STRICT,1790,2469,1470,1057,344,3,25,11,2699,6,1269,567,0,2,ERROR_ON_MISSING_STUB,linux,65
+requests,types-requests,https://github.com/psf/requests,COMPLETE,"Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.",1015,UP_TO_DATE,UPLOADED,NOT_STRICT,379,132,133,66,19,1,8,4,116,34,5,51,0,0,ERROR_ON_MISSING_STUB,linux,4
 requests-oauthlib,types-requests-oauthlib,https://github.com/requests/requests-oauthlib,COMPLETE,-,268,UP_TO_DATE,UPLOADED,NOT_STRICT,115,20,45,4,50,3,1,0,25,1,7,13,0,0,ERROR_ON_MISSING_STUB,linux,0
 retry,types-retry,https://github.com/invl/retry,COMPLETE,-,28,UP_TO_DATE,UPLOADED,STRICT,17,0,2,0,0,0,2,0,1,0,0,0,0,0,ERROR_ON_MISSING_STUB,linux,3
 s2clientprotocol,types-s2clientprotocol,https://github.com/Blizzard/s2client-proto,COMPLETE,Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 3.6.1 on [s2client-proto 5.0.12.91115.0](https://github.com/Blizzard/s2client-proto/tree/c04df4adbe274858a4eb8417175ee32ad02fd609),5029,UP_TO_DATE,UPLOADED,STRICT,856,0,676,0,0,0,0,0,1864,0,0,239,0,0,ERROR_ON_MISSING_STUB,linux,1
 seaborn,types-seaborn,https://github.com/mwaskom/seaborn,COMPLETE,-,2587,UP_TO_DATE,UPLOADED,NOT_STRICT,1445,25,357,2,34,7,155,17,282,13,24,100,1,0,ERROR_ON_MISSING_STUB,linux,5
-setuptools,types-setuptools,https://github.com/pypa/setuptools,COMPLETE,-,3133,OUT_OF_DATE,UPLOADED,STRICT_ON_SOME_FILES,1001,434,843,263,46,13,21,1,658,87,285,187,0,0,ERROR_ON_MISSING_STUB,linux;win32,111
+setuptools,types-setuptools,https://github.com/pypa/setuptools,COMPLETE,-,3140,UP_TO_DATE,UPLOADED,STRICT_ON_SOME_FILES,1001,434,845,262,45,13,21,1,660,87,285,187,0,0,ERROR_ON_MISSING_STUB,linux;win32,109
 simplejson,types-simplejson,https://github.com/simplejson/simplejson,COMPLETE,-,277,UP_TO_DATE,UPLOADED,STRICT,180,0,24,0,0,0,46,6,49,7,0,6,0,0,ERROR_ON_MISSING_STUB,linux,11
 singledispatch,types-singledispatch,https://github.com/jaraco/singledispatch,COMPLETE,-,27,UP_TO_DATE,UPLOADED,STRICT,16,0,12,0,0,0,7,0,3,1,0,2,0,0,ERROR_ON_MISSING_STUB,linux,0
 six,types-six,https://github.com/benjaminp/six,COMPLETE,-,335,UP_TO_DATE,UPLOADED,STRICT,69,0,38,0,0,0,8,6,13,0,0,3,0,0,ERROR_ON_MISSING_STUB,linux,25
 slumber,types-slumber,https://github.com/samgiles/slumber,COMPLETE,-,74,UP_TO_DATE,UPLOADED,STRICT,43,0,25,0,0,0,11,5,9,0,0,15,0,0,ERROR_ON_MISSING_STUB,linux,2
-stdlib,-,https://github.com/python/cpython,STDLIB,-,55793,STDLIB,NOT_CURRENTLY_UPLOADED,STRICT_ON_SOME_FILES,26002,823,14374,368,74,11,1939,831,8255,535,152,2410,26,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,1620
-stripe,types-stripe,https://github.com/stripe/stripe-python,PARTIAL,-,1532,OBSOLETE,UPLOADED,NOT_STRICT,270,396,108,172,156,0,5,4,157,42,0,136,1,0,MISSING_STUBS_IGNORED,linux,8
+stdlib,-,https://github.com/python/cpython,STDLIB,-,56071,STDLIB,NOT_CURRENTLY_UPLOADED,STRICT_ON_SOME_FILES,26172,823,14406,368,74,11,1959,837,8258,535,152,2412,26,0,ERROR_ON_MISSING_STUB,darwin;linux;win32,1423
 tabulate,types-tabulate,https://github.com/astanin/python-tabulate,COMPLETE,-,60,UP_TO_DATE,UPLOADED,STRICT,15,0,3,0,0,0,2,0,26,0,0,4,0,0,ERROR_ON_MISSING_STUB,linux,0
 tensorflow,types-tensorflow,https://github.com/tensorflow/tensorflow,PARTIAL,Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .,25535,UP_TO_DATE,UPLOADED,NOT_STRICT,5324,8,3033,4,23,58,60,34,5294,5,7,928,1,0,MISSING_STUBS_IGNORED,linux,51
 toml,types-toml,https://github.com/uiri/toml,COMPLETE,-,136,UP_TO_DATE,UPLOADED,STRICT,71,0,41,0,0,0,21,5,14,2,0,14,2,0,ERROR_ON_MISSING_STUB,linux,4
 toposort,types-toposort,https://gitlab.com/ericvsmith/toposort,COMPLETE,-,13,UP_TO_DATE,UPLOADED,STRICT,4,0,4,0,0,0,1,0,1,1,0,2,0,0,ERROR_ON_MISSING_STUB,linux,0
 tqdm,types-tqdm,https://github.com/tqdm/tqdm,COMPLETE,-,1379,UP_TO_DATE,UPLOADED,NOT_STRICT,811,146,164,27,38,8,1,1,100,0,74,36,0,0,ERROR_ON_MISSING_STUB,linux,2
 translationstring,types-translationstring,https://github.com/Pylons/translationstring,COMPLETE,-,73,UP_TO_DATE,UPLOADED,STRICT,62,0,18,0,0,0,6,1,4,1,0,7,0,0,ERROR_ON_MISSING_STUB,linux,4
 tree-sitter,types-tree-sitter,https://github.com/tree-sitter/py-tree-sitter,COMPLETE,-,123,OBSOLETE,UPLOADED,STRICT,25,0,52,0,0,0,0,2,4,0,0,7,0,0,ERROR_ON_MISSING_STUB,linux,36
```

### Comparing `typeshed_stats-24.5.23/examples/example.json` & `typeshed_stats-24.5.26/examples/example.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9847664961301323%*

 * *Differences: {'115': "{'number_of_lines': 329, 'package_status': 'UP_TO_DATE', 'annotation_stats': "*

 * *        "{'annotated_parameters': 176, 'annotated_returns': 147}}",*

 * * '131': "{'number_of_lines': 1015, 'annotation_stats': {'annotated_parameters': 379, "*

 * *        "'unannotated_parameters': 132, 'annotated_returns': 133, 'unannotated_returns': 66, "*

 * *        "'explicit_Incomplete_returns': 1, 'explicit_Any_parameters': 8, 'explicit_Any_returns': "*

 * *        "4, 'explicit_Any_variables': 34, 'explicit_Incomplete_variables':  […]*

```diff
@@ -304,32 +304,32 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/asweigart/pyautogui"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 142,
+            "annotated_parameters": 143,
             "annotated_returns": 101,
-            "annotated_variables": 734,
+            "annotated_variables": 736,
             "classdefs": 24,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 10,
             "explicit_Any_returns": 18,
             "explicit_Any_variables": 60,
             "explicit_Incomplete_parameters": 28,
             "explicit_Incomplete_returns": 0,
             "explicit_Incomplete_variables": 0,
             "unannotated_parameters": 52,
             "unannotated_returns": 37
         },
         "completeness_level": "PARTIAL",
         "extra_description": null,
-        "number_of_lines": 1045,
+        "number_of_lines": 1051,
         "package_name": "PyMySQL",
         "package_status": "UP_TO_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-PyMySQL",
         "stubtest_settings": {
             "allowlist_length": 11,
             "platforms": [
@@ -1361,34 +1361,34 @@
             "strictness": "MISSING_STUBS_IGNORED"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/tiran/defusedxml"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 775,
-            "annotated_returns": 290,
+            "annotated_parameters": 782,
+            "annotated_returns": 292,
             "annotated_variables": 206,
-            "classdefs": 127,
+            "classdefs": 128,
             "classdefs_with_Any": 2,
             "classdefs_with_Incomplete": 24,
             "explicit_Any_parameters": 19,
             "explicit_Any_returns": 25,
             "explicit_Any_variables": 2,
             "explicit_Incomplete_parameters": 315,
             "explicit_Incomplete_returns": 7,
             "explicit_Incomplete_variables": 83,
-            "unannotated_parameters": 379,
+            "unannotated_parameters": 376,
             "unannotated_returns": 270
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
-        "number_of_lines": 1886,
+        "number_of_lines": 1899,
         "package_name": "docker",
-        "package_status": "UP_TO_DATE",
+        "package_status": "OUT_OF_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-docker",
         "stubtest_settings": {
             "allowlist_length": 7,
             "platforms": [
                 "linux"
             ],
@@ -3321,15 +3321,15 @@
             "unannotated_parameters": 254,
             "unannotated_returns": 75
         },
         "completeness_level": "PARTIAL",
         "extra_description": "Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)",
         "number_of_lines": 4825,
         "package_name": "protobuf",
-        "package_status": "UP_TO_DATE",
+        "package_status": "OUT_OF_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-protobuf",
         "stubtest_settings": {
             "allowlist_length": 11,
             "platforms": [
                 "linux"
             ],
@@ -3925,16 +3925,16 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/tvorog/pytest-lazy-fixture"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 174,
-            "annotated_returns": 146,
+            "annotated_parameters": 176,
+            "annotated_returns": 147,
             "annotated_variables": 72,
             "classdefs": 18,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 1,
             "explicit_Any_parameters": 17,
             "explicit_Any_returns": 0,
             "explicit_Any_variables": 1,
@@ -3942,17 +3942,17 @@
             "explicit_Incomplete_returns": 0,
             "explicit_Incomplete_variables": 1,
             "unannotated_parameters": 2,
             "unannotated_returns": 4
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
-        "number_of_lines": 328,
+        "number_of_lines": 329,
         "package_name": "python-crontab",
-        "package_status": "OUT_OF_DATE",
+        "package_status": "UP_TO_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-python-crontab",
         "stubtest_settings": {
             "allowlist_length": 2,
             "platforms": [
                 "linux"
             ],
@@ -4435,32 +4435,66 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/mrabarnett/mrab-regex"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 373,
-            "annotated_returns": 129,
+            "annotated_parameters": 1790,
+            "annotated_returns": 1470,
+            "annotated_variables": 2699,
+            "classdefs": 567,
+            "classdefs_with_Any": 0,
+            "classdefs_with_Incomplete": 2,
+            "explicit_Any_parameters": 25,
+            "explicit_Any_returns": 11,
+            "explicit_Any_variables": 6,
+            "explicit_Incomplete_parameters": 344,
+            "explicit_Incomplete_returns": 3,
+            "explicit_Incomplete_variables": 1269,
+            "unannotated_parameters": 2469,
+            "unannotated_returns": 1057
+        },
+        "completeness_level": "COMPLETE",
+        "extra_description": null,
+        "number_of_lines": 7731,
+        "package_name": "reportlab",
+        "package_status": "UP_TO_DATE",
+        "pyright_setting": "NOT_STRICT",
+        "stub_distribution_name": "types-reportlab",
+        "stubtest_settings": {
+            "allowlist_length": 65,
+            "platforms": [
+                "linux"
+            ],
+            "strictness": "ERROR_ON_MISSING_STUB"
+        },
+        "upload_status": "UPLOADED",
+        "upstream_url": null
+    },
+    {
+        "annotation_stats": {
+            "annotated_parameters": 379,
+            "annotated_returns": 133,
             "annotated_variables": 116,
             "classdefs": 51,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
-            "explicit_Any_parameters": 9,
-            "explicit_Any_returns": 5,
-            "explicit_Any_variables": 39,
+            "explicit_Any_parameters": 8,
+            "explicit_Any_returns": 4,
+            "explicit_Any_variables": 34,
             "explicit_Incomplete_parameters": 19,
-            "explicit_Incomplete_returns": 0,
-            "explicit_Incomplete_variables": 0,
-            "unannotated_parameters": 134,
-            "unannotated_returns": 69
+            "explicit_Incomplete_returns": 1,
+            "explicit_Incomplete_variables": 5,
+            "unannotated_parameters": 132,
+            "unannotated_returns": 66
         },
         "completeness_level": "COMPLETE",
         "extra_description": "Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.",
-        "number_of_lines": 1001,
+        "number_of_lines": 1015,
         "package_name": "requests",
         "package_status": "UP_TO_DATE",
         "pyright_setting": "NOT_STRICT",
         "stub_distribution_name": "types-requests",
         "stubtest_settings": {
             "allowlist_length": 4,
             "platforms": [
@@ -4606,37 +4640,37 @@
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/mwaskom/seaborn"
     },
     {
         "annotation_stats": {
             "annotated_parameters": 1001,
-            "annotated_returns": 843,
-            "annotated_variables": 658,
+            "annotated_returns": 845,
+            "annotated_variables": 660,
             "classdefs": 187,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 21,
             "explicit_Any_returns": 1,
             "explicit_Any_variables": 87,
-            "explicit_Incomplete_parameters": 46,
+            "explicit_Incomplete_parameters": 45,
             "explicit_Incomplete_returns": 13,
             "explicit_Incomplete_variables": 285,
             "unannotated_parameters": 434,
-            "unannotated_returns": 263
+            "unannotated_returns": 262
         },
         "completeness_level": "COMPLETE",
         "extra_description": null,
-        "number_of_lines": 3133,
+        "number_of_lines": 3140,
         "package_name": "setuptools",
-        "package_status": "OUT_OF_DATE",
+        "package_status": "UP_TO_DATE",
         "pyright_setting": "STRICT_ON_SOME_FILES",
         "stub_distribution_name": "types-setuptools",
         "stubtest_settings": {
-            "allowlist_length": 111,
+            "allowlist_length": 109,
             "platforms": [
                 "linux",
                 "win32"
             ],
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
@@ -4776,84 +4810,50 @@
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "UPLOADED",
         "upstream_url": "https://github.com/samgiles/slumber"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 26002,
-            "annotated_returns": 14374,
-            "annotated_variables": 8255,
-            "classdefs": 2410,
+            "annotated_parameters": 26172,
+            "annotated_returns": 14406,
+            "annotated_variables": 8258,
+            "classdefs": 2412,
             "classdefs_with_Any": 26,
             "classdefs_with_Incomplete": 0,
-            "explicit_Any_parameters": 1939,
-            "explicit_Any_returns": 831,
+            "explicit_Any_parameters": 1959,
+            "explicit_Any_returns": 837,
             "explicit_Any_variables": 535,
             "explicit_Incomplete_parameters": 74,
             "explicit_Incomplete_returns": 11,
             "explicit_Incomplete_variables": 152,
             "unannotated_parameters": 823,
             "unannotated_returns": 368
         },
         "completeness_level": "STDLIB",
         "extra_description": null,
-        "number_of_lines": 55793,
+        "number_of_lines": 56071,
         "package_name": "stdlib",
         "package_status": "STDLIB",
         "pyright_setting": "STRICT_ON_SOME_FILES",
         "stub_distribution_name": "-",
         "stubtest_settings": {
-            "allowlist_length": 1620,
+            "allowlist_length": 1423,
             "platforms": [
                 "darwin",
                 "linux",
                 "win32"
             ],
             "strictness": "ERROR_ON_MISSING_STUB"
         },
         "upload_status": "NOT_CURRENTLY_UPLOADED",
         "upstream_url": "https://github.com/python/cpython"
     },
     {
         "annotation_stats": {
-            "annotated_parameters": 270,
-            "annotated_returns": 108,
-            "annotated_variables": 157,
-            "classdefs": 136,
-            "classdefs_with_Any": 1,
-            "classdefs_with_Incomplete": 0,
-            "explicit_Any_parameters": 5,
-            "explicit_Any_returns": 4,
-            "explicit_Any_variables": 42,
-            "explicit_Incomplete_parameters": 156,
-            "explicit_Incomplete_returns": 0,
-            "explicit_Incomplete_variables": 0,
-            "unannotated_parameters": 396,
-            "unannotated_returns": 172
-        },
-        "completeness_level": "PARTIAL",
-        "extra_description": null,
-        "number_of_lines": 1532,
-        "package_name": "stripe",
-        "package_status": "OBSOLETE",
-        "pyright_setting": "NOT_STRICT",
-        "stub_distribution_name": "types-stripe",
-        "stubtest_settings": {
-            "allowlist_length": 8,
-            "platforms": [
-                "linux"
-            ],
-            "strictness": "MISSING_STUBS_IGNORED"
-        },
-        "upload_status": "UPLOADED",
-        "upstream_url": "https://github.com/stripe/stripe-python"
-    },
-    {
-        "annotation_stats": {
             "annotated_parameters": 15,
             "annotated_returns": 3,
             "annotated_variables": 26,
             "classdefs": 4,
             "classdefs_with_Any": 0,
             "classdefs_with_Incomplete": 0,
             "explicit_Any_parameters": 2,
```

### Comparing `typeshed_stats-24.5.23/examples/example.md` & `typeshed_stats-24.5.26/examples/example.md`

 * *Files 1% similar despite different names*

```diff
@@ -519,15 +519,15 @@
 
 ### Stub distribution name
 
 `types-PyMySQL`
 
 ### Number of lines
 
-1,045 (excluding blank lines)
+1,051 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -544,25 +544,25 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `PyMySQL`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 142
+    - Annotated parameters: 143
     - Unannotated parameters: 52
     - Explicit `Any` parameters: 10
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 28
 - Returns:
     - Annotated returns: 101
     - Unannotated returns: 37
     - Explicit `Any` returns: 18
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 734
+    - Annotated variables: 736
     - Explicit `Any` variables: 60
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 24
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
@@ -2284,19 +2284,19 @@
 
 ### Stub distribution name
 
 `types-docker`
 
 ### Number of lines
 
-1,886 (excluding blank lines)
+1,899 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *out of date*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
@@ -2309,29 +2309,29 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `docker`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 775
-    - Unannotated parameters: 379
+    - Annotated parameters: 782
+    - Unannotated parameters: 376
     - Explicit `Any` parameters: 19
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 315
 - Returns:
-    - Annotated returns: 290
+    - Annotated returns: 292
     - Unannotated returns: 270
     - Explicit `Any` returns: 25
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
 - Variables:
     - Annotated variables: 206
     - Explicit `Any` variables: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 83
 - Class definitions:
-    - Total class definitions: 127
+    - Total class definitions: 128
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 24
 
 ---
 
 ## Info on typeshed's stubs for `dockerfile-parse`
 
@@ -5547,17 +5547,17 @@
 
 `types-protobuf`
 
 ### Number of lines
 
 4,825 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *out of date*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
@@ -6567,19 +6567,19 @@
 
 ### Stub distribution name
 
 `types-python-crontab`
 
 ### Number of lines
 
-328 (excluding blank lines)
+329 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
@@ -6592,20 +6592,20 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `python-crontab`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 174
+    - Annotated parameters: 176
     - Unannotated parameters: 2
     - Explicit `Any` parameters: 17
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
 - Returns:
-    - Annotated returns: 146
+    - Annotated returns: 147
     - Unannotated returns: 4
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 72
     - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
@@ -7414,14 +7414,67 @@
 - Class definitions:
     - Total class definitions: 7
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `reportlab`
+
+### Stub distribution name
+
+`types-reportlab`
+
+### Number of lines
+
+7,731 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 65 unique allowlist entries for `reportlab` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `reportlab`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 1,790
+    - Unannotated parameters: 2,469
+    - Explicit `Any` parameters: 25
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 344
+- Returns:
+    - Annotated returns: 1,470
+    - Unannotated returns: 1,057
+    - Explicit `Any` returns: 11
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 3
+- Variables:
+    - Annotated variables: 2,699
+    - Explicit `Any` variables: 6
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1,269
+- Class definitions:
+    - Total class definitions: 567
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 2
+
+---
+
 ## Info on typeshed's stubs for `requests`
 
 ### Extra description
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 ### Upstream repo URL
@@ -7430,15 +7483,15 @@
 
 ### Stub distribution name
 
 `types-requests`
 
 ### Number of lines
 
-1,001 (excluding blank lines)
+1,015 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7455,27 +7508,27 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `requests`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 373
-    - Unannotated parameters: 134
-    - Explicit `Any` parameters: 9
+    - Annotated parameters: 379
+    - Unannotated parameters: 132
+    - Explicit `Any` parameters: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 19
 - Returns:
-    - Annotated returns: 129
-    - Unannotated returns: 69
-    - Explicit `Any` returns: 5
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Annotated returns: 133
+    - Unannotated returns: 66
+    - Explicit `Any` returns: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
 - Variables:
     - Annotated variables: 116
-    - Explicit `Any` variables: 39
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Explicit `Any` variables: 34
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 5
 - Class definitions:
     - Total class definitions: 51
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
@@ -7719,50 +7772,50 @@
 
 ### Stub distribution name
 
 `types-setuptools`
 
 ### Number of lines
 
-3,133 (excluding blank lines)
+3,140 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 111 unique allowlist entries for `setuptools` when running stubtest in CI.
+Typeshed currently has 109 unique allowlist entries for `setuptools` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict on some files*
 
 Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for `setuptools`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
     - Annotated parameters: 1,001
     - Unannotated parameters: 434
     - Explicit `Any` parameters: 21
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 46
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 45
 - Returns:
-    - Annotated returns: 843
-    - Unannotated returns: 263
+    - Annotated returns: 845
+    - Unannotated returns: 262
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 13
 - Variables:
-    - Annotated variables: 658
+    - Annotated variables: 660
     - Explicit `Any` variables: 87
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 285
 - Class definitions:
     - Total class definitions: 187
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
@@ -8000,15 +8053,15 @@
 
 ### Upstream repo URL
 
 [https://github.com/python/cpython](https://github.com/python/cpython)
 
 ### Number of lines
 
-55,793 (excluding blank lines)
+56,071 (excluding blank lines)
 
 ### Package status: *stdlib*
 
 These are typeshed's stubs for the standard library. Typeshed's stdlib stubs are generally fairly up to date, and are tested against all currently supported Python versions in typeshed's CI.
 
 ### Upload status: *not currently uploaded*
 
@@ -8016,100 +8069,43 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
-Typeshed currently has 1,620 unique allowlist entries for the stdlib when running stubtest in CI.
+Typeshed currently has 1,423 unique allowlist entries for the stdlib when running stubtest in CI.
 
 ### Pyright settings in CI: *strict on some files*
 
 Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for the stdlib
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 26,002
+    - Annotated parameters: 26,172
     - Unannotated parameters: 823
-    - Explicit `Any` parameters: 1,939
+    - Explicit `Any` parameters: 1,959
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 74
 - Returns:
-    - Annotated returns: 14,374
+    - Annotated returns: 14,406
     - Unannotated returns: 368
-    - Explicit `Any` returns: 831
+    - Explicit `Any` returns: 837
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 11
 - Variables:
-    - Annotated variables: 8,255
+    - Annotated variables: 8,258
     - Explicit `Any` variables: 535
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 152
 - Class definitions:
-    - Total class definitions: 2,410
+    - Total class definitions: 2,412
     - Class definitions with `Any`: 26
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `stripe`
-
-### Upstream repo URL
-
-[https://github.com/stripe/stripe-python](https://github.com/stripe/stripe-python)
-
-### Stub distribution name
-
-`types-stripe`
-
-### Number of lines
-
-1,532 (excluding blank lines)
-
-### Package status: *obsolete*
-
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *missing stubs ignored*
-
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
-
-In CI, stubtest is run on `linux` only.
-
-Typeshed currently has 8 unique allowlist entries for `stripe` when running stubtest in CI.
-
-### Pyright settings in CI: *not strict*
-
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
-
-### Statistics on the annotations in typeshed's stubs for `stripe`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 270
-    - Unannotated parameters: 396
-    - Explicit `Any` parameters: 5
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 156
-- Returns:
-    - Annotated returns: 108
-    - Unannotated returns: 172
-    - Explicit `Any` returns: 4
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 157
-    - Explicit `Any` variables: 42
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 136
-    - Class definitions with `Any`: 1
-    - Class definitions marked as at least partially `Incomplete`: 0
-
----
-
 ## Info on typeshed's stubs for `tabulate`
 
 ### Upstream repo URL
 
 [https://github.com/astanin/python-tabulate](https://github.com/astanin/python-tabulate)
 
 ### Stub distribution name
```

### Comparing `typeshed_stats-24.5.23/scripts/regenerate.py` & `typeshed_stats-24.5.26/scripts/regenerate.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/scripts/runtests.py` & `typeshed_stats-24.5.26/scripts/runtests.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/src/typeshed_stats/_cli.py` & `typeshed_stats-24.5.26/src/typeshed_stats/_cli.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/src/typeshed_stats/_markdown_template.md.jinja` & `typeshed_stats-24.5.26/src/typeshed_stats/_markdown_template.md.jinja`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/src/typeshed_stats/gather.py` & `typeshed_stats-24.5.26/src/typeshed_stats/gather.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/src/typeshed_stats/serialize.py` & `typeshed_stats-24.5.26/src/typeshed_stats/serialize.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/stats_website/big_logo.png` & `typeshed_stats-24.5.26/stats_website/big_logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/stats_website/gather.md` & `typeshed_stats-24.5.26/stats_website/gather.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/stats_website/logo.png` & `typeshed_stats-24.5.26/stats_website/logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/stats_website/stats-csv.md` & `typeshed_stats-24.5.26/stats_website/stats-csv.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/stats_website/.snippets/links.md` & `typeshed_stats-24.5.26/stats_website/.snippets/links.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/stats_website/javascripts/filtertable.js` & `typeshed_stats-24.5.26/stats_website/javascripts/filtertable.js`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/tests/conftest.py` & `typeshed_stats-24.5.26/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/tests/test___all__.py` & `typeshed_stats-24.5.26/tests/test___all__.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/tests/test__cli.py` & `typeshed_stats-24.5.26/tests/test__cli.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/tests/test_gather.py` & `typeshed_stats-24.5.26/tests/test_gather.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/tests/test_running_from_command_line.py` & `typeshed_stats-24.5.26/tests/test_running_from_command_line.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/tests/test_serialize.py` & `typeshed_stats-24.5.26/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/.gitignore` & `typeshed_stats-24.5.26/.gitignore`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/LICENSE` & `typeshed_stats-24.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/README.md` & `typeshed_stats-24.5.26/README.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/pyproject.toml` & `typeshed_stats-24.5.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-24.5.23/PKG-INFO` & `typeshed_stats-24.5.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typeshed_stats
-Version: 24.5.23
+Version: 24.5.26
 Summary: Library and command-line tool to gather stats on typeshed packages
 Project-URL: Homepage, https://github.com/AlexWaygood/typeshed-stats
 Project-URL: Bug Tracker, https://github.com/AlexWaygood/typeshed-stats/issues
 Author-email: Alex Waygood <alex.waygood@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: stubs,typeshed,typing
```

