# Comparing `tmp/coverage-7.5.0.tar.gz` & `tmp/coverage-7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.5.0.tar", last modified: Tue Apr 23 17:16:04 2024, max compression
+gzip compressed data, was "coverage-7.5.1.tar", last modified: Sat May  4 14:44:36 2024, max compression
```

## Comparing `coverage-7.5.0.tar` & `coverage-7.5.1.tar`

### file list

```diff
@@ -1,465 +1,462 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-23 17:15:53.000000 coverage-7.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-23 17:15:53.000000 coverage-7.5.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.927390 coverage-7.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.927390 coverage-7.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/ISSUE_TEMPLATE/support.md
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.927390 coverage-7.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-23 17:15:53.000000 coverage-7.5.0/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 17:15:53.000000 coverage-7.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    57461 2024-04-23 17:15:53.000000 coverage-7.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-23 17:15:53.000000 coverage-7.5.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-23 17:15:53.000000 coverage-7.5.0/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-23 17:15:53.000000 coverage-7.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-23 17:15:53.000000 coverage-7.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-23 17:15:53.000000 coverage-7.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 17:15:53.000000 coverage-7.5.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-23 17:16:03.999390 coverage-7.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-23 17:15:53.000000 coverage-7.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-23 17:15:53.000000 coverage-7.5.0/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.931390 coverage-7.5.0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/comment_on_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/download_gha_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/ghrel_template.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/parse_relnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 17:15:53.000000 coverage-7.5.0/ci/trigger_build_kits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.939390 coverage-7.5.0/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    21955 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    51686 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.943390 coverage-7.5.0/coverage/ctracer/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/datastack.c
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/datastack.h
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/filedisp.c
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/filedisp.h
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/module.c
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/stats.h
--rw-r--r--   0 runner    (1001) docker     (127)    34412 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/tracer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/tracer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/ctracer/util.h
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/disposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/execfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    28591 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.943390 coverage-7.5.0/coverage/htmlfiles/
--rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/pyfile.html
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    18457 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/htmlfiles/style.scss
--rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/inorout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/jsonreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/lcovreport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/numbits.py
--rw-r--r--   0 runner    (1001) docker     (127)    54693 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/phystokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/plugin_support.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/pytracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/report_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/sqldata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/sqlitedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/sysmon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/templite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/tomlconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/tracer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-23 17:15:53.000000 coverage-7.5.0/coverage/xmlreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 17:16:03.000000 coverage-7.5.0/coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.947390 coverage-7.5.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.947390 coverage-7.5.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/_static/coverage.css
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/api_coverage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/api_coveragedata.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/api_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/api_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/branch.rst
--rw-r--r--   0 runner    (1001) docker     (127)   112606 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    44589 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/cog_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/dbschema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/dict.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/excluding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/howitworks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.951390 coverage-7.5.0/doc/media/
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
--rw-r--r--   0 runner    (1001) docker     (127)   165210 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/media/sleepy-snake-600.png
--rw-r--r--   0 runner    (1001) docker     (127)    24168 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/media/sleepy-snake-circle-150.png
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/migrating.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/other.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/python-coverage.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.951390 coverage-7.5.0/doc/sample_html/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/sample_html/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/sample_html/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/sample_html/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/sleepy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/source.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/subprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/trouble.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-23 17:15:53.000000 coverage-7.5.0/doc/whatsnew5x.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-23 17:15:53.000000 coverage-7.5.0/howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16609 2024-04-23 17:15:53.000000 coverage-7.5.0/igor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.955390 coverage-7.5.0/lab/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.955390 coverage-7.5.0/lab/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)    23241 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/benchmark/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/benchmark/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/bpo_prelude.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/branch_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/branches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/compare_times.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/coverage-03.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/coverage-04.dtd
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/find_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/genpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/goals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/hack_pyc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/new-data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.955390 coverage-7.5.0/lab/notes/
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/notes/bug1303.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/notes/pypy-738-decorated-functions.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/parse_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/pick.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/platform_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/run_sysmon.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/run_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/select_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/show_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/show_pyc.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 17:15:53.000000 coverage-7.5.0/lab/treetopy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-23 17:15:53.000000 coverage-7.5.0/metacov.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-23 17:15:53.000000 coverage-7.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.959390 coverage-7.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/light-threads.in
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/light-threads.pip
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pytest.in
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/pytest.pip
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 17:15:53.000000 coverage-7.5.0/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:16:03.999390 coverage-7.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-23 17:15:53.000000 coverage-7.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/balance_xdist_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/coveragetest.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/covmodzip1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/gold/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.915390 coverage-7.5.0/tests/gold/annotate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/gold/annotate/anno_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/anno_dir/multi.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/anno_dir/z_80084bf2fba02475___init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/anno_dir/z_80084bf2fba02475_a.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2___init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2_b.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/gold/annotate/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/encodings/utf8.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/gold/annotate/mae/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/mae/mae.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/gold/annotate/multi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.971390 coverage-7.5.0/tests/gold/annotate/multi/a/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/multi/a/__init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/multi/a/a.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/annotate/multi/b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/multi/b/__init__.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/multi/b/b.py,cover
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/multi/multi.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/annotate/white/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/annotate/white/white.py,cover
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/html/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/html/a/
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/a/a_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/a/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/a/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/a/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/html/b_branch/
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/b_branch/b_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/b_branch/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/b_branch/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/b_branch/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/html/bom/
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/bom/bom_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/bom/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/bom/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/bom/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.975390 coverage-7.5.0/tests/gold/html/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/contexts/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/contexts/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/contexts/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/contexts/two_tests_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.979390 coverage-7.5.0/tests/gold/html/isolatin1/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/isolatin1/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/isolatin1/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/isolatin1/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/isolatin1/isolatin1_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.979390 coverage-7.5.0/tests/gold/html/omit_1/
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/m2_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_1/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.979390 coverage-7.5.0/tests/gold/html/omit_2/
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_2/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_2/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_2/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_2/m2_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_2/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_2/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.983390 coverage-7.5.0/tests/gold/html/omit_3/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_3/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_3/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_3/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_3/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_3/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.983390 coverage-7.5.0/tests/gold/html/omit_4/
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_4/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_4/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_4/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_4/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_4/m3_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_4/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.983390 coverage-7.5.0/tests/gold/html/omit_5/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_5/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_5/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_5/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_5/m1_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/omit_5/main_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.983390 coverage-7.5.0/tests/gold/html/other/
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/other/blah_blah_other_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/other/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/other/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/other/here_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/other/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.987390 coverage-7.5.0/tests/gold/html/partial/
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial/partial_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.987390 coverage-7.5.0/tests/gold/html/partial_626/
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial_626/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial_626/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial_626/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/partial_626/partial_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.987390 coverage-7.5.0/tests/gold/html/styled/
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/styled/a_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/styled/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/styled/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/styled/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/styled/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/styled/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.987390 coverage-7.5.0/tests/gold/html/support/
--rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/support/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/support/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/support/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/support/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/support/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/gold/html/unicode/
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/unicode/class_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/unicode/function_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/unicode/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/html/unicode/unicode_py.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.919390 coverage-7.5.0/tests/gold/testing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/gold/testing/getty/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/testing/getty/gettysburg.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/gold/testing/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/testing/xml/output.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.919390 coverage-7.5.0/tests/gold/xml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/gold/xml/x_xml/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/xml/x_xml/coverage.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/gold/xml/y_xml_branch/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/gold/xml/y_xml_branch/coverage.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/goldtest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/js/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/modules/aa/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/afile.odd.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/afile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/modules/aa/bb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/bb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/bb/bfile.odd.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/bb/bfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/aa/bb/cc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/bb/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/bb/cc/cfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.991390 coverage-7.5.0/tests/modules/aa/bb.odd/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/bb.odd/bfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/aa/zfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/ambiguous/pkg1/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/ambiguous/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/ambiguous/pkg1/ambiguous.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/covmod1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.919390 coverage-7.5.0/tests/modules/namespace_420/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/namespace_420/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/namespace_420/sub1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/pkg1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/p1a.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/p1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/p1c.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/runmod2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/pkg1/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/sub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/sub/ps1a.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg1/sub/runmod3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.995390 coverage-7.5.0/tests/modules/pkg2/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg2/p2a.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/pkg2/p2b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/modules/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/plugins/a_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/plugins/another.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/modules/process_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/process_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/process_test/try_execfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/runmod1.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/modules/usepkgs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.923390 coverage-7.5.0/tests/moremodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.919390 coverage-7.5.0/tests/moremodules/namespace_420/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/moremodules/namespace_420/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/namespace_420/sub2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/moremodules/othermods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/othermods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/othermods/othera.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/othermods/otherb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/moremodules/othermods/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/othermods/sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/othermods/sub/osa.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/moremodules/othermods/sub/osb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/osinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/plugin1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/plugin2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/plugin_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/qunit/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/qunit/jquery.tmpl.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/select_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/stress_phystoken.tok
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/stress_phystoken_dos.tok
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    55256 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_arcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44715 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)    31725 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16582 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10991 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_execfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_filereporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_goldtest.py
--rw-r--r--   0 runner    (1001) docker     (127)    49985 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_lcov.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_numbits.py
--rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_oddball.py
--rw-r--r--   0 runner    (1001) docker     (127)    31902 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_phystokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    44097 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    50581 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43130 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_report_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_report_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_sqlitedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_templite.py
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13664 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/test_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/testenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.923390 coverage-7.5.0/tests/zipsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:16:03.999390 coverage-7.5.0/tests/zipsrc/zip1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/zipsrc/zip1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-23 17:15:53.000000 coverage-7.5.0/tests/zipsrc/zip1/zip1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-23 17:15:53.000000 coverage-7.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-04 14:44:25.000000 coverage-7.5.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-04 14:44:25.000000 coverage-7.5.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.516669 coverage-7.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.516669 coverage-7.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/ISSUE_TEMPLATE/support.md
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.516669 coverage-7.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-04 14:44:25.000000 coverage-7.5.1/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-04 14:44:25.000000 coverage-7.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    59054 2024-05-04 14:44:25.000000 coverage-7.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-04 14:44:25.000000 coverage-7.5.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-04 14:44:25.000000 coverage-7.5.1/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-04 14:44:25.000000 coverage-7.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-04 14:44:25.000000 coverage-7.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-04 14:44:25.000000 coverage-7.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-04 14:44:25.000000 coverage-7.5.1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-04 14:44:36.584669 coverage-7.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-04 14:44:25.000000 coverage-7.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-04 14:44:25.000000 coverage-7.5.1/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.520669 coverage-7.5.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/comment_on_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/download_gha_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/ghrel_template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/parse_relnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-04 14:44:25.000000 coverage-7.5.1/ci/trigger_build_kits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.528669 coverage-7.5.1/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34250 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21955 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51686 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.532669 coverage-7.5.1/coverage/ctracer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/datastack.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/datastack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/filedisp.c
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/filedisp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/stats.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34412 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/tracer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/tracer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/ctracer/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/disposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/execfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.532669 coverage-7.5.1/coverage/htmlfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    24699 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/pyfile.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18457 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/htmlfiles/style.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/inorout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/jsonreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/lcovreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/numbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54717 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/phystokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/plugin_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/pytracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/report_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/sqldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/sqlitedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/sysmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/templite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/tomlconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/tracer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-04 14:44:25.000000 coverage-7.5.1/coverage/xmlreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 14:44:36.000000 coverage-7.5.1/coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/_static/coverage.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_coveragedata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/api_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/branch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   112606 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    44589 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/cog_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/dbschema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/excluding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/howitworks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165210 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/sleepy-snake-600.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24168 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/media/sleepy-snake-circle-150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/migrating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/other.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/python-coverage.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.540669 coverage-7.5.1/doc/sample_html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/sample_html/favicon_32_cb_58284776.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/sample_html/keybd_closed_cb_ce680311.png
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/sleepy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/source.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/subprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/trouble.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-04 14:44:25.000000 coverage-7.5.1/doc/whatsnew5x.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-04 14:44:25.000000 coverage-7.5.1/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16609 2024-05-04 14:44:25.000000 coverage-7.5.1/igor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.544669 coverage-7.5.1/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.544669 coverage-7.5.1/lab/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)    23241 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/benchmark/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/benchmark/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/bpo_prelude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/branch_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2066 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/compare_times.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/coverage-03.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/coverage-04.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/find_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/genpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/goals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/hack_pyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/new-data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.544669 coverage-7.5.1/lab/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/notes/bug1303.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/notes/pypy-738-decorated-functions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/parse_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/pick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/platform_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/run_sysmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/run_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/select_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/show_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/show_pyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/lab/treetopy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-04 14:44:25.000000 coverage-7.5.1/metacov.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-04 14:44:25.000000 coverage-7.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.548669 coverage-7.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/light-threads.in
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/light-threads.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pytest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/pytest.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-04 14:44:25.000000 coverage-7.5.1/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:44:36.584669 coverage-7.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-04 14:44:25.000000 coverage-7.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/balance_xdist_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/coveragetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/covmodzip1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.504670 coverage-7.5.1/tests/gold/annotate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/anno_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/multi.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_80084bf2fba02475___init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_80084bf2fba02475_a.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2___init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/anno_dir/z_b039179a8a4ce2c2_b.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/encodings/utf8.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/mae/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/mae/mae.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/multi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/multi/a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/a/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/a/a.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/multi/b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/b/__init__.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/b/b.py,cover
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/multi/multi.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/annotate/white/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/annotate/white/white.py,cover
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.560669 coverage-7.5.1/tests/gold/html/a/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/a_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/a/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/b_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/b_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/b_branch/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/bom/
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/bom_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/bom/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/contexts/two_tests_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/isolatin1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/isolatin1/isolatin1_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.564669 coverage-7.5.1/tests/gold/html/omit_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/m2_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_1/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/m2_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_2/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_3/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/m3_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_4/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.568669 coverage-7.5.1/tests/gold/html/omit_5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/m1_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/omit_5/main_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/other/
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/blah_blah_other_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/here_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/other/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/partial/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial/partial_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/partial_626/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/partial_626/partial_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/styled/
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/a_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/myextra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/styled/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.572669 coverage-7.5.1/tests/gold/html/support/
+-rw-r--r--   0 runner    (1001) docker     (127)    24699 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/support/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/html/unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/class_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/function_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/html/unicode/unicode_py.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/gold/testing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/testing/getty/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/testing/getty/gettysburg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/testing/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/testing/xml/output.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/gold/xml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/xml/x_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/xml/x_xml/coverage.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/gold/xml/y_xml_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/gold/xml/y_xml_branch/coverage.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/goldtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/js/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/afile.odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/afile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/bb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/bfile.odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/bfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/bb/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb/cc/cfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/aa/bb.odd/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/bb.odd/bfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/aa/zfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.576669 coverage-7.5.1/tests/modules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/ambiguous/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/ambiguous/pkg1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/ambiguous/pkg1/ambiguous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/covmod1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/modules/namespace_420/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/namespace_420/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/namespace_420/sub1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/p1a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/p1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/p1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/runmod2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/pkg1/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/ps1a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg1/sub/runmod3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/pkg2/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg2/p2a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/pkg2/p2b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/plugins/a_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/plugins/another.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/modules/process_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/process_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/process_test/try_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/runmod1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/modules/usepkgs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/moremodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.508669 coverage-7.5.1/tests/moremodules/namespace_420/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.580669 coverage-7.5.1/tests/moremodules/namespace_420/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/namespace_420/sub2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/moremodules/othermods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/othera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/otherb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/moremodules/othermods/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/sub/osa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/moremodules/othermods/sub/osb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/osinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/plugin1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/plugin2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/plugin_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/qunit/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/qunit/jquery.tmpl.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/select_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/stress_phystoken.tok
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/stress_phystoken_dos.tok
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55256 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63291 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_arcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44715 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31725 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38001 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16582 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10991 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_filereporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_goldtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_lcov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_numbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_oddball.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32720 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_phystokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44141 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50581 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43130 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_report_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_report_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_sqlitedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_templite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13664 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22006 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/test_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/testenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.512669 coverage-7.5.1/tests/zipsrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:36.584669 coverage-7.5.1/tests/zipsrc/zip1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/zipsrc/zip1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 14:44:25.000000 coverage-7.5.1/tests/zipsrc/zip1/zip1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-04 14:44:25.000000 coverage-7.5.1/tox.ini
```

### Comparing `coverage-7.5.0/.editorconfig` & `coverage-7.5.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.git-blame-ignore-revs` & `coverage-7.5.1/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `coverage-7.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/ISSUE_TEMPLATE/config.yml` & `coverage-7.5.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `coverage-7.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/ISSUE_TEMPLATE/support.md` & `coverage-7.5.1/.github/ISSUE_TEMPLATE/support.md`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/workflows/codeql-analysis.yml` & `coverage-7.5.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/workflows/coverage.yml` & `coverage-7.5.1/.github/workflows/coverage.yml`

 * *Files 4% similar despite different names*

```diff
@@ -65,23 +65,21 @@
           # Windows pypy 3.9 and 3.10 get stuck with PyPy 7.3.15.  I hope to
           # unstick them, but I don't want that to block all other progress, so
           # skip them for now.
           - os: windows
             python-version: "pypy-3.9"
           - os: windows
             python-version: "pypy-3.10"
-        # GitHub is rolling out macos 14, but it doesn't have Python 3.8 or 3.9.
-        # https://mastodon.social/@hugovk/112320493602782374
-        include:
-          - python-version: "3.8"
-            os: "macos"
-            os-version: "13"
-          - python-version: "3.9"
-            os: "macos"
-            os-version: "13"
+        # If we need to tweak the os version we can do it with an include like
+        # this:
+        #  include:
+        #    - python-version: "3.8"
+        #      os: "macos"
+        #      os-version: "13"
+
       # If one job fails, stop the whole thing.
       fail-fast: true
 
     steps:
       - name: "Check out the repo"
         uses: "actions/checkout@v4"
```

### Comparing `coverage-7.5.0/.github/workflows/dependency-review.yml` & `coverage-7.5.1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/workflows/kit.yml` & `coverage-7.5.1/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/workflows/python-nightly.yml` & `coverage-7.5.1/.github/workflows/python-nightly.yml`

 * *Files 8% similar despite different names*

```diff
@@ -27,41 +27,49 @@
 
 concurrency:
   group: "${{ github.workflow }}-${{ github.ref }}"
   cancel-in-progress: true
 
 jobs:
   tests:
-    name: "${{ matrix.python-version }}"
-    # Choose a recent Ubuntu that deadsnakes still builds all the versions for.
-    # For example, deadsnakes doesn't provide 3.10 nightly for 22.04 (jammy)
-    # because jammy ships 3.10, and deadsnakes doesn't want to clobber it.
-    # https://launchpad.net/~deadsnakes/+archive/ubuntu/nightly/+packages
-    # https://github.com/deadsnakes/issues/issues/234
-    # See https://github.com/deadsnakes/nightly for the source of the nightly
-    # builds.
-    # bionic: 18, focal: 20, jammy: 22, noble: 24
-    runs-on: ubuntu-22.04
+    name: "${{ matrix.python-version }} on ${{ matrix.os-short }}"
+    runs-on: "${{ matrix.os }}"
     # If it doesn't finish in an hour, it's not going to. Don't spin for six
     # hours needlessly.
     timeout-minutes: 60
 
     strategy:
       matrix:
+        os:
+          # Choose a recent Ubuntu that deadsnakes still builds all the versions for.
+          # For example, deadsnakes doesn't provide 3.10 nightly for 22.04 (jammy)
+          # because jammy ships 3.10, and deadsnakes doesn't want to clobber it.
+          # https://launchpad.net/~deadsnakes/+archive/ubuntu/nightly/+packages
+          # https://github.com/deadsnakes/issues/issues/234
+          # See https://github.com/deadsnakes/nightly for the source of the nightly
+          # builds.
+          # bionic: 18, focal: 20, jammy: 22, noble: 24
+          - "ubuntu-22.04"
+        os-short:
+          - "ubuntu"
         python-version:
           # When changing this list, be sure to check the [gh] list in
           # tox.ini so that tox will run properly. PYVERSIONS
           # Available versions:
           # https://launchpad.net/~deadsnakes/+archive/ubuntu/nightly/+packages
           - "3.12-dev"
           - "3.13-dev"
           # https://github.com/actions/setup-python#available-versions-of-pypy
           - "pypy-3.8-nightly"
           - "pypy-3.9-nightly"
           - "pypy-3.10-nightly"
+        include:
+            - python-version: "pypy-3.10-nightly"
+              os: "windows-latest"
+              os-short: "windows"
       fail-fast: false
 
     steps:
       - name: "Check out the repo"
         uses: "actions/checkout@v4"
 
       - name: "Install ${{ matrix.python-version }} with deadsnakes"
```

### Comparing `coverage-7.5.0/.github/workflows/quality.yml` & `coverage-7.5.1/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/.github/workflows/testsuite.yml` & `coverage-7.5.1/.github/workflows/testsuite.yml`

 * *Files 7% similar despite different names*

```diff
@@ -53,28 +53,26 @@
           - "3.13"
           - "pypy-3.8"
           - "pypy-3.9"
           - "pypy-3.10"
         exclude:
           # Windows pypy 3.9 and 3.10 get stuck with PyPy 7.3.15.  I hope to
           # unstick them, but I don't want that to block all other progress, so
-          # skip them for now.
+          # skip them for now. These excludes can be removed once GitHub uses
+          # PyPy 7.3.16 on Windows.  https://github.com/pypy/pypy/issues/4876
           - os: windows
             python-version: "pypy-3.9"
           - os: windows
             python-version: "pypy-3.10"
-        # GitHub is rolling out macos 14, but it doesn't have Python 3.8 or 3.9.
-        # https://mastodon.social/@hugovk/112320493602782374
-        include:
-          - python-version: "3.8"
-            os: "macos"
-            os-version: "13"
-          - python-version: "3.9"
-            os: "macos"
-            os-version: "13"
+        # If we need to tweak the os version we can do it with an include like
+        # this:
+        #  include:
+        #    - python-version: "3.8"
+        #      os: "macos"
+        #      os-version: "13"
 
       fail-fast: false
 
     steps:
       - name: "Check out the repo"
         uses: "actions/checkout@v4"
```

