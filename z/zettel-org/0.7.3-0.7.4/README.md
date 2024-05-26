# Comparing `tmp/zettel_org-0.7.3.tar.gz` & `tmp/zettel_org-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel_org-0.7.3.tar", last modified: Sat May 18 01:59:35 2024, max compression
+gzip compressed data, was "zettel_org-0.7.4.tar", last modified: Sun May 26 14:41:42 2024, max compression
```

## Comparing `zettel_org-0.7.3.tar` & `zettel_org-0.7.4.tar`

### file list

```diff
@@ -1,196 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-18 01:59:27.000000 zettel_org-0.7.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-18 01:59:27.000000 zettel_org-0.7.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-18 01:59:27.000000 zettel_org-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-18 01:59:27.000000 zettel_org-0.7.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-18 01:59:27.000000 zettel_org-0.7.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-18 01:59:35.728771 zettel_org-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-18 01:59:27.000000 zettel_org-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3093 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 01:59:27.000000 zettel_org-0.7.3/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.700770 zettel_org-0.7.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/tags_and_ids.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/examples/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_query/all_contexts.zoq
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_query/open_projects.zoq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-18 01:59:27.000000 zettel_org-0.7.3/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-18 01:59:27.000000 zettel_org-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-18 01:59:27.000000 zettel_org-0.7.3/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-18 01:59:35.732771 zettel_org-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-18 01:59:27.000000 zettel_org-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.700770 zettel_org-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:59:31.000000 zettel_org-0.7.3/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/app/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/domain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/domain/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/messages/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/messages/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/domain/models/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/models/_zorg_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/models/_zorg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/CommonLexerRules.g4
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/ZorgQuery.g4
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)    16243 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   121459 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/grammar/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQuery.interp
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQuery.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryListener.py
--rw-r--r--   0 runner    (1001) docker     (127)    92723 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/service/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16269 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/_file_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/_query_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/messagebus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/service/swog/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/swog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/swog/_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/zid_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/storage/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-18 01:59:27.000000 zettel_org-0.7.3/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_action_open.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    62043 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_db.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    29656 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_query.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.678907 zettel_org-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.654907 zettel_org-0.7.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.654907 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.654907 zettel_org-0.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-26 14:41:34.000000 zettel_org-0.7.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-26 14:41:34.000000 zettel_org-0.7.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-26 14:41:34.000000 zettel_org-0.7.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-26 14:41:34.000000 zettel_org-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-26 14:41:34.000000 zettel_org-0.7.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-26 14:41:34.000000 zettel_org-0.7.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-26 14:41:42.678907 zettel_org-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-26 14:41:34.000000 zettel_org-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.654907 zettel_org-0.7.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3093 2024-05-26 14:41:34.000000 zettel_org-0.7.4/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-26 14:41:34.000000 zettel_org-0.7.4/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-26 14:41:34.000000 zettel_org-0.7.4/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-26 14:41:34.000000 zettel_org-0.7.4/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-26 14:41:34.000000 zettel_org-0.7.4/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.654907 zettel_org-0.7.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.654907 zettel_org-0.7.4/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 14:41:34.000000 zettel_org-0.7.4/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 14:41:34.000000 zettel_org-0.7.4/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.646907 zettel_org-0.7.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/examples/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_query/all_contexts.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_query/desc_filter.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_query/file_filter.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 14:41:34.000000 zettel_org-0.7.4/examples/zorg_query/open_projects.zoq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-26 14:41:34.000000 zettel_org-0.7.4/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-26 14:41:34.000000 zettel_org-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-26 14:41:34.000000 zettel_org-0.7.4/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-26 14:41:34.000000 zettel_org-0.7.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-26 14:41:34.000000 zettel_org-0.7.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-26 14:41:34.000000 zettel_org-0.7.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.658908 zettel_org-0.7.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-26 14:41:34.000000 zettel_org-0.7.4/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-26 14:41:42.678907 zettel_org-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-26 14:41:34.000000 zettel_org-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.646907 zettel_org-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.678907 zettel_org-0.7.4/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-26 14:41:42.000000 zettel_org-0.7.4/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-26 14:41:42.000000 zettel_org-0.7.4/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:41:42.000000 zettel_org-0.7.4/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 14:41:42.000000 zettel_org-0.7.4/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:41:38.000000 zettel_org-0.7.4/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-26 14:41:42.000000 zettel_org-0.7.4/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 14:41:42.000000 zettel_org-0.7.4/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.662907 zettel_org-0.7.4/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.662907 zettel_org-0.7.4/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.662907 zettel_org-0.7.4/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.662907 zettel_org-0.7.4/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.662907 zettel_org-0.7.4/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/messages/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.662907 zettel_org-0.7.4/src/zorg/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/models/_zorg_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/models/_zorg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.666907 zettel_org-0.7.4/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/CommonLexerRules.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/ZorgQuery.g4
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.666907 zettel_org-0.7.4/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122442 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.666907 zettel_org-0.7.4/src/zorg/grammar/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQuery.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQuery.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)    13132 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106001 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/grammar/zorg_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.670907 zettel_org-0.7.4/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.670907 zettel_org-0.7.4/src/zorg/service/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/compiler/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/compiler/_file_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/compiler/_query_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/messagebus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.670907 zettel_org-0.7.4/src/zorg/service/swog/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/swog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/swog/_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/swog/_zoq_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.670907 zettel_org-0.7.4/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.670907 zettel_org-0.7.4/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-26 14:41:34.000000 zettel_org-0.7.4/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-26 14:41:34.000000 zettel_org-0.7.4/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.674908 zettel_org-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.674908 zettel_org-0.7.4/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__snapshots__/test_run_action_open.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    62043 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__snapshots__/test_run_query.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:41:42.678907 zettel_org-0.7.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/data/order_by_file.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-26 14:41:34.000000 zettel_org-0.7.4/tox.ini
```

### Comparing `zettel_org-0.7.3/.cruft.json` & `zettel_org-0.7.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/.github/labels.yml` & `zettel_org-0.7.4/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/.github/workflows/ci.yml` & `zettel_org-0.7.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/.gitignore` & `zettel_org-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/.pylintrc` & `zettel_org-0.7.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/.readthedocs.yml` & `zettel_org-0.7.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/CHANGELOG.md` & `zettel_org-0.7.4/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,29 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.3...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.4...HEAD)
+
+
+## [0.7.4](https://github.com/bbugyi200/zorg/compare/0.7.3...0.7.4) - 2024-05-26
+
+### Added
+
+* Support for related file section to query pages.
+* Support for `f=GLOB` style file-filters in zorg queries.
+* Support for selecting files and tags using zorg queries.
+* Auto-refresh query pages when they are open (e.g. via `action open`).
+
+### Fixed
+
+* Bug which caused modify date or ZID to not show in query pages.
 
 
 ## [0.7.3](https://github.com/bbugyi200/zorg/compare/0.7.2...0.7.3) - 2024-05-17
 
 ### Added
 
 * Add support for the various new WHERE filters and new GROUP BY dimensions.
```

### Comparing `zettel_org-0.7.3/CONTRIBUTING.md` & `zettel_org-0.7.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/Dockerfile` & `zettel_org-0.7.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/Makefile` & `zettel_org-0.7.4/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/PKG-INFO` & `zettel_org-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.7.3
+Version: 0.7.4
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `zettel_org-0.7.3/README.md` & `zettel_org-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/bin/build_zorg_grammars` & `zettel_org-0.7.4/bin/build_zorg_grammars`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/bin/check_cc` & `zettel_org-0.7.4/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/bin/publish_docs` & `zettel_org-0.7.4/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/bin/quick-lints` & `zettel_org-0.7.4/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/bin/render_all_cogs` & `zettel_org-0.7.4/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/docs/Makefile` & `zettel_org-0.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/docs/make.bat` & `zettel_org-0.7.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/docs/source/conf.py` & `zettel_org-0.7.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/examples/zorg_file/20240323.zo` & `zettel_org-0.7.4/examples/zorg_file/20240323.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/examples/zorg_file/scrambled_prj_notes.zo` & `zettel_org-0.7.4/examples/zorg_file/scrambled_prj_notes.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/examples/zorg_file/subsections.zo` & `zettel_org-0.7.4/examples/zorg_file/subsections.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/lib/bugyi.sh` & `zettel_org-0.7.4/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/requirements-dev.in` & `zettel_org-0.7.4/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/requirements-dev.txt` & `zettel_org-0.7.4/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 #
 #    "make update-requirements"
 #
 -e file:.#egg=zettel-org>=0.dev
     # via -r requirements-dev.in
 alabaster==0.7.16
     # via sphinx
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 antlr4-python3-runtime==4.13.1
     # via
     #   -r requirements.in
     #   zettel-org
 antlr4-tools==0.2.1
     # via -r requirements-dev.in
 arrow==1.3.0
     # via cookiecutter
-astroid==3.2.1
+astroid==3.2.2
     # via pylint
 babel==2.15.0
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
 black==24.4.2
     # via -r requirements-dev.in
@@ -73,15 +73,15 @@
     #   cruft
     #   pip-tools
     #   typer
 cogapp==3.4.1
     # via -r requirements-dev.in
 cookiecutter==2.6.0
     # via cruft
-coverage[toml]==7.5.1
+coverage[toml]==7.5.2
     # via pytest-cov
 cruft[pyproject]==2.15.0
     # via -r requirements-dev.in
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
@@ -182,15 +182,15 @@
     # via -r requirements-dev.in
 pyflakes==3.2.0
     # via flake8
 pygments==2.18.0
     # via
     #   rich
     #   sphinx
-pylint==3.2.0
+pylint==3.2.2
     # via -r requirements-dev.in
 pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
 pytest==7.4.4
     # via
@@ -210,15 +210,15 @@
     # via pydantic-settings
 python-slugify==8.0.4
     # via cookiecutter
 pyyaml==6.0.1
     # via
     #   bolton-clack
     #   cookiecutter
-requests==2.31.0
+requests==2.32.2
     # via
     #   cookiecutter
     #   sphinx
 rich==13.7.1
     # via
     #   -r requirements.in
     #   cookiecutter
@@ -303,15 +303,15 @@
     #   zettel-org
 typer==0.12.3
     # via cruft
 types-python-dateutil==2.9.0.20240316
     # via arrow
 types-tqdm==4.66.0.20240417
     # via -r requirements-dev.in
-typing-extensions==4.11.0
+typing-extensions==4.12.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pydantic-core
     #   sqlalchemy
@@ -326,11 +326,11 @@
     # via tox
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via pip-tools
-setuptools==69.5.1
+setuptools==70.0.0
     # via
     #   pip-tools
     #   setuptools-scm
```

### Comparing `zettel_org-0.7.3/requirements.txt` & `zettel_org-0.7.4/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    "make update-requirements"
 #
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 antlr4-python3-runtime==4.13.1
     # via -r requirements.in
 bolton-clack==0.3.12
     # via -r requirements.in
 bolton-eris==0.2.3
     # via
@@ -64,14 +64,14 @@
     # via sqlmodel
 sqlmodel==0.0.18
     # via -r requirements.in
 structlog==24.1.0
     # via bolton-logrus
 tqdm==4.66.4
     # via -r requirements.in
-typing-extensions==4.11.0
+typing-extensions==4.12.0
     # via
     #   pydantic
     #   pydantic-core
     #   sqlalchemy
 vimala==0.2.0
     # via -r requirements.in
