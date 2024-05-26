# Comparing `tmp/pycobertura-3.3.1.tar.gz` & `tmp/pycobertura-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycobertura-3.3.1.tar", last modified: Sat Feb 17 21:35:13 2024, max compression
+gzip compressed data, was "pycobertura-3.3.2.tar", last modified: Sun May 26 07:23:20 2024, max compression
```

## Comparing `pycobertura-3.3.1.tar` & `pycobertura-3.3.2.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.230203 pycobertura-3.3.1/
--rw-r--r--   0 alexandre   (501) staff       (20)       32 2024-02-17 00:58:35.000000 pycobertura-3.3.1/.coveragerc
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.207202 pycobertura-3.3.1/.github/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.211938 pycobertura-3.3.1/.github/workflows/
--rw-r--r--   0 alexandre   (501) staff       (20)      650 2024-02-17 00:58:35.000000 pycobertura-3.3.1/.github/workflows/build-and-test-pycobertura.yml
--rw-r--r--   0 alexandre   (501) staff       (20)      604 2024-02-17 00:58:35.000000 pycobertura-3.3.1/.gitignore
--rw-r--r--   0 alexandre   (501) staff       (20)    16523 2024-02-17 21:31:47.000000 pycobertura-3.3.1/CHANGES.md
--rw-r--r--   0 alexandre   (501) staff       (20)     1103 2024-02-17 00:58:35.000000 pycobertura-3.3.1/LICENSE
--rw-r--r--   0 alexandre   (501) staff       (20)    24565 2024-02-17 21:35:13.230126 pycobertura-3.3.1/PKG-INFO
--rw-r--r--   0 alexandre   (501) staff       (20)    23460 2024-02-17 00:58:35.000000 pycobertura-3.3.1/README.md
--rw-r--r--   0 alexandre   (501) staff       (20)        6 2024-02-17 21:31:14.000000 pycobertura-3.3.1/__version__
--rw-r--r--   0 alexandre   (501) staff       (20)     2697 2024-02-17 00:58:35.000000 pycobertura-3.3.1/aysha-logo.svg
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.213466 pycobertura-3.3.1/images/
--rw-r--r--   0 alexandre   (501) staff       (20)    30894 2024-02-17 00:58:35.000000 pycobertura-3.3.1/images/example_csv_diff_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)   172765 2024-02-17 00:58:35.000000 pycobertura-3.3.1/images/example_github_annotation_diff.png
--rw-r--r--   0 alexandre   (501) staff       (20)   103005 2024-02-17 00:58:35.000000 pycobertura-3.3.1/images/example_github_annotation_show.png
--rw-r--r--   0 alexandre   (501) staff       (20)    61287 2024-02-17 00:58:35.000000 pycobertura-3.3.1/images/example_json_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    53710 2024-02-17 00:58:35.000000 pycobertura-3.3.1/images/example_markdown_diff_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    45822 2024-02-17 00:58:35.000000 pycobertura-3.3.1/images/example_yaml_output.png
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.215008 pycobertura-3.3.1/pycobertura/
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      135 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/__main__.py
--rw-r--r--   0 alexandre   (501) staff       (20)     9607 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/cli.py
--rw-r--r--   0 alexandre   (501) staff       (20)    16490 2024-02-17 21:30:28.000000 pycobertura-3.3.1/pycobertura/cobertura.py
--rw-r--r--   0 alexandre   (501) staff       (20)     4944 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/filesystem.py
--rw-r--r--   0 alexandre   (501) staff       (20)    18010 2024-02-17 21:30:28.000000 pycobertura-3.3.1/pycobertura/reporters.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.217132 pycobertura-3.3.1/pycobertura/templates/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      624 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/filters.py
--rw-r--r--   0 alexandre   (501) staff       (20)     2805 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/html-delta.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)     1764 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/html.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)      473 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/macro.source.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)     7797 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/normalize.css
--rw-r--r--   0 alexandre   (501) staff       (20)    11452 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/templates/skeleton.css
--rw-r--r--   0 alexandre   (501) staff       (20)     7151 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pycobertura/utils.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.229805 pycobertura-3.3.1/pycobertura.egg-info/
--rw-r--r--   0 alexandre   (501) staff       (20)    24565 2024-02-17 21:35:13.000000 pycobertura-3.3.1/pycobertura.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (501) staff       (20)     3774 2024-02-17 21:35:13.000000 pycobertura-3.3.1/pycobertura.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (501) staff       (20)        1 2024-02-17 21:35:13.000000 pycobertura-3.3.1/pycobertura.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (501) staff       (20)       60 2024-02-17 21:35:13.000000 pycobertura-3.3.1/pycobertura.egg-info/entry_points.txt
--rw-r--r--   0 alexandre   (501) staff       (20)        1 2024-02-17 21:25:11.000000 pycobertura-3.3.1/pycobertura.egg-info/not-zip-safe
--rw-r--r--   0 alexandre   (501) staff       (20)       44 2024-02-17 21:35:13.000000 pycobertura-3.3.1/pycobertura.egg-info/requires.txt
--rw-r--r--   0 alexandre   (501) staff       (20)       12 2024-02-17 21:35:13.000000 pycobertura-3.3.1/pycobertura.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (501) staff       (20)      122 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pyproject.toml
--rw-r--r--   0 alexandre   (501) staff       (20)      997 2024-02-17 00:58:35.000000 pycobertura-3.3.1/pytest.ini
--rwxr-xr-x   0 alexandre   (501) staff       (20)      418 2024-02-17 21:35:06.000000 pycobertura-3.3.1/release.sh
--rw-r--r--   0 alexandre   (501) staff       (20)     1301 2024-02-17 21:35:13.230524 pycobertura-3.3.1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       38 2024-02-17 00:58:35.000000 pycobertura-3.3.1/setup.py
--rw-r--r--   0 alexandre   (501) staff       (20)       82 2024-02-17 00:58:35.000000 pycobertura-3.3.1/test-requirements.txt
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.222124 pycobertura-3.3.1/tests/
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/.testgitignore
--rw-r--r--   0 alexandre   (501) staff       (20)      748 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/README.generate-dummy-coverage-for-testing.md
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1162 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/cobertura-generated-by-istanbul-from-coffeescript.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      450 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/cobertura-no-branch-rate.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     7963 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/cobertura.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.222783 pycobertura-3.3.1/tests/dummy/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.229616 pycobertura-3.3.1/tests/dummy/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       41 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)      995 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/dummy-with-prefix.zip
--rw-r--r--   0 alexandre   (501) staff       (20)      687 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/dummy.zip
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      179 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.223122 pycobertura-3.3.1/tests/dummy.diffcoverage/
--rw-r--r--   0 alexandre   (501) staff       (20)     1181 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.diffcoverage/new-coverage.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1193 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.diffcoverage/old-coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.223425 pycobertura-3.3.1/tests/dummy.linestatus/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.223593 pycobertura-3.3.1/tests/dummy.linestatus/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)       14 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.linestatus/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      623 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.linestatus/test1.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      578 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.linestatus/test2.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.224068 pycobertura-3.3.1/tests/dummy.moved/
--rw-r--r--   0 alexandre   (501) staff       (20)     1604 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.224672 pycobertura-3.3.1/tests/dummy.moved/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/dummy/dummy5.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1037 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.moved/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)      861 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.original-better-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      852 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.original-full-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      858 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.original.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.225144 pycobertura-3.3.1/tests/dummy.source1/
--rw-r--r--   0 alexandre   (501) staff       (20)     1456 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.225663 pycobertura-3.3.1/tests/dummy.source1/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/dummy/dummy4.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source1/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.226082 pycobertura-3.3.1/tests/dummy.source2/
--rw-r--r--   0 alexandre   (501) staff       (20)     1423 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.226599 pycobertura-3.3.1/tests/dummy.source2/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       44 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)      209 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/dummy/dummy3.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      179 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.source2/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.227022 pycobertura-3.3.1/tests/dummy.uncovered/
--rw-r--r--   0 alexandre   (501) staff       (20)     1178 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.227949 pycobertura-3.3.1/tests/dummy.uncovered/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      114 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      178 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.227458 pycobertura-3.3.1/tests/dummy.uncovered.addcode/
--rw-r--r--   0 alexandre   (501) staff       (20)     1250 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered.addcode/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.227707 pycobertura-3.3.1/tests/dummy.uncovered.addcode/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered.addcode/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      185 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered.addcode/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered.addcode/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      178 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.uncovered.addcode/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1093 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.with-dummy2-better-and-worse.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1092 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.with-dummy2-better-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1080 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.with-dummy2-full-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1090 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.with-dummy2-no-cov.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.228361 pycobertura-3.3.1/tests/dummy.zeroexit1/
--rw-r--r--   0 alexandre   (501) staff       (20)      969 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit1/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.228593 pycobertura-3.3.1/tests/dummy.zeroexit1/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit1/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      108 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit1/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       58 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit1/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.229004 pycobertura-3.3.1/tests/dummy.zeroexit2/
--rw-r--r--   0 alexandre   (501) staff       (20)     1000 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit2/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2024-02-17 21:35:13.229244 pycobertura-3.3.1/tests/dummy.zeroexit2/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit2/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      134 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit2/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit2/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       68 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/dummy.zeroexit2/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)    32392 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_cli.py
--rw-r--r--   0 alexandre   (501) staff       (20)     9213 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_cobertura.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6435 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_cobertura_diff.py
--rw-r--r--   0 alexandre   (501) staff       (20)      127 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_colorize.py
--rw-r--r--   0 alexandre   (501) staff       (20)      429 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_extrapolate_coverage.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6853 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_filesystem.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6429 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_hunkify_coverage.py
--rw-r--r--   0 alexandre   (501) staff       (20)      187 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_imports.py
--rw-r--r--   0 alexandre   (501) staff       (20)      251 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_main.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1166 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_rangify.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1076 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_reconcile_lines.py
--rw-r--r--   0 alexandre   (501) staff       (20)      926 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_regex_utils.py
--rw-r--r--   0 alexandre   (501) staff       (20)    23766 2024-02-17 21:30:28.000000 pycobertura-3.3.1/tests/test_reporters.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1175 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/test_stringify.py
--rw-r--r--   0 alexandre   (501) staff       (20)      420 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tests/utils.py
--rw-r--r--   0 alexandre   (501) staff       (20)      551 2024-02-17 00:58:35.000000 pycobertura-3.3.1/tox.ini
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.309036 pycobertura-3.3.2/
+-rw-r--r--   0 alexandre   (502) staff       (20)       32 2024-05-26 06:05:52.000000 pycobertura-3.3.2/.coveragerc
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.274270 pycobertura-3.3.2/.github/
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.280195 pycobertura-3.3.2/.github/workflows/
+-rw-r--r--   0 alexandre   (502) staff       (20)      650 2024-05-26 06:05:52.000000 pycobertura-3.3.2/.github/workflows/build-and-test-pycobertura.yml
+-rw-r--r--   0 alexandre   (502) staff       (20)      604 2024-05-26 06:05:52.000000 pycobertura-3.3.2/.gitignore
+-rw-r--r--   0 alexandre   (502) staff       (20)    16617 2024-05-26 07:23:01.000000 pycobertura-3.3.2/CHANGES.md
+-rw-r--r--   0 alexandre   (502) staff       (20)     1103 2024-05-26 06:05:52.000000 pycobertura-3.3.2/LICENSE
+-rw-r--r--   0 alexandre   (502) staff       (20)    24565 2024-05-26 07:23:20.308854 pycobertura-3.3.2/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)    23460 2024-05-26 06:05:52.000000 pycobertura-3.3.2/README.md
+-rw-r--r--   0 alexandre   (502) staff       (20)        6 2024-05-26 07:23:01.000000 pycobertura-3.3.2/__version__
+-rw-r--r--   0 alexandre   (502) staff       (20)     2697 2024-05-26 06:05:52.000000 pycobertura-3.3.2/aysha-logo.svg
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.283366 pycobertura-3.3.2/images/
+-rw-r--r--   0 alexandre   (502) staff       (20)    30894 2024-05-26 06:05:52.000000 pycobertura-3.3.2/images/example_csv_diff_output.png
+-rw-r--r--   0 alexandre   (502) staff       (20)   172765 2024-05-26 06:05:52.000000 pycobertura-3.3.2/images/example_github_annotation_diff.png
+-rw-r--r--   0 alexandre   (502) staff       (20)   103005 2024-05-26 06:05:52.000000 pycobertura-3.3.2/images/example_github_annotation_show.png
+-rw-r--r--   0 alexandre   (502) staff       (20)    61287 2024-05-26 06:05:52.000000 pycobertura-3.3.2/images/example_json_output.png
+-rw-r--r--   0 alexandre   (502) staff       (20)    53710 2024-05-26 06:05:52.000000 pycobertura-3.3.2/images/example_markdown_diff_output.png
+-rw-r--r--   0 alexandre   (502) staff       (20)    45822 2024-05-26 06:05:52.000000 pycobertura-3.3.2/images/example_yaml_output.png
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.285558 pycobertura-3.3.2/pycobertura/
+-rw-r--r--   0 alexandre   (502) staff       (20)      119 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      135 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/__main__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     9607 2024-05-26 06:30:29.000000 pycobertura-3.3.2/pycobertura/cli.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    16825 2024-05-26 07:22:58.000000 pycobertura-3.3.2/pycobertura/cobertura.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     4944 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/filesystem.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    18010 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/reporters.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.288951 pycobertura-3.3.2/pycobertura/templates/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      624 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/filters.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     2805 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/html-delta.jinja2
+-rw-r--r--   0 alexandre   (502) staff       (20)     1764 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/html.jinja2
+-rw-r--r--   0 alexandre   (502) staff       (20)      473 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/macro.source.jinja2
+-rw-r--r--   0 alexandre   (502) staff       (20)     7797 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/normalize.css
+-rw-r--r--   0 alexandre   (502) staff       (20)    11452 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/templates/skeleton.css
+-rw-r--r--   0 alexandre   (502) staff       (20)     7151 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pycobertura/utils.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.308379 pycobertura-3.3.2/pycobertura.egg-info/
+-rw-r--r--   0 alexandre   (502) staff       (20)    24565 2024-05-26 07:23:20.000000 pycobertura-3.3.2/pycobertura.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (502) staff       (20)     3774 2024-05-26 07:23:20.000000 pycobertura-3.3.2/pycobertura.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        1 2024-05-26 07:23:20.000000 pycobertura-3.3.2/pycobertura.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       60 2024-05-26 07:23:20.000000 pycobertura-3.3.2/pycobertura.egg-info/entry_points.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)        1 2024-05-26 06:54:21.000000 pycobertura-3.3.2/pycobertura.egg-info/not-zip-safe
+-rw-r--r--   0 alexandre   (502) staff       (20)       44 2024-05-26 07:23:20.000000 pycobertura-3.3.2/pycobertura.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)       12 2024-05-26 07:23:20.000000 pycobertura-3.3.2/pycobertura.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (502) staff       (20)      122 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pyproject.toml
+-rw-r--r--   0 alexandre   (502) staff       (20)      997 2024-05-26 06:05:52.000000 pycobertura-3.3.2/pytest.ini
+-rwxr-xr-x   0 alexandre   (502) staff       (20)      415 2024-05-26 06:05:52.000000 pycobertura-3.3.2/release.sh
+-rw-r--r--   0 alexandre   (502) staff       (20)     1301 2024-05-26 07:23:20.309409 pycobertura-3.3.2/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)       38 2024-05-26 06:05:52.000000 pycobertura-3.3.2/setup.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       82 2024-05-26 06:05:52.000000 pycobertura-3.3.2/test-requirements.txt
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.296373 pycobertura-3.3.2/tests/
+-rw-r--r--   0 alexandre   (502) staff       (20)       64 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/.testgitignore
+-rw-r--r--   0 alexandre   (502) staff       (20)      748 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/README.generate-dummy-coverage-for-testing.md
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1162 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/cobertura-generated-by-istanbul-from-coffeescript.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)      450 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/cobertura-no-branch-rate.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)     7963 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/cobertura.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.297870 pycobertura-3.3.2/tests/dummy/
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.307987 pycobertura-3.3.2/tests/dummy/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       41 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       20 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      995 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/dummy-with-prefix.zip
+-rw-r--r--   0 alexandre   (502) staff       (20)      687 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/dummy.zip
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)      179 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy/test_dummy.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.298298 pycobertura-3.3.2/tests/dummy.diffcoverage/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1181 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.diffcoverage/new-coverage.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)     1193 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.diffcoverage/old-coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.298694 pycobertura-3.3.2/tests/dummy.linestatus/
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.298902 pycobertura-3.3.2/tests/dummy.linestatus/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)       14 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.linestatus/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      623 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.linestatus/test1.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)      578 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.linestatus/test2.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.299512 pycobertura-3.3.2/tests/dummy.moved/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1604 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.300168 pycobertura-3.3.2/tests/dummy.moved/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       56 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       20 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       64 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/dummy/dummy5.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1037 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)      119 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.moved/test_dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      861 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.original-better-cov.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)      852 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.original-full-cov.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)      858 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.original.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.300746 pycobertura-3.3.2/tests/dummy.source1/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1456 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.301470 pycobertura-3.3.2/tests/dummy.source1/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       56 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       20 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       64 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/dummy/dummy4.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)      119 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source1/test_dummy.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.302174 pycobertura-3.3.2/tests/dummy.source2/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1423 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.303124 pycobertura-3.3.2/tests/dummy.source2/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       56 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)       44 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      209 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/dummy/dummy3.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)      179 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.source2/test_dummy.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.303856 pycobertura-3.3.2/tests/dummy.uncovered/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1178 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.305285 pycobertura-3.3.2/tests/dummy.uncovered/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      114 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)      178 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered/test_dummy.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.304566 pycobertura-3.3.2/tests/dummy.uncovered.addcode/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1250 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered.addcode/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.304980 pycobertura-3.3.2/tests/dummy.uncovered.addcode/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered.addcode/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      185 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered.addcode/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered.addcode/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)      178 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.uncovered.addcode/test_dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1093 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.with-dummy2-better-and-worse.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)     1092 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.with-dummy2-better-cov.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)     1080 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.with-dummy2-full-cov.xml
+-rw-r--r--   0 alexandre   (502) staff       (20)     1090 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.with-dummy2-no-cov.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.305989 pycobertura-3.3.2/tests/dummy.zeroexit1/
+-rw-r--r--   0 alexandre   (502) staff       (20)      969 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit1/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.306371 pycobertura-3.3.2/tests/dummy.zeroexit1/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit1/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      108 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit1/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit1/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)       58 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit1/test_dummy.py
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.307094 pycobertura-3.3.2/tests/dummy.zeroexit2/
+-rw-r--r--   0 alexandre   (502) staff       (20)     1000 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit2/coverage.xml
+drwxr-xr-x   0 alexandre   (502) staff       (20)        0 2024-05-26 07:23:20.307418 pycobertura-3.3.2/tests/dummy.zeroexit2/dummy/
+-rw-r--r--   0 alexandre   (502) staff       (20)        0 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit2/dummy/__init__.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      134 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit2/dummy/dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1032 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit2/setup.cfg
+-rw-r--r--   0 alexandre   (502) staff       (20)       68 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/dummy.zeroexit2/test_dummy.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    32392 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_cli.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     9213 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_cobertura.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     6435 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_cobertura_diff.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      127 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_colorize.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      429 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_extrapolate_coverage.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     6853 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_filesystem.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     6429 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_hunkify_coverage.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      187 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_imports.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      251 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_main.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1166 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_rangify.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1076 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_reconcile_lines.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      926 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_regex_utils.py
+-rw-r--r--   0 alexandre   (502) staff       (20)    23766 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_reporters.py
+-rw-r--r--   0 alexandre   (502) staff       (20)     1175 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/test_stringify.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      420 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tests/utils.py
+-rw-r--r--   0 alexandre   (502) staff       (20)      551 2024-05-26 06:05:52.000000 pycobertura-3.3.2/tox.ini
```

### Comparing `pycobertura-3.3.1/.github/workflows/build-and-test-pycobertura.yml` & `pycobertura-3.3.2/.github/workflows/build-and-test-pycobertura.yml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/.gitignore` & `pycobertura-3.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/CHANGES.md` & `pycobertura-3.3.2/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Release Notes
 
 ## Unreleased
 