### Comparing `coverage-7.5.0/.readthedocs.yaml` & `coverage-7.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/CHANGES.rst` & `coverage-7.5.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,60 @@
     ..  .. _changes_9-8-1:
     ..
     ..  Version 9.8.1 — 2027-07-27
     ..  --------------------------
 
 .. scriv-start-here
 
+.. _changes_7-5-1:
+
+Version 7.5.1 — 2024-05-04
+--------------------------
+
+- Fix: a pragma comment on the continuation lines of a multi-line statement
+  now excludes the statement and its body, the same as if the pragma is
+  on the first line. This closes `issue 754`_. The fix was contributed by
+  `Daniel Diniz <pull 1773_>`_.
+
+- Fix: very complex source files like `this one <resolvent_lookup_>`_ could
+  cause a maximum recursion error when creating an HTML report.  This is now
+  fixed, closing `issue 1774`_.
+
+- HTML report improvements:
+
+  - Support files (JavaScript and CSS) referenced by the HTML report now have
+    hashes added to their names to ensure updated files are used instead of
+    stale cached copies.
+
+  - Missing branch coverage explanations that said "the condition was never
+    false" now read "the condition was always true" because it's easier to
+    understand.
+
+  - Column sort order is remembered better as you move between the index pages,
+    fixing `issue 1766`_.  Thanks, `Daniel Diniz <pull 1768_>`_.
+
+
+.. _resolvent_lookup: https://github.com/sympy/sympy/blob/130950f3e6b3f97fcc17f4599ac08f70fdd2e9d4/sympy/polys/numberfields/resolvent_lookup.py
+.. _issue 754: https://github.com/nedbat/coveragepy/issues/754
+.. _issue 1766: https://github.com/nedbat/coveragepy/issues/1766
+.. _pull 1768: https://github.com/nedbat/coveragepy/pull/1768
+.. _pull 1773: https://github.com/nedbat/coveragepy/pull/1773
+.. _issue 1774: https://github.com/nedbat/coveragepy/issues/1774
+
+
 .. _changes_7-5-0:
 
 Version 7.5.0 — 2024-04-23
 --------------------------
 
 - Added initial support for function and class reporting in the HTML report.
   There are now three index pages which link to each other: files, functions,
   and classes.  Other reports don't yet have this information, but it will be
   added in the future where it makes sense.  Feedback gladly accepted!
+  Finishes `issue 780`_.
 
 - Other HTML report improvements:
 
   - There is now a "hide covered" checkbox to filter out 100% files, finishing
     `issue 1384`_.
 
   - The index page is always sorted by one of its columns, with clearer
@@ -46,14 +83,15 @@
 - The debug output showing which configuration files were tried now shows
   absolute paths to help diagnose problems where settings aren't taking effect,
   and is renamed from "attempted_config_files" to the more logical
   "config_files_attempted."
 
 - Python 3.13.0a6 is supported.
 
+.. _issue 780: https://github.com/nedbat/coveragepy/issues/780
 .. _issue 1384: https://github.com/nedbat/coveragepy/issues/1384
 .. _issue 1765: https://github.com/nedbat/coveragepy/issues/1765
 
 
 .. _changes_7-4-4:
 
 Version 7.4.4 — 2024-03-14
```

### Comparing `coverage-7.5.0/CITATION.cff` & `coverage-7.5.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/CONTRIBUTORS.txt` & `coverage-7.5.1/CONTRIBUTORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 Clément Pit-Claudel
 Conrad Ho
 Cosimo Lupo
 Dan Hemberger
 Dan Riti
 Dan Wandschneider
 Danek Duvall
+Daniel Diniz
 Daniel Hahler
 Danny Allen
 David Christian
 David MacIver
 David Stanek
 David Szotten
 Dennis Sweeney
```

### Comparing `coverage-7.5.0/LICENSE.txt` & `coverage-7.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/MANIFEST.in` & `coverage-7.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/Makefile` & `coverage-7.5.1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Makefile for utility work on coverage.py.
 
 .DEFAULT_GOAL := help
 
 
 ##@ Utilities
 
-.PHONY: help clean_platform clean sterile
+.PHONY: help clean_platform clean sterile install
 
 help:					## Show this help.
 	@# Adapted from https://www.thapaliya.com/en/writings/well-documented-makefiles/
 	@echo Available targets:
 	@awk -F ':.*##' '/^[^: ]+:.*##/{printf "  \033[1m%-20s\033[m %s\n",$$1,$$2} /^##@/{printf "\n%s\n",substr($$0,5)}' $(MAKEFILE_LIST)
 
 _clean_platform:
@@ -46,14 +46,17 @@
 	@rm -rf tests/actual
 	@-make -C tests/gold/html clean
 
 sterile: clean				## Remove all non-controlled content, even if expensive.
 	rm -rf .tox
 	rm -f cheats.txt
 
+install:				## Install the developer tools
+	python3 -m pip install -r requirements/dev.pip
+
 
 ##@ Tests and quality checks
 
 .PHONY: lint smoke
 
 lint:					## Run linters and checkers.
 	tox -q -e lint
@@ -69,18 +72,18 @@
 
 .PHONY: metacov metahtml metasmoke
 
 metacov:				## Run meta-coverage, measuring ourself.
 	COVERAGE_COVERAGE=yes tox -q $(ARGS)
 
 metahtml:				## Produce meta-coverage HTML reports.
-	python igor.py combine_html
+	tox exec -q $(ARGS) -- python3 igor.py combine_html
 
 metasmoke:
-	COVERAGE_TEST_CORES=ctrace ARGS="-e py39" make metacov metahtml
+	COVERAGE_TEST_CORES=ctrace ARGS="-e py39" make --keep-going metacov metahtml
 
 
 ##@ Requirements management
 
 # When updating requirements, a few rules to follow:
 #
 # 1) Don't install more than one .pip file at once. Always use pip-compile to
@@ -188,14 +191,15 @@
 relbranch:				#: Create the branch for releasing (see howto.txt).
 	git switch -c nedbat/release-$$(date +%Y%m%d)
 
 relcommit1:				#: Commit the first release changes (see howto.txt).
 	git commit -am "docs: prep for $$(python setup.py --version)"
 
 relcommit2:				#: Commit the latest sample HTML report (see howto.txt).