```

### Comparing `zettel_org-0.7.3/setup.cfg` & `zettel_org-0.7.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/setup.py` & `zettel_org-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.7.3"}
+USE_SCM_VERSION = {"fallback_version": "0.7.4"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `zettel_org-0.7.3/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.7.4/src/zettel_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.7.3
+Version: 0.7.4
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `zettel_org-0.7.3/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.7.4/src/zettel_org.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 examples/zorg_file/priority.zo
 examples/zorg_file/property.zo
 examples/zorg_file/scrambled_prj_notes.zo
 examples/zorg_file/subnotes.zo
 examples/zorg_file/subsections.zo
 examples/zorg_file/tags_and_ids.zo
 examples/zorg_query/all_contexts.zoq
+examples/zorg_query/desc_filter.zoq
+examples/zorg_query/file_filter.zoq
 examples/zorg_query/open_projects.zoq
 lib/bugyi.sh
 scripts/README.md
 src/zettel_org.egg-info/PKG-INFO
 src/zettel_org.egg-info/SOURCES.txt
 src/zettel_org.egg-info/dependency_links.txt
 src/zettel_org.egg-info/entry_points.txt
@@ -126,14 +128,15 @@
 src/zorg/service/zid_manager.py
 src/zorg/service/compiler/__init__.py
 src/zorg/service/compiler/_api.py
 src/zorg/service/compiler/_file_compiler.py
 src/zorg/service/compiler/_query_compiler.py
 src/zorg/service/swog/__init__.py
 src/zorg/service/swog/_executor.py
+src/zorg/service/swog/_zoq_file.py
 src/zorg/storage/__init__.py
 src/zorg/storage/sql/__init__.py
 src/zorg/storage/sql/converters.py
 src/zorg/storage/sql/engine.py
 src/zorg/storage/sql/models.py
 src/zorg/storage/sql/repo.py
 src/zorg/storage/sql/session.py
@@ -154,8 +157,9 @@
 tests/__snapshots__/test_run_edit.ambr
 tests/__snapshots__/test_run_query.ambr
 tests/__snapshots__/test_run_template.ambr
 tests/data/day_log.zot
 tests/data/done_log.zot
 tests/data/habit_log.zot
 tests/data/hello.zot
-tests/data/links.zo
+tests/data/links.zo
+tests/data/order_by_file.zoq
```

### Comparing `zettel_org-0.7.3/src/zorg/app/config.py` & `zettel_org-0.7.4/src/zorg/app/config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/app/runners/__init__.py` & `zettel_org-0.7.4/src/zorg/app/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/app/runners/_run_action.py` & `zettel_org-0.7.4/src/zorg/app/runners/_run_action.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Contains runners for the 'zorg action' command."""
 
-import datetime as dt
 from pathlib import Path
-from typing import Final, Optional
+from typing import Callable, Final, Optional
 
 from logrus import Logger
 
 from ...service import common as c, swog
 from ...service.templates import init_from_template
 from ...storage.sql.session import SQLSession
 from ..config import OpenActionConfig
@@ -28,14 +27,17 @@
     link_word_idx_map: dict[str, tuple[int, int]] = {}
     for word in zo_line.split(" "):
         left_idx = word.find("[[")
         right_idx = word.find("]]")
         if left_idx >= 0 and right_idx >= 0:
             link_word_idx_map[word] = (left_idx, right_idx)
 
+    refresh_zoq_file = _refresh_zoq_file_factory(
+        cfg.zettel_dir, cfg.database_url, cfg.verbose
+    )
     if link_word_idx_map:
         word_left_right: Optional[tuple[str, int, int]] = None
         if len(link_word_idx_map) == 1:
             word = list(link_word_idx_map.keys())[0]
             left_idx, right_idx = link_word_idx_map[word]
             word_left_right = word, left_idx, right_idx
         elif cfg.option_idx is None:
@@ -56,46 +58,44 @@
         if word_left_right is not None:
             word, left_idx, right_idx = word_left_right
             link_parts = word[left_idx + 2 : right_idx].split("::")
             link_base = link_parts[0]
             link_base = link_base if "." in link_base else f"{link_base}.zo"
             link_path = c.prepend_zdir(cfg.zettel_dir, [Path(link_base)])[0]
 
-            init_from_template(
-                cfg.zettel_dir,
-                cfg.template_pattern_map,
-                link_path,
-                var_map={
-                    "parent": (
-                        str(zo_path)
-                        .replace(".zo", "")
-                        .replace(str(cfg.zettel_dir) + "/", "")
-                    )
-                },
-            )
+            if not link_path.exists():
+                init_from_template(
+                    cfg.zettel_dir,
+                    cfg.template_pattern_map,
+                    link_path,
+                    var_map={
+                        "parent": (
+                            str(zo_path)
+                            .replace(".zo", "")
+                            .replace(str(cfg.zettel_dir) + "/", "")
+                        )
+                    },
+                )
+            elif link_path.suffix == ".zoq":
+                refresh_zoq_file(link_path)
+
             print(f"EDIT {link_path}")
             if len(link_parts) > 1:
                 print(f"SEARCH id::{link_parts[1]}")
-
     else:
-        name_sep = " | "
-        if zo_line.startswith(("# S ", "# W ")) and name_sep in zo_line:
-            query_string, query_name = zo_line.strip()[2:].split(name_sep)
-            with SQLSession(
-                cfg.zettel_dir, cfg.database_url, verbose=cfg.verbose
-            ) as session:
-                query_results = swog.execute(session, query_string)
-
-            query_path = cfg.zettel_dir / f"{query_name}.zoq"
-
-            date_spec = dt.datetime.now().strftime("%Y-%m-%d at %H:%M:%S")
-            with query_path.open("w") as f:
-                f.write(
-                    f"# {query_string} | {query_name}\n#\n# Saved query"
-                    f" generated on {date_spec}.\n\n{query_results}"
-                )
-
-            print(f"EDIT {query_path}")
+        if zo_line.startswith(("# S ", "# W ")):
+            refresh_zoq_file(zo_path)
+            print(f"EDIT {zo_path}")
         else:
             print(f"ECHO {_MSG_NOTHING_TO_OPEN} #{cfg.line_number}")
 
     return 0
+
+
+def _refresh_zoq_file_factory(
+    zdir: Path, db_url: str, verbose: int
+) -> Callable[[Path], None]:
+    def refresh_zoq_file(zoq_path: Path) -> None:
+        with SQLSession(zdir, db_url, verbose=verbose) as session:
+            swog.refresh_zoq_file(session, zoq_path)
+
+    return refresh_zoq_file
```

### Comparing `zettel_org-0.7.3/src/zorg/app/runners/_run_compile.py` & `zettel_org-0.7.4/src/zorg/app/runners/_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/app/runners/_run_db.py` & `zettel_org-0.7.4/src/zorg/app/runners/_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/app/runners/_run_edit.py` & `zettel_org-0.7.4/src/zorg/app/runners/_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/app/runners/_run_template.py` & `zettel_org-0.7.4/src/zorg/app/runners/_run_template.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/domain/messages/commands.py` & `zettel_org-0.7.4/src/zorg/domain/messages/commands.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/domain/messages/events.py` & `zettel_org-0.7.4/src/zorg/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/domain/models/_zorg_file.py` & `zettel_org-0.7.4/src/zorg/domain/models/_zorg_file.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/domain/models/_zorg_query.py` & `zettel_org-0.7.4/src/zorg/domain/models/_zorg_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 
     value: str
     case_sensitive: Optional[bool] = None
     op: DescOperator = DescOperator.CONTAINS
 
 
 @dataclass(frozen=True)
+class FileFilter:
+    """Represents a single file filter (e.g. 'f=foobar' or 'f=*baz*')."""
+
+    path_glob: str
+    negated: bool = False
+
+
+@dataclass(frozen=True)
 class PropertyFilter:
     """Represents a single property filter (e.g. 'due:<=0d' or '!recur:*')."""
 
     key: str
     value: str = ""
     op: PropertyOperator = PropertyOperator.EXISTS
     value_type: PropertyValueType = PropertyValueType.STRING
@@ -49,14 +57,15 @@
     """Tag used to filter ZorgNotes."""
 
     allowed_note_types: set[NoteType] = field(default_factory=set)
     areas: set[str] = field(default_factory=set)
     contexts: set[str] = field(default_factory=set)
     create_date_ranges: set[DateRange] = field(default_factory=set)
     desc_filters: set[DescFilter] = field(default_factory=set)
+    file_filters: set[FileFilter] = field(default_factory=set)
     modify_date_ranges: set[DateRange] = field(default_factory=set)
     or_filters: list["WhereOrFilter"] = field(default_factory=list)
     people: set[str] = field(default_factory=set)
     property_filters: set[PropertyFilter] = field(default_factory=set)
     priorities: set[TodoPriorityType] = field(default_factory=set)
     projects: set[str] = field(default_factory=set)
```

### Comparing `zettel_org-0.7.3/src/zorg/domain/types.py` & `zettel_org-0.7.4/src/zorg/domain/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,19 +231,17 @@
 def _to_comparable_note_type(todo_payload: Optional["TodoPayload"]) -> str:
     if todo_payload is None:
         return NoteType.BASIC.to_header_label()
     else:
         return todo_payload.status.to_header_label()
 
 
-def _to_comparable_priority(
-    todo_payload: Optional["TodoPayload"],
-) -> TodoPriorityType:
+def _to_comparable_priority(todo_payload: Optional["TodoPayload"]) -> str:
     if todo_payload is None:
-        return "P9"
+        return ""
     else:
         return todo_payload.priority
 
 
 def _to_comparable_file(file_path: Optional[Path]) -> str:
     assert file_path is not None
     link_name = str(file_path).replace(".zo", "")
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/CommonLexerRules.g4` & `zettel_org-0.7.4/src/zorg/grammar/CommonLexerRules.g4`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/grammar/ZorgFile.g4` & `zettel_org-0.7.4/src/zorg/grammar/ZorgFile.g4`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 context : AT_SIGN ID ;
 person  : PERCENT ID ;
 project : PLUS ID ;
 
 // quotes and links
 quoted     : (SQUOTE (atom | priority | '[[' | ']]')+ SQUOTE | DQUOTE atom+ DQUOTE) ;
 link       : '[[' id_group ']]' ;
-ref        : '[' id_group ']' ;
+ref        : '[' id_group (SPACE id_group)* ']' ;
 
 // sections
 h1_section : h1_header NL* block* (NL? h2_section)* ;
 h2_section : h2_header NL* block* (NL? h3_section)* ;
 h3_section : h3_header NL* block* (NL? h4_section)* ;
 h4_section : h4_header NL* block* ;
 h1_header  : HASH HASH HASH HASH HASH HASH HASH HASH HASH space_atoms eol ;
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files 4% similar despite different names*

```diff
@@ -136,8 +136,8 @@
 h2_header
 h3_header
 h4_header
 eol
 
 
 atn:
-[4, 1, 42, 470, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 1, 0, 1, 0, 3, 0, 99, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 104, 8, 1, 11, 1, 12, 1, 105, 1, 2, 1, 2, 3, 2, 110, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 115, 8, 3, 11, 3, 12, 3, 116, 1, 3, 5, 3, 120, 8, 3, 10, 3, 12, 3, 123, 9, 3, 1, 3, 5, 3, 126, 8, 3, 10, 3, 12, 3, 129, 9, 3, 1, 3, 5, 3, 132, 8, 3, 10, 3, 12, 3, 135, 9, 3, 1, 4, 4, 4, 138, 8, 4, 11, 4, 12, 4, 139, 1, 4, 5, 4, 143, 8, 4, 10, 4, 12, 4, 146, 9, 4, 1, 5, 1, 5, 1, 5, 1, 5, 3, 5, 152, 8, 5, 1, 6, 1, 6, 1, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 7, 5, 7, 162, 8, 7, 10, 7, 12, 7, 165, 9, 7, 1, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 4, 10, 175, 8, 10, 11, 10, 12, 10, 176, 1, 10, 5, 10, 180, 8, 10, 10, 10, 12, 10, 183, 9, 10, 1, 11, 1, 11, 1, 11, 5, 11, 188, 8, 11, 10, 11, 12, 11, 191, 9, 11, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 5, 13, 198, 8, 13, 10, 13, 12, 13, 201, 9, 13, 1, 14, 1, 14, 1, 14, 3, 14, 206, 8, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 3, 15, 215, 8, 15, 1, 16, 1, 16, 1, 16, 3, 16, 220, 8, 16, 1, 17, 1, 17, 1, 18, 4, 18, 225, 8, 18, 11, 18, 12, 18, 226, 1, 19, 1, 19, 1, 19, 3, 19, 232, 8, 19, 1, 19, 1, 19, 5, 19, 236, 8, 19, 10, 19, 12, 19, 239, 9, 19, 1, 19, 1, 19, 3, 19, 243, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 248, 8, 19, 10, 19, 12, 19, 251, 9, 19, 3, 19, 253, 8, 19, 1, 19, 3, 19, 256, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 265, 8, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 4, 23, 276, 8, 23, 11, 23, 12, 23, 277, 1, 23, 1, 23, 5, 23, 282, 8, 23, 10, 23, 12, 23, 285, 9, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 3, 24, 296, 8, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 3, 27, 309, 8, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 31, 3, 31, 321, 8, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 4, 36, 340, 8, 36, 11, 36, 12, 36, 341, 1, 36, 1, 36, 1, 36, 4, 36, 347, 8, 36, 11, 36, 12, 36, 348, 1, 36, 1, 36, 3, 36, 353, 8, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 1, 38, 1, 39, 1, 39, 5, 39, 365, 8, 39, 10, 39, 12, 39, 368, 9, 39, 1, 39, 5, 39, 371, 8, 39, 10, 39, 12, 39, 374, 9, 39, 1, 39, 3, 39, 377, 8, 39, 1, 39, 5, 39, 380, 8, 39, 10, 39, 12, 39, 383, 9, 39, 1, 40, 1, 40, 5, 40, 387, 8, 40, 10, 40, 12, 40, 390, 9, 40, 1, 40, 5, 40, 393, 8, 40, 10, 40, 12, 40, 396, 9, 40, 1, 40, 3, 40, 399, 8, 40, 1, 40, 5, 40, 402, 8, 40, 10, 40, 12, 40, 405, 9, 40, 1, 41, 1, 41, 5, 41, 409, 8, 41, 10, 41, 12, 41, 412, 9, 41, 1, 41, 5, 41, 415, 8, 41, 10, 41, 12, 41, 418, 9, 41, 1, 41, 3, 41, 421, 8, 41, 1, 41, 5, 41, 424, 8, 41, 10, 41, 12, 41, 427, 9, 41, 1, 42, 1, 42, 5, 42, 431, 8, 42, 10, 42, 12, 42, 434, 9, 42, 1, 42, 5, 42, 437, 8, 42, 10, 42, 12, 42, 440, 9, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 47, 1, 47, 1, 47, 0, 0, 48, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 0, 5, 2, 0, 9, 9, 38, 38, 4, 0, 22, 22, 28, 28, 30, 31, 38, 41, 2, 0, 25, 27, 42, 42, 1, 0, 32, 35, 1, 1, 7, 7, 498, 0, 96, 1, 0, 0, 0, 2, 103, 1, 0, 0, 0, 4, 107, 1, 0, 0, 0, 6, 114, 1, 0, 0, 0, 8, 137, 1, 0, 0, 0, 10, 151, 1, 0, 0, 0, 12, 153, 1, 0, 0, 0, 14, 158, 1, 0, 0, 0, 16, 166, 1, 0, 0, 0, 18, 169, 1, 0, 0, 0, 20, 171, 1, 0, 0, 0, 22, 184, 1, 0, 0, 0, 24, 192, 1, 0, 0, 0, 26, 195, 1, 0, 0, 0, 28, 202, 1, 0, 0, 0, 30, 214, 1, 0, 0, 0, 32, 216, 1, 0, 0, 0, 34, 221, 1, 0, 0, 0, 36, 224, 1, 0, 0, 0, 38, 228, 1, 0, 0, 0, 40, 264, 1, 0, 0, 0, 42, 266, 1, 0, 0, 0, 44, 268, 1, 0, 0, 0, 46, 273, 1, 0, 0, 0, 48, 295, 1, 0, 0, 0, 50, 297, 1, 0, 0, 0, 52, 299, 1, 0, 0, 0, 54, 308, 1, 0, 0, 0, 56, 310, 1, 0, 0, 0, 58, 312, 1, 0, 0, 0, 60, 314, 1, 0, 0, 0, 62, 320, 1, 0, 0, 0, 64, 322, 1, 0, 0, 0, 66, 325, 1, 0, 0, 0, 68, 328, 1, 0, 0, 0, 70, 331, 1, 0, 0, 0, 72, 352, 1, 0, 0, 0, 74, 354, 1, 0, 0, 0, 76, 358, 1, 0, 0, 0, 78, 362, 1, 0, 0, 0, 80, 384, 1, 0, 0, 0, 82, 406, 1, 0, 0, 0, 84, 428, 1, 0, 0, 0, 86, 441, 1, 0, 0, 0, 88, 453, 1, 0, 0, 0, 90, 457, 1, 0, 0, 0, 92, 461, 1, 0, 0, 0, 94, 467, 1, 0, 0, 0, 96, 98, 3, 2, 1, 0, 97, 99, 3, 6, 3, 0, 98, 97, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 100, 1, 0, 0, 0, 100, 101, 5, 0, 0, 1, 101, 1, 1, 0, 0, 0, 102, 104, 3, 4, 2, 0, 103, 102, 1, 0, 0, 0, 104, 105, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 105, 106, 1, 0, 0, 0, 106, 3, 1, 0, 0, 0, 107, 109, 5, 32, 0, 0, 108, 110, 3, 36, 18, 0, 109, 108, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 111, 1, 0, 0, 0, 111, 112, 5, 7, 0, 0, 112, 5, 1, 0, 0, 0, 113, 115, 5, 7, 0, 0, 114, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 114, 1, 0, 0, 0, 116, 117, 1, 0, 0, 0, 117, 121, 1, 0, 0, 0, 118, 120, 3, 8, 4, 0, 119, 118, 1, 0, 0, 0, 120, 123, 1, 0, 0, 0, 121, 119, 1, 0, 0, 0, 121, 122, 1, 0, 0, 0, 122, 127, 1, 0, 0, 0, 123, 121, 1, 0, 0, 0, 124, 126, 3, 80, 40, 0, 125, 124, 1, 0, 0, 0, 126, 129, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 127, 128, 1, 0, 0, 0, 128, 133, 1, 0, 0, 0, 129, 127, 1, 0, 0, 0, 130, 132, 3, 78, 39, 0, 131, 130, 1, 0, 0, 0, 132, 135, 1, 0, 0, 0, 133, 131, 1, 0, 0, 0, 133, 134, 1, 0, 0, 0, 134, 7, 1, 0, 0, 0, 135, 133, 1, 0, 0, 0, 136, 138, 3, 10, 5, 0, 137, 136, 1, 0, 0, 0, 138, 139, 1, 0, 0, 0, 139, 137, 1, 0, 0, 0, 139, 140, 1, 0, 0, 0, 140, 144, 1, 0, 0, 0, 141, 143, 5, 7, 0, 0, 142, 141, 1, 0, 0, 0, 143, 146, 1, 0, 0, 0, 144, 142, 1, 0, 0, 0, 144, 145, 1, 0, 0, 0, 145, 9, 1, 0, 0, 0, 146, 144, 1, 0, 0, 0, 147, 152, 3, 26, 13, 0, 148, 152, 3, 14, 7, 0, 149, 152, 3, 12, 6, 0, 150, 152, 3, 4, 2, 0, 151, 147, 1, 0, 0, 0, 151, 148, 1, 0, 0, 0, 151, 149, 1, 0, 0, 0, 151, 150, 1, 0, 0, 0, 152, 11, 1, 0, 0, 0, 153, 154, 3, 76, 38, 0, 154, 155, 5, 42, 0, 0, 155, 156, 3, 36, 18, 0, 156, 157, 5, 7, 0, 0, 157, 13, 1, 0, 0, 0, 158, 159, 5, 25, 0, 0, 159, 163, 3, 16, 8, 0, 160, 162, 3, 22, 11, 0, 161, 160, 1, 0, 0, 0, 162, 165, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 163, 164, 1, 0, 0, 0, 164, 15, 1, 0, 0, 0, 165, 163, 1, 0, 0, 0, 166, 167, 3, 18, 9, 0, 167, 168, 5, 7, 0, 0, 168, 17, 1, 0, 0, 0, 169, 170, 3, 20, 10, 0, 170, 19, 1, 0, 0, 0, 171, 181, 3, 36, 18, 0, 172, 174, 5, 7, 0, 0, 173, 175, 5, 29, 0, 0, 174, 173, 1, 0, 0, 0, 175, 176, 1, 0, 0, 0, 176, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 180, 3, 36, 18, 0, 179, 172, 1, 0, 0, 0, 180, 183, 1, 0, 0, 0, 181, 179, 1, 0, 0, 0, 181, 182, 1, 0, 0, 0, 182, 21, 1, 0, 0, 0, 183, 181, 1, 0, 0, 0, 184, 185, 5, 20, 0, 0, 185, 189, 3, 16, 8, 0, 186, 188, 3, 24, 12, 0, 187, 186, 1, 0, 0, 0, 188, 191, 1, 0, 0, 0, 189, 187, 1, 0, 0, 0, 189, 190, 1, 0, 0, 0, 190, 23, 1, 0, 0, 0, 191, 189, 1, 0, 0, 0, 192, 193, 5, 21, 0, 0, 193, 194, 3, 16, 8, 0, 194, 25, 1, 0, 0, 0, 195, 199, 3, 28, 14, 0, 196, 198, 3, 22, 11, 0, 197, 196, 1, 0, 0, 0, 198, 201, 1, 0, 0, 0, 199, 197, 1, 0, 0, 0, 199, 200, 1, 0, 0, 0, 200, 27, 1, 0, 0, 0, 201, 199, 1, 0, 0, 0, 202, 205, 3, 30, 15, 0, 203, 204, 5, 29, 0, 0, 204, 206, 3, 34, 17, 0, 205, 203, 1, 0, 0, 0, 205, 206, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 3, 18, 9, 0, 208, 209, 5, 7, 0, 0, 209, 29, 1, 0, 0, 0, 210, 215, 5, 8, 0, 0, 211, 215, 3, 32, 16, 0, 212, 215, 5, 40, 0, 0, 213, 215, 5, 41, 0, 0, 214, 210, 1, 0, 0, 0, 214, 211, 1, 0, 0, 0, 214, 212, 1, 0, 0, 0, 214, 213, 1, 0, 0, 0, 215, 31, 1, 0, 0, 0, 216, 219, 7, 0, 0, 0, 217, 218, 5, 42, 0, 0, 218, 220, 3, 52, 26, 0, 219, 217, 1, 0, 0, 0, 219, 220, 1, 0, 0, 0, 220, 33, 1, 0, 0, 0, 221, 222, 5, 15, 0, 0, 222, 35, 1, 0, 0, 0, 223, 225, 3, 38, 19, 0, 224, 223, 1, 0, 0, 0, 225, 226, 1, 0, 0, 0, 226, 224, 1, 0, 0, 0, 226, 227, 1, 0, 0, 0, 227, 37, 1, 0, 0, 0, 228, 231, 5, 29, 0, 0, 229, 230, 5, 36, 0, 0, 230, 232, 3, 56, 28, 0, 231, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 237, 1, 0, 0, 0, 233, 236, 3, 56, 28, 0, 234, 236, 5, 37, 0, 0, 235, 233, 1, 0, 0, 0, 235, 234, 1, 0, 0, 0, 236, 239, 1, 0, 0, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 242, 1, 0, 0, 0, 239, 237, 1, 0, 0, 0, 240, 243, 3, 40, 20, 0, 241, 243, 3, 72, 36, 0, 242, 240, 1, 0, 0, 0, 242, 241, 1, 0, 0, 0, 242, 243, 1, 0, 0, 0, 243, 252, 1, 0, 0, 0, 244, 249, 3, 54, 27, 0, 245, 248, 3, 54, 27, 0, 246, 248, 3, 48, 24, 0, 247, 245, 1, 0, 0, 0, 247, 246, 1, 0, 0, 0, 248, 251, 1, 0, 0, 0, 249, 247, 1, 0, 0, 0, 249, 250, 1, 0, 0, 0, 250, 253, 1, 0, 0, 0, 251, 249, 1, 0, 0, 0, 252, 244, 1, 0, 0, 0, 252, 253, 1, 0, 0, 0, 253, 255, 1, 0, 0, 0, 254, 256, 3, 76, 38, 0, 255, 254, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 39, 1, 0, 0, 0, 257, 265, 3, 60, 30, 0, 258, 265, 3, 62, 31, 0, 259, 265, 3, 74, 37, 0, 260, 265, 3, 44, 22, 0, 261, 265, 3, 46, 23, 0, 262, 265, 3, 76, 38, 0, 263, 265, 3, 34, 17, 0, 264, 257, 1, 0, 0, 0, 264, 258, 1, 0, 0, 0, 264, 259, 1, 0, 0, 0, 264, 260, 1, 0, 0, 0, 264, 261, 1, 0, 0, 0, 264, 262, 1, 0, 0, 0, 264, 263, 1, 0, 0, 0, 265, 41, 1, 0, 0, 0, 266, 267, 5, 17, 0, 0, 267, 43, 1, 0, 0, 0, 268, 269, 5, 16, 0, 0, 269, 270, 5, 42, 0, 0, 270, 271, 5, 42, 0, 0, 271, 272, 3, 46, 23, 0, 272, 45, 1, 0, 0, 0, 273, 283, 3, 48, 24, 0, 274, 276, 3, 58, 29, 0, 275, 274, 1, 0, 0, 0, 276, 277, 1, 0, 0, 0, 277, 275, 1, 0, 0, 0, 277, 278, 1, 0, 0, 0, 278, 279, 1, 0, 0, 0, 279, 280, 3, 48, 24, 0, 280, 282, 1, 0, 0, 0, 281, 275, 1, 0, 0, 0, 282, 285, 1, 0, 0, 0, 283, 281, 1, 0, 0, 0, 283, 284, 1, 0, 0, 0, 284, 47, 1, 0, 0, 0, 285, 283, 1, 0, 0, 0, 286, 296, 5, 16, 0, 0, 287, 296, 5, 19, 0, 0, 288, 296, 5, 14, 0, 0, 289, 296, 5, 15, 0, 0, 290, 296, 3, 50, 25, 0, 291, 296, 3, 52, 26, 0, 292, 296, 3, 42, 21, 0, 293, 296, 5, 8, 0, 0, 294, 296, 5, 9, 0, 0, 295, 286, 1, 0, 0, 0, 295, 287, 1, 0, 0, 0, 295, 288, 1, 0, 0, 0, 295, 289, 1, 0, 0, 0, 295, 290, 1, 0, 0, 0, 295, 291, 1, 0, 0, 0, 295, 292, 1, 0, 0, 0, 295, 293, 1, 0, 0, 0, 295, 294, 1, 0, 0, 0, 296, 49, 1, 0, 0, 0, 297, 298, 5, 10, 0, 0, 298, 51, 1, 0, 0, 0, 299, 300, 5, 11, 0, 0, 300, 53, 1, 0, 0, 0, 301, 309, 5, 36, 0, 0, 302, 309, 5, 37, 0, 0, 303, 309, 5, 24, 0, 0, 304, 309, 5, 23, 0, 0, 305, 309, 3, 56, 28, 0, 306, 309, 3, 60, 30, 0, 307, 309, 3, 58, 29, 0, 308, 301, 1, 0, 0, 0, 308, 302, 1, 0, 0, 0, 308, 303, 1, 0, 0, 0, 308, 304, 1, 0, 0, 0, 308, 305, 1, 0, 0, 0, 308, 306, 1, 0, 0, 0, 308, 307, 1, 0, 0, 0, 309, 55, 1, 0, 0, 0, 310, 311, 7, 1, 0, 0, 311, 57, 1, 0, 0, 0, 312, 313, 7, 2, 0, 0, 313, 59, 1, 0, 0, 0, 314, 315, 7, 3, 0, 0, 315, 61, 1, 0, 0, 0, 316, 321, 3, 64, 32, 0, 317, 321, 3, 66, 33, 0, 318, 321, 3, 68, 34, 0, 319, 321, 3, 70, 35, 0, 320, 316, 1, 0, 0, 0, 320, 317, 1, 0, 0, 0, 320, 318, 1, 0, 0, 0, 320, 319, 1, 0, 0, 0, 321, 63, 1, 0, 0, 0, 322, 323, 5, 32, 0, 0, 323, 324, 5, 16, 0, 0, 324, 65, 1, 0, 0, 0, 325, 326, 5, 33, 0, 0, 326, 327, 5, 16, 0, 0, 327, 67, 1, 0, 0, 0, 328, 329, 5, 35, 0, 0, 329, 330, 5, 16, 0, 0, 330, 69, 1, 0, 0, 0, 331, 332, 5, 34, 0, 0, 332, 333, 5, 16, 0, 0, 333, 71, 1, 0, 0, 0, 334, 339, 5, 36, 0, 0, 335, 340, 3, 40, 20, 0, 336, 340, 3, 34, 17, 0, 337, 340, 5, 1, 0, 0, 338, 340, 5, 2, 0, 0, 339, 335, 1, 0, 0, 0, 339, 336, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 338, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 339, 1, 0, 0, 0, 341, 342, 1, 0, 0, 0, 342, 343, 1, 0, 0, 0, 343, 353, 5, 36, 0, 0, 344, 346, 5, 37, 0, 0, 345, 347, 3, 40, 20, 0, 346, 345, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 346, 1, 0, 0, 0, 348, 349, 1, 0, 0, 0, 349, 350, 1, 0, 0, 0, 350, 351, 5, 37, 0, 0, 351, 353, 1, 0, 0, 0, 352, 334, 1, 0, 0, 0, 352, 344, 1, 0, 0, 0, 353, 73, 1, 0, 0, 0, 354, 355, 5, 1, 0, 0, 355, 356, 3, 46, 23, 0, 356, 357, 5, 2, 0, 0, 357, 75, 1, 0, 0, 0, 358, 359, 5, 3, 0, 0, 359, 360, 3, 46, 23, 0, 360, 361, 5, 4, 0, 0, 361, 77, 1, 0, 0, 0, 362, 366, 3, 86, 43, 0, 363, 365, 5, 7, 0, 0, 364, 363, 1, 0, 0, 0, 365, 368, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 366, 367, 1, 0, 0, 0, 367, 372, 1, 0, 0, 0, 368, 366, 1, 0, 0, 0, 369, 371, 3, 8, 4, 0, 370, 369, 1, 0, 0, 0, 371, 374, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 372, 373, 1, 0, 0, 0, 373, 381, 1, 0, 0, 0, 374, 372, 1, 0, 0, 0, 375, 377, 5, 7, 0, 0, 376, 375, 1, 0, 0, 0, 376, 377, 1, 0, 0, 0, 377, 378, 1, 0, 0, 0, 378, 380, 3, 80, 40, 0, 379, 376, 1, 0, 0, 0, 380, 383, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 381, 382, 1, 0, 0, 0, 382, 79, 1, 0, 0, 0, 383, 381, 1, 0, 0, 0, 384, 388, 3, 88, 44, 0, 385, 387, 5, 7, 0, 0, 386, 385, 1, 0, 0, 0, 387, 390, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 388, 389, 1, 0, 0, 0, 389, 394, 1, 0, 0, 0, 390, 388, 1, 0, 0, 0, 391, 393, 3, 8, 4, 0, 392, 391, 1, 0, 0, 0, 393, 396, 1, 0, 0, 0, 394, 392, 1, 0, 0, 0, 394, 395, 1, 0, 0, 0, 395, 403, 1, 0, 0, 0, 396, 394, 1, 0, 0, 0, 397, 399, 5, 7, 0, 0, 398, 397, 1, 0, 0, 0, 398, 399, 1, 0, 0, 0, 399, 400, 1, 0, 0, 0, 400, 402, 3, 82, 41, 0, 401, 398, 1, 0, 0, 0, 402, 405, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 403, 404, 1, 0, 0, 0, 404, 81, 1, 0, 0, 0, 405, 403, 1, 0, 0, 0, 406, 410, 3, 90, 45, 0, 407, 409, 5, 7, 0, 0, 408, 407, 1, 0, 0, 0, 409, 412, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 410, 411, 1, 0, 0, 0, 411, 416, 1, 0, 0, 0, 412, 410, 1, 0, 0, 0, 413, 415, 3, 8, 4, 0, 414, 413, 1, 0, 0, 0, 415, 418, 1, 0, 0, 0, 416, 414, 1, 0, 0, 0, 416, 417, 1, 0, 0, 0, 417, 425, 1, 0, 0, 0, 418, 416, 1, 0, 0, 0, 419, 421, 5, 7, 0, 0, 420, 419, 1, 0, 0, 0, 420, 421, 1, 0, 0, 0, 421, 422, 1, 0, 0, 0, 422, 424, 3, 84, 42, 0, 423, 420, 1, 0, 0, 0, 424, 427, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 425, 426, 1, 0, 0, 0, 426, 83, 1, 0, 0, 0, 427, 425, 1, 0, 0, 0, 428, 432, 3, 92, 46, 0, 429, 431, 5, 7, 0, 0, 430, 429, 1, 0, 0, 0, 431, 434, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 432, 433, 1, 0, 0, 0, 433, 438, 1, 0, 0, 0, 434, 432, 1, 0, 0, 0, 435, 437, 3, 8, 4, 0, 436, 435, 1, 0, 0, 0, 437, 440, 1, 0, 0, 0, 438, 436, 1, 0, 0, 0, 438, 439, 1, 0, 0, 0, 439, 85, 1, 0, 0, 0, 440, 438, 1, 0, 0, 0, 441, 442, 5, 32, 0, 0, 442, 443, 5, 32, 0, 0, 443, 444, 5, 32, 0, 0, 444, 445, 5, 32, 0, 0, 445, 446, 5, 32, 0, 0, 446, 447, 5, 32, 0, 0, 447, 448, 5, 32, 0, 0, 448, 449, 5, 32, 0, 0, 449, 450, 5, 32, 0, 0, 450, 451, 3, 36, 18, 0, 451, 452, 3, 94, 47, 0, 452, 87, 1, 0, 0, 0, 453, 454, 5, 5, 0, 0, 454, 455, 3, 36, 18, 0, 455, 456, 3, 94, 47, 0, 456, 89, 1, 0, 0, 0, 457, 458, 5, 6, 0, 0, 458, 459, 3, 36, 18, 0, 459, 460, 3, 94, 47, 0, 460, 91, 1, 0, 0, 0, 461, 462, 5, 25, 0, 0, 462, 463, 5, 25, 0, 0, 463, 464, 5, 25, 0, 0, 464, 465, 3, 36, 18, 0, 465, 466, 3, 94, 47, 0, 466, 93, 1, 0, 0, 0, 467, 468, 7, 4, 0, 0, 468, 95, 1, 0, 0, 0, 51, 98, 105, 109, 116, 121, 127, 133, 139, 144, 151, 163, 176, 181, 189, 199, 205, 214, 219, 226, 231, 235, 237, 242, 247, 249, 252, 255, 264, 277, 283, 295, 308, 320, 339, 341, 348, 352, 366, 372, 376, 381, 388, 394, 398, 403, 410, 416, 420, 425, 432, 438]
+[4, 1, 42, 477, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 1, 0, 1, 0, 3, 0, 99, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 104, 8, 1, 11, 1, 12, 1, 105, 1, 2, 1, 2, 3, 2, 110, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 115, 8, 3, 11, 3, 12, 3, 116, 1, 3, 5, 3, 120, 8, 3, 10, 3, 12, 3, 123, 9, 3, 1, 3, 5, 3, 126, 8, 3, 10, 3, 12, 3, 129, 9, 3, 1, 3, 5, 3, 132, 8, 3, 10, 3, 12, 3, 135, 9, 3, 1, 4, 4, 4, 138, 8, 4, 11, 4, 12, 4, 139, 1, 4, 5, 4, 143, 8, 4, 10, 4, 12, 4, 146, 9, 4, 1, 5, 1, 5, 1, 5, 1, 5, 3, 5, 152, 8, 5, 1, 6, 1, 6, 1, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 7, 5, 7, 162, 8, 7, 10, 7, 12, 7, 165, 9, 7, 1, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 4, 10, 175, 8, 10, 11, 10, 12, 10, 176, 1, 10, 5, 10, 180, 8, 10, 10, 10, 12, 10, 183, 9, 10, 1, 11, 1, 11, 1, 11, 5, 11, 188, 8, 11, 10, 11, 12, 11, 191, 9, 11, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 5, 13, 198, 8, 13, 10, 13, 12, 13, 201, 9, 13, 1, 14, 1, 14, 1, 14, 3, 14, 206, 8, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 3, 15, 215, 8, 15, 1, 16, 1, 16, 1, 16, 3, 16, 220, 8, 16, 1, 17, 1, 17, 1, 18, 4, 18, 225, 8, 18, 11, 18, 12, 18, 226, 1, 19, 1, 19, 1, 19, 3, 19, 232, 8, 19, 1, 19, 1, 19, 5, 19, 236, 8, 19, 10, 19, 12, 19, 239, 9, 19, 1, 19, 1, 19, 3, 19, 243, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 248, 8, 19, 10, 19, 12, 19, 251, 9, 19, 3, 19, 253, 8, 19, 1, 19, 3, 19, 256, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 265, 8, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 4, 23, 276, 8, 23, 11, 23, 12, 23, 277, 1, 23, 1, 23, 5, 23, 282, 8, 23, 10, 23, 12, 23, 285, 9, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 3, 24, 296, 8, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 3, 27, 309, 8, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 31, 3, 31, 321, 8, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 4, 36, 340, 8, 36, 11, 36, 12, 36, 341, 1, 36, 1, 36, 1, 36, 4, 36, 347, 8, 36, 11, 36, 12, 36, 348, 1, 36, 1, 36, 3, 36, 353, 8, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 1, 38, 5, 38, 363, 8, 38, 10, 38, 12, 38, 366, 9, 38, 1, 38, 1, 38, 1, 39, 1, 39, 5, 39, 372, 8, 39, 10, 39, 12, 39, 375, 9, 39, 1, 39, 5, 39, 378, 8, 39, 10, 39, 12, 39, 381, 9, 39, 1, 39, 3, 39, 384, 8, 39, 1, 39, 5, 39, 387, 8, 39, 10, 39, 12, 39, 390, 9, 39, 1, 40, 1, 40, 5, 40, 394, 8, 40, 10, 40, 12, 40, 397, 9, 40, 1, 40, 5, 40, 400, 8, 40, 10, 40, 12, 40, 403, 9, 40, 1, 40, 3, 40, 406, 8, 40, 1, 40, 5, 40, 409, 8, 40, 10, 40, 12, 40, 412, 9, 40, 1, 41, 1, 41, 5, 41, 416, 8, 41, 10, 41, 12, 41, 419, 9, 41, 1, 41, 5, 41, 422, 8, 41, 10, 41, 12, 41, 425, 9, 41, 1, 41, 3, 41, 428, 8, 41, 1, 41, 5, 41, 431, 8, 41, 10, 41, 12, 41, 434, 9, 41, 1, 42, 1, 42, 5, 42, 438, 8, 42, 10, 42, 12, 42, 441, 9, 42, 1, 42, 5, 42, 444, 8, 42, 10, 42, 12, 42, 447, 9, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 47, 1, 47, 1, 47, 0, 0, 48, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 0, 5, 2, 0, 9, 9, 38, 38, 4, 0, 22, 22, 28, 28, 30, 31, 38, 41, 2, 0, 25, 27, 42, 42, 1, 0, 32, 35, 1, 1, 7, 7, 506, 0, 96, 1, 0, 0, 0, 2, 103, 1, 0, 0, 0, 4, 107, 1, 0, 0, 0, 6, 114, 1, 0, 0, 0, 8, 137, 1, 0, 0, 0, 10, 151, 1, 0, 0, 0, 12, 153, 1, 0, 0, 0, 14, 158, 1, 0, 0, 0, 16, 166, 1, 0, 0, 0, 18, 169, 1, 0, 0, 0, 20, 171, 1, 0, 0, 0, 22, 184, 1, 0, 0, 0, 24, 192, 1, 0, 0, 0, 26, 195, 1, 0, 0, 0, 28, 202, 1, 0, 0, 0, 30, 214, 1, 0, 0, 0, 32, 216, 1, 0, 0, 0, 34, 221, 1, 0, 0, 0, 36, 224, 1, 0, 0, 0, 38, 228, 1, 0, 0, 0, 40, 264, 1, 0, 0, 0, 42, 266, 1, 0, 0, 0, 44, 268, 1, 0, 0, 0, 46, 273, 1, 0, 0, 0, 48, 295, 1, 0, 0, 0, 50, 297, 1, 0, 0, 0, 52, 299, 1, 0, 0, 0, 54, 308, 1, 0, 0, 0, 56, 310, 1, 0, 0, 0, 58, 312, 1, 0, 0, 0, 60, 314, 1, 0, 0, 0, 62, 320, 1, 0, 0, 0, 64, 322, 1, 0, 0, 0, 66, 325, 1, 0, 0, 0, 68, 328, 1, 0, 0, 0, 70, 331, 1, 0, 0, 0, 72, 352, 1, 0, 0, 0, 74, 354, 1, 0, 0, 0, 76, 358, 1, 0, 0, 0, 78, 369, 1, 0, 0, 0, 80, 391, 1, 0, 0, 0, 82, 413, 1, 0, 0, 0, 84, 435, 1, 0, 0, 0, 86, 448, 1, 0, 0, 0, 88, 460, 1, 0, 0, 0, 90, 464, 1, 0, 0, 0, 92, 468, 1, 0, 0, 0, 94, 474, 1, 0, 0, 0, 96, 98, 3, 2, 1, 0, 97, 99, 3, 6, 3, 0, 98, 97, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 100, 1, 0, 0, 0, 100, 101, 5, 0, 0, 1, 101, 1, 1, 0, 0, 0, 102, 104, 3, 4, 2, 0, 103, 102, 1, 0, 0, 0, 104, 105, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 105, 106, 1, 0, 0, 0, 106, 3, 1, 0, 0, 0, 107, 109, 5, 32, 0, 0, 108, 110, 3, 36, 18, 0, 109, 108, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 111, 1, 0, 0, 0, 111, 112, 5, 7, 0, 0, 112, 5, 1, 0, 0, 0, 113, 115, 5, 7, 0, 0, 114, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 114, 1, 0, 0, 0, 116, 117, 1, 0, 0, 0, 117, 121, 1, 0, 0, 0, 118, 120, 3, 8, 4, 0, 119, 118, 1, 0, 0, 0, 120, 123, 1, 0, 0, 0, 121, 119, 1, 0, 0, 0, 121, 122, 1, 0, 0, 0, 122, 127, 1, 0, 0, 0, 123, 121, 1, 0, 0, 0, 124, 126, 3, 80, 40, 0, 125, 124, 1, 0, 0, 0, 126, 129, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 127, 128, 1, 0, 0, 0, 128, 133, 1, 0, 0, 0, 129, 127, 1, 0, 0, 0, 130, 132, 3, 78, 39, 0, 131, 130, 1, 0, 0, 0, 132, 135, 1, 0, 0, 0, 133, 131, 1, 0, 0, 0, 133, 134, 1, 0, 0, 0, 134, 7, 1, 0, 0, 0, 135, 133, 1, 0, 0, 0, 136, 138, 3, 10, 5, 0, 137, 136, 1, 0, 0, 0, 138, 139, 1, 0, 0, 0, 139, 137, 1, 0, 0, 0, 139, 140, 1, 0, 0, 0, 140, 144, 1, 0, 0, 0, 141, 143, 5, 7, 0, 0, 142, 141, 1, 0, 0, 0, 143, 146, 1, 0, 0, 0, 144, 142, 1, 0, 0, 0, 144, 145, 1, 0, 0, 0, 145, 9, 1, 0, 0, 0, 146, 144, 1, 0, 0, 0, 147, 152, 3, 26, 13, 0, 148, 152, 3, 14, 7, 0, 149, 152, 3, 12, 6, 0, 150, 152, 3, 4, 2, 0, 151, 147, 1, 0, 0, 0, 151, 148, 1, 0, 0, 0, 151, 149, 1, 0, 0, 0, 151, 150, 1, 0, 0, 0, 152, 11, 1, 0, 0, 0, 153, 154, 3, 76, 38, 0, 154, 155, 5, 42, 0, 0, 155, 156, 3, 36, 18, 0, 156, 157, 5, 7, 0, 0, 157, 13, 1, 0, 0, 0, 158, 159, 5, 25, 0, 0, 159, 163, 3, 16, 8, 0, 160, 162, 3, 22, 11, 0, 161, 160, 1, 0, 0, 0, 162, 165, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 163, 164, 1, 0, 0, 0, 164, 15, 1, 0, 0, 0, 165, 163, 1, 0, 0, 0, 166, 167, 3, 18, 9, 0, 167, 168, 5, 7, 0, 0, 168, 17, 1, 0, 0, 0, 169, 170, 3, 20, 10, 0, 170, 19, 1, 0, 0, 0, 171, 181, 3, 36, 18, 0, 172, 174, 5, 7, 0, 0, 173, 175, 5, 29, 0, 0, 174, 173, 1, 0, 0, 0, 175, 176, 1, 0, 0, 0, 176, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 180, 3, 36, 18, 0, 179, 172, 1, 0, 0, 0, 180, 183, 1, 0, 0, 0, 181, 179, 1, 0, 0, 0, 181, 182, 1, 0, 0, 0, 182, 21, 1, 0, 0, 0, 183, 181, 1, 0, 0, 0, 184, 185, 5, 20, 0, 0, 185, 189, 3, 16, 8, 0, 186, 188, 3, 24, 12, 0, 187, 186, 1, 0, 0, 0, 188, 191, 1, 0, 0, 0, 189, 187, 1, 0, 0, 0, 189, 190, 1, 0, 0, 0, 190, 23, 1, 0, 0, 0, 191, 189, 1, 0, 0, 0, 192, 193, 5, 21, 0, 0, 193, 194, 3, 16, 8, 0, 194, 25, 1, 0, 0, 0, 195, 199, 3, 28, 14, 0, 196, 198, 3, 22, 11, 0, 197, 196, 1, 0, 0, 0, 198, 201, 1, 0, 0, 0, 199, 197, 1, 0, 0, 0, 199, 200, 1, 0, 0, 0, 200, 27, 1, 0, 0, 0, 201, 199, 1, 0, 0, 0, 202, 205, 3, 30, 15, 0, 203, 204, 5, 29, 0, 0, 204, 206, 3, 34, 17, 0, 205, 203, 1, 0, 0, 0, 205, 206, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 3, 18, 9, 0, 208, 209, 5, 7, 0, 0, 209, 29, 1, 0, 0, 0, 210, 215, 5, 8, 0, 0, 211, 215, 3, 32, 16, 0, 212, 215, 5, 40, 0, 0, 213, 215, 5, 41, 0, 0, 214, 210, 1, 0, 0, 0, 214, 211, 1, 0, 0, 0, 214, 212, 1, 0, 0, 0, 214, 213, 1, 0, 0, 0, 215, 31, 1, 0, 0, 0, 216, 219, 7, 0, 0, 0, 217, 218, 5, 42, 0, 0, 218, 220, 3, 52, 26, 0, 219, 217, 1, 0, 0, 0, 219, 220, 1, 0, 0, 0, 220, 33, 1, 0, 0, 0, 221, 222, 5, 15, 0, 0, 222, 35, 1, 0, 0, 0, 223, 225, 3, 38, 19, 0, 224, 223, 1, 0, 0, 0, 225, 226, 1, 0, 0, 0, 226, 224, 1, 0, 0, 0, 226, 227, 1, 0, 0, 0, 227, 37, 1, 0, 0, 0, 228, 231, 5, 29, 0, 0, 229, 230, 5, 36, 0, 0, 230, 232, 3, 56, 28, 0, 231, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 237, 1, 0, 0, 0, 233, 236, 3, 56, 28, 0, 234, 236, 5, 37, 0, 0, 235, 233, 1, 0, 0, 0, 235, 234, 1, 0, 0, 0, 236, 239, 1, 0, 0, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 242, 1, 0, 0, 0, 239, 237, 1, 0, 0, 0, 240, 243, 3, 40, 20, 0, 241, 243, 3, 72, 36, 0, 242, 240, 1, 0, 0, 0, 242, 241, 1, 0, 0, 0, 242, 243, 1, 0, 0, 0, 243, 252, 1, 0, 0, 0, 244, 249, 3, 54, 27, 0, 245, 248, 3, 54, 27, 0, 246, 248, 3, 48, 24, 0, 247, 245, 1, 0, 0, 0, 247, 246, 1, 0, 0, 0, 248, 251, 1, 0, 0, 0, 249, 247, 1, 0, 0, 0, 249, 250, 1, 0, 0, 0, 250, 253, 1, 0, 0, 0, 251, 249, 1, 0, 0, 0, 252, 244, 1, 0, 0, 0, 252, 253, 1, 0, 0, 0, 253, 255, 1, 0, 0, 0, 254, 256, 3, 76, 38, 0, 255, 254, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 39, 1, 0, 0, 0, 257, 265, 3, 60, 30, 0, 258, 265, 3, 62, 31, 0, 259, 265, 3, 74, 37, 0, 260, 265, 3, 44, 22, 0, 261, 265, 3, 46, 23, 0, 262, 265, 3, 76, 38, 0, 263, 265, 3, 34, 17, 0, 264, 257, 1, 0, 0, 0, 264, 258, 1, 0, 0, 0, 264, 259, 1, 0, 0, 0, 264, 260, 1, 0, 0, 0, 264, 261, 1, 0, 0, 0, 264, 262, 1, 0, 0, 0, 264, 263, 1, 0, 0, 0, 265, 41, 1, 0, 0, 0, 266, 267, 5, 17, 0, 0, 267, 43, 1, 0, 0, 0, 268, 269, 5, 16, 0, 0, 269, 270, 5, 42, 0, 0, 270, 271, 5, 42, 0, 0, 271, 272, 3, 46, 23, 0, 272, 45, 1, 0, 0, 0, 273, 283, 3, 48, 24, 0, 274, 276, 3, 58, 29, 0, 275, 274, 1, 0, 0, 0, 276, 277, 1, 0, 0, 0, 277, 275, 1, 0, 0, 0, 277, 278, 1, 0, 0, 0, 278, 279, 1, 0, 0, 0, 279, 280, 3, 48, 24, 0, 280, 282, 1, 0, 0, 0, 281, 275, 1, 0, 0, 0, 282, 285, 1, 0, 0, 0, 283, 281, 1, 0, 0, 0, 283, 284, 1, 0, 0, 0, 284, 47, 1, 0, 0, 0, 285, 283, 1, 0, 0, 0, 286, 296, 5, 16, 0, 0, 287, 296, 5, 19, 0, 0, 288, 296, 5, 14, 0, 0, 289, 296, 5, 15, 0, 0, 290, 296, 3, 50, 25, 0, 291, 296, 3, 52, 26, 0, 292, 296, 3, 42, 21, 0, 293, 296, 5, 8, 0, 0, 294, 296, 5, 9, 0, 0, 295, 286, 1, 0, 0, 0, 295, 287, 1, 0, 0, 0, 295, 288, 1, 0, 0, 0, 295, 289, 1, 0, 0, 0, 295, 290, 1, 0, 0, 0, 295, 291, 1, 0, 0, 0, 295, 292, 1, 0, 0, 0, 295, 293, 1, 0, 0, 0, 295, 294, 1, 0, 0, 0, 296, 49, 1, 0, 0, 0, 297, 298, 5, 10, 0, 0, 298, 51, 1, 0, 0, 0, 299, 300, 5, 11, 0, 0, 300, 53, 1, 0, 0, 0, 301, 309, 5, 36, 0, 0, 302, 309, 5, 37, 0, 0, 303, 309, 5, 24, 0, 0, 304, 309, 5, 23, 0, 0, 305, 309, 3, 56, 28, 0, 306, 309, 3, 60, 30, 0, 307, 309, 3, 58, 29, 0, 308, 301, 1, 0, 0, 0, 308, 302, 1, 0, 0, 0, 308, 303, 1, 0, 0, 0, 308, 304, 1, 0, 0, 0, 308, 305, 1, 0, 0, 0, 308, 306, 1, 0, 0, 0, 308, 307, 1, 0, 0, 0, 309, 55, 1, 0, 0, 0, 310, 311, 7, 1, 0, 0, 311, 57, 1, 0, 0, 0, 312, 313, 7, 2, 0, 0, 313, 59, 1, 0, 0, 0, 314, 315, 7, 3, 0, 0, 315, 61, 1, 0, 0, 0, 316, 321, 3, 64, 32, 0, 317, 321, 3, 66, 33, 0, 318, 321, 3, 68, 34, 0, 319, 321, 3, 70, 35, 0, 320, 316, 1, 0, 0, 0, 320, 317, 1, 0, 0, 0, 320, 318, 1, 0, 0, 0, 320, 319, 1, 0, 0, 0, 321, 63, 1, 0, 0, 0, 322, 323, 5, 32, 0, 0, 323, 324, 5, 16, 0, 0, 324, 65, 1, 0, 0, 0, 325, 326, 5, 33, 0, 0, 326, 327, 5, 16, 0, 0, 327, 67, 1, 0, 0, 0, 328, 329, 5, 35, 0, 0, 329, 330, 5, 16, 0, 0, 330, 69, 1, 0, 0, 0, 331, 332, 5, 34, 0, 0, 332, 333, 5, 16, 0, 0, 333, 71, 1, 0, 0, 0, 334, 339, 5, 36, 0, 0, 335, 340, 3, 40, 20, 0, 336, 340, 3, 34, 17, 0, 337, 340, 5, 1, 0, 0, 338, 340, 5, 2, 0, 0, 339, 335, 1, 0, 0, 0, 339, 336, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 338, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 339, 1, 0, 0, 0, 341, 342, 1, 0, 0, 0, 342, 343, 1, 0, 0, 0, 343, 353, 5, 36, 0, 0, 344, 346, 5, 37, 0, 0, 345, 347, 3, 40, 20, 0, 346, 345, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 346, 1, 0, 0, 0, 348, 349, 1, 0, 0, 0, 349, 350, 1, 0, 0, 0, 350, 351, 5, 37, 0, 0, 351, 353, 1, 0, 0, 0, 352, 334, 1, 0, 0, 0, 352, 344, 1, 0, 0, 0, 353, 73, 1, 0, 0, 0, 354, 355, 5, 1, 0, 0, 355, 356, 3, 46, 23, 0, 356, 357, 5, 2, 0, 0, 357, 75, 1, 0, 0, 0, 358, 359, 5, 3, 0, 0, 359, 364, 3, 46, 23, 0, 360, 361, 5, 29, 0, 0, 361, 363, 3, 46, 23, 0, 362, 360, 1, 0, 0, 0, 363, 366, 1, 0, 0, 0, 364, 362, 1, 0, 0, 0, 364, 365, 1, 0, 0, 0, 365, 367, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 367, 368, 5, 4, 0, 0, 368, 77, 1, 0, 0, 0, 369, 373, 3, 86, 43, 0, 370, 372, 5, 7, 0, 0, 371, 370, 1, 0, 0, 0, 372, 375, 1, 0, 0, 0, 373, 371, 1, 0, 0, 0, 373, 374, 1, 0, 0, 0, 374, 379, 1, 0, 0, 0, 375, 373, 1, 0, 0, 0, 376, 378, 3, 8, 4, 0, 377, 376, 1, 0, 0, 0, 378, 381, 1, 0, 0, 0, 379, 377, 1, 0, 0, 0, 379, 380, 1, 0, 0, 0, 380, 388, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 382, 384, 5, 7, 0, 0, 383, 382, 1, 0, 0, 0, 383, 384, 1, 0, 0, 0, 384, 385, 1, 0, 0, 0, 385, 387, 3, 80, 40, 0, 386, 383, 1, 0, 0, 0, 387, 390, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 388, 389, 1, 0, 0, 0, 389, 79, 1, 0, 0, 0, 390, 388, 1, 0, 0, 0, 391, 395, 3, 88, 44, 0, 392, 394, 5, 7, 0, 0, 393, 392, 1, 0, 0, 0, 394, 397, 1, 0, 0, 0, 395, 393, 1, 0, 0, 0, 395, 396, 1, 0, 0, 0, 396, 401, 1, 0, 0, 0, 397, 395, 1, 0, 0, 0, 398, 400, 3, 8, 4, 0, 399, 398, 1, 0, 0, 0, 400, 403, 1, 0, 0, 0, 401, 399, 1, 0, 0, 0, 401, 402, 1, 0, 0, 0, 402, 410, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 404, 406, 5, 7, 0, 0, 405, 404, 1, 0, 0, 0, 405, 406, 1, 0, 0, 0, 406, 407, 1, 0, 0, 0, 407, 409, 3, 82, 41, 0, 408, 405, 1, 0, 0, 0, 409, 412, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 410, 411, 1, 0, 0, 0, 411, 81, 1, 0, 0, 0, 412, 410, 1, 0, 0, 0, 413, 417, 3, 90, 45, 0, 414, 416, 5, 7, 0, 0, 415, 414, 1, 0, 0, 0, 416, 419, 1, 0, 0, 0, 417, 415, 1, 0, 0, 0, 417, 418, 1, 0, 0, 0, 418, 423, 1, 0, 0, 0, 419, 417, 1, 0, 0, 0, 420, 422, 3, 8, 4, 0, 421, 420, 1, 0, 0, 0, 422, 425, 1, 0, 0, 0, 423, 421, 1, 0, 0, 0, 423, 424, 1, 0, 0, 0, 424, 432, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 426, 428, 5, 7, 0, 0, 427, 426, 1, 0, 0, 0, 427, 428, 1, 0, 0, 0, 428, 429, 1, 0, 0, 0, 429, 431, 3, 84, 42, 0, 430, 427, 1, 0, 0, 0, 431, 434, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 432, 433, 1, 0, 0, 0, 433, 83, 1, 0, 0, 0, 434, 432, 1, 0, 0, 0, 435, 439, 3, 92, 46, 0, 436, 438, 5, 7, 0, 0, 437, 436, 1, 0, 0, 0, 438, 441, 1, 0, 0, 0, 439, 437, 1, 0, 0, 0, 439, 440, 1, 0, 0, 0, 440, 445, 1, 0, 0, 0, 441, 439, 1, 0, 0, 0, 442, 444, 3, 8, 4, 0, 443, 442, 1, 0, 0, 0, 444, 447, 1, 0, 0, 0, 445, 443, 1, 0, 0, 0, 445, 446, 1, 0, 0, 0, 446, 85, 1, 0, 0, 0, 447, 445, 1, 0, 0, 0, 448, 449, 5, 32, 0, 0, 449, 450, 5, 32, 0, 0, 450, 451, 5, 32, 0, 0, 451, 452, 5, 32, 0, 0, 452, 453, 5, 32, 0, 0, 453, 454, 5, 32, 0, 0, 454, 455, 5, 32, 0, 0, 455, 456, 5, 32, 0, 0, 456, 457, 5, 32, 0, 0, 457, 458, 3, 36, 18, 0, 458, 459, 3, 94, 47, 0, 459, 87, 1, 0, 0, 0, 460, 461, 5, 5, 0, 0, 461, 462, 3, 36, 18, 0, 462, 463, 3, 94, 47, 0, 463, 89, 1, 0, 0, 0, 464, 465, 5, 6, 0, 0, 465, 466, 3, 36, 18, 0, 466, 467, 3, 94, 47, 0, 467, 91, 1, 0, 0, 0, 468, 469, 5, 25, 0, 0, 469, 470, 5, 25, 0, 0, 470, 471, 5, 25, 0, 0, 471, 472, 3, 36, 18, 0, 472, 473, 3, 94, 47, 0, 473, 93, 1, 0, 0, 0, 474, 475, 7, 4, 0, 0, 475, 95, 1, 0, 0, 0, 52, 98, 105, 109, 116, 121, 127, 133, 139, 144, 151, 163, 176, 181, 189, 199, 205, 214, 219, 226, 231, 235, 237, 242, 247, 249, 252, 255, 264, 277, 283, 295, 308, 320, 339, 341, 348, 352, 364, 373, 379, 383, 388, 395, 401, 405, 410, 417, 423, 427, 432, 439, 445]
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.tokens` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFile.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.7.4/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,42,470,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,42,477,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
         2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
         7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
         2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,45,2,46,
         7,46,2,47,7,47,1,0,1,0,3,0,99,8,0,1,0,1,0,1,1,4,1,104,8,1,11,1,12,
@@ -36,156 +36,159 @@
         8,23,11,23,12,23,277,1,23,1,23,5,23,282,8,23,10,23,12,23,285,9,23,
         1,24,1,24,1,24,1,24,1,24,1,24,1,24,1,24,1,24,3,24,296,8,24,1,25,
         1,25,1,26,1,26,1,27,1,27,1,27,1,27,1,27,1,27,1,27,3,27,309,8,27,
         1,28,1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,31,1,31,3,31,321,8,31,
         1,32,1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,1,36,
         1,36,1,36,1,36,1,36,4,36,340,8,36,11,36,12,36,341,1,36,1,36,1,36,
         4,36,347,8,36,11,36,12,36,348,1,36,1,36,3,36,353,8,36,1,37,1,37,
-        1,37,1,37,1,38,1,38,1,38,1,38,1,39,1,39,5,39,365,8,39,10,39,12,39,
-        368,9,39,1,39,5,39,371,8,39,10,39,12,39,374,9,39,1,39,3,39,377,8,
-        39,1,39,5,39,380,8,39,10,39,12,39,383,9,39,1,40,1,40,5,40,387,8,
-        40,10,40,12,40,390,9,40,1,40,5,40,393,8,40,10,40,12,40,396,9,40,
-        1,40,3,40,399,8,40,1,40,5,40,402,8,40,10,40,12,40,405,9,40,1,41,
-        1,41,5,41,409,8,41,10,41,12,41,412,9,41,1,41,5,41,415,8,41,10,41,
-        12,41,418,9,41,1,41,3,41,421,8,41,1,41,5,41,424,8,41,10,41,12,41,
-        427,9,41,1,42,1,42,5,42,431,8,42,10,42,12,42,434,9,42,1,42,5,42,
-        437,8,42,10,42,12,42,440,9,42,1,43,1,43,1,43,1,43,1,43,1,43,1,43,
-        1,43,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,44,1,45,1,45,1,45,1,45,
-        1,46,1,46,1,46,1,46,1,46,1,46,1,47,1,47,1,47,0,0,48,0,2,4,6,8,10,
-        12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,
-        56,58,60,62,64,66,68,70,72,74,76,78,80,82,84,86,88,90,92,94,0,5,
-        2,0,9,9,38,38,4,0,22,22,28,28,30,31,38,41,2,0,25,27,42,42,1,0,32,
-        35,1,1,7,7,498,0,96,1,0,0,0,2,103,1,0,0,0,4,107,1,0,0,0,6,114,1,
-        0,0,0,8,137,1,0,0,0,10,151,1,0,0,0,12,153,1,0,0,0,14,158,1,0,0,0,
-        16,166,1,0,0,0,18,169,1,0,0,0,20,171,1,0,0,0,22,184,1,0,0,0,24,192,
-        1,0,0,0,26,195,1,0,0,0,28,202,1,0,0,0,30,214,1,0,0,0,32,216,1,0,
-        0,0,34,221,1,0,0,0,36,224,1,0,0,0,38,228,1,0,0,0,40,264,1,0,0,0,
-        42,266,1,0,0,0,44,268,1,0,0,0,46,273,1,0,0,0,48,295,1,0,0,0,50,297,
-        1,0,0,0,52,299,1,0,0,0,54,308,1,0,0,0,56,310,1,0,0,0,58,312,1,0,
-        0,0,60,314,1,0,0,0,62,320,1,0,0,0,64,322,1,0,0,0,66,325,1,0,0,0,
-        68,328,1,0,0,0,70,331,1,0,0,0,72,352,1,0,0,0,74,354,1,0,0,0,76,358,
-        1,0,0,0,78,362,1,0,0,0,80,384,1,0,0,0,82,406,1,0,0,0,84,428,1,0,
-        0,0,86,441,1,0,0,0,88,453,1,0,0,0,90,457,1,0,0,0,92,461,1,0,0,0,
-        94,467,1,0,0,0,96,98,3,2,1,0,97,99,3,6,3,0,98,97,1,0,0,0,98,99,1,
-        0,0,0,99,100,1,0,0,0,100,101,5,0,0,1,101,1,1,0,0,0,102,104,3,4,2,
-        0,103,102,1,0,0,0,104,105,1,0,0,0,105,103,1,0,0,0,105,106,1,0,0,
-        0,106,3,1,0,0,0,107,109,5,32,0,0,108,110,3,36,18,0,109,108,1,0,0,
-        0,109,110,1,0,0,0,110,111,1,0,0,0,111,112,5,7,0,0,112,5,1,0,0,0,
-        113,115,5,7,0,0,114,113,1,0,0,0,115,116,1,0,0,0,116,114,1,0,0,0,
-        116,117,1,0,0,0,117,121,1,0,0,0,118,120,3,8,4,0,119,118,1,0,0,0,
-        120,123,1,0,0,0,121,119,1,0,0,0,121,122,1,0,0,0,122,127,1,0,0,0,
-        123,121,1,0,0,0,124,126,3,80,40,0,125,124,1,0,0,0,126,129,1,0,0,
-        0,127,125,1,0,0,0,127,128,1,0,0,0,128,133,1,0,0,0,129,127,1,0,0,
-        0,130,132,3,78,39,0,131,130,1,0,0,0,132,135,1,0,0,0,133,131,1,0,
-        0,0,133,134,1,0,0,0,134,7,1,0,0,0,135,133,1,0,0,0,136,138,3,10,5,
-        0,137,136,1,0,0,0,138,139,1,0,0,0,139,137,1,0,0,0,139,140,1,0,0,
-        0,140,144,1,0,0,0,141,143,5,7,0,0,142,141,1,0,0,0,143,146,1,0,0,
-        0,144,142,1,0,0,0,144,145,1,0,0,0,145,9,1,0,0,0,146,144,1,0,0,0,
-        147,152,3,26,13,0,148,152,3,14,7,0,149,152,3,12,6,0,150,152,3,4,
-        2,0,151,147,1,0,0,0,151,148,1,0,0,0,151,149,1,0,0,0,151,150,1,0,
-        0,0,152,11,1,0,0,0,153,154,3,76,38,0,154,155,5,42,0,0,155,156,3,
-        36,18,0,156,157,5,7,0,0,157,13,1,0,0,0,158,159,5,25,0,0,159,163,
-        3,16,8,0,160,162,3,22,11,0,161,160,1,0,0,0,162,165,1,0,0,0,163,161,
-        1,0,0,0,163,164,1,0,0,0,164,15,1,0,0,0,165,163,1,0,0,0,166,167,3,
-        18,9,0,167,168,5,7,0,0,168,17,1,0,0,0,169,170,3,20,10,0,170,19,1,
-        0,0,0,171,181,3,36,18,0,172,174,5,7,0,0,173,175,5,29,0,0,174,173,
-        1,0,0,0,175,176,1,0,0,0,176,174,1,0,0,0,176,177,1,0,0,0,177,178,
-        1,0,0,0,178,180,3,36,18,0,179,172,1,0,0,0,180,183,1,0,0,0,181,179,
-        1,0,0,0,181,182,1,0,0,0,182,21,1,0,0,0,183,181,1,0,0,0,184,185,5,
-        20,0,0,185,189,3,16,8,0,186,188,3,24,12,0,187,186,1,0,0,0,188,191,
-        1,0,0,0,189,187,1,0,0,0,189,190,1,0,0,0,190,23,1,0,0,0,191,189,1,
-        0,0,0,192,193,5,21,0,0,193,194,3,16,8,0,194,25,1,0,0,0,195,199,3,
-        28,14,0,196,198,3,22,11,0,197,196,1,0,0,0,198,201,1,0,0,0,199,197,
-        1,0,0,0,199,200,1,0,0,0,200,27,1,0,0,0,201,199,1,0,0,0,202,205,3,
-        30,15,0,203,204,5,29,0,0,204,206,3,34,17,0,205,203,1,0,0,0,205,206,
-        1,0,0,0,206,207,1,0,0,0,207,208,3,18,9,0,208,209,5,7,0,0,209,29,
-        1,0,0,0,210,215,5,8,0,0,211,215,3,32,16,0,212,215,5,40,0,0,213,215,
-        5,41,0,0,214,210,1,0,0,0,214,211,1,0,0,0,214,212,1,0,0,0,214,213,
-        1,0,0,0,215,31,1,0,0,0,216,219,7,0,0,0,217,218,5,42,0,0,218,220,
-        3,52,26,0,219,217,1,0,0,0,219,220,1,0,0,0,220,33,1,0,0,0,221,222,
-        5,15,0,0,222,35,1,0,0,0,223,225,3,38,19,0,224,223,1,0,0,0,225,226,
-        1,0,0,0,226,224,1,0,0,0,226,227,1,0,0,0,227,37,1,0,0,0,228,231,5,
-        29,0,0,229,230,5,36,0,0,230,232,3,56,28,0,231,229,1,0,0,0,231,232,
-        1,0,0,0,232,237,1,0,0,0,233,236,3,56,28,0,234,236,5,37,0,0,235,233,
-        1,0,0,0,235,234,1,0,0,0,236,239,1,0,0,0,237,235,1,0,0,0,237,238,
-        1,0,0,0,238,242,1,0,0,0,239,237,1,0,0,0,240,243,3,40,20,0,241,243,
-        3,72,36,0,242,240,1,0,0,0,242,241,1,0,0,0,242,243,1,0,0,0,243,252,
-        1,0,0,0,244,249,3,54,27,0,245,248,3,54,27,0,246,248,3,48,24,0,247,
-        245,1,0,0,0,247,246,1,0,0,0,248,251,1,0,0,0,249,247,1,0,0,0,249,
-        250,1,0,0,0,250,253,1,0,0,0,251,249,1,0,0,0,252,244,1,0,0,0,252,
-        253,1,0,0,0,253,255,1,0,0,0,254,256,3,76,38,0,255,254,1,0,0,0,255,
-        256,1,0,0,0,256,39,1,0,0,0,257,265,3,60,30,0,258,265,3,62,31,0,259,
-        265,3,74,37,0,260,265,3,44,22,0,261,265,3,46,23,0,262,265,3,76,38,
-        0,263,265,3,34,17,0,264,257,1,0,0,0,264,258,1,0,0,0,264,259,1,0,
-        0,0,264,260,1,0,0,0,264,261,1,0,0,0,264,262,1,0,0,0,264,263,1,0,
-        0,0,265,41,1,0,0,0,266,267,5,17,0,0,267,43,1,0,0,0,268,269,5,16,
-        0,0,269,270,5,42,0,0,270,271,5,42,0,0,271,272,3,46,23,0,272,45,1,
-        0,0,0,273,283,3,48,24,0,274,276,3,58,29,0,275,274,1,0,0,0,276,277,
-        1,0,0,0,277,275,1,0,0,0,277,278,1,0,0,0,278,279,1,0,0,0,279,280,
-        3,48,24,0,280,282,1,0,0,0,281,275,1,0,0,0,282,285,1,0,0,0,283,281,
-        1,0,0,0,283,284,1,0,0,0,284,47,1,0,0,0,285,283,1,0,0,0,286,296,5,
-        16,0,0,287,296,5,19,0,0,288,296,5,14,0,0,289,296,5,15,0,0,290,296,
-        3,50,25,0,291,296,3,52,26,0,292,296,3,42,21,0,293,296,5,8,0,0,294,
-        296,5,9,0,0,295,286,1,0,0,0,295,287,1,0,0,0,295,288,1,0,0,0,295,
-        289,1,0,0,0,295,290,1,0,0,0,295,291,1,0,0,0,295,292,1,0,0,0,295,
-        293,1,0,0,0,295,294,1,0,0,0,296,49,1,0,0,0,297,298,5,10,0,0,298,
-        51,1,0,0,0,299,300,5,11,0,0,300,53,1,0,0,0,301,309,5,36,0,0,302,
-        309,5,37,0,0,303,309,5,24,0,0,304,309,5,23,0,0,305,309,3,56,28,0,
-        306,309,3,60,30,0,307,309,3,58,29,0,308,301,1,0,0,0,308,302,1,0,
-        0,0,308,303,1,0,0,0,308,304,1,0,0,0,308,305,1,0,0,0,308,306,1,0,
-        0,0,308,307,1,0,0,0,309,55,1,0,0,0,310,311,7,1,0,0,311,57,1,0,0,
-        0,312,313,7,2,0,0,313,59,1,0,0,0,314,315,7,3,0,0,315,61,1,0,0,0,
-        316,321,3,64,32,0,317,321,3,66,33,0,318,321,3,68,34,0,319,321,3,
-        70,35,0,320,316,1,0,0,0,320,317,1,0,0,0,320,318,1,0,0,0,320,319,
-        1,0,0,0,321,63,1,0,0,0,322,323,5,32,0,0,323,324,5,16,0,0,324,65,
-        1,0,0,0,325,326,5,33,0,0,326,327,5,16,0,0,327,67,1,0,0,0,328,329,
-        5,35,0,0,329,330,5,16,0,0,330,69,1,0,0,0,331,332,5,34,0,0,332,333,
-        5,16,0,0,333,71,1,0,0,0,334,339,5,36,0,0,335,340,3,40,20,0,336,340,
-        3,34,17,0,337,340,5,1,0,0,338,340,5,2,0,0,339,335,1,0,0,0,339,336,
-        1,0,0,0,339,337,1,0,0,0,339,338,1,0,0,0,340,341,1,0,0,0,341,339,
-        1,0,0,0,341,342,1,0,0,0,342,343,1,0,0,0,343,353,5,36,0,0,344,346,
-        5,37,0,0,345,347,3,40,20,0,346,345,1,0,0,0,347,348,1,0,0,0,348,346,
-        1,0,0,0,348,349,1,0,0,0,349,350,1,0,0,0,350,351,5,37,0,0,351,353,
-        1,0,0,0,352,334,1,0,0,0,352,344,1,0,0,0,353,73,1,0,0,0,354,355,5,
-        1,0,0,355,356,3,46,23,0,356,357,5,2,0,0,357,75,1,0,0,0,358,359,5,
-        3,0,0,359,360,3,46,23,0,360,361,5,4,0,0,361,77,1,0,0,0,362,366,3,
-        86,43,0,363,365,5,7,0,0,364,363,1,0,0,0,365,368,1,0,0,0,366,364,
-        1,0,0,0,366,367,1,0,0,0,367,372,1,0,0,0,368,366,1,0,0,0,369,371,
-        3,8,4,0,370,369,1,0,0,0,371,374,1,0,0,0,372,370,1,0,0,0,372,373,
-        1,0,0,0,373,381,1,0,0,0,374,372,1,0,0,0,375,377,5,7,0,0,376,375,
-        1,0,0,0,376,377,1,0,0,0,377,378,1,0,0,0,378,380,3,80,40,0,379,376,
-        1,0,0,0,380,383,1,0,0,0,381,379,1,0,0,0,381,382,1,0,0,0,382,79,1,
-        0,0,0,383,381,1,0,0,0,384,388,3,88,44,0,385,387,5,7,0,0,386,385,
-        1,0,0,0,387,390,1,0,0,0,388,386,1,0,0,0,388,389,1,0,0,0,389,394,
-        1,0,0,0,390,388,1,0,0,0,391,393,3,8,4,0,392,391,1,0,0,0,393,396,
-        1,0,0,0,394,392,1,0,0,0,394,395,1,0,0,0,395,403,1,0,0,0,396,394,
-        1,0,0,0,397,399,5,7,0,0,398,397,1,0,0,0,398,399,1,0,0,0,399,400,
-        1,0,0,0,400,402,3,82,41,0,401,398,1,0,0,0,402,405,1,0,0,0,403,401,
-        1,0,0,0,403,404,1,0,0,0,404,81,1,0,0,0,405,403,1,0,0,0,406,410,3,
-        90,45,0,407,409,5,7,0,0,408,407,1,0,0,0,409,412,1,0,0,0,410,408,
-        1,0,0,0,410,411,1,0,0,0,411,416,1,0,0,0,412,410,1,0,0,0,413,415,
-        3,8,4,0,414,413,1,0,0,0,415,418,1,0,0,0,416,414,1,0,0,0,416,417,
-        1,0,0,0,417,425,1,0,0,0,418,416,1,0,0,0,419,421,5,7,0,0,420,419,
-        1,0,0,0,420,421,1,0,0,0,421,422,1,0,0,0,422,424,3,84,42,0,423,420,
-        1,0,0,0,424,427,1,0,0,0,425,423,1,0,0,0,425,426,1,0,0,0,426,83,1,
-        0,0,0,427,425,1,0,0,0,428,432,3,92,46,0,429,431,5,7,0,0,430,429,
-        1,0,0,0,431,434,1,0,0,0,432,430,1,0,0,0,432,433,1,0,0,0,433,438,
-        1,0,0,0,434,432,1,0,0,0,435,437,3,8,4,0,436,435,1,0,0,0,437,440,
-        1,0,0,0,438,436,1,0,0,0,438,439,1,0,0,0,439,85,1,0,0,0,440,438,1,
-        0,0,0,441,442,5,32,0,0,442,443,5,32,0,0,443,444,5,32,0,0,444,445,
-        5,32,0,0,445,446,5,32,0,0,446,447,5,32,0,0,447,448,5,32,0,0,448,
-        449,5,32,0,0,449,450,5,32,0,0,450,451,3,36,18,0,451,452,3,94,47,
-        0,452,87,1,0,0,0,453,454,5,5,0,0,454,455,3,36,18,0,455,456,3,94,
-        47,0,456,89,1,0,0,0,457,458,5,6,0,0,458,459,3,36,18,0,459,460,3,
-        94,47,0,460,91,1,0,0,0,461,462,5,25,0,0,462,463,5,25,0,0,463,464,
-        5,25,0,0,464,465,3,36,18,0,465,466,3,94,47,0,466,93,1,0,0,0,467,
-        468,7,4,0,0,468,95,1,0,0,0,51,98,105,109,116,121,127,133,139,144,
+        1,37,1,37,1,38,1,38,1,38,1,38,5,38,363,8,38,10,38,12,38,366,9,38,
+        1,38,1,38,1,39,1,39,5,39,372,8,39,10,39,12,39,375,9,39,1,39,5,39,
+        378,8,39,10,39,12,39,381,9,39,1,39,3,39,384,8,39,1,39,5,39,387,8,
+        39,10,39,12,39,390,9,39,1,40,1,40,5,40,394,8,40,10,40,12,40,397,
+        9,40,1,40,5,40,400,8,40,10,40,12,40,403,9,40,1,40,3,40,406,8,40,
+        1,40,5,40,409,8,40,10,40,12,40,412,9,40,1,41,1,41,5,41,416,8,41,
+        10,41,12,41,419,9,41,1,41,5,41,422,8,41,10,41,12,41,425,9,41,1,41,
+        3,41,428,8,41,1,41,5,41,431,8,41,10,41,12,41,434,9,41,1,42,1,42,
+        5,42,438,8,42,10,42,12,42,441,9,42,1,42,5,42,444,8,42,10,42,12,42,
+        447,9,42,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,
+        1,43,1,44,1,44,1,44,1,44,1,45,1,45,1,45,1,45,1,46,1,46,1,46,1,46,
+        1,46,1,46,1,47,1,47,1,47,0,0,48,0,2,4,6,8,10,12,14,16,18,20,22,24,
+        26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,
+        70,72,74,76,78,80,82,84,86,88,90,92,94,0,5,2,0,9,9,38,38,4,0,22,
+        22,28,28,30,31,38,41,2,0,25,27,42,42,1,0,32,35,1,1,7,7,506,0,96,
+        1,0,0,0,2,103,1,0,0,0,4,107,1,0,0,0,6,114,1,0,0,0,8,137,1,0,0,0,
+        10,151,1,0,0,0,12,153,1,0,0,0,14,158,1,0,0,0,16,166,1,0,0,0,18,169,
+        1,0,0,0,20,171,1,0,0,0,22,184,1,0,0,0,24,192,1,0,0,0,26,195,1,0,
+        0,0,28,202,1,0,0,0,30,214,1,0,0,0,32,216,1,0,0,0,34,221,1,0,0,0,
+        36,224,1,0,0,0,38,228,1,0,0,0,40,264,1,0,0,0,42,266,1,0,0,0,44,268,
+        1,0,0,0,46,273,1,0,0,0,48,295,1,0,0,0,50,297,1,0,0,0,52,299,1,0,
+        0,0,54,308,1,0,0,0,56,310,1,0,0,0,58,312,1,0,0,0,60,314,1,0,0,0,
+        62,320,1,0,0,0,64,322,1,0,0,0,66,325,1,0,0,0,68,328,1,0,0,0,70,331,
+        1,0,0,0,72,352,1,0,0,0,74,354,1,0,0,0,76,358,1,0,0,0,78,369,1,0,
+        0,0,80,391,1,0,0,0,82,413,1,0,0,0,84,435,1,0,0,0,86,448,1,0,0,0,
+        88,460,1,0,0,0,90,464,1,0,0,0,92,468,1,0,0,0,94,474,1,0,0,0,96,98,
+        3,2,1,0,97,99,3,6,3,0,98,97,1,0,0,0,98,99,1,0,0,0,99,100,1,0,0,0,
+        100,101,5,0,0,1,101,1,1,0,0,0,102,104,3,4,2,0,103,102,1,0,0,0,104,
+        105,1,0,0,0,105,103,1,0,0,0,105,106,1,0,0,0,106,3,1,0,0,0,107,109,
+        5,32,0,0,108,110,3,36,18,0,109,108,1,0,0,0,109,110,1,0,0,0,110,111,
+        1,0,0,0,111,112,5,7,0,0,112,5,1,0,0,0,113,115,5,7,0,0,114,113,1,
+        0,0,0,115,116,1,0,0,0,116,114,1,0,0,0,116,117,1,0,0,0,117,121,1,
+        0,0,0,118,120,3,8,4,0,119,118,1,0,0,0,120,123,1,0,0,0,121,119,1,
+        0,0,0,121,122,1,0,0,0,122,127,1,0,0,0,123,121,1,0,0,0,124,126,3,
+        80,40,0,125,124,1,0,0,0,126,129,1,0,0,0,127,125,1,0,0,0,127,128,
+        1,0,0,0,128,133,1,0,0,0,129,127,1,0,0,0,130,132,3,78,39,0,131,130,
+        1,0,0,0,132,135,1,0,0,0,133,131,1,0,0,0,133,134,1,0,0,0,134,7,1,
+        0,0,0,135,133,1,0,0,0,136,138,3,10,5,0,137,136,1,0,0,0,138,139,1,
+        0,0,0,139,137,1,0,0,0,139,140,1,0,0,0,140,144,1,0,0,0,141,143,5,
+        7,0,0,142,141,1,0,0,0,143,146,1,0,0,0,144,142,1,0,0,0,144,145,1,
+        0,0,0,145,9,1,0,0,0,146,144,1,0,0,0,147,152,3,26,13,0,148,152,3,
+        14,7,0,149,152,3,12,6,0,150,152,3,4,2,0,151,147,1,0,0,0,151,148,
+        1,0,0,0,151,149,1,0,0,0,151,150,1,0,0,0,152,11,1,0,0,0,153,154,3,
+        76,38,0,154,155,5,42,0,0,155,156,3,36,18,0,156,157,5,7,0,0,157,13,
+        1,0,0,0,158,159,5,25,0,0,159,163,3,16,8,0,160,162,3,22,11,0,161,
+        160,1,0,0,0,162,165,1,0,0,0,163,161,1,0,0,0,163,164,1,0,0,0,164,
+        15,1,0,0,0,165,163,1,0,0,0,166,167,3,18,9,0,167,168,5,7,0,0,168,
+        17,1,0,0,0,169,170,3,20,10,0,170,19,1,0,0,0,171,181,3,36,18,0,172,
+        174,5,7,0,0,173,175,5,29,0,0,174,173,1,0,0,0,175,176,1,0,0,0,176,
+        174,1,0,0,0,176,177,1,0,0,0,177,178,1,0,0,0,178,180,3,36,18,0,179,
+        172,1,0,0,0,180,183,1,0,0,0,181,179,1,0,0,0,181,182,1,0,0,0,182,
+        21,1,0,0,0,183,181,1,0,0,0,184,185,5,20,0,0,185,189,3,16,8,0,186,
+        188,3,24,12,0,187,186,1,0,0,0,188,191,1,0,0,0,189,187,1,0,0,0,189,
+        190,1,0,0,0,190,23,1,0,0,0,191,189,1,0,0,0,192,193,5,21,0,0,193,
+        194,3,16,8,0,194,25,1,0,0,0,195,199,3,28,14,0,196,198,3,22,11,0,
+        197,196,1,0,0,0,198,201,1,0,0,0,199,197,1,0,0,0,199,200,1,0,0,0,
+        200,27,1,0,0,0,201,199,1,0,0,0,202,205,3,30,15,0,203,204,5,29,0,
+        0,204,206,3,34,17,0,205,203,1,0,0,0,205,206,1,0,0,0,206,207,1,0,
+        0,0,207,208,3,18,9,0,208,209,5,7,0,0,209,29,1,0,0,0,210,215,5,8,
+        0,0,211,215,3,32,16,0,212,215,5,40,0,0,213,215,5,41,0,0,214,210,
+        1,0,0,0,214,211,1,0,0,0,214,212,1,0,0,0,214,213,1,0,0,0,215,31,1,
+        0,0,0,216,219,7,0,0,0,217,218,5,42,0,0,218,220,3,52,26,0,219,217,
+        1,0,0,0,219,220,1,0,0,0,220,33,1,0,0,0,221,222,5,15,0,0,222,35,1,
+        0,0,0,223,225,3,38,19,0,224,223,1,0,0,0,225,226,1,0,0,0,226,224,
+        1,0,0,0,226,227,1,0,0,0,227,37,1,0,0,0,228,231,5,29,0,0,229,230,
+        5,36,0,0,230,232,3,56,28,0,231,229,1,0,0,0,231,232,1,0,0,0,232,237,
+        1,0,0,0,233,236,3,56,28,0,234,236,5,37,0,0,235,233,1,0,0,0,235,234,
+        1,0,0,0,236,239,1,0,0,0,237,235,1,0,0,0,237,238,1,0,0,0,238,242,
+        1,0,0,0,239,237,1,0,0,0,240,243,3,40,20,0,241,243,3,72,36,0,242,
+        240,1,0,0,0,242,241,1,0,0,0,242,243,1,0,0,0,243,252,1,0,0,0,244,
+        249,3,54,27,0,245,248,3,54,27,0,246,248,3,48,24,0,247,245,1,0,0,
+        0,247,246,1,0,0,0,248,251,1,0,0,0,249,247,1,0,0,0,249,250,1,0,0,
+        0,250,253,1,0,0,0,251,249,1,0,0,0,252,244,1,0,0,0,252,253,1,0,0,
+        0,253,255,1,0,0,0,254,256,3,76,38,0,255,254,1,0,0,0,255,256,1,0,
+        0,0,256,39,1,0,0,0,257,265,3,60,30,0,258,265,3,62,31,0,259,265,3,
+        74,37,0,260,265,3,44,22,0,261,265,3,46,23,0,262,265,3,76,38,0,263,
+        265,3,34,17,0,264,257,1,0,0,0,264,258,1,0,0,0,264,259,1,0,0,0,264,
+        260,1,0,0,0,264,261,1,0,0,0,264,262,1,0,0,0,264,263,1,0,0,0,265,
+        41,1,0,0,0,266,267,5,17,0,0,267,43,1,0,0,0,268,269,5,16,0,0,269,
+        270,5,42,0,0,270,271,5,42,0,0,271,272,3,46,23,0,272,45,1,0,0,0,273,
+        283,3,48,24,0,274,276,3,58,29,0,275,274,1,0,0,0,276,277,1,0,0,0,
+        277,275,1,0,0,0,277,278,1,0,0,0,278,279,1,0,0,0,279,280,3,48,24,
+        0,280,282,1,0,0,0,281,275,1,0,0,0,282,285,1,0,0,0,283,281,1,0,0,
+        0,283,284,1,0,0,0,284,47,1,0,0,0,285,283,1,0,0,0,286,296,5,16,0,
+        0,287,296,5,19,0,0,288,296,5,14,0,0,289,296,5,15,0,0,290,296,3,50,
+        25,0,291,296,3,52,26,0,292,296,3,42,21,0,293,296,5,8,0,0,294,296,
+        5,9,0,0,295,286,1,0,0,0,295,287,1,0,0,0,295,288,1,0,0,0,295,289,
+        1,0,0,0,295,290,1,0,0,0,295,291,1,0,0,0,295,292,1,0,0,0,295,293,
+        1,0,0,0,295,294,1,0,0,0,296,49,1,0,0,0,297,298,5,10,0,0,298,51,1,
+        0,0,0,299,300,5,11,0,0,300,53,1,0,0,0,301,309,5,36,0,0,302,309,5,
+        37,0,0,303,309,5,24,0,0,304,309,5,23,0,0,305,309,3,56,28,0,306,309,
+        3,60,30,0,307,309,3,58,29,0,308,301,1,0,0,0,308,302,1,0,0,0,308,
+        303,1,0,0,0,308,304,1,0,0,0,308,305,1,0,0,0,308,306,1,0,0,0,308,
+        307,1,0,0,0,309,55,1,0,0,0,310,311,7,1,0,0,311,57,1,0,0,0,312,313,
+        7,2,0,0,313,59,1,0,0,0,314,315,7,3,0,0,315,61,1,0,0,0,316,321,3,
+        64,32,0,317,321,3,66,33,0,318,321,3,68,34,0,319,321,3,70,35,0,320,
+        316,1,0,0,0,320,317,1,0,0,0,320,318,1,0,0,0,320,319,1,0,0,0,321,
+        63,1,0,0,0,322,323,5,32,0,0,323,324,5,16,0,0,324,65,1,0,0,0,325,
+        326,5,33,0,0,326,327,5,16,0,0,327,67,1,0,0,0,328,329,5,35,0,0,329,
+        330,5,16,0,0,330,69,1,0,0,0,331,332,5,34,0,0,332,333,5,16,0,0,333,
+        71,1,0,0,0,334,339,5,36,0,0,335,340,3,40,20,0,336,340,3,34,17,0,
+        337,340,5,1,0,0,338,340,5,2,0,0,339,335,1,0,0,0,339,336,1,0,0,0,
+        339,337,1,0,0,0,339,338,1,0,0,0,340,341,1,0,0,0,341,339,1,0,0,0,
+        341,342,1,0,0,0,342,343,1,0,0,0,343,353,5,36,0,0,344,346,5,37,0,
+        0,345,347,3,40,20,0,346,345,1,0,0,0,347,348,1,0,0,0,348,346,1,0,
+        0,0,348,349,1,0,0,0,349,350,1,0,0,0,350,351,5,37,0,0,351,353,1,0,
+        0,0,352,334,1,0,0,0,352,344,1,0,0,0,353,73,1,0,0,0,354,355,5,1,0,
+        0,355,356,3,46,23,0,356,357,5,2,0,0,357,75,1,0,0,0,358,359,5,3,0,
+        0,359,364,3,46,23,0,360,361,5,29,0,0,361,363,3,46,23,0,362,360,1,
+        0,0,0,363,366,1,0,0,0,364,362,1,0,0,0,364,365,1,0,0,0,365,367,1,
+        0,0,0,366,364,1,0,0,0,367,368,5,4,0,0,368,77,1,0,0,0,369,373,3,86,
+        43,0,370,372,5,7,0,0,371,370,1,0,0,0,372,375,1,0,0,0,373,371,1,0,
+        0,0,373,374,1,0,0,0,374,379,1,0,0,0,375,373,1,0,0,0,376,378,3,8,
+        4,0,377,376,1,0,0,0,378,381,1,0,0,0,379,377,1,0,0,0,379,380,1,0,
+        0,0,380,388,1,0,0,0,381,379,1,0,0,0,382,384,5,7,0,0,383,382,1,0,
+        0,0,383,384,1,0,0,0,384,385,1,0,0,0,385,387,3,80,40,0,386,383,1,
+        0,0,0,387,390,1,0,0,0,388,386,1,0,0,0,388,389,1,0,0,0,389,79,1,0,
+        0,0,390,388,1,0,0,0,391,395,3,88,44,0,392,394,5,7,0,0,393,392,1,
+        0,0,0,394,397,1,0,0,0,395,393,1,0,0,0,395,396,1,0,0,0,396,401,1,
+        0,0,0,397,395,1,0,0,0,398,400,3,8,4,0,399,398,1,0,0,0,400,403,1,
+        0,0,0,401,399,1,0,0,0,401,402,1,0,0,0,402,410,1,0,0,0,403,401,1,
+        0,0,0,404,406,5,7,0,0,405,404,1,0,0,0,405,406,1,0,0,0,406,407,1,
+        0,0,0,407,409,3,82,41,0,408,405,1,0,0,0,409,412,1,0,0,0,410,408,
+        1,0,0,0,410,411,1,0,0,0,411,81,1,0,0,0,412,410,1,0,0,0,413,417,3,
+        90,45,0,414,416,5,7,0,0,415,414,1,0,0,0,416,419,1,0,0,0,417,415,
+        1,0,0,0,417,418,1,0,0,0,418,423,1,0,0,0,419,417,1,0,0,0,420,422,
+        3,8,4,0,421,420,1,0,0,0,422,425,1,0,0,0,423,421,1,0,0,0,423,424,
+        1,0,0,0,424,432,1,0,0,0,425,423,1,0,0,0,426,428,5,7,0,0,427,426,
+        1,0,0,0,427,428,1,0,0,0,428,429,1,0,0,0,429,431,3,84,42,0,430,427,
+        1,0,0,0,431,434,1,0,0,0,432,430,1,0,0,0,432,433,1,0,0,0,433,83,1,
+        0,0,0,434,432,1,0,0,0,435,439,3,92,46,0,436,438,5,7,0,0,437,436,
+        1,0,0,0,438,441,1,0,0,0,439,437,1,0,0,0,439,440,1,0,0,0,440,445,
+        1,0,0,0,441,439,1,0,0,0,442,444,3,8,4,0,443,442,1,0,0,0,444,447,
+        1,0,0,0,445,443,1,0,0,0,445,446,1,0,0,0,446,85,1,0,0,0,447,445,1,
+        0,0,0,448,449,5,32,0,0,449,450,5,32,0,0,450,451,5,32,0,0,451,452,
+        5,32,0,0,452,453,5,32,0,0,453,454,5,32,0,0,454,455,5,32,0,0,455,
+        456,5,32,0,0,456,457,5,32,0,0,457,458,3,36,18,0,458,459,3,94,47,
+        0,459,87,1,0,0,0,460,461,5,5,0,0,461,462,3,36,18,0,462,463,3,94,
+        47,0,463,89,1,0,0,0,464,465,5,6,0,0,465,466,3,36,18,0,466,467,3,
+        94,47,0,467,91,1,0,0,0,468,469,5,25,0,0,469,470,5,25,0,0,470,471,
+        5,25,0,0,471,472,3,36,18,0,472,473,3,94,47,0,473,93,1,0,0,0,474,
+        475,7,4,0,0,475,95,1,0,0,0,52,98,105,109,116,121,127,133,139,144,
         151,163,176,181,189,199,205,214,219,226,231,235,237,242,247,249,
-        252,255,264,277,283,295,308,320,339,341,348,352,366,372,376,381,
-        388,394,398,403,410,416,420,425,432,438
+        252,255,264,277,283,295,308,320,339,341,348,352,364,373,379,383,
+        388,395,401,405,410,417,423,427,432,439,445
     ]
 
 class ZorgFileParser ( Parser ):
 
     grammarFileName = "ZorgFile.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -2896,17 +2899,26 @@
     class RefContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def id_group(self):
-            return self.getTypedRuleContext(ZorgFileParser.Id_groupContext,0)
+        def id_group(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgFileParser.Id_groupContext)
+            else:
+                return self.getTypedRuleContext(ZorgFileParser.Id_groupContext,i)
+
 
+        def SPACE(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgFileParser.SPACE)
+            else:
+                return self.getToken(ZorgFileParser.SPACE, i)
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_ref
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterRef" ):
                 listener.enterRef(self)
@@ -2918,21 +2930,34 @@
 
 
 
     def ref(self):
 
         localctx = ZorgFileParser.RefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 76, self.RULE_ref)
+        self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 358
             self.match(ZorgFileParser.T__2)
             self.state = 359
             self.id_group()
-            self.state = 360
+            self.state = 364
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while _la==29:
+                self.state = 360
+                self.match(ZorgFileParser.SPACE)
+                self.state = 361
+                self.id_group()
+                self.state = 366
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+
+            self.state = 367
             self.match(ZorgFileParser.T__3)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2987,53 +3012,53 @@
     def h1_section(self):
 
         localctx = ZorgFileParser.H1_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 78, self.RULE_h1_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 362
+            self.state = 369
             self.h1_header()
-            self.state = 366
+            self.state = 373
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,37,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 363
+                    self.state = 370
                     self.match(ZorgFileParser.NL) 
-                self.state = 368
+                self.state = 375
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,37,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
 
-            self.state = 372
+            self.state = 379
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 369
+                    self.state = 376
                     self.block() 
-                self.state = 374
+                self.state = 381
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
 
-            self.state = 381
+            self.state = 388
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==5 or _la==7:
-                self.state = 376
+                self.state = 383
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==7:
-                    self.state = 375
+                    self.state = 382
                     self.match(ZorgFileParser.NL)
 
 
-                self.state = 378
+                self.state = 385
                 self.h2_section()
-                self.state = 383
+                self.state = 390
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3090,56 +3115,56 @@
     def h2_section(self):
 
         localctx = ZorgFileParser.H2_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 80, self.RULE_h2_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 384
+            self.state = 391
             self.h2_header()
-            self.state = 388
+            self.state = 395
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 385
+                    self.state = 392
                     self.match(ZorgFileParser.NL) 
-                self.state = 390
+                self.state = 397
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
 
-            self.state = 394
+            self.state = 401
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 391
+                    self.state = 398
                     self.block() 
-                self.state = 396
+                self.state = 403
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
 
-            self.state = 403
+            self.state = 410
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 398
+                    self.state = 405
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 397
+                        self.state = 404
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 400
+                    self.state = 407
                     self.h3_section() 
-                self.state = 405
+                self.state = 412
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3194,56 +3219,56 @@
     def h3_section(self):
 
         localctx = ZorgFileParser.H3_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 82, self.RULE_h3_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 406
+            self.state = 413
             self.h3_header()
-            self.state = 410
+            self.state = 417
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 407
+                    self.state = 414
                     self.match(ZorgFileParser.NL) 
-                self.state = 412
+                self.state = 419
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
 
-            self.state = 416
+            self.state = 423
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 413
+                    self.state = 420
                     self.block() 
-                self.state = 418
+                self.state = 425
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
 
-            self.state = 425
+            self.state = 432
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,48,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 420
+                    self.state = 427
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 419
+                        self.state = 426
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 422
+                    self.state = 429
                     self.h4_section() 
-                self.state = 427
+                self.state = 434
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,48,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3290,37 +3315,37 @@
 
     def h4_section(self):
 
         localctx = ZorgFileParser.H4_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 84, self.RULE_h4_section)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 428
+            self.state = 435
             self.h4_header()
-            self.state = 432
+            self.state = 439
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 429
+                    self.state = 436
                     self.match(ZorgFileParser.NL) 
-                self.state = 434
+                self.state = 441
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
 
-            self.state = 438
+            self.state = 445
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 435
+                    self.state = 442
                     self.block() 
-                self.state = 440
+                self.state = 447
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3364,35 +3389,35 @@
 
     def h1_header(self):
 
         localctx = ZorgFileParser.H1_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 86, self.RULE_h1_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 441
+            self.state = 448
             self.match(ZorgFileParser.HASH)
-            self.state = 442
+            self.state = 449
             self.match(ZorgFileParser.HASH)
-            self.state = 443
+            self.state = 450
             self.match(ZorgFileParser.HASH)
-            self.state = 444
+            self.state = 451
             self.match(ZorgFileParser.HASH)
-            self.state = 445
+            self.state = 452
             self.match(ZorgFileParser.HASH)
-            self.state = 446
+            self.state = 453
             self.match(ZorgFileParser.HASH)
-            self.state = 447
+            self.state = 454
             self.match(ZorgFileParser.HASH)
-            self.state = 448
+            self.state = 455
             self.match(ZorgFileParser.HASH)
-            self.state = 449
+            self.state = 456
             self.match(ZorgFileParser.HASH)
-            self.state = 450
+            self.state = 457
             self.space_atoms()
-            self.state = 451
+            self.state = 458
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3430,19 +3455,19 @@
 
     def h2_header(self):
 
         localctx = ZorgFileParser.H2_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 88, self.RULE_h2_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 453
+            self.state = 460
             self.match(ZorgFileParser.T__4)
-            self.state = 454
+            self.state = 461
             self.space_atoms()
-            self.state = 455
+            self.state = 462
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3480,19 +3505,19 @@
 
     def h3_header(self):
 
         localctx = ZorgFileParser.H3_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 90, self.RULE_h3_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 457
+            self.state = 464
             self.match(ZorgFileParser.T__5)
-            self.state = 458
+            self.state = 465
             self.space_atoms()
-            self.state = 459
+            self.state = 466
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3536,23 +3561,23 @@
 
     def h4_header(self):
 
         localctx = ZorgFileParser.H4_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 92, self.RULE_h4_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 461
+            self.state = 468
             self.match(ZorgFileParser.DASH)
-            self.state = 462
+            self.state = 469
             self.match(ZorgFileParser.DASH)
-            self.state = 463
+            self.state = 470
             self.match(ZorgFileParser.DASH)
-            self.state = 464
+            self.state = 471
             self.space_atoms()
-            self.state = 465
+            self.state = 472
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3589,15 +3614,15 @@
     def eol(self):
 
         localctx = ZorgFileParser.EolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 94, self.RULE_eol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 467
+            self.state = 474
             _la = self._input.LA(1)
             if not(_la==-1 or _la==7):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp` & `zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 '8'
 '9'
 '!'
 '0'
 '<='
 '>='
 'c'
+'f='
 'create'
 'modify'
 'priority'
 'file'
 'type'
 null
 'o'
@@ -85,14 +86,15 @@
 null
 null
 null
 null
 null
 null
 null
+null
 NL
 LOWER_O
 LOWER_X
 DATE
 TIME
 CREATE_RANGE_HEAD
 MODIFY_RANGE_HEAD
@@ -148,14 +150,15 @@
 T__18
 T__19
 T__20
 T__21
 T__22
 T__23
 T__24
+T__25
 NL
 LOWER_O
 LOWER_X
 DATE
 TIME
 CREATE_RANGE_HEAD
 MODIFY_RANGE_HEAD
@@ -201,8 +204,8 @@
 DEFAULT_TOKEN_CHANNEL
 HIDDEN
 
 mode names:
 DEFAULT_MODE
 
 atn:
-[4, 0, 61, 359, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 2, 48, 7, 48, 2, 49, 7, 49, 2, 50, 7, 50, 2, 51, 7, 51, 2, 52, 7, 52, 2, 53, 7, 53, 2, 54, 7, 54, 2, 55, 7, 55, 2, 56, 7, 56, 2, 57, 7, 57, 2, 58, 7, 58, 2, 59, 7, 59, 2, 60, 7, 60, 2, 61, 7, 61, 2, 62, 7, 62, 2, 63, 7, 63, 2, 64, 7, 64, 2, 65, 7, 65, 2, 66, 7, 66, 2, 67, 7, 67, 2, 68, 7, 68, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 11, 1, 11, 1, 12, 1, 12, 1, 13, 1, 13, 1, 14, 1, 14, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 17, 1, 18, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 25, 3, 25, 220, 8, 25, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 28, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 5, 34, 259, 8, 34, 10, 34, 12, 34, 262, 9, 34, 1, 35, 1, 35, 1, 35, 1, 35, 1, 35, 3, 35, 269, 8, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 1, 37, 1, 37, 1, 37, 5, 37, 281, 8, 37, 10, 37, 12, 37, 284, 9, 37, 1, 38, 1, 38, 1, 38, 1, 38, 1, 39, 1, 39, 1, 39, 1, 39, 1, 39, 1, 39, 1, 40, 1, 40, 1, 41, 1, 41, 1, 42, 1, 42, 1, 43, 1, 43, 1, 44, 1, 44, 1, 45, 1, 45, 1, 46, 1, 46, 1, 47, 1, 47, 1, 48, 1, 48, 1, 49, 1, 49, 1, 50, 1, 50, 1, 51, 1, 51, 1, 52, 1, 52, 1, 53, 1, 53, 1, 54, 1, 54, 1, 55, 1, 55, 1, 56, 1, 56, 1, 57, 1, 57, 1, 58, 1, 58, 1, 59, 1, 59, 1, 60, 1, 60, 1, 61, 1, 61, 1, 62, 1, 62, 1, 63, 1, 63, 3, 63, 344, 8, 63, 1, 64, 1, 64, 1, 65, 1, 65, 1, 66, 1, 66, 1, 67, 1, 67, 3, 67, 354, 8, 67, 1, 68, 1, 68, 3, 68, 358, 8, 68, 0, 0, 69, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 36, 73, 37, 75, 38, 77, 39, 79, 40, 81, 41, 83, 42, 85, 43, 87, 44, 89, 45, 91, 46, 93, 47, 95, 48, 97, 49, 99, 50, 101, 51, 103, 52, 105, 53, 107, 54, 109, 55, 111, 56, 113, 57, 115, 58, 117, 59, 119, 60, 121, 61, 123, 0, 125, 0, 127, 0, 129, 0, 131, 0, 133, 0, 135, 0, 137, 0, 1, 0, 2, 9, 0, 33, 33, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 93, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 359, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 0, 71, 1, 0, 0, 0, 0, 73, 1, 0, 0, 0, 0, 75, 1, 0, 0, 0, 0, 77, 1, 0, 0, 0, 0, 79, 1, 0, 0, 0, 0, 81, 1, 0, 0, 0, 0, 83, 1, 0, 0, 0, 0, 85, 1, 0, 0, 0, 0, 87, 1, 0, 0, 0, 0, 89, 1, 0, 0, 0, 0, 91, 1, 0, 0, 0, 0, 93, 1, 0, 0, 0, 0, 95, 1, 0, 0, 0, 0, 97, 1, 0, 0, 0, 0, 99, 1, 0, 0, 0, 0, 101, 1, 0, 0, 0, 0, 103, 1, 0, 0, 0, 0, 105, 1, 0, 0, 0, 0, 107, 1, 0, 0, 0, 0, 109, 1, 0, 0, 0, 0, 111, 1, 0, 0, 0, 0, 113, 1, 0, 0, 0, 0, 115, 1, 0, 0, 0, 0, 117, 1, 0, 0, 0, 0, 119, 1, 0, 0, 0, 0, 121, 1, 0, 0, 0, 1, 139, 1, 0, 0, 0, 3, 141, 1, 0, 0, 0, 5, 143, 1, 0, 0, 0, 7, 145, 1, 0, 0, 0, 9, 147, 1, 0, 0, 0, 11, 152, 1, 0, 0, 0, 13, 155, 1, 0, 0, 0, 15, 157, 1, 0, 0, 0, 17, 159, 1, 0, 0, 0, 19, 161, 1, 0, 0, 0, 21, 163, 1, 0, 0, 0, 23, 165, 1, 0, 0, 0, 25, 167, 1, 0, 0, 0, 27, 169, 1, 0, 0, 0, 29, 171, 1, 0, 0, 0, 31, 173, 1, 0, 0, 0, 33, 175, 1, 0, 0, 0, 35, 177, 1, 0, 0, 0, 37, 180, 1, 0, 0, 0, 39, 183, 1, 0, 0, 0, 41, 185, 1, 0, 0, 0, 43, 192, 1, 0, 0, 0, 45, 199, 1, 0, 0, 0, 47, 208, 1, 0, 0, 0, 49, 213, 1, 0, 0, 0, 51, 219, 1, 0, 0, 0, 53, 223, 1, 0, 0, 0, 55, 225, 1, 0, 0, 0, 57, 227, 1, 0, 0, 0, 59, 238, 1, 0, 0, 0, 61, 243, 1, 0, 0, 0, 63, 246, 1, 0, 0, 0, 65, 249, 1, 0, 0, 0, 67, 252, 1, 0, 0, 0, 69, 255, 1, 0, 0, 0, 71, 263, 1, 0, 0, 0, 73, 270, 1, 0, 0, 0, 75, 277, 1, 0, 0, 0, 77, 285, 1, 0, 0, 0, 79, 289, 1, 0, 0, 0, 81, 295, 1, 0, 0, 0, 83, 297, 1, 0, 0, 0, 85, 299, 1, 0, 0, 0, 87, 301, 1, 0, 0, 0, 89, 303, 1, 0, 0, 0, 91, 305, 1, 0, 0, 0, 93, 307, 1, 0, 0, 0, 95, 309, 1, 0, 0, 0, 97, 311, 1, 0, 0, 0, 99, 313, 1, 0, 0, 0, 101, 315, 1, 0, 0, 0, 103, 317, 1, 0, 0, 0, 105, 319, 1, 0, 0, 0, 107, 321, 1, 0, 0, 0, 109, 323, 1, 0, 0, 0, 111, 325, 1, 0, 0, 0, 113, 327, 1, 0, 0, 0, 115, 329, 1, 0, 0, 0, 117, 331, 1, 0, 0, 0, 119, 333, 1, 0, 0, 0, 121, 335, 1, 0, 0, 0, 123, 337, 1, 0, 0, 0, 125, 339, 1, 0, 0, 0, 127, 343, 1, 0, 0, 0, 129, 345, 1, 0, 0, 0, 131, 347, 1, 0, 0, 0, 133, 349, 1, 0, 0, 0, 135, 353, 1, 0, 0, 0, 137, 357, 1, 0, 0, 0, 139, 140, 5, 83, 0, 0, 140, 2, 1, 0, 0, 0, 141, 142, 5, 87, 0, 0, 142, 4, 1, 0, 0, 0, 143, 144, 5, 79, 0, 0, 144, 6, 1, 0, 0, 0, 145, 146, 5, 71, 0, 0, 146, 8, 1, 0, 0, 0, 147, 148, 5, 110, 0, 0, 148, 149, 5, 111, 0, 0, 149, 150, 5, 116, 0, 0, 150, 151, 5, 101, 0, 0, 151, 10, 1, 0, 0, 0, 152, 153, 5, 111, 0, 0, 153, 154, 5, 114, 0, 0, 154, 12, 1, 0, 0, 0, 155, 156, 5, 49, 0, 0, 156, 14, 1, 0, 0, 0, 157, 158, 5, 50, 0, 0, 158, 16, 1, 0, 0, 0, 159, 160, 5, 51, 0, 0, 160, 18, 1, 0, 0, 0, 161, 162, 5, 52, 0, 0, 162, 20, 1, 0, 0, 0, 163, 164, 5, 53, 0, 0, 164, 22, 1, 0, 0, 0, 165, 166, 5, 54, 0, 0, 166, 24, 1, 0, 0, 0, 167, 168, 5, 55, 0, 0, 168, 26, 1, 0, 0, 0, 169, 170, 5, 56, 0, 0, 170, 28, 1, 0, 0, 0, 171, 172, 5, 57, 0, 0, 172, 30, 1, 0, 0, 0, 173, 174, 5, 33, 0, 0, 174, 32, 1, 0, 0, 0, 175, 176, 5, 48, 0, 0, 176, 34, 1, 0, 0, 0, 177, 178, 5, 60, 0, 0, 178, 179, 5, 61, 0, 0, 179, 36, 1, 0, 0, 0, 180, 181, 5, 62, 0, 0, 181, 182, 5, 61, 0, 0, 182, 38, 1, 0, 0, 0, 183, 184, 5, 99, 0, 0, 184, 40, 1, 0, 0, 0, 185, 186, 5, 99, 0, 0, 186, 187, 5, 114, 0, 0, 187, 188, 5, 101, 0, 0, 188, 189, 5, 97, 0, 0, 189, 190, 5, 116, 0, 0, 190, 191, 5, 101, 0, 0, 191, 42, 1, 0, 0, 0, 192, 193, 5, 109, 0, 0, 193, 194, 5, 111, 0, 0, 194, 195, 5, 100, 0, 0, 195, 196, 5, 105, 0, 0, 196, 197, 5, 102, 0, 0, 197, 198, 5, 121, 0, 0, 198, 44, 1, 0, 0, 0, 199, 200, 5, 112, 0, 0, 200, 201, 5, 114, 0, 0, 201, 202, 5, 105, 0, 0, 202, 203, 5, 111, 0, 0, 203, 204, 5, 114, 0, 0, 204, 205, 5, 105, 0, 0, 205, 206, 5, 116, 0, 0, 206, 207, 5, 121, 0, 0, 207, 46, 1, 0, 0, 0, 208, 209, 5, 102, 0, 0, 209, 210, 5, 105, 0, 0, 210, 211, 5, 108, 0, 0, 211, 212, 5, 101, 0, 0, 212, 48, 1, 0, 0, 0, 213, 214, 5, 116, 0, 0, 214, 215, 5, 121, 0, 0, 215, 216, 5, 112, 0, 0, 216, 217, 5, 101, 0, 0, 217, 50, 1, 0, 0, 0, 218, 220, 5, 13, 0, 0, 219, 218, 1, 0, 0, 0, 219, 220, 1, 0, 0, 0, 220, 221, 1, 0, 0, 0, 221, 222, 5, 10, 0, 0, 222, 52, 1, 0, 0, 0, 223, 224, 5, 111, 0, 0, 224, 54, 1, 0, 0, 0, 225, 226, 5, 120, 0, 0, 226, 56, 1, 0, 0, 0, 227, 228, 5, 50, 0, 0, 228, 229, 3, 129, 64, 0, 229, 230, 3, 129, 64, 0, 230, 231, 3, 129, 64, 0, 231, 232, 3, 87, 43, 0, 232, 233, 3, 133, 66, 0, 233, 234, 3, 129, 64, 0, 234, 235, 3, 87, 43, 0, 235, 236, 3, 131, 65, 0, 236, 237, 3, 129, 64, 0, 237, 58, 1, 0, 0, 0, 238, 239, 2, 48, 50, 0, 239, 240, 3, 129, 64, 0, 240, 241, 2, 48, 53, 0, 241, 242, 3, 129, 64, 0, 242, 60, 1, 0, 0, 0, 243, 244, 3, 85, 42, 0, 244, 245, 3, 73, 36, 0, 245, 62, 1, 0, 0, 0, 246, 247, 3, 83, 41, 0, 247, 248, 3, 73, 36, 0, 248, 64, 1, 0, 0, 0, 249, 250, 3, 121, 60, 0, 250, 251, 3, 73, 36, 0, 251, 66, 1, 0, 0, 0, 252, 253, 5, 80, 0, 0, 253, 254, 3, 129, 64, 0, 254, 68, 1, 0, 0, 0, 255, 260, 3, 137, 68, 0, 256, 259, 3, 137, 68, 0, 257, 259, 3, 93, 46, 0, 258, 256, 1, 0, 0, 0, 258, 257, 1, 0, 0, 0, 259, 262, 1, 0, 0, 0, 260, 258, 1, 0, 0, 0, 260, 261, 1, 0, 0, 0, 261, 70, 1, 0, 0, 0, 262, 260, 1, 0, 0, 0, 263, 264, 3, 73, 36, 0, 264, 265, 3, 101, 50, 0, 265, 266, 3, 127, 63, 0, 266, 268, 3, 127, 63, 0, 267, 269, 3, 127, 63, 0, 268, 267, 1, 0, 0, 0, 268, 269, 1, 0, 0, 0, 269, 72, 1, 0, 0, 0, 270, 271, 3, 129, 64, 0, 271, 272, 3, 129, 64, 0, 272, 273, 3, 133, 66, 0, 273, 274, 3, 129, 64, 0, 274, 275, 3, 131, 65, 0, 275, 276, 3, 129, 64, 0, 276, 74, 1, 0, 0, 0, 277, 282, 3, 129, 64, 0, 278, 281, 3, 137, 68, 0, 279, 281, 3, 93, 46, 0, 280, 278, 1, 0, 0, 0, 280, 279, 1, 0, 0, 0, 281, 284, 1, 0, 0, 0, 282, 280, 1, 0, 0, 0, 282, 283, 1, 0, 0, 0, 283, 76, 1, 0, 0, 0, 284, 282, 1, 0, 0, 0, 285, 286, 5, 32, 0, 0, 286, 287, 5, 32, 0, 0, 287, 288, 5, 45, 0, 0, 288, 78, 1, 0, 0, 0, 289, 290, 5, 32, 0, 0, 290, 291, 5, 32, 0, 0, 291, 292, 5, 32, 0, 0, 292, 293, 5, 32, 0, 0, 293, 294, 5, 45, 0, 0, 294, 80, 1, 0, 0, 0, 295, 296, 7, 0, 0, 0, 296, 82, 1, 0, 0, 0, 297, 298, 5, 36, 0, 0, 298, 84, 1, 0, 0, 0, 299, 300, 5, 94, 0, 0, 300, 86, 1, 0, 0, 0, 301, 302, 5, 45, 0, 0, 302, 88, 1, 0, 0, 0, 303, 304, 5, 46, 0, 0, 304, 90, 1, 0, 0, 0, 305, 306, 5, 47, 0, 0, 306, 92, 1, 0, 0, 0, 307, 308, 5, 95, 0, 0, 308, 94, 1, 0, 0, 0, 309, 310, 5, 32, 0, 0, 310, 96, 1, 0, 0, 0, 311, 312, 5, 40, 0, 0, 312, 98, 1, 0, 0, 0, 313, 314, 5, 41, 0, 0, 314, 100, 1, 0, 0, 0, 315, 316, 5, 35, 0, 0, 316, 102, 1, 0, 0, 0, 317, 318, 5, 64, 0, 0, 318, 104, 1, 0, 0, 0, 319, 320, 5, 43, 0, 0, 320, 106, 1, 0, 0, 0, 321, 322, 5, 37, 0, 0, 322, 108, 1, 0, 0, 0, 323, 324, 5, 39, 0, 0, 324, 110, 1, 0, 0, 0, 325, 326, 5, 34, 0, 0, 326, 112, 1, 0, 0, 0, 327, 328, 5, 126, 0, 0, 328, 114, 1, 0, 0, 0, 329, 330, 5, 42, 0, 0, 330, 116, 1, 0, 0, 0, 331, 332, 5, 60, 0, 0, 332, 118, 1, 0, 0, 0, 333, 334, 5, 62, 0, 0, 334, 120, 1, 0, 0, 0, 335, 336, 5, 58, 0, 0, 336, 122, 1, 0, 0, 0, 337, 338, 2, 65, 90, 0, 338, 124, 1, 0, 0, 0, 339, 340, 2, 97, 122, 0, 340, 126, 1, 0, 0, 0, 341, 344, 3, 129, 64, 0, 342, 344, 7, 1, 0, 0, 343, 341, 1, 0, 0, 0, 343, 342, 1, 0, 0, 0, 344, 128, 1, 0, 0, 0, 345, 346, 2, 48, 57, 0, 346, 130, 1, 0, 0, 0, 347, 348, 2, 48, 51, 0, 348, 132, 1, 0, 0, 0, 349, 350, 2, 48, 49, 0, 350, 134, 1, 0, 0, 0, 351, 354, 3, 123, 61, 0, 352, 354, 3, 125, 62, 0, 353, 351, 1, 0, 0, 0, 353, 352, 1, 0, 0, 0, 354, 136, 1, 0, 0, 0, 355, 358, 3, 135, 67, 0, 356, 358, 3, 129, 64, 0, 357, 355, 1, 0, 0, 0, 357, 356, 1, 0, 0, 0, 358, 138, 1, 0, 0, 0, 10, 0, 219, 258, 260, 268, 280, 282, 343, 353, 357, 0]
+[4, 0, 62, 364, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 2, 48, 7, 48, 2, 49, 7, 49, 2, 50, 7, 50, 2, 51, 7, 51, 2, 52, 7, 52, 2, 53, 7, 53, 2, 54, 7, 54, 2, 55, 7, 55, 2, 56, 7, 56, 2, 57, 7, 57, 2, 58, 7, 58, 2, 59, 7, 59, 2, 60, 7, 60, 2, 61, 7, 61, 2, 62, 7, 62, 2, 63, 7, 63, 2, 64, 7, 64, 2, 65, 7, 65, 2, 66, 7, 66, 2, 67, 7, 67, 2, 68, 7, 68, 2, 69, 7, 69, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 11, 1, 11, 1, 12, 1, 12, 1, 13, 1, 13, 1, 14, 1, 14, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 17, 1, 18, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 25, 1, 25, 1, 25, 1, 25, 1, 25, 1, 26, 3, 26, 225, 8, 26, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 29, 1, 30, 1, 30, 1, 30, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 5, 35, 264, 8, 35, 10, 35, 12, 35, 267, 9, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 3, 36, 274, 8, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 5, 38, 286, 8, 38, 10, 38, 12, 38, 289, 9, 38, 1, 39, 1, 39, 1, 39, 1, 39, 1, 40, 1, 40, 1, 40, 1, 40, 1, 40, 1, 40, 1, 41, 1, 41, 1, 42, 1, 42, 1, 43, 1, 43, 1, 44, 1, 44, 1, 45, 1, 45, 1, 46, 1, 46, 1, 47, 1, 47, 1, 48, 1, 48, 1, 49, 1, 49, 1, 50, 1, 50, 1, 51, 1, 51, 1, 52, 1, 52, 1, 53, 1, 53, 1, 54, 1, 54, 1, 55, 1, 55, 1, 56, 1, 56, 1, 57, 1, 57, 1, 58, 1, 58, 1, 59, 1, 59, 1, 60, 1, 60, 1, 61, 1, 61, 1, 62, 1, 62, 1, 63, 1, 63, 1, 64, 1, 64, 3, 64, 349, 8, 64, 1, 65, 1, 65, 1, 66, 1, 66, 1, 67, 1, 67, 1, 68, 1, 68, 3, 68, 359, 8, 68, 1, 69, 1, 69, 3, 69, 363, 8, 69, 0, 0, 70, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 36, 73, 37, 75, 38, 77, 39, 79, 40, 81, 41, 83, 42, 85, 43, 87, 44, 89, 45, 91, 46, 93, 47, 95, 48, 97, 49, 99, 50, 101, 51, 103, 52, 105, 53, 107, 54, 109, 55, 111, 56, 113, 57, 115, 58, 117, 59, 119, 60, 121, 61, 123, 62, 125, 0, 127, 0, 129, 0, 131, 0, 133, 0, 135, 0, 137, 0, 139, 0, 1, 0, 2, 9, 0, 33, 33, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 93, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 364, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 0, 71, 1, 0, 0, 0, 0, 73, 1, 0, 0, 0, 0, 75, 1, 0, 0, 0, 0, 77, 1, 0, 0, 0, 0, 79, 1, 0, 0, 0, 0, 81, 1, 0, 0, 0, 0, 83, 1, 0, 0, 0, 0, 85, 1, 0, 0, 0, 0, 87, 1, 0, 0, 0, 0, 89, 1, 0, 0, 0, 0, 91, 1, 0, 0, 0, 0, 93, 1, 0, 0, 0, 0, 95, 1, 0, 0, 0, 0, 97, 1, 0, 0, 0, 0, 99, 1, 0, 0, 0, 0, 101, 1, 0, 0, 0, 0, 103, 1, 0, 0, 0, 0, 105, 1, 0, 0, 0, 0, 107, 1, 0, 0, 0, 0, 109, 1, 0, 0, 0, 0, 111, 1, 0, 0, 0, 0, 113, 1, 0, 0, 0, 0, 115, 1, 0, 0, 0, 0, 117, 1, 0, 0, 0, 0, 119, 1, 0, 0, 0, 0, 121, 1, 0, 0, 0, 0, 123, 1, 0, 0, 0, 1, 141, 1, 0, 0, 0, 3, 143, 1, 0, 0, 0, 5, 145, 1, 0, 0, 0, 7, 147, 1, 0, 0, 0, 9, 149, 1, 0, 0, 0, 11, 154, 1, 0, 0, 0, 13, 157, 1, 0, 0, 0, 15, 159, 1, 0, 0, 0, 17, 161, 1, 0, 0, 0, 19, 163, 1, 0, 0, 0, 21, 165, 1, 0, 0, 0, 23, 167, 1, 0, 0, 0, 25, 169, 1, 0, 0, 0, 27, 171, 1, 0, 0, 0, 29, 173, 1, 0, 0, 0, 31, 175, 1, 0, 0, 0, 33, 177, 1, 0, 0, 0, 35, 179, 1, 0, 0, 0, 37, 182, 1, 0, 0, 0, 39, 185, 1, 0, 0, 0, 41, 187, 1, 0, 0, 0, 43, 190, 1, 0, 0, 0, 45, 197, 1, 0, 0, 0, 47, 204, 1, 0, 0, 0, 49, 213, 1, 0, 0, 0, 51, 218, 1, 0, 0, 0, 53, 224, 1, 0, 0, 0, 55, 228, 1, 0, 0, 0, 57, 230, 1, 0, 0, 0, 59, 232, 1, 0, 0, 0, 61, 243, 1, 0, 0, 0, 63, 248, 1, 0, 0, 0, 65, 251, 1, 0, 0, 0, 67, 254, 1, 0, 0, 0, 69, 257, 1, 0, 0, 0, 71, 260, 1, 0, 0, 0, 73, 268, 1, 0, 0, 0, 75, 275, 1, 0, 0, 0, 77, 282, 1, 0, 0, 0, 79, 290, 1, 0, 0, 0, 81, 294, 1, 0, 0, 0, 83, 300, 1, 0, 0, 0, 85, 302, 1, 0, 0, 0, 87, 304, 1, 0, 0, 0, 89, 306, 1, 0, 0, 0, 91, 308, 1, 0, 0, 0, 93, 310, 1, 0, 0, 0, 95, 312, 1, 0, 0, 0, 97, 314, 1, 0, 0, 0, 99, 316, 1, 0, 0, 0, 101, 318, 1, 0, 0, 0, 103, 320, 1, 0, 0, 0, 105, 322, 1, 0, 0, 0, 107, 324, 1, 0, 0, 0, 109, 326, 1, 0, 0, 0, 111, 328, 1, 0, 0, 0, 113, 330, 1, 0, 0, 0, 115, 332, 1, 0, 0, 0, 117, 334, 1, 0, 0, 0, 119, 336, 1, 0, 0, 0, 121, 338, 1, 0, 0, 0, 123, 340, 1, 0, 0, 0, 125, 342, 1, 0, 0, 0, 127, 344, 1, 0, 0, 0, 129, 348, 1, 0, 0, 0, 131, 350, 1, 0, 0, 0, 133, 352, 1, 0, 0, 0, 135, 354, 1, 0, 0, 0, 137, 358, 1, 0, 0, 0, 139, 362, 1, 0, 0, 0, 141, 142, 5, 83, 0, 0, 142, 2, 1, 0, 0, 0, 143, 144, 5, 87, 0, 0, 144, 4, 1, 0, 0, 0, 145, 146, 5, 79, 0, 0, 146, 6, 1, 0, 0, 0, 147, 148, 5, 71, 0, 0, 148, 8, 1, 0, 0, 0, 149, 150, 5, 110, 0, 0, 150, 151, 5, 111, 0, 0, 151, 152, 5, 116, 0, 0, 152, 153, 5, 101, 0, 0, 153, 10, 1, 0, 0, 0, 154, 155, 5, 111, 0, 0, 155, 156, 5, 114, 0, 0, 156, 12, 1, 0, 0, 0, 157, 158, 5, 49, 0, 0, 158, 14, 1, 0, 0, 0, 159, 160, 5, 50, 0, 0, 160, 16, 1, 0, 0, 0, 161, 162, 5, 51, 0, 0, 162, 18, 1, 0, 0, 0, 163, 164, 5, 52, 0, 0, 164, 20, 1, 0, 0, 0, 165, 166, 5, 53, 0, 0, 166, 22, 1, 0, 0, 0, 167, 168, 5, 54, 0, 0, 168, 24, 1, 0, 0, 0, 169, 170, 5, 55, 0, 0, 170, 26, 1, 0, 0, 0, 171, 172, 5, 56, 0, 0, 172, 28, 1, 0, 0, 0, 173, 174, 5, 57, 0, 0, 174, 30, 1, 0, 0, 0, 175, 176, 5, 33, 0, 0, 176, 32, 1, 0, 0, 0, 177, 178, 5, 48, 0, 0, 178, 34, 1, 0, 0, 0, 179, 180, 5, 60, 0, 0, 180, 181, 5, 61, 0, 0, 181, 36, 1, 0, 0, 0, 182, 183, 5, 62, 0, 0, 183, 184, 5, 61, 0, 0, 184, 38, 1, 0, 0, 0, 185, 186, 5, 99, 0, 0, 186, 40, 1, 0, 0, 0, 187, 188, 5, 102, 0, 0, 188, 189, 5, 61, 0, 0, 189, 42, 1, 0, 0, 0, 190, 191, 5, 99, 0, 0, 191, 192, 5, 114, 0, 0, 192, 193, 5, 101, 0, 0, 193, 194, 5, 97, 0, 0, 194, 195, 5, 116, 0, 0, 195, 196, 5, 101, 0, 0, 196, 44, 1, 0, 0, 0, 197, 198, 5, 109, 0, 0, 198, 199, 5, 111, 0, 0, 199, 200, 5, 100, 0, 0, 200, 201, 5, 105, 0, 0, 201, 202, 5, 102, 0, 0, 202, 203, 5, 121, 0, 0, 203, 46, 1, 0, 0, 0, 204, 205, 5, 112, 0, 0, 205, 206, 5, 114, 0, 0, 206, 207, 5, 105, 0, 0, 207, 208, 5, 111, 0, 0, 208, 209, 5, 114, 0, 0, 209, 210, 5, 105, 0, 0, 210, 211, 5, 116, 0, 0, 211, 212, 5, 121, 0, 0, 212, 48, 1, 0, 0, 0, 213, 214, 5, 102, 0, 0, 214, 215, 5, 105, 0, 0, 215, 216, 5, 108, 0, 0, 216, 217, 5, 101, 0, 0, 217, 50, 1, 0, 0, 0, 218, 219, 5, 116, 0, 0, 219, 220, 5, 121, 0, 0, 220, 221, 5, 112, 0, 0, 221, 222, 5, 101, 0, 0, 222, 52, 1, 0, 0, 0, 223, 225, 5, 13, 0, 0, 224, 223, 1, 0, 0, 0, 224, 225, 1, 0, 0, 0, 225, 226, 1, 0, 0, 0, 226, 227, 5, 10, 0, 0, 227, 54, 1, 0, 0, 0, 228, 229, 5, 111, 0, 0, 229, 56, 1, 0, 0, 0, 230, 231, 5, 120, 0, 0, 231, 58, 1, 0, 0, 0, 232, 233, 5, 50, 0, 0, 233, 234, 3, 131, 65, 0, 234, 235, 3, 131, 65, 0, 235, 236, 3, 131, 65, 0, 236, 237, 3, 89, 44, 0, 237, 238, 3, 135, 67, 0, 238, 239, 3, 131, 65, 0, 239, 240, 3, 89, 44, 0, 240, 241, 3, 133, 66, 0, 241, 242, 3, 131, 65, 0, 242, 60, 1, 0, 0, 0, 243, 244, 2, 48, 50, 0, 244, 245, 3, 131, 65, 0, 245, 246, 2, 48, 53, 0, 246, 247, 3, 131, 65, 0, 247, 62, 1, 0, 0, 0, 248, 249, 3, 87, 43, 0, 249, 250, 3, 75, 37, 0, 250, 64, 1, 0, 0, 0, 251, 252, 3, 85, 42, 0, 252, 253, 3, 75, 37, 0, 253, 66, 1, 0, 0, 0, 254, 255, 3, 123, 61, 0, 255, 256, 3, 75, 37, 0, 256, 68, 1, 0, 0, 0, 257, 258, 5, 80, 0, 0, 258, 259, 3, 131, 65, 0, 259, 70, 1, 0, 0, 0, 260, 265, 3, 139, 69, 0, 261, 264, 3, 139, 69, 0, 262, 264, 3, 95, 47, 0, 263, 261, 1, 0, 0, 0, 263, 262, 1, 0, 0, 0, 264, 267, 1, 0, 0, 0, 265, 263, 1, 0, 0, 0, 265, 266, 1, 0, 0, 0, 266, 72, 1, 0, 0, 0, 267, 265, 1, 0, 0, 0, 268, 269, 3, 75, 37, 0, 269, 270, 3, 103, 51, 0, 270, 271, 3, 129, 64, 0, 271, 273, 3, 129, 64, 0, 272, 274, 3, 129, 64, 0, 273, 272, 1, 0, 0, 0, 273, 274, 1, 0, 0, 0, 274, 74, 1, 0, 0, 0, 275, 276, 3, 131, 65, 0, 276, 277, 3, 131, 65, 0, 277, 278, 3, 135, 67, 0, 278, 279, 3, 131, 65, 0, 279, 280, 3, 133, 66, 0, 280, 281, 3, 131, 65, 0, 281, 76, 1, 0, 0, 0, 282, 287, 3, 131, 65, 0, 283, 286, 3, 139, 69, 0, 284, 286, 3, 95, 47, 0, 285, 283, 1, 0, 0, 0, 285, 284, 1, 0, 0, 0, 286, 289, 1, 0, 0, 0, 287, 285, 1, 0, 0, 0, 287, 288, 1, 0, 0, 0, 288, 78, 1, 0, 0, 0, 289, 287, 1, 0, 0, 0, 290, 291, 5, 32, 0, 0, 291, 292, 5, 32, 0, 0, 292, 293, 5, 45, 0, 0, 293, 80, 1, 0, 0, 0, 294, 295, 5, 32, 0, 0, 295, 296, 5, 32, 0, 0, 296, 297, 5, 32, 0, 0, 297, 298, 5, 32, 0, 0, 298, 299, 5, 45, 0, 0, 299, 82, 1, 0, 0, 0, 300, 301, 7, 0, 0, 0, 301, 84, 1, 0, 0, 0, 302, 303, 5, 36, 0, 0, 303, 86, 1, 0, 0, 0, 304, 305, 5, 94, 0, 0, 305, 88, 1, 0, 0, 0, 306, 307, 5, 45, 0, 0, 307, 90, 1, 0, 0, 0, 308, 309, 5, 46, 0, 0, 309, 92, 1, 0, 0, 0, 310, 311, 5, 47, 0, 0, 311, 94, 1, 0, 0, 0, 312, 313, 5, 95, 0, 0, 313, 96, 1, 0, 0, 0, 314, 315, 5, 32, 0, 0, 315, 98, 1, 0, 0, 0, 316, 317, 5, 40, 0, 0, 317, 100, 1, 0, 0, 0, 318, 319, 5, 41, 0, 0, 319, 102, 1, 0, 0, 0, 320, 321, 5, 35, 0, 0, 321, 104, 1, 0, 0, 0, 322, 323, 5, 64, 0, 0, 323, 106, 1, 0, 0, 0, 324, 325, 5, 43, 0, 0, 325, 108, 1, 0, 0, 0, 326, 327, 5, 37, 0, 0, 327, 110, 1, 0, 0, 0, 328, 329, 5, 39, 0, 0, 329, 112, 1, 0, 0, 0, 330, 331, 5, 34, 0, 0, 331, 114, 1, 0, 0, 0, 332, 333, 5, 126, 0, 0, 333, 116, 1, 0, 0, 0, 334, 335, 5, 42, 0, 0, 335, 118, 1, 0, 0, 0, 336, 337, 5, 60, 0, 0, 337, 120, 1, 0, 0, 0, 338, 339, 5, 62, 0, 0, 339, 122, 1, 0, 0, 0, 340, 341, 5, 58, 0, 0, 341, 124, 1, 0, 0, 0, 342, 343, 2, 65, 90, 0, 343, 126, 1, 0, 0, 0, 344, 345, 2, 97, 122, 0, 345, 128, 1, 0, 0, 0, 346, 349, 3, 131, 65, 0, 347, 349, 7, 1, 0, 0, 348, 346, 1, 0, 0, 0, 348, 347, 1, 0, 0, 0, 349, 130, 1, 0, 0, 0, 350, 351, 2, 48, 57, 0, 351, 132, 1, 0, 0, 0, 352, 353, 2, 48, 51, 0, 353, 134, 1, 0, 0, 0, 354, 355, 2, 48, 49, 0, 355, 136, 1, 0, 0, 0, 356, 359, 3, 125, 62, 0, 357, 359, 3, 127, 63, 0, 358, 356, 1, 0, 0, 0, 358, 357, 1, 0, 0, 0, 359, 138, 1, 0, 0, 0, 360, 363, 3, 137, 68, 0, 361, 363, 3, 131, 65, 0, 362, 360, 1, 0, 0, 0, 362, 361, 1, 0, 0, 0, 363, 140, 1, 0, 0, 0, 10, 0, 224, 263, 265, 273, 285, 287, 348, 358, 362, 0]
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.py` & `zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,139 +6,141 @@
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     return [
-        4,0,61,359,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
+        4,0,62,364,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
         2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,
         13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,
         19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,
         26,7,26,2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,
         32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,
         39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,
         45,2,46,7,46,2,47,7,47,2,48,7,48,2,49,7,49,2,50,7,50,2,51,7,51,2,
         52,7,52,2,53,7,53,2,54,7,54,2,55,7,55,2,56,7,56,2,57,7,57,2,58,7,
         58,2,59,7,59,2,60,7,60,2,61,7,61,2,62,7,62,2,63,7,63,2,64,7,64,2,
-        65,7,65,2,66,7,66,2,67,7,67,2,68,7,68,1,0,1,0,1,1,1,1,1,2,1,2,1,
-        3,1,3,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,6,1,6,1,7,1,7,1,8,1,8,1,
-        9,1,9,1,10,1,10,1,11,1,11,1,12,1,12,1,13,1,13,1,14,1,14,1,15,1,15,
-        1,16,1,16,1,17,1,17,1,17,1,18,1,18,1,18,1,19,1,19,1,20,1,20,1,20,
-        1,20,1,20,1,20,1,20,1,21,1,21,1,21,1,21,1,21,1,21,1,21,1,22,1,22,
-        1,22,1,22,1,22,1,22,1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,23,1,24,
-        1,24,1,24,1,24,1,24,1,25,3,25,220,8,25,1,25,1,25,1,26,1,26,1,27,
-        1,27,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,29,
-        1,29,1,29,1,29,1,29,1,30,1,30,1,30,1,31,1,31,1,31,1,32,1,32,1,32,
-        1,33,1,33,1,33,1,34,1,34,1,34,5,34,259,8,34,10,34,12,34,262,9,34,
-        1,35,1,35,1,35,1,35,1,35,3,35,269,8,35,1,36,1,36,1,36,1,36,1,36,
-        1,36,1,36,1,37,1,37,1,37,5,37,281,8,37,10,37,12,37,284,9,37,1,38,
-        1,38,1,38,1,38,1,39,1,39,1,39,1,39,1,39,1,39,1,40,1,40,1,41,1,41,
-        1,42,1,42,1,43,1,43,1,44,1,44,1,45,1,45,1,46,1,46,1,47,1,47,1,48,
-        1,48,1,49,1,49,1,50,1,50,1,51,1,51,1,52,1,52,1,53,1,53,1,54,1,54,
-        1,55,1,55,1,56,1,56,1,57,1,57,1,58,1,58,1,59,1,59,1,60,1,60,1,61,
-        1,61,1,62,1,62,1,63,1,63,3,63,344,8,63,1,64,1,64,1,65,1,65,1,66,
-        1,66,1,67,1,67,3,67,354,8,67,1,68,1,68,3,68,358,8,68,0,0,69,1,1,
-        3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,27,14,
-        29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,49,25,
-        51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,71,36,
-        73,37,75,38,77,39,79,40,81,41,83,42,85,43,87,44,89,45,91,46,93,47,
-        95,48,97,49,99,50,101,51,103,52,105,53,107,54,109,55,111,56,113,
-        57,115,58,117,59,119,60,121,61,123,0,125,0,127,0,129,0,131,0,133,
-        0,135,0,137,0,1,0,2,9,0,33,33,38,38,44,44,59,59,61,61,63,63,91,93,
-        96,96,123,125,6,0,65,72,74,78,80,90,97,105,107,107,109,122,359,0,
-        1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,
-        0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,
-        0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,
-        0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,
-        0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,
-        0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,
-        0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,0,0,69,1,0,0,0,0,71,1,
-        0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,0,0,79,1,0,0,0,0,81,1,
-        0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,1,0,0,0,0,89,1,0,0,0,0,91,1,
-        0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,1,0,0,0,0,99,1,0,0,0,0,101,
-        1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,107,1,0,0,0,0,109,1,0,0,0,
-        0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,0,0,0,117,1,0,0,0,0,119,1,
-        0,0,0,0,121,1,0,0,0,1,139,1,0,0,0,3,141,1,0,0,0,5,143,1,0,0,0,7,
-        145,1,0,0,0,9,147,1,0,0,0,11,152,1,0,0,0,13,155,1,0,0,0,15,157,1,
-        0,0,0,17,159,1,0,0,0,19,161,1,0,0,0,21,163,1,0,0,0,23,165,1,0,0,
-        0,25,167,1,0,0,0,27,169,1,0,0,0,29,171,1,0,0,0,31,173,1,0,0,0,33,
-        175,1,0,0,0,35,177,1,0,0,0,37,180,1,0,0,0,39,183,1,0,0,0,41,185,
-        1,0,0,0,43,192,1,0,0,0,45,199,1,0,0,0,47,208,1,0,0,0,49,213,1,0,
-        0,0,51,219,1,0,0,0,53,223,1,0,0,0,55,225,1,0,0,0,57,227,1,0,0,0,
-        59,238,1,0,0,0,61,243,1,0,0,0,63,246,1,0,0,0,65,249,1,0,0,0,67,252,
-        1,0,0,0,69,255,1,0,0,0,71,263,1,0,0,0,73,270,1,0,0,0,75,277,1,0,
-        0,0,77,285,1,0,0,0,79,289,1,0,0,0,81,295,1,0,0,0,83,297,1,0,0,0,
-        85,299,1,0,0,0,87,301,1,0,0,0,89,303,1,0,0,0,91,305,1,0,0,0,93,307,
-        1,0,0,0,95,309,1,0,0,0,97,311,1,0,0,0,99,313,1,0,0,0,101,315,1,0,
-        0,0,103,317,1,0,0,0,105,319,1,0,0,0,107,321,1,0,0,0,109,323,1,0,
-        0,0,111,325,1,0,0,0,113,327,1,0,0,0,115,329,1,0,0,0,117,331,1,0,
-        0,0,119,333,1,0,0,0,121,335,1,0,0,0,123,337,1,0,0,0,125,339,1,0,
-        0,0,127,343,1,0,0,0,129,345,1,0,0,0,131,347,1,0,0,0,133,349,1,0,
-        0,0,135,353,1,0,0,0,137,357,1,0,0,0,139,140,5,83,0,0,140,2,1,0,0,
-        0,141,142,5,87,0,0,142,4,1,0,0,0,143,144,5,79,0,0,144,6,1,0,0,0,
-        145,146,5,71,0,0,146,8,1,0,0,0,147,148,5,110,0,0,148,149,5,111,0,
-        0,149,150,5,116,0,0,150,151,5,101,0,0,151,10,1,0,0,0,152,153,5,111,
-        0,0,153,154,5,114,0,0,154,12,1,0,0,0,155,156,5,49,0,0,156,14,1,0,
-        0,0,157,158,5,50,0,0,158,16,1,0,0,0,159,160,5,51,0,0,160,18,1,0,
-        0,0,161,162,5,52,0,0,162,20,1,0,0,0,163,164,5,53,0,0,164,22,1,0,
-        0,0,165,166,5,54,0,0,166,24,1,0,0,0,167,168,5,55,0,0,168,26,1,0,
-        0,0,169,170,5,56,0,0,170,28,1,0,0,0,171,172,5,57,0,0,172,30,1,0,
-        0,0,173,174,5,33,0,0,174,32,1,0,0,0,175,176,5,48,0,0,176,34,1,0,
-        0,0,177,178,5,60,0,0,178,179,5,61,0,0,179,36,1,0,0,0,180,181,5,62,
-        0,0,181,182,5,61,0,0,182,38,1,0,0,0,183,184,5,99,0,0,184,40,1,0,
-        0,0,185,186,5,99,0,0,186,187,5,114,0,0,187,188,5,101,0,0,188,189,
-        5,97,0,0,189,190,5,116,0,0,190,191,5,101,0,0,191,42,1,0,0,0,192,
-        193,5,109,0,0,193,194,5,111,0,0,194,195,5,100,0,0,195,196,5,105,
-        0,0,196,197,5,102,0,0,197,198,5,121,0,0,198,44,1,0,0,0,199,200,5,
-        112,0,0,200,201,5,114,0,0,201,202,5,105,0,0,202,203,5,111,0,0,203,
-        204,5,114,0,0,204,205,5,105,0,0,205,206,5,116,0,0,206,207,5,121,
-        0,0,207,46,1,0,0,0,208,209,5,102,0,0,209,210,5,105,0,0,210,211,5,
-        108,0,0,211,212,5,101,0,0,212,48,1,0,0,0,213,214,5,116,0,0,214,215,
-        5,121,0,0,215,216,5,112,0,0,216,217,5,101,0,0,217,50,1,0,0,0,218,
-        220,5,13,0,0,219,218,1,0,0,0,219,220,1,0,0,0,220,221,1,0,0,0,221,
-        222,5,10,0,0,222,52,1,0,0,0,223,224,5,111,0,0,224,54,1,0,0,0,225,
-        226,5,120,0,0,226,56,1,0,0,0,227,228,5,50,0,0,228,229,3,129,64,0,
-        229,230,3,129,64,0,230,231,3,129,64,0,231,232,3,87,43,0,232,233,
-        3,133,66,0,233,234,3,129,64,0,234,235,3,87,43,0,235,236,3,131,65,
-        0,236,237,3,129,64,0,237,58,1,0,0,0,238,239,2,48,50,0,239,240,3,
-        129,64,0,240,241,2,48,53,0,241,242,3,129,64,0,242,60,1,0,0,0,243,
-        244,3,85,42,0,244,245,3,73,36,0,245,62,1,0,0,0,246,247,3,83,41,0,
-        247,248,3,73,36,0,248,64,1,0,0,0,249,250,3,121,60,0,250,251,3,73,
-        36,0,251,66,1,0,0,0,252,253,5,80,0,0,253,254,3,129,64,0,254,68,1,
-        0,0,0,255,260,3,137,68,0,256,259,3,137,68,0,257,259,3,93,46,0,258,
-        256,1,0,0,0,258,257,1,0,0,0,259,262,1,0,0,0,260,258,1,0,0,0,260,
-        261,1,0,0,0,261,70,1,0,0,0,262,260,1,0,0,0,263,264,3,73,36,0,264,
-        265,3,101,50,0,265,266,3,127,63,0,266,268,3,127,63,0,267,269,3,127,
-        63,0,268,267,1,0,0,0,268,269,1,0,0,0,269,72,1,0,0,0,270,271,3,129,
-        64,0,271,272,3,129,64,0,272,273,3,133,66,0,273,274,3,129,64,0,274,
-        275,3,131,65,0,275,276,3,129,64,0,276,74,1,0,0,0,277,282,3,129,64,
-        0,278,281,3,137,68,0,279,281,3,93,46,0,280,278,1,0,0,0,280,279,1,
-        0,0,0,281,284,1,0,0,0,282,280,1,0,0,0,282,283,1,0,0,0,283,76,1,0,
-        0,0,284,282,1,0,0,0,285,286,5,32,0,0,286,287,5,32,0,0,287,288,5,
-        45,0,0,288,78,1,0,0,0,289,290,5,32,0,0,290,291,5,32,0,0,291,292,
-        5,32,0,0,292,293,5,32,0,0,293,294,5,45,0,0,294,80,1,0,0,0,295,296,
-        7,0,0,0,296,82,1,0,0,0,297,298,5,36,0,0,298,84,1,0,0,0,299,300,5,
-        94,0,0,300,86,1,0,0,0,301,302,5,45,0,0,302,88,1,0,0,0,303,304,5,
-        46,0,0,304,90,1,0,0,0,305,306,5,47,0,0,306,92,1,0,0,0,307,308,5,
-        95,0,0,308,94,1,0,0,0,309,310,5,32,0,0,310,96,1,0,0,0,311,312,5,
-        40,0,0,312,98,1,0,0,0,313,314,5,41,0,0,314,100,1,0,0,0,315,316,5,
-        35,0,0,316,102,1,0,0,0,317,318,5,64,0,0,318,104,1,0,0,0,319,320,
-        5,43,0,0,320,106,1,0,0,0,321,322,5,37,0,0,322,108,1,0,0,0,323,324,
-        5,39,0,0,324,110,1,0,0,0,325,326,5,34,0,0,326,112,1,0,0,0,327,328,
-        5,126,0,0,328,114,1,0,0,0,329,330,5,42,0,0,330,116,1,0,0,0,331,332,
-        5,60,0,0,332,118,1,0,0,0,333,334,5,62,0,0,334,120,1,0,0,0,335,336,
-        5,58,0,0,336,122,1,0,0,0,337,338,2,65,90,0,338,124,1,0,0,0,339,340,
-        2,97,122,0,340,126,1,0,0,0,341,344,3,129,64,0,342,344,7,1,0,0,343,
-        341,1,0,0,0,343,342,1,0,0,0,344,128,1,0,0,0,345,346,2,48,57,0,346,
-        130,1,0,0,0,347,348,2,48,51,0,348,132,1,0,0,0,349,350,2,48,49,0,
-        350,134,1,0,0,0,351,354,3,123,61,0,352,354,3,125,62,0,353,351,1,
-        0,0,0,353,352,1,0,0,0,354,136,1,0,0,0,355,358,3,135,67,0,356,358,
-        3,129,64,0,357,355,1,0,0,0,357,356,1,0,0,0,358,138,1,0,0,0,10,0,
-        219,258,260,268,280,282,343,353,357,0
+        65,7,65,2,66,7,66,2,67,7,67,2,68,7,68,2,69,7,69,1,0,1,0,1,1,1,1,
+        1,2,1,2,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,6,1,6,1,7,1,7,
+        1,8,1,8,1,9,1,9,1,10,1,10,1,11,1,11,1,12,1,12,1,13,1,13,1,14,1,14,
+        1,15,1,15,1,16,1,16,1,17,1,17,1,17,1,18,1,18,1,18,1,19,1,19,1,20,
+        1,20,1,20,1,21,1,21,1,21,1,21,1,21,1,21,1,21,1,22,1,22,1,22,1,22,
+        1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,23,1,23,1,23,1,23,1,23,1,24,
+        1,24,1,24,1,24,1,24,1,25,1,25,1,25,1,25,1,25,1,26,3,26,225,8,26,
+        1,26,1,26,1,27,1,27,1,28,1,28,1,29,1,29,1,29,1,29,1,29,1,29,1,29,
+        1,29,1,29,1,29,1,29,1,30,1,30,1,30,1,30,1,30,1,31,1,31,1,31,1,32,
+        1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,5,35,264,
+        8,35,10,35,12,35,267,9,35,1,36,1,36,1,36,1,36,1,36,3,36,274,8,36,
+        1,37,1,37,1,37,1,37,1,37,1,37,1,37,1,38,1,38,1,38,5,38,286,8,38,
+        10,38,12,38,289,9,38,1,39,1,39,1,39,1,39,1,40,1,40,1,40,1,40,1,40,
+        1,40,1,41,1,41,1,42,1,42,1,43,1,43,1,44,1,44,1,45,1,45,1,46,1,46,
+        1,47,1,47,1,48,1,48,1,49,1,49,1,50,1,50,1,51,1,51,1,52,1,52,1,53,
+        1,53,1,54,1,54,1,55,1,55,1,56,1,56,1,57,1,57,1,58,1,58,1,59,1,59,
+        1,60,1,60,1,61,1,61,1,62,1,62,1,63,1,63,1,64,1,64,3,64,349,8,64,
+        1,65,1,65,1,66,1,66,1,67,1,67,1,68,1,68,3,68,359,8,68,1,69,1,69,
+        3,69,363,8,69,0,0,70,1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,
+        10,21,11,23,12,25,13,27,14,29,15,31,16,33,17,35,18,37,19,39,20,41,
+        21,43,22,45,23,47,24,49,25,51,26,53,27,55,28,57,29,59,30,61,31,63,
+        32,65,33,67,34,69,35,71,36,73,37,75,38,77,39,79,40,81,41,83,42,85,
+        43,87,44,89,45,91,46,93,47,95,48,97,49,99,50,101,51,103,52,105,53,
+        107,54,109,55,111,56,113,57,115,58,117,59,119,60,121,61,123,62,125,
+        0,127,0,129,0,131,0,133,0,135,0,137,0,139,0,1,0,2,9,0,33,33,38,38,
+        44,44,59,59,61,61,63,63,91,93,96,96,123,125,6,0,65,72,74,78,80,90,
+        97,105,107,107,109,122,364,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,
+        7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,
+        1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,
+        1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,
+        1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,
+        1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,
+        1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,
+        1,0,0,0,0,69,1,0,0,0,0,71,1,0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,
+        1,0,0,0,0,79,1,0,0,0,0,81,1,0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,
+        1,0,0,0,0,89,1,0,0,0,0,91,1,0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,
+        1,0,0,0,0,99,1,0,0,0,0,101,1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,
+        107,1,0,0,0,0,109,1,0,0,0,0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,
+        0,0,0,117,1,0,0,0,0,119,1,0,0,0,0,121,1,0,0,0,0,123,1,0,0,0,1,141,
+        1,0,0,0,3,143,1,0,0,0,5,145,1,0,0,0,7,147,1,0,0,0,9,149,1,0,0,0,
+        11,154,1,0,0,0,13,157,1,0,0,0,15,159,1,0,0,0,17,161,1,0,0,0,19,163,
+        1,0,0,0,21,165,1,0,0,0,23,167,1,0,0,0,25,169,1,0,0,0,27,171,1,0,
+        0,0,29,173,1,0,0,0,31,175,1,0,0,0,33,177,1,0,0,0,35,179,1,0,0,0,
+        37,182,1,0,0,0,39,185,1,0,0,0,41,187,1,0,0,0,43,190,1,0,0,0,45,197,
+        1,0,0,0,47,204,1,0,0,0,49,213,1,0,0,0,51,218,1,0,0,0,53,224,1,0,
+        0,0,55,228,1,0,0,0,57,230,1,0,0,0,59,232,1,0,0,0,61,243,1,0,0,0,
+        63,248,1,0,0,0,65,251,1,0,0,0,67,254,1,0,0,0,69,257,1,0,0,0,71,260,
+        1,0,0,0,73,268,1,0,0,0,75,275,1,0,0,0,77,282,1,0,0,0,79,290,1,0,
+        0,0,81,294,1,0,0,0,83,300,1,0,0,0,85,302,1,0,0,0,87,304,1,0,0,0,
+        89,306,1,0,0,0,91,308,1,0,0,0,93,310,1,0,0,0,95,312,1,0,0,0,97,314,
+        1,0,0,0,99,316,1,0,0,0,101,318,1,0,0,0,103,320,1,0,0,0,105,322,1,
+        0,0,0,107,324,1,0,0,0,109,326,1,0,0,0,111,328,1,0,0,0,113,330,1,
+        0,0,0,115,332,1,0,0,0,117,334,1,0,0,0,119,336,1,0,0,0,121,338,1,
+        0,0,0,123,340,1,0,0,0,125,342,1,0,0,0,127,344,1,0,0,0,129,348,1,
+        0,0,0,131,350,1,0,0,0,133,352,1,0,0,0,135,354,1,0,0,0,137,358,1,
+        0,0,0,139,362,1,0,0,0,141,142,5,83,0,0,142,2,1,0,0,0,143,144,5,87,
+        0,0,144,4,1,0,0,0,145,146,5,79,0,0,146,6,1,0,0,0,147,148,5,71,0,
+        0,148,8,1,0,0,0,149,150,5,110,0,0,150,151,5,111,0,0,151,152,5,116,
+        0,0,152,153,5,101,0,0,153,10,1,0,0,0,154,155,5,111,0,0,155,156,5,
+        114,0,0,156,12,1,0,0,0,157,158,5,49,0,0,158,14,1,0,0,0,159,160,5,
+        50,0,0,160,16,1,0,0,0,161,162,5,51,0,0,162,18,1,0,0,0,163,164,5,
+        52,0,0,164,20,1,0,0,0,165,166,5,53,0,0,166,22,1,0,0,0,167,168,5,
+        54,0,0,168,24,1,0,0,0,169,170,5,55,0,0,170,26,1,0,0,0,171,172,5,
+        56,0,0,172,28,1,0,0,0,173,174,5,57,0,0,174,30,1,0,0,0,175,176,5,
+        33,0,0,176,32,1,0,0,0,177,178,5,48,0,0,178,34,1,0,0,0,179,180,5,
+        60,0,0,180,181,5,61,0,0,181,36,1,0,0,0,182,183,5,62,0,0,183,184,
+        5,61,0,0,184,38,1,0,0,0,185,186,5,99,0,0,186,40,1,0,0,0,187,188,
+        5,102,0,0,188,189,5,61,0,0,189,42,1,0,0,0,190,191,5,99,0,0,191,192,
+        5,114,0,0,192,193,5,101,0,0,193,194,5,97,0,0,194,195,5,116,0,0,195,
+        196,5,101,0,0,196,44,1,0,0,0,197,198,5,109,0,0,198,199,5,111,0,0,
+        199,200,5,100,0,0,200,201,5,105,0,0,201,202,5,102,0,0,202,203,5,
+        121,0,0,203,46,1,0,0,0,204,205,5,112,0,0,205,206,5,114,0,0,206,207,
+        5,105,0,0,207,208,5,111,0,0,208,209,5,114,0,0,209,210,5,105,0,0,
+        210,211,5,116,0,0,211,212,5,121,0,0,212,48,1,0,0,0,213,214,5,102,
+        0,0,214,215,5,105,0,0,215,216,5,108,0,0,216,217,5,101,0,0,217,50,
+        1,0,0,0,218,219,5,116,0,0,219,220,5,121,0,0,220,221,5,112,0,0,221,
+        222,5,101,0,0,222,52,1,0,0,0,223,225,5,13,0,0,224,223,1,0,0,0,224,
+        225,1,0,0,0,225,226,1,0,0,0,226,227,5,10,0,0,227,54,1,0,0,0,228,
+        229,5,111,0,0,229,56,1,0,0,0,230,231,5,120,0,0,231,58,1,0,0,0,232,
+        233,5,50,0,0,233,234,3,131,65,0,234,235,3,131,65,0,235,236,3,131,
+        65,0,236,237,3,89,44,0,237,238,3,135,67,0,238,239,3,131,65,0,239,
+        240,3,89,44,0,240,241,3,133,66,0,241,242,3,131,65,0,242,60,1,0,0,
+        0,243,244,2,48,50,0,244,245,3,131,65,0,245,246,2,48,53,0,246,247,
+        3,131,65,0,247,62,1,0,0,0,248,249,3,87,43,0,249,250,3,75,37,0,250,
+        64,1,0,0,0,251,252,3,85,42,0,252,253,3,75,37,0,253,66,1,0,0,0,254,
+        255,3,123,61,0,255,256,3,75,37,0,256,68,1,0,0,0,257,258,5,80,0,0,
+        258,259,3,131,65,0,259,70,1,0,0,0,260,265,3,139,69,0,261,264,3,139,
+        69,0,262,264,3,95,47,0,263,261,1,0,0,0,263,262,1,0,0,0,264,267,1,
+        0,0,0,265,263,1,0,0,0,265,266,1,0,0,0,266,72,1,0,0,0,267,265,1,0,
+        0,0,268,269,3,75,37,0,269,270,3,103,51,0,270,271,3,129,64,0,271,
+        273,3,129,64,0,272,274,3,129,64,0,273,272,1,0,0,0,273,274,1,0,0,
+        0,274,74,1,0,0,0,275,276,3,131,65,0,276,277,3,131,65,0,277,278,3,
+        135,67,0,278,279,3,131,65,0,279,280,3,133,66,0,280,281,3,131,65,
+        0,281,76,1,0,0,0,282,287,3,131,65,0,283,286,3,139,69,0,284,286,3,
+        95,47,0,285,283,1,0,0,0,285,284,1,0,0,0,286,289,1,0,0,0,287,285,
+        1,0,0,0,287,288,1,0,0,0,288,78,1,0,0,0,289,287,1,0,0,0,290,291,5,
+        32,0,0,291,292,5,32,0,0,292,293,5,45,0,0,293,80,1,0,0,0,294,295,
+        5,32,0,0,295,296,5,32,0,0,296,297,5,32,0,0,297,298,5,32,0,0,298,
+        299,5,45,0,0,299,82,1,0,0,0,300,301,7,0,0,0,301,84,1,0,0,0,302,303,
+        5,36,0,0,303,86,1,0,0,0,304,305,5,94,0,0,305,88,1,0,0,0,306,307,
+        5,45,0,0,307,90,1,0,0,0,308,309,5,46,0,0,309,92,1,0,0,0,310,311,
+        5,47,0,0,311,94,1,0,0,0,312,313,5,95,0,0,313,96,1,0,0,0,314,315,
+        5,32,0,0,315,98,1,0,0,0,316,317,5,40,0,0,317,100,1,0,0,0,318,319,
+        5,41,0,0,319,102,1,0,0,0,320,321,5,35,0,0,321,104,1,0,0,0,322,323,
+        5,64,0,0,323,106,1,0,0,0,324,325,5,43,0,0,325,108,1,0,0,0,326,327,
+        5,37,0,0,327,110,1,0,0,0,328,329,5,39,0,0,329,112,1,0,0,0,330,331,
+        5,34,0,0,331,114,1,0,0,0,332,333,5,126,0,0,333,116,1,0,0,0,334,335,
+        5,42,0,0,335,118,1,0,0,0,336,337,5,60,0,0,337,120,1,0,0,0,338,339,
+        5,62,0,0,339,122,1,0,0,0,340,341,5,58,0,0,341,124,1,0,0,0,342,343,
+        2,65,90,0,343,126,1,0,0,0,344,345,2,97,122,0,345,128,1,0,0,0,346,
+        349,3,131,65,0,347,349,7,1,0,0,348,346,1,0,0,0,348,347,1,0,0,0,349,
+        130,1,0,0,0,350,351,2,48,57,0,351,132,1,0,0,0,352,353,2,48,51,0,
+        353,134,1,0,0,0,354,355,2,48,49,0,355,136,1,0,0,0,356,359,3,125,
+        62,0,357,359,3,127,63,0,358,356,1,0,0,0,358,357,1,0,0,0,359,138,
+        1,0,0,0,360,363,3,137,68,0,361,363,3,131,65,0,362,360,1,0,0,0,362,
+        361,1,0,0,0,363,140,1,0,0,0,10,0,224,263,265,273,285,287,348,358,
+        362,0
     ]
 
 class ZorgQueryLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
@@ -164,59 +166,60 @@
     T__18 = 19
     T__19 = 20
     T__20 = 21
     T__21 = 22
     T__22 = 23
     T__23 = 24
     T__24 = 25
-    NL = 26
-    LOWER_O = 27
-    LOWER_X = 28
-    DATE = 29
-    TIME = 30
-    CREATE_RANGE_HEAD = 31
-    MODIFY_RANGE_HEAD = 32
-    DATE_RANGE_TAIL = 33
-    PRIORITY = 34
-    ID = 35
-    ZID = 36
-    SHORT_DATE = 37
-    NUM_ID = 38
-    TWO_SPACE_DASH = 39
-    FOUR_SPACE_DASH = 40
-    SYMBOL = 41
-    DOLLAR = 42
-    HAT = 43
-    DASH = 44
-    DOT = 45
-    FSLASH = 46
-    UNDERSCORE = 47
-    SPACE = 48
-    LPAREN = 49
-    RPAREN = 50
-    HASH = 51
-    AT_SIGN = 52
-    PLUS = 53
-    PERCENT = 54
-    SQUOTE = 55
-    DQUOTE = 56
-    TILDE = 57
-    STAR = 58
-    LANGLE = 59
-    RANGLE = 60
-    COLON = 61
+    T__25 = 26
+    NL = 27
+    LOWER_O = 28
+    LOWER_X = 29
+    DATE = 30
+    TIME = 31
+    CREATE_RANGE_HEAD = 32
+    MODIFY_RANGE_HEAD = 33
+    DATE_RANGE_TAIL = 34
+    PRIORITY = 35
+    ID = 36
+    ZID = 37
+    SHORT_DATE = 38
+    NUM_ID = 39
+    TWO_SPACE_DASH = 40
+    FOUR_SPACE_DASH = 41
+    SYMBOL = 42
+    DOLLAR = 43
+    HAT = 44
+    DASH = 45
+    DOT = 46
+    FSLASH = 47
+    UNDERSCORE = 48
+    SPACE = 49
+    LPAREN = 50
+    RPAREN = 51
+    HASH = 52
+    AT_SIGN = 53
+    PLUS = 54
+    PERCENT = 55
+    SQUOTE = 56
+    DQUOTE = 57
+    TILDE = 58
+    STAR = 59
+    LANGLE = 60
+    RANGLE = 61
+    COLON = 62
 
     channelNames = [ u"DEFAULT_TOKEN_CHANNEL", u"HIDDEN" ]
 
     modeNames = [ "DEFAULT_MODE" ]
 
     literalNames = [ "<INVALID>",
             "'S'", "'W'", "'O'", "'G'", "'note'", "'or'", "'1'", "'2'", 
             "'3'", "'4'", "'5'", "'6'", "'7'", "'8'", "'9'", "'!'", "'0'", 
-            "'<='", "'>='", "'c'", "'create'", "'modify'", "'priority'", 
+            "'<='", "'>='", "'c'", "'f='", "'create'", "'modify'", "'priority'", 
             "'file'", "'type'", "'o'", "'x'", "'  -'", "'    -'", "'$'", 
             "'^'", "'-'", "'.'", "'/'", "'_'", "' '", "'('", "')'", "'#'", 
             "'@'", "'+'", "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'", 
             "':'" ]
 
     symbolicNames = [ "<INVALID>",
             "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", 
@@ -225,19 +228,19 @@
             "SYMBOL", "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
             "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", 
             "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "COLON" ]
 
     ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "T__6", 
                   "T__7", "T__8", "T__9", "T__10", "T__11", "T__12", "T__13", 
                   "T__14", "T__15", "T__16", "T__17", "T__18", "T__19", 
-                  "T__20", "T__21", "T__22", "T__23", "T__24", "NL", "LOWER_O", 
-                  "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", "MODIFY_RANGE_HEAD", 
-                  "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", "SHORT_DATE", 
-                  "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", 
-                  "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+                  "T__20", "T__21", "T__22", "T__23", "T__24", "T__25", 
+                  "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", 
+                  "MODIFY_RANGE_HEAD", "DATE_RANGE_TAIL", "PRIORITY", "ID", 
+                  "ZID", "SHORT_DATE", "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", 
+                  "SYMBOL", "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
                   "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
                   "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", 
                   "RANGLE", "COLON", "UPPER_LETTER", "LOWER_LETTER", "ZID_CHAR", 
                   "NUM", "FIRST_D_NUM", "FIRST_M_NUM", "ALPHA", "ALPHANUM" ]
 
     grammarFileName = "ZorgQuery.g4"
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryListener.py` & `zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryListener.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,23 @@
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#desc_filter.
     def exitDesc_filter(self, ctx:ZorgQueryParser.Desc_filterContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgQueryParser#file_filter.
+    def enterFile_filter(self, ctx:ZorgQueryParser.File_filterContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#file_filter.
+    def exitFile_filter(self, ctx:ZorgQueryParser.File_filterContext):
+        pass
+
+
     # Enter a parse tree produced by ZorgQueryParser#zid.
     def enterZid(self, ctx:ZorgQueryParser.ZidContext):
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#zid.
     def exitZid(self, ctx:ZorgQueryParser.ZidContext):
         pass
@@ -301,14 +310,50 @@
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#time.
     def exitTime(self, ctx:ZorgQueryParser.TimeContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgQueryParser#any_non_squote.
+    def enterAny_non_squote(self, ctx:ZorgQueryParser.Any_non_squoteContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#any_non_squote.
+    def exitAny_non_squote(self, ctx:ZorgQueryParser.Any_non_squoteContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#non_tag_symbol.
+    def enterNon_tag_symbol(self, ctx:ZorgQueryParser.Non_tag_symbolContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#non_tag_symbol.
+    def exitNon_tag_symbol(self, ctx:ZorgQueryParser.Non_tag_symbolContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#id_symbol.
+    def enterId_symbol(self, ctx:ZorgQueryParser.Id_symbolContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#id_symbol.
+    def exitId_symbol(self, ctx:ZorgQueryParser.Id_symbolContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#tag_symbol.
+    def enterTag_symbol(self, ctx:ZorgQueryParser.Tag_symbolContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#tag_symbol.
+    def exitTag_symbol(self, ctx:ZorgQueryParser.Tag_symbolContext):
+        pass
+
+
     # Enter a parse tree produced by ZorgQueryParser#group_by_body.
     def enterGroup_by_body(self, ctx:ZorgQueryParser.Group_by_bodyContext):
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#group_by_body.
     def exitGroup_by_body(self, ctx:ZorgQueryParser.Group_by_bodyContext):
         pass
```

### Comparing `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryParser.py` & `zettel_org-0.7.4/src/zorg/grammar/zorg_query/ZorgQueryParser.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,127 +6,143 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,61,316,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,62,356,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
         2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
         7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
-        2,40,7,40,2,41,7,41,1,0,1,0,3,0,87,8,0,1,1,1,1,3,1,91,8,1,1,2,1,
-        2,1,2,3,2,96,8,2,1,2,1,2,1,2,3,2,101,8,2,1,2,1,2,3,2,105,8,2,1,3,
-        1,3,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,6,1,6,1,6,1,6,1,7,1,7,1,7,
-        1,7,1,8,1,8,1,8,1,8,1,8,1,8,3,8,131,8,8,1,9,1,9,1,10,1,10,1,11,1,
-        11,1,11,1,11,1,11,5,11,142,8,11,10,11,12,11,145,9,11,1,12,1,12,1,
-        12,5,12,150,8,12,10,12,12,12,153,9,12,1,13,1,13,1,13,1,13,1,13,1,
-        13,1,13,1,13,3,13,163,8,13,1,14,4,14,166,8,14,11,14,12,14,167,1,
-        15,1,15,1,16,1,16,1,16,3,16,175,8,16,1,17,3,17,178,8,17,1,17,1,17,
-        1,17,1,17,3,17,184,8,17,1,18,1,18,1,19,1,19,1,19,1,20,1,20,1,20,
-        1,21,1,21,1,21,1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,24,1,24,3,24,
-        206,8,24,1,25,1,25,3,25,210,8,25,1,26,3,26,213,8,26,1,26,1,26,1,
-        26,3,26,218,8,26,1,26,1,26,4,26,222,8,26,11,26,12,26,223,3,26,226,
-        8,26,1,26,3,26,229,8,26,1,26,3,26,232,8,26,1,27,1,27,1,28,3,28,237,
-        8,28,1,28,3,28,240,8,28,1,28,1,28,1,28,1,28,5,28,246,8,28,10,28,
-        12,28,249,9,28,1,28,1,28,1,29,1,29,1,30,1,30,1,30,1,30,1,30,1,30,
-        1,30,1,30,1,30,3,30,264,8,30,1,31,1,31,1,32,1,32,1,33,1,33,1,33,
-        3,33,273,8,33,1,33,1,33,3,33,277,8,33,1,33,1,33,3,33,281,8,33,1,
-        34,1,34,1,34,1,34,1,34,1,34,1,34,3,34,290,8,34,1,35,1,35,1,35,5,
-        35,295,8,35,10,35,12,35,298,9,35,1,36,1,36,1,36,1,36,3,36,304,8,
-        36,1,37,1,37,1,38,1,38,1,39,1,39,1,40,1,40,1,41,1,41,1,41,0,0,42,
-        0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,
-        46,48,50,52,54,56,58,60,62,64,66,68,70,72,74,76,78,80,82,0,4,4,0,
-        27,28,44,44,57,57,59,60,1,0,7,15,2,0,7,15,17,17,2,0,18,19,59,60,
-        330,0,84,1,0,0,0,2,90,1,0,0,0,4,95,1,0,0,0,6,106,1,0,0,0,8,108,1,
-        0,0,0,10,112,1,0,0,0,12,116,1,0,0,0,14,120,1,0,0,0,16,130,1,0,0,
-        0,18,132,1,0,0,0,20,134,1,0,0,0,22,136,1,0,0,0,24,146,1,0,0,0,26,
-        162,1,0,0,0,28,165,1,0,0,0,30,169,1,0,0,0,32,171,1,0,0,0,34,177,
-        1,0,0,0,36,185,1,0,0,0,38,187,1,0,0,0,40,190,1,0,0,0,42,193,1,0,
-        0,0,44,196,1,0,0,0,46,199,1,0,0,0,48,203,1,0,0,0,50,207,1,0,0,0,
-        52,212,1,0,0,0,54,233,1,0,0,0,56,236,1,0,0,0,58,252,1,0,0,0,60,263,
-        1,0,0,0,62,265,1,0,0,0,64,267,1,0,0,0,66,269,1,0,0,0,68,289,1,0,
-        0,0,70,291,1,0,0,0,72,303,1,0,0,0,74,305,1,0,0,0,76,307,1,0,0,0,
-        78,309,1,0,0,0,80,311,1,0,0,0,82,313,1,0,0,0,84,86,3,2,1,0,85,87,
-        5,26,0,0,86,85,1,0,0,0,86,87,1,0,0,0,87,1,1,0,0,0,88,91,3,4,2,0,
-        89,91,3,6,3,0,90,88,1,0,0,0,90,89,1,0,0,0,91,3,1,0,0,0,92,93,3,8,
-        4,0,93,94,5,48,0,0,94,96,1,0,0,0,95,92,1,0,0,0,95,96,1,0,0,0,96,
-        97,1,0,0,0,97,100,3,10,5,0,98,99,5,48,0,0,99,101,3,12,6,0,100,98,
-        1,0,0,0,100,101,1,0,0,0,101,104,1,0,0,0,102,103,5,48,0,0,103,105,
-        3,14,7,0,104,102,1,0,0,0,104,105,1,0,0,0,105,5,1,0,0,0,106,107,3,
-        8,4,0,107,7,1,0,0,0,108,109,5,1,0,0,109,110,5,48,0,0,110,111,3,16,
-        8,0,111,9,1,0,0,0,112,113,5,2,0,0,113,114,5,48,0,0,114,115,3,20,
-        10,0,115,11,1,0,0,0,116,117,5,3,0,0,117,118,5,48,0,0,118,119,3,70,
-        35,0,119,13,1,0,0,0,120,121,5,4,0,0,121,122,5,48,0,0,122,123,3,66,
-        33,0,123,15,1,0,0,0,124,131,3,80,40,0,125,131,3,18,9,0,126,131,5,
-        52,0,0,127,131,5,51,0,0,128,131,5,53,0,0,129,131,5,54,0,0,130,124,
-        1,0,0,0,130,125,1,0,0,0,130,126,1,0,0,0,130,127,1,0,0,0,130,128,
-        1,0,0,0,130,129,1,0,0,0,131,17,1,0,0,0,132,133,5,5,0,0,133,19,1,
-        0,0,0,134,135,3,22,11,0,135,21,1,0,0,0,136,143,3,24,12,0,137,138,
-        5,48,0,0,138,139,5,6,0,0,139,140,5,48,0,0,140,142,3,24,12,0,141,
-        137,1,0,0,0,142,145,1,0,0,0,143,141,1,0,0,0,143,144,1,0,0,0,144,
-        23,1,0,0,0,145,143,1,0,0,0,146,151,3,26,13,0,147,148,5,48,0,0,148,
-        150,3,26,13,0,149,147,1,0,0,0,150,153,1,0,0,0,151,149,1,0,0,0,151,
-        152,1,0,0,0,152,25,1,0,0,0,153,151,1,0,0,0,154,163,3,28,14,0,155,
-        163,3,32,16,0,156,163,3,34,17,0,157,163,3,46,23,0,158,163,3,48,24,
-        0,159,163,3,50,25,0,160,163,3,52,26,0,161,163,3,56,28,0,162,154,
-        1,0,0,0,162,155,1,0,0,0,162,156,1,0,0,0,162,157,1,0,0,0,162,158,
-        1,0,0,0,162,159,1,0,0,0,162,160,1,0,0,0,162,161,1,0,0,0,163,27,1,
-        0,0,0,164,166,3,30,15,0,165,164,1,0,0,0,166,167,1,0,0,0,167,165,
-        1,0,0,0,167,168,1,0,0,0,168,29,1,0,0,0,169,170,7,0,0,0,170,31,1,
-        0,0,0,171,174,5,34,0,0,172,173,5,44,0,0,173,175,7,1,0,0,174,172,
-        1,0,0,0,174,175,1,0,0,0,175,33,1,0,0,0,176,178,3,36,18,0,177,176,
-        1,0,0,0,177,178,1,0,0,0,178,183,1,0,0,0,179,184,3,38,19,0,180,184,
-        3,40,20,0,181,184,3,42,21,0,182,184,3,44,22,0,183,179,1,0,0,0,183,
-        180,1,0,0,0,183,181,1,0,0,0,183,182,1,0,0,0,184,35,1,0,0,0,185,186,
-        5,16,0,0,186,37,1,0,0,0,187,188,5,51,0,0,188,189,5,35,0,0,189,39,
-        1,0,0,0,190,191,5,52,0,0,191,192,5,35,0,0,192,41,1,0,0,0,193,194,
-        5,54,0,0,194,195,5,35,0,0,195,43,1,0,0,0,196,197,5,53,0,0,197,198,
-        5,35,0,0,198,45,1,0,0,0,199,200,5,49,0,0,200,201,3,22,11,0,201,202,
-        5,50,0,0,202,47,1,0,0,0,203,205,5,31,0,0,204,206,5,33,0,0,205,204,
-        1,0,0,0,205,206,1,0,0,0,206,49,1,0,0,0,207,209,5,32,0,0,208,210,
-        5,33,0,0,209,208,1,0,0,0,209,210,1,0,0,0,210,51,1,0,0,0,211,213,
-        3,36,18,0,212,211,1,0,0,0,212,213,1,0,0,0,213,214,1,0,0,0,214,215,
-        5,35,0,0,215,217,5,61,0,0,216,218,3,54,27,0,217,216,1,0,0,0,217,
-        218,1,0,0,0,218,231,1,0,0,0,219,226,5,35,0,0,220,222,7,2,0,0,221,
-        220,1,0,0,0,222,223,1,0,0,0,223,221,1,0,0,0,223,224,1,0,0,0,224,
-        226,1,0,0,0,225,219,1,0,0,0,225,221,1,0,0,0,226,228,1,0,0,0,227,
-        229,5,58,0,0,228,227,1,0,0,0,228,229,1,0,0,0,229,232,1,0,0,0,230,
-        232,5,58,0,0,231,225,1,0,0,0,231,230,1,0,0,0,232,53,1,0,0,0,233,
-        234,7,3,0,0,234,55,1,0,0,0,235,237,3,36,18,0,236,235,1,0,0,0,236,
-        237,1,0,0,0,237,239,1,0,0,0,238,240,5,20,0,0,239,238,1,0,0,0,239,
-        240,1,0,0,0,240,241,1,0,0,0,241,242,5,55,0,0,242,247,3,60,30,0,243,
-        244,5,48,0,0,244,246,3,60,30,0,245,243,1,0,0,0,246,249,1,0,0,0,247,
-        245,1,0,0,0,247,248,1,0,0,0,248,250,1,0,0,0,249,247,1,0,0,0,250,
-        251,5,55,0,0,251,57,1,0,0,0,252,253,5,36,0,0,253,59,1,0,0,0,254,
-        264,5,35,0,0,255,264,5,38,0,0,256,264,5,33,0,0,257,264,5,34,0,0,
-        258,264,3,62,31,0,259,264,3,64,32,0,260,264,3,58,29,0,261,264,5,
-        27,0,0,262,264,5,28,0,0,263,254,1,0,0,0,263,255,1,0,0,0,263,256,
-        1,0,0,0,263,257,1,0,0,0,263,258,1,0,0,0,263,259,1,0,0,0,263,260,
-        1,0,0,0,263,261,1,0,0,0,263,262,1,0,0,0,264,61,1,0,0,0,265,266,5,
-        29,0,0,266,63,1,0,0,0,267,268,5,30,0,0,268,65,1,0,0,0,269,272,3,
-        68,34,0,270,271,5,48,0,0,271,273,3,68,34,0,272,270,1,0,0,0,272,273,
-        1,0,0,0,273,276,1,0,0,0,274,275,5,48,0,0,275,277,3,68,34,0,276,274,
-        1,0,0,0,276,277,1,0,0,0,277,280,1,0,0,0,278,279,5,48,0,0,279,281,
-        3,68,34,0,280,278,1,0,0,0,280,281,1,0,0,0,281,67,1,0,0,0,282,290,
-        3,80,40,0,283,290,3,82,41,0,284,290,3,78,39,0,285,290,5,52,0,0,286,
-        290,5,51,0,0,287,290,5,54,0,0,288,290,5,53,0,0,289,282,1,0,0,0,289,
-        283,1,0,0,0,289,284,1,0,0,0,289,285,1,0,0,0,289,286,1,0,0,0,289,
-        287,1,0,0,0,289,288,1,0,0,0,290,69,1,0,0,0,291,296,3,72,36,0,292,
-        293,5,48,0,0,293,295,3,72,36,0,294,292,1,0,0,0,295,298,1,0,0,0,296,
-        294,1,0,0,0,296,297,1,0,0,0,297,71,1,0,0,0,298,296,1,0,0,0,299,304,
-        3,74,37,0,300,304,3,76,38,0,301,304,3,78,39,0,302,304,3,82,41,0,
-        303,299,1,0,0,0,303,300,1,0,0,0,303,301,1,0,0,0,303,302,1,0,0,0,
-        304,73,1,0,0,0,305,306,5,21,0,0,306,75,1,0,0,0,307,308,5,22,0,0,
-        308,77,1,0,0,0,309,310,5,23,0,0,310,79,1,0,0,0,311,312,5,24,0,0,
-        312,81,1,0,0,0,313,314,5,25,0,0,314,83,1,0,0,0,31,86,90,95,100,104,
-        130,143,151,162,167,174,177,183,205,209,212,217,223,225,228,231,
-        236,239,247,263,272,276,280,289,296,303
+        2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,45,2,46,
+        7,46,1,0,1,0,3,0,97,8,0,1,1,1,1,3,1,101,8,1,1,2,1,2,1,2,3,2,106,
+        8,2,1,2,1,2,1,2,3,2,111,8,2,1,2,1,2,3,2,115,8,2,1,3,1,3,1,4,1,4,
+        1,4,1,4,1,5,1,5,1,5,1,5,1,6,1,6,1,6,1,6,1,7,1,7,1,7,1,7,1,8,1,8,
+        1,8,1,8,1,8,1,8,3,8,141,8,8,1,9,1,9,1,10,1,10,1,11,1,11,1,11,1,11,
+        1,11,5,11,152,8,11,10,11,12,11,155,9,11,1,12,1,12,1,12,5,12,160,
+        8,12,10,12,12,12,163,9,12,1,13,1,13,1,13,1,13,1,13,1,13,1,13,1,13,
+        1,13,3,13,174,8,13,1,14,4,14,177,8,14,11,14,12,14,178,1,15,1,15,
+        1,16,1,16,1,16,3,16,186,8,16,1,17,3,17,189,8,17,1,17,1,17,1,17,1,
+        17,3,17,195,8,17,1,18,1,18,1,19,1,19,1,19,1,20,1,20,1,20,1,21,1,
+        21,1,21,1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,24,1,24,3,24,217,8,
+        24,1,25,1,25,3,25,221,8,25,1,26,3,26,224,8,26,1,26,1,26,1,26,3,26,
+        229,8,26,1,26,1,26,4,26,233,8,26,11,26,12,26,234,1,26,3,26,238,8,
+        26,1,27,1,27,1,28,3,28,243,8,28,1,28,3,28,246,8,28,1,28,1,28,5,28,
+        250,8,28,10,28,12,28,253,9,28,1,28,1,28,1,28,5,28,258,8,28,10,28,
+        12,28,261,9,28,1,28,1,28,1,29,3,29,266,8,29,1,29,1,29,1,29,3,29,
+        271,8,29,3,29,273,8,29,1,29,1,29,3,29,277,8,29,1,30,1,30,1,31,1,
+        31,1,31,1,31,1,31,1,31,1,31,1,31,1,31,3,31,290,8,31,1,32,1,32,1,
+        33,1,33,1,34,1,34,1,34,1,34,1,34,1,34,3,34,302,8,34,1,35,1,35,1,
+        36,1,36,1,37,1,37,1,38,1,38,1,38,3,38,313,8,38,1,38,1,38,3,38,317,
+        8,38,1,38,1,38,3,38,321,8,38,1,39,1,39,1,39,1,39,1,39,1,39,1,39,
+        3,39,330,8,39,1,40,1,40,1,40,5,40,335,8,40,10,40,12,40,338,9,40,
+        1,41,1,41,1,41,1,41,3,41,344,8,41,1,42,1,42,1,43,1,43,1,44,1,44,
+        1,45,1,45,1,46,1,46,1,46,0,0,47,0,2,4,6,8,10,12,14,16,18,20,22,24,
+        26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,
+        70,72,74,76,78,80,82,84,86,88,90,92,0,7,4,0,28,29,45,45,58,58,60,
+        61,1,0,7,15,2,0,7,15,17,17,2,0,18,19,60,61,4,0,42,42,48,48,50,51,
+        58,61,2,0,45,47,62,62,1,0,52,55,375,0,94,1,0,0,0,2,100,1,0,0,0,4,
+        105,1,0,0,0,6,116,1,0,0,0,8,118,1,0,0,0,10,122,1,0,0,0,12,126,1,
+        0,0,0,14,130,1,0,0,0,16,140,1,0,0,0,18,142,1,0,0,0,20,144,1,0,0,
+        0,22,146,1,0,0,0,24,156,1,0,0,0,26,173,1,0,0,0,28,176,1,0,0,0,30,
+        180,1,0,0,0,32,182,1,0,0,0,34,188,1,0,0,0,36,196,1,0,0,0,38,198,
+        1,0,0,0,40,201,1,0,0,0,42,204,1,0,0,0,44,207,1,0,0,0,46,210,1,0,
+        0,0,48,214,1,0,0,0,50,218,1,0,0,0,52,223,1,0,0,0,54,239,1,0,0,0,
+        56,242,1,0,0,0,58,265,1,0,0,0,60,278,1,0,0,0,62,289,1,0,0,0,64,291,
+        1,0,0,0,66,293,1,0,0,0,68,301,1,0,0,0,70,303,1,0,0,0,72,305,1,0,
+        0,0,74,307,1,0,0,0,76,309,1,0,0,0,78,329,1,0,0,0,80,331,1,0,0,0,
+        82,343,1,0,0,0,84,345,1,0,0,0,86,347,1,0,0,0,88,349,1,0,0,0,90,351,
+        1,0,0,0,92,353,1,0,0,0,94,96,3,2,1,0,95,97,5,27,0,0,96,95,1,0,0,
+        0,96,97,1,0,0,0,97,1,1,0,0,0,98,101,3,4,2,0,99,101,3,6,3,0,100,98,
+        1,0,0,0,100,99,1,0,0,0,101,3,1,0,0,0,102,103,3,8,4,0,103,104,5,49,
+        0,0,104,106,1,0,0,0,105,102,1,0,0,0,105,106,1,0,0,0,106,107,1,0,
+        0,0,107,110,3,10,5,0,108,109,5,49,0,0,109,111,3,12,6,0,110,108,1,
+        0,0,0,110,111,1,0,0,0,111,114,1,0,0,0,112,113,5,49,0,0,113,115,3,
+        14,7,0,114,112,1,0,0,0,114,115,1,0,0,0,115,5,1,0,0,0,116,117,3,8,
+        4,0,117,7,1,0,0,0,118,119,5,1,0,0,119,120,5,49,0,0,120,121,3,16,
+        8,0,121,9,1,0,0,0,122,123,5,2,0,0,123,124,5,49,0,0,124,125,3,20,
+        10,0,125,11,1,0,0,0,126,127,5,3,0,0,127,128,5,49,0,0,128,129,3,80,
+        40,0,129,13,1,0,0,0,130,131,5,4,0,0,131,132,5,49,0,0,132,133,3,76,
+        38,0,133,15,1,0,0,0,134,141,3,90,45,0,135,141,3,18,9,0,136,141,5,
+        53,0,0,137,141,5,52,0,0,138,141,5,54,0,0,139,141,5,55,0,0,140,134,
+        1,0,0,0,140,135,1,0,0,0,140,136,1,0,0,0,140,137,1,0,0,0,140,138,
+        1,0,0,0,140,139,1,0,0,0,141,17,1,0,0,0,142,143,5,5,0,0,143,19,1,
+        0,0,0,144,145,3,22,11,0,145,21,1,0,0,0,146,153,3,24,12,0,147,148,
+        5,49,0,0,148,149,5,6,0,0,149,150,5,49,0,0,150,152,3,24,12,0,151,
+        147,1,0,0,0,152,155,1,0,0,0,153,151,1,0,0,0,153,154,1,0,0,0,154,
+        23,1,0,0,0,155,153,1,0,0,0,156,161,3,26,13,0,157,158,5,49,0,0,158,
+        160,3,26,13,0,159,157,1,0,0,0,160,163,1,0,0,0,161,159,1,0,0,0,161,
+        162,1,0,0,0,162,25,1,0,0,0,163,161,1,0,0,0,164,174,3,28,14,0,165,
+        174,3,32,16,0,166,174,3,34,17,0,167,174,3,46,23,0,168,174,3,48,24,
+        0,169,174,3,50,25,0,170,174,3,52,26,0,171,174,3,56,28,0,172,174,
+        3,58,29,0,173,164,1,0,0,0,173,165,1,0,0,0,173,166,1,0,0,0,173,167,
+        1,0,0,0,173,168,1,0,0,0,173,169,1,0,0,0,173,170,1,0,0,0,173,171,
+        1,0,0,0,173,172,1,0,0,0,174,27,1,0,0,0,175,177,3,30,15,0,176,175,
+        1,0,0,0,177,178,1,0,0,0,178,176,1,0,0,0,178,179,1,0,0,0,179,29,1,
+        0,0,0,180,181,7,0,0,0,181,31,1,0,0,0,182,185,5,35,0,0,183,184,5,
+        45,0,0,184,186,7,1,0,0,185,183,1,0,0,0,185,186,1,0,0,0,186,33,1,
+        0,0,0,187,189,3,36,18,0,188,187,1,0,0,0,188,189,1,0,0,0,189,194,
+        1,0,0,0,190,195,3,38,19,0,191,195,3,40,20,0,192,195,3,42,21,0,193,
+        195,3,44,22,0,194,190,1,0,0,0,194,191,1,0,0,0,194,192,1,0,0,0,194,
+        193,1,0,0,0,195,35,1,0,0,0,196,197,5,16,0,0,197,37,1,0,0,0,198,199,
+        5,52,0,0,199,200,5,36,0,0,200,39,1,0,0,0,201,202,5,53,0,0,202,203,
+        5,36,0,0,203,41,1,0,0,0,204,205,5,55,0,0,205,206,5,36,0,0,206,43,
+        1,0,0,0,207,208,5,54,0,0,208,209,5,36,0,0,209,45,1,0,0,0,210,211,
+        5,50,0,0,211,212,3,22,11,0,212,213,5,51,0,0,213,47,1,0,0,0,214,216,
+        5,32,0,0,215,217,5,34,0,0,216,215,1,0,0,0,216,217,1,0,0,0,217,49,
+        1,0,0,0,218,220,5,33,0,0,219,221,5,34,0,0,220,219,1,0,0,0,220,221,
+        1,0,0,0,221,51,1,0,0,0,222,224,3,36,18,0,223,222,1,0,0,0,223,224,
+        1,0,0,0,224,225,1,0,0,0,225,226,5,36,0,0,226,228,5,62,0,0,227,229,
+        3,54,27,0,228,227,1,0,0,0,228,229,1,0,0,0,229,237,1,0,0,0,230,238,
+        3,62,31,0,231,233,7,2,0,0,232,231,1,0,0,0,233,234,1,0,0,0,234,232,
+        1,0,0,0,234,235,1,0,0,0,235,238,1,0,0,0,236,238,5,59,0,0,237,230,
+        1,0,0,0,237,232,1,0,0,0,237,236,1,0,0,0,238,53,1,0,0,0,239,240,7,
+        3,0,0,240,55,1,0,0,0,241,243,3,36,18,0,242,241,1,0,0,0,242,243,1,
+        0,0,0,243,245,1,0,0,0,244,246,5,20,0,0,245,244,1,0,0,0,245,246,1,
+        0,0,0,246,247,1,0,0,0,247,251,5,56,0,0,248,250,3,68,34,0,249,248,
+        1,0,0,0,250,253,1,0,0,0,251,249,1,0,0,0,251,252,1,0,0,0,252,254,
+        1,0,0,0,253,251,1,0,0,0,254,259,3,62,31,0,255,256,5,49,0,0,256,258,
+        3,62,31,0,257,255,1,0,0,0,258,261,1,0,0,0,259,257,1,0,0,0,259,260,
+        1,0,0,0,260,262,1,0,0,0,261,259,1,0,0,0,262,263,5,56,0,0,263,57,
+        1,0,0,0,264,266,3,36,18,0,265,264,1,0,0,0,265,266,1,0,0,0,266,267,
+        1,0,0,0,267,272,5,21,0,0,268,270,5,59,0,0,269,271,5,48,0,0,270,269,
+        1,0,0,0,270,271,1,0,0,0,271,273,1,0,0,0,272,268,1,0,0,0,272,273,
+        1,0,0,0,273,274,1,0,0,0,274,276,3,62,31,0,275,277,5,59,0,0,276,275,
+        1,0,0,0,276,277,1,0,0,0,277,59,1,0,0,0,278,279,5,37,0,0,279,61,1,
+        0,0,0,280,290,5,36,0,0,281,290,5,39,0,0,282,290,5,34,0,0,283,290,
+        5,35,0,0,284,290,3,64,32,0,285,290,3,66,33,0,286,290,3,60,30,0,287,
+        290,5,28,0,0,288,290,5,29,0,0,289,280,1,0,0,0,289,281,1,0,0,0,289,
+        282,1,0,0,0,289,283,1,0,0,0,289,284,1,0,0,0,289,285,1,0,0,0,289,
+        286,1,0,0,0,289,287,1,0,0,0,289,288,1,0,0,0,290,63,1,0,0,0,291,292,
+        5,30,0,0,292,65,1,0,0,0,293,294,5,31,0,0,294,67,1,0,0,0,295,302,
+        5,57,0,0,296,302,5,44,0,0,297,302,5,43,0,0,298,302,3,70,35,0,299,
+        302,3,74,37,0,300,302,3,72,36,0,301,295,1,0,0,0,301,296,1,0,0,0,
+        301,297,1,0,0,0,301,298,1,0,0,0,301,299,1,0,0,0,301,300,1,0,0,0,
+        302,69,1,0,0,0,303,304,7,4,0,0,304,71,1,0,0,0,305,306,7,5,0,0,306,
+        73,1,0,0,0,307,308,7,6,0,0,308,75,1,0,0,0,309,312,3,78,39,0,310,
+        311,5,49,0,0,311,313,3,78,39,0,312,310,1,0,0,0,312,313,1,0,0,0,313,
+        316,1,0,0,0,314,315,5,49,0,0,315,317,3,78,39,0,316,314,1,0,0,0,316,
+        317,1,0,0,0,317,320,1,0,0,0,318,319,5,49,0,0,319,321,3,78,39,0,320,
+        318,1,0,0,0,320,321,1,0,0,0,321,77,1,0,0,0,322,330,3,90,45,0,323,
+        330,3,92,46,0,324,330,3,88,44,0,325,330,5,53,0,0,326,330,5,52,0,
+        0,327,330,5,55,0,0,328,330,5,54,0,0,329,322,1,0,0,0,329,323,1,0,
+        0,0,329,324,1,0,0,0,329,325,1,0,0,0,329,326,1,0,0,0,329,327,1,0,
+        0,0,329,328,1,0,0,0,330,79,1,0,0,0,331,336,3,82,41,0,332,333,5,49,
+        0,0,333,335,3,82,41,0,334,332,1,0,0,0,335,338,1,0,0,0,336,334,1,
+        0,0,0,336,337,1,0,0,0,337,81,1,0,0,0,338,336,1,0,0,0,339,344,3,84,
+        42,0,340,344,3,86,43,0,341,344,3,88,44,0,342,344,3,92,46,0,343,339,
+        1,0,0,0,343,340,1,0,0,0,343,341,1,0,0,0,343,342,1,0,0,0,344,83,1,
+        0,0,0,345,346,5,22,0,0,346,85,1,0,0,0,347,348,5,23,0,0,348,87,1,
+        0,0,0,349,350,5,24,0,0,350,89,1,0,0,0,351,352,5,25,0,0,352,91,1,
+        0,0,0,353,354,5,26,0,0,354,93,1,0,0,0,35,96,100,105,110,114,140,
+        153,161,173,178,185,188,194,216,220,223,228,234,237,242,245,251,
+        259,265,270,272,276,289,301,312,316,320,329,336,343
     ]
 
 class ZorgQueryParser ( Parser ):
 
     grammarFileName = "ZorgQuery.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -134,31 +150,31 @@
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     sharedContextCache = PredictionContextCache()
 
     literalNames = [ "<INVALID>", "'S'", "'W'", "'O'", "'G'", "'note'", 
                      "'or'", "'1'", "'2'", "'3'", "'4'", "'5'", "'6'", "'7'", 
                      "'8'", "'9'", "'!'", "'0'", "'<='", "'>='", "'c'", 
-                     "'create'", "'modify'", "'priority'", "'file'", "'type'", 
-                     "<INVALID>", "'o'", "'x'", "<INVALID>", "<INVALID>", 
+                     "'f='", "'create'", "'modify'", "'priority'", "'file'", 
+                     "'type'", "<INVALID>", "'o'", "'x'", "<INVALID>", "<INVALID>", 
                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                      "'  -'", "'    -'", "<INVALID>", "'$'", "'^'", "'-'", 
                      "'.'", "'/'", "'_'", "' '", "'('", "')'", "'#'", "'@'", 
                      "'+'", "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'", 
                      "':'" ]
 
     symbolicNames = [ "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
-                      "<INVALID>", "<INVALID>", "NL", "LOWER_O", "LOWER_X", 
-                      "DATE", "TIME", "CREATE_RANGE_HEAD", "MODIFY_RANGE_HEAD", 
+                      "<INVALID>", "<INVALID>", "<INVALID>", "NL", "LOWER_O", 
+                      "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", "MODIFY_RANGE_HEAD", 
                       "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", "SHORT_DATE", 
                       "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", 
                       "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
                       "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
                       "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", 
                       "RANGLE", "COLON" ]
 
@@ -187,37 +203,43 @@
     RULE_project = 22
     RULE_subfilter = 23
     RULE_create_range = 24
     RULE_modify_range = 25
     RULE_prop_filter = 26
     RULE_prop_op = 27
     RULE_desc_filter = 28
-    RULE_zid = 29
-    RULE_id = 30
-    RULE_date = 31
-    RULE_time = 32
-    RULE_group_by_body = 33
-    RULE_group_by_atom = 34
-    RULE_order_by_body = 35
-    RULE_order_by_atom = 36
-    RULE_create = 37
-    RULE_modify = 38
-    RULE_priority = 39
-    RULE_file = 40
-    RULE_type = 41
+    RULE_file_filter = 29
+    RULE_zid = 30
+    RULE_id = 31
+    RULE_date = 32
+    RULE_time = 33
+    RULE_any_non_squote = 34
+    RULE_non_tag_symbol = 35
+    RULE_id_symbol = 36
+    RULE_tag_symbol = 37
+    RULE_group_by_body = 38
+    RULE_group_by_atom = 39
+    RULE_order_by_body = 40
+    RULE_order_by_atom = 41
+    RULE_create = 42
+    RULE_modify = 43
+    RULE_priority = 44
+    RULE_file = 45
+    RULE_type = 46
 
     ruleNames =  [ "prog", "query", "where_query", "select_query", "select", 
                    "where", "order_by", "group_by", "select_body", "note", 
                    "where_body", "or_filter", "and_filter", "where_atom", 
                    "note_type", "note_type_char", "priority_range", "tag", 
                    "not_op", "area", "context", "person", "project", "subfilter", 
                    "create_range", "modify_range", "prop_filter", "prop_op", 
-                   "desc_filter", "zid", "id", "date", "time", "group_by_body", 
-                   "group_by_atom", "order_by_body", "order_by_atom", "create", 
-                   "modify", "priority", "file", "type" ]
+                   "desc_filter", "file_filter", "zid", "id", "date", "time", 
+                   "any_non_squote", "non_tag_symbol", "id_symbol", "tag_symbol", 
+                   "group_by_body", "group_by_atom", "order_by_body", "order_by_atom", 
+                   "create", "modify", "priority", "file", "type" ]
 
     EOF = Token.EOF
     T__0=1
     T__1=2
     T__2=3
     T__3=4
     T__4=5
@@ -237,50 +259,51 @@
     T__18=19
     T__19=20
     T__20=21
     T__21=22
     T__22=23
     T__23=24
     T__24=25
-    NL=26
-    LOWER_O=27
-    LOWER_X=28
-    DATE=29
-    TIME=30
-    CREATE_RANGE_HEAD=31
-    MODIFY_RANGE_HEAD=32
-    DATE_RANGE_TAIL=33
-    PRIORITY=34
-    ID=35
-    ZID=36
-    SHORT_DATE=37
-    NUM_ID=38
-    TWO_SPACE_DASH=39
-    FOUR_SPACE_DASH=40
-    SYMBOL=41
-    DOLLAR=42
-    HAT=43
-    DASH=44
-    DOT=45
-    FSLASH=46
-    UNDERSCORE=47
-    SPACE=48
-    LPAREN=49
-    RPAREN=50
-    HASH=51
-    AT_SIGN=52
-    PLUS=53
-    PERCENT=54
-    SQUOTE=55
-    DQUOTE=56
-    TILDE=57
-    STAR=58
-    LANGLE=59
-    RANGLE=60
-    COLON=61
+    T__25=26
+    NL=27
+    LOWER_O=28
+    LOWER_X=29
+    DATE=30
+    TIME=31
+    CREATE_RANGE_HEAD=32
+    MODIFY_RANGE_HEAD=33
+    DATE_RANGE_TAIL=34
+    PRIORITY=35
+    ID=36
+    ZID=37
+    SHORT_DATE=38
+    NUM_ID=39
+    TWO_SPACE_DASH=40
+    FOUR_SPACE_DASH=41
+    SYMBOL=42
+    DOLLAR=43
+    HAT=44
+    DASH=45
+    DOT=46
+    FSLASH=47
+    UNDERSCORE=48
+    SPACE=49
+    LPAREN=50
+    RPAREN=51
+    HASH=52
+    AT_SIGN=53
+    PLUS=54
+    PERCENT=55
+    SQUOTE=56
+    DQUOTE=57
+    TILDE=58
+    STAR=59
+    LANGLE=60
+    RANGLE=61
+    COLON=62
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
@@ -318,21 +341,21 @@
     def prog(self):
 
         localctx = ZorgQueryParser.ProgContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_prog)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 84
+            self.state = 94
             self.query()
-            self.state = 86
+            self.state = 96
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==26:
-                self.state = 85
+            if _la==27:
+                self.state = 95
                 self.match(ZorgQueryParser.NL)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -371,26 +394,26 @@
 
 
     def query(self):
 
         localctx = ZorgQueryParser.QueryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_query)
         try:
-            self.state = 90
+            self.state = 100
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,1,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 88
+                self.state = 98
                 self.where_query()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 89
+                self.state = 99
                 self.select_query()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -446,43 +469,43 @@
     def where_query(self):
 
         localctx = ZorgQueryParser.Where_queryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_where_query)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 95
+            self.state = 105
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==1:
-                self.state = 92
+                self.state = 102
                 self.select()
-                self.state = 93
+                self.state = 103
                 self.match(ZorgQueryParser.SPACE)
 
 
-            self.state = 97
+            self.state = 107
             self.where()
-            self.state = 100
+            self.state = 110
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,3,self._ctx)
             if la_ == 1:
-                self.state = 98
+                self.state = 108
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 99
+                self.state = 109
                 self.order_by()
 
 
-            self.state = 104
+            self.state = 114
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==48:
-                self.state = 102
+            if _la==49:
+                self.state = 112
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 103
+                self.state = 113
                 self.group_by()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -518,15 +541,15 @@
 
     def select_query(self):
 
         localctx = ZorgQueryParser.Select_queryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_select_query)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 106
+            self.state = 116
             self.select()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -563,19 +586,19 @@
 
     def select(self):
 
         localctx = ZorgQueryParser.SelectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_select)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 108
+            self.state = 118
             self.match(ZorgQueryParser.T__0)
-            self.state = 109
+            self.state = 119
             self.match(ZorgQueryParser.SPACE)
-            self.state = 110
+            self.state = 120
             self.select_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -612,19 +635,19 @@
 
     def where(self):
 
         localctx = ZorgQueryParser.WhereContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_where)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 112
+            self.state = 122
             self.match(ZorgQueryParser.T__1)
-            self.state = 113
+            self.state = 123
             self.match(ZorgQueryParser.SPACE)
-            self.state = 114
+            self.state = 124
             self.where_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -661,19 +684,19 @@
 
     def order_by(self):
 
         localctx = ZorgQueryParser.Order_byContext(self, self._ctx, self.state)
         self.enterRule(localctx, 12, self.RULE_order_by)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 116
+            self.state = 126
             self.match(ZorgQueryParser.T__2)
-            self.state = 117
+            self.state = 127
             self.match(ZorgQueryParser.SPACE)
-            self.state = 118
+            self.state = 128
             self.order_by_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -710,19 +733,19 @@
 
     def group_by(self):
 
         localctx = ZorgQueryParser.Group_byContext(self, self._ctx, self.state)
         self.enterRule(localctx, 14, self.RULE_group_by)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 120
+            self.state = 130
             self.match(ZorgQueryParser.T__3)
-            self.state = 121
+            self.state = 131
             self.match(ZorgQueryParser.SPACE)
-            self.state = 122
+            self.state = 132
             self.group_by_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -771,45 +794,45 @@
 
 
     def select_body(self):
 
         localctx = ZorgQueryParser.Select_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 16, self.RULE_select_body)
         try:
-            self.state = 130
+            self.state = 140
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [24]:
+            if token in [25]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 124
+                self.state = 134
                 self.file_()
                 pass
             elif token in [5]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 125
+                self.state = 135
                 self.note()
                 pass
-            elif token in [52]:
+            elif token in [53]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 126
+                self.state = 136
                 self.match(ZorgQueryParser.AT_SIGN)
                 pass
-            elif token in [51]:
+            elif token in [52]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 127
+                self.state = 137
                 self.match(ZorgQueryParser.HASH)
                 pass
-            elif token in [53]:
+            elif token in [54]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 128
+                self.state = 138
                 self.match(ZorgQueryParser.PLUS)
                 pass
-            elif token in [54]:
+            elif token in [55]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 129
+                self.state = 139
                 self.match(ZorgQueryParser.PERCENT)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -844,15 +867,15 @@
 
     def note(self):
 
         localctx = ZorgQueryParser.NoteContext(self, self._ctx, self.state)
         self.enterRule(localctx, 18, self.RULE_note)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 132
+            self.state = 142
             self.match(ZorgQueryParser.T__4)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -886,15 +909,15 @@
 
     def where_body(self):
 
         localctx = ZorgQueryParser.Where_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 20, self.RULE_where_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 134
+            self.state = 144
             self.or_filter()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -937,30 +960,30 @@
 
     def or_filter(self):
 
         localctx = ZorgQueryParser.Or_filterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 22, self.RULE_or_filter)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 136
+            self.state = 146
             self.and_filter()
-            self.state = 143
+            self.state = 153
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,6,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 137
+                    self.state = 147
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 138
+                    self.state = 148
                     self.match(ZorgQueryParser.T__5)
-                    self.state = 139
+                    self.state = 149
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 140
+                    self.state = 150
                     self.and_filter() 
-                self.state = 145
+                self.state = 155
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,6,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1005,26 +1028,26 @@
 
     def and_filter(self):
 
         localctx = ZorgQueryParser.And_filterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 24, self.RULE_and_filter)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 146
+            self.state = 156
             self.where_atom()
-            self.state = 151
+            self.state = 161
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 147
+                    self.state = 157
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 148
+                    self.state = 158
                     self.where_atom() 
-                self.state = 153
+                self.state = 163
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1068,14 +1091,18 @@
             return self.getTypedRuleContext(ZorgQueryParser.Prop_filterContext,0)
 
 
         def desc_filter(self):
             return self.getTypedRuleContext(ZorgQueryParser.Desc_filterContext,0)
 
 
+        def file_filter(self):
+            return self.getTypedRuleContext(ZorgQueryParser.File_filterContext,0)
+
+
         def getRuleIndex(self):
             return ZorgQueryParser.RULE_where_atom
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterWhere_atom" ):
                 listener.enterWhere_atom(self)
 
@@ -1087,65 +1114,71 @@
 
 
     def where_atom(self):
 
         localctx = ZorgQueryParser.Where_atomContext(self, self._ctx, self.state)
         self.enterRule(localctx, 26, self.RULE_where_atom)
         try:
-            self.state = 162
+            self.state = 173
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,8,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 154
+                self.state = 164
                 self.note_type()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 155
+                self.state = 165
                 self.priority_range()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 156
+                self.state = 166
                 self.tag()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 157
+                self.state = 167
                 self.subfilter()
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 158
+                self.state = 168
                 self.create_range()
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 159
+                self.state = 169
                 self.modify_range()
                 pass
 
             elif la_ == 7:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 160
+                self.state = 170
                 self.prop_filter()
                 pass
 
             elif la_ == 8:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 161
+                self.state = 171
                 self.desc_filter()
                 pass
 
+            elif la_ == 9:
+                self.enterOuterAlt(localctx, 9)
+                self.state = 172
+                self.file_filter()
+                pass
+
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1183,24 +1216,24 @@
     def note_type(self):
 
         localctx = ZorgQueryParser.Note_typeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 28, self.RULE_note_type)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 165 
+            self.state = 176 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 164
+                self.state = 175
                 self.note_type_char()
-                self.state = 167 
+                self.state = 178 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1873515037574823936) != 0)):
+                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 3747030075149647872) != 0)):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -1250,17 +1283,17 @@
     def note_type_char(self):
 
         localctx = ZorgQueryParser.Note_type_charContext(self, self._ctx, self.state)
         self.enterRule(localctx, 30, self.RULE_note_type_char)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 169
+            self.state = 180
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1873515037574823936) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 3747030075149647872) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1300,23 +1333,23 @@
     def priority_range(self):
 
         localctx = ZorgQueryParser.Priority_rangeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 32, self.RULE_priority_range)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 171
+            self.state = 182
             self.match(ZorgQueryParser.PRIORITY)
-            self.state = 174
+            self.state = 185
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==44:
-                self.state = 172
+            if _la==45:
+                self.state = 183
                 self.match(ZorgQueryParser.DASH)
-                self.state = 173
+                self.state = 184
                 _la = self._input.LA(1)
                 if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 65408) != 0)):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
 
@@ -1374,39 +1407,39 @@
     def tag(self):
 
         localctx = ZorgQueryParser.TagContext(self, self._ctx, self.state)
         self.enterRule(localctx, 34, self.RULE_tag)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 177
+            self.state = 188
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==16:
-                self.state = 176
+                self.state = 187
                 self.not_op()
 
 
-            self.state = 183
+            self.state = 194
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [51]:
-                self.state = 179
+            if token in [52]:
+                self.state = 190
                 self.area()
                 pass
-            elif token in [52]:
-                self.state = 180
+            elif token in [53]:
+                self.state = 191
                 self.context()
                 pass
-            elif token in [54]:
-                self.state = 181
+            elif token in [55]:
+                self.state = 192
                 self.person()
                 pass
-            elif token in [53]:
-                self.state = 182
+            elif token in [54]:
+                self.state = 193
                 self.project()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1441,15 +1474,15 @@
 
     def not_op(self):
 
         localctx = ZorgQueryParser.Not_opContext(self, self._ctx, self.state)
         self.enterRule(localctx, 36, self.RULE_not_op)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 185
+            self.state = 196
             self.match(ZorgQueryParser.T__15)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1485,17 +1518,17 @@
 
     def area(self):
 
         localctx = ZorgQueryParser.AreaContext(self, self._ctx, self.state)
         self.enterRule(localctx, 38, self.RULE_area)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 187
+            self.state = 198
             self.match(ZorgQueryParser.HASH)
-            self.state = 188
+            self.state = 199
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1531,17 +1564,17 @@
 
     def context(self):
 
         localctx = ZorgQueryParser.ContextContext(self, self._ctx, self.state)
         self.enterRule(localctx, 40, self.RULE_context)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 190
+            self.state = 201
             self.match(ZorgQueryParser.AT_SIGN)
-            self.state = 191
+            self.state = 202
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1577,17 +1610,17 @@
 
     def person(self):
 
         localctx = ZorgQueryParser.PersonContext(self, self._ctx, self.state)
         self.enterRule(localctx, 42, self.RULE_person)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 193
+            self.state = 204
             self.match(ZorgQueryParser.PERCENT)
-            self.state = 194
+            self.state = 205
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1623,17 +1656,17 @@
 
     def project(self):
 
         localctx = ZorgQueryParser.ProjectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 44, self.RULE_project)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 196
+            self.state = 207
             self.match(ZorgQueryParser.PLUS)
-            self.state = 197
+            self.state = 208
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1673,19 +1706,19 @@
 
     def subfilter(self):
 
         localctx = ZorgQueryParser.SubfilterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 46, self.RULE_subfilter)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 199
+            self.state = 210
             self.match(ZorgQueryParser.LPAREN)
-            self.state = 200
+            self.state = 211
             self.or_filter()
-            self.state = 201
+            self.state = 212
             self.match(ZorgQueryParser.RPAREN)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1722,21 +1755,21 @@
     def create_range(self):
 
         localctx = ZorgQueryParser.Create_rangeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 48, self.RULE_create_range)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 203
+            self.state = 214
             self.match(ZorgQueryParser.CREATE_RANGE_HEAD)
-            self.state = 205
+            self.state = 216
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==33:
-                self.state = 204
+            if _la==34:
+                self.state = 215
                 self.match(ZorgQueryParser.DATE_RANGE_TAIL)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1775,21 +1808,21 @@
     def modify_range(self):
 
         localctx = ZorgQueryParser.Modify_rangeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 50, self.RULE_modify_range)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 207
+            self.state = 218
             self.match(ZorgQueryParser.MODIFY_RANGE_HEAD)
-            self.state = 209
+            self.state = 220
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==33:
-                self.state = 208
+            if _la==34:
+                self.state = 219
                 self.match(ZorgQueryParser.DATE_RANGE_TAIL)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1801,23 +1834,24 @@
     class Prop_filterContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def ID(self, i:int=None):
-            if i is None:
-                return self.getTokens(ZorgQueryParser.ID)
-            else:
-                return self.getToken(ZorgQueryParser.ID, i)
+        def ID(self):
+            return self.getToken(ZorgQueryParser.ID, 0)
 
         def COLON(self):
             return self.getToken(ZorgQueryParser.COLON, 0)
 
+        def id_(self):
+            return self.getTypedRuleContext(ZorgQueryParser.IdContext,0)
+
+
         def STAR(self):
             return self.getToken(ZorgQueryParser.STAR, 0)
 
         def not_op(self):
             return self.getTypedRuleContext(ZorgQueryParser.Not_opContext,0)
 
 
@@ -1842,78 +1876,62 @@
     def prop_filter(self):
 
         localctx = ZorgQueryParser.Prop_filterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 52, self.RULE_prop_filter)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 212
+            self.state = 223
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==16:
-                self.state = 211
+                self.state = 222
                 self.not_op()
 
 
-            self.state = 214
+            self.state = 225
             self.match(ZorgQueryParser.ID)
-            self.state = 215
+            self.state = 226
             self.match(ZorgQueryParser.COLON)
-            self.state = 217
+            self.state = 228
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if (((_la) & ~0x3f) == 0 and ((1 << _la) & 1729382256911056896) != 0):
-                self.state = 216
+            if (((_la) & ~0x3f) == 0 and ((1 << _la) & 3458764513821327360) != 0):
+                self.state = 227
                 self.prop_op()
 
 
-            self.state = 231
+            self.state = 237
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [7, 8, 9, 10, 11, 12, 13, 14, 15, 17, 35]:
-                self.state = 225
+            if token in [28, 29, 30, 31, 34, 35, 36, 37, 39]:
+                self.state = 230
+                self.id_()
+                pass
+            elif token in [7, 8, 9, 10, 11, 12, 13, 14, 15, 17]:
+                self.state = 232 
                 self._errHandler.sync(self)
-                token = self._input.LA(1)
-                if token in [35]:
-                    self.state = 219
-                    self.match(ZorgQueryParser.ID)
-                    pass
-                elif token in [7, 8, 9, 10, 11, 12, 13, 14, 15, 17]:
-                    self.state = 221 
+                _la = self._input.LA(1)
+                while True:
+                    self.state = 231
+                    _la = self._input.LA(1)
+                    if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 196480) != 0)):
+                        self._errHandler.recoverInline(self)
+                    else:
+                        self._errHandler.reportMatch(self)
+                        self.consume()
+                    self.state = 234 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    while True:
-                        self.state = 220
-                        _la = self._input.LA(1)
-                        if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 196480) != 0)):
-                            self._errHandler.recoverInline(self)
-                        else:
-                            self._errHandler.reportMatch(self)
-                            self.consume()
-                        self.state = 223 
-                        self._errHandler.sync(self)
-                        _la = self._input.LA(1)
-                        if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 196480) != 0)):
-                            break
-
-                    pass
-                else:
-                    raise NoViableAltException(self)
-
-                self.state = 228
-                self._errHandler.sync(self)
-                _la = self._input.LA(1)
-                if _la==58:
-                    self.state = 227
-                    self.match(ZorgQueryParser.STAR)
-
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 196480) != 0)):
+                        break
 
                 pass
-            elif token in [58]:
-                self.state = 230
+            elif token in [59]:
+                self.state = 236
                 self.match(ZorgQueryParser.STAR)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1954,17 +1972,17 @@
     def prop_op(self):
 
         localctx = ZorgQueryParser.Prop_opContext(self, self._ctx, self.state)
         self.enterRule(localctx, 54, self.RULE_prop_op)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 233
+            self.state = 239
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1729382256911056896) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 3458764513821327360) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1994,14 +2012,21 @@
                 return self.getTypedRuleContext(ZorgQueryParser.IdContext,i)
 
 
         def not_op(self):
             return self.getTypedRuleContext(ZorgQueryParser.Not_opContext,0)
 
 
+        def any_non_squote(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgQueryParser.Any_non_squoteContext)
+            else:
+                return self.getTypedRuleContext(ZorgQueryParser.Any_non_squoteContext,i)
+
+
         def SPACE(self, i:int=None):
             if i is None:
                 return self.getTokens(ZorgQueryParser.SPACE)
             else:
                 return self.getToken(ZorgQueryParser.SPACE, i)
 
         def getRuleIndex(self):
@@ -2021,57 +2046,157 @@
     def desc_filter(self):
 
         localctx = ZorgQueryParser.Desc_filterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 56, self.RULE_desc_filter)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 236
+            self.state = 242
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==16:
-                self.state = 235
+                self.state = 241
                 self.not_op()
 
 
-            self.state = 239
+            self.state = 245
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==20:
-                self.state = 238
+                self.state = 244
                 self.match(ZorgQueryParser.T__19)
 
 
-            self.state = 241
+            self.state = 247
             self.match(ZorgQueryParser.SQUOTE)
-            self.state = 242
+            self.state = 251
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while (((_la) & ~0x3f) == 0 and ((1 << _la) & 9150747094816915456) != 0):
+                self.state = 248
+                self.any_non_squote()
+                self.state = 253
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+
+            self.state = 254
             self.id_()
-            self.state = 247
+            self.state = 259
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==48:
-                self.state = 243
+            while _la==49:
+                self.state = 255
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 244
+                self.state = 256
                 self.id_()
-                self.state = 249
+                self.state = 261
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
-            self.state = 250
+            self.state = 262
             self.match(ZorgQueryParser.SQUOTE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
+    class File_filterContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def id_(self):
+            return self.getTypedRuleContext(ZorgQueryParser.IdContext,0)
+
+
+        def not_op(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Not_opContext,0)
+
+
+        def STAR(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgQueryParser.STAR)
+            else:
+                return self.getToken(ZorgQueryParser.STAR, i)
+
+        def UNDERSCORE(self):
+            return self.getToken(ZorgQueryParser.UNDERSCORE, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_file_filter
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterFile_filter" ):
+                listener.enterFile_filter(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitFile_filter" ):
+                listener.exitFile_filter(self)
+
+
+
+
+    def file_filter(self):
+
+        localctx = ZorgQueryParser.File_filterContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 58, self.RULE_file_filter)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 265
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==16:
+                self.state = 264
+                self.not_op()
+
+
+            self.state = 267
+            self.match(ZorgQueryParser.T__20)
+            self.state = 272
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==59:
+                self.state = 268
+                self.match(ZorgQueryParser.STAR)
+                self.state = 270
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+                if _la==48:
+                    self.state = 269
+                    self.match(ZorgQueryParser.UNDERSCORE)
+
+
+
+
+            self.state = 274
+            self.id_()
+            self.state = 276
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==59:
+                self.state = 275
+                self.match(ZorgQueryParser.STAR)
+
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
     class ZidContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
@@ -2091,18 +2216,18 @@
 
 
 
 
     def zid(self):
 
         localctx = ZorgQueryParser.ZidContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 58, self.RULE_zid)
+        self.enterRule(localctx, 60, self.RULE_zid)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 252
+            self.state = 278
             self.match(ZorgQueryParser.ZID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2159,62 +2284,62 @@
 
 
 
 
     def id_(self):
 
         localctx = ZorgQueryParser.IdContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 60, self.RULE_id)
+        self.enterRule(localctx, 62, self.RULE_id)
         try:
-            self.state = 263
+            self.state = 289
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [35]:
+            if token in [36]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 254
+                self.state = 280
                 self.match(ZorgQueryParser.ID)
                 pass
-            elif token in [38]:
+            elif token in [39]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 255
+                self.state = 281
                 self.match(ZorgQueryParser.NUM_ID)
                 pass
-            elif token in [33]:
+            elif token in [34]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 256
+                self.state = 282
                 self.match(ZorgQueryParser.DATE_RANGE_TAIL)
                 pass
-            elif token in [34]:
+            elif token in [35]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 257
+                self.state = 283
                 self.match(ZorgQueryParser.PRIORITY)
                 pass
-            elif token in [29]:
+            elif token in [30]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 258
+                self.state = 284
                 self.date()
                 pass
-            elif token in [30]:
+            elif token in [31]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 259
+                self.state = 285
                 self.time()
                 pass
-            elif token in [36]:
+            elif token in [37]:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 260
+                self.state = 286
                 self.zid()
                 pass
-            elif token in [27]:
+            elif token in [28]:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 261
+                self.state = 287
                 self.match(ZorgQueryParser.LOWER_O)
                 pass
-            elif token in [28]:
+            elif token in [29]:
                 self.enterOuterAlt(localctx, 9)
-                self.state = 262
+                self.state = 288
                 self.match(ZorgQueryParser.LOWER_X)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2248,18 +2373,18 @@
 
 
 
 
     def date(self):
 
         localctx = ZorgQueryParser.DateContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 62, self.RULE_date)
+        self.enterRule(localctx, 64, self.RULE_date)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 265
+            self.state = 291
             self.match(ZorgQueryParser.DATE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2289,28 +2414,300 @@
 
 
 
 
     def time(self):
 
         localctx = ZorgQueryParser.TimeContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 64, self.RULE_time)
+        self.enterRule(localctx, 66, self.RULE_time)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 267
+            self.state = 293
             self.match(ZorgQueryParser.TIME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
+    class Any_non_squoteContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def DQUOTE(self):
+            return self.getToken(ZorgQueryParser.DQUOTE, 0)
+
+        def HAT(self):
+            return self.getToken(ZorgQueryParser.HAT, 0)
+
+        def DOLLAR(self):
+            return self.getToken(ZorgQueryParser.DOLLAR, 0)
+
+        def non_tag_symbol(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Non_tag_symbolContext,0)
+
+
+        def tag_symbol(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Tag_symbolContext,0)
+
+
+        def id_symbol(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Id_symbolContext,0)
+
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_any_non_squote
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterAny_non_squote" ):
+                listener.enterAny_non_squote(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitAny_non_squote" ):
+                listener.exitAny_non_squote(self)
+
+
+
+
+    def any_non_squote(self):
+
+        localctx = ZorgQueryParser.Any_non_squoteContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 68, self.RULE_any_non_squote)
+        try:
+            self.state = 301
+            self._errHandler.sync(self)
+            token = self._input.LA(1)
+            if token in [57]:
+                self.enterOuterAlt(localctx, 1)
+                self.state = 295
+                self.match(ZorgQueryParser.DQUOTE)
+                pass
+            elif token in [44]:
+                self.enterOuterAlt(localctx, 2)
+                self.state = 296
+                self.match(ZorgQueryParser.HAT)
+                pass
+            elif token in [43]:
+                self.enterOuterAlt(localctx, 3)
+                self.state = 297
+                self.match(ZorgQueryParser.DOLLAR)
+                pass
+            elif token in [42, 48, 50, 51, 58, 59, 60, 61]:
+                self.enterOuterAlt(localctx, 4)
+                self.state = 298
+                self.non_tag_symbol()
+                pass
+            elif token in [52, 53, 54, 55]:
+                self.enterOuterAlt(localctx, 5)
+                self.state = 299
+                self.tag_symbol()
+                pass
+            elif token in [45, 46, 47, 62]:
+                self.enterOuterAlt(localctx, 6)
+                self.state = 300
+                self.id_symbol()
+                pass
+            else:
+                raise NoViableAltException(self)
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Non_tag_symbolContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def LANGLE(self):
+            return self.getToken(ZorgQueryParser.LANGLE, 0)
+
+        def RANGLE(self):
+            return self.getToken(ZorgQueryParser.RANGLE, 0)
+
+        def STAR(self):
+            return self.getToken(ZorgQueryParser.STAR, 0)
+
+        def TILDE(self):
+            return self.getToken(ZorgQueryParser.TILDE, 0)
+
+        def SYMBOL(self):
+            return self.getToken(ZorgQueryParser.SYMBOL, 0)
+
+        def LPAREN(self):
+            return self.getToken(ZorgQueryParser.LPAREN, 0)
+
+        def RPAREN(self):
+            return self.getToken(ZorgQueryParser.RPAREN, 0)
+
+        def UNDERSCORE(self):
+            return self.getToken(ZorgQueryParser.UNDERSCORE, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_non_tag_symbol
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterNon_tag_symbol" ):
+                listener.enterNon_tag_symbol(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitNon_tag_symbol" ):
+                listener.exitNon_tag_symbol(self)
+
+
+
+
+    def non_tag_symbol(self):
+
+        localctx = ZorgQueryParser.Non_tag_symbolContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 70, self.RULE_non_tag_symbol)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 303
+            _la = self._input.LA(1)
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 4327119215019425792) != 0)):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Id_symbolContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def DASH(self):
+            return self.getToken(ZorgQueryParser.DASH, 0)
+
+        def DOT(self):
+            return self.getToken(ZorgQueryParser.DOT, 0)
+
+        def FSLASH(self):
+            return self.getToken(ZorgQueryParser.FSLASH, 0)
+
+        def COLON(self):
+            return self.getToken(ZorgQueryParser.COLON, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_id_symbol
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterId_symbol" ):
+                listener.enterId_symbol(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitId_symbol" ):
+                listener.exitId_symbol(self)
+
+
+
+
+    def id_symbol(self):
+
+        localctx = ZorgQueryParser.Id_symbolContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 72, self.RULE_id_symbol)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 305
+            _la = self._input.LA(1)
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 4611932309032009728) != 0)):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Tag_symbolContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def HASH(self):
+            return self.getToken(ZorgQueryParser.HASH, 0)
+
+        def AT_SIGN(self):
+            return self.getToken(ZorgQueryParser.AT_SIGN, 0)
+
+        def PERCENT(self):
+            return self.getToken(ZorgQueryParser.PERCENT, 0)
+
+        def PLUS(self):
+            return self.getToken(ZorgQueryParser.PLUS, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_tag_symbol
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterTag_symbol" ):
+                listener.enterTag_symbol(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitTag_symbol" ):
+                listener.exitTag_symbol(self)
+
+
+
+
+    def tag_symbol(self):
+
+        localctx = ZorgQueryParser.Tag_symbolContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 74, self.RULE_tag_symbol)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 307
+            _la = self._input.LA(1)
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 67553994410557440) != 0)):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
     class Group_by_bodyContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
@@ -2340,47 +2737,47 @@
 
 
 
 
     def group_by_body(self):
 
         localctx = ZorgQueryParser.Group_by_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 66, self.RULE_group_by_body)
+        self.enterRule(localctx, 76, self.RULE_group_by_body)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 269
+            self.state = 309
             self.group_by_atom()
-            self.state = 272
+            self.state = 312
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,25,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,29,self._ctx)
             if la_ == 1:
-                self.state = 270
+                self.state = 310
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 271
+                self.state = 311
                 self.group_by_atom()
 
 
-            self.state = 276
+            self.state = 316
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,26,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,30,self._ctx)
             if la_ == 1:
-                self.state = 274
+                self.state = 314
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 275
+                self.state = 315
                 self.group_by_atom()
 
 
-            self.state = 280
+            self.state = 320
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==48:
-                self.state = 278
+            if _la==49:
+                self.state = 318
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 279
+                self.state = 319
                 self.group_by_atom()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -2433,52 +2830,52 @@
 
 
 
 
     def group_by_atom(self):
 
         localctx = ZorgQueryParser.Group_by_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 68, self.RULE_group_by_atom)
+        self.enterRule(localctx, 78, self.RULE_group_by_atom)
         try:
-            self.state = 289
+            self.state = 329
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [24]:
+            if token in [25]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 282
+                self.state = 322
                 self.file_()
                 pass
-            elif token in [25]:
+            elif token in [26]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 283
+                self.state = 323
                 self.type_()
                 pass
-            elif token in [23]:
+            elif token in [24]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 284
+                self.state = 324
                 self.priority()
                 pass
-            elif token in [52]:
+            elif token in [53]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 285
+                self.state = 325
                 self.match(ZorgQueryParser.AT_SIGN)
                 pass
-            elif token in [51]:
+            elif token in [52]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 286
+                self.state = 326
                 self.match(ZorgQueryParser.HASH)
                 pass
-            elif token in [54]:
+            elif token in [55]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 287
+                self.state = 327
                 self.match(ZorgQueryParser.PERCENT)
                 pass
-            elif token in [53]:
+            elif token in [54]:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 288
+                self.state = 328
                 self.match(ZorgQueryParser.PLUS)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2522,31 +2919,31 @@
 
 
 
 
     def order_by_body(self):
 
         localctx = ZorgQueryParser.Order_by_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 70, self.RULE_order_by_body)
+        self.enterRule(localctx, 80, self.RULE_order_by_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 291
+            self.state = 331
             self.order_by_atom()
-            self.state = 296
+            self.state = 336
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,29,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,33,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 292
+                    self.state = 332
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 293
+                    self.state = 333
                     self.order_by_atom() 
-                self.state = 298
+                self.state = 338
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,29,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,33,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2589,37 +2986,37 @@
 
 
 
 
     def order_by_atom(self):
 
         localctx = ZorgQueryParser.Order_by_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 72, self.RULE_order_by_atom)
+        self.enterRule(localctx, 82, self.RULE_order_by_atom)
         try:
-            self.state = 303
+            self.state = 343
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [21]:
+            if token in [22]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 299
+                self.state = 339
                 self.create()
                 pass
-            elif token in [22]:
+            elif token in [23]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 300
+                self.state = 340
                 self.modify()
                 pass
-            elif token in [23]:
+            elif token in [24]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 301
+                self.state = 341
                 self.priority()
                 pass
-            elif token in [25]:
+            elif token in [26]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 302
+                self.state = 342
                 self.type_()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2651,19 +3048,19 @@
 
 
 
 
     def create(self):
 
         localctx = ZorgQueryParser.CreateContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 74, self.RULE_create)
+        self.enterRule(localctx, 84, self.RULE_create)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 305
-            self.match(ZorgQueryParser.T__20)
+            self.state = 345
+            self.match(ZorgQueryParser.T__21)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2690,19 +3087,19 @@
 
 
 
 
     def modify(self):
 
         localctx = ZorgQueryParser.ModifyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 76, self.RULE_modify)
+        self.enterRule(localctx, 86, self.RULE_modify)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 307
-            self.match(ZorgQueryParser.T__21)
+            self.state = 347
+            self.match(ZorgQueryParser.T__22)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2729,19 +3126,19 @@
 
 
 
 
     def priority(self):
 
         localctx = ZorgQueryParser.PriorityContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 78, self.RULE_priority)
+        self.enterRule(localctx, 88, self.RULE_priority)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 309
-            self.match(ZorgQueryParser.T__22)
+            self.state = 349
+            self.match(ZorgQueryParser.T__23)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2768,19 +3165,19 @@
 
 
 
 
     def file_(self):
 
         localctx = ZorgQueryParser.FileContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 80, self.RULE_file)
+        self.enterRule(localctx, 90, self.RULE_file)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 311
-            self.match(ZorgQueryParser.T__23)
+            self.state = 351
+            self.match(ZorgQueryParser.T__24)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2807,19 +3204,19 @@
 
 
 
 
     def type_(self):
 
         localctx = ZorgQueryParser.TypeContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 82, self.RULE_type)
+        self.enterRule(localctx, 92, self.RULE_type)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 313
-            self.match(ZorgQueryParser.T__24)
+            self.state = 353
+            self.match(ZorgQueryParser.T__25)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `zettel_org-0.7.3/src/zorg/service/common.py` & `zettel_org-0.7.4/src/zorg/service/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/service/compiler/_api.py` & `zettel_org-0.7.4/src/zorg/service/compiler/_api.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/service/compiler/_file_compiler.py` & `zettel_org-0.7.4/src/zorg/service/compiler/_file_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Contains service logic used to compile zorg files."""
 
 from dataclasses import dataclass, field
 import datetime as dt
 from functools import partial
-from typing import Any, Literal, Optional
+from typing import Any, Final, Literal, Optional
 
 import antlr4
 from antlr4.error.ErrorListener import ErrorListener
 from logrus import Logger
 from typist import assert_never
 
 from .. import dates as zdt
@@ -15,14 +15,15 @@
 from ...domain.types import NoteType, TodoPriorityType, TodoStatusPrefixChar
 from ...grammar.zorg_file.ZorgFileListener import ZorgFileListener
 from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
 
 
 TagName = Literal["areas", "contexts", "people", "projects"]
 
+_DEFAULT_PRIORITY: Final[TodoPriorityType] = "P3"
 _LOGGER = Logger(__name__)
 
 
 class ErrorManager(ErrorListener):
     """Keeps track of zorg file syntax errors."""
 
     def __init__(self) -> None:
@@ -117,18 +118,18 @@
     def enterHead(self, ctx: ZorgFileParser.HeadContext) -> None:  # noqa: D102
         del ctx
         self._s.in_head = True
 
     def enterId(self, ctx: ZorgFileParser.IdContext) -> None:  # noqa: D102
         if self._s.in_note:
             self._s.ids_in_note += 1
-            if self._s.ids_in_note == 1 and zdt.is_short_date(
+            if self._s.ids_in_note == 1 and zdt.is_short_date_spec(
                 short_date := ctx.getText()
             ):
-                self._s.modify_date = zdt.from_short_date(short_date)
+                self._s.modify_date = zdt.from_short_date_spec(short_date)
             elif (
                 self._s.ids_in_note == 1
                 or (self._s.ids_in_note == 2 and self._s.modify_date)
             ) and zdt.is_zid(zid := ctx.getText()):
                 self._s.zid = zid
                 zorg_id_date = f"20{zid.split('#')[0]}"
                 self._s.note_date = dt.datetime.strptime(
@@ -225,15 +226,15 @@
             )
             self.zorg_file.has_errors = True
         else:
             todo = Note(id_note_body.getText(), **kwargs)
             self.zorg_file.notes.append(todo)
 
         # Reset todo priority and status back to defaults.
-        self._s.todo_priority = "P2"
+        self._s.todo_priority = _DEFAULT_PRIORITY
         self._s.todo_status = NoteType.OPEN_TODO
 
     def exitH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = False
@@ -439,15 +440,15 @@
     h1_date: Optional[dt.date] = None
     h2_date: Optional[dt.date] = None
     h3_date: Optional[dt.date] = None
     h4_date: Optional[dt.date] = None
     note_date: Optional[dt.date] = None
     modify_date: Optional[dt.date] = None
 
-    todo_priority: TodoPriorityType = "P2"
+    todo_priority: TodoPriorityType = _DEFAULT_PRIORITY
     todo_status: NoteType = NoteType.OPEN_TODO
 
     @property
     def areas(self) -> list[str]:
         """Area tags that are currently in-scope."""
         return self._get_current_tags("areas")
```

### Comparing `zettel_org-0.7.3/src/zorg/service/compiler/_query_compiler.py` & `zettel_org-0.7.4/src/zorg/service/compiler/_query_compiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Contains service logic used to compile zorg queries."""
 
 import datetime as dt
-from typing import Optional, cast
+from typing import Optional, Union, cast
 
 from logrus import Logger
 
 from .. import dates as zdt
 from ...domain.models import (
     DateRange,
     DescFilter,
+    FileFilter,
     PropertyFilter,
     Query,
     WhereAndFilter,
     WhereOrFilter,
 )
 from ...domain.types import (
     DescOperator,
@@ -74,66 +75,48 @@
         create_date_ranges: set[DateRange] = set()
         modify_date_ranges: set[DateRange] = set()
         people: set[str] = set()
         priorities: set[TodoPriorityType] = set()
         projects: set[str] = set()
         property_filters: set[PropertyFilter] = set()
         desc_filters: set[DescFilter] = set()
+        file_filters: set[FileFilter] = set()
 
         where_atoms = cast(
             list[ZorgQueryParser.Where_atomContext], ctx.where_atom()
         )
         for where_atom in where_atoms:
-            if where_atom.note_type():
-                note_type = cast(
-                    ZorgQueryParser.Note_typeContext,
-                    where_atom.note_type(),
-                )
+            if w := where_atom.note_type():
+                note_type = cast(ZorgQueryParser.Note_typeContext, w)
                 note_type_chars = cast(
                     list[ZorgQueryParser.Note_type_charContext],
                     note_type.note_type_char(),
                 )
                 _add_note_types(note_type_chars, allowed_note_types)
-            elif where_atom.priority_range():
-                priority_range = cast(
-                    ZorgQueryParser.Priority_rangeContext,
-                    where_atom.priority_range(),
-                )
+            elif w := where_atom.priority_range():
+                priority_range = cast(ZorgQueryParser.Priority_rangeContext, w)
                 _add_priorities(priority_range, priorities)
-            # TODO(bugyi): De-duplicate create range and modify range parsing.
-            elif x := where_atom.create_range():
-                create_range = cast(ZorgQueryParser.Create_rangeContext, x)
+            elif w := where_atom.create_range():
+                create_range = cast(ZorgQueryParser.Create_rangeContext, w)
                 short_start_date = create_range.CREATE_RANGE_HEAD().getText()[
                     1:
                 ]
-                start_date = zdt.from_short_date(short_start_date)
-
-                end_date: Optional[dt.date] = None
-                if date_range_tail := create_range.DATE_RANGE_TAIL():
-                    short_end_date = date_range_tail.getText()[1:]
-                    end_date = zdt.from_short_date(short_end_date)
-
-                date_range = DateRange(start_date, end_date)
-                create_date_ranges.add(date_range)
-            elif x := where_atom.modify_range():
-                modify_range = cast(ZorgQueryParser.Modify_rangeContext, x)
+                create_date_ranges.add(
+                    _get_date_range(create_range, short_start_date)
+                )
+            elif w := where_atom.modify_range():
+                modify_range = cast(ZorgQueryParser.Modify_rangeContext, w)
                 short_start_date = modify_range.MODIFY_RANGE_HEAD().getText()[
                     1:
                 ]
-                start_date = zdt.from_short_date(short_start_date)
-
-                end_date = None
-                if date_range_tail := modify_range.DATE_RANGE_TAIL():
-                    short_end_date = date_range_tail.getText()[1:]
-                    end_date = zdt.from_short_date(short_end_date)
-
-                date_range = DateRange(start_date, end_date)
-                modify_date_ranges.add(date_range)
-            elif where_atom.tag():
-                tag = cast(ZorgQueryParser.TagContext, where_atom.tag())
+                modify_date_ranges.add(
+                    _get_date_range(modify_range, short_start_date)
+                )
+            elif w := where_atom.tag():
+                tag = cast(ZorgQueryParser.TagContext, w)
                 minus = "-" if tag.not_op() else ""
                 if tag.area():
                     tag_set = areas
                     tag_id = tag.area().ID()
                 elif tag.context():
                     tag_set = contexts
                     tag_id = tag.context().ID()
@@ -143,50 +126,59 @@
                 elif tag.project():
                     tag_set = projects
                     tag_id = tag.project().ID()
                 else:
                     raise RuntimeError(f"Invalid Tag: {tag.getText()}")
 
                 tag_set.add(f"{minus}{tag_id.getText()}")
-            elif where_atom.prop_filter():
-                key, op_value = where_atom.prop_filter().getText().split(":")
-                negated = False
-                if key[0] == "!":
-                    negated = True
-                    key = key[1:]
-                op, value = _split_op_value(op_value)
-                value_type = _get_value_type(value)
-                property_filter = PropertyFilter(
-                    key, value, op=op, value_type=value_type, negated=negated
-                )
-                property_filters.add(property_filter)
-            elif where_atom.desc_filter():
-                desc_filter = where_atom.desc_filter().getText()
+            elif w := where_atom.prop_filter():
+                property_filters.add(_get_property_filter(w))
+            elif w := where_atom.desc_filter():
+                desc_filter = w.getText()
                 desc_op = DescOperator.CONTAINS
                 case_sensitive: Optional[bool] = None
                 if desc_filter[0] == "!":
                     desc_op = DescOperator.NOT_CONTAINS
                     desc_filter = desc_filter[1:]
                 if desc_filter[0] == "c":
                     desc_filter = desc_filter[1:]
                     case_sensitive = True
                 value = desc_filter[1:-1]
                 desc_filters.add(
                     DescFilter(
                         value=value, op=desc_op, case_sensitive=case_sensitive
                     )
                 )
+            elif w := where_atom.file_filter():
+                if w.getText().startswith("!"):
+                    negated = True
+                    path_glob = w.getText()[3:]
+                else:
+                    negated = False
+                    path_glob = w.getText()[2:]
+                path_glob = (
+                    path_glob if path_glob.endswith("*") else f"{path_glob}.zo"
+                )
+                file_filters.add(FileFilter(path_glob, negated=negated))
+            # Subfilters are handled in a different method. See the
+            # enterSubfilter() and exitSubfilter() methods for more
+            # information.
+            elif not where_atom.subfilter():
+                _LOGGER.warning(
+                    f"Unrecognized where atom: {where_atom.getText()}"
+                )
 
         self._and_filter_groups[-1].append(
             WhereAndFilter(
                 allowed_note_types=allowed_note_types,
                 areas=areas,
                 contexts=contexts,
                 create_date_ranges=create_date_ranges,
                 desc_filters=desc_filters,
+                file_filters=file_filters,
                 modify_date_ranges=modify_date_ranges,
                 people=people,
                 priorities=priorities,
                 projects=projects,
                 property_filters=property_filters,
             )
         )
@@ -224,27 +216,27 @@
         self, ctx: ZorgQueryParser.Order_by_bodyContext
     ) -> None:  # noqa: D102
         order_by_types = []
         for order_by_atom in cast(
             list[ZorgQueryParser.Order_by_atomContext], ctx.order_by_atom()
         ):
             if order_by_atom.create():
-                group_by_type = OrderByType.CREATE_DATE
+                order_by_type = OrderByType.CREATE_DATE
             elif order_by_atom.modify():
-                group_by_type = OrderByType.MODIFY_DATE
+                order_by_type = OrderByType.MODIFY_DATE
             elif order_by_atom.priority():
-                group_by_type = OrderByType.PRIORITY
+                order_by_type = OrderByType.PRIORITY
             elif order_by_atom.type_():
-                group_by_type = OrderByType.NOTE_TYPE
+                order_by_type = OrderByType.NOTE_TYPE
             else:
                 raise RuntimeError(
                     f"Invalid GROUP BY atom: {order_by_atom.getText()}"
                 )
 
-            order_by_types.append(group_by_type)
+            order_by_types.append(order_by_type)
         self.zorg_query.order_by = tuple(order_by_types)
 
     def enterSubfilter(
         self, ctx: ZorgQueryParser.SubfilterContext
     ) -> None:  # noqa: D102
         del ctx
         self._and_filter_groups.append([])
@@ -268,14 +260,46 @@
         self, ctx: ZorgQueryParser.WhereContext
     ) -> None:  # noqa: D102
         del ctx
         where = WhereOrFilter(self._and_filter_groups[-1])
         self.zorg_query.where = where
 
 
+def _get_date_range(
+    range_ctx: Union[
+        ZorgQueryParser.Create_rangeContext,
+        ZorgQueryParser.Modify_rangeContext,
+    ],
+    short_start_date: str,
+) -> DateRange:
+    start_date = zdt.from_short_date_spec(short_start_date)
+
+    end_date: Optional[dt.date] = None
+    if date_range_tail := range_ctx.DATE_RANGE_TAIL():
+        short_end_date = date_range_tail.getText()[1:]
+        end_date = zdt.from_short_date_spec(short_end_date)
+
+    return DateRange(start_date, end_date)
+
+
+def _get_property_filter(
+    w: ZorgQueryParser.Prop_filterContext,
+) -> PropertyFilter:
+    key, op_value = w.getText().split(":")
+    negated = False
+    if key[0] == "!":
+        negated = True
+        key = key[1:]
+    op, value = _split_op_value(op_value)
+    value_type = _get_value_type(value)
+    return PropertyFilter(
+        key, value, op=op, value_type=value_type, negated=negated
+    )
+
+
 def _split_op_value(op_value: str) -> tuple[PropertyOperator, str]:
     if op_value[0] == "<":
         op_value = op_value[1:]
         if op_value[0] == "=":
             return (PropertyOperator.LE, op_value[1:])
         return (PropertyOperator.LT, op_value)
     elif op_value[0] == ">":
@@ -286,15 +310,15 @@
     elif op_value[0] == "*" and len(op_value) == 1:
         return (PropertyOperator.EXISTS, "")
     else:
         return (PropertyOperator.EQ, op_value)
 
 
 def _get_value_type(value: str) -> PropertyValueType:
-    if zdt.is_date(value):
+    if zdt.is_date_spec(value):
         return PropertyValueType.DATE
     elif all(ch.isdigit() for ch in value):
         return PropertyValueType.INTEGER
 
     return PropertyValueType.STRING
```

### Comparing `zettel_org-0.7.3/src/zorg/service/dates.py` & `zettel_org-0.7.4/src/zorg/service/dates.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 from typing import Final
 
 
 _SHORT_DATE_FMT: Final = "%Y%m%d"
 _LONG_DATE_FMT: Final = "%Y-%m-%d"
 
 
-def from_short_date(short_date: str) -> dt.date:
+def from_date_spec(date_spec: str) -> dt.date:
+    """Converts some date string spec to an actual date."""
+    if is_short_date_spec(date_spec):
+        return from_short_date_spec(date_spec)
+    elif _is_long_date_spec(date_spec):
+        return _from_long_date_spec(date_spec)
+    else:
+        raise RuntimeError(f"Unrecognize date format: {date_spec}")
+
+
+def from_short_date_spec(short_date: str) -> dt.date:
     """Creates a date from a short zorg date of the form YYMMDD."""
     return dt.datetime.strptime(f"20{short_date}", _SHORT_DATE_FMT).date()
 
 
-def from_long_date(long_date: str) -> dt.date:
-    """Creates a date from a long zorg date of the form YYYY-MM-DD."""
-    return dt.datetime.strptime(long_date, _LONG_DATE_FMT).date()
+def is_short_date_spec(short_date: str) -> bool:
+    """Returns True iff {short_date} is a valid short date."""
+    return len(short_date) == 6 and all(ch.isdigit() for ch in short_date)
 
 
-def to_date(date_spec: str) -> dt.date:
-    """Converts some date string spec to an actual date."""
-    if is_short_date(date_spec):
-        return from_short_date(date_spec)
-    elif is_long_date(date_spec):
-        return from_long_date(date_spec)
-    else:
-        raise RuntimeError(f"Unrecognize date format: {date_spec}")
+def is_date_spec(date_spec: str) -> bool:
+    """Returns True iff {date_spec} is a valid zorg date."""
+    return is_short_date_spec(date_spec) or _is_long_date_spec(date_spec)
+
 
+def is_zid(zid: str) -> bool:
+    """Returns True iff {zid} is a valid ZID."""
+    return len(zid) == 9 and is_short_date_spec(zid[:6]) and zid[6] == "#"
 
-def to_short_date(date: dt.date) -> str:
+
+def to_short_date_spec(date: dt.date) -> str:
     """Creates a short zorg date of the form YYMMDD from a date."""
     return date.strftime(_SHORT_DATE_FMT)[2:]
 
 
-def is_short_date(short_date: str) -> bool:
-    """Returns True iff {short_date} is a valid short date."""
-    return len(short_date) == 6 and all(ch.isdigit() for ch in short_date)
+def _from_long_date_spec(long_date: str) -> dt.date:
+    """Creates a date from a long zorg date of the form YYYY-MM-DD."""
+    return dt.datetime.strptime(long_date, _LONG_DATE_FMT).date()
 
 
-def is_long_date(long_date: str) -> bool:
+def _is_long_date_spec(long_date: str) -> bool:
     """Returns True iff {long_date} is a valid long date."""
     return (
         len(long_date) == 10
         and {long_date[4], long_date[7]} == {"-"}
         and all(ch.isdigit() for ch in long_date.replace("-", ""))
     )
-
-
-def is_date(date_spec: str) -> bool:
-    """Returns True iff {date_spec} is a valid zorg date."""
-    return is_short_date(date_spec) or is_long_date(date_spec)
-
-
-def is_zid(zid: str) -> bool:
-    """Returns True iff {zid} is a valid ZID."""
-    return len(zid) == 9 and is_short_date(zid[:6]) and zid[6] == "#"
```

### Comparing `zettel_org-0.7.3/src/zorg/service/file_groups.py` & `zettel_org-0.7.4/src/zorg/service/file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/service/handlers.py` & `zettel_org-0.7.4/src/zorg/service/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,35 @@
 import sys
 from typing import Callable, Iterable, Iterator, Optional, Sequence
 
 from logrus import Logger
 from tqdm import tqdm
 import vimala
 
-from . import common as c, dates as zdt
+from . import common as c, dates as zdt, swog
 from .. import APP_NAME
 from ..domain.messages import commands, events
 from ..domain.models import File, Note
 from ..domain.types import Color
 from ..storage.sql.session import SQLSession
 from .compiler import walk_zorg_file
 from .zid_manager import ZIDManager
 
 
 _LOGGER = Logger(__name__)
 
-_ThingFirstLineAdder = Callable[[str, str], str]
-_ThingGetter = Callable[[Note], str]
+_AddThingToFirstLine = Callable[[str, str], str]
+_GetThing = Callable[[Note], str]
 
 
 def edit_files(cmd: commands.EditCommand, session: SQLSession) -> None:
     """Command handler for the EditCommand."""
+    for path in cmd.paths:
+        if path.suffix == ".zoq":
+            swog.refresh_zoq_file(session, path)
     vimala.vim(
         *cmd.paths,
         commands=_process_vim_commands(cmd.zettel_dir, cmd.vim_commands),
     ).unwrap()
     session.add_message(events.EditorClosedEvent(edit_cmd=cmd))
 
 
@@ -209,15 +212,15 @@
     del session
 
     _update_zo_file(
         zdir=event.zettel_dir,
         zo_path=event.zorg_file_path,
         notes_to_update=event.new_notes,
         add_thing_to_first_line=_add_zid_to_line,
-        thing_getter=attrgetter("zid"),
+        get_thing=attrgetter("zid"),
         log_message="Adding ZIDs to zorg file",
     )
 
 
 def increment_zid_counters(
     event: events.DBModifiedEvent, session: SQLSession
 ) -> None:
@@ -232,21 +235,21 @@
 
 
 def update_note_modify_dates(
     event: events.ModifiedZorgNotesEvent, session: SQLSession
 ) -> None:
     """Creates or updates note modify dates."""
     del session
-    today_short_date = zdt.to_short_date(dt.date.today())
+    today_short_date = zdt.to_short_date_spec(dt.date.today())
     _update_zo_file(
         zdir=event.zettel_dir,
         zo_path=event.zorg_file_path,
         notes_to_update=event.modified_notes,
         add_thing_to_first_line=_add_or_update_modify_date,
-        thing_getter=lambda _: today_short_date,
+        get_thing=lambda _: today_short_date,
         log_message="Updating modify dates",
     )
 
 
 def _get_zo_paths_to_index(zdir: Path) -> list[Path]:
     return sorted(zdir.rglob("*.zo"), key=lambda p: p.name)
 
@@ -293,20 +296,22 @@
 
     return f"{line_before_zid}{zid} {' '.join(words)}"
 
 
 def _hash_file(filepath: Path, chunk_size: int = 8192) -> str:
     """Hashes a file using SHA256 algorithm and returns the hash value.
 
-    Args:
-        filepath: Path to the file to be hashed.
-        chunk_size: Size of chunks to read the file. Default is 8192 bytes.
-
-    Returns:
-        A SHA256 hash of the file's contents.
+    Arguments:
+    ----------
+    filepath: Path to the file to be hashed.
+    chunk_size: Size of chunks to read the file. Default is 8192 bytes.
+
+    Return:
+    -------
+    A SHA256 hash of the file's contents.
     """
     hasher = hashlib.sha256()  # Initialize the hasher
     with filepath.open("rb") as file:
         while chunk := file.read(chunk_size):
             hasher.update(chunk)
     return hasher.hexdigest()
 
@@ -329,14 +334,17 @@
     notes = old_zorg_file.notes if old_zorg_file else []
     old_zid_map = {note.zid: note for note in notes if note.zid is not None}
     for note in zorg_file.notes:
         old_note = old_zid_map.get(note.zid, None) if note.zid else None
         note_has_changed = old_note and note != old_note
         note_is_new = old_note is None and note.zid is not None
         if note.modify_date != today and (note_has_changed or note_is_new):
+            note.modify_date = today
+            modify_short_date = zdt.to_short_date_spec(dt.date.today())
+            note.body = f"{modify_short_date} {note.body.lstrip()}"
             modified_notes.append(note)
     if modified_notes:
         zorg_file.events.append(
             events.ModifiedZorgNotesEvent(zdir, zorg_file.path, modified_notes)
         )
 
 
@@ -367,29 +375,29 @@
 
 
 def _update_zo_file(
     *,
     zdir: Path,
     zo_path: Path,
     notes_to_update: Sequence[Note],
-    add_thing_to_first_line: _ThingFirstLineAdder,
-    thing_getter: _ThingGetter,
+    add_thing_to_first_line: _AddThingToFirstLine,
+    get_thing: _GetThing,
     log_message: str,
 ) -> None:
     zlines = zo_path.read_text().split("\n")
     for note in notes_to_update:
         assert note.zid is not None
         assert note.line_no is not None
 
         start_idx = note.line_no - 1
         end_idx = note.line_no + len(note.body.split("\n")) - 1
         new_note_lines = zlines[start_idx:end_idx]
         first_note_line = new_note_lines[0]
         new_note_lines[0] = add_thing_to_first_line(
-            thing_getter(note), first_note_line
+            get_thing(note), first_note_line
         )
         zlines = zlines[:start_idx] + new_note_lines + zlines[end_idx:]
 
     _LOGGER.info(
         log_message,
         zorg_file=str(zo_path),
         notes_to_update=len(notes_to_update),
```

### Comparing `zettel_org-0.7.3/src/zorg/service/messagebus.py` & `zettel_org-0.7.4/src/zorg/service/messagebus.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/service/templates.py` & `zettel_org-0.7.4/src/zorg/service/templates.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/service/zid_manager.py` & `zettel_org-0.7.4/src/zorg/service/zid_manager.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/storage/sql/converters.py` & `zettel_org-0.7.4/src/zorg/storage/sql/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import operator
 from pathlib import Path
 from typing import Any, Callable, Optional, TypeVar, cast
 
 import metaman
 from sqlalchemy import func
 from sqlmodel import Integer, Session, and_, or_, select
-from sqlmodel.sql.expression import ColumnElement, SelectOfScalar
+from sqlmodel.sql.expression import Column, ColumnElement, SelectOfScalar
 
 from . import models as sql
 from ...domain.models import (
     File,
     Note,
     TodoPayload,
     WhereAndFilter,
@@ -46,19 +46,33 @@
 def to_select_of_note(
     or_filter: Optional[WhereOrFilter], session: Session
 ) -> SelectOfScalar[sql.ZorgNote]:
     """Converts a WhereOrFilter to a SQL SELECT that will fetch ZorgNotes."""
     if or_filter is None or not or_filter.and_filters:
         return select(sql.ZorgNote)
 
-    return select(sql.ZorgNote).where(
-        or_(*[
-            _SONConverter(and_filter, session).to_note_clause()
-            for and_filter in or_filter.and_filters
-        ])
+    return (
+        select(sql.ZorgNote)
+        .join(
+            sql.ZorgFileLink,
+            cast(ColumnElement, sql.ZorgNote.id == sql.ZorgFileLink.note_id),
+        )
+        .join(
+            sql.ZorgFile,
+            cast(
+                ColumnElement, sql.ZorgFileLink.zorg_file_id == sql.ZorgFile.id
+            ),
+        )
+        .where(
+            or_(*[
+                _SONConverter(and_filter, session).to_note_clause()
+                for and_filter in or_filter.and_filters
+            ])
+        )
+        .order_by(cast(Column, sql.ZorgNote.id))
     )
 
 
 @dataclass(frozen=True)
 class _SONConverter:
     """Converts a WhereAndFilter to a ColumnElement."""
 
@@ -207,15 +221,15 @@
             elif property_filter.op != PropertyOperator.EXISTS:
                 comp_op = comp_op_map[property_filter.op]
 
                 value_type_map: dict[
                     PropertyValueType,
                     tuple[Callable[[Any], Any], Callable[[Any], Any]],
                 ] = {
-                    PropertyValueType.DATE: (func.date, zdt.to_date),
+                    PropertyValueType.DATE: (func.date, zdt.from_date_spec),
                     PropertyValueType.INTEGER: (_col_to_int, int),
                     PropertyValueType.STRING: (_noop, _noop),
                 }
                 cast_model, cast_value = value_type_map[
                     property_filter.value_type
                 ]
                 subquery = subquery.where(
@@ -227,14 +241,15 @@
 
             and_conds.append(op(subquery))
 
         return and_(and_conds[0], *and_conds[1:])
 
     @_son_converter_parser
     def desc_filters(self) -> Optional[ColumnElement]:
+        """Converter tht handles desc filters."""
         and_conds = []
         if not self.and_filter.desc_filters:
             return None
 
         for desc_filter in self.and_filter.desc_filters:
             case_sensitive = desc_filter.case_sensitive
             if case_sensitive is None:
@@ -268,14 +283,29 @@
                 }
                 op = op_map[desc_filter.op]
                 op_arg = like_arg
 
             and_conds.append(op(op_arg))
         return and_(and_conds[0], *and_conds[1:])
 
+    @_son_converter_parser
+    def file_filters(self) -> Optional[ColumnElement]:
+        """Converter tht handles file filters."""
+        and_conds = []
+        if not self.and_filter.file_filters:
+            return None
+        for file_filter in self.and_filter.file_filters:
+            like_op = (
+                sql.ZorgFile.path.not_like  # type: ignore[attr-defined]
+                if file_filter.negated
+                else sql.ZorgFile.path.like  # type: ignore[attr-defined]
+            )
+            and_conds.append(like_op(file_filter.path_glob.replace("*", "%")))
+        return and_(and_conds[0], *and_conds[1:])
+
 
 def _noop(value: _T) -> _T:
     """A function that does nothing."""
     return value
 
 
 def _col_to_int(value: Any) -> Any:
@@ -291,15 +321,15 @@
 
 
 class ZorgFileConverter(EntityConverter[File, sql.ZorgFile]):
     """Converts File domain entities to/from ZorgFile sqlmodels."""
 
     def __init__(self, zdir: Path, session: Session) -> None:
         self._zdir = zdir
-        self._note_converter = ZorgNoteConverter(session)
+        self._note_converter = ZorgNoteConverter(zdir, session)
         self._all_sql_notes: list[sql.ZorgNote] = []
 
     def from_entity(self, entity: File) -> sql.ZorgFile:
         """Model-to-SQL-model converter for a ZorgFile."""
         sql_notes = []
         for note in entity.notes:
             sql_note = self._note_converter.from_entity(note)
@@ -322,16 +352,18 @@
             ],
         )
 
 
 class ZorgNoteConverter(EntityConverter[Note, sql.ZorgNote]):
     """Converts Note domain entities to/from ZorgNote sqlmodels."""
 
-    def __init__(self, session: Session) -> None:
+    def __init__(self, zdir: Path, session: Session) -> None:
+        self._zdir = zdir
         self._session = session
+
         self._tag_cache: dict[Any, dict[str, Any]] = defaultdict(lambda: {})
         self._property_cache: dict[str, sql.Property] = {}
 
     def from_entity(self, entity: Note) -> sql.ZorgNote:
         """Model-to-SQL-model converter for a ZorgNote."""
         # HACK: Needed to prevent errors of the form:
         #   SAWarning: Object of type <ZorgNote> not in session...
@@ -400,14 +432,26 @@
                 prop_link = sql.PropertyLink(
                     prop=prop, todo=sql_zorg_note, value=v
                 )
 
             property_links.append(prop_link)
 
         sql_zorg_note.property_links = property_links
+
+        # Convert 'zorg_file' field.
+        if entity.file_path is not None:
+            stripped_file_path = common.strip_zdir(
+                self._zdir, entity.file_path
+            )
+            stmt = select(sql.ZorgFile).where(
+                sql.ZorgFile.path == stripped_file_path
+            )
+            results = session.exec(stmt)
+            sql_zorg_note.zorg_file = results.first()
+
         return sql_zorg_note
 
     def to_entity(self, sql_model: sql.ZorgNote) -> Note:
         """Model-to-SQL-model converter for a Note."""
         todo_payload = (
             TodoPayload(
                 status=sql_model.todo_status,
```

### Comparing `zettel_org-0.7.3/src/zorg/storage/sql/engine.py` & `zettel_org-0.7.4/src/zorg/storage/sql/engine.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/storage/sql/models.py` & `zettel_org-0.7.4/src/zorg/storage/sql/models.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/src/zorg/storage/sql/repo.py` & `zettel_org-0.7.4/src/zorg/storage/sql/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def __init__(
         self, zettel_dir: Path, session: Session, *, verbose: int = 0
     ) -> None:
         self._zettel_dir = zettel_dir
         self._session = session
         self._converter = ZorgFileConverter(zettel_dir, session)
-        self._note_converter = ZorgNoteConverter(session)
+        self._note_converter = ZorgNoteConverter(zettel_dir, session)
         self._verbose = verbose
 
         self.seen: list[File] = []
 
     def add(self, zorg_file: File, /, *, key: str = None) -> ErisResult[str]:
         """Adds a new file to the DB.
 
@@ -136,14 +136,15 @@
     new_notes = []
     zid_manager = ZIDManager(zdir)
     for note in zorg_file.notes:
         if note.zid is None:
             _LOGGER.debug("Found new zorg note", zorg_note=note)
             zid = zid_manager.get_next(note.create_date)
             note.zid = zid
+            note.body = f"{zid} {note.body.lstrip()}"
             new_notes.append(note)
     if new_notes:
         zorg_file.events.append(
             NewZorgNotesEvent(
                 zdir, zorg_file_path=zorg_file.path, new_notes=new_notes
             )
         )
```

### Comparing `zettel_org-0.7.3/src/zorg/storage/sql/session.py` & `zettel_org-0.7.4/src/zorg/storage/sql/session.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/targets.mk` & `zettel_org-0.7.4/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/__snapshots__/test_run_action_open.ambr` & `zettel_org-0.7.4/tests/__snapshots__/test_run_action_open.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # serializer version: 1
 # name: test_action_open__bad[YAMLConfigFile-line_with_no_links]
   '''
-  ECHO We did not find anything zorg knows how to open on line #12
+  ECHO We did not find anything zorg knows how to open on line #10
   
   '''
 # ---
 # name: test_action_open__query[YAMLConfigFile-order_by_file_query]
   '''
-  # W (o or x or ~ or < or > or -) O priority modify G file | order_by_file
+  # W (o or x or ~ or < or > or -) O priority modify G file
   #
   # Saved query generated on 2000-01-03 at 12:00:00.
   
   ######### [[20240323]]
   - 240323#0J #gtd pomodoro
   - 240323#0K #own Buy rubber duck
   - 240323#0L +zorg Parametrize test_run_compile()
@@ -29,50 +29,50 @@
   - 240323#0a +laundry wip: fold darks
   - 240323#0b +laundry fold darks
   - 240323#0c +laundry wash delicates
   - 240323#0d +zorg [[xmind/zorg_e2e_query_arch.xmind]]
   
   
   ######### [[basic]]
-  o P2 240510#02 bazbuz is ok too...
   - 240510#00 First note in first block
   - 240510#01 Second note in first block
+  o P3 240510#02 bazbuz is ok too...
   
   
   ######### [[links]]
   - 240510#03 Some note with a [[bar.sh]] link to a bash script.
   - 240510#04 Some note with a link in parens (see [[baz]]).
   - 240510#05 Some note with a link in parens and a block-level link ([[buz::fuzz]]).
   - 240510#06 Some note that references an old 200101#12 ZID.
   
   
   ######### [[multiblocks]]
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
   - 240510#09 A note about life...
   - 240510#0B With a note
   - 240510#0C Some note in section 0
   - 240510#0D Note A1
   - 240510#0E Note A2
   - 240510#0F Note B
   - 240510#0G Note C
   - 240510#0H Note D
   - 240510#0J Note E
+  o P3 240510#07 Some todo
+  o P3 240510#08 Another related todo
+  o P3 240510#0A Some other todo
   
   
   ######### [[priority]]
   o P0 240313#03 High Priority TODO
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
   
   
   ######### [[property]]
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
   - 240330#02 This note contains a key::value pair.
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
   
   
   ######### [[scrambled_prj_notes]]
   - 240510#0L Sqtdicu Gfwebkj: fdxd://rd/czge-nxgz-vmuncaf
   - 240510#0M Reqzlu Zkba Inzlqq Zusqxur: pclx://hn/oqdu-syxf-oxzpzp-hxdszea
   - 240510#0N Tzus %clyzajrm: +cmeq ylevgv frxb gevcfp xa 26cb
   - 240510#0P Eongcgfy tho pscz giwq arjebc@?
@@ -138,45 +138,45 @@
   - 240510#1Y Ikr lr 20 pggmb
   - 240510#1Z Ttx-yecb mxovcuwbc
   - 240510#1a Rzq-itde mpfj
   - 240510#1b Zee-lpfg uqogce bk khxsvgrkq bbgvmf
   
   
   ######### [[subnotes]]
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
   - 240510#1c foobar
   - 240510#1e Todo subnote A
   - 240510#1f Todo subnote B
   - 240510#1h Todo subsubnote C
   - 240510#1k This note has many subnotes.
   - 240510#1m This note contains a key::value pair.
   - 240510#1n bazbuz
   - 240510#1o pig
   - 240510#1r is fat
   - 240510#1s is stinky
+  o P3 240510#1d This todo is due::2024-03-30 and has some subnotes
   
   
   ######### [[subsections]]
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
   - 240510#1t Note about A1
   - 240510#1u Note about something
   - 240510#1v Another note
   - 240510#1x A note on the second section.
   - 240510#1z A sub-note.
   - 240510#20 And another note.
   - 240510#22 This is inside of h4_section!
   - 240510#23 A note on the third section.
   - 240510#24 A sub-note.
   - 240510#25 And another note.
   - 240510#27 This is the final section!
+  o P3 240510#1w A todo for something
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
   
   
   ######### [[tags_and_ids]]
   - 240408#0X Some note
-  - 240408#NO Da nah nah nuh...
+  - 000103#00 240408#NO Da nah nah nuh...
   - 240509 240408#0X Some note with a modify date
   - 240510#29 Projects can start with a number, but CANNOT be all numbers
   - 301231#X0 When I talk to %pig I always want to @puke.
   '''
 # ---
```

### Comparing `zettel_org-0.7.3/tests/__snapshots__/test_run_compile.ambr` & `zettel_org-0.7.4/tests/__snapshots__/test_run_compile.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#02'}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-links]
   '''
@@ -299,27 +299,27 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#07'},
              {'areas': [],
               'body': ' 240510#08 Another related todo',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#08'},
              {'areas': [],
               'body': '240510#09 A note about life...',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
@@ -334,15 +334,15 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#0A'},
              {'areas': [],
               'body': '240510#0B With a note',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
@@ -491,15 +491,15 @@
               'contexts': ['due'],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {'due': '2024-03-13', 'p': '1'},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#0K'}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-scrambled_prj_notes]
   '''
@@ -1264,15 +1264,15 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {'due': '2024-03-30', 'p': '1'},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#1d'},
              {'areas': [],
               'body': '240510#1e Todo subnote A',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
@@ -1413,15 +1413,15 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#1w'},
              {'areas': [],
               'body': '240510#1x A note on the second section.',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
@@ -1458,15 +1458,15 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#21'},
              {'areas': [],
               'body': '240510#22 This is inside of h4_section!',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
@@ -1514,15 +1514,15 @@
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
               'modify_date': FakeDate(2024, 5, 10),
               'people': [],
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'P2',
+              'todo_payload': {'priority': 'P3',
                                'status': <NoteType.OPEN_TODO: 2>},
               'zid': '240510#26'},
              {'areas': [],
               'body': '240510#27 This is the final section!',
               'contexts': [],
               'create_date': FakeDate(2024, 5, 10),
               'links': [],
```

### Comparing `zettel_org-0.7.3/tests/__snapshots__/test_run_db.ambr` & `zettel_org-0.7.4/tests/__snapshots__/test_run_db.ambr`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
   12
 # ---
 # name: test_run_db_create__todo_priorities[YAMLConfigFile]
   list([
     'P0',
     'P1',
     'P2',
+    'P3',
   ])
 # ---
 # name: test_run_db_create__todo_statuses[YAMLConfigFile]
   list([
     'OPEN_TODO',
   ])
 # ---
```

### Comparing `zettel_org-0.7.3/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.7.4/tests/__snapshots__/test_run_edit.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/__snapshots__/test_run_query.ambr` & `zettel_org-0.7.4/tests/__snapshots__/test_run_query.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,58 @@
 # serializer version: 1
+# name: test_query[YAMLConfigFile-desc_filter]
+  '''
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
+  - 240510#1c foobar
+  
+  '''
+# ---
 # name: test_query[YAMLConfigFile-filter_by_create_and_modify]
   '''
   - 240509 240408#0X Some note with a modify date
   
   '''
 # ---
+# name: test_query[YAMLConfigFile-filter_by_property_eq]
+  '''
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
+  
+  '''
+# ---
+# name: test_query[YAMLConfigFile-filter_by_property_gt]
+  '''
+  - 240323#0U +zorg Test against all examples/ files
+  - 240323#0V +zorg wip: Replace 'john@' with '%john'
+  - 240323#0W +laundry dry whites
+  - 240323#0X +zorg wip: migrate people
+  - 240323#0Y +zorg Finished 'john@' to '%john' migration
+  - 240323#0Z +zorg Updated grammar to handle quotes
+  - 240323#0a +laundry wip: fold darks
+  - 240323#0b +laundry fold darks
+  - 240323#0c +laundry wash delicates
+  - 240323#0d +zorg [[xmind/zorg_e2e_query_arch.xmind]]
+  
+  '''
+# ---
 # name: test_query[YAMLConfigFile-group_by_context]
   '''
   o P0 240313#03 High Priority TODO
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
-  o P2 240510#02 bazbuz is ok too...
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
+  o P3 240510#02 bazbuz is ok too...
+  o P3 240510#07 Some todo
+  o P3 240510#08 Another related todo
+  o P3 240510#0A Some other todo
+  o P3 240510#1d This todo is due::2024-03-30 and has some subnotes
+  o P3 240510#1w A todo for something
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
   - 240330#02 This note contains a key::value pair.
-  - 240408#NO Da nah nah nuh...
+  - 000103#00 240408#NO Da nah nah nuh...
   - 240510#00 First note in first block
   - 240510#01 Second note in first block
   - 240510#03 Some note with a [[bar.sh]] link to a bash script.
   - 240510#04 Some note with a link in parens (see [[baz]]).
   - 240510#05 Some note with a link in parens and a block-level link ([[buz::fuzz]]).
   - 240510#06 Some note that references an old 200101#12 ZID.
   - 240510#09 A note about life...
@@ -122,15 +151,15 @@
   - 240510#24 A sub-note.
   - 240510#25 And another note.
   - 240510#27 This is the final section!
   - 240510#29 Projects can start with a number, but CANNOT be all numbers
   
   
   ######### @due
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
   
   
   ######### @dzwk
   - 240510#1R Git [[desd_cd_kdzb.yhdxx]] hgq lkl[1] @dzwk
   
   
   ######### @fat_pig
@@ -165,23 +194,23 @@
   '''
 # ---
 # name: test_query[YAMLConfigFile-group_by_people]
   '''
   o P0 240313#03 High Priority TODO
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
-  o P2 240510#02 bazbuz is ok too...
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
+  o P3 240510#02 bazbuz is ok too...
+  o P3 240510#07 Some todo
+  o P3 240510#08 Another related todo
+  o P3 240510#0A Some other todo
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
+  o P3 240510#1d This todo is due::2024-03-30 and has some subnotes
+  o P3 240510#1w A todo for something
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
   - 240323#0J #gtd pomodoro
   - 240323#0K #own Buy rubber duck
   - 240323#0L +zorg Parametrize test_run_compile()
   - 240323#0M +zorg Move models.py and file_groups.py
   - 240323#0N +zorg Add links to grammar
   - 240323#0P +zorg Fix grammar so it works with this file
   - 240323#0R +zorg Add this file to test data
@@ -193,15 +222,15 @@
   - 240323#0Y +zorg Finished 'john@' to '%john' migration
   - 240323#0Z +zorg Updated grammar to handle quotes
   - 240323#0a +laundry wip: fold darks
   - 240323#0b +laundry fold darks
   - 240323#0c +laundry wash delicates
   - 240323#0d +zorg [[xmind/zorg_e2e_query_arch.xmind]]
   - 240330#02 This note contains a key::value pair.
-  - 240408#NO Da nah nah nuh...
+  - 000103#00 240408#NO Da nah nah nuh...
   - 240408#0X Some note
   - 240509 240408#0X Some note with a modify date
   - 240510#00 First note in first block
   - 240510#01 Second note in first block
   - 240510#03 Some note with a [[bar.sh]] link to a bash script.
   - 240510#04 Some note with a link in parens (see [[baz]]).
   - 240510#05 Some note with a link in parens and a block-level link ([[buz::fuzz]]).
@@ -316,23 +345,23 @@
 # ---
 # name: test_query[YAMLConfigFile-group_by_type_area_project]
   '''
   ######### 1 | OPEN TODOS
   o P0 240313#03 High Priority TODO
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
-  o P2 240510#02 bazbuz is ok too...
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
+  o P3 240510#02 bazbuz is ok too...
+  o P3 240510#07 Some todo
+  o P3 240510#08 Another related todo
+  o P3 240510#0A Some other todo
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
+  o P3 240510#1d This todo is due::2024-03-30 and has some subnotes
+  o P3 240510#1w A todo for something
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
   
   
   ######### 4 | NOTES
   - 240330#02 This note contains a key::value pair.
   - 240510#00 First note in first block
   - 240510#01 Second note in first block
   - 240510#03 Some note with a [[bar.sh]] link to a bash script.
@@ -498,15 +527,15 @@
   - 240323#0K #own Buy rubber duck
   
   ======= #tags
   ***** +2_be_or_not_2_be | +bad
   - 240510#29 Projects can start with a number, but CANNOT be all numbers
   
   ***** +bad | +to_the_bone
-  - 240408#NO Da nah nah nuh...
+  - 000103#00 240408#NO Da nah nah nuh...
   
   ***** +foobar
   - 240408#0X Some note
   - 240509 240408#0X Some note with a modify date
   
   ======= #tags | #thoughts
   ***** +bazbuz | +foobar
@@ -534,50 +563,50 @@
   - 240323#0a +laundry wip: fold darks
   - 240323#0b +laundry fold darks
   - 240323#0c +laundry wash delicates
   - 240323#0d +zorg [[xmind/zorg_e2e_query_arch.xmind]]
   
   
   ######### [[basic]]
-  o P2 240510#02 bazbuz is ok too...
   - 240510#00 First note in first block
   - 240510#01 Second note in first block
+  o P3 240510#02 bazbuz is ok too...
   
   
   ######### [[links]]
   - 240510#03 Some note with a [[bar.sh]] link to a bash script.
   - 240510#04 Some note with a link in parens (see [[baz]]).
   - 240510#05 Some note with a link in parens and a block-level link ([[buz::fuzz]]).
   - 240510#06 Some note that references an old 200101#12 ZID.
   
   
   ######### [[multiblocks]]
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
   - 240510#09 A note about life...
   - 240510#0B With a note
   - 240510#0C Some note in section 0
   - 240510#0D Note A1
   - 240510#0E Note A2
   - 240510#0F Note B
   - 240510#0G Note C
   - 240510#0H Note D
   - 240510#0J Note E
+  o P3 240510#07 Some todo
+  o P3 240510#08 Another related todo
+  o P3 240510#0A Some other todo
   
   
   ######### [[priority]]
   o P0 240313#03 High Priority TODO
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
   
   
   ######### [[property]]
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
   - 240330#02 This note contains a key::value pair.
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
   
   
   ######### [[scrambled_prj_notes]]
   - 240510#0L Sqtdicu Gfwebkj: fdxd://rd/czge-nxgz-vmuncaf
   - 240510#0M Reqzlu Zkba Inzlqq Zusqxur: pclx://hn/oqdu-syxf-oxzpzp-hxdszea
   - 240510#0N Tzus %clyzajrm: +cmeq ylevgv frxb gevcfp xa 26cb
   - 240510#0P Eongcgfy tho pscz giwq arjebc@?
@@ -643,46 +672,46 @@
   - 240510#1Y Ikr lr 20 pggmb
   - 240510#1Z Ttx-yecb mxovcuwbc
   - 240510#1a Rzq-itde mpfj
   - 240510#1b Zee-lpfg uqogce bk khxsvgrkq bbgvmf
   
   
   ######### [[subnotes]]
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
   - 240510#1c foobar
   - 240510#1e Todo subnote A
   - 240510#1f Todo subnote B
   - 240510#1h Todo subsubnote C
   - 240510#1k This note has many subnotes.
   - 240510#1m This note contains a key::value pair.
   - 240510#1n bazbuz
   - 240510#1o pig
   - 240510#1r is fat
   - 240510#1s is stinky
+  o P3 240510#1d This todo is due::2024-03-30 and has some subnotes
   
   
   ######### [[subsections]]
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
   - 240510#1t Note about A1
   - 240510#1u Note about something
   - 240510#1v Another note
   - 240510#1x A note on the second section.
   - 240510#1z A sub-note.
   - 240510#20 And another note.
   - 240510#22 This is inside of h4_section!
   - 240510#23 A note on the third section.
   - 240510#24 A sub-note.
   - 240510#25 And another note.
   - 240510#27 This is the final section!
+  o P3 240510#1w A todo for something
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
   
   
   ######### [[tags_and_ids]]
-  - 240408#NO Da nah nah nuh...
+  - 000103#00 240408#NO Da nah nah nuh...
   - 240408#0X Some note
   - 240509 240408#0X Some note with a modify date
   - 240510#29 Projects can start with a number, but CANNOT be all numbers
   - 301231#X0 When I talk to %pig I always want to @puke.
   
   '''
 # ---
@@ -692,40 +721,76 @@
   
   '''
 # ---
 # name: test_query[YAMLConfigFile-mid_and_low_priority]
   '''
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
-  o P2 240510#02 bazbuz is ok too...
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
   
   '''
 # ---
 # name: test_query[YAMLConfigFile-open_todos]
   '''
   o P0 240313#03 High Priority TODO
   o P1 240313#04 Medium Priority TODO
   o P2 240313#05 Low Priority TODO
-  o P2 240510#02 bazbuz is ok too...
-  o P2 240510#07 Some todo
-  o P2 240510#08 Another related todo
-  o P2 240510#0A Some other todo
-  o P2 240510#0K This todo is @due today! | due::2024-03-13
-  o P2 240510#1d This todo is due::2024-03-30 and has some subnotes
-  o P2 240510#1w A todo for something
-  o P2 240510#21 Some foobar todo.
-  o P2 240510#26 Some foobar todo.
+  o P3 240510#02 bazbuz is ok too...
+  o P3 240510#07 Some todo
+  o P3 240510#08 Another related todo
+  o P3 240510#0A Some other todo
+  o P3 240510#0K This todo is @due today! | due::2024-03-13
+  o P3 240510#1d This todo is due::2024-03-30 and has some subnotes
+  o P3 240510#1w A todo for something
+  o P3 240510#21 Some foobar todo.
+  o P3 240510#26 Some foobar todo.
+  
+  '''
+# ---
+# name: test_query[YAMLConfigFile-select_files_with_todos]
+  '''
+  basic.zo
+  multiblocks.zo
+  priority.zo
+  property.zo
+  subnotes.zo
+  subsections.zo
+  
+  '''
+# ---
+# name: test_query[YAMLConfigFile-select_projects]
+  '''
+  2_be_or_not_2_be
+  arms
+  bad
+  bazbuz
+  bmlakcr
+  bqf
+  cmeq
+  cpv_mociy
+  fgifr
+  foobar
+  ipyt
+  judo
+  jws_pkaft
+  laundry
+  lozmhqjd
+  okwz
+  owwnfb
+  qbsum
+  rgw_sxtvx
+  saxy
+  to_the_bone
+  uahi
+  vd_clxi
+  vennc
+  vfntwi
+  wjybwa
+  xoao
+  zorg
+  zv_jzdd_djqa
   
   '''
 # ---
 # name: test_query[YAMLConfigFile-zorg_notes]
   '''
   ######### [[20240323]]
   - 240323#0L +zorg Parametrize test_run_compile()
```

### Comparing `zettel_org-0.7.3/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.7.4/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/common.py` & `zettel_org-0.7.4/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/conftest.py` & `zettel_org-0.7.4/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     assert ec == 0
     return query_zettel_dir
 
 
 def _get_zettel_dir(tmp_path: Path) -> Path:
     zdir = tmp_path / "org"
     zdir.mkdir()
-    for zo_path in _get_all_zo_and_zot_paths():
+    for zo_path in _get_all_zo_paths():
         zettel_zo_path = zdir / zo_path.name
         zettel_zo_path.write_bytes(zo_path.read_bytes())
     return zdir
 
 
 @fixture(scope="session", name="main")
 def main_fixture(make_config_file: MakeConfigFile) -> c.MainType:
@@ -84,16 +84,20 @@
 @fixture(autouse=True, scope="session")
 def frozen_time() -> Iterator[None]:
     """Freeze time until our tests are done running."""
     with freeze_time(f"{c.TODAY}T{c.hh}:{c.mm}:00.123456Z"):
         yield
 
 
-def _get_all_zo_and_zot_paths() -> list[Path]:
-    """Returns a list of Paths for all the *.zo files.
+def _get_all_zo_paths() -> list[Path]:
+    """Returns a list of Paths for all the *.zo[tq] files.
 
     These names will be relative to the zorg root directory.
     """
     zorg_root_dir = Path(__file__).parent.parent
     return list(
-        it.chain(zorg_root_dir.rglob("*.zo"), zorg_root_dir.rglob("*.zot"))
+        it.chain(
+            zorg_root_dir.rglob("*.zo"),
+            zorg_root_dir.rglob("*.zot"),
+            zorg_root_dir.rglob("*.zoq"),
+        )
     )
```

### Comparing `zettel_org-0.7.3/tests/data/day_log.zot` & `zettel_org-0.7.4/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/data/done_log.zot` & `zettel_org-0.7.4/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/data/habit_log.zot` & `zettel_org-0.7.4/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/test_config.py` & `zettel_org-0.7.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/test_file_groups.py` & `zettel_org-0.7.4/tests/test_file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/test_run_action_open.py` & `zettel_org-0.7.4/tests/test_run_action_open.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,69 +13,74 @@
 
 
 params = mark.parametrize
 
 
 @params(
     "lineno,zo_name",
-    [(7, "foo.zo"), (9, "bar.sh"), (10, "baz.zo")],
+    [(5, "foo.zo"), (7, "bar.sh"), (8, "baz.zo")],
 )
 def test_action_open__good(
     open_action_main: c.MainType,
     capsys: CaptureFixture,
     zettel_dir: Path,
     lineno: int,
     zo_name: str,
 ) -> None:
     """Test the 'action open' command's simple happy path."""
     open_action_main(str(lineno))
 
     capture = capsys.readouterr()
-    assert capture.err == ""
     assert capture.out == f"EDIT {zettel_dir}/{zo_name}\n"
 
 
-@params("lineno", [param(12, id="line_with_no_links")])
+@params("lineno", [param(10, id="line_with_no_links")])
 def test_action_open__bad(
     open_action_main: c.MainType,
     capsys: CaptureFixture,
     snapshot: Snapshot,
     lineno: int,
 ) -> None:
     """Test the 'action open' command's sad path."""
     open_action_main(str(lineno))
 
     capture = capsys.readouterr()
-    assert capture.err == ""
     assert capture.out == snapshot
 
 
 @params(
     "lineno,zo_name",
-    [param(5, "order_by_file.zoq", id="order_by_file_query")],
+    [param(1, "order_by_file.zoq", id="order_by_file_query")],
 )
 def test_action_open__query(
-    open_action_main: c.MainType,
+    main: c.MainType,
     capsys: CaptureFixture,
     snapshot: Snapshot,
     db_zettel_dir: Path,
     lineno: int,
     zo_name: str,
 ) -> None:
     """Test the 'action open' command with a SWOG query."""
-    open_action_main(str(lineno), zdir=db_zettel_dir)
+    query_zo_path = db_zettel_dir / zo_name
+    exit_code = main(
+        "--dir",
+        str(db_zettel_dir),
+        "action",
+        "open",
+        str(query_zo_path),
+        str(lineno),
+    )
+    assert exit_code == 0
 
     capture = capsys.readouterr()
-    query_zo_path = db_zettel_dir / zo_name
-    assert capture.err == ""
     assert capture.out == f"EDIT {query_zo_path}\n"
     assert query_zo_path.read_text() == snapshot
 
 
-@params("lineno,zo_name,link_prop", [param(11, "buz.zo", "fuzz")])
+@params("lineno,zo_name,link_prop", [param(9, "buz.zo", "fuzz")])
 def testActionOpen_withProperty_sendsSearchMsg(
     open_action_main: c.MainType,
     capsys: CaptureFixture,
     db_zettel_dir: Path,
     lineno: int,
     zo_name: str,
     link_prop: str,
@@ -86,29 +91,27 @@
     with a '::' separator. For example, a link of the form [[foo::bar]] should
     trigger the 'SEARCH bar' message.
     """
     open_action_main(str(lineno), zdir=db_zettel_dir)
 
     capture = capsys.readouterr()
     zo_path = db_zettel_dir / zo_name
-    assert capture.err == ""
     assert capture.out.strip().split("\n") == [
         f"EDIT {zo_path}",
         f"SEARCH id::{link_prop}",
     ]
 
 
 @fixture(name="open_action_main")
 def open_action_main_fixture(main: c.MainType, zettel_dir: Path) -> c.MainType:
     """Wrapper for main() fixture that is tailered to 'action open' tests."""
 
     def open_action_main(*args: str, zdir: Path = None, **kwargs: Any) -> int:
         zdir = zdir or zettel_dir
         exit_code = main(
-            "--log=null",
             "--dir",
             str(zdir),
             "action",
             "open",
             str(zdir / "links.zo"),
             *args,
             **kwargs,
```

### Comparing `zettel_org-0.7.3/tests/test_run_compile.py` & `zettel_org-0.7.4/tests/test_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/test_run_db.py` & `zettel_org-0.7.4/tests/test_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/test_run_edit.py` & `zettel_org-0.7.4/tests/test_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.3/tests/test_run_query.py` & `zettel_org-0.7.4/tests/test_run_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,19 @@
         param(
             "S note W (o or x or ~ or < or > or -) G type # +",
             id="group_by_type_area_project",
         ),
         param("(o or x or ~ or < or > or -) G @", id="group_by_context"),
         param("(o or x or ~ or < or > or -) G %", id="group_by_people"),
         param("^240408 $240509", id="filter_by_create_and_modify"),
+        param("due:2024-03-13", id="filter_by_property_eq"),
+        param("p:>5", id="filter_by_property_gt"),
+        param("'foo'", id="desc_filter"),
+        param("S +", id="select_projects"),
+        param("S file W o", id="select_files_with_todos"),
     ],
 )
 def test_query(
     main: c.MainType,
     capsys: CaptureFixture,
     snapshot: Snapshot,
     db_zettel_dir: Path,
```

### Comparing `zettel_org-0.7.3/tests/test_run_template.py` & `zettel_org-0.7.4/tests/test_run_template.py`

 * *Files identical despite different names*