+## 3.3.2 (2024-05-26)
+* Improve error message as to why parsing the Cobertura report failed.
+
 ## 3.3.1 (2024-02-17)
 * Fix total stmts, miss and cover values in the coverage report when an ignore
   regex is passed. Thanks @danctorres
 
 ## 3.3.0 (2024-01-14)
 
 * Feat: Support executing pycobertura as a python module with: `python -m
```

### Comparing `pycobertura-3.3.1/LICENSE` & `pycobertura-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/PKG-INFO` & `pycobertura-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobertura
-Version: 3.3.1
+Version: 3.3.2
 Summary: "A Cobertura coverage parser that can diff reports and show coverage progress."
 Home-page: https://github.com/aconrad/pycobertura
 Author: "Alex Conrad"
 Author-email: "alexandre.conrad@gmail.com"
 Maintainer: "Alex Conrad"
 Maintainer-email: "alexandre.conrad@gmail.com"
 Keywords: "cobertura coverage diff report parser parse xml"
@@ -634,15 +634,15 @@
 The line rate decreased from 80% to 75% but uncovered lines is still at 1. In
 this case, failing the build based on line rate is inappropriate, thus making
 the line rate the wrong metric to look at when validating coverage.
 
 The basic idea is that a code base may have technical debt of N uncovered lines
 and you want to prevent N from ever going up.
 