+	git add doc/sample_html
 	git commit -am "docs: sample HTML for $$(python setup.py --version)"
 
 kit:					## Make the source distribution.
 	python -m build
 
 kit_upload:				## Upload the built distributions to PyPI.
 	twine upload dist/*
```

### Comparing `coverage-7.5.0/NOTICE.txt` & `coverage-7.5.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/PKG-INFO` & `coverage-7.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: coverage
-Version: 7.5.0
+Version: 7.5.1
 Summary: Code coverage measurement for Python
 Home-page: https://github.com/nedbat/coveragepy
-Author: Ned Batchelder and 225 others
+Author: Ned Batchelder and 226 others
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
-Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.0
+Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.1
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-coverage?utm_source=pypi-coverage&utm_medium=referral&utm_campaign=pypi
 Project-URL: Issues, https://github.com/nedbat/coveragepy/issues
 Project-URL: Mastodon, https://hachyderm.io/@coveragepy
 Project-URL: Mastodon (nedbat), https://hachyderm.io/@nedbat
 Keywords: code coverage testing
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,15 @@
 
 * Python 3.8 through 3.12, and 3.13.0a6 and up.
 * PyPy3 versions 3.8 through 3.10.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
-.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.0/
+.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.1/
 .. _GitHub: https://github.com/nedbat/coveragepy
 
 **New in 7.x:**
 initial function/class reporting;
 experimental support for sys.monitoring;
 dropped support for Python 3.7;
 added ``Coverage.collect()`` context manager;
@@ -108,23 +108,23 @@
 
 Getting Started
 ---------------
 
 Looking to run ``coverage`` on your test suite? See the `Quick Start section`_
 of the docs.
 
-.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.0/#quick-start
+.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.1/#quick-start
 
 
 Change history
 --------------
 
 The complete history of changes is on the `change history page`_.
 
-.. _change history page: https://coverage.readthedocs.io/en/7.5.0/changes.html
+.. _change history page: https://coverage.readthedocs.io/en/7.5.1/changes.html
 
 
 Code of Conduct
 ---------------
 
 Everyone participating in the coverage.py project is expected to treat other
 people with respect and to follow the guidelines articulated in the `Python
@@ -135,15 +135,15 @@
 
 Contributing
 ------------
 
 Found a bug? Want to help improve the code or documentation? See the
 `Contributing section`_ of the docs.
 
-.. _Contributing section: https://coverage.readthedocs.io/en/7.5.0/contributing.html
+.. _Contributing section: https://coverage.readthedocs.io/en/7.5.1/contributing.html
 
 
 Security
 --------
 
 To report a security vulnerability, please use the `Tidelift security
 contact`_.  Tidelift will coordinate the fix and disclosure.
@@ -163,15 +163,15 @@
 .. |test-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml
     :alt: Test suite status
 .. |quality-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml
     :alt: Quality check status
 .. |docs| image:: https://readthedocs.org/projects/coverage/badge/?version=latest&style=flat
-    :target: https://coverage.readthedocs.io/en/7.5.0/
+    :target: https://coverage.readthedocs.io/en/7.5.1/
     :alt: Documentation
 .. |kit| image:: https://img.shields.io/pypi/v/coverage
     :target: https://pypi.org/project/coverage/
     :alt: PyPI status
 .. |versions| image:: https://img.shields.io/pypi/pyversions/coverage.svg?logo=python&logoColor=FBE072
     :target: https://pypi.org/project/coverage/
     :alt: Python versions supported
```

### Comparing `coverage-7.5.0/README.rst` & `coverage-7.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/ci/comment_on_fixes.py` & `coverage-7.5.1/ci/comment_on_fixes.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/ci/download_gha_artifacts.py` & `coverage-7.5.1/ci/download_gha_artifacts.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/ci/parse_relnotes.py` & `coverage-7.5.1/ci/parse_relnotes.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/ci/session.py` & `coverage-7.5.1/ci/session.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/ci/trigger_build_kits.py` & `coverage-7.5.1/ci/trigger_build_kits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/__init__.py` & `coverage-7.5.1/coverage/__init__.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/annotate.py` & `coverage-7.5.1/coverage/annotate.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/bytecode.py` & `coverage-7.5.1/coverage/bytecode.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/cmdline.py` & `coverage-7.5.1/coverage/cmdline.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/collector.py` & `coverage-7.5.1/coverage/collector.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/config.py` & `coverage-7.5.1/coverage/config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/context.py` & `coverage-7.5.1/coverage/context.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/control.py` & `coverage-7.5.1/coverage/control.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/datastack.c` & `coverage-7.5.1/coverage/ctracer/datastack.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/datastack.h` & `coverage-7.5.1/coverage/ctracer/datastack.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/filedisp.c` & `coverage-7.5.1/coverage/ctracer/filedisp.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/filedisp.h` & `coverage-7.5.1/coverage/ctracer/filedisp.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/module.c` & `coverage-7.5.1/coverage/ctracer/module.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/stats.h` & `coverage-7.5.1/coverage/ctracer/stats.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/tracer.c` & `coverage-7.5.1/coverage/ctracer/tracer.c`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/tracer.h` & `coverage-7.5.1/coverage/ctracer/tracer.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/ctracer/util.h` & `coverage-7.5.1/coverage/ctracer/util.h`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/data.py` & `coverage-7.5.1/coverage/data.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/debug.py` & `coverage-7.5.1/coverage/debug.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/disposition.py` & `coverage-7.5.1/coverage/disposition.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/env.py` & `coverage-7.5.1/coverage/env.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/exceptions.py` & `coverage-7.5.1/coverage/exceptions.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/execfile.py` & `coverage-7.5.1/coverage/execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/files.py` & `coverage-7.5.1/coverage/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,16 +83,14 @@
                     cf = f
                     break
         cf = abs_file(cf)
         CANONICAL_FILENAME_CACHE[filename] = cf
     return CANONICAL_FILENAME_CACHE[filename]
 
 
-MAX_FLAT = 100
-
 def flat_rootname(filename: str) -> str:
     """A base for a flat file name to correspond to this file.
 
     Useful for writing files about the code where you want all the files in
     the same directory, but need to differentiate same-named files from
     different directories.
```

### Comparing `coverage-7.5.0/coverage/html.py` & `coverage-7.5.1/coverage/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import collections
 import dataclasses
 import datetime
 import functools
 import json
 import os
 import re
-import shutil
 import string
 
 from dataclasses import dataclass, field
 from typing import Any, Iterable, TYPE_CHECKING
 
 import coverage
 from coverage.data import CoverageData, add_data_to_hash
@@ -217,15 +216,14 @@
 
     # These files will be copied from the htmlfiles directory to the output
     # directory.
     STATIC_FILES = [
         "style.css",
         "coverage_html.js",
         "keybd_closed.png",
-        "keybd_open.png",
         "favicon_32.png",
     ]
 
     def __init__(self, cov: Coverage) -> None:
         self.coverage = cov
         self.config = self.coverage.config
         self.directory = self.config.html_dir
@@ -235,19 +233,15 @@
             self.skip_covered = self.config.skip_covered
         self.skip_empty = self.config.html_skip_empty
         if self.skip_empty is None:
             self.skip_empty = self.config.skip_empty
 
         title = self.config.html_title
 
-        self.extra_css: str | None
-        if self.config.extra_css:
-            self.extra_css = os.path.basename(self.config.extra_css)
-        else:
-            self.extra_css = None
+        self.extra_css = bool(self.config.extra_css)
 
         self.data = self.coverage.get_data()
         self.has_arcs = self.data.has_arcs()
 
         self.index_pages: dict[str, IndexPage] = {
             "file": self.new_index_page("file", "files"),
         }
@@ -267,14 +261,15 @@
             "__url__": __url__,
             "__version__": coverage.__version__,
             "title": title,
             "time_stamp": format_local_datetime(datetime.datetime.now()),
             "extra_css": self.extra_css,
             "has_arcs": self.has_arcs,
             "show_contexts": self.config.show_contexts,
+            "statics": {},
 
             # Constants for all reports.
             # These css classes determine which lines are highlighted by default.
             "category": {
                 "exc": "exc show_exc",
                 "mis": "mis show_mis",
                 "par": "par run show_par",
@@ -320,14 +315,17 @@
                 files_to_report.append(ftr)
             else:
                 file_be_gone(os.path.join(self.directory, ftr.html_filename))
 
         if not have_data:
             raise NoDataError("No data to report.")
 
+        self.make_directory()
+        self.make_local_static_report_files()
+
         if files_to_report:
             for ftr1, ftr2 in zip(files_to_report[:-1], files_to_report[1:]):
                 ftr1.next_html = ftr2.html_filename
                 ftr2.prev_html = ftr1.html_filename
             files_to_report[0].prev_html = "index.html"
             files_to_report[-1].next_html = "index.html"
 
@@ -344,44 +342,59 @@
         else:
             first_html = final_html = "index.html"
         self.write_file_index_page(first_html, final_html)
 
         # Write function and class index pages.
         self.write_region_index_pages(files_to_report)
 
-        self.make_local_static_report_files()
         return (
             self.index_pages["file"].totals.n_statements
             and self.index_pages["file"].totals.pc_covered
         )
 
     def make_directory(self) -> None:
         """Make sure our htmlcov directory exists."""
         ensure_dir(self.directory)
         if not os.listdir(self.directory):
             self.directory_was_empty = True
 
+    def copy_static_file(self, src: str, slug: str = "") -> None:
+        """Copy a static file into the output directory with cache busting."""
+        with open(src, "rb") as f:
+            text = f.read()
+        h = Hasher()
+        h.update(text)
+        cache_bust = h.hexdigest()[:8]
+        src_base = os.path.basename(src)
+        dest = src_base.replace(".", f"_cb_{cache_bust}.")
+        if not slug:
+            slug = src_base.replace(".", "_")
+        self.template_globals["statics"][slug] = dest # type: ignore
+        with open(os.path.join(self.directory, dest), "wb") as f:
+            f.write(text)
+
     def make_local_static_report_files(self) -> None:
         """Make local instances of static files for HTML report."""
+
         # The files we provide must always be copied.
         for static in self.STATIC_FILES:
-            shutil.copyfile(data_filename(static), os.path.join(self.directory, static))
+            self.copy_static_file(data_filename(static))
+
+        # The user may have extra CSS they want copied.
+        if self.extra_css:
+            assert self.config.extra_css is not None
+            self.copy_static_file(self.config.extra_css, slug="extra_css")
 
         # Only write the .gitignore file if the directory was originally empty.
-        # .gitignore can't be copied from the source tree because it would
-        # prevent the static files from being checked in.
+        # .gitignore can't be copied from the source tree because if it was in
+        # the source tree, it would stop the static files from being checked in.
         if self.directory_was_empty:
             with open(os.path.join(self.directory, ".gitignore"), "w") as fgi:
                 fgi.write("# Created by coverage.py\n*\n")
 
-        # The user may have extra CSS they want copied.
-        if self.extra_css:
-            assert self.config.extra_css is not None
-            shutil.copyfile(self.config.extra_css, os.path.join(self.directory, self.extra_css))
-
     def should_report(self, analysis: Analysis, index_page: IndexPage) -> bool:
         """Determine if we'll report this file or region."""
         # Get the numbers for this file.
         nums = analysis.numbers
         index_page.totals += nums
 
         if self.skip_covered:
@@ -404,16 +417,14 @@
         """Generate an HTML page for one source file.
 
         If the page on disk is already correct based on our incremental status
         checking, then the page doesn't have to be generated, and this function
         only does page summary bookkeeping.
 
         """
-        self.make_directory()
-
         # Find out if the page on disk is already correct.
         if self.incr.can_skip_file(self.data, ftr.fr, ftr.rootname):
             self.index_pages["file"].summaries.append(self.incr.index_info(ftr.rootname))
             return
 
         # Write the HTML page for this source file.
         file_data = self.datagen.data_for_file(ftr.fr, ftr.analysis)
@@ -498,16 +509,14 @@
             nums = ftr.analysis.numbers,
         )
         self.index_pages["file"].summaries.append(index_info)
         self.incr.set_index_info(ftr.rootname, index_info)
 
     def write_file_index_page(self, first_html: str, final_html: str) -> None:
         """Write the file index page for this report."""
-        self.make_directory()
-
         index_file = self.write_index_page(
             self.index_pages["file"],
             first_html=first_html,
             final_html=final_html,
         )
 
         print_href = stdout_link(index_file, f"file://{os.path.abspath(index_file)}")
```

### Comparing `coverage-7.5.0/coverage/htmlfiles/coverage_html.js` & `coverage-7.5.1/coverage/htmlfiles/coverage_html.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -77,18 +77,42 @@
 
     // Sort all rows and afterwards append them in order to move them in the DOM.
     Array.from(th.closest("table").querySelectorAll("tbody tr"))
         .sort((rowA, rowB) => rowComparator(rowA, rowB, column) * (direction === "ascending" ? 1 : -1))
         .forEach(tr => tr.parentElement.appendChild(tr));
 
     // Save the sort order for next time.
-    localStorage.setItem(coverage.INDEX_SORT_STORAGE, JSON.stringify({
-        column,
-        direction
-    }));
+    if (th.id !== "region") {
+        let th_id = "file"; // Sort by file if we don't have a column id
+        let current_direction = direction;
+        const stored_list = localStorage.getItem(coverage.INDEX_SORT_STORAGE);
+        if (stored_list) {
+            ({
+                th_id,
+                direction
+            } = JSON.parse(stored_list))
+        }
+        localStorage.setItem(coverage.INDEX_SORT_STORAGE, JSON.stringify({
+            "th_id": th.id,
+            "direction": current_direction
+        }));
+        if (th.id !== th_id || document.getElementById("region")) {
+            // Sort column has changed, unset sorting by function or class.
+            localStorage.setItem(coverage.SORTED_BY_REGION, JSON.stringify({
+                "by_region": false,
+                "region_direction": current_direction
+            }));
+        }
+    } else {
+        // Sort column has changed to by function or class, remember that.
+        localStorage.setItem(coverage.SORTED_BY_REGION, JSON.stringify({
+            "by_region": true,
+            "region_direction": direction
+        }));
+    }
 }
 
 // Find all the elements with data-shortcut attribute, and use them to assign a shortcut key.
 coverage.assign_shortkeys = function() {
     document.querySelectorAll("[data-shortcut]").forEach(element => {
         document.addEventListener("keypress", event => {
             if (event.target.tagName.toLowerCase() === "input") {
@@ -226,30 +250,51 @@
 // Set up the click-to-sort columns.
 coverage.wire_up_sorting = function() {
     document.querySelectorAll("[data-sortable] th[aria-sort]").forEach(
         th => th.addEventListener("click", e => sortColumn(e.target))
     );
 
     // Look for a localStorage item containing previous sort settings:
-    var column = 0,
+    let th_id = "file",
         direction = "ascending";
     const stored_list = localStorage.getItem(coverage.INDEX_SORT_STORAGE);
     if (stored_list) {
         ({
-            column,
+            th_id,
             direction
         } = JSON.parse(stored_list));
     }
+    let by_region = false,
+        region_direction = "ascending";
+    const sorted_by_region = localStorage.getItem(coverage.SORTED_BY_REGION);
+    if (sorted_by_region) {
+        ({
+            by_region,
+            region_direction
+        } = JSON.parse(sorted_by_region));
+    }
 
-    const th = document.querySelector("[data-sortable]").tHead.rows[0].cells[column]; // nosemgrep: eslint.detect-object-injection
+    const region_id = "region";
+    if (by_region && document.getElementById(region_id)) {
+        direction = region_direction;
+    }
+    // If we are in a page that has a column with id of "region", sort on
+    // it if the last sort was by function or class.
+    let th;
+    if (document.getElementById(region_id)) {
+        th = document.getElementById(by_region ? region_id : th_id);
+    } else {
+        th = document.getElementById(th_id);
+    }
     th.setAttribute("aria-sort", direction === "ascending" ? "descending" : "ascending");
     th.click()
 };
 
 coverage.INDEX_SORT_STORAGE = "COVERAGE_INDEX_SORT_2";
+coverage.SORTED_BY_REGION = "COVERAGE_SORT_REGION";
 
 // Loaded on index.html
 coverage.index_ready = function() {
     coverage.assign_shortkeys();
     coverage.wire_up_filter();
     coverage.wire_up_sorting();
```

### Comparing `coverage-7.5.0/coverage/htmlfiles/favicon_32.png` & `coverage-7.5.1/coverage/htmlfiles/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/htmlfiles/index.html` & `coverage-7.5.1/coverage/htmlfiles/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 {# For details: https://github.com/nedbat/coveragepy/blob/master/NOTICE.txt #}
 
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>{{ title|escape }}</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
+    <link rel="icon" sizes="32x32" href="{{ statics.favicon_32_png }}">
+    <link rel="stylesheet" href="{{ statics.style_css }}" type="text/css">
     {% if extra_css %}
-        <link rel="stylesheet" href="{{ extra_css }}" type="text/css">
+        <link rel="stylesheet" href="{{ statics.extra_css }}" type="text/css">
     {% endif %}
-    <script src="coverage_html.js" defer></script>
+    <script src="{{ statics.coverage_html_js }}" defer></script>
 </head>
 <body class="indexfile">
 
 <header>
     <div class="content">
         <h1>{{ title|escape }}:
             <span class="pc_cov">{{totals.pc_covered_str}}%</span>
         </h1>
 
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="{{ statics.keybd_closed_png }}" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         {% if column2 %}
@@ -78,26 +78,26 @@
 </header>
 
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             {# The title="" attr doesn't work in Safari. #}
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
                 {% if column2 %}
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">{{ column2 }}<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">{{ column2 }}<span class="arrows"></span></th>
                 {% endif %}
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
                 {% if has_arcs %}
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
                 {% endif %}
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             {% for region in regions %}
             <tr class="region">
                 <td class="name left"><a href="{{region.url}}">{{region.file}}</a></td>
                 {% if column2 %}
```

### Comparing `coverage-7.5.0/coverage/htmlfiles/keybd_closed.png` & `coverage-7.5.1/coverage/htmlfiles/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/htmlfiles/pyfile.html` & `coverage-7.5.1/coverage/htmlfiles/pyfile.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 {# For details: https://github.com/nedbat/coveragepy/blob/master/NOTICE.txt #}
 
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for {{relative_filename|escape}}: {{nums.pc_covered_str}}%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
+    <link rel="icon" sizes="32x32" href="{{ statics.favicon_32_png }}">
+    <link rel="stylesheet" href="{{ statics.style_css }}" type="text/css">
     {% if extra_css %}
-        <link rel="stylesheet" href="{{ extra_css }}" type="text/css">
+        <link rel="stylesheet" href="{{ statics.extra_css }}" type="text/css">
     {% endif %}
 
     {% if contexts_json %}
     <script type="text/javascript">
         contexts = {{ contexts_json }}
     </script>
     {% endif %}
 
-    <script src="coverage_html.js" defer></script>
+    <script src="{{ statics.coverage_html_js }}" defer></script>
 </head>
 <body class="pyfile">
 
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>{{relative_filename|escape}}</b>:
             <span class="pc_cov">{{nums.pc_covered_str}}%</span>
         </h1>
 
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="{{ statics.keybd_closed_png }}" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
```

### Comparing `coverage-7.5.0/coverage/htmlfiles/style.css` & `coverage-7.5.1/coverage/htmlfiles/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/htmlfiles/style.scss` & `coverage-7.5.1/coverage/htmlfiles/style.scss`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/inorout.py` & `coverage-7.5.1/coverage/inorout.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/jsonreport.py` & `coverage-7.5.1/coverage/jsonreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/lcovreport.py` & `coverage-7.5.1/coverage/lcovreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/misc.py` & `coverage-7.5.1/coverage/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """Miscellaneous stuff for coverage.py."""
 
 from __future__ import annotations
 
 import contextlib
 import datetime
 import errno
+import functools
 import hashlib
 import importlib
 import importlib.util
 import inspect
 import locale
 import os
 import os.path
@@ -309,14 +310,15 @@
     sys.modules[modname] = mod
     assert spec.loader is not None
     spec.loader.exec_module(mod)
 
     return mod
 
 
+@functools.lru_cache(maxsize=None)
 def _human_key(s: str) -> tuple[list[str | int], str]:
     """Turn a string into a list of string and number chunks.
 
     "z23a" -> (["z", 23, "a"], "z23a")
 
     The original string is appended as a last value to ensure the
     key is unique enough so that "x1y" and "x001y" can be distinguished.
```

### Comparing `coverage-7.5.0/coverage/multiproc.py` & `coverage-7.5.1/coverage/multiproc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/numbits.py` & `coverage-7.5.1/coverage/numbits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/parser.py` & `coverage-7.5.1/coverage/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         """
         combined = join_regex(regexes)
         regex_c = re.compile(combined)
         matches = set()
         for i, ltext in enumerate(self.lines, start=1):
             if regex_c.search(ltext):
-                matches.add(i)
+                matches.add(self._multiline.get(i, i))
         return matches
 
     def _raw_parse(self) -> None:
         """Parse the source to find the interesting facts about its lines.
 
         A handful of attributes are updated.
 
@@ -1089,15 +1089,15 @@
     _handle__FunctionDef = _handle_decorated
     _handle__AsyncFunctionDef = _handle_decorated
 
     def _handle__If(self, node: ast.If) -> set[ArcStart]:
         start = self.line_for_node(node.test)
         from_start = ArcStart(start, cause="the condition on line {lineno} was never true")
         exits = self.add_body_arcs(node.body, from_start=from_start)
-        from_start = ArcStart(start, cause="the condition on line {lineno} was never false")
+        from_start = ArcStart(start, cause="the condition on line {lineno} was always true")
         exits |= self.add_body_arcs(node.orelse, from_start=from_start)
         return exits
 
     if sys.version_info >= (3, 10):
         def _handle__Match(self, node: ast.Match) -> set[ArcStart]:
             start = self.line_for_node(node)
             last_start = start
@@ -1283,15 +1283,15 @@
         exits = self.add_body_arcs(node.body, from_start=from_start)
         for xit in exits:
             self.add_arc(xit.lineno, to_top, xit.cause)
         exits = set()
         my_block = self.block_stack.pop()
         assert isinstance(my_block, LoopBlock)
         exits.update(my_block.break_exits)
-        from_start = ArcStart(start, cause="the condition on line {lineno} was never false")
+        from_start = ArcStart(start, cause="the condition on line {lineno} was always true")
         if node.orelse:
             else_exits = self.add_body_arcs(node.orelse, from_start=from_start)
             exits |= else_exits
         else:
             # No `else` clause: you can exit from the start.
             if not constant_test:
                 exits.add(from_start)
```

### Comparing `coverage-7.5.0/coverage/phystokens.py` & `coverage-7.5.1/coverage/phystokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,34 +74,27 @@
             last_line = ltext
         if ttype not in (tokenize.NEWLINE, tokenize.NL):
             last_ttext = ttext
         yield tokenize.TokenInfo(ttype, ttext, (slineno, scol), (elineno, ecol), ltext)
         last_lineno = elineno
 
 
-class SoftKeywordFinder(ast.NodeVisitor):
+def find_soft_key_lines(source: str) -> set[TLineNo]:
     """Helper for finding lines with soft keywords, like match/case lines."""
-    def __init__(self, source: str) -> None:
-        # This will be the set of line numbers that start with a soft keyword.
-        self.soft_key_lines: set[TLineNo] = set()
-        self.visit(ast.parse(source))
-
-    if sys.version_info >= (3, 10):
-        def visit_Match(self, node: ast.Match) -> None:
-            """Invoked by ast.NodeVisitor.visit"""
-            self.soft_key_lines.add(node.lineno)
+    soft_key_lines: set[TLineNo] = set()
+
+    for node in ast.walk(ast.parse(source)):
+        if sys.version_info >= (3, 10) and isinstance(node, ast.Match):
+            soft_key_lines.add(node.lineno)
             for case in node.cases:
-                self.soft_key_lines.add(case.pattern.lineno)
-            self.generic_visit(node)
+                soft_key_lines.add(case.pattern.lineno)
+        elif sys.version_info >= (3, 12) and isinstance(node, ast.TypeAlias):
+            soft_key_lines.add(node.lineno)
 
-    if sys.version_info >= (3, 12):
-        def visit_TypeAlias(self, node: ast.TypeAlias) -> None:
-            """Invoked by ast.NodeVisitor.visit"""
-            self.soft_key_lines.add(node.lineno)
-            self.generic_visit(node)
+    return soft_key_lines
 
 
 def source_token_lines(source: str) -> TSourceTokenLines:
     """Generate a series of lines, one for each line in `source`.
 
     Each line is a list of pairs, each pair is a token::
 
@@ -120,15 +113,15 @@
     line: list[tuple[str, str]] = []
     col = 0
 
     source = source.expandtabs(8).replace("\r\n", "\n")
     tokgen = generate_tokens(source)
 
     if env.PYBEHAVIOR.soft_keywords:
-        soft_key_lines = SoftKeywordFinder(source).soft_key_lines
+        soft_key_lines = find_soft_key_lines(source)
 
     for ttype, ttext, (sline, scol), (_, ecol), _ in _phys_tokens(tokgen):
         mark_start = True
         for part in re.split("(\n)", ttext):
             if part == "\n":
                 yield line
                 line = []
@@ -147,16 +140,15 @@
                     if keyword.iskeyword(ttext):
                         # Hard keywords are always keywords.
                         tok_class = "key"
                     elif sys.version_info >= (3, 10):   # PYVERSIONS
                         # Need the version_info check to keep mypy from borking
                         # on issoftkeyword here.
                         if env.PYBEHAVIOR.soft_keywords and keyword.issoftkeyword(ttext):
-                            # Soft keywords appear at the start of the line,
-                            # on lines that start match or case statements.
+                            # Soft keywords appear at the start of their line.
                             if len(line) == 0:
                                 is_start_of_line = True
                             elif (len(line) == 1) and line[0][0] == "ws":
                                 is_start_of_line = True
                             else:
                                 is_start_of_line = False
                             if is_start_of_line and sline in soft_key_lines:
```

### Comparing `coverage-7.5.0/coverage/plugin.py` & `coverage-7.5.1/coverage/plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/plugin_support.py` & `coverage-7.5.1/coverage/plugin_support.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/python.py` & `coverage-7.5.1/coverage/python.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/pytracer.py` & `coverage-7.5.1/coverage/pytracer.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/regions.py` & `coverage-7.5.1/coverage/regions.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,34 +17,48 @@
 class Context:
     """The nested named context of a function or class."""
     name: str
     kind: str
     lines: set[int]
 
 
-class RegionFinder(ast.NodeVisitor):
+class RegionFinder:
     """An ast visitor that will find and track regions of code.
 
     Functions and classes are tracked by name. Results are in the .regions
     attribute.
 
     """
     def __init__(self) -> None:
         self.regions: list[CodeRegion] = []
         self.context: list[Context] = []
 
     def parse_source(self, source: str) -> None:
         """Parse `source` and walk the ast to populate the .regions attribute."""
-        self.visit(ast.parse(source))
+        self.handle_node(ast.parse(source))
 
     def fq_node_name(self) -> str:
         """Get the current fully qualified name we're processing."""
         return ".".join(c.name for c in self.context)
 
-    def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
+    def handle_node(self, node: ast.AST) -> None:
+        """Recursively handle any node."""
+        if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
+            self.handle_FunctionDef(node)
+        elif isinstance(node, ast.ClassDef):
+            self.handle_ClassDef(node)
+        else:
+            self.handle_node_body(node)
+
+    def handle_node_body(self, node: ast.AST) -> None:
+        """Recursively handle the nodes in this node's body, if any."""
+        for body_node in getattr(node, "body", ()):
+            self.handle_node(body_node)
+
+    def handle_FunctionDef(self, node: ast.FunctionDef | ast.AsyncFunctionDef) -> None:
         """Called for `def` or `async def`."""
         lines = set(range(node.body[0].lineno, cast(int, node.body[-1].end_lineno) + 1))
         if self.context and self.context[-1].kind == "class":
             # Function bodies are part of their enclosing class.
             self.context[-1].lines |= lines
         # Function bodies should be excluded from the nearest enclosing function.
         for ancestor in reversed(self.context):
@@ -56,35 +70,33 @@
             CodeRegion(
                 kind="function",
                 name=self.fq_node_name(),
                 start=node.lineno,
                 lines=lines,
             )
         )
-        self.generic_visit(node)
+        self.handle_node_body(node)
         self.context.pop()
 
-    visit_AsyncFunctionDef = visit_FunctionDef  # type: ignore[assignment]
-
-    def visit_ClassDef(self, node: ast.ClassDef) -> None:
+    def handle_ClassDef(self, node: ast.ClassDef) -> None:
         """Called for `class`."""
         # The lines for a class are the lines in the methods of the class.
         # We start empty, and count on visit_FunctionDef to add the lines it
         # finds.
         lines: set[int] = set()
         self.context.append(Context(node.name, "class", lines))
         self.regions.append(
             CodeRegion(
                 kind="class",
                 name=self.fq_node_name(),
                 start=node.lineno,
                 lines=lines,
             )
         )
-        self.generic_visit(node)
+        self.handle_node_body(node)
         self.context.pop()
         # Class bodies should be excluded from the enclosing classes.
         for ancestor in reversed(self.context):
             if ancestor.kind == "class":
                 ancestor.lines -= lines
```

### Comparing `coverage-7.5.0/coverage/report.py` & `coverage-7.5.1/coverage/report.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/report_core.py` & `coverage-7.5.1/coverage/report_core.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/results.py` & `coverage-7.5.1/coverage/results.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/sqldata.py` & `coverage-7.5.1/coverage/sqldata.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/sqlitedb.py` & `coverage-7.5.1/coverage/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/sysmon.py` & `coverage-7.5.1/coverage/sysmon.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/templite.py` & `coverage-7.5.1/coverage/templite.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/tomlconfig.py` & `coverage-7.5.1/coverage/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/tracer.pyi` & `coverage-7.5.1/coverage/tracer.pyi`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/types.py` & `coverage-7.5.1/coverage/types.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage/version.py` & `coverage-7.5.1/coverage/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """The version and URL for coverage.py"""
 # This file is exec'ed in setup.py, don't import anything!
 
 from __future__ import annotations
 
 # version_info: same semantics as sys.version_info.
 # _dev: the .devN suffix if any.
-version_info = (7, 5, 0, "final", 0)
+version_info = (7, 5, 1, "final", 0)
 _dev = 0
 
 
 def _make_version(
     major: int,
     minor: int,
     micro: int,
```

### Comparing `coverage-7.5.0/coverage/xmlreport.py` & `coverage-7.5.1/coverage/xmlreport.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/coverage.egg-info/PKG-INFO` & `coverage-7.5.1/coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: coverage
-Version: 7.5.0
+Version: 7.5.1
 Summary: Code coverage measurement for Python
 Home-page: https://github.com/nedbat/coveragepy
-Author: Ned Batchelder and 225 others
+Author: Ned Batchelder and 226 others
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
-Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.0
+Project-URL: Documentation, https://coverage.readthedocs.io/en/7.5.1
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-coverage?utm_source=pypi-coverage&utm_medium=referral&utm_campaign=pypi
 Project-URL: Issues, https://github.com/nedbat/coveragepy/issues
 Project-URL: Mastodon, https://hachyderm.io/@coveragepy
 Project-URL: Mastodon (nedbat), https://hachyderm.io/@nedbat
 Keywords: code coverage testing
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,15 @@
 
 * Python 3.8 through 3.12, and 3.13.0a6 and up.
 * PyPy3 versions 3.8 through 3.10.
 
 Documentation is on `Read the Docs`_.  Code repository and issue tracker are on
 `GitHub`_.
 
-.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.0/
+.. _Read the Docs: https://coverage.readthedocs.io/en/7.5.1/
 .. _GitHub: https://github.com/nedbat/coveragepy
 
 **New in 7.x:**
 initial function/class reporting;
 experimental support for sys.monitoring;
 dropped support for Python 3.7;
 added ``Coverage.collect()`` context manager;
@@ -108,23 +108,23 @@
 
 Getting Started
 ---------------
 
 Looking to run ``coverage`` on your test suite? See the `Quick Start section`_
 of the docs.
 
-.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.0/#quick-start
+.. _Quick Start section: https://coverage.readthedocs.io/en/7.5.1/#quick-start
 
 
 Change history
 --------------
 
 The complete history of changes is on the `change history page`_.
 
-.. _change history page: https://coverage.readthedocs.io/en/7.5.0/changes.html
+.. _change history page: https://coverage.readthedocs.io/en/7.5.1/changes.html
 
 
 Code of Conduct
 ---------------
 
 Everyone participating in the coverage.py project is expected to treat other
 people with respect and to follow the guidelines articulated in the `Python
@@ -135,15 +135,15 @@
 
 Contributing
 ------------
 
 Found a bug? Want to help improve the code or documentation? See the
 `Contributing section`_ of the docs.
 
-.. _Contributing section: https://coverage.readthedocs.io/en/7.5.0/contributing.html
+.. _Contributing section: https://coverage.readthedocs.io/en/7.5.1/contributing.html
 
 
 Security
 --------
 
 To report a security vulnerability, please use the `Tidelift security
 contact`_.  Tidelift will coordinate the fix and disclosure.
@@ -163,15 +163,15 @@
 .. |test-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/testsuite.yml
     :alt: Test suite status
 .. |quality-status| image:: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml/badge.svg?branch=master&event=push
     :target: https://github.com/nedbat/coveragepy/actions/workflows/quality.yml
     :alt: Quality check status
 .. |docs| image:: https://readthedocs.org/projects/coverage/badge/?version=latest&style=flat
-    :target: https://coverage.readthedocs.io/en/7.5.0/
+    :target: https://coverage.readthedocs.io/en/7.5.1/
     :alt: Documentation
 .. |kit| image:: https://img.shields.io/pypi/v/coverage
     :target: https://pypi.org/project/coverage/
     :alt: PyPI status
 .. |versions| image:: https://img.shields.io/pypi/pyversions/coverage.svg?logo=python&logoColor=FBE072
     :target: https://pypi.org/project/coverage/
     :alt: Python versions supported
```

### Comparing `coverage-7.5.0/coverage.egg-info/SOURCES.txt` & `coverage-7.5.1/coverage.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 coverage/ctracer/tracer.c
 coverage/ctracer/tracer.h
 coverage/ctracer/util.h
 coverage/htmlfiles/coverage_html.js
 coverage/htmlfiles/favicon_32.png
 coverage/htmlfiles/index.html
 coverage/htmlfiles/keybd_closed.png
-coverage/htmlfiles/keybd_open.png
 coverage/htmlfiles/pyfile.html
 coverage/htmlfiles/style.css
 coverage/htmlfiles/style.scss
 doc/api.rst
 doc/api_coverage.rst
 doc/api_coveragedata.rst
 doc/api_exceptions.rst
@@ -138,17 +137,16 @@
 doc/trouble.rst
 doc/whatsnew5x.rst
 doc/_static/coverage.css
 doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
 doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
 doc/media/sleepy-snake-600.png
 doc/media/sleepy-snake-circle-150.png
-doc/sample_html/favicon_32.png
-doc/sample_html/keybd_closed.png
-doc/sample_html/keybd_open.png
+doc/sample_html/favicon_32_cb_58284776.png
+doc/sample_html/keybd_closed_cb_ce680311.png
 lab/README.txt
 lab/bpo_prelude.py
 lab/branch_trace.py
 lab/branches.py
 lab/compare_times.sh
 lab/coverage-03.dtd
 lab/coverage-04.dtd
@@ -320,22 +318,21 @@
 tests/gold/html/partial/partial_py.html
 tests/gold/html/partial_626/class_index.html
 tests/gold/html/partial_626/function_index.html
 tests/gold/html/partial_626/index.html
 tests/gold/html/partial_626/partial_py.html
 tests/gold/html/styled/a_py.html
 tests/gold/html/styled/class_index.html
-tests/gold/html/styled/extra.css
 tests/gold/html/styled/function_index.html
 tests/gold/html/styled/index.html
+tests/gold/html/styled/myextra.css
 tests/gold/html/styled/style.css
 tests/gold/html/support/coverage_html.js
 tests/gold/html/support/favicon_32.png
 tests/gold/html/support/keybd_closed.png
-tests/gold/html/support/keybd_open.png
 tests/gold/html/support/style.css
 tests/gold/html/unicode/class_index.html
 tests/gold/html/unicode/function_index.html
 tests/gold/html/unicode/index.html
 tests/gold/html/unicode/unicode_py.html
 tests/gold/testing/getty/gettysburg.txt
 tests/gold/testing/xml/output.xml
```

### Comparing `coverage-7.5.0/doc/_static/coverage.css` & `coverage-7.5.1/doc/_static/coverage.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/api.rst` & `coverage-7.5.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/api_module.rst` & `coverage-7.5.1/doc/api_module.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/api_plugin.rst` & `coverage-7.5.1/doc/api_plugin.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/branch.rst` & `coverage-7.5.1/doc/branch.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/changes.rst` & `coverage-7.5.1/doc/changes.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/cmd.rst` & `coverage-7.5.1/doc/cmd.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/cog_helpers.py` & `coverage-7.5.1/doc/cog_helpers.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/conf.py` & `coverage-7.5.1/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 # @@@ editable
 copyright = "2009–2024, Ned Batchelder" # pylint: disable=redefined-builtin
 # The short X.Y.Z version.
-version = "7.5.0"
+version = "7.5.1"
 # The full version, including alpha/beta/rc tags.
-release = "7.5.0"
+release = "7.5.1"
 # The date of release, in "monthname day, year" format.
-release_date = "April 23, 2024"
+release_date = "May 4, 2024"
 # @@@ end
 
 rst_epilog = f"""
 .. |release_date| replace:: {release_date}
 .. |coverage-equals-release| replace:: coverage=={release}
 .. |doc-url| replace:: https://coverage.readthedocs.io/en/{release}
 .. |br| raw:: html
@@ -122,18 +122,17 @@
 #modindex_common_prefix = []
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
 
 nitpick_ignore = [
-    ("py:class", "frame"),
-    ("py:class", "module"),
     ("py:class", "DefaultValue"),
     ("py:class", "FilePath"),
+    ("py:class", "types.FrameType"),
     ("py:class", "TWarnFn"),
     ("py:class", "TDebugCtl"),
 ]
 
 nitpick_ignore_regex = [
     (r"py:class", r"coverage\..*\..*"),
 ]
```

### Comparing `coverage-7.5.0/doc/config.rst` & `coverage-7.5.1/doc/config.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/contexts.rst` & `coverage-7.5.1/doc/contexts.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/contributing.rst` & `coverage-7.5.1/doc/contributing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,17 @@
     Ideally, use Python3.8 (the lowest version coverage.py supports).
 
 #.  Clone the repository::
 
     $ git clone https://github.com/GITHUB_USER/coveragepy
     $ cd coveragepy
 
-#.  Install the requirements::
+#.  Install the requirements with either of these commands::
 
+    $ make install
     $ python3 -m pip install -r requirements/dev.pip
 
     Note: You may need to upgrade pip to install the requirements.
 
 
 Running the tests
 -----------------
```

### Comparing `coverage-7.5.0/doc/dbschema.rst` & `coverage-7.5.1/doc/dbschema.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/dict.txt` & `coverage-7.5.1/doc/dict.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/excluding.rst` & `coverage-7.5.1/doc/excluding.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/faq.rst` & `coverage-7.5.1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/howitworks.rst` & `coverage-7.5.1/doc/howitworks.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/index.rst` & `coverage-7.5.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/install.rst` & `coverage-7.5.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png` & `coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png` & `coverage-7.5.1/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/media/sleepy-snake-600.png` & `coverage-7.5.1/doc/media/sleepy-snake-600.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/media/sleepy-snake-circle-150.png` & `coverage-7.5.1/doc/media/sleepy-snake-circle-150.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/migrating.rst` & `coverage-7.5.1/doc/migrating.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/other.rst` & `coverage-7.5.1/doc/other.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/plugins.rst` & `coverage-7.5.1/doc/plugins.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/python-coverage.1.txt` & `coverage-7.5.1/doc/python-coverage.1.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/requirements.pip` & `coverage-7.5.1/doc/requirements.pip`

 * *Files 14% similar despite different names*

```diff
@@ -2,50 +2,57 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    make doc_upgrade
 #
 alabaster==0.7.16
     # via sphinx
+anyio==4.3.0
+    # via
+    #   starlette
+    #   watchfiles
 attrs==23.2.0
     # via scriv
 babel==2.14.0
     # via sphinx
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   click-log
     #   scriv
+    #   uvicorn
 click-log==0.4.0
     # via scriv
 cogapp==3.4.1
     # via -r doc/requirements.in
 colorama==0.4.6
     # via sphinx-autobuild
 doc8==1.1.1
     # via -r doc/requirements.in
 docutils==0.20.1
     # via
     #   doc8
     #   restructuredtext-lint
     #   sphinx
     #   sphinx-rtd-theme
-idna==3.6
-    # via requests
+h11==0.14.0
+    # via uvicorn
+idna==3.7
+    # via
+    #   anyio
+    #   requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.3
     # via
     #   scriv
     #   sphinx
-livereload==2.6.3
-    # via sphinx-autobuild
 markdown-it-py==3.0.0
     # via scriv
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 packaging==24.0
@@ -64,28 +71,28 @@
     # via
     #   scriv
     #   sphinx
 restructuredtext-lint==1.4.0
     # via doc8
 scriv==1.5.1
     # via -r doc/requirements.in
-six==1.16.0
-    # via livereload
+sniffio==1.3.1
+    # via anyio
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r doc/requirements.in
     #   sphinx-autobuild
     #   sphinx-code-tabs
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-restbuilder
     #   sphinxcontrib-spelling
-sphinx-autobuild==2024.2.4
+sphinx-autobuild==2024.4.16
     # via -r doc/requirements.in
 sphinx-code-tabs==0.5.5
     # via -r doc/requirements.in
 sphinx-rtd-theme==2.0.0
     # via -r doc/requirements.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
@@ -101,13 +108,19 @@
     # via sphinx
 sphinxcontrib-restbuilder==0.3
     # via -r doc/requirements.in
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r doc/requirements.in
+starlette==0.37.2
+    # via sphinx-autobuild
 stevedore==5.2.0
     # via doc8
-tornado==6.4
-    # via livereload
 urllib3==2.2.1
     # via requests
+uvicorn==0.29.0
+    # via sphinx-autobuild
+watchfiles==0.21.0
+    # via sphinx-autobuild
+websockets==12.0
+    # via sphinx-autobuild
```

### Comparing `coverage-7.5.0/doc/sample_html/favicon_32.png` & `coverage-7.5.1/doc/sample_html/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/sample_html/keybd_closed.png` & `coverage-7.5.1/doc/sample_html/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/sleepy.rst` & `coverage-7.5.1/doc/sleepy.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/source.rst` & `coverage-7.5.1/doc/source.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/subprocess.rst` & `coverage-7.5.1/doc/subprocess.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/trouble.rst` & `coverage-7.5.1/doc/trouble.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/doc/whatsnew5x.rst` & `coverage-7.5.1/doc/whatsnew5x.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/howto.txt` & `coverage-7.5.1/howto.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/igor.py` & `coverage-7.5.1/igor.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/benchmark/benchmark.py` & `coverage-7.5.1/lab/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/benchmark/empty.py` & `coverage-7.5.1/lab/benchmark/empty.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/benchmark/run.py` & `coverage-7.5.1/lab/benchmark/run.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/branches.py` & `coverage-7.5.1/lab/branches.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/compare_times.sh` & `coverage-7.5.1/lab/compare_times.sh`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/coverage-03.dtd` & `coverage-7.5.1/lab/coverage-03.dtd`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/coverage-04.dtd` & `coverage-7.5.1/lab/coverage-04.dtd`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/extract_code.py` & `coverage-7.5.1/lab/extract_code.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/find_class.py` & `coverage-7.5.1/lab/find_class.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/genpy.py` & `coverage-7.5.1/lab/genpy.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/goals.py` & `coverage-7.5.1/lab/goals.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/hack_pyc.py` & `coverage-7.5.1/lab/hack_pyc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/new-data.js` & `coverage-7.5.1/lab/new-data.js`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/notes/bug1303.txt` & `coverage-7.5.1/lab/notes/bug1303.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/notes/pypy-738-decorated-functions.txt` & `coverage-7.5.1/lab/notes/pypy-738-decorated-functions.txt`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/parse_all.py` & `coverage-7.5.1/lab/parse_all.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/parser.py` & `coverage-7.5.1/lab/parser.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/pick.py` & `coverage-7.5.1/lab/pick.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/platform_info.py` & `coverage-7.5.1/lab/platform_info.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/run_sysmon.py` & `coverage-7.5.1/lab/run_sysmon.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/run_trace.py` & `coverage-7.5.1/lab/run_trace.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/select_contexts.py` & `coverage-7.5.1/lab/select_contexts.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/lab/show_pyc.py` & `coverage-7.5.1/lab/show_pyc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/metacov.ini` & `coverage-7.5.1/metacov.ini`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     # OS error conditions that we can't (or don't care to) replicate.
     pragma: cant happen
 
     # Obscure bugs in specific versions of interpreters, and so probably no
     # longer tested.
     pragma: obscure
 
+    # Lines that will never be called, but satisfy the type checker
+    pragma: never called
+
 partial_branches =
     pragma: part covered
     # A for-loop that always hits its break statement
     pragma: always breaks
     pragma: part started
     # If we're asserting that any() is true, it didn't finish.
     assert any\(
```

### Comparing `coverage-7.5.0/pyproject.toml` & `coverage-7.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/requirements/dev.in` & `coverage-7.5.1/requirements/dev.in`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/requirements/dev.pip` & `coverage-7.5.1/requirements/dev.pip`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 #    make upgrade
 #
 astroid==3.1.0
     # via pylint
 attrs==23.2.0
     # via hypothesis
-backports-tarfile==1.1.0
+backports-tarfile==1.1.1
     # via jaraco-context
 build==1.2.1
     # via check-manifest
 cachetools==5.3.3
     # via tox
 certifi==2024.2.2
     # via requests
@@ -45,15 +45,15 @@
     # via
     #   tox
     #   virtualenv
 flaky==3.8.1
     # via -r requirements/pytest.in
 greenlet==3.0.3
     # via -r requirements/dev.in
-hypothesis==6.100.1
+hypothesis==6.100.2
     # via -r requirements/pytest.in
 idna==3.7
     # via requests
 importlib-metadata==7.1.0
     # via
     #   build
     #   keyring
@@ -68,15 +68,15 @@
     # via keyring
 jaraco-context==5.3.0
     # via keyring
 jaraco-functools==4.0.1
     # via keyring
 jedi==0.19.1
     # via pudb
-keyring==25.1.0
+keyring==25.2.0
     # via twine
 libsass==0.23.0
     # via -r requirements/dev.in
 markdown-it-py==3.0.0
     # via rich
 mccabe==0.7.0
     # via pylint
@@ -95,15 +95,15 @@
     #   pyproject-api
     #   pytest
     #   tox
 parso==0.8.4
     # via jedi
 pkginfo==1.10.0
     # via twine
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   pylint
     #   tox
     #   virtualenv
 pluggy==1.5.0
     # via
     #   pytest
@@ -118,15 +118,15 @@
     #   rich
 pylint==3.1.0
     # via -r requirements/dev.in
 pyproject-api==1.6.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r requirements/pytest.in
     #   pytest-xdist
 pytest-xdist==3.5.0
     # via -r requirements/pytest.in
 readme-renderer==43.0
     # via
@@ -154,15 +154,15 @@
     #   pylint
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
 tomlkit==0.12.4
     # via pylint
-tox==4.14.2
+tox==4.15.0
     # via
     #   -r requirements/tox.in
     #   tox-gh
 tox-gh==1.3.1
     # via -r requirements/tox.in
 twine==5.0.0
     # via -r requirements/dev.in
@@ -172,21 +172,21 @@
     #   pylint
     #   rich
     #   urwid
 urllib3==2.2.1
     # via
     #   requests
     #   twine
-urwid==2.6.10
+urwid==2.6.11
     # via
     #   pudb
     #   urwid-readline
 urwid-readline==0.14
     # via pudb
-virtualenv==20.25.3
+virtualenv==20.26.0
     # via
     #   -r requirements/pip.in
     #   tox
 wcwidth==0.2.13
     # via urwid
 zipp==3.18.1
     # via
```

### Comparing `coverage-7.5.0/requirements/kit.pip` & `coverage-7.5.1/requirements/kit.pip`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 importlib-metadata==7.1.0
     # via build
 packaging==24.0
     # via
     #   auditwheel
     #   build
     #   cibuildwheel
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via cibuildwheel
 pyelftools==0.31
     # via auditwheel
 pyproject-hooks==1.0.0
     # via build
 tomli==2.0.1
     # via
```

### Comparing `coverage-7.5.0/requirements/light-threads.pip` & `coverage-7.5.1/requirements/light-threads.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/requirements/mypy.pip` & `coverage-7.5.1/requirements/mypy.pip`

 * *Files 12% similar despite different names*

```diff
@@ -12,29 +12,29 @@
     # via
     #   hypothesis
     #   pytest
 execnet==2.1.1
     # via pytest-xdist
 flaky==3.8.1
     # via -r requirements/pytest.in
-hypothesis==6.100.1
+hypothesis==6.100.2
     # via -r requirements/pytest.in
 iniconfig==2.0.0
     # via pytest
-mypy==1.9.0
+mypy==1.10.0
     # via -r requirements/mypy.in
 mypy-extensions==1.0.0
     # via mypy
 packaging==24.0
     # via pytest
 pluggy==1.5.0
     # via pytest
 pygments==2.17.2
     # via -r requirements/pytest.in
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r requirements/pytest.in
     #   pytest-xdist
 pytest-xdist==3.5.0
     # via -r requirements/pytest.in
 sortedcontainers==2.4.0
     # via hypothesis
```

### Comparing `coverage-7.5.0/requirements/pip-tools.pip` & `coverage-7.5.1/requirements/pip-tools.pip`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/requirements/pytest.in` & `coverage-7.5.1/requirements/pytest.in`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/requirements/pytest.pip` & `coverage-7.5.1/requirements/pytest.pip`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     # via
     #   hypothesis
     #   pytest
 execnet==2.1.1
     # via pytest-xdist
 flaky==3.8.1
     # via -r requirements/pytest.in
-hypothesis==6.100.1
+hypothesis==6.100.2
     # via -r requirements/pytest.in
 iniconfig==2.0.0
     # via pytest
 packaging==24.0
     # via pytest
 pluggy==1.5.0
     # via pytest
 pygments==2.17.2
     # via -r requirements/pytest.in
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r requirements/pytest.in
     #   pytest-xdist
 pytest-xdist==3.5.0
     # via -r requirements/pytest.in
 sortedcontainers==2.4.0
     # via hypothesis
```

### Comparing `coverage-7.5.0/requirements/tox.pip` & `coverage-7.5.1/requirements/tox.pip`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     # via
     #   tox
     #   virtualenv
 packaging==24.0
     # via
     #   pyproject-api
     #   tox
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   tox
     #   virtualenv
 pluggy==1.5.0
     # via tox
 pyproject-api==1.6.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.14.2
+tox==4.15.0
     # via
     #   -r requirements/tox.in
     #   tox-gh
 tox-gh==1.3.1
     # via -r requirements/tox.in
-virtualenv==20.25.3
+virtualenv==20.26.0
     # via tox
```

### Comparing `coverage-7.5.0/setup.py` & `coverage-7.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/balance_xdist_plugin.py` & `coverage-7.5.1/tests/balance_xdist_plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/conftest.py` & `coverage-7.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/coveragetest.py` & `coverage-7.5.1/tests/coveragetest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/README.rst` & `coverage-7.5.1/tests/gold/README.rst`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/annotate/white/white.py,cover` & `coverage-7.5.1/tests/gold/annotate/white/white.py,cover`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/html/Makefile` & `coverage-7.5.1/tests/gold/html/Makefile`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/html/a/a_py.html` & `coverage-7.5.1/tests/gold/html/a/a_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for a.py: 67%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>a.py</b>:
             <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -89,14 +89,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 33 ssttaatteemmeennttss ?  22 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1if 1 < 2: 
 _2 # Needed a < to look at HTML entities. 
 _3 a = 3 
 _4else: 
 _5 a = 4 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/a/class_index.html` & `coverage-7.5.1/tests/gold/html/omit_5/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">67%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
-                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
@@ -45,71 +44,75 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button" href="index.html">Files</a>
+                <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="a_py.html">a.py</a></td>
-                <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>3</td>
-                <td>1</td>
+                <td class="name left"><a href="m1_py.html">m1.py</a></td>
+                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
+            </tr>
+            <tr class="region">
+                <td class="name left"><a href="main_py.html">main.py</a></td>
+                <td>8</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td class="name left">&nbsp;</td>
-                <td>3</td>
-                <td>1</td>
+                <td>10</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td class="right" data-ratio="10 10">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href=""></a>
-        <a id="nextFileLink" class="nav" href=""></a>
+        <a id="prevFileLink" class="nav" href="main_py.html"></a>
+        <a id="nextFileLink" class="nav" href="m1_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f n s m x c   change column sorting
+f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee  ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_a_._p_y  _(_n_o_ _c_l_a_s_s_) 3          1       0        67%
-Total            3          1       0        67%
+********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
+FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_1_._p_y   2          0       0        100%
+_m_a_i_n_._p_y 8          0       0        100%
+Total   10         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/a/function_index.html` & `coverage-7.5.1/tests/gold/html/a/function_index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="a_py.html">a.py</a></td>
                 <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>3</td>
@@ -95,16 +95,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
 FFiillee  ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _a_._p_y  _(_n_o_ _f_u_n_c_t_i_o_n_) 3          1       0        67%
 Total               3          1       0        67%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/a/index.html` & `coverage-7.5.1/tests/gold/html/a/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,28 +49,28 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="a_py.html">a.py</a></td>
                 <td>3</td>
                 <td>1</td>
@@ -91,16 +91,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="a_py.html"></a>
         <a id="nextFileLink" class="nav" href="a_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
 FFiillee  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _a_._p_y  3          1       0        67%
 Total 3          1       0        67%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/b_branch/b_py.html` & `coverage-7.5.1/tests/gold/html/b_branch/b_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for b.py: 70%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>b.py</b>:
             <span class="pc_cov">70%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -62,16 +62,16 @@
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">4<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 08:04 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -80,32 +80,32 @@
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">def</span> <span class="nam">one</span><span class="op">(</span><span class="nam">x</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">    <span class="com"># This will be a branch that misses the else.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">    <span class="key">if</span> <span class="nam">x</span> <span class="op">&lt;</span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">3&#x202F;&#x219B;&#x202F;6</span><span class="annotate long">line 3 didn't jump to line 6, because the condition on line 3 was never false</span></span></p>
+    <p class="par run show_par"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">    <span class="key">if</span> <span class="nam">x</span> <span class="op">&lt;</span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">3&#x202F;&#x219B;&#x202F;6</span><span class="annotate long">line 3 didn't jump to line 6, because the condition on line 3 was always true</span></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">        <span class="nam">a</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">        <span class="nam">a</span> <span class="op">=</span> <span class="num">4</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">one</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">def</span> <span class="nam">two</span><span class="op">(</span><span class="nam">x</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="com"># A missed else that branches to "exit"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">if</span> <span class="nam">x</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">12&#x202F;&#x219B;&#x202F;exit</span><span class="annotate long">line 12 didn't return from function 'two', because the condition on line 12 was never false</span></span></p>
+    <p class="par run show_par"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">if</span> <span class="nam">x</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">12&#x202F;&#x219B;&#x202F;exit</span><span class="annotate long">line 12 didn't return from function 'two', because the condition on line 12 was always true</span></span></p>
     <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="nam">a</span> <span class="op">=</span> <span class="num">5</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">two</span><span class="op">(</span><span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">def</span> <span class="nam">three</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="com"># This if has two branches, *neither* one taken.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="key">if</span> <span class="nam">name_error_this_variable_doesnt_exist</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">20&#x202F;&#x219B;&#x202F;21,&nbsp;&nbsp; 20&#x202F;&#x219B;&#x202F;23</span><span class="annotate long">2 missed branches: 1) line 20 didn't jump to line 21, because the condition on line 20 was never true, 2) line 20 didn't jump to line 23, because the condition on line 20 was never false</span></span></p>
+    <p class="par run show_par"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="key">if</span> <span class="nam">name_error_this_variable_doesnt_exist</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">20&#x202F;&#x219B;&#x202F;21,&nbsp;&nbsp; 20&#x202F;&#x219B;&#x202F;23</span><span class="annotate long">2 missed branches: 1) line 20 didn't jump to line 21, because the condition on line 20 was never true, 2) line 20 didn't jump to line 23, because the condition on line 20 was always true</span></span></p>
     <p class="mis show_mis"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">            <span class="nam">a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">            <span class="nam">a</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">except</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="nam">three</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
@@ -113,14 +113,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 08:04 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,43 +5,43 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1177 ssttaatteemmeennttss ?  1144 rruunn 33 mmiissssiinngg 00 eexxcclluuddeedd 44 ppaarrttiiaall **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-25 08:04 -0400
 _1def one(x): 
 _2 # This will be a branch that misses the else. 
 _3 if x < 2: 3 ↛ 6line 3 didn't jump to line 6, because the condition on line 3
-was never false
+was always true
 _4 a = 3 
 _5 else: 
 _6 a = 4 
 _7 
 _8one(1) 
 _9 
 _1_0def two(x): 
 _1_1 # A missed else that branches to "exit" 
 _1_2 if x: 12 ↛ exitline 12 didn't return from function 'two', because the
-condition on line 12 was never false
+condition on line 12 was always true
 _1_3 a = 5 
 _1_4 
 _1_5two(1) 
 _1_6 
 _1_7def three(): 
 _1_8 try: 
 _1_9 # This if has two branches, *neither* one taken. 
 _2_0 if name_error_this_variable_doesnt_exist: 20 ↛ 21,   20 ↛ 232 missed
 branches: 1) line 20 didn't jump to line 21, because the condition on line 20
 was never true, 2) line 20 didn't jump to line 23, because the condition on
-line 20 was never false
+line 20 was always true
 _2_1 a = 1 
 _2_2 else: 
 _2_3 a = 2 
 _2_4 except: 
 _2_5 pass 
 _2_6 
 _2_7three() 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-25 08:04 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/b_branch/class_index.html` & `coverage-7.5.1/tests/gold/html/b_branch/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">70%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
-                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>b</kbd>
                         <kbd>p</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
@@ -47,77 +46,74 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button" href="index.html">Files</a>
+                <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="b_py.html">b.py</a></td>
-                <td class="name left"><a href="b_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>6</td>
-                <td>0</td>
-                <td>0</td>
+                <td>17</td>
+                <td>3</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="6 6">100%</td>
+                <td>6</td>
+                <td>4</td>
+                <td class="right" data-ratio="16 23">70%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td class="name left">&nbsp;</td>
-                <td>6</td>
-                <td>0</td>
-                <td>0</td>
+                <td>17</td>
+                <td>3</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="6 6">100%</td>
+                <td>6</td>
+                <td>4</td>
+                <td class="right" data-ratio="16 23">70%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href=""></a>
-        <a id="nextFileLink" class="nav" href=""></a>
+        <a id="prevFileLink" class="nav" href="b_py.html"></a>
+        <a id="nextFileLink" class="nav" href="b_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 7700%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f n s m x b p c   change column sorting
+f s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee  ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
-_b_._p_y  _(_n_o_ _c_l_a_s_s_) 6          0       0        0        0       100%
-Total            6          0       0        0        0       100%
+********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
+FFiillee  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
+_b_._p_y  17         3       0        6        4       70%
+Total 17         3       0        6        4       70%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/b_branch/function_index.html` & `coverage-7.5.1/tests/gold/html/b_branch/function_index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">70%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -52,31 +52,31 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="b_py.html#t1">b.py</a></td>
                 <td class="name left"><a href="b_py.html#t1"><data value='one'>one</data></a></td>
                 <td>3</td>
@@ -133,16 +133,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,16 +3,16 @@
 Shortcuts on this page
 f n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
 FFiillee  ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
 _b_._p_y  _o_n_e           3          1       0        2        1       60%
 _b_._p_y  _t_w_o           2          0       0        2        1       75%
 _b_._p_y  _t_h_r_e_e         6          2       0        2        2       50%
 _b_._p_y  _(_n_o_ _f_u_n_c_t_i_o_n_) 6          0       0        0        0       100%
 Total               17         3       0        6        4       70%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/b_branch/index.html` & `coverage-7.5.1/tests/gold/html/omit_1/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">70%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
-                        <kbd>b</kbd>
-                        <kbd>p</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
                         <kbd>[</kbd>
                         <kbd>]</kbd>
                         &nbsp; prev/next file
@@ -51,69 +49,84 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="b_py.html">b.py</a></td>
-                <td>17</td>
-                <td>3</td>
-                <td>0</td>
-                <td>6</td>
-                <td>4</td>
-                <td class="right" data-ratio="16 23">70%</td>
+                <td class="name left"><a href="m1_py.html">m1.py</a></td>
+                <td>2</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
+            </tr>
+            <tr class="region">
+                <td class="name left"><a href="m2_py.html">m2.py</a></td>
+                <td>2</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
+            </tr>
+            <tr class="region">
+                <td class="name left"><a href="m3_py.html">m3.py</a></td>
+                <td>2</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
+            </tr>
+            <tr class="region">
+                <td class="name left"><a href="main_py.html">main.py</a></td>
+                <td>8</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>17</td>
-                <td>3</td>
+                <td>14</td>
+                <td>0</td>
                 <td>0</td>
-                <td>6</td>
-                <td>4</td>
-                <td class="right" data-ratio="16 23">70%</td>
+                <td class="right" data-ratio="14 14">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="b_py.html"></a>
-        <a id="nextFileLink" class="nav" href="b_py.html"></a>
+        <a id="prevFileLink" class="nav" href="main_py.html"></a>
+        <a id="nextFileLink" class="nav" href="m1_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
-************ CCoovveerraaggee rreeppoorrtt:: 7700%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x b p c   change column sorting
+f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
-_b_._p_y  17         3       0        6        4       70%
-Total 17         3       0        6        4       70%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
+FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_1_._p_y   2          0       0        100%
+_m_2_._p_y   2          0       0        100%
+_m_3_._p_y   2          0       0        100%
+_m_a_i_n_._p_y 8          0       0        100%
+Total   14         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/bom/bom_py.html` & `coverage-7.5.1/tests/gold/html/bom/bom_py.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for bom.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>bom.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -89,14 +89,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 33 ssttaatteemmeennttss ?  33 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1# A Python source file in utf-8, with BOM. 
 _2math = "3×4 = 12, ÷2 = 6±0" 
 _3 
 _4assert len(math) == 18 
 _5assert len(math.encode('utf-8')) == 21 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/bom/class_index.html` & `coverage-7.5.1/tests/gold/html/a/class_index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,61 +50,61 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="bom_py.html">bom.py</a></td>
-                <td class="name left"><a href="bom_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td class="name left"><a href="a_py.html">a.py</a></td>
+                <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="3 3">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
                 <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="3 3">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee   ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_b_o_m_._p_y _(_n_o_ _c_l_a_s_s_) 3          0       0        100%
-Total             3          0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
+FFiillee  ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_a_._p_y  _(_n_o_ _c_l_a_s_s_) 3          1       0        67%
+Total            3          1       0        67%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/bom/function_index.html` & `coverage-7.5.1/tests/gold/html/styled/function_index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+        <link rel="stylesheet" href="myextra_cb_232e8e19.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,61 +51,61 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="bom_py.html">bom.py</a></td>
-                <td class="name left"><a href="bom_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td class="name left"><a href="a_py.html">a.py</a></td>
+                <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="3 3">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
                 <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="3 3">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee   ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_b_o_m_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 3          0       0        100%
-Total                3          0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee  ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_a_._p_y  _(_n_o_ _f_u_n_c_t_i_o_n_) 3          1       0        67%
+Total               3          1       0        67%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/bom/index.html` & `coverage-7.5.1/tests/gold/html/isolatin1/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,63 +49,63 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="bom_py.html">bom.py</a></td>
-                <td>3</td>
+                <td class="name left"><a href="isolatin1_py.html">isolatin1.py</a></td>
+                <td>2</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="3 3">100%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>3</td>
+                <td>2</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="3 3">100%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="bom_py.html"></a>
-        <a id="nextFileLink" class="nav" href="bom_py.html"></a>
+        <a id="prevFileLink" class="nav" href="isolatin1_py.html"></a>
+        <a id="nextFileLink" class="nav" href="isolatin1_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee   ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_b_o_m_._p_y 3          0       0        100%
-Total  3          0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
+FFiillee         ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_i_s_o_l_a_t_i_n_1_._p_y 2          0       0        100%
+Total        2          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/contexts/class_index.html` & `coverage-7.5.1/tests/gold/html/styled/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+        <link rel="stylesheet" href="myextra_cb_232e8e19.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
-                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
@@ -45,71 +45,68 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button" href="index.html">Files</a>
+                <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="two_tests_py.html">two_tests.py</a></td>
-                <td class="name left"><a href="two_tests_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>7</td>
+                <td class="name left"><a href="a_py.html">a.py</a></td>
+                <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="7 7">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td class="name left">&nbsp;</td>
-                <td>7</td>
-                <td>0</td>
+                <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="7 7">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href=""></a>
-        <a id="nextFileLink" class="nav" href=""></a>
+        <a id="prevFileLink" class="nav" href="a_py.html"></a>
+        <a id="nextFileLink" class="nav" href="a_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f n s m x c   change column sorting
+f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee         ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_t_w_o___t_e_s_t_s_._p_y _(_n_o_ _c_l_a_s_s_) 7          0       0        100%
-Total                   7          0       0        100%
+********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
+FFiillee  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_a_._p_y  3          1       0        67%
+Total 3          1       0        67%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/contexts/function_index.html` & `coverage-7.5.1/tests/gold/html/contexts/function_index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">94%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="two_tests_py.html#t1">two_tests.py</a></td>
                 <td class="name left"><a href="two_tests_py.html#t1"><data value='helper'>helper</data></a></td>
                 <td>1</td>
@@ -119,16 +119,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,16 +3,16 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee         ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _t_w_o___t_e_s_t_s_._p_y _h_e_l_p_e_r        1          0       0        100%
 _t_w_o___t_e_s_t_s_._p_y _t_e_s_t___o_n_e      2          0       0        100%
 _t_w_o___t_e_s_t_s_._p_y _t_e_s_t___t_w_o      7          1       0        86%
 _t_w_o___t_e_s_t_s_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 7          0       0        100%
 Total                      17         1       0        94%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/contexts/index.html` & `coverage-7.5.1/tests/gold/html/unicode/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">94%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,63 +49,63 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="two_tests_py.html">two_tests.py</a></td>
-                <td>17</td>
-                <td>1</td>
+                <td class="name left"><a href="unicode_py.html">unicode.py</a></td>
+                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="16 17">94%</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>17</td>
-                <td>1</td>
+                <td>2</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="16 17">94%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="two_tests_py.html"></a>
-        <a id="nextFileLink" class="nav" href="two_tests_py.html"></a>
+        <a id="prevFileLink" class="nav" href="unicode_py.html"></a>
+        <a id="nextFileLink" class="nav" href="unicode_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 9944%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee         ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_t_w_o___t_e_s_t_s_._p_y 17         1       0        94%
-Total        17         1       0        94%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
+FFiillee       ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_u_n_i_c_o_d_e_._p_y 2          0       0        100%
+Total      2          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/contexts/two_tests_py.html` & `coverage-7.5.1/tests/gold/html/contexts/two_tests_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for two_tests.py: 94%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
     <script type="text/javascript">
         contexts = {
   "a": "(empty)",
   "b": "two_tests.test_two",
   "c": "two_tests.test_one"
 }
     </script>
-    <script src="coverage_html.js" defer></script>
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>two_tests.py</b>:
             <span class="pc_cov">94%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -67,16 +67,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -113,14 +113,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1177 ssttaatteemmeennttss ?  1166 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1def helper(lineno): (empty)
 _2 x = 2 ??3 ctx1acb
 _3 
 _4def test_one(): (empty)
 _5 a = 5 ??1 ctx1c
 _6 helper(6) ??1 ctx1c
 _7 
@@ -29,9 +29,9 @@
 _1_6 16 
 _1_7 ) 
 _1_8 
 _1_9test_one() (empty)
 _2_0x = 20 (empty)
 _2_1helper(21) (empty)
 _2_2test_two() (empty)
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/isolatin1/class_index.html` & `coverage-7.5.1/tests/gold/html/contexts/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">94%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
-                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
@@ -45,71 +44,68 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button" href="index.html">Files</a>
+                <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="isolatin1_py.html">isolatin1.py</a></td>
-                <td class="name left"><a href="isolatin1_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>2</td>
+                <td class="name left"><a href="two_tests_py.html">two_tests.py</a></td>
+                <td>17</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="16 17">94%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td class="name left">&nbsp;</td>
-                <td>2</td>
-                <td>0</td>
+                <td>17</td>
+                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="16 17">94%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href=""></a>
-        <a id="nextFileLink" class="nav" href=""></a>
+        <a id="prevFileLink" class="nav" href="two_tests_py.html"></a>
+        <a id="nextFileLink" class="nav" href="two_tests_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 9944%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f n s m x c   change column sorting
+f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee         ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_i_s_o_l_a_t_i_n_1_._p_y _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
-Total                   2          0       0        100%
+********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
+FFiillee         ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_t_w_o___t_e_s_t_s_._p_y 17         1       0        94%
+Total        17         1       0        94%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/isolatin1/function_index.html` & `coverage-7.5.1/tests/gold/html/isolatin1/class_index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -46,39 +46,39 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button current">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button" href="function_index.html">Functions</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="isolatin1_py.html">isolatin1.py</a></td>
-                <td class="name left"><a href="isolatin1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td class="name left"><a href="isolatin1_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tbody>
         <tfoot>
@@ -95,16 +95,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -2,14 +2,14 @@
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee         ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_i_s_o_l_a_t_i_n_1_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
-Total                      2          0       0        100%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
+FFiillee         ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_i_s_o_l_a_t_i_n_1_._p_y _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
+Total                   2          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/isolatin1/index.html` & `coverage-7.5.1/tests/gold/html/partial/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">91%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
+                        <kbd>b</kbd>
+                        <kbd>p</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
                         <kbd>[</kbd>
                         <kbd>]</kbd>
                         &nbsp; prev/next file
@@ -49,63 +51,69 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-29 17:40 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="isolatin1_py.html">isolatin1.py</a></td>
-                <td>2</td>
+                <td class="name left"><a href="partial_py.html">partial.py</a></td>
+                <td>7</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td>1</td>
+                <td>4</td>
+                <td>1</td>
+                <td class="right" data-ratio="10 11">91%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>2</td>
-                <td>0</td>
+                <td>7</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td>1</td>
+                <td>4</td>
+                <td>1</td>
+                <td class="right" data-ratio="10 11">91%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-29 17:40 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="isolatin1_py.html"></a>
-        <a id="nextFileLink" class="nav" href="isolatin1_py.html"></a>
+        <a id="prevFileLink" class="nav" href="partial_py.html"></a>
+        <a id="nextFileLink" class="nav" href="partial_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 9911%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x c   change column sorting
+f s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee         ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_i_s_o_l_a_t_i_n_1_._p_y 2          0       0        100%
-Total        2          0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-29 17:40 -0300
+FFiillee       ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
+_p_a_r_t_i_a_l_._p_y 7          0       1        4        1       91%
+Total      7          0       1        4        1       91%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-29 17:40 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/isolatin1/isolatin1_py.html` & `coverage-7.5.1/tests/gold/html/isolatin1/isolatin1_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for isolatin1.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>isolatin1.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -89,14 +89,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1# -*- coding: iso8859-1 -*- 
 _2# A Python source file in another encoding. 
 _3 
 _4math = "3×4 = 12, ÷2 = 6±0" 
 _5assert len(math) == 18 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/class_index.html` & `coverage-7.5.1/tests/gold/html/omit_1/class_index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m1_py.html">m1.py</a></td>
                 <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>2</td>
@@ -119,16 +119,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,16 +3,16 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_1_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_2_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_3_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _c_l_a_s_s_) 8          0       0        100%
 Total              14         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/function_index.html` & `coverage-7.5.1/tests/gold/html/omit_1/function_index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m1_py.html">m1.py</a></td>
                 <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>2</td>
@@ -119,16 +119,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,16 +3,16 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_1_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_2_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_3_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
 Total                 14         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/index.html` & `coverage-7.5.1/tests/gold/html/omit_4/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,46 +49,39 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m1_py.html">m1.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="m2_py.html">m2.py</a></td>
-                <td>2</td>
-                <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
-            </tr>
-            <tr class="region">
                 <td class="name left"><a href="m3_py.html">m3.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
@@ -98,30 +91,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>14</td>
+                <td>12</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="14 14">100%</td>
+                <td class="right" data-ratio="12 12">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="main_py.html"></a>
         <a id="nextFileLink" class="nav" href="m1_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,16 +3,15 @@
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
 FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_1_._p_y   2          0       0        100%
-_m_2_._p_y   2          0       0        100%
 _m_3_._p_y   2          0       0        100%
 _m_a_i_n_._p_y 8          0       0        100%
-Total   14         0       0        100%
+Total   12         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/m1_py.html` & `coverage-7.5.1/tests/gold/html/omit_2/m2_py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for m1.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <title>Coverage for m2.py: 100%</title>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>m1.py</b>:
+            <span class="text">Coverage for </span><b>m2.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -58,42 +58,42 @@
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="m2_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="m3_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
             <button type="button" class="button_next_file" data-shortcut="]"></button>
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m1a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m1b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m2a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m2b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="m2_py.html">&#xbb; next</a>
+            <a class="nav" href="m3_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-************ CCoovveerraaggee ffoorr mm11..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr mm22..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
-_1m1a = 1 
-_2m1b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
+_1m2a = 1 
+_2m2b = 2 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/m2_py.html` & `coverage-7.5.1/tests/gold/html/omit_5/m1_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for m2.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <title>Coverage for m1.py: 100%</title>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>m2.py</b>:
+            <span class="text">Coverage for </span><b>m1.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,44 +56,44 @@
         <h2>
             <span class="text">2 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="m3_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
             <button type="button" class="button_next_file" data-shortcut="]"></button>
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m2a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m2b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m1a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m1b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="m3_py.html">&#xbb; next</a>
+            <a class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-************ CCoovveerraaggee ffoorr mm22..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr mm11..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
-_1m2a = 1 
-_2m2b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
+_1m1a = 1 
+_2m1b = 2 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/m3_py.html` & `coverage-7.5.1/tests/gold/html/omit_4/m3_py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for m3.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>m3.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">2 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="m2_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -82,18 +82,18 @@
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m3a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m3b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="m2_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1m3a = 1 
 _2m3b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_1/main_py.html` & `coverage-7.5.1/tests/gold/html/omit_5/main_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for main.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>main.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">8 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">8<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -90,18 +90,18 @@
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">assert</span> <span class="nam">m1</span><span class="op">.</span><span class="nam">m1a</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">assert</span> <span class="nam">m2</span><span class="op">.</span><span class="nam">m2a</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">assert</span> <span class="nam">m3</span><span class="op">.</span><span class="nam">m3a</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,21 +5,21 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1import m1 
 _2import m2 
 _3import m3 
 _4 
 _5a = 5 
 _6b = 6 
 _7 
 _8assert m1.m1a == 1 
 _9assert m2.m2a == 1 
 _1_0assert m3.m3a == 1 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_2/class_index.html` & `coverage-7.5.1/tests/gold/html/omit_2/class_index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m2_py.html">m2.py</a></td>
                 <td class="name left"><a href="m2_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>2</td>
@@ -111,16 +111,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_2_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_3_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _c_l_a_s_s_) 8          0       0        100%
 Total              12         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_2/function_index.html` & `coverage-7.5.1/tests/gold/html/omit_2/function_index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m2_py.html">m2.py</a></td>
                 <td class="name left"><a href="m2_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>2</td>
@@ -111,16 +111,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_2_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_3_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
 Total                 12         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_2/index.html` & `coverage-7.5.1/tests/gold/html/other/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">80%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,77 +49,70 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:17 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="m2_py.html">m2.py</a></td>
-                <td>2</td>
+                <td class="name left"><a href="z_0730f1441bcc04fe_other_py.html">C:\Users\ddini\AppData\Local\Temp\pytest-of-ddini\pytest-9\popen-gw6\t1\othersrc\other.py</a></td>
+                <td>1</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="m3_py.html">m3.py</a></td>
-                <td>2</td>
+                <td class="name left"><a href="here_py.html">here.py</a></td>
+                <td>4</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
-            </tr>
-            <tr class="region">
-                <td class="name left"><a href="main_py.html">main.py</a></td>
-                <td>8</td>
-                <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="8 8">100%</td>
+                <td class="right" data-ratio="3 4">75%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>12</td>
-                <td>0</td>
+                <td>5</td>
+                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="12 12">100%</td>
+                <td class="right" data-ratio="4 5">80%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:17 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="main_py.html"></a>
-        <a id="nextFileLink" class="nav" href="m2_py.html"></a>
+        <a id="prevFileLink" class="nav" href="here_py.html"></a>
+        <a id="nextFileLink" class="nav" href="z_0730f1441bcc04fe_other_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_m_2_._p_y   2          0       0        100%
-_m_3_._p_y   2          0       0        100%
-_m_a_i_n_._p_y 8          0       0        100%
-Total   12         0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:17 -0300
+FFiillee                                      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_C_:_\_U_s_e_r_s_\_d_d_i_n_i_\_A_p_p_D_a_t_a_\_L_o_c_a_l_\_T_e_m_p_\_p_y_t_e_s_t_-
+_o_f_-_d_d_i_n_i_\_p_y_t_e_s_t_-_9_\_p_o_p_e_n_-                  1          0       0        100%
+_g_w_6_\_t_1_\_o_t_h_e_r_s_r_c_\_o_t_h_e_r_._p_y
+_h_e_r_e_._p_y                                   4          1       0        75%
+Total                                     5          1       0        80%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:17 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_2/m2_py.html` & `coverage-7.5.1/tests/gold/html/omit_1/m2_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for m2.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>m2.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">2 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="m3_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -82,18 +82,18 @@
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m2a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m2b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="m3_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1m2a = 1 
 _2m2b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_2/m3_py.html` & `coverage-7.5.1/tests/gold/html/omit_1/m3_py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for m3.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>m3.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="m2_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -86,14 +86,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="m2_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1m3a = 1 
 _2m3b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_2/main_py.html` & `coverage-7.5.1/tests/gold/html/omit_1/main_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for main.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>main.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -94,14 +94,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,21 +5,21 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1import m1 
 _2import m2 
 _3import m3 
 _4 
 _5a = 5 
 _6b = 6 
 _7 
 _8assert m1.m1a == 1 
 _9assert m2.m2a == 1 
 _1_0assert m3.m3a == 1 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_3/class_index.html` & `coverage-7.5.1/tests/gold/html/omit_3/class_index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m3_py.html">m3.py</a></td>
                 <td class="name left"><a href="m3_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>2</td>
@@ -103,16 +103,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,14 +3,14 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_3_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _c_l_a_s_s_) 8          0       0        100%
 Total              10         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_3/function_index.html` & `coverage-7.5.1/tests/gold/html/omit_4/function_index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,33 +50,41 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
+                <td class="name left"><a href="m1_py.html">m1.py</a></td>
+                <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>2</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
+            </tr>
+            <tr class="region">
                 <td class="name left"><a href="m3_py.html">m3.py</a></td>
                 <td class="name left"><a href="m3_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
@@ -89,30 +97,30 @@
                 <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>10</td>
+                <td>12</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="10 10">100%</td>
+                <td class="right" data-ratio="12 12">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_1_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_3_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
-Total                 10         0       0        100%
+Total                 12         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_3/index.html` & `coverage-7.5.1/tests/gold/html/omit_2/index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,32 +49,39 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
+                <td class="name left"><a href="m2_py.html">m2.py</a></td>
+                <td>2</td>
+                <td>0</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
+            </tr>
+            <tr class="region">
                 <td class="name left"><a href="m3_py.html">m3.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
@@ -84,35 +91,35 @@
                 <td>0</td>
                 <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>10</td>
+                <td>12</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="10 10">100%</td>
+                <td class="right" data-ratio="12 12">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="main_py.html"></a>
-        <a id="nextFileLink" class="nav" href="m3_py.html"></a>
+        <a id="nextFileLink" class="nav" href="m2_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
 FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_2_._p_y   2          0       0        100%
 _m_3_._p_y   2          0       0        100%
 _m_a_i_n_._p_y 8          0       0        100%
-Total   10         0       0        100%
+Total   12         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_3/m3_py.html` & `coverage-7.5.1/tests/gold/html/omit_3/m3_py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for m3.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>m3.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -86,14 +86,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1m3a = 1 
 _2m3b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_3/main_py.html` & `coverage-7.5.1/tests/gold/html/omit_2/main_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for main.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>main.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -94,14 +94,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,21 +5,21 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1import m1 
 _2import m2 
 _3import m3 
 _4 
 _5a = 5 
 _6b = 6 
 _7 
 _8assert m1.m1a == 1 
 _9assert m2.m2a == 1 
 _1_0assert m3.m3a == 1 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_4/class_index.html` & `coverage-7.5.1/tests/gold/html/omit_4/class_index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,29 +50,29 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m1_py.html">m1.py</a></td>
                 <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>2</td>
@@ -111,16 +111,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
 FFiillee    ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _m_1_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_3_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
 _m_a_i_n_._p_y _(_n_o_ _c_l_a_s_s_) 8          0       0        100%
 Total              12         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_4/function_index.html` & `coverage-7.5.1/tests/gold/html/omit_5/class_index.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -46,81 +46,73 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button current">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button" href="function_index.html">Functions</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="m1_py.html">m1.py</a></td>
-                <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>2</td>
-                <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
-            </tr>
-            <tr class="region">
-                <td class="name left"><a href="m3_py.html">m3.py</a></td>
-                <td class="name left"><a href="m3_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="main_py.html">main.py</a></td>
-                <td class="name left"><a href="main_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td class="name left"><a href="main_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>8</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>12</td>
+                <td>10</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="12 12">100%</td>
+                <td class="right" data-ratio="10 10">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -2,16 +2,15 @@
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_m_1_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
-_m_3_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
-_m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
-Total                 12         0       0        100%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee    ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_1_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
+_m_a_i_n_._p_y _(_n_o_ _c_l_a_s_s_) 8          0       0        100%
+Total              10         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_4/index.html` & `coverage-7.5.1/tests/gold/html/other/class_index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">80%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
+                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
@@ -44,82 +45,79 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button current">Files</a>
+                <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:17 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="m1_py.html">m1.py</a></td>
-                <td>2</td>
+                <td class="name left"><a href="z_0730f1441bcc04fe_other_py.html">C:\Users\ddini\AppData\Local\Temp\pytest-of-ddini\pytest-9\popen-gw6\t1\othersrc\other.py</a></td>
+                <td class="name left"><a href="z_0730f1441bcc04fe_other_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>1</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="m3_py.html">m3.py</a></td>
-                <td>2</td>
+                <td class="name left"><a href="here_py.html">here.py</a></td>
+                <td class="name left"><a href="here_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>4</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
-            </tr>
-            <tr class="region">
-                <td class="name left"><a href="main_py.html">main.py</a></td>
-                <td>8</td>
-                <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="8 8">100%</td>
+                <td class="right" data-ratio="3 4">75%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>12</td>
-                <td>0</td>
+                <td class="name left">&nbsp;</td>
+                <td>5</td>
+                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="12 12">100%</td>
+                <td class="right" data-ratio="4 5">80%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:17 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="main_py.html"></a>
-        <a id="nextFileLink" class="nav" href="m1_py.html"></a>
+        <a id="prevFileLink" class="nav" href=""></a>
+        <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x c   change column sorting
+f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_m_1_._p_y   2          0       0        100%
-_m_3_._p_y   2          0       0        100%
-_m_a_i_n_._p_y 8          0       0        100%
-Total   12         0       0        100%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:17 -0300
+FFiillee                                    ccllaassss  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_C_:
+_\_U_s_e_r_s_\_d_d_i_n_i_\_A_p_p_D_a_t_a_\_L_o_c_a_l_\_T_e_m_p_\_p_y_t_e_s_t_- _(_n_o    1          0       0        100%
+_o_f_-_d_d_i_n_i_\_p_y_t_e_s_t_-_9_\_p_o_p_e_n_-                _c_l_a_s_s_)
+_g_w_6_\_t_1_\_o_t_h_e_r_s_r_c_\_o_t_h_e_r_._p_y
+_h_e_r_e_._p_y                                 _(_n_o    4          1       0        75%
+                                        _c_l_a_s_s_)
+Total                                          5          1       0        80%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:17 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_4/m1_py.html` & `coverage-7.5.1/tests/gold/html/omit_2/m3_py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for m1.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <title>Coverage for m3.py: 100%</title>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>m1.py</b>:
+            <span class="text">Coverage for </span><b>m3.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,44 +56,44 @@
         <h2>
             <span class="text">2 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="m2_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="m3_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
             <button type="button" class="button_next_file" data-shortcut="]"></button>
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m1a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m1b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m3a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m3b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="m2_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="m3_py.html">&#xbb; next</a>
+            <a class="nav" href="main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-************ CCoovveerraaggee ffoorr mm11..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr mm33..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
-_1m1a = 1 
-_2m1b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
+_1m3a = 1 
+_2m3b = 2 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_4/m3_py.html` & `coverage-7.5.1/tests/gold/html/omit_1/m1_py.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for m3.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <title>Coverage for m1.py: 100%</title>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>m3.py</b>:
+            <span class="text">Coverage for </span><b>m1.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,44 +56,44 @@
         <h2>
             <span class="text">2 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="m2_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
             <button type="button" class="button_next_file" data-shortcut="]"></button>
             <button type="button" class="button_to_index" data-shortcut="u"></button>
             <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m3a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m3b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="nam">m1a</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m1b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="main_py.html">&#xbb; next</a>
+            <a class="nav" href="m2_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-************ CCoovveerraaggee ffoorr mm33..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr mm11..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
-_1m3a = 1 
-_2m3b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
+_1m1a = 1 
+_2m1b = 2 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_4/main_py.html` & `coverage-7.5.1/tests/gold/html/omit_3/main_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for main.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>main.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -94,14 +94,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,21 +5,21 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1import m1 
 _2import m2 
 _3import m3 
 _4 
 _5a = 5 
 _6b = 6 
 _7 
 _8assert m1.m1a == 1 
 _9assert m2.m2a == 1 
 _1_0assert m3.m3a == 1 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_5/class_index.html` & `coverage-7.5.1/tests/gold/html/styled/class_index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+        <link rel="stylesheet" href="myextra_cb_232e8e19.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,69 +51,61 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="m1_py.html">m1.py</a></td>
-                <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>2</td>
+                <td class="name left"><a href="a_py.html">a.py</a></td>
+                <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
-            </tr>
-            <tr class="region">
-                <td class="name left"><a href="main_py.html">main.py</a></td>
-                <td class="name left"><a href="main_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>8</td>
-                <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="8 8">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>10</td>
-                <td>0</td>
+                <td>3</td>
+                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="10 10">100%</td>
+                <td class="right" data-ratio="2 3">67%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee    ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_m_1_._p_y   _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
-_m_a_i_n_._p_y _(_n_o_ _c_l_a_s_s_) 8          0       0        100%
-Total              10         0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee  ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_a_._p_y  _(_n_o_ _c_l_a_s_s_) 3          1       0        67%
+Total            3          1       0        67%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_5/function_index.html` & `coverage-7.5.1/tests/gold/html/other/function_index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">80%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,69 +50,69 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:17 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="m1_py.html">m1.py</a></td>
-                <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>2</td>
+                <td class="name left"><a href="z_0730f1441bcc04fe_other_py.html">C:\Users\ddini\AppData\Local\Temp\pytest-of-ddini\pytest-9\popen-gw6\t1\othersrc\other.py</a></td>
+                <td class="name left"><a href="z_0730f1441bcc04fe_other_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>1</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="main_py.html">main.py</a></td>
-                <td class="name left"><a href="main_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>8</td>
+                <td class="name left"><a href="here_py.html">here.py</a></td>
+                <td class="name left"><a href="here_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>4</td>
+                <td>1</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="8 8">100%</td>
+                <td class="right" data-ratio="3 4">75%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>10</td>
-                <td>0</td>
+                <td>5</td>
+                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="10 10">100%</td>
+                <td class="right" data-ratio="4 5">80%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:17 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,16 +1,20 @@
-************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_m_1_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
-_m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
-Total                 10         0       0        100%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:17 -0300
+FFiillee                                    ffuunnccttiioonn  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_C_:
+_\_U_s_e_r_s_\_d_d_i_n_i_\_A_p_p_D_a_t_a_\_L_o_c_a_l_\_T_e_m_p_\_p_y_t_e_s_t_- _(_n_o       1          0       0        100%
+_o_f_-_d_d_i_n_i_\_p_y_t_e_s_t_-_9_\_p_o_p_e_n_-                _f_u_n_c_t_i_o_n_)
+_g_w_6_\_t_1_\_o_t_h_e_r_s_r_c_\_o_t_h_e_r_._p_y
+_h_e_r_e_._p_y                                 _(_n_o       4          1       0        75%
+                                        _f_u_n_c_t_i_o_n_)
+Total                                             5          1       0        80%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:17 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_5/index.html` & `coverage-7.5.1/tests/gold/html/omit_3/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -49,33 +49,33 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="m1_py.html">m1.py</a></td>
+                <td class="name left"><a href="m3_py.html">m3.py</a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
                 <td class="name left"><a href="main_py.html">main.py</a></td>
@@ -98,21 +98,21 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="main_py.html"></a>
-        <a id="nextFileLink" class="nav" href="m1_py.html"></a>
+        <a id="nextFileLink" class="nav" href="m3_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -3,14 +3,14 @@
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
 FFiillee    ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_m_1_._p_y   2          0       0        100%
+_m_3_._p_y   2          0       0        100%
 _m_a_i_n_._p_y 8          0       0        100%
 Total   10         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_5/m1_py.html` & `coverage-7.5.1/tests/gold/html/omit_4/m1_py.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for m1.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>m1.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -58,18 +58,18 @@
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">2<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="main_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="m3_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -84,16 +84,16 @@
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">m1b</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="main_py.html">&#xbb; next</a>
+            <a class="nav" href="m3_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1m1a = 1 
 _2m1b = 2 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/omit_5/main_py.html` & `coverage-7.5.1/tests/gold/html/omit_4/main_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for main.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>main.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">8 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">8<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -90,18 +90,18 @@
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">assert</span> <span class="nam">m1</span><span class="op">.</span><span class="nam">m1a</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">assert</span> <span class="nam">m2</span><span class="op">.</span><span class="nam">m2a</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">assert</span> <span class="nam">m3</span><span class="op">.</span><span class="nam">m3a</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="m1_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="m3_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,21 +5,21 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1import m1 
 _2import m2 
 _3import m3 
 _4 
 _5a = 5 
 _6b = 6 
 _7 
 _8assert m1.m1a == 1 
 _9assert m2.m2a == 1 
 _1_0assert m3.m3a == 1 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/other/blah_blah_other_py.html` & `coverage-7.5.1/tests/gold/html/other/blah_blah_other_py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for /private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-259/popen-gw0/t75/othersrc/other.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <title>Coverage for /private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-293/t40/othersrc/other.py: 100%</title>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_03907183.png">
+    <link rel="stylesheet" href="style_cb_03907183.css" type="text/css">
+    <script src="coverage_html_cb_03907183.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>/private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-259/popen-gw0/t75/othersrc/other.py</b>:
+            <span class="text">Coverage for </span><b>/private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-293/t40/othersrc/other.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_03907183.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="here_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 08:10 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -88,14 +88,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="here_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 08:10 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 ************ CCoovveerraaggee ffoorr //pprriivvaattee//vvaarr//ffoollddeerrss//66jj//kkhhnn00mmccrrjj3355dd11kk33yyyyllppll88zzll008800000000ggnn//TT//
-ppyytteesstt--ooff--nneedd//ppyytteesstt--225599//ppooppeenn--ggww00//tt7755//ootthheerrssrrcc//ootthheerr..ppyy:: 110000%% ************
+ppyytteesstt--ooff--nneedd//ppyytteesstt--229933//tt4400//ootthheerrssrrcc//ootthheerr..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  11 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 08:10 -0400
 _1# A file in another directory. We're checking that it ends up in the 
 _2# HTML report. 
 _3 
 _4print("This is the other src!") 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 08:10 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/other/class_index.html` & `coverage-7.5.1/tests/gold/html/omit_5/function_index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">80%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -46,73 +46,73 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button current">Functions</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="z_a11f93934cf4431e_other_py.html">/private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-259/popen-gw0/t75/othersrc/other.py</a></td>
-                <td class="name left"><a href="z_a11f93934cf4431e_other_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>1</td>
+                <td class="name left"><a href="m1_py.html">m1.py</a></td>
+                <td class="name left"><a href="m1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>2</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="1 1">100%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="here_py.html">here.py</a></td>
-                <td class="name left"><a href="here_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>4</td>
-                <td>1</td>
+                <td class="name left"><a href="main_py.html">main.py</a></td>
+                <td class="name left"><a href="main_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>8</td>
                 <td>0</td>
-                <td class="right" data-ratio="3 4">75%</td>
+                <td>0</td>
+                <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>5</td>
-                <td>1</td>
+                <td>10</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="4 5">80%</td>
+                <td class="right" data-ratio="10 10">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,19 +1,16 @@
-************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee                            ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_/_p_r_i_v_a_t_e_/_v_a_r_/_f_o_l_d_e_r_s_/_6_j_/
-_k_h_n_0_m_c_r_j_3_5_d_1_k_3_y_y_l_p_l_8_z_l_0_8_0_0_0_0_g_n_/ _(_n_o_ _c_l_a_s_s_) 1          0       0        100%
-_T_/_p_y_t_e_s_t_-_o_f_-_n_e_d_/_p_y_t_e_s_t_-_2_5_9_/
-_p_o_p_e_n_-_g_w_0_/_t_7_5_/_o_t_h_e_r_s_r_c_/_o_t_h_e_r_._p_y
-_h_e_r_e_._p_y                         _(_n_o_ _c_l_a_s_s_) 4          1       0        75%
-Total                                      5          1       0        80%
+********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_1_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
+_m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
+Total                 10         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/other/function_index.html` & `coverage-7.5.1/tests/gold/html/omit_3/function_index.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">80%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -50,69 +50,69 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="z_a11f93934cf4431e_other_py.html">/private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-259/popen-gw0/t75/othersrc/other.py</a></td>
-                <td class="name left"><a href="z_a11f93934cf4431e_other_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>1</td>
+                <td class="name left"><a href="m3_py.html">m3.py</a></td>
+                <td class="name left"><a href="m3_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>2</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="1 1">100%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="region">
-                <td class="name left"><a href="here_py.html">here.py</a></td>
-                <td class="name left"><a href="here_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>4</td>
-                <td>1</td>
+                <td class="name left"><a href="main_py.html">main.py</a></td>
+                <td class="name left"><a href="main_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>8</td>
                 <td>0</td>
-                <td class="right" data-ratio="3 4">75%</td>
+                <td>0</td>
+                <td class="right" data-ratio="8 8">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>5</td>
-                <td>1</td>
+                <td>10</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="4 5">80%</td>
+                <td class="right" data-ratio="10 10">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,20 +1,16 @@
-************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee                            ffuunnccttiioonn  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_/_p_r_i_v_a_t_e_/_v_a_r_/_f_o_l_d_e_r_s_/_6_j_/
-_k_h_n_0_m_c_r_j_3_5_d_1_k_3_y_y_l_p_l_8_z_l_0_8_0_0_0_0_g_n_/ _(_n_o       1          0       0        100%
-_T_/_p_y_t_e_s_t_-_o_f_-_n_e_d_/_p_y_t_e_s_t_-_2_5_9_/     _f_u_n_c_t_i_o_n_)
-_p_o_p_e_n_-_g_w_0_/_t_7_5_/_o_t_h_e_r_s_r_c_/_o_t_h_e_r_._p_y
-_h_e_r_e_._p_y                         _(_n_o       4          1       0        75%
-                                _f_u_n_c_t_i_o_n_)
-Total                                     5          1       0        80%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee    ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_m_3_._p_y   _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
+_m_a_i_n_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 8          0       0        100%
+Total                 10         0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/other/here_py.html` & `coverage-7.5.1/tests/gold/html/other/here_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for here.py: 75%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_03907183.png">
+    <link rel="stylesheet" href="style_cb_03907183.css" type="text/css">
+    <script src="coverage_html_cb_03907183.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>here.py</b>:
             <span class="pc_cov">75%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_03907183.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">4 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">3<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">1<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_a11f93934cf4431e_other_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="z_24e758a651d768e5_other_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 08:10 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -86,18 +86,18 @@
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">    <span class="nam">h</span> <span class="op">=</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">    <span class="nam">h</span> <span class="op">=</span> <span class="num">4</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_a11f93934cf4431e_other_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="z_24e758a651d768e5_other_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 08:10 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 44 ssttaatteemmeennttss ?  33 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 08:10 -0400
 _1import other 
 _2 
 _3if 1 < 2: 
 _4 h = 3 
 _5else: 
 _6 h = 4 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 08:10 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/other/index.html` & `coverage-7.5.1/tests/gold/html/b_branch/class_index.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">80%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
+                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
+                        <kbd>b</kbd>
+                        <kbd>p</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
                         <kbd>[</kbd>
                         <kbd>]</kbd>
                         &nbsp; prev/next file
@@ -44,75 +47,77 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button current">Files</a>
+                <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="z_a11f93934cf4431e_other_py.html">/private/var/folders/6j/khn0mcrj35d1k3yylpl8zl080000gn/T/pytest-of-ned/pytest-259/popen-gw0/t75/othersrc/other.py</a></td>
-                <td>1</td>
+                <td class="name left"><a href="b_py.html">b.py</a></td>
+                <td class="name left"><a href="b_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>6</td>
+                <td>0</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="1 1">100%</td>
-            </tr>
-            <tr class="region">
-                <td class="name left"><a href="here_py.html">here.py</a></td>
-                <td>4</td>
-                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="3 4">75%</td>
+                <td class="right" data-ratio="6 6">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>5</td>
-                <td>1</td>
+                <td class="name left">&nbsp;</td>
+                <td>6</td>
+                <td>0</td>
+                <td>0</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="4 5">80%</td>
+                <td class="right" data-ratio="6 6">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="here_py.html"></a>
-        <a id="nextFileLink" class="nav" href="z_a11f93934cf4431e_other_py.html"></a>
+        <a id="prevFileLink" class="nav" href=""></a>
+        <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,19 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 8800%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x c   change column sorting
+f n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee                                      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_/_p_r_i_v_a_t_e_/_v_a_r_/_f_o_l_d_e_r_s_/_6_j_/
-_k_h_n_0_m_c_r_j_3_5_d_1_k_3_y_y_l_p_l_8_z_l_0_8_0_0_0_0_g_n_/_T_/_p_y_t_e_s_t_-  1          0       0        100%
-_o_f_-_n_e_d_/_p_y_t_e_s_t_-_2_5_9_/_p_o_p_e_n_-_g_w_0_/_t_7_5_/_o_t_h_e_r_s_r_c_/
-_o_t_h_e_r_._p_y
-_h_e_r_e_._p_y                                   4          1       0        75%
-Total                                     5          1       0        80%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
+FFiillee  ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
+_b_._p_y  _(_n_o_ _c_l_a_s_s_) 6          0       0        0        0       100%
+Total            6          0       0        0        0       100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial/class_index.html` & `coverage-7.5.1/tests/gold/html/partial/class_index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">91%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -52,31 +52,31 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-29 17:40 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="partial_py.html">partial.py</a></td>
                 <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
                 <td>7</td>
@@ -103,16 +103,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-29 17:40 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 Shortcuts on this page
 f n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-29 17:40 -0300
 FFiillee       ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
 _p_a_r_t_i_a_l_._p_y _(_n_o_ _c_l_a_s_s_) 7          0       1        4        1       91%
 Total                 7          0       1        4        1       91%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-29 17:40 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial/function_index.html` & `coverage-7.5.1/tests/gold/html/partial_626/class_index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">91%</span>
+            <span class="pc_cov">87%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -48,71 +48,71 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button current">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button" href="function_index.html">Functions</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="partial_py.html">partial.py</a></td>
-                <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>7</td>
+                <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>9</td>
                 <td>0</td>
                 <td>1</td>
-                <td>4</td>
-                <td>1</td>
-                <td class="right" data-ratio="10 11">91%</td>
+                <td>6</td>
+                <td>2</td>
+                <td class="right" data-ratio="13 15">87%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>7</td>
+                <td>9</td>
                 <td>0</td>
                 <td>1</td>
-                <td>4</td>
-                <td>1</td>
-                <td class="right" data-ratio="10 11">91%</td>
+                <td>6</td>
+                <td>2</td>
+                <td class="right" data-ratio="13 15">87%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 9911%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8877%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
-_p_a_r_t_i_a_l_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 7          0       1        4        1       91%
-Total                    7          0       1        4        1       91%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee       ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
+_p_a_r_t_i_a_l_._p_y _(_n_o_ _c_l_a_s_s_) 9          0       1        6        2       87%
+Total                 9          0       1        6        2       87%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial/index.html` & `coverage-7.5.1/tests/gold/html/partial_626/function_index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">91%</span>
+            <span class="pc_cov">87%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
+                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>b</kbd>
                         <kbd>p</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
@@ -46,74 +47,77 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button current">Files</a>
-                <a class="button" href="function_index.html">Functions</a>
+                <a class="button" href="index.html">Files</a>
+                <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="partial_py.html">partial.py</a></td>
-                <td>7</td>
+                <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>9</td>
                 <td>0</td>
                 <td>1</td>
-                <td>4</td>
-                <td>1</td>
-                <td class="right" data-ratio="10 11">91%</td>
+                <td>6</td>
+                <td>2</td>
+                <td class="right" data-ratio="13 15">87%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>7</td>
+                <td class="name left">&nbsp;</td>
+                <td>9</td>
                 <td>0</td>
                 <td>1</td>
-                <td>4</td>
-                <td>1</td>
-                <td class="right" data-ratio="10 11">91%</td>
+                <td>6</td>
+                <td>2</td>
+                <td class="right" data-ratio="13 15">87%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="partial_py.html"></a>
-        <a id="nextFileLink" class="nav" href="partial_py.html"></a>
+        <a id="prevFileLink" class="nav" href=""></a>
+        <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 9911%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 8877%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x b p c   change column sorting
+f n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
-_p_a_r_t_i_a_l_._p_y 7          0       1        4        1       91%
-Total      7          0       1        4        1       91%
+********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee       ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
+_p_a_r_t_i_a_l_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 9          0       1        6        2       87%
+Total                    9          0       1        6        2       87%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial/partial_py.html` & `coverage-7.5.1/tests/gold/html/partial/partial_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for partial.py: 91%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>partial.py</b>:
             <span class="pc_cov">91%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -62,16 +62,16 @@
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">1<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 08:07 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -81,15 +81,15 @@
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># partial branches and excluded lines</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">a</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">while</span> <span class="str">"no peephole"</span><span class="op">.</span><span class="nam">upper</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>        <span class="com"># t4</span>&nbsp;</span><span class="r"><span class="annotate short">4&#x202F;&#x219B;&#x202F;7</span><span class="annotate long">line 4 didn't jump to line 7, because the condition on line 4 was never false</span></span></p>
+    <p class="par run show_par"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">while</span> <span class="str">"no peephole"</span><span class="op">.</span><span class="nam">upper</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>        <span class="com"># t4</span>&nbsp;</span><span class="r"><span class="annotate short">4&#x202F;&#x219B;&#x202F;7</span><span class="annotate long">line 4 didn't jump to line 7, because the condition on line 4 was always true</span></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">    <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">while</span> <span class="nam">a</span><span class="op">:</span>        <span class="com"># pragma: no branch</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">if</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">never_happen</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
@@ -103,14 +103,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 08:07 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,29 +5,29 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 77 ssttaatteemmeennttss ?  77 rruunn 00 mmiissssiinngg 11 eexxcclluuddeedd 11 ppaarrttiiaall **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-25 08:07 -0400
 _1# partial branches and excluded lines 
 _2a = 2 
 _3 
 _4while "no peephole".upper(): # t4 4 ↛ 7line 4 didn't jump to line 7, because
-the condition on line 4 was never false
+the condition on line 4 was always true
 _5 break 
 _6 
 _7while a: # pragma: no branch 
 _8 break 
 _9 
 _1_0if 0: 
 _1_1 never_happen() 
 _1_2 
 _1_3if 13: 
 _1_4 a = 14 
 _1_5 
 _1_6if a == 16: 
 _1_7 raise ZeroDivisionError("17") 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-25 08:07 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/partial_626/class_index.html` & `coverage-7.5.1/tests/gold/html/partial/function_index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">87%</span>
+            <span class="pc_cov">91%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -48,71 +48,71 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button current">Functions</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-29 17:40 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="partial_py.html">partial.py</a></td>
-                <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>9</td>
+                <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>7</td>
                 <td>0</td>
                 <td>1</td>
-                <td>6</td>
-                <td>2</td>
-                <td class="right" data-ratio="13 15">87%</td>
+                <td>4</td>
+                <td>1</td>
+                <td class="right" data-ratio="10 11">91%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>9</td>
+                <td>7</td>
                 <td>0</td>
                 <td>1</td>
-                <td>6</td>
-                <td>2</td>
-                <td class="right" data-ratio="13 15">87%</td>
+                <td>4</td>
+                <td>1</td>
+                <td class="right" data-ratio="10 11">91%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-29 17:40 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 8877%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 9911%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
-_p_a_r_t_i_a_l_._p_y _(_n_o_ _c_l_a_s_s_) 9          0       1        6        2       87%
-Total                 9          0       1        6        2       87%
+********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-29 17:40 -0300
+FFiillee       ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
+_p_a_r_t_i_a_l_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 7          0       1        4        1       91%
+Total                    7          0       1        4        1       91%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-29 17:40 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial_626/function_index.html` & `coverage-7.5.1/tests/gold/html/bom/class_index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">87%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
-                        <kbd>b</kbd>
-                        <kbd>p</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
                         <kbd>[</kbd>
                         <kbd>]</kbd>
                         &nbsp; prev/next file
@@ -48,71 +46,65 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button current">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button" href="function_index.html">Functions</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="partial_py.html">partial.py</a></td>
-                <td class="name left"><a href="partial_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>9</td>
+                <td class="name left"><a href="bom_py.html">bom.py</a></td>
+                <td class="name left"><a href="bom_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>3</td>
                 <td>0</td>
-                <td>1</td>
-                <td>6</td>
-                <td>2</td>
-                <td class="right" data-ratio="13 15">87%</td>
+                <td>0</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>9</td>
+                <td>3</td>
+                <td>0</td>
                 <td>0</td>
-                <td>1</td>
-                <td>6</td>
-                <td>2</td>
-                <td class="right" data-ratio="13 15">87%</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 8877%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f n s m x b p c   change column sorting
+f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
-_p_a_r_t_i_a_l_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 9          0       1        6        2       87%
-Total                    9          0       1        6        2       87%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee   ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_b_o_m_._p_y _(_n_o_ _c_l_a_s_s_) 3          0       0        100%
+Total             3          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial_626/index.html` & `coverage-7.5.1/tests/gold/html/partial_626/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">87%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -51,30 +51,30 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="branches" aria-sort="none" data-default-sort-order="descending" data-shortcut="b">branches<span class="arrows"></span></th>
+                <th id="partial" aria-sort="none" data-default-sort-order="descending" data-shortcut="p">partial<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
                 <td class="name left"><a href="partial_py.html">partial.py</a></td>
                 <td>9</td>
                 <td>0</td>
@@ -99,16 +99,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:02 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="partial_py.html"></a>
         <a id="nextFileLink" class="nav" href="partial_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
 Shortcuts on this page
 f s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
 FFiillee       ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
 _p_a_r_t_i_a_l_._p_y 9          0       1        6        2       87%
 Total      9          0       1        6        2       87%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:02 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/partial_626/partial_py.html` & `coverage-7.5.1/tests/gold/html/partial_626/partial_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for partial.py: 87%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>partial.py</b>:
             <span class="pc_cov">87%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -62,16 +62,16 @@
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">2<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 08:04 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -81,36 +81,36 @@
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># partial branches and excluded lines</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="nam">a</span> <span class="op">=</span> <span class="num">2</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">while</span> <span class="str">"no peephole"</span><span class="op">.</span><span class="nam">upper</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>        <span class="com"># t4</span>&nbsp;</span><span class="r"><span class="annotate short">4&#x202F;&#x219B;&#x202F;7</span><span class="annotate long">line 4 didn't jump to line 7, because the condition on line 4 was never false</span></span></p>
+    <p class="par run show_par"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">while</span> <span class="str">"no peephole"</span><span class="op">.</span><span class="nam">upper</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>        <span class="com"># t4</span>&nbsp;</span><span class="r"><span class="annotate short">4&#x202F;&#x219B;&#x202F;7</span><span class="annotate long">line 4 didn't jump to line 7, because the condition on line 4 was always true</span></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">    <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">while</span> <span class="nam">a</span><span class="op">:</span>        <span class="com"># pragma: no branch</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">if</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">never_happen</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">if</span> <span class="num">13</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">13&#x202F;&#x219B;&#x202F;16</span><span class="annotate long">line 13 didn't jump to line 16, because the condition on line 13 was never false</span></span></p>
+    <p class="par run show_par"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">if</span> <span class="num">13</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">13&#x202F;&#x219B;&#x202F;16</span><span class="annotate long">line 13 didn't jump to line 16, because the condition on line 13 was always true</span></span></p>
     <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">a</span> <span class="op">=</span> <span class="num">14</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">if</span> <span class="nam">a</span> <span class="op">==</span> <span class="num">16</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">raise</span> <span class="nam">ZeroDivisionError</span><span class="op">(</span><span class="str">"17"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 08:04 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,30 +5,30 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 99 ssttaatteemmeennttss ?  99 rruunn 00 mmiissssiinngg 11 eexxcclluuddeedd 22 ppaarrttiiaall **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-25 08:04 -0400
 _1# partial branches and excluded lines 
 _2a = 2 
 _3 
 _4while "no peephole".upper(): # t4 4 ↛ 7line 4 didn't jump to line 7, because
-the condition on line 4 was never false
+the condition on line 4 was always true
 _5 break 
 _6 
 _7while a: # pragma: no branch 
 _8 break 
 _9 
 _1_0if 0: 
 _1_1 never_happen() 
 _1_2 
 _1_3if 13: 13 ↛ 16line 13 didn't jump to line 16, because the condition on line
-13 was never false
+13 was always true
 _1_4 a = 14 
 _1_5 
 _1_6if a == 16: 
 _1_7 raise ZeroDivisionError("17") 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-25 08:04 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/styled/a_py.html` & `coverage-7.5.1/tests/gold/html/styled/a_py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for a.py: 67%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-        <link rel="stylesheet" href="extra.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+        <link rel="stylesheet" href="myextra_cb_232e8e19.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>a.py</b>:
             <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -61,16 +61,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 16:04 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -90,14 +90,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 16:04 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 33 ssttaatteemmeennttss ?  22 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 16:04 -0400
 _1if 1 < 2: 
 _2 # Needed a < to look at HTML entities. 
 _3 a = 3 
 _4else: 
 _5 a = 4 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 16:04 -0400
```

### Comparing `coverage-7.5.0/tests/gold/html/styled/class_index.html` & `coverage-7.5.1/tests/gold/html/unicode/class_index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-        <link rel="stylesheet" href="extra.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">67%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -51,61 +50,61 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="a_py.html">a.py</a></td>
-                <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
-                <td>3</td>
-                <td>1</td>
+                <td class="name left"><a href="unicode_py.html">unicode.py</a></td>
+                <td class="name left"><a href="unicode_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>3</td>
-                <td>1</td>
+                <td>2</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee  ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_a_._p_y  _(_n_o_ _c_l_a_s_s_) 3          1       0        67%
-Total            3          1       0        67%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee       ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_u_n_i_c_o_d_e_._p_y _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
+Total                 2          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/styled/function_index.html` & `coverage-7.5.1/tests/gold/html/unicode/function_index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-        <link rel="stylesheet" href="extra.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">67%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -51,61 +50,61 @@
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
                 <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="a_py.html">a.py</a></td>
-                <td class="name left"><a href="a_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>3</td>
-                <td>1</td>
+                <td class="name left"><a href="unicode_py.html">unicode.py</a></td>
+                <td class="name left"><a href="unicode_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td>0</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>3</td>
-                <td>1</td>
+                <td>2</td>
+                <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee  ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_a_._p_y  _(_n_o_ _f_u_n_c_t_i_o_n_) 3          1       0        67%
-Total               3          1       0        67%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee       ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_u_n_i_c_o_d_e_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
+Total                    2          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/styled/index.html` & `coverage-7.5.1/tests/gold/html/bom/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-        <link rel="stylesheet" href="extra.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_f81f1c3a.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">67%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>s</kbd>
@@ -50,63 +49,63 @@
         </form>
         <h2>
                 <a class="button current">Files</a>
                 <a class="button" href="function_index.html">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="a_py.html">a.py</a></td>
+                <td class="name left"><a href="bom_py.html">bom.py</a></td>
                 <td>3</td>
-                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td>0</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>3</td>
-                <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 3">67%</td>
+                <td>0</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-25 23:03 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="a_py.html"></a>
-        <a id="nextFileLink" class="nav" href="a_py.html"></a>
+        <a id="prevFileLink" class="nav" href="bom_py.html"></a>
+        <a id="nextFileLink" class="nav" href="bom_py.html"></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 6677%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
 ********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_a_._p_y  3          1       0        67%
-Total 3          1       0        67%
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
+FFiillee   ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_b_o_m_._p_y 3          0       0        100%
+Total  3          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-25 23:03 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/styled/style.css` & `coverage-7.5.1/tests/gold/html/styled/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/html/support/coverage_html.js` & `coverage-7.5.1/tests/gold/html/support/coverage_html.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -77,18 +77,42 @@
 
     // Sort all rows and afterwards append them in order to move them in the DOM.
     Array.from(th.closest("table").querySelectorAll("tbody tr"))
         .sort((rowA, rowB) => rowComparator(rowA, rowB, column) * (direction === "ascending" ? 1 : -1))
         .forEach(tr => tr.parentElement.appendChild(tr));
 
     // Save the sort order for next time.
-    localStorage.setItem(coverage.INDEX_SORT_STORAGE, JSON.stringify({
-        column,
-        direction
-    }));
+    if (th.id !== "region") {
+        let th_id = "file"; // Sort by file if we don't have a column id
+        let current_direction = direction;
+        const stored_list = localStorage.getItem(coverage.INDEX_SORT_STORAGE);
+        if (stored_list) {
+            ({
+                th_id,
+                direction
+            } = JSON.parse(stored_list))
+        }
+        localStorage.setItem(coverage.INDEX_SORT_STORAGE, JSON.stringify({
+            "th_id": th.id,
+            "direction": current_direction
+        }));
+        if (th.id !== th_id || document.getElementById("region")) {
+            // Sort column has changed, unset sorting by function or class.
+            localStorage.setItem(coverage.SORTED_BY_REGION, JSON.stringify({
+                "by_region": false,
+                "region_direction": current_direction
+            }));
+        }
+    } else {
+        // Sort column has changed to by function or class, remember that.
+        localStorage.setItem(coverage.SORTED_BY_REGION, JSON.stringify({
+            "by_region": true,
+            "region_direction": direction
+        }));
+    }
 }
 
 // Find all the elements with data-shortcut attribute, and use them to assign a shortcut key.
 coverage.assign_shortkeys = function() {
     document.querySelectorAll("[data-shortcut]").forEach(element => {
         document.addEventListener("keypress", event => {
             if (event.target.tagName.toLowerCase() === "input") {
@@ -226,30 +250,51 @@
 // Set up the click-to-sort columns.
 coverage.wire_up_sorting = function() {
     document.querySelectorAll("[data-sortable] th[aria-sort]").forEach(
         th => th.addEventListener("click", e => sortColumn(e.target))
     );
 
     // Look for a localStorage item containing previous sort settings:
-    var column = 0,
+    let th_id = "file",
         direction = "ascending";
     const stored_list = localStorage.getItem(coverage.INDEX_SORT_STORAGE);
     if (stored_list) {
         ({
-            column,
+            th_id,
             direction
         } = JSON.parse(stored_list));
     }
+    let by_region = false,
+        region_direction = "ascending";
+    const sorted_by_region = localStorage.getItem(coverage.SORTED_BY_REGION);
+    if (sorted_by_region) {
+        ({
+            by_region,
+            region_direction
+        } = JSON.parse(sorted_by_region));
+    }
 
-    const th = document.querySelector("[data-sortable]").tHead.rows[0].cells[column]; // nosemgrep: eslint.detect-object-injection
+    const region_id = "region";
+    if (by_region && document.getElementById(region_id)) {
+        direction = region_direction;
+    }
+    // If we are in a page that has a column with id of "region", sort on
+    // it if the last sort was by function or class.
+    let th;
+    if (document.getElementById(region_id)) {
+        th = document.getElementById(by_region ? region_id : th_id);
+    } else {
+        th = document.getElementById(th_id);
+    }
     th.setAttribute("aria-sort", direction === "ascending" ? "descending" : "ascending");
     th.click()
 };
 
 coverage.INDEX_SORT_STORAGE = "COVERAGE_INDEX_SORT_2";
+coverage.SORTED_BY_REGION = "COVERAGE_SORT_REGION";
 
 // Loaded on index.html
 coverage.index_ready = function() {
     coverage.assign_shortkeys();
     coverage.wire_up_filter();
     coverage.wire_up_sorting();
```

### Comparing `coverage-7.5.0/tests/gold/html/support/favicon_32.png` & `coverage-7.5.1/tests/gold/html/support/favicon_32.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/html/support/keybd_closed.png` & `coverage-7.5.1/tests/gold/html/support/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/html/support/style.css` & `coverage-7.5.1/tests/gold/html/support/style.css`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/html/unicode/class_index.html` & `coverage-7.5.1/tests/gold/html/isolatin1/function_index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -46,39 +46,39 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button" href="function_index.html">Functions</a>
-                <a class="button current">Classes</a>
+                <a class="button current">Functions</a>
+                <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="unicode_py.html">unicode.py</a></td>
-                <td class="name left"><a href="unicode_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td class="name left"><a href="isolatin1_py.html">isolatin1.py</a></td>
+                <td class="name left"><a href="isolatin1_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
                 <td>2</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
         </tbody>
         <tfoot>
@@ -95,16 +95,16 @@
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:13 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -2,14 +2,14 @@
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_u_n_i_c_o_d_e_._p_y _(_n_o_ _c_l_a_s_s_) 2          0       0        100%
-Total                 2          0       0        100%
+********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
+FFiillee         ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_i_s_o_l_a_t_i_n_1_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
+Total                      2          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:13 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/unicode/function_index.html` & `coverage-7.5.1/tests/gold/html/contexts/class_index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
                         <kbd>n</kbd>
@@ -46,65 +46,65 @@
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
                 <a class="button" href="index.html">Files</a>
-                <a class="button current">Functions</a>
-                <a class="button" href="class_index.html">Classes</a>
+                <a class="button" href="function_index.html">Functions</a>
+                <a class="button current">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">class<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="unicode_py.html">unicode.py</a></td>
-                <td class="name left"><a href="unicode_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
-                <td>2</td>
+                <td class="name left"><a href="two_tests_py.html">two_tests.py</a></td>
+                <td class="name left"><a href="two_tests_py.html"><data value=''><span class='no-noun'>(no class)</span></data></a></td>
+                <td>7</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="7 7">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td class="name left">&nbsp;</td>
-                <td>2</td>
+                <td>7</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="7 7">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href=""></a>
         <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
```

#### html2text {}

```diff
@@ -2,14 +2,14 @@
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_u_n_i_c_o_d_e_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 2          0       0        100%
-Total                    2          0       0        100%
+********** _FF_ii_ll_ee_ss _FF_uu_nn_cc_tt_ii_oo_nn_ss CCllaasssseess **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee         ccllaassss      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_t_w_o___t_e_s_t_s_._p_y _(_n_o_ _c_l_a_s_s_) 7          0       0        100%
+Total                   7          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/unicode/index.html` & `coverage-7.5.1/tests/gold/html/bom/function_index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage report</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_718ce007.css" type="text/css">
+    <script src="coverage_html_cb_d1c4fcc4.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>f</kbd>
+                        <kbd>n</kbd>
                         <kbd>s</kbd>
                         <kbd>m</kbd>
                         <kbd>x</kbd>
                         <kbd>c</kbd>
                         &nbsp; change column sorting
                     </p>
                     <p>
@@ -44,68 +45,71 @@
             <input id="filter" type="text" value="" placeholder="filter...">
             <div>
                 <input id="hide100" type="checkbox" >
                 <label for="hide100">hide covered</label>
             </div>
         </form>
         <h2>
-                <a class="button current">Files</a>
-                <a class="button" href="function_index.html">Functions</a>
+                <a class="button" href="index.html">Files</a>
+                <a class="button current">Functions</a>
                 <a class="button" href="class_index.html">Classes</a>
         </h2>
         <p class="text">
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
-                <th class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
-                <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
-                <th class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
+                <th id="file" class="name left" aria-sort="none" data-shortcut="f">File<span class="arrows"></span></th>
+                <th id="region" class="name left" aria-sort="none" data-default-sort-order="ascending" data-shortcut="n">function<span class="arrows"></span></th>
+                <th id="statements" aria-sort="none" data-default-sort-order="descending" data-shortcut="s">statements<span class="arrows"></span></th>
+                <th id="missing" aria-sort="none" data-default-sort-order="descending" data-shortcut="m">missing<span class="arrows"></span></th>
+                <th id="excluded" aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded<span class="arrows"></span></th>
+                <th id="coverage" class="right" aria-sort="none" data-shortcut="c">coverage<span class="arrows"></span></th>
             </tr>
         </thead>
         <tbody>
             <tr class="region">
-                <td class="name left"><a href="unicode_py.html">unicode.py</a></td>
-                <td>2</td>
+                <td class="name left"><a href="bom_py.html">bom.py</a></td>
+                <td class="name left"><a href="bom_py.html"><data value=''><span class='no-noun'>(no function)</span></data></a></td>
+                <td>3</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>2</td>
+                <td class="name left">&nbsp;</td>
+                <td>3</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="2 2">100%</td>
+                <td class="right" data-ratio="3 3">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-28 13:14 -0300
         </p>
     </div>
     <aside class="hidden">
-        <a id="prevFileLink" class="nav" href="unicode_py.html"></a>
-        <a id="nextFileLink" class="nav" href="unicode_py.html"></a>
+        <a id="prevFileLink" class="nav" href=""></a>
+        <a id="nextFileLink" class="nav" href=""></a>
         <button type="button" class="button_prev_file" data-shortcut="["></button>
         <button type="button" class="button_next_file" data-shortcut="]"></button>
         <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
     </aside>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ************ CCoovveerraaggee rreeppoorrtt:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
-f s m x c   change column sorting
+f n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
 ??hide covered
-********** FFiilleess _FF_uu_nn_cc_tt_ii_oo_nn_ss _CC_ll_aa_ss_ss_ee_ss **********
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
-FFiillee       ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_u_n_i_c_o_d_e_._p_y 2          0       0        100%
-Total      2          0       0        100%
+********** _FF_ii_ll_ee_ss FFuunnccttiioonnss _CC_ll_aa_ss_ss_ee_ss **********
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
+FFiillee   ffuunnccttiioonn      ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
+_b_o_m_._p_y _(_n_o_ _f_u_n_c_t_i_o_n_) 3          0       0        100%
+Total                3          0       0        100%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at 2024-04-21 10:39 -0400
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at 2024-04-28 13:14 -0300
```

### Comparing `coverage-7.5.0/tests/gold/html/unicode/unicode_py.html` & `coverage-7.5.1/tests/gold/html/unicode/unicode_py.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <title>Coverage for unicode.py: 100%</title>
-    <link rel="icon" sizes="32x32" href="favicon_32.png">
-    <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <link rel="icon" sizes="32x32" href="favicon_32_cb_58284776.png">
+    <link rel="stylesheet" href="style_cb_8e611ae1.css" type="text/css">
+    <script src="coverage_html_cb_606408f0.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>unicode.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed_cb_ce680311.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -60,16 +60,16 @@
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"></button>
             <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
             <button type="button" class="button_top_of_page" data-shortcut="0"></button>
             <button type="button" class="button_first_chunk" data-shortcut="1"></button>
             <button type="button" class="button_prev_file" data-shortcut="["></button>
@@ -89,14 +89,14 @@
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0a1.dev1">coverage.py v7.5.0a1.dev1</a>,
-            created at 2024-04-21 10:39 -0400
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.1a0.dev1">coverage.py v7.5.1a0.dev1</a>,
+            created at 2024-04-24 09:22 -0400
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
 _1# -*- coding: utf-8 -*- 
 _2# A Python source file with exotic characters. 
 _3 
 _4upside_down = "ʎd˙ǝbɐɹǝʌoɔ" 
 _5surrogate = "db40,dd00: x???" 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0_a_1_._d_e_v_1, created at
-2024-04-21 10:39 -0400
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._1_a_0_._d_e_v_1, created at
+2024-04-24 09:22 -0400
```

### Comparing `coverage-7.5.0/tests/gold/xml/x_xml/coverage.xml` & `coverage-7.5.1/tests/gold/xml/x_xml/coverage.xml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/gold/xml/y_xml_branch/coverage.xml` & `coverage-7.5.1/tests/gold/xml/y_xml_branch/coverage.xml`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/goldtest.py` & `coverage-7.5.1/tests/goldtest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/helpers.py` & `coverage-7.5.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/js/index.html` & `coverage-7.5.1/tests/js/index.html`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/js/tests.js` & `coverage-7.5.1/tests/js/tests.js`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/mixins.py` & `coverage-7.5.1/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/modules/plugins/another.py` & `coverage-7.5.1/tests/modules/plugins/another.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/modules/process_test/try_execfile.py` & `coverage-7.5.1/tests/modules/process_test/try_execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/osinfo.py` & `coverage-7.5.1/tests/osinfo.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/plugin1.py` & `coverage-7.5.1/tests/plugin1.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/plugin2.py` & `coverage-7.5.1/tests/plugin2.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/plugin_config.py` & `coverage-7.5.1/tests/plugin_config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/qunit/jquery.tmpl.min.js` & `coverage-7.5.1/tests/qunit/jquery.tmpl.min.js`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/select_plugin.py` & `coverage-7.5.1/tests/select_plugin.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/stress_phystoken.tok` & `coverage-7.5.1/tests/stress_phystoken.tok`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/stress_phystoken_dos.tok` & `coverage-7.5.1/tests/stress_phystoken_dos.tok`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_annotate.py` & `coverage-7.5.1/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_api.py` & `coverage-7.5.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_arcs.py` & `coverage-7.5.1/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_cmdline.py` & `coverage-7.5.1/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_collector.py` & `coverage-7.5.1/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_concurrency.py` & `coverage-7.5.1/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_config.py` & `coverage-7.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_context.py` & `coverage-7.5.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_coverage.py` & `coverage-7.5.1/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_data.py` & `coverage-7.5.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_debug.py` & `coverage-7.5.1/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_execfile.py` & `coverage-7.5.1/tests/test_execfile.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_filereporter.py` & `coverage-7.5.1/tests/test_filereporter.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_files.py` & `coverage-7.5.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_goldtest.py` & `coverage-7.5.1/tests/test_goldtest.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_html.py` & `coverage-7.5.1/tests/test_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,35 +104,35 @@
         # 12:00 to 12:01:59, or two minutes.
         self.assert_recent_datetime(
             timestamp,
             seconds=120,
             msg=f"Time stamp is wrong: {timestamp}",
         )
 
-    def assert_valid_hrefs(self) -> None:
+    def assert_valid_hrefs(self, directory: str = "htmlcov") -> None:
         """Assert that the hrefs in htmlcov/*.html are valid.
 
         Doesn't check external links (those with a protocol).
         """
         hrefs = collections.defaultdict(set)
-        for fname in glob.glob("htmlcov/*.html"):
+        for fname in glob.glob(f"{directory}/*.html"):
             with open(fname) as fhtml:
                 html = fhtml.read()
             for href in re.findall(r""" href=['"]([^'"]*)['"]""", html):
                 if href.startswith("#"):
                     assert re.search(fr""" id=['"]{href[1:]}['"]""", html), (
                         f"Fragment {href!r} in {fname} has no anchor"
                     )
                     continue
                 if "://" in href:
                     continue
                 href = href.partition("#")[0]   # ignore fragment in URLs.
                 hrefs[href].add(fname)
         for href, sources in hrefs.items():
-            assert os.path.exists(f"htmlcov/{href}"), (
+            assert os.path.exists(f"{directory}/{href}"), (
                 f"These files link to {href!r}, which doesn't exist: {', '.join(sources)}"
             )
 
 
 class FileWriteTracker:
     """A fake object to track how `open` is used to write files."""
     def __init__(self, written: set[str]) -> None:
@@ -181,17 +181,24 @@
         """Assert that all the expected htmlcov files exist."""
         self.assert_exists("htmlcov/index.html")
         self.assert_exists("htmlcov/function_index.html")
         self.assert_exists("htmlcov/class_index.html")
         self.assert_exists("htmlcov/main_file_py.html")
         self.assert_exists("htmlcov/helper1_py.html")
         self.assert_exists("htmlcov/helper2_py.html")
-        self.assert_exists("htmlcov/style.css")
-        self.assert_exists("htmlcov/coverage_html.js")
         self.assert_exists("htmlcov/.gitignore")
+        # Cache-busted files have random data in the name, but they should all
+        # be there, and there should only be one of each.
+        statics = ["style.css", "coverage_html.js", "keybd_closed.png", "favicon_32.png"]
+        files = os.listdir("htmlcov")
+        for static in statics:
+            base, ext = os.path.splitext(static)
+            busted_file_pattern = fr"{base}_cb_\w{{8}}{ext}"
+            matches = [m for f in files if (m := re.fullmatch(busted_file_pattern, f))]
+            assert len(matches) == 1, f"Found {len(matches)} files for {static}"
 
     def test_html_created(self) -> None:
         # Test basic HTML generation: files should be created.
         self.create_initial_files()
         self.run_coverage()
         self.assert_htmlcov_files_exist()
 
@@ -687,33 +694,47 @@
     """Specialized compare function for our HTML files."""
     __tracebackhide__ = True    # pytest, please don't show me this function.
     scrubs = [
         (r'/coverage\.readthedocs\.io/?[-.\w/]*', '/coverage.readthedocs.io/VER'),
         (r'coverage\.py v[\d.abcdev]+', 'coverage.py vVER'),
         (r'created at \d\d\d\d-\d\d-\d\d \d\d:\d\d [-+]\d\d\d\d', 'created at DATE'),
         (r'created at \d\d\d\d-\d\d-\d\d \d\d:\d\d', 'created at DATE'),
+        # Static files have cache busting.
+        (r'_cb_\w{8}\.', '_CB.'),
         # Occasionally an absolute path is in the HTML report.
         (filepath_to_regex(TESTS_DIR), 'TESTS_DIR'),
         (filepath_to_regex(flat_rootname(str(TESTS_DIR))), '_TESTS_DIR'),
         # The temp dir the tests make.
         (filepath_to_regex(os.getcwd()), 'TEST_TMPDIR'),
         (filepath_to_regex(flat_rootname(str(os.getcwd()))), '_TEST_TMPDIR'),
         (filepath_to_regex(abs_file(os.getcwd())), 'TEST_TMPDIR'),
         (filepath_to_regex(flat_rootname(str(abs_file(os.getcwd())))), '_TEST_TMPDIR'),
         (r'/private/var/[\w/]+/pytest-of-\w+/pytest-\d+/(popen-gw\d+/)?t\d+', 'TEST_TMPDIR'),
+        # If the gold files were created on Windows, we need to scrub Windows paths also:
+        (r'[A-Z]:\\Users\\[\w\\]+\\pytest-of-\w+\\pytest-\d+\\(popen-gw\d+\\)?t\d+', 'TEST_TMPDIR'),
     ]
-    if env.WINDOWS:
-        # For file paths...
-        scrubs += [(r"\\", "/")]
     if extra_scrubs:
         scrubs += extra_scrubs
     compare(expected, actual, file_pattern="*.html", scrubs=scrubs)
 
 
-class HtmlGoldTest(CoverageTest):
+def unbust(directory: str) -> None:
+    """Find files with cache busting, and rename them to simple names.
+
+    This makes it possible for us to compare gold files.
+    """
+    with change_dir(directory):
+        for fname in os.listdir("."):
+            base, ext = os.path.splitext(fname)
+            base, _, _ = base.partition("_cb_")
+            if base != fname:
+                os.rename(fname, base + ext)
+
+
+class HtmlGoldTest(HtmlTestHelpers, CoverageTest):
     """Tests of HTML reporting that use gold files."""
 
     def test_a(self) -> None:
         self.make_file("a.py", """\
             if 1 < 2:
                 # Needed a < to look at HTML entities.
                 a = 3
@@ -787,25 +808,25 @@
              '<span class="op">&lt;</span> <span class="num">2</span>'),
             ('    <span class="nam">a</span> <span class="op">=</span> ' +
              '<span class="num">3</span>'),
             '<span class="pc_cov">70%</span>',
 
             ('<span class="annotate short">3&#x202F;&#x219B;&#x202F;6</span>' +
              '<span class="annotate long">line 3 didn\'t jump to line 6, ' +
-                            'because the condition on line 3 was never false</span>'),
+                            'because the condition on line 3 was always true</span>'),
             ('<span class="annotate short">12&#x202F;&#x219B;&#x202F;exit</span>' +
              '<span class="annotate long">line 12 didn\'t return from function \'two\', ' +
-                            'because the condition on line 12 was never false</span>'),
+                            'because the condition on line 12 was always true</span>'),
             ('<span class="annotate short">20&#x202F;&#x219B;&#x202F;21,&nbsp;&nbsp; ' +
                             '20&#x202F;&#x219B;&#x202F;23</span>' +
              '<span class="annotate long">2 missed branches: ' +
                             '1) line 20 didn\'t jump to line 21, ' +
                                 'because the condition on line 20 was never true, ' +
                             '2) line 20 didn\'t jump to line 23, ' +
-                                'because the condition on line 20 was never false</span>'),
+                                'because the condition on line 20 was always true</span>'),
         )
         contains(
             "out/b_branch/index.html",
             '<a href="b_py.html">b.py</a>',
             '<span class="pc_cov">70%</span>',
             '<td class="right" data-ratio="16 23">70%</td>',
         )
@@ -960,15 +981,16 @@
         actual_file = list(glob.glob("out/other/*_other_py.html"))
         assert len(actual_file) == 1
         os.rename(actual_file[0], "out/other/blah_blah_other_py.html")
 
         compare_html(
             gold_path("html/other"), "out/other",
             extra_scrubs=[
-                (r'href="z_[0-9a-z]{16}_', 'href="_TEST_TMPDIR_othersrc_'),
+                (r'href="z_[0-9a-z]{16}_other_', 'href="_TEST_TMPDIR_other_othersrc_'),
+                (r'TEST_TMPDIR\\othersrc\\other.py', 'TEST_TMPDIR/othersrc/other.py'),
             ],
         )
         contains(
             'out/other/index.html',
             '<a href="here_py.html">here.py</a>',
             'other_py.html">',
             'other.py</a>',
@@ -1046,36 +1068,37 @@
             if 1 < 2:
                 # Needed a < to look at HTML entities.
                 a = 3
             else:
                 a = 4
             """)
 
-        self.make_file("extra.css", "/* Doesn't matter what goes in here, it gets copied. */\n")
+        self.make_file("myfile/myextra.css", "/* Doesn't matter what's here, it gets copied. */\n")
 
         cov = coverage.Coverage()
         a = self.start_import_stop(cov, "a")
-        cov.html_report(a, directory="out/styled", extra_css="extra.css")
-
+        cov.html_report(a, directory="out/styled", extra_css="myfile/myextra.css")
+        self.assert_valid_hrefs("out/styled")
         compare_html(gold_path("html/styled"), "out/styled")
+        unbust("out/styled")
         compare(gold_path("html/styled"), "out/styled", file_pattern="*.css")
-        contains(
+        contains_rx(
             "out/styled/a_py.html",
-            '<link rel="stylesheet" href="extra.css" type="text/css">',
-            ('<span class="key">if</span> <span class="num">1</span> ' +
-             '<span class="op">&lt;</span> <span class="num">2</span>'),
-            ('    <span class="nam">a</span> <span class="op">=</span> ' +
-             '<span class="num">3</span>'),
-            '<span class="pc_cov">67%</span>',
+            r'<link rel="stylesheet" href="myextra_cb_\w{8}.css" type="text/css">',
+            (r'<span class="key">if</span> <span class="num">1</span> ' +
+             r'<span class="op">&lt;</span> <span class="num">2</span>'),
+            (r'    <span class="nam">a</span> <span class="op">=</span> ' +
+             r'<span class="num">3</span>'),
+            r'<span class="pc_cov">67%</span>',
         )
-        contains(
+        contains_rx(
             "out/styled/index.html",
-            '<link rel="stylesheet" href="extra.css" type="text/css">',
-            '<a href="a_py.html">a.py</a>',
-            '<span class="pc_cov">67%</span>',
+            r'<link rel="stylesheet" href="myextra_cb_\w{8}.css" type="text/css">',
+            r'<a href="a_py.html">a.py</a>',
+            r'<span class="pc_cov">67%</span>',
         )
 
     def test_tabbed(self) -> None:
         # The file contents would look like this with 8-space tabs:
         #   x = 1
         #   if x:
         #           a = "tabbed"                            # aligned comments
```

### Comparing `coverage-7.5.0/tests/test_json.py` & `coverage-7.5.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_lcov.py` & `coverage-7.5.1/tests/test_lcov.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_misc.py` & `coverage-7.5.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_mixins.py` & `coverage-7.5.1/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_numbits.py` & `coverage-7.5.1/tests/test_numbits.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_oddball.py` & `coverage-7.5.1/tests/test_oddball.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_parser.py` & `coverage-7.5.1/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,14 +421,32 @@
                     x = 1    # Now it is skipped.
 
             f()
             """,
         )
         assert parser.statements == {1,7}
 
+    def test_multiline_if_no_branch(self) -> None:
+        # From https://github.com/nedbat/coveragepy/issues/754
+        parser = self.parse_text("""\
+            if (this_is_a_verylong_boolean_expression == True   # pragma: no branch
+                and another_long_expression and here_another_expression):
+                do_something()
+            """,
+        )
+        parser2 = self.parse_text("""\
+            if this_is_a_verylong_boolean_expression == True and another_long_expression \\
+                and here_another_expression:  # pragma: no branch
+                do_something()
+            """,
+        )
+        assert parser.statements == parser2.statements == {1, 3}
+        pragma_re = ".*pragma: no branch.*"
+        assert parser.lines_matching(pragma_re) == parser2.lines_matching(pragma_re)
+
     def test_excluding_function(self) -> None:
         parser = self.parse_text("""\
             def fn(foo):      # nocover
                 a = 1
                 b = 2
                 c = 3
 
@@ -755,28 +773,28 @@
             def func10():
                 while something(11):
                     thing(12)
                 more_stuff(13)
             """)
         expected = "line 1 didn't jump to line 2, because the condition on line 1 was never true"
         assert expected == parser.missing_arc_description(1, 2)
-        expected = "line 1 didn't jump to line 3, because the condition on line 1 was never false"
+        expected = "line 1 didn't jump to line 3, because the condition on line 1 was always true"
         assert expected == parser.missing_arc_description(1, 3)
         expected = (
             "line 6 didn't return from function 'func5', " +
             "because the loop on line 6 didn't complete"
         )
         assert expected == parser.missing_arc_description(6, -5)
         expected = "line 6 didn't jump to line 7, because the loop on line 6 never started"
         assert expected == parser.missing_arc_description(6, 7)
         expected = "line 11 didn't jump to line 12, because the condition on line 11 was never true"
         assert expected == parser.missing_arc_description(11, 12)
         expected = (
             "line 11 didn't jump to line 13, " +
-            "because the condition on line 11 was never false"
+            "because the condition on line 11 was always true"
         )
         assert expected == parser.missing_arc_description(11, 13)
 
     def test_missing_arc_descriptions_for_small_callables(self) -> None:
         parser = self.parse_text("""\
             callables = [
                 lambda: 2,
```

### Comparing `coverage-7.5.0/tests/test_phystokens.py` & `coverage-7.5.1/tests/test_phystokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
                             pass
 
             class case(): pass
             def match():
                 global case
             """)
         tokens = list(source_token_lines(source))
+        print(tokens)
         assert tokens[0][0] == ("key", "match")
         assert tokens[0][4] == ("nam", "match")
         assert tokens[1][1] == ("key", "case")
         assert tokens[2][1] == ("nam", "match")
         assert tokens[2][5] == ("nam", "case")
         assert tokens[3][1] == ("key", "case")
         assert tokens[4][1] == ("nam", "match")
```

### Comparing `coverage-7.5.0/tests/test_plugins.py` & `coverage-7.5.1/tests/test_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from tests.coveragetest import CoverageTest
 from tests.helpers import CheckUniqueFilenames, swallow_warnings
 
 
 class NullConfig(TPluginConfig):
     """A plugin configure thing when we don't really need one."""
     def get_plugin_options(self, plugin: str) -> TConfigSectionOut:
-        return {}
+        return {}   # pragma: never called
 
 
 class FakeConfig(TPluginConfig):
     """A fake config for use in tests."""
 
     def __init__(self, plugin: str, options: dict[str, Any]) -> None:
         self.plugin = plugin
@@ -280,15 +280,16 @@
         self.make_file("simple.py", "a = 1")
 
         cov = coverage.Coverage()
         cov.set_option("run:plugins", ["tests.plugin1"])
 
         if testenv.PY_TRACER:
             core = "PyTracer"
-        elif testenv.SYS_MON:
+        else:
+            assert testenv.SYS_MON
             core = "SysMonitor"
 
         expected_warnings = [
             fr"Plugin file tracers \(tests.plugin1.Plugin\) aren't supported with {core}",
         ]
         with self.assert_warnings(cov, expected_warnings):
             self.start_import_stop(cov, "simple")
```

### Comparing `coverage-7.5.0/tests/test_process.py` & `coverage-7.5.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_python.py` & `coverage-7.5.1/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_regions.py` & `coverage-7.5.1/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_report.py` & `coverage-7.5.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_report_common.py` & `coverage-7.5.1/tests/test_report_common.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_report_core.py` & `coverage-7.5.1/tests/test_report_core.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_results.py` & `coverage-7.5.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_setup.py` & `coverage-7.5.1/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_sqlitedb.py` & `coverage-7.5.1/tests/test_sqlitedb.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_templite.py` & `coverage-7.5.1/tests/test_templite.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_testing.py` & `coverage-7.5.1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_venv.py` & `coverage-7.5.1/tests/test_venv.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_version.py` & `coverage-7.5.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/test_xml.py` & `coverage-7.5.1/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tests/testenv.py` & `coverage-7.5.1/tests/testenv.py`

 * *Files identical despite different names*

### Comparing `coverage-7.5.0/tox.ini` & `coverage-7.5.1/tox.ini`

 * *Files identical despite different names*