-### pycobertura sounds cool, but how to I generate a Cobertura file?
+### pycobertura sounds cool, but how do I generate a Cobertura file?
 
 Depending on your programing language, you need to find a tool that measures
 code coverage and generates a Cobertura report which is an XML representation
 of your code coverage results.
 
 In Python, [coverage.py](http://nedbatchelder.com/code/coverage/) is a great
 tool for measuring code coverage and plugins such as
```

### Comparing `pycobertura-3.3.1/README.md` & `pycobertura-3.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
 The line rate decreased from 80% to 75% but uncovered lines is still at 1. In
 this case, failing the build based on line rate is inappropriate, thus making
 the line rate the wrong metric to look at when validating coverage.
 
 The basic idea is that a code base may have technical debt of N uncovered lines
 and you want to prevent N from ever going up.
 
-### pycobertura sounds cool, but how to I generate a Cobertura file?
+### pycobertura sounds cool, but how do I generate a Cobertura file?
 
 Depending on your programing language, you need to find a tool that measures
 code coverage and generates a Cobertura report which is an XML representation
 of your code coverage results.
 
 In Python, [coverage.py](http://nedbatchelder.com/code/coverage/) is a great
 tool for measuring code coverage and plugins such as
```

### Comparing `pycobertura-3.3.1/aysha-logo.svg` & `pycobertura-3.3.2/aysha-logo.svg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/images/example_csv_diff_output.png` & `pycobertura-3.3.2/images/example_csv_diff_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/images/example_github_annotation_diff.png` & `pycobertura-3.3.2/images/example_github_annotation_diff.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/images/example_github_annotation_show.png` & `pycobertura-3.3.2/images/example_github_annotation_show.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/images/example_json_output.png` & `pycobertura-3.3.2/images/example_json_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/images/example_markdown_diff_output.png` & `pycobertura-3.3.2/images/example_markdown_diff_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/images/example_yaml_output.png` & `pycobertura-3.3.2/images/example_yaml_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/cli.py` & `pycobertura-3.3.2/pycobertura/cli.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/cobertura.py` & `pycobertura-3.3.2/pycobertura/cobertura.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,25 +50,35 @@
             - a file path
             - an XML string
 
         The optional keyword argument `filesystem` describes how to retrieve the
         source files referenced in the report. Please check the
         `pycobertura.filesystem` module to learn more about filesystems.
         """
+        errors = []
         for load_func in [
             self._load_from_file,
             self._load_from_string,
         ]:
             try:
                 self.xml = load_func(report)
                 break
-            except BaseException:
+            except BaseException as e:
+                errors.append(e)
                 pass
         else:
-            raise self.InvalidCoverageReport("Invalid coverage file: {}".format(report))
+            raise self.InvalidCoverageReport(
+                """\
+Invalid coverage report: {}.
+The following exceptions occurred while attempting to parse the report:
+* While treating the report as a filename: {}.
+* While treating the report as an XML Cobertura string: {}""".format(
+                    report, errors[0], errors[1]
+                )
+            )
 
         self.filesystem = filesystem
         self.report = report
 
         self._class_elements_by_file_name = self._make_class_elements_by_filename()
 
     def _make_class_elements_by_filename(self):
```

### Comparing `pycobertura-3.3.1/pycobertura/filesystem.py` & `pycobertura-3.3.2/pycobertura/filesystem.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/reporters.py` & `pycobertura-3.3.2/pycobertura/reporters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/templates/filters.py` & `pycobertura-3.3.2/pycobertura/templates/filters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/templates/html-delta.jinja2` & `pycobertura-3.3.2/pycobertura/templates/html-delta.jinja2`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/templates/html.jinja2` & `pycobertura-3.3.2/pycobertura/templates/html.jinja2`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/templates/normalize.css` & `pycobertura-3.3.2/pycobertura/templates/normalize.css`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/templates/skeleton.css` & `pycobertura-3.3.2/pycobertura/templates/skeleton.css`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura/utils.py` & `pycobertura-3.3.2/pycobertura/utils.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pycobertura.egg-info/PKG-INFO` & `pycobertura-3.3.2/pycobertura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobertura
-Version: 3.3.1
+Version: 3.3.2
 Summary: "A Cobertura coverage parser that can diff reports and show coverage progress."
 Home-page: https://github.com/aconrad/pycobertura
 Author: "Alex Conrad"
 Author-email: "alexandre.conrad@gmail.com"
 Maintainer: "Alex Conrad"
 Maintainer-email: "alexandre.conrad@gmail.com"
 Keywords: "cobertura coverage diff report parser parse xml"
@@ -634,15 +634,15 @@
 The line rate decreased from 80% to 75% but uncovered lines is still at 1. In
 this case, failing the build based on line rate is inappropriate, thus making
 the line rate the wrong metric to look at when validating coverage.
 
 The basic idea is that a code base may have technical debt of N uncovered lines
 and you want to prevent N from ever going up.
 
-### pycobertura sounds cool, but how to I generate a Cobertura file?
+### pycobertura sounds cool, but how do I generate a Cobertura file?
 
 Depending on your programing language, you need to find a tool that measures
 code coverage and generates a Cobertura report which is an XML representation
 of your code coverage results.
 
 In Python, [coverage.py](http://nedbatchelder.com/code/coverage/) is a great
 tool for measuring code coverage and plugins such as
```

### Comparing `pycobertura-3.3.1/pycobertura.egg-info/SOURCES.txt` & `pycobertura-3.3.2/pycobertura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/pytest.ini` & `pycobertura-3.3.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/setup.cfg` & `pycobertura-3.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/README.generate-dummy-coverage-for-testing.md` & `pycobertura-3.3.2/tests/README.generate-dummy-coverage-for-testing.md`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/cobertura-generated-by-istanbul-from-coffeescript.xml` & `pycobertura-3.3.2/tests/cobertura-generated-by-istanbul-from-coffeescript.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/cobertura.xml` & `pycobertura-3.3.2/tests/cobertura.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy/dummy-with-prefix.zip` & `pycobertura-3.3.2/tests/dummy/dummy-with-prefix.zip`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy/dummy.zip` & `pycobertura-3.3.2/tests/dummy/dummy.zip`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy/setup.cfg` & `pycobertura-3.3.2/tests/dummy/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.diffcoverage/new-coverage.xml` & `pycobertura-3.3.2/tests/dummy.diffcoverage/new-coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.diffcoverage/old-coverage.xml` & `pycobertura-3.3.2/tests/dummy.diffcoverage/old-coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.linestatus/test1.xml` & `pycobertura-3.3.2/tests/dummy.linestatus/test1.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.linestatus/test2.xml` & `pycobertura-3.3.2/tests/dummy.linestatus/test2.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.moved/coverage.xml` & `pycobertura-3.3.2/tests/dummy.moved/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.moved/setup.cfg` & `pycobertura-3.3.2/tests/dummy.moved/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.original-better-cov.xml` & `pycobertura-3.3.2/tests/dummy.original-better-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.original-full-cov.xml` & `pycobertura-3.3.2/tests/dummy.original-full-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.original.xml` & `pycobertura-3.3.2/tests/dummy.original.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.source1/coverage.xml` & `pycobertura-3.3.2/tests/dummy.source1/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.source1/setup.cfg` & `pycobertura-3.3.2/tests/dummy.source1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.source2/coverage.xml` & `pycobertura-3.3.2/tests/dummy.source2/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.source2/setup.cfg` & `pycobertura-3.3.2/tests/dummy.source2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.uncovered/coverage.xml` & `pycobertura-3.3.2/tests/dummy.uncovered/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.uncovered/setup.cfg` & `pycobertura-3.3.2/tests/dummy.uncovered/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.uncovered.addcode/coverage.xml` & `pycobertura-3.3.2/tests/dummy.uncovered.addcode/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.uncovered.addcode/setup.cfg` & `pycobertura-3.3.2/tests/dummy.uncovered.addcode/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.with-dummy2-better-and-worse.xml` & `pycobertura-3.3.2/tests/dummy.with-dummy2-better-and-worse.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.with-dummy2-better-cov.xml` & `pycobertura-3.3.2/tests/dummy.with-dummy2-better-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.with-dummy2-full-cov.xml` & `pycobertura-3.3.2/tests/dummy.with-dummy2-full-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.with-dummy2-no-cov.xml` & `pycobertura-3.3.2/tests/dummy.with-dummy2-no-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.zeroexit1/coverage.xml` & `pycobertura-3.3.2/tests/dummy.zeroexit1/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.zeroexit1/setup.cfg` & `pycobertura-3.3.2/tests/dummy.zeroexit1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.zeroexit2/coverage.xml` & `pycobertura-3.3.2/tests/dummy.zeroexit2/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/dummy.zeroexit2/setup.cfg` & `pycobertura-3.3.2/tests/dummy.zeroexit2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_cli.py` & `pycobertura-3.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_cobertura.py` & `pycobertura-3.3.2/tests/test_cobertura.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_cobertura_diff.py` & `pycobertura-3.3.2/tests/test_cobertura_diff.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_filesystem.py` & `pycobertura-3.3.2/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_hunkify_coverage.py` & `pycobertura-3.3.2/tests/test_hunkify_coverage.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_rangify.py` & `pycobertura-3.3.2/tests/test_rangify.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_reconcile_lines.py` & `pycobertura-3.3.2/tests/test_reconcile_lines.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_regex_utils.py` & `pycobertura-3.3.2/tests/test_regex_utils.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_reporters.py` & `pycobertura-3.3.2/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tests/test_stringify.py` & `pycobertura-3.3.2/tests/test_stringify.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.3.1/tox.ini` & `pycobertura-3.3.2/tox.ini`

 * *Files identical despite different names*

