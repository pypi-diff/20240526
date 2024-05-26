# Comparing `tmp/irispie-0.8.1.tar.gz` & `tmp/irispie-0.9.0.tar.gz`

## Comparing `irispie-0.8.1.tar` & `irispie-0.9.0.tar`

### file list

```diff
@@ -1,105 +1,108 @@
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 irispie-0.8.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 irispie-0.8.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/.obsidian/app.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/.obsidian/appearance.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/.obsidian/workspace.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/architecture/Untitled.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/architecture/steady.canvas
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.8.1/docs/series/example.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/__init__.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/dataslabs.py
--rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/dates.py
--rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/exceptions.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/quantities.py
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/sources.py
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/transforms.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13365 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/conveniences/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/conveniences/copies.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/conveniences/descriptions.py
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/conveniences/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/databanks/__init__.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/databanks/_exports.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/databanks/_imports.py
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/databanks/_imports2.py
--rw-r--r--   0        0        0    12723 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/databanks/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/equators/steady.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/evaluators/__init__.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/default.spc~
--rw-r--r--   0        0        0   272964 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/libgcc_s.1.dylib
--rw-r--r--   0        0        0  1572232 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/libgfortran.3.dylib
--rw-r--r--   0        0        0   282056 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/libquadmath.0.dylib
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/template.spc
--rw-r--r--   0        0        0  2580776 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/x12awin.exe
--rwxr-xr-x   0        0        0  4041944 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/x13asmac
--rwxr-xr-x   0        0        0  4423264 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/x13asunix
--rw-r--r--   0        0        0  3661312 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/executables/x13aswin.exe
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/explanatories/__init__.py
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/explanatories/main.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    16760 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9306 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/incidences/blazer.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/incidences/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/jacobians/__init__.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/jacobians/_base.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/_flags.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/_get.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/_simulate.py
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/_steady.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/invariants.py
--rw-r--r--   0        0        0    11745 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/main.py
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/algebraic.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/plans/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/plans/main.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/sequentials/__init__.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/sequentials/_simulate.py
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/sequentials/main.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/series/__init__.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/series/_conversion.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/series/_hp.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/series/_plotly.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/series/_x13.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 irispie-0.8.1/src/irispie/series/main.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.8.1/tests/.gitkeep
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 irispie-0.8.1/tests/dataman/dates/frequency_letters.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 irispie-0.8.1/tests/dataman/dates/sdmx_dates.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 irispie-0.8.1/tests/series/hpf_test.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 irispie-0.8.1/tests/series/shift_test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.8.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.8.1/LICENCE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.8.1/README.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 irispie-0.9.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 irispie-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/.obsidian/app.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/.obsidian/appearance.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/.obsidian/hotkeys.json
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/.obsidian/workspace.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/architecture/Untitled.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/architecture/steady.canvas
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.9.0/docs/series/example.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/__init__.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/dataslabs.py
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/dates.py
+-rw-r--r--   0        0        0     8889 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/namings.py
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/quantities.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/sources.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/transforms.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/conveniences/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/conveniences/copies.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/conveniences/descriptions.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/conveniences/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/databanks/__init__.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/databanks/_exports.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/databanks/_imports.py
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/databanks/_imports2.py
+-rw-r--r--   0        0        0    11921 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/databanks/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/evaluators/__init__.py
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0    10513 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/default.spc~
+-rw-r--r--   0        0        0   272964 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/libgcc_s.1.dylib
+-rw-r--r--   0        0        0  1572232 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/libgfortran.3.dylib
+-rw-r--r--   0        0        0   282056 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/libquadmath.0.dylib
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/template.spc
+-rw-r--r--   0        0        0  2580776 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/x12awin.exe
+-rwxr-xr-x   0        0        0  4041944 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/x13asmac
+-rwxr-xr-x   0        0        0  4423264 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/x13asunix
+-rw-r--r--   0        0        0  3661312 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/executables/x13aswin.exe
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/explanatories/__init__.py
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/explanatories/main.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/covariances.py
+-rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0    13556 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/incidences/blazer.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/incidences/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/jacobians/__init__.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/jacobians/_base.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/_covariances.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/_flags.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/_get.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/_simulate.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/_steady.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/main.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/algebraic.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/plans/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/plans/main.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/sequentials/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/sequentials/_simulate.py
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/sequentials/main.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/series/__init__.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/series/_conversion.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/series/_hp.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/series/_plotly.py
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/series/_x13.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 irispie-0.9.0/src/irispie/series/main.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.9.0/tests/.gitkeep
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 irispie-0.9.0/tests/dataman/dates/frequency_letters.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 irispie-0.9.0/tests/dataman/dates/sdmx_dates.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 irispie-0.9.0/tests/series/hpf_test.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 irispie-0.9.0/tests/series/shift_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.9.0/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.9.0/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.9.0/PKG-INFO
```

### Comparing `irispie-0.8.1/.github/workflows/publish-to-pypi.yml` & `irispie-0.9.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/docs/.obsidian/core-plugins-migration.json` & `irispie-0.9.0/docs/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/docs/.obsidian/workspace.json` & `irispie-0.9.0/docs/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/docs/algorithms/detach-unit-roots.md` & `irispie-0.9.0/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/docs/milestones/March-2023.md` & `irispie-0.9.0/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/docs/milestones/iris-gray.png` & `irispie-0.9.0/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/docs/series/example.py` & `irispie-0.9.0/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/__init__.py` & `irispie-0.9.0/src/irispie/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,20 +28,24 @@
 
 from .explanatories import *
 from .explanatories import __all__ as explanatories_all
 
 from .plans.main import *
 from .plans.main import __all__ as plans_all
 
+from .namings import *
+from .namings import __all__ as namings_all
+
 
 __all__ = (
     *dates_all,
     *series_all,
     *databanks_all,
     *models_all,
     *quantities_all,
     *equations_all,
     *sequentials_all,
     *explanatories_all,
     *plans_all,
+    *namings_all,
 )
```

### Comparing `irispie-0.8.1/src/irispie/dataslabs.py` & `irispie-0.9.0/src/irispie/dataslabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,20 @@
 
     @property
     def num_ext_periods(self, /, ) -> int:
         """
         """
         return len(self.column_dates)
 
+    @property
+    def num_rows(self, /, ) -> int:
+        """
+        """
+        return self.data.shape[0] if self.data is not None else 0
+
     def remove_terminal(self, /, ) -> None:
         """
         """
         last_base_column = self.base_columns[-1]
         self.data = self.data[:, :last_base_column+1]
         self.column_dates = self.column_dates[:last_base_column+1]
```

### Comparing `irispie-0.8.1/src/irispie/dates.py` & `irispie-0.9.0/src/irispie/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         """
         t = _dt.date.today()
         return DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_ymd(t.year, t.month, t.day, )
 
     def to_iso_string(
         self,
         /,
-        position: Literal["start"] | Literal["middle"] | Literal["end"] = "start",
+        position: Literal["start", "middle", "end", ] = "start",
     ) -> str:
         year, month, day = self.to_ymd(position=position, )
         return f"{year:04g}-{month:02g}-{day:02g}"
 
     to_plotly_date = _ft.partialmethod(to_iso_string, position="middle")
 
     def __init__(self, serial=0) -> None:
@@ -437,15 +437,15 @@
 
     def get_year(self) -> int:
         return self.to_year_period()[0]
 
     def to_ymd(
         self, 
         /,
-        position: Literal["start"] | Literal["middle"] | Literal["end"] = "middle",
+        position: Literal["start", "middle", "end", ] = "middle",
     ) -> tuple[int, int, int]:
         year, per = self.to_year_period()
         return year, *self.month_day_resolution[position][per]
 
     def __str__(self) -> str:
         year, per = self.to_year_period()
         letter = self.frequency.letter
@@ -468,15 +468,15 @@
     def create_tty(self, ) -> Self:
         year, per = self.to_year_period()
         return self.from_year_period(year, 1) if per != 1 else None
 
     def to_daily(
         self,
         /,
-        position: Literal["start"] | Literal["middle"] | Literal["end"] = "middle"
+        position: Literal["start", "middle", "end", ] = "middle"
     ) -> DailyDater:
         try:
             return DailyDater.from_ymd(*self.to_ymd(position=position, ), )
         except:
             from IPython import embed; embed()
     #]
 
@@ -530,26 +530,26 @@
 
     @_remove_blanks
     def __repr__(self) -> str: return f"hh{self.to_year_period()}"
 
     def to_ymd(
         self, 
         /,
-        position: Literal["start"] | Literal["middle"] | Literal["end"] = "middle",
+        position: Literal["start", "middle", "end", ] = "middle",
     ) -> tuple[int, int, int]:
         year, per = self.to_year_period()
         return (
             year,
             *{"start": (1, 1), "middle": (6, 3), "end": (12, 31)}[position],
         )
 
     def get_month(
         self,
         /,
-        position: Literal["start"] | Literal["middle"] | Literal["end"] = "middle",
+        position: Literal["start", "middle", "end", ] = "middle",
     ) -> int:
         _, per = self.to_year_period()
         return month_resolution[position][per]
 
     @staticmethod
     def month_to_period(month: int, ) -> int:
         return 1+((month-1)//6)
@@ -671,15 +671,15 @@
         return self._step
 
     @property
     def _class(self):
         return type(self._start_date) if not self.needs_resolve else None
 
     @property
-    def direction(self, ) -> Literal["forward"] | Literal["backward"]:
+    def direction(self, ) -> Literal["forward", "backward", ]:
         return "forward" if self._step > 0 else "backward"
 
     @property
     def _serials(self) -> range | None:
         return range(self._start_date.serial, self._end_date.serial+_sign(self._step), self._step) if not self.needs_resolve else None
 
     # @property
```

### Comparing `irispie-0.8.1/src/irispie/equations.py` & `irispie-0.9.0/src/irispie/equations.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     #[
     error_log = tuple(_it.chain.from_iterable(
         eqn.finalize(name_to_id)
         for eqn in equations
     ))
     if error_log:
         raise _wrongdoings.IrisPieError(
-            ["Some names used in equations not declared"]
+            ("Some names used in equations are not declared", )
             + error_log
         )
     #]
 
 
 def generate_names_from_human(human: str) -> Iterable[str]:
     """
```

### Comparing `irispie-0.8.1/src/irispie/exceptions.py` & `irispie-0.9.0/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/quantities.py` & `irispie-0.9.0/src/irispie/quantities.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,20 +172,20 @@
     return custom_quantities, invalid_names
 
 
 def lookup_qids_by_name(
     quantities: Iterable[Quantity],
     custom_names: Iterable[str],
     /,
-) -> tuple[tuple[int], tuple[str]]:
+) -> tuple[tuple[int, ...], tuple[str, ...]]:
     """
     Lookup quantities by name, and return a list of quantities and a list
     of invalid names
     """
-    custom_names = list(custom_names)
+    custom_names = tuple(custom_names)
     name_to_qid  = create_name_to_qid(quantities)
     custom_qids = tuple(
         name_to_qid[n]
         for n in custom_names if n in name_to_qid
     )
     invalid_names = tuple(
         n for n in custom_names if n not in name_to_qid
```

### Comparing `irispie-0.8.1/src/irispie/sources.py` & `irispie-0.9.0/src/irispie/sources.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,32 +71,38 @@
 
 class AlgebraicSource:
     """
     """
     #[
     __slots__ = (
         "quantities", "dynamic_equations", "steady_equations",
-        "log_variables", "all_but", "context", "sealed",
+        "log_variables", "all_but", "context", "shock_qid_to_std_qid",
+        "sealed",
     )
     def __init__(self, /) -> None:
         self.quantities = []
         self.dynamic_equations = []
         self.steady_equations = []
         self.log_variables = []
         self.all_but = []
         self.context = None
         self.sealed = False
+        self.shock_qid_to_std_qid = None
 
     def seal(self, /) -> None:
         _check_unique_names(qty.human for qty in self.quantities)
-        self._add_stds()
         self.quantities = _reorder_by_kind(self.quantities)
         self.dynamic_equations = _reorder_by_kind(self.dynamic_equations)
         self.steady_equations = _reorder_by_kind(self.steady_equations)
         self.quantities = _stamp_id(self.quantities)
+        #
+        self.shock_qid_to_std_qid = {}
+        self._add_stds(_quantities.QuantityKind.TRANSITION_SHOCK, _quantities.QuantityKind.TRANSITION_STD, )
+        self._add_stds(_quantities.QuantityKind.MEASUREMENT_SHOCK, _quantities.QuantityKind.MEASUREMENT_STD, )
+        #
         self.dynamic_equations = _stamp_id(self.dynamic_equations)
         self.steady_equations = _stamp_id(self.steady_equations)
         self._populate_logly()
         self.sealed = True
 
     @property
     def num_quantities(self, /) -> int:
@@ -158,32 +164,14 @@
             for i, ein in enumerate(equation_inputs, start=offset)
         ]
         self.steady_equations = self.steady_equations + [
             _equations.Equation(id=None, human=_handle_white_spaces(ein[1][1] if ein[1][1] else ein[1][0]), kind=kind, description=ein[0].strip(), entry=i)
             for i, ein in enumerate(equation_inputs, start=offset)
         ]
 
-    def _add_stds(self) -> None:
-        """
-        """
-        def _create_std_input_from_shock(shock):
-            description = _STD_DESCRIPTION + (shock.description if shock.description else shock.human)
-            human = STD_PREFIX + shock.human
-            return(description, human)
-        #
-        transition_shocks = (q for q in self.quantities if q.kind in _quantities.QuantityKind.TRANSITION_SHOCK)
-        if transition_shocks:
-            transition_std_inputs = (_create_std_input_from_shock(i) for i in transition_shocks)
-            self._add_quantities(transition_std_inputs, _quantities.QuantityKind.TRANSITION_STD)
-        #
-        measurement_shocks = (q for q in self.quantities if q.kind in _quantities.QuantityKind.MEASUREMENT_SHOCK)
-        if measurement_shocks:
-            measurement_std_inputs = (_create_std_input_from_shock(i) for i in measurement_shocks)
-            self._add_quantities(measurement_std_inputs, _quantities.QuantityKind.MEASUREMENT_STD)
-
     def _populate_logly(self, /) -> None:
         default_logly = self._resolve_default_logly()
         qid_to_logly = { 
             qty.id: default_logly if qty.human not in self.log_variables else not default_logly
             for qty in self.quantities
             if qty.kind in LOGLY_VARIABLE
         }
@@ -196,14 +184,31 @@
         return all(a=="all-but" for a in self.all_but) or all(a=="" for a in self.all_but) if self.all_but else True
 
     def _resolve_default_logly(self, /) -> bool:
         if not self._is_logly_consistent():
             raise Exception("Inconsistent use of !all-but in !log-variables")
         return self.all_but.pop()=="all-but" if self.all_but else False
 
+    def _add_stds(
+        self,
+        shock_kind: _quantities.QuantityKind,
+        std_kind: _quantities.QuantityKind,
+        /,
+    ) -> None:
+        """
+        """
+        shocks = (q for q in self.quantities if q.kind in shock_kind)
+        for std_qid, shock in enumerate(shocks, start=len(self.quantities)):
+            std_human = _create_std_name(shock, )
+            std_logly = False
+            std_description = _create_std_description(shock, )
+            std_quantity = _quantities.Quantity(std_qid, std_human, std_kind, std_logly, std_description, )
+            self.quantities.append(std_quantity, )
+            self.shock_qid_to_std_qid[shock.id] = std_qid
+
     @classmethod
     def from_lists(
         cls,
         /,
         transition_variables: Iterable[QuantityInput],
         transition_equations: Iterable[EquationInput], 
         transition_shocks: Iterable[QuantityInput] | None = None,
@@ -279,14 +284,26 @@
 
 
 def _handle_white_spaces(x: str, /) -> str:
     return _re.sub(r"[\s\n\r]+", "", x)
 
 
 def _reorder_by_kind(items: Iterable, /) -> Iterable:
-    return sorted(items, key=lambda x: (x.kind.value, x.entry))
+    return list(sorted(items, key=lambda x: (x.kind.value, x.entry)))
 
 
 def _stamp_id(items: Iterable, /) -> Iterable:
     return [ i.set_id(_id) for _id, i in enumerate(items) ]
 
 
+def _create_std_name(
+    shock: _quantities.Quantity,
+    /,
+) -> str:
+    return STD_PREFIX + shock.human
+
+def _create_std_description(
+    shock: _quantities.Quantity,
+    /,
+) -> str:
+    return _STD_DESCRIPTION + (shock.description if shock.description else shock.human)
+
```

### Comparing `irispie-0.8.1/src/irispie/transforms.py` & `irispie-0.9.0/src/irispie/transforms.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/wrongdoings.py` & `irispie-0.9.0/src/irispie/wrongdoings.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from typing import (TypeAlias, Literal, Callable, )
 from collections.abc import (Iterable, )
 import warnings as _wa
 #]
 
 
-HOW: TypeAlias = Literal["error"] | Literal["warning"] | Literal["silent"]
+HOW: TypeAlias = Literal["error", "warning", "silent"]
+
 
 _PLAIN_PREFIX = ""
 _LIST_PREFIX = "××× "
 
 
 class IrisPieError(Exception):
     """
```

### Comparing `irispie-0.8.1/src/irispie/aldi/adaptations.py` & `irispie-0.9.0/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/aldi/differentiators.py` & `irispie-0.9.0/src/irispie/aldi/differentiators.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 from collections.abc import (Iterable, Sequence, )
 import numpy as _np
 import copy as _cp
 
 from ..exceptions import ListException
 
 from ..aldi import finite_differentiators as af_
-from ..aldi import adaptations as aa_
-from ..incidences import main as _incidence
+from ..aldi import adaptations as _adaptations
+from ..incidences import main as _incidences
+from ..equators import plain as _equators
 from .. import equations as _equations
 #]
 
 
 class ValueMixin:
     #[
     @property
@@ -276,31 +277,34 @@
         """
         self._eid_to_wrts = eid_to_wrts
         self._qid_to_logly = qid_to_logly or {}
         self._num_columns_to_eval = num_columns_to_eval
         self._populate_equations(equations, )
         #
         all_tokens = set(_equations.generate_all_tokens_from_equations(self._equations, ), )
-        self.min_shift = _incidence.get_min_shift(all_tokens, )
-        self.max_shift = _incidence.get_max_shift(all_tokens, )
+        self.min_shift = _incidences.get_min_shift(all_tokens, )
+        self.max_shift = _incidences.get_max_shift(all_tokens, )
         self.shape_data = (
-            1 + (_incidence.get_max_qid(all_tokens) or 0),
+            1 + (_incidences.get_max_qid(all_tokens) or 0),
             -self.min_shift + num_columns_to_eval + self.max_shift,
         )
         #
         self._populate_atom_dict(atom_factory, )
         #
         custom_functions = { 
             k: af_.finite_differentiator(v) 
             for k, v in custom_functions.items()
         } if custom_functions else None
-        custom_functions = aa_.add_function_adaptations_to_custom_functions(custom_functions)
+        custom_functions = _adaptations.add_function_adaptations_to_custom_functions(custom_functions)
         custom_functions["Atom"] = Atom
         #
-        self._equator = _ep.PlainEquator(self._equations, custom_functions, )
+        self._equator = _equators.PlainEquator(
+            self._equations,
+            custom_functions=custom_functions,
+        )
 
     @property
     def _t_zero(self, /, ) -> int:
         """
         """
         return -self.min_shift
 
@@ -323,15 +327,15 @@
         self,
         equations: Iterable[_equations.Equation],
         /,
     ) -> None:
         """
         """
         self._equations = tuple(
-            _adapt_equation_for_aldi(e, _self._get_diff_shape_for_eid(e.id), )
+            _adapt_equation_for_aldi(e, self._get_diff_shape_for_eid(e.id), )
             for e in equations
         )
 
     def _populate_atom_dict(
         self,
         atom_factory: AtomFactoryProtocol,
         /,
@@ -340,14 +344,15 @@
         * atom_factory -- Implement create_diff_for_token, create_data_index_for_token, get_logly_for_token
         * qid_to_logly -- Dictionary of qid to logly
         * columns_to_eval -- Tuple of (first, last) column indices to be evaluated
         """
         columns_to_eval = self._get_columns_to_eval()
         self._x = {}
         for eqn in self._equations:
+            self._x[eqn.id] = {}
             for tok in eqn.incidence:
                 atom = Atom.in_context(
                     diff=atom_factory.create_diff_for_token(tok, self._eid_to_wrts[eqn.id], ),
                     data_index=atom_factory.create_data_index_for_token(tok, columns_to_eval, ),
                     logly=self._qid_to_logly.get(tok.qid, False, ),
                 )
                 self._x[eqn.id][(tok.qid, tok.shift)] = atom
@@ -358,15 +363,15 @@
         steady_array: _np.ndarray,
     ) -> Iterable[Atom]:
         """
         Evaluate and return the list of final atoms, one atom for each equation
         """
         self._verify_data_array_shape(data_array.shape, )
         Atom._data_context = data_array
-        output = self._equator.eval(self._x, None, steady_array, )
+        output = self._equator.eval(self._x, 0, steady_array, )
         Atom._data_context = None
         return output
 
     def eval_to_arrays(
         self,
         *args,
     ) -> tuple[_np.ndarray, _np.ndarray]:
@@ -404,15 +409,15 @@
     diff_shape: tuple[int, int],
     /,
 ) -> _equations.Equation:
     """
     """
     #[
     aldi_equation = _cp.deepcopy(equation)
-    aldi_equation.xtring = aldi_equation.xtring.replace("x[", f"x[{eid}][")
+    aldi_equation.xtring = aldi_equation.xtring.replace("x[", f"x[{aldi_equation.id}][")
     aldi_equation.xtring += f" + Atom.zero({diff_shape}, )"
     return aldi_equation
     #]
 
 
 class InvalidInputDataArrayShape(ListException, ):
     """
@@ -431,25 +436,25 @@
 class AtomFactoryProtocol(Protocol, ):
     """
     Protocol for creating atoms representing tokens
     """
     #[
     def create_diff_for_token(
         self,
-        token: _incidence.Token,
+        token: _incidences.Token,
         wrts: tuple[Any, ...],
     ) -> _np.ndarray:
         """
         Create a diff for an atom representing a given token
         """
         ...
 
     def create_data_index_for_token(
         self,
-        token: _incidence.Token,
+        token: _incidences.Token,
         columns_to_eval: tuple[int, int],
     ) -> tuple[int, slice]:
         """
         Create a data index for an atom representing a given token
         """
         ...
     #]
```

### Comparing `irispie-0.8.1/src/irispie/aldi/express.py~` & `irispie-0.9.0/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/aldi/finite_differentiators.py` & `irispie-0.9.0/src/irispie/aldi/finite_differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/aldi/invariators.py` & `irispie-0.9.0/src/irispie/aldi/invariators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/aldi/maps.py` & `irispie-0.9.0/src/irispie/aldi/maps.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/conveniences/views.py` & `irispie-0.9.0/src/irispie/conveniences/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     elif x is ...:
         s = "..."
     elif isinstance(x, Number):
         s = str(x)
     elif isinstance(x, str):
         s = f'"{x}"'
     elif isinstance(x, _np.ndarray) or isinstance(x, list) or isinstance(x, tuple):
-        s = _re.sub("\n + ", " ", repr(x))
+        s = _re.sub(r"\n+ +", " ", repr(x))
     elif hasattr(x, "_get_first_line_view"):
         s = x._get_first_line_view()
     else:
         s = repr(type(x))
     return s if len(s)<_REPR_MAX_LEN else s[0:_REPR_MAX_LEN] + _REPR_CONT
     #]
```

### Comparing `irispie-0.8.1/src/irispie/databanks/_exports.py` & `irispie-0.9.0/src/irispie/databanks/_exports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/databanks/_imports.py` & `irispie-0.9.0/src/irispie/databanks/_imports.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/databanks/_imports2.py` & `irispie-0.9.0/src/irispie/databanks/_imports2.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/databanks/main.py` & `irispie-0.9.0/src/irispie/databanks/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 __all__ = [
     "Databank",
 ]
 
 
 SourceNames: TypeAlias = Iterable[str] | str | Callable[[str], bool] | None
 TargetNames: TypeAlias = Iterable[str] | str | Callable[[str], str] | None
-InterpretRange: TypeAlias = Literal["base"] | Literal["extended"]
+InterpretRange: TypeAlias = Literal["base", "extended", ]
 
 
 class SteadyDatabankableProtocol(Protocol):
     """
     """
     #[
     def get_min_max_shifts(self, *args) -> tuple(int, int): ...
@@ -71,21 +71,21 @@
 
 _EXTENDED_RANGE_TUPLE_RESOLUTION = {
     "base": _extended_range_tuple_from_base_range,
     "extended": _extended_range_tuple_from_extended_range,
 }
 
 
-_SERIES_CONSTRUCTOR_RESOLUTION = {
+_SERIES_CONSTRUCTOR_FACTORY = {
     "start_date": _series.Series.from_start_date_and_values,
     "range": _series.Series.from_dates_and_values,
 }
 
 
-_ARRAY_TRANSPOSER_RESOLUTION = {
+_ARRAY_TRANSPOSER_FACTORY = {
     "vertical": _np.transpose,
     "horizontal": lambda x: x,
 }
 
 
 class Databank(
     _imports.DatabankImportMixin,
@@ -123,28 +123,30 @@
         cls,
         array: _np.ndarray,
         qid_to_name: Sequence[str] | dict[int, str],
         dates: _dates.Dater,
         /,
         add_to_databank: Self | None = None,
         qid_to_description: dict[int, str] | None = None,
-        array_orientation: Literal["vertical"] | Literal["horizontal"] = "vertical",
-        interpret_dates: Literal["start_date"] | Literal["range"] = "start_date",
+        array_orientation: Literal["vertical", "horizontal", ] = "vertical",
+        interpret_dates: Literal["start_date", "range", ] = "start_date",
     ) -> Self:
         """
         """
         self = add_to_databank if add_to_databank else cls()
-        constructor = _SERIES_CONSTRUCTOR_RESOLUTION[interpret_dates]
-        transposer = _ARRAY_TRANSPOSER_RESOLUTION[array_orientation]
+        constructor = _SERIES_CONSTRUCTOR_FACTORY[interpret_dates]
+        transposer = _ARRAY_TRANSPOSER_FACTORY[array_orientation]
         for qid, data in enumerate(transposer(array)):
             name = qid_to_name.get(qid, None)
             if not name:
                 continue
+            if data.ndim == 1:
+                data = data.reshape(-1, 1)
             description = qid_to_description[qid] if qid_to_description else ""
-            series = constructor(dates, data.reshape(-1, 1), description=description)
+            series = constructor(dates, data, description=description)
             self[name] = series
         return self
 
     @classmethod
     def for_simulation(
         cls,
         simulatable: SimulatableProtocol,
@@ -350,49 +352,20 @@
         if num_columns < 1:
             raise Exception("Empty date range is not allowed when creating steady databank")
         steady_databank = steady_databankable._get_steady_databank(start_date, end_date, deviation=deviation)
         self.update(steady_databank)
 
     add_zero = _ft.partialmethod(add_steady, deviation=True)
 
-###     def __getitem__(self, name):
-###         return self.__dict__[name]
-### 
-###     def __setitem__(self, name, value) -> None:
-###         self.__dict__[name] = value
-### 
-###     def __or__(self, other) -> Self:
-###         new = _co.deepcopy(self)
-###         new.__dict__.update(other.__dict__)
-###         return new
-### 
-###     def _update(
-###         self,
-###         other: Databank,
-###         /,
-###     ) -> Self:
-###         """
-###         Update self using items from other
-###         """
-###         self.__dict__.update(other.__dict__)
+    def __or__(self, other) -> Self:
+        new = _co.deepcopy(self)
+        new.update(other, )
+        return new
     #]
 
-
-#
-# Add databank methods without the leading underscore
-#
-### exceptions = ["_description", ]
-### single_underscore_names = [
-###     n for n in dir(Databank) 
-###     if n.startswith("_") and not n.startswith("__") and not n.endswith("_") and n not in exceptions
-### ]
-### for n in single_underscore_names:
-###     setattr(Databank, n.removeprefix("_"), getattr(Databank, n))
-
-
 def _resolve_source_target_names(
     source_names: SourceNames,
     target_names: TargetNames,
     context_names: Iterable[str],
     /,
 ) -> tuple[Iterable[str], Iterable[str]]:
     """
```

### Comparing `irispie-0.8.1/src/irispie/equators/plain.py` & `irispie-0.9.0/src/irispie/equators/plain.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         self,
         custom_functions: dict | None = None,
         /,
     ) -> None:
         """
         """
         custom_functions = _aa.add_function_adaptations_to_custom_functions(custom_functions, )
-        joined_xtrings = " , ".join(i.xtring for i in self_equations)
-        func_string = _eq.EVALUATOR_PREAMBLE + "(" + joined_xtrings + " , )"
-        self._func = eval(func_string, custom_functions, )
+        joined_xtrings = "  ,  ".join(i.xtring for i in self._equations)
+        self._func_str = _eq.EVALUATOR_PREAMBLE + "(" + joined_xtrings + " , )"
+        self._func = eval(self._func_str, custom_functions, )
 
     def _populate_min_max_shifts(self, /, ) -> None:
         """
         """
         self.min_shift = _eq.get_min_shift_from_equations(self._equations, )
         self.max_shift = _eq.get_max_shift_from_equations(self._equations, )
```

### Comparing `irispie-0.8.1/src/irispie/equators/steady.py` & `irispie-0.9.0/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/evaluators/printers.py` & `irispie-0.9.0/src/irispie/evaluators/printers.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 #[
 from collections.abc import (Iterable, )
 from numbers import (Number, )
 import numpy as _np
 import scipy as _sp
+import os as _os
 
 from .. import equations as _equations
 from .. import quantities as _quantities
 #]
 
 
 class IterPrinter:
@@ -34,39 +35,39 @@
         every: int = 1,
     ) -> None:
         """
         """
         self._populate_equations(equations)
         self._populate_quantities(qids, qid_to_logly, qid_to_name, )
         ...
-        self._iter_count = 0
+        self._func_count = 0
         self._curr_f = None
         self._curr_x = None
         self._prev_x = None
         self._prev_f = None
         self._every = every
 
     def next(self, x, f, j_done, /, ) -> None:
         """
-        Handle next iteration
+        Handle next function evaluation
         """
-        self._curr_f = f.flatten()
-        self._curr_x = x.flatten()
+        self._curr_f = _np.array(tuple(f))
+        self._curr_x = _np.array(tuple(x))
         f_norm = _sp.linalg.norm(self._curr_f, 2)
-        if self._iter_count == 0:
+        if self._func_count == 0:
             dimension = (self._curr_f.size, self._curr_x.size, )
             self.print_header(dimension, )
         self._last_iter_string = self.get_iter_string(f_norm, j_done, *self.find_worst_diff_x(), *self.find_worst_equation(), )
-        if self._iter_count % self._every == 0:
-            print(self._last_iter_string)
+        if self._func_count % self._every == 0:
+            _print_to_width(self._last_iter_string)
         self._prev_x = self._curr_x
         self._prev_f = self._curr_f
         self._curr_f = None
         self._curr_x = None
-        self._iter_count += 1
+        self._func_count += 1
 
     def find_worst_equation(self, /, ) -> tuple[Number, str]:
         """
         Find the largest function residual and the corresponding equation
         """
         index = _np.argmax(_np.abs(self._curr_f))
         worst_f = _np.abs(self._curr_f[index])
@@ -86,30 +87,30 @@
         worst_qid = self._qids[index]
         maybelog_worst_name = self._qid_to_print[worst_qid]
         maybelog_worst_name = _clip_string_exactly(maybelog_worst_name, self._MAX_LEN_NAME_STRING)
         return f"{worst_diff_x:.5e}", maybelog_worst_name
 
     def print_header(self, dimension, /, ) -> None:
         """
-        Print header for iterations
+        Print header for fuction evaluations
         """
         dim_string = f"Dimension: {dimension[0]}×{dimension[1]}"
-        header = f"{'iter':>5}   {'‖ƒ‖':>11}   {'∇ƒ':>5}   {'max|∆x|':>11}   {' ':10}   {'max|ƒ|':>11}   {''}"
+        header = f"{'ƒ-count':>8}   {'‖ƒ‖':>11}   {'∇ƒ':>5}   {'max|∆x|':>11}   {' ':10}   {'max|ƒ|':>11}   {''}"
         len_header = len(header) + self._MAX_LEN_EQUATION_STRING + 1
         self._divider_line = self._HEADER_DIVIDER_CHAR * len_header
         upper_divider = self._divider_line
         upper_divider = self._divider_line[0:2] + dim_string + self._divider_line[2 + len(dim_string):]
         lower_divider = self._divider_line
-        print("", upper_divider, header, lower_divider, sep="\n")
+        _print_to_width("", upper_divider, header, lower_divider, )
 
     def print_footer(self, /, ) -> None:
         """
         Print footer for iterations
         """
-        print(self._divider_line, self._last_iter_string, self._divider_line, sep="\n")
+        _print_to_width(self._divider_line, self._last_iter_string, self._divider_line, )
 
     def get_iter_string(
         self,
         f_norm: Number,
         j_done: bool,
         worst_diff_x: str | None,
         worst_diff_x_name: str | None,
@@ -117,21 +118,21 @@
         worst_equation: str,
         /,
     ) -> None:
         """
         Print info on current iteration
         """
         j_done_string = "√" if j_done else "×"
-        return f"{self._iter_count:5g}   {f_norm:.5e}   {j_done_string:>5}   {worst_diff_x}   {worst_diff_x_name}   {worst_f}   {worst_equation}"
+        return f"{self._func_count:8g}   {f_norm:.5e}   {j_done_string:>5}   {worst_diff_x}   {worst_diff_x_name}   {worst_f}   {worst_equation}"
 
     def reset(self, /, ) -> None:
         """
         Reset iterations printer
         """
-        self._iter_count = 0
+        self._func_count = 0
         self._prev_x = None
         self._prev_f = None
     #]
 
 
 class FlatSteadyIterPrinter(IterPrinter, ):
     """
@@ -201,12 +202,21 @@
     max_length: int,
     /,
 ) -> str:
     """
     Clip string to exactly to max length
     """
     return (
-        full_string[:max_length-1] + "…" 
+        full_string[:max_length-1] + "⋯" 
         if len(full_string) > max_length else f"{full_string:{max_length}}"
     )
 
 
+def _print_to_width(*args, ) -> None:
+    """
+    """
+    width = _os.get_terminal_size().columns
+    for text in args:
+        if len(text) > width:
+            text = text[:width-1] + "⋯"
+        print(text)
+
```

### Comparing `irispie-0.8.1/src/irispie/evaluators/steady.py` & `irispie-0.9.0/src/irispie/evaluators/steady.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Steady state evaluator
 """
 
 
 #[
-import numpy as _np
 from collections.abc import (Iterable, )
 from types import (EllipsisType, )
+from typing import (Any, )
 from numbers import (Number, )
+import itertools as _it
+import numpy as _np
 
 from .. import equations as _equations
 from .. import quantities as _quantities
 from ..equators import steady as _equators
 from ..jacobians import steady as _jacobians
 from ..models import variants as _variants
 
@@ -39,21 +41,25 @@
         wrt_equations: Iterable[_equations.Equation],
         all_quantities: Iterable[_quantities.Quantity],
         wrt_qids_levels: list[int],
         wrt_qids_changes: list[int],
         variant: _variants.Variant,
         /,
         custom_functions: dict | None = None,
+        iter_printer_settings: dict[str, Any] | None = None,
     ) -> None:
         """
         """
         wrt_equations = list(wrt_equations, )
         #
-        # Create an overall self.wrt_qids comprising qids from both levels
-        # and changes, and then logical indices for levels and changes
+        # Create an overall long list `self.wrt_qids` comprising qids from both
+        # levels and changes, and then logical indices
+        # `self._bool_index_wrt_levels` and `._bool_index_wrt_changes` for
+        # accessing the levels and changes within the long list
+        #
         self._merge_levels_and_changes(wrt_qids_levels, wrt_qids_changes, )
         #
         qid_to_logly = _quantities.create_qid_to_logly(all_quantities, )
         qid_to_name = _quantities.create_qid_to_name(all_quantities, )
         #
         shift_vec, t_zero = _prepare_time_shifts(wrt_equations, )
         self._shift_vec = shift_vec
@@ -61,49 +67,66 @@
         #
         self._index_logly = list(_quantities.generate_index_logly(self.wrt_qids, qid_to_logly, ))
         #
         # Vectors self._maybelog_init_levels and
         # self._maybelog_init_changes are the initial guesses from the
         # variant data with missing values filled in for the long list of
         # wrt_qids. The actual values iterated over are
-        # self.maybelog_levels[self._index_wrt_levels] and
-        # self.maybelog_changes[self._index_wrt_changes].
+        # self.maybelog_levels[self._bool_index_wrt_levels] and
+        # self.maybelog_changes[self._bool_index_wrt_changes].
+        #
         maybelog_levels, maybelog_changes = variant.retrieve_maybelog_values_for_qids(self.wrt_qids, qid_to_logly, )
         maybelog_levels, maybelog_changes = _fill_missing(maybelog_levels, maybelog_changes, )
         self._maybelog_init_levels = maybelog_levels
         self._maybelog_init_changes = maybelog_changes
         #
-        self._num_levels = sum(self._index_wrt_levels)
-        self._num_changes = sum(self._index_wrt_changes)
+        self._num_levels = sum(self._bool_index_wrt_levels)
+        self._num_changes = sum(self._bool_index_wrt_changes)
         #
         self.init_guess = _np.hstack((
-            self._maybelog_init_levels[self._index_wrt_levels],
-            self._maybelog_init_changes[self._index_wrt_changes],
+            self._maybelog_init_levels[self._bool_index_wrt_levels],
+            self._maybelog_init_changes[self._bool_index_wrt_changes],
         ))
         #
         self._steady_array = variant.create_steady_array(qid_to_logly, num_columns=shift_vec.shape[1], shift_in_first_column=-t_zero, )
         self._update_steady_array(self.init_guess)
         #
         # Set up components
-        self._equator = self._equator_factory(wrt_equations, t_zero, custom_functions=custom_functions, )
-        self._jacobian = self._jacobian_factory(wrt_equations, self.wrt_qids, qid_to_logly, custom_functions=custom_functions, )
-        self._iter_printer = self._iter_printer_factory(wrt_equations, self.wrt_qids, qid_to_logly, qid_to_name, every=1, )
+        self._equator = self._equator_factory(
+            wrt_equations,
+            t_zero,
+            custom_functions=custom_functions,
+        )
+        self._jacobian = self._jacobian_factory(
+            wrt_equations,
+            self.wrt_qids,
+            qid_to_logly,
+            custom_functions=custom_functions,
+        )
+        iter_printer_settings = iter_printer_settings or {}
+        self.iter_printer = self._iter_printer_factory(
+            wrt_equations,
+            self.wrt_qids,
+            qid_to_logly,
+            qid_to_name,
+            **iter_printer_settings,
+        )
 
     def eval(
         self,
         maybelog_guess: _np.ndarray,
         /,
     ) -> tuple[_np.ndarray, _np.ndarray]:
         """
         """
         self._update_steady_array(maybelog_guess, )
         equator = self._equator.eval(self._steady_array, )
         jacobian = self._jacobian.eval(self._steady_array, )
-        jacobian = jacobian[:, self._index_wrt_levels + self._index_wrt_changes]
-        self._iter_printer.next(maybelog_guess, equator, True, )
+        jacobian = jacobian[:, self._bool_index_wrt_levels + self._bool_index_wrt_changes]
+        self.iter_printer.next(maybelog_guess, equator, True, )
         return equator, jacobian
 
     def _merge_levels_and_changes(
         self,
         wrt_qids_levels: list[str],
         wrt_qids_changes: list[str],
         /,
@@ -116,14 +139,40 @@
         self,
         current_guess: _np.ndarray,
         /,
     ) -> None:
         """
         """
         ...
+
+    def extract_levels(
+        self,
+        guess: _np.ndarray,
+        /,
+    ) -> tuple[_np.ndarray, tuple[int, ...]]:
+        """
+        """
+        levels = self._get_maybelog_levels(guess, )
+        levels[self._index_logly] = _np.exp(levels[self._index_logly])
+        levels = levels[self._bool_index_wrt_levels]
+        wrt_qids_levels = tuple(_it.compress(self.wrt_qids, self._bool_index_wrt_levels, ))
+        return levels, wrt_qids_levels
+
+    def extract_changes(
+        self,
+        guess: _np.ndarray,
+        /,
+    ) -> tuple[_np.ndarray, tuple[int, ...]]:
+        """
+        """
+        changes = self._get_maybelog_changes(guess, )
+        changes[self._index_logly] = _np.exp(changes[self._index_logly])
+        changes = changes[self._bool_index_wrt_changes]
+        wrt_qids_changes = tuple(_it.compress(self.wrt_qids, self._bool_index_wrt_changes, ))
+        return changes, wrt_qids_changes
     #]
 
 
 class FlatSteadyEvaluator(SteadyEvaluator, ):
     """
     """
     #[
@@ -134,27 +183,27 @@
     def _merge_levels_and_changes(
         self,
         wrt_qids_levels: list[int],
         wrt_qids_changes: list[int],
         /,
     ) -> None:
         self.wrt_qids = list(set(wrt_qids_levels))
-        self._index_wrt_levels = [qid in wrt_qids_levels for qid in self.wrt_qids]
-        self._index_wrt_changes = []
+        self._bool_index_wrt_levels = [qid in wrt_qids_levels for qid in self.wrt_qids]
+        self._bool_index_wrt_changes = []
 
     def _get_maybelog_levels(
         self,
         current_guess: _np.ndarray,
         /,
     ) -> _np.ndarray:
         """
         """
         new_maybelog_levels = _np.copy(self._maybelog_init_levels)
-        if self._index_wrt_levels:
-            new_maybelog_levels[self._index_wrt_levels] = current_guess
+        if self._bool_index_wrt_levels:
+            new_maybelog_levels[self._bool_index_wrt_levels] = current_guess
         return new_maybelog_levels
 
     def _get_maybelog_changes(
         self,
         current_guess: _np.ndarray,
         /,
     ) -> _np.ndarray:
@@ -187,39 +236,39 @@
     def _merge_levels_and_changes(
         self,
         wrt_qids_levels: list[str],
         wrt_qids_changes: list[str],
         /,
     ) -> None:
         self.wrt_qids = list(set(wrt_qids_levels) | set(wrt_qids_changes))
-        self._index_wrt_levels = [qid in wrt_qids_levels for qid in self.wrt_qids]
-        self._index_wrt_changes = [qid in wrt_qids_changes for qid in self.wrt_qids]
+        self._bool_index_wrt_levels = [qid in wrt_qids_levels for qid in self.wrt_qids]
+        self._bool_index_wrt_changes = [qid in wrt_qids_changes for qid in self.wrt_qids]
 
     def _get_maybelog_levels(
         self,
         current_guess: _np.ndarray,
         /,
     ) -> _np.ndarray:
         """
         """
         new_maybelog_levels = _np.copy(self._maybelog_init_levels)
-        if self._index_wrt_levels:
-            new_maybelog_levels[self._index_wrt_levels] = current_guess[:self._num_levels]
+        if self._bool_index_wrt_levels:
+            new_maybelog_levels[self._bool_index_wrt_levels] = current_guess[:self._num_levels]
         return new_maybelog_levels
 
     def _get_maybelog_changes(
         self,
         current_guess: _np.ndarray,
         /,
     ) -> _np.ndarray:
         """
         """
         new_maybelog_changes = _np.copy(self._maybelog_init_changes)
-        if self._index_wrt_changes:
-            new_maybelog_changes[self._index_wrt_changes] = current_guess[self._num_levels:]
+        if self._bool_index_wrt_changes:
+            new_maybelog_changes[self._bool_index_wrt_changes] = current_guess[self._num_levels:]
         return new_maybelog_changes
 
     def _update_steady_array(
         self,
         current_guess: _np.ndarray,
         /,
     ) -> None:
```

### Comparing `irispie-0.8.1/src/irispie/executables/default.spc~` & `irispie-0.9.0/src/irispie/executables/default.spc~`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/libgcc_s.1.dylib` & `irispie-0.9.0/src/irispie/executables/libgcc_s.1.dylib`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/libgfortran.3.dylib` & `irispie-0.9.0/src/irispie/executables/libgfortran.3.dylib`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/libquadmath.0.dylib` & `irispie-0.9.0/src/irispie/executables/libquadmath.0.dylib`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/x12awin.exe` & `irispie-0.9.0/src/irispie/executables/x12awin.exe`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/x13asmac` & `irispie-0.9.0/src/irispie/executables/x13asmac`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/x13asunix` & `irispie-0.9.0/src/irispie/executables/x13asunix`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/executables/x13aswin.exe` & `irispie-0.9.0/src/irispie/executables/x13aswin.exe`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/explanatories/main.py` & `irispie-0.9.0/src/irispie/explanatories/main.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/fords/descriptors.py` & `irispie-0.9.0/src/irispie/fords/descriptors.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import numpy as np_
 
 from ..incidences import main as _incidence
 from .. import equations as _equations
 from .. import quantities as _quantities
 from ..aldi import differentiators as _differentiators
 from ..aldi import maps as _maps
+from .. import sources as _sources
 #]
 
 
 class _AtomFactory:
     """
     """
     #[
@@ -149,18 +150,20 @@
     """
     #[
     transition_eids: Iterable[int] | None = None
     measurement_eids: Iterable[int] | None = None
     eid_to_wrt_tokens: dict[int, Iterable[_incidence.Token]] | None = None
     #
     transition_variables: Iterable[_incidence.Token] | None = None
+    transition_variables_logly: tuple[bool, ...] | None = None
     initial_conditions: Iterable[bool] | None = None,
-    transition_shocks: Iterable[_incidence.Token] | None = None 
+    transition_shocks: tuple[_incidence.Token, ...] | None = None 
     measurement_variables: Iterable[_incidence.Token] | None = None
-    measurement_shocks: Iterable[_incidence.Token] | None = None 
+    measurement_variables_logly: tuple[bool, ...] | None = None
+    measurement_shocks: tuple[_incidence.Token, ...] | None = None 
     #
     shape_A_excl_dynid: tuple[int, int] | None = None
     shape_B_excl_dynid: tuple[int, int] | None = None
     shape_C_excl_dynid: tuple[int, int] | None = None
     shape_D_excl_dynid: tuple[int, int] | None = None
     shape_F: tuple[int, int] | None = None
     shape_G: tuple[int, int] | None = None
@@ -172,54 +175,78 @@
         equations: Iterable[_equations.Equation],
         quantities: Iterable[_quantities.Quantity],
         /,
     ) -> None:
         """
         Construct system vectors from a list of equations and a list of quantities
         """
-        self.transition_eids = sorted([eqn.id for eqn in equations if eqn.kind in _equations.EquationKind.TRANSITION_EQUATION])
-        self.measurement_eids = sorted([eqn.id for eqn in equations if eqn.kind in _equations.EquationKind.MEASUREMENT_EQUATION])
-        qid_to_kind = _quantities.create_qid_to_kind(quantities)
+        qid_to_logly = _quantities.create_qid_to_logly(quantities, )
+        #
+        self.transition_eids \
+            = sorted([eqn.id for eqn in equations if eqn.kind in _equations.EquationKind.TRANSITION_EQUATION])
+        self.measurement_eids \
+            = sorted([eqn.id for eqn in equations if eqn.kind in _equations.EquationKind.MEASUREMENT_EQUATION])
+        qid_to_kind = _quantities.create_qid_to_kind(quantities, )
         all_tokens = set(_equations.generate_all_tokens_from_equations(equations))
         all_wrt_tokens = set(_incidence.generate_tokens_of_kinds(all_tokens, qid_to_kind, _SYSTEM_QUANTITY))
         self.eid_to_wrt_tokens = _equations.create_eid_to_wrt_tokens(equations, all_wrt_tokens)
         #
-        actual_tokens_transition_variables = set(_incidence.generate_tokens_of_kinds(all_tokens, qid_to_kind, _quantities.QuantityKind.TRANSITION_VARIABLE))
+        actual_tokens_transition_variables \
+            = set(_incidence.generate_tokens_of_kinds(all_tokens, qid_to_kind, _quantities.QuantityKind.TRANSITION_VARIABLE))
         #
         # Make adjustment for transition variables in measurement
         # equations: each x(t-k) in measurement needs to be in the current
         # dated (LHS) vector of transition variables; this is done by
         # pretending x(t-k-1) is needed
-        adjusted_tokens_transition_variables = _adjust_for_measurement_equations(actual_tokens_transition_variables, equations, qid_to_kind)
         #
-        self.transition_variables = _incidence.sort_tokens(_create_system_transition_vector(adjusted_tokens_transition_variables))
+        adjusted_tokens_transition_variables \
+            = _adjust_for_measurement_equations(actual_tokens_transition_variables, equations, qid_to_kind)
+        #
+        self.transition_variables \
+            = _incidence.sort_tokens(_create_system_transition_vector(adjusted_tokens_transition_variables))
+        self.transition_variables_logly \
+            = tuple(qid_to_logly[tok.qid] for tok in self.transition_variables)
         self.initial_conditions = [
             _incidence.Token(t.qid, t.shift-1) in actual_tokens_transition_variables and t.shift <= 0
             for t in self.transition_variables
         ]
-        self.transition_shocks = _incidence.sort_tokens(
-            _incidence.generate_tokens_of_kinds(all_tokens, qid_to_kind, _quantities.QuantityKind.TRANSITION_SHOCK)
-        )
         #
-        self.measurement_variables = _incidence.sort_tokens(
-            _incidence.generate_tokens_of_kinds(all_tokens, qid_to_kind, _quantities.QuantityKind.MEASUREMENT_VARIABLE)
-        )
-        self.measurement_shocks = _incidence.sort_tokens(
-            _incidence.generate_tokens_of_kinds(all_tokens, qid_to_kind, _quantities.QuantityKind.MEASUREMENT_SHOCK)
-        )
+        # Transition shocks
         #
-        self.shape_A_excl_dynid = (len(self.transition_eids), len(self.transition_variables))
-        self.shape_B_excl_dynid = self.shape_A_excl_dynid
-        self.shape_C_excl_dynid = (len(self.transition_eids), 1)
-        self.shape_D_excl_dynid = (len(self.transition_eids), len(self.transition_shocks))
+        self.transition_shocks \
+            = tuple(_incidence.sort_tokens(_incidence.generate_tokens_of_kinds(
+                all_tokens, qid_to_kind, _quantities.QuantityKind.TRANSITION_SHOCK,
+            )))
+        #
+        # Measurement variables
+        #
+        self.measurement_variables \
+            = tuple(_incidence.sort_tokens(_incidence.generate_tokens_of_kinds(
+                all_tokens, qid_to_kind, _quantities.QuantityKind.MEASUREMENT_VARIABLE,
+            )))
+        self.measurement_variables_logly \
+            = tuple(qid_to_logly[tok.qid] for tok in self.measurement_variables)
+        #
+        # Measurement shocks
+        #
+        self.measurement_shocks \
+            = tuple(_incidence.sort_tokens(_incidence.generate_tokens_of_kinds(
+                all_tokens, qid_to_kind, _quantities.QuantityKind.MEASUREMENT_SHOCK,
+            )))
         #
-        self.shape_F = (len(self.measurement_eids), len(self.measurement_variables))
-        self.shape_G = (len(self.measurement_eids), len(self.transition_variables))
-        self.shape_H = (len(self.measurement_eids), 1)
-        self.shape_J = (len(self.measurement_eids), len(self.measurement_shocks))
+        # Shapes of matrices
+        #
+        self.shape_A_excl_dynid = (len(self.transition_eids), len(self.transition_variables), )
+        self.shape_B_excl_dynid = self.shape_A_excl_dynid
+        self.shape_C_excl_dynid = (len(self.transition_eids), 1, )
+        self.shape_D_excl_dynid = (len(self.transition_eids), len(self.transition_shocks), )
+        self.shape_F = (len(self.measurement_eids), len(self.measurement_variables), )
+        self.shape_G = (len(self.measurement_eids), len(self.transition_variables), )
+        self.shape_H = (len(self.measurement_eids), 1, )
+        self.shape_J = (len(self.measurement_eids), len(self.measurement_shocks), )
 
     def get_num_backwards(self) -> int:
         return _get_num_backwards(self.transition_variables)
 
     def get_num_forwards(self) -> int:
         return _get_num_forwards(self.transition_variables)
     #]
@@ -227,42 +254,45 @@
 
 @_dc.dataclass(slots=True, )
 class SolutionVectors:
     """
     Vectors of quantities in first-order solution matrices
     """
     #[
-    transition_variables: Iterable[_incidence.Token] | None = None
-    initial_conditions: Iterable[bool] | None = None,
-    transition_shocks: Iterable[_incidence.Token] | None = None 
-    measurement_variables: Iterable[_incidence.Token] | None = None
-    measurement_shocks: Iterable[_incidence.Token] | None = None 
+    transition_variables: tuple[_incidence.Token] | None = None
+    initial_conditions: tuple[bool] | None = None,
+    transition_shocks: tuple[_incidence.Token] | None = None 
+    measurement_variables: tuple[_incidence.Token] | None = None
+    measurement_shocks: tuple[_incidence.Token] | None = None 
 
     def __init__(self, system_vectors: SystemVectors, /, ) -> None:
         """
         Construct solution vectors and initial conditions indicator
         """
-        self.transition_variables, self.initial_conditions = _solution_vector_from_system_vector(system_vectors.transition_variables, system_vectors.initial_conditions)
-        self.transition_shocks = system_vectors.transition_shocks
-        self.measurement_variables = system_vectors.measurement_variables
-        self.measurement_shocks = system_vectors.measurement_shocks
+        self.transition_variables, self.initial_conditions = \
+            _solution_vector_from_system_vector(system_vectors.transition_variables, system_vectors.initial_conditions)
+        self.transition_shocks = tuple(system_vectors.transition_shocks)
+        self.measurement_variables = tuple(system_vectors.measurement_variables)
+        self.measurement_shocks = tuple(system_vectors.measurement_shocks)
 
     def get_initials(
         self,
-        /, 
-        kind: Literal["required"] | Literal["discarded"] = "required",
+        /,
     ) -> Iterable[_incidence.Token]:
         """
         Get tokens representing required initial conditions
         """
         return list(it_.compress(self.transition_variables, self.initial_conditions))
     #]
 
 
-def _create_system_transition_vector(tokens_transition_variables: Iterable[_incidence.Token], /, ) -> Iterable[_incidence.Token]:
+def _create_system_transition_vector(
+    tokens_transition_variables: Iterable[_incidence.Token],
+    /,
+) -> Iterable[_incidence.Token]:
     """
     From tokens of transition variables, create vector of transition variables
     along columns of matrix A in unsolved system
     """
     #[
     tokens_transition_variables = set(tokens_transition_variables)
     min_shifts = _incidence.get_some_shift_by_quantities(tokens_transition_variables, lambda x: min(min(x), -1))
@@ -280,15 +310,18 @@
     /,
 ) -> Iterable[_incidence.Token]:
     """
     From sorted system vector, get vector of transition variables in solved
     system and the indicator of required initial conditions
     """
     num_forwards = _get_num_forwards(system_transition_vector)
-    return system_transition_vector[num_forwards:], initial_conditions[num_forwards:]
+    return (
+        tuple(system_transition_vector[num_forwards:]),
+        tuple(initial_conditions[num_forwards:]),
+    )
 
 
 def _get_num_forwards(system_transition_vector: Iterable[_incidence.Token]):
     """
     Number of forward-looking tokens in a vector of tokens
     """
     return sum(1 for t in system_transition_vector if t.shift>0)
@@ -469,8 +502,7 @@
     measurement_eids: list[int],
     /
 ) -> Iterable[_equations.Equation]:
     eid_to_equation = { eqn.id:eqn for eqn in equations }
     system_eids = transition_eids + measurement_eids
     return ( eid_to_equation[eid] for eid in system_eids )
 
-
```

### Comparing `irispie-0.8.1/src/irispie/fords/simulators.py` & `irispie-0.9.0/src/irispie/fords/simulators.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ..databanks import main as _databanks
 #]
 
 
 def simulate_flat(
     solution: _solutions.Solution,
     solution_vectors: _descriptors.SolutionVectors,
+    boolex_logly: tuple[bool, ...],
     data: np_.ndarray,
     columns_to_run: list[int],
     deviation: bool,
     anticipate: bool,
 ):
     column_start = columns_to_run[0]
     column_slice = slice(column_start, column_start+len(columns_to_run))
@@ -32,14 +33,17 @@
     R = solution.R
     K = solution.K if not deviation else 0
 
     Z = solution.Z
     H = solution.H
     D = solution.D if not deviation else 0
 
+    if any(boolex_logly):
+        data[boolex_logly, :] = np_.log(data[boolex_logly, :])
+
     curr_state = np_.array([
         data[t.qid, column_start-1+t.shift] 
         for t in vec.transition_variables
     ], dtype=float).reshape(-1, 1)
 
     missing_initials = np_.isnan(curr_state)
     unnecessary_initials = ~np_.array(vec.initial_conditions).reshape(-1, 1)
@@ -93,9 +97,12 @@
 
         y = Z @ curr_state + H @ measurement_shocks[:, (t,)] + D
         data[measurement_variables_to_slab, t] = y.flat
 
     data[transition_shocks_in_slab, :] = transition_shocks
     data[measurement_shocks_in_slab, :] = measurement_shocks
 
+    if any(boolex_logly):
+        data[boolex_logly, :] = np_.exp(data[boolex_logly, :])
+
     return data
```

### Comparing `irispie-0.8.1/src/irispie/fords/steadiers.py` & `irispie-0.9.0/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/incidences/blazer.py` & `irispie-0.9.0/src/irispie/incidences/blazer.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,35 +45,49 @@
     if eids is None:
         eids = range(im.shape[0])
     if qids is None:
         qids = range(im.shape[1])
     eids = tuple(eids)
     qids = tuple(qids)
     #
+    # Step 1: Prefetch quantities/equations that can be ordered first
+    # individually (an equation only has one quantity), and ordered last
+    # individually (a quantity only occurs in one equation)
+    #
     eids_first, qids_first, eids_last, qids_last, eids_inner, qids_inner, im_inner \
     = prefetch(im, eids=eids, qids=qids, )
     #
+    # Step 2: If there is a remaining core of interdependent equations, run
+    # a naive triangularization algorithm on it
+    #
     if im_inner.size > 0:
         eids_inner, qids_inner, im_inner, *_ \
         = triangularize_inner_block(im_inner, eids=eids_inner, qids=qids_inner, )
     #
+    # Combine the results
+    #
     eids = eids_first + eids_inner + eids_last
     qids = qids_first + qids_inner + qids_last
+    #
+    # Step 3: Create a tuple with a Block object for each block of
+    # equations and equantities
+    #
+    first_blocks = tuple(_Block(eid, qid, ) for eid, qid in zip(eids_first, qids_first, ))
+    inner_blocks = tuple(_generate_inner_blocks(im_inner, eids=eids_inner, qids=qids_inner, ))
+    last_blocks = tuple(_Block(eid, qid, ) for eid, qid in zip(eids_last, qids_last, ))
+    #
     info = {
         "eids_first": eids_first,
         "qids_first": qids_first,
         "eids_last": eids_last,
         "qids_last": qids_last,
         "eids_inner": eids_inner,
         "qids_inner": qids_inner,
         "im_inner": im_inner,
     }
-    first_blocks = tuple(_Block(eid, qid, ) for eid, qid in zip(eids_first, qids_first, ))
-    inner_blocks = tuple(_generate_inner_blocks(im_inner, eids=eids_inner, qids=qids_inner, ))
-    last_blocks = tuple(_Block(eid, qid, ) for eid, qid in zip(eids_last, qids_last, ))
     return first_blocks + inner_blocks + last_blocks, info
     #]
 
 
 def _generate_inner_blocks(
     im: _np.ndarray,
     eids: Iterable[int],
@@ -151,19 +165,19 @@
         if qids is None:
             qids = range(im.shape[1])
         eids = tuple(eids)
         qids = tuple(qids)
         #
         eids_first, qids_first, \
             eids_last, qids_last, \
-            eids_rem, qids_rem, inc_rem, \
-            = prefetch(inc, eids=eids, qids=qids, )
+            eids_rem, qids_rem, im_rem, \
+            = prefetch(im, eids=eids, qids=qids, )
         #
         fail = \
-            inc_rem.size or eids_rem or qids_rem \
+            im_rem.size or eids_rem or qids_rem \
             or eids_first != qids_first \
             or eids_last != qids_last
         if fail:
             _wrongdoings.IrisPieError("Cannot find strict sequential reordering", )
         return eids_first + eids_last
         #]
```

### Comparing `irispie-0.8.1/src/irispie/incidences/main.py` & `irispie-0.9.0/src/irispie/incidences/main.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/jacobians/_base.py` & `irispie-0.9.0/src/irispie/jacobians/_base.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/jacobians/steady.py` & `irispie-0.9.0/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/models/_flags.py` & `irispie-0.9.0/src/irispie/models/_flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/models/_get.py` & `irispie-0.9.0/src/irispie/models/_get.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 Quantities that are time series in model databanks
 """
 _TIME_SERIES_QUANTITY = _quantities.QuantityKind.VARIABLE | _quantities.QuantityKind.SHOCK
 
 
 _DATABANK_OUTPUT_FORMAT_RESOLUTION = {
     "dict": lambda x: x,
-    "Databank": lambda x: _databanks.Databank._from_dict(x),
-    "databank": lambda x: _databanks.Databank._from_dict(x),
+    "Databank": lambda x: _databanks.Databank.from_dict(x),
+    "databank": lambda x: _databanks.Databank.from_dict(x),
     "json": lambda x: js_.dumps(x),
     "json4": lambda x: js_.dumps(x, indent=4),
 }
 
 
 def _decorate_output_format(func: Callable, ):
     """
@@ -51,106 +51,104 @@
 
 
 class GetMixin:
     """
     Frontend getter methods for Model objects
     """
     #[
-    def _get_values_from_primary_variant(
-        self,
-        /,
-        variant_attr: Literal["levels"] | Literal["changes"],
-        kind: _quantities.QuantityKind,
-        **kwargs,
-    ) -> dict[str, Number]:
-        """
-        """
-        qid_to_name = self.create_qid_to_name()
-        qids = list(_quantities.generate_qids_by_kind(self._invariant._quantities, kind))
-        x = self._variants[0].retrieve_values(variant_attr, qids)
-        return {
-            qid_to_name[q]: float(x[i, 0])
-            for i, q in enumerate(qids)
-        }
-
     @_decorate_output_format
     def get_steady_levels(
         self,
         /,
         **kwargs,
     ) -> dict[str, Number]:
-        return self._get_values_from_primary_variant(variant_attr="levels", kind=_sources.LOGLY_VARIABLE, **kwargs, )
+        qids = _quantities.generate_qids_by_kind(self._invariant._quantities, _sources.LOGLY_VARIABLE, )
+        return self._get_values("levels", qids, **kwargs, )
 
     @_decorate_output_format
     def get_steady_changes(
         self,
         /,
         **kwargs,
     ) -> dict[str, Number]:
-        return self._get_values_from_primary_variant(variant_attr="changes", kind=_sources.LOGLY_VARIABLE, **kwargs, )
+        qids = _quantities.generate_qids_by_kind(self._invariant._quantities, _sources.LOGLY_VARIABLE, )
+        return self._get_values("changes", qids, **kwargs, )
 
     @_decorate_output_format
     def get_steady(
         self,
         /,
         **kwargs,
     ) -> dict[str, Number]:
-        levels = self._get_values_from_primary_variant(variant_attr="levels", kind=_sources.LOGLY_VARIABLE, **kwargs, )
-        changes = self._get_values_from_primary_variant(variant_attr="changes", kind=_sources.LOGLY_VARIABLE, **kwargs, )
-        return { k: (levels[k], changes[k]) for k in levels.keys() }
+        """
+        """
+        qids = tuple(_quantities.generate_qids_by_kind(self._invariant._quantities, _sources.LOGLY_VARIABLE, ))
+        levels = self._get_values("levels", qids, **kwargs, )
+        changes = self._get_values("changes", qids, **kwargs, )
+        if self.is_singleton:
+            out = {
+                k: (levels[k], changes[k], )
+                for k in levels.keys()
+            }
+        else:
+            out = { k: None for k in levels.keys() }
+            for k in levels.keys():
+                out[k] = list(zip(levels[k], changes[k]))
+        return out
 
     @_decorate_output_format
     def get_parameters(
         self,
         /,
         **kwargs,
     ) -> dict[str, Number]:
-        return self._get_values_from_primary_variant(variant_attr="levels", kind=_quantities.QuantityKind.PARAMETER)
+        qids = _quantities.generate_qids_by_kind(self._invariant._quantities, _quantities.QuantityKind.PARAMETER, )
+        return self._get_values("levels", qids, **kwargs, )
 
     @_decorate_output_format
     def get_stds(
         self,
         /,
         **kwargs,
     ) -> dict[str, Number]:
-        return self._get_values_from_primary_variant(variant_attr="levels", kind=_quantities.QuantityKind.STD)
+        qids = _quantities.generate_qids_by_kind(self._invariant._quantities, _quantities.QuantityKind.STD, )
+        return self._get_values("levels", qids, **kwargs, )
 
     @_decorate_output_format
     def get_parameters_stds(
         self,
         /,
         **kwargs,
     ) -> dict[str, Number]:
-        return self._get_values_from_primary_variant(variant_attr="levels", kind=_quantities.QuantityKind.PARAMETER_OR_STD)
+        qids = _quantities.generate_qids_by_kind(self._invariant._quantities, _quantities.QuantityKind.PARAMETER_OR_STD, )
+        return self._get_values("levels", qids, **kwargs, )
 
     @_decorate_output_format
     def get_log_status(
         self,
         /,
-        **kwargs,
     ) -> dict[str, bool]:
         return {
             qty.human: qty.logly
             for qty in self._invariant._quantities
             if qty.kind in _sources.LOGLY_VARIABLE
         }
 
     def get_initials(
         self,
         /,
-        kind: Literal["required"] | Literal["discarded"] = "required",
     ) -> _incidence.Tokens:
         """
         Get required list of initial conditions
         """
         # Get the tokens of state vector with actual incidence in the
         # model, and lag them by one period to get initial conditions
         initial_tokens = [
             _incidence.Token(t.qid, t.shift-1)
-            for t in self._invariant._dynamic_descriptor.solution_vectors.get_initials(kind, )
+            for t in self._invariant.dynamic_descriptor.solution_vectors.get_initials()
         ]
         return _incidence.print_tokens(initial_tokens, self.create_qid_to_name(), )
 
     def _get_steady_databank(
         self,
         start_date: _dates.Dater,
         end_date: _dates.Dater,
@@ -169,31 +167,31 @@
         )
         #
         qid_to_kind = self.create_qid_to_kind()
         qid_to_name = {
             qid: (name if qid_to_kind[qid] in _TIME_SERIES_QUANTITY else "")
             for qid, name in self.create_qid_to_name().items()
         }
-        qid_to_descriptor = self.create_qid_to_descriptor()
+        qid_to_description = self.create_qid_to_description()
         #
-        return _databanks.Databank._from_array(
+        return _databanks.Databank.from_array(
             array, qid_to_name, start_date, 
             array_orientation="horizontal",
             interpret_dates="start_date",
-            qid_to_descriptor=qid_to_descriptor,
+            qid_to_description=qid_to_description,
         )
 
     def get_solution_vectors(self, /, ) -> _descriptors.SolutionVectors:
         """
         Get the solution vectors of the model
         """
-        return self._invariant._dynamic_descriptor.solution_vectors
+        return self._invariant.dynamic_descriptor.solution_vectors
 
     def get_all_solution_matrices(self, /, ):
-        return [ v.solution for v in self._variants ]
+        return tuple(v.solution for v in self._variants)
 
     def get_solution_matrices(self, /, ):
         return self._variants[0].solution
 
     def get_dynamic_equations(
         self,
         /,
@@ -232,9 +230,40 @@
         return self._invariant._flags
 
     def get_custom_functions(
         self,
         /,
     ) -> dict[str, Callable]:
         return self._invariant._function_context
+
+    def _get_values(
+        self,
+        variant_attr: Literal["levels", "changes"],
+        qids: Iterable[int],
+        /,
+        **kwargs,
+    ) -> dict[str, Any]:
+        """
+        """
+        custom_round = kwargs.pop("round", None, )
+        def apply(value: Number) -> Number:
+            value = float(value)
+            return round(value, custom_round) if custom_round is not None else value
+        #
+        if self.is_singleton:
+            def insert_value(out_dict, name, value):
+                out_dict[name] = apply(value)
+        else:
+            def insert_value(out_dict, name, value):
+                out_dict.setdefault(name, []).append(apply(value))
+        #
+        qids = tuple(qids)
+        qid_to_name = self.create_qid_to_name()
+        out_dict = {}
+        #
+        for v in self._variants:
+            values = v.retrieve_values(variant_attr, qids)
+            for qid, value in zip(qids, values):
+                insert_value(out_dict, qid_to_name[qid], value)
+        return out_dict
     #]
```

### Comparing `irispie-0.8.1/src/irispie/models/_simulate.py` & `irispie-0.9.0/src/irispie/models/_simulate.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,30 @@
         /,
         anticipate: bool = True,
         deviation: bool = False,
         prepend_input: bool = True,
     ) -> _databanks.Databank:
         """
         """
+
         dataslabs = tuple(
             _dataslabs.Dataslab.from_databank_for_simulation(self, in_databank, base_range, column=i, )
             for i in range(self.num_variants)
         )
 
+        qid_to_logly = self.create_qid_to_logly()
+        boolex_logly = tuple(
+            qid_to_logly[qid] or False
+            for qid in range(dataslabs[0].num_rows)
+        )
+
         for variant, dataslab in zip(self._variants, dataslabs):
             new_data = dataslab.copy_data()
             new_data = _simulators.simulate_flat(
-                variant.solution, self.get_solution_vectors(),
+                variant.solution, self.get_solution_vectors(), boolex_logly,
                 new_data, dataslab.base_columns, deviation, anticipate,
             )
             dataslab.data = new_data
             dataslab.remove_columns(dataslab.base_columns[-1] - dataslab.num_ext_periods + 1)
 
         out_databank = _dataslabs.multiple_to_databank(dataslabs)
         if prepend_input:
```

### Comparing `irispie-0.8.1/src/irispie/models/_steady.py` & `irispie-0.9.0/src/irispie/models/_steady.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,88 +2,83 @@
 """
 
 
 #[
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-import functools as _ft
-import numpy as _np
-import itertools as _it
 from numbers import (Number, )
 from collections.abc import (Iterable, Callable, )
 from typing import (TypeAlias, Any, Literal, )
+import copy as _copy
+import functools as _ft
+import itertools as _it
+import numpy as _np
+import scipy as _sp
 
 from .. import equations as _eq
-from .. import quantities as _qu
-from .. import wrongdoings as _wd
+from .. import quantities as _quantities
+from .. import wrongdoings as _wrongdoings
 from ..fords import steadiers as _fs
-from ..evaluators import steady as _es
+from ..evaluators import steady as _evaluators
 
 from . import variants as _variants
 from . import _flags
 #]
 
 
-_SteadySolverReturn: TypeAlias = tuple[
-    _np.ndarray, tuple[int], _np.ndarray, tuple[int],
-]
-
-_EquationSwitch: TypeAlias = Literal["steady"] | Literal["dynamic"]
-
-
 class SteadyMixin:
     """
     """
     def steady(
         self,
         /,
-        **kwargs, 
+        **kwargs,
     ) -> list[dict]:
         """
         Calculate steady state for each Variant within this Model
         """
         model_flags = _flags.Flags.update_from_kwargs(self.get_flags(), **kwargs)
         solver = self._choose_steady_solver(model_flags.is_linear, model_flags.is_flat, )
-        info = tuple({} for _ in self._variants)
-        for i, v in enumerate(self._variants):
-            levels, qids_levels, changes, qids_changes = solver(v, model_flags, )
-            v.update_levels_from_array(levels, qids_levels, )
-            v.update_changes_from_array(changes, qids_changes, )
+        info = tuple(
+            solver(v, model_flags, **kwargs, )
+            for v in self._variants
+        )
         return info
 
-
     def _steady_linear(
         self, 
         variant: _variants.Variant,
         model_flags: _flags.Flags,
         /,
+        *,
         algorithm: Callable,
-    ) -> _SteadySolverReturn:
+        **kwargs,
+    ) -> dict[str, Any]:
         """
         """
         #
         # Calculate first-order system for steady equations for this variant
         system = self._systemize(
             variant,
-            self._invariant._steady_descriptor,
+            self._invariant.steady_descriptor,
             model_flags,
         )
         #
         #=======================================================================
         # Core algorithm: Calculate steady state for this variant
         Xi, Y, dXi, dY = algorithm(system)
         levels = _np.hstack(( Xi.flat, Y.flat )).flatten()
         changes = _np.hstack(( dXi.flat, dY.flat )).flatten()
         #=======================================================================
         #
-        # Extract only tokens with zero shift
+        # From first-order state space, extract only tokens with zero shift
         tokens = tuple(_it.chain(
-            self._invariant._steady_descriptor.system_vectors.transition_variables,
-            self._invariant._steady_descriptor.system_vectors.measurement_variables,
+            self._invariant.steady_descriptor.system_vectors.transition_variables,
+            self._invariant.steady_descriptor.system_vectors.measurement_variables,
         ))
         #
         # True for tokens with zero shift, e.g. [True, False, True, ... ]
         zero_shift_index = [ not t.shift for t in tokens ]
         #
         # Extract steady levels for quantities with zero shift
         levels = levels[zero_shift_index]
@@ -91,39 +86,109 @@
         qids = tuple(t.qid for t in _it.compress(tokens, zero_shift_index))
         #
         # Delogarithmize when needed
         qid_to_logly = self.create_qid_to_logly()
         levels = _apply_delog_on_vector(levels, qids, qid_to_logly)
         changes = _apply_delog_on_vector(changes, qids, qid_to_logly)
         #
-        return levels, qids, changes, qids
-
-    _steady_linear_flat = _ft.partialmethod(_steady_linear, algorithm=_fs.solve_steady_linear_flat)
-    _steady_linear_nonflat = _ft.partialmethod(_steady_linear, algorithm=_fs.solve_steady_linear_nonflat)
-
-
-    def _steady_nonlinear_flat(
-        self,
-        variant: _variants.Variant,
-        /,
-    ) -> _SteadySolverReturn:
-        """
-        """
-        return None, None, None, None
+        v.update_levels_from_array(levels, qids, )
+        v.update_changes_from_array(changes, qids, )
+        #
+        info = {}
+        return info
 
+    _steady_linear_flat = _ft.partialmethod(
+        _steady_linear,
+        algorithm=_fs.solve_steady_linear_flat,
+    )
+
+    _steady_linear_nonflat = _ft.partialmethod(
+        _steady_linear,
+        algorithm=_fs.solve_steady_linear_nonflat,
+    )
 
-    def _steady_nonlinear_nonflat(
+    def _steady_nonlinear(
         self,
         variant: _variants.Variant,
+        model_flags: _flags.Flags,
         /,
-    ) -> _SteadySolverReturn:
+        evaluator_class: type,
+        *,
+        fix: Iterable[str] | None = None,
+        fix_level: Iterable[str] | None = None,
+        fix_change: Iterable[str] | None = None,
+        optim_settings: dict[str, Any] | None = None,
+        iter_printer_settings: dict[str, Any] | None = None,
+        **kwargs,
+    ) -> None:
         """
         """
-        return None, None, None, None
+        optim_settings = \
+            _DEFAULT_OPTIM_SETTINGS if optim_settings is None \
+            else _DEFAULT_OPTIM_SETTINGS | optim_settings
+        #
+        # REFACTOR
+        #
+        wrt_equations = self.get_steady_equations()
+        fixable_quantities = \
+            self.get_quantities(kind=_quantities.QuantityKind.ENDOGENOUS_VARIABLE, )
+        wrt_qids_levels = \
+            _resolve_qids_fixed(fixable_quantities, fix, fix_level, )
+        wrt_qids_changes = \
+            _resolve_qids_fixed(fixable_quantities, fix, fix_change, )
+        steady_evaluator = evaluator_class(
+            wrt_equations,
+            self.get_quantities(),
+            wrt_qids_levels,
+            wrt_qids_changes,
+            variant,
+            iter_printer_settings=iter_printer_settings,
+        )
+        #
+        optim_result = _sp.optimize.root(
+           steady_evaluator.eval,
+           steady_evaluator.init_guess,
+           method="lm",
+           jac=True,
+           options=optim_settings,
+        )
+        #
+        steady_evaluator.iter_printer.print_footer()
+        #
+        final_guess = optim_result.x
+        func_norm = _sp.linalg.norm(optim_result.fun, 2, )
+        success = func_norm < optim_settings["ftol"]
+        if not success:
+            raise _wrongdoings.IrisPieError(
+                "Steady state calculations failed to converge"
+            )
+        #
+        levels, wrt_qids_levels = steady_evaluator.extract_levels(final_guess, )
+        variant.update_levels_from_array(levels, wrt_qids_levels, )
+        changes, wrt_qids_changes = steady_evaluator.extract_changes(final_guess, )
+        variant.update_changes_from_array(changes, wrt_qids_changes, )
+        #
+        info = {
+            "success": success,
+            "status": optim_result.status,
+            "num_func_evals": optim_result.nfev,
+            "num_jacob_evals": optim_result.njev,
+            "optim_result": optim_result,
+        }
+        return info
 
+    _steady_nonlinear_flat = _ft.partialmethod(
+        _steady_nonlinear,
+        evaluator_class=_evaluators.FlatSteadyEvaluator,
+    )
+
+    _steady_nonlinear_nonflat = _ft.partialmethod(
+        _steady_nonlinear,
+        evaluator_class=_evaluators.NonflatSteadyEvaluator,
+    )
 
     def _choose_steady_solver(
         self,
         is_linear: bool,
         is_flat: bool,
         /,
     ) -> Callable:
@@ -136,50 +201,53 @@
             case (False, True):
                 return self._steady_nonlinear_flat
             case (True, False):
                 return self._steady_linear_nonflat
             case (True, True):
                 return self._steady_linear_flat
 
-
     def check_steady(
         self,
         /,
-        equation_switch: _EquationSwitch = "dynamic",
-        when_fails: _wd.HOW = "error",
+        equation_switch: Literal["steady", "dynamic"] = "dynamic",
+        when_fails: _wrongdoings.HOW = "error",
         tolerance: float = 1e-12,
     ) -> tuple[bool, tuple[dict, ...]]:
         """
         Verify currently assigned steady state in dynamic or steady equations for each Variant within this Model
         """
         qid_to_logly = self.create_qid_to_logly()
         equator = self._choose_plain_equator(equation_switch)
         steady_arrays = (
             v.create_steady_array(
                 qid_to_logly,
                 num_columns=equator.min_num_columns + 1,
                 shift_in_first_column=equator.min_shift,
             ) for v in self._variants
         )
+        #
         # REFACTOR
+        #
         t_zero = -equator.min_shift
         dis = [ 
             _np.hstack((
                 equator.eval(x, t_zero, x[:, t_zero]),
                 equator.eval(x, t_zero+1, x[:, t_zero+1]),
             ))
             for x in steady_arrays
         ]
+        #
         # REFACTOR
+        #
         max_abs_dis = [ _np.max(_np.abs(d)) for d in dis ]
         status = [ d < tolerance for d in max_abs_dis ]
         all_status = all(status)
         if not all_status:
             message = "Invalid steady state"
-            _wd.throw(when_fails, message)
+            _wrongdoings.throw(when_fails, message)
         details = tuple(
             {"discrepancies": d, "max_abs_discrepancy": m, "is_valid": s}
             for d, m, s in zip(dis, max_abs_dis, status)
         )
         return all_status, details
 
 
@@ -194,7 +262,43 @@
     """
     logly_index = [ qid_to_logly[qid] for qid in qids ]
     vector = _np.copy(vector)
     if any(logly_index):
         vector[logly_index] = _np.exp(vector[logly_index])
     return vector
 
+def _resolve_qids_fixed(
+    fixable_quantities,
+    fix: Iterable[str] | str | None,
+    fix_spec: Iterable[str] | str | None,
+) -> tuple[int, ...]:
+    """
+    """
+    if fix is None:
+        fix = ()
+    elif isinstance(fix, str):
+        fix = (fix, )
+    if fix_spec is None:
+        fix_spec = ()
+    elif isinstance(fix_spec, str):
+        fix_spec = (fix_spec, )
+    fix = tuple(i for i in set(fix) | set(fix_spec) if not i.startswith("!"))
+    qids_fixed, invalid_names = \
+        _quantities.lookup_qids_by_name(fixable_quantities, fix, )
+    if invalid_names:
+        raise _wrongdoings.IrisPieError(
+            (f"Cannot fix these names:", ) + invalid_names
+        )
+    wrt_qids = tuple(
+        q.id
+        for q in fixable_quantities
+        if q.id not in qids_fixed
+    )
+    return wrt_qids
+
+
+_DEFAULT_OPTIM_SETTINGS = {
+    "ftol": 1e-12,
+    "xtol": 1e-12,
+    "gtol": 1e-12,
+}
+
```

### Comparing `irispie-0.8.1/src/irispie/models/invariants.py` & `irispie-0.9.0/src/irispie/models/invariants.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 
 
 #[
 from __future__ import annotations
 
 from typing import (Self, Callable, )
+import copy as _copy
 
 from .. import equations as _equations
 from .. import quantities as _quantities
 from .. import wrongdoings as _wrongdoings
 from ..fords import descriptors as _descriptors
 from ..equators import plain as _equators
 
@@ -28,18 +29,21 @@
     Invariant part of a Model object
     """
     #[
     __slots__ = (
         "_flags",
         "_function_context",
         "_quantities",
+        "shock_qid_to_std_qid",
         "_dynamic_equations",
         "_steady_equations",
-        "_dynamic_descriptor",
-        "_steady_descriptor",
+        "dynamic_descriptor",
+        "steady_descriptor",
+        "_plain_equator_for_dynamic_equations",
+        "_plain_equator_for_steady_equations",
         "_min_shift",
         "_max_shift",
     )
     def __init__(
         self,
         model_source,
         /,
@@ -49,28 +53,29 @@
     ) -> Self:
         """
         """
         self._flags = _flags.Flags.from_kwargs(**kwargs, )
         #
         self._populate_function_context(context)
         #
-        self._quantities = _cp.deepcopy(model_source.quantities, )
-        self._dynamic_equations = _cp_deepcopy(model_source.dynamic_equations, )
-        self._steady_equations = _cp.deepcopy(model_source.steady_equations, )
+        self._quantities = _copy.deepcopy(model_source.quantities, )
+        self.shock_qid_to_std_qid = _copy.deepcopy(model_source.shock_qid_to_std_qid, )
+        self._dynamic_equations = _copy.deepcopy(model_source.dynamic_equations, )
+        self._steady_equations = _copy.deepcopy(model_source.steady_equations, )
         #
         name_to_qid = _quantities.create_name_to_qid(self._quantities, )
         _equations.finalize_dynamic_equations(self._dynamic_equations, name_to_qid, )
         _equations.finalize_steady_equations(self._steady_equations, name_to_qid, )
         #
         if check_syntax:
             _check_syntax(self._dynamic_equations, self._function_context, )
             _check_syntax(self._steady_equations, self._function_context, )
         #
-        self._dynamic_descriptor = _descriptors.Descriptor(self._dynamic_equations, self._quantities, self._function_context, )
-        self._steady_descriptor = _descriptors.Descriptor(self._steady_equations, self._quantities, self._function_context, )
+        self.dynamic_descriptor = _descriptors.Descriptor(self._dynamic_equations, self._quantities, self._function_context, )
+        self.steady_descriptor = _descriptors.Descriptor(self._steady_equations, self._quantities, self._function_context, )
         #
         self._plain_equator_for_dynamic_equations = _equators.PlainEquator(
             _equations.generate_equations_of_kind( self._dynamic_equations, _PLAIN_EQUATOR_EQUATION, ),
             custom_functions=self._function_context,
         )
         #
         self._plain_equator_for_steady_equations = _equators.PlainEquator(
```

### Comparing `irispie-0.8.1/src/irispie/models/main.py` & `irispie-0.9.0/src/irispie/models/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 """
 """
 
 
 #[
 from __future__ import annotations
 
-from typing import (Self, TypeAlias, Literal, )
+from typing import (Self, Any, TypeAlias, Literal, )
 from collections.abc import (Iterable, Callable, )
 from numbers import (Number, )
 import copy as _co
 import numpy as _np
 import itertools as _it
 import functools as _ft
 
 from .. import equations as _equations
 from .. import quantities as _quantities
-from .. import wrongdoings as _wd
 from .. import sources as _sources
 from .. import dates as _dates
 from ..parsers import common as _pc
 from ..databanks import main as _databanks
-from ..fords import solutions as _sl
+from ..fords import solutions as _solutions
 from ..fords import steadiers as _fs
-from ..fords import descriptors as _de
-from ..fords import systems as _sy
+from ..fords import descriptors as _descriptors
+from ..fords import systems as _systems
+from .. import wrongdoings as _wrongdoings
 
 from . import variants as _variants
 from . import invariants as _invariants
-from . import _flags
-from . import _simulate
-from . import _steady
-from . import _get
+from . import _covariances as _covariances
+from . import _flags as _flags
+from . import _simulate as _simulate
+from . import _steady as _steady
+from . import _get as _get
 #]
 
 
-#[
 __all__ = [
     "Model"
 ]
 
 
-_SteadySolverReturn: TypeAlias = tuple[
-    _np.ndarray|None, Iterable[int]|None,
-    _np.ndarray|None, Iterable[int]|None,
-]
-
-
-_EquationSwitch: TypeAlias = Literal["dynamic"] | Literal["steady"]
-#]
-
-
 class Model(
     _sources.SourceMixin,
     _simulate.SimulateMixin,
     _steady.SteadyMixin,
+    _covariances.CoverianceMixin,
     _get.GetMixin,
 ):
     """
 
     """
     #[
     __slots__ = (
@@ -73,33 +64,25 @@
         self._invariant = None
         self._variants = None
 
     def assign(
         self,
         /,
         **kwargs,
-    ) -> Self:
+    ) -> None:
         """
         """
-        garbage_key = None
-        qid_to_value = _rekey_dict(kwargs, _quantities.create_name_to_qid(self._invariant._quantities))
-        for v in self._variants:
-            v.update_values_from_dict(qid_to_value)
+        name_to_qid = self.create_name_to_qid()
+        qid_to_name = self.create_qid_to_name()
         #
-        self._enforce_auto_values()
-        return self
-
-    def assign_from_databank(
-        self,
-        databank: _databanks.Databank,
-        /,
-    ) -> Self:
-        """
-        """
-        return self.assign(**databank.__dict__)
+        qid_to_value = _rekey_dict(kwargs, name_to_qid, )
+        for vid, variant in enumerate(self._variants, ):
+            qid_to_value_variant = _extract_dict_variant(qid_to_value, vid, qid_to_name, )
+            variant.update_values_from_dict(qid_to_value_variant, )
+            self._enforce_auto_values(variant, )
 
     def copy(self) -> Self:
         """
         Create a deep copy of the Model object
         """
         return _co.deepcopy(self)
 
@@ -119,14 +102,21 @@
         """
         if new_num < self.num_variants:
             self._shrink_num_variants(new_num, )
         elif new_num > self.num_variants:
             self._expand_num_variants(new_num, )
         return self
 
+    @property
+    def is_singleton(self, /, ) -> bool:
+        """
+        True for Models with only one variant
+        """
+        return self.num_variants == 1
+
     def change_logly(
         self,
         new_logly: bool,
         some_names: Iterable[str] | None = None,
         /
     ) -> None:
         """
@@ -166,19 +156,19 @@
 
     def create_qid_to_name(self, /, ) -> dict[int, str]:
         return _quantities.create_qid_to_name(self._invariant._quantities)
 
     def create_qid_to_kind(self, /, ) -> dict[int, str]:
         return _quantities.create_qid_to_kind(self._invariant._quantities)
 
-    def create_qid_to_descriptor(self, /, ) -> dict[int, str]:
+    def create_qid_to_description(self, /, ) -> dict[int, str]:
         """
         Create a dictionary mapping from quantity id to quantity descriptor
         """
-        return _quantities.create_qid_to_descriptor(self._invariant._quantities)
+        return _quantities.create_qid_to_description(self._invariant._quantities)
 
     def create_qid_to_logly(self, /, ) -> dict[int, bool]:
         """
         Create a dictionary mapping from quantity id to quantity log-status
         """
         return _quantities.create_qid_to_logly(self._invariant._quantities)
 
@@ -212,33 +202,33 @@
         deviation: bool,
         **kwargs,
     ) -> _np.ndarray:
         return {
             True: self.create_zero_array, False: self.create_steady_array,
         }[deviation](**kwargs)
 
-    def _enforce_auto_values(self, /, ) -> None:
+    def _enforce_auto_values(self, variant, /, ) -> None:
         """
         """
         #
         # Reset levels of shocks to zero, remove changes
         #
         assign_shocks = {
             qid: (0, _np.nan)
             for qid in _quantities.generate_qids_by_kind(self._invariant._quantities, _quantities.QuantityKind.SHOCK)
         }
-        self._variants[0].update_values_from_dict(assign_shocks)
+        variant.update_values_from_dict(assign_shocks)
         #
         # Remove changes from quantities that are not logly variables
         #
         assign_non_logly = {
             qid: (..., _np.nan)
-            for qid in  _quantities.generate_qids_by_kind(self._invariant._quantities, ~sources.LOGLY_VARIABLE)
+            for qid in _quantities.generate_qids_by_kind(self._invariant._quantities, ~_sources.LOGLY_VARIABLE)
         }
-        self._variants[0].update_values_from_dict(assign_non_logly)
+        variant.update_values_from_dict(assign_non_logly)
 
     def _shrink_num_variants(self, new_num: int, /, ) -> None:
         """
         """
         if new_num<1:
             raise Exception('Number of variants must be one or more')
         self._variants = self._variants[0:new_num]
@@ -249,46 +239,48 @@
         for i in range(self.num_variants, new_num):
             self._variants.append(_co.deepcopy(self._variants[-1]))
 
     def systemize(
         self,
         /,
         **kwargs,
-    ) -> Iterable[_sy.System]:
+    ) -> Iterable[_systems.System]:
         """
         Create unsolved first-order system for each variant
         """
         model_flags = self._invariant._flags.update_from_kwargs(**kwargs, )
-        return [
-            self._systemize(variant, self._invariant._dynamic_descriptor, model_flags, )
+        return tuple(
+            self._systemize(variant, self._invariant.dynamic_descriptor, model_flags, )
             for variant in self._variants
-        ]
+        )
 
     def _systemize(
         self,
         variant: _variants.Variant,
-        descriptor: _de.Descriptor,
+        descriptor: _descriptors.Descriptor,
         model_flags: flags.Flags,
         /,
-    ) -> _sy.System:
+    ) -> _systems.System:
         """
         Create unsolved first-order system for one variant
         """
         ac = descriptor.aldi_context
         num_columns = ac.shape_data[1]
         qid_to_logly = self.create_qid_to_logly()
         #
         if model_flags.is_linear:
-            data_array = variant.create_zero_array(qid_to_logly, num_columns=num_columns, shift_in_first_column=ac.min_shift)
+            data_array = variant.create_zero_array(qid_to_logly, num_columns=num_columns, shift_in_first_column=ac.min_shift, )
+            data_array_lagged = None
             steady_array = variant.create_steady_array(qid_to_logly, num_columns=1, ).reshape(-1)
         else:
-            data_array = variant.create_steady_array(qid_to_logly, num_columns=num_columns, )
+            data_array = variant.create_steady_array(qid_to_logly, num_columns=num_columns, shift_in_first_column=ac.min_shift, )
+            data_array_lagged = variant.create_steady_array(qid_to_logly, num_columns=num_columns, shift_in_first_column=ac.min_shift-1, )
             steady_array = data_array[:, -ac.min_shift]
         #
-        return _sy.System(descriptor, data_array, steady_array, )
+        return _systems.System(descriptor, data_array, steady_array, model_flags, data_array_lagged, )
 
     def solve(
         self,
         /,
         **kwargs,
     ) -> None:
         """
@@ -303,20 +295,20 @@
         variant: _variants.Variant,
         model_flags: flags.Flags,
         /,
     ) -> None:
         """
         Calculate first-order solution for one Variant of this Model
         """
-        system = self._systemize(variant, self._invariant._dynamic_descriptor, model_flags, )
-        variant.solution = _sl.Solution(self._invariant._dynamic_descriptor, system, )
+        system = self._systemize(variant, self._invariant.dynamic_descriptor, model_flags, )
+        variant.solution = _solutions.Solution(self._invariant.dynamic_descriptor, system, )
 
     def _choose_plain_equator(
         self,
-        equation_switch: _EquationSwitch,
+        equation_switch: Literal["dynamic", "steady", ],
         /,
     ) -> Callable | None:
         """
         """
         match equation_switch:
             case "dynamic":
                 return self._invariant._plain_equator_for_dynamic_equations
@@ -327,15 +319,19 @@
         self,
         default_std: Number | None = None,
         /,
     ) -> None:
         """
         """
         default_std = default_std if default_std is not None else _DEFAULT_STD_RESOLUTION(self.get_flags())
-        self.assign(**{ k: default_std for k in _quantities.generate_quantity_names_by_kind(self._invariant._quantities, _quantities.QuantityKind.STD) })
+        dict_to_assign = {
+            k: default_std
+            for k in _quantities.generate_quantity_names_by_kind(self._invariant._quantities, _quantities.QuantityKind.STD, )
+        }
+        self.assign(**dict_to_assign, )
 
     @classmethod
     def from_source(
         cls,
         source: _sources.AlgebraicSource,
         /,
         default_std: int | None = None,
@@ -348,18 +344,18 @@
         #
         self._invariant = _invariants.Invariant(
             source,
             context=context,
             **kwargs,
         )
         #
-        self._variants = [ _variants.Variant(self._invariant._quantities) ]
-        #
-        self._enforce_auto_values()
-        self._assign_default_stds(default_std)
+        self._variants = [ _variants.Variant(self._invariant._quantities, ) ]
+        for v in self._variants:
+            self._enforce_auto_values(v, )
+        self._assign_default_stds(default_std, )
         #
         return self
 
     def from_self(self, ) -> Self:
         """
         Create a new Model object with pointers to invariant and variants of this Model object
         """
@@ -373,29 +369,29 @@
     #
 
     def get_min_max_shifts(self) -> tuple[int, int]:
         """
         """
         return self._invariant._min_shift, self._invariant._max_shift
 
-    def get_databank_names(self, /, ) -> list[str]:
+    def get_databank_names(self, plan, /, ) -> tuple[str, ...]:
         qid_to_name = self.create_qid_to_name()
-        return [ qid_to_name[qid] for qid in range(len(qid_to_name)) ]
+        return tuple(qid_to_name[qid] for qid in range(len(qid_to_name)))
     #]
 
 
 _DEFAULT_STD_LINEAR = 1
 _DEFAULT_STD_NONLINEAR = 0.01
 _DEFAULT_STD_RESOLUTION = lambda flags: {
     True: _DEFAULT_STD_LINEAR,
     False: _DEFAULT_STD_NONLINEAR,
 }[flags.is_linear]
 
 
-def _rekey_dict(dict_to_rekey: dict, old_key_to_new_key: dict, /, garbage_key=None) -> dict:
+def _rekey_dict(dict_to_rekey: dict, old_key_to_new_key: dict, /, garbage_key=None, ) -> dict:
     #[
     new_dict = {
         old_key_to_new_key.get(key, garbage_key): value
         for key, value in dict_to_rekey.items()
     }
     if garbage_key in new_dict:
         del new_dict[garbage_key]
@@ -412,7 +408,37 @@
     elif isinstance(variants, slice):
         return range(*variants.indices(self.num_variants))
     else:
         return [v for v in variants]
     #]
 
 
+def _extract_dict_variant(
+    qid_to_value: dict[int, Any],
+    vid: int,
+    qid_to_name: dict[int, str],
+    /,
+) -> dict[int, tuple[Number|Ellipsis, Number|Ellipsis]]:
+    """
+    """
+    def _extract_value_variant(
+        value: list | tuple | Number,
+        name: str,
+        /,
+    ) -> tuple[Number|Ellipsis, Number|Ellipsis]:
+        """
+        """
+        if isinstance(value, Iterable, ) and not isinstance(value, str, ) and not isinstance(value, tuple, ):
+            value = list(value, )[vid]
+        if isinstance(value, Number, ) or value is Ellipsis:
+            value = (value, Ellipsis, )
+        if not isinstance(value, tuple, ) or len(value) != 2:
+            raise _wrongdoings.IrisPieError(
+                f"Invalid type of value assigned to this Model quantity: \"{name}\"",
+            )
+        return value
+        #
+    return {
+        qid: _extract_value_variant(value, qid_to_name[qid], )
+        for qid, value in qid_to_value.items()
+    }
+
```

### Comparing `irispie-0.8.1/src/irispie/models/variants.py` & `irispie-0.9.0/src/irispie/models/variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,26 +53,28 @@
         self.levels = _update_from_array(self.levels, levels, qids, )
 
     def update_changes_from_array(self, changes: _np.ndarray, qids: Iterable[int], /, ) -> None:
         self.changes = _update_from_array(self.changes, changes, qids, )
 
     def retrieve_values(
         self,
-        attr: Literal["levels"] | Literal["changes"],
-        qids: Iterable[int]|None = None,
+        attr: Literal["levels", "changes"],
+        qids: Iterable[int] | None = None,
         /,
     ) -> _np.ndarray:
-        values = _np.copy(getattr(self, attr)).reshape(-1, 1)
+        # values = _np.copy(getattr(self, attr)).reshape(-1, 1)
+        values = _np.copy(getattr(self, attr, ), )
+        qids = list(qids, )
         return values[qids] if qids is not None else values
 
     def retrieve_maybelog_values_for_qids(
         self,
         qids: Iterable[int],
         qid_to_logly: dict[int, bool],
-    ) -> tuple[_np.ndarray, _np.ndarray, ]:
+    ) -> tuple[_np.ndarray, ..., ]:
         """
         """
         qids = list(qids)
         index_logly = list(_quantities.generate_index_logly(qids, qid_to_logly, ))
         #
         # Extract initial guesses for levels and changes
         maybelog_levels = self.levels[qids].flatten()
```

### Comparing `irispie-0.8.1/src/irispie/parsers/algebraic.py` & `irispie-0.9.0/src/irispie/parsers/algebraic.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/parsers/common.py` & `irispie-0.9.0/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/parsers/preparser.py` & `irispie-0.9.0/src/irispie/parsers/preparser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/parsers/pseudofunctions.py` & `irispie-0.9.0/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/parsers/substitutions.py` & `irispie-0.9.0/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/plans/main.py` & `irispie-0.9.0/src/irispie/plans/main.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/sequentials/_simulate.py` & `irispie-0.9.0/src/irispie/sequentials/_simulate.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/sequentials/main.py` & `irispie-0.9.0/src/irispie/sequentials/main.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/series/_conversion.py` & `irispie-0.9.0/src/irispie/series/_conversion.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/series/_hp.py` & `irispie-0.9.0/src/irispie/series/_hp.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/series/_plotly.py` & `irispie-0.9.0/src/irispie/series/_plotly.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/src/irispie/series/_x13.py` & `irispie-0.9.0/src/irispie/series/_x13.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def x13(
         self,
         *,
         range: _dates.Ranger | EllipsisType = ...,
         when_error: _wrongdoings.HOW = "warning",
         clean_up: bool = True,
         output: str = "sa",
-        mode: Literal["mult"] | Literal["add"] | Literal["pseudoadd"] | Literal["logadd"] = "mult",
+        mode: Literal["mult", "add", "pseudoadd", "logadd", ] = "mult",
         **kwargs,
     ) -> tuple[Self, dict]:
         """
         """
         range = tuple(self._resolve_dates(range))
         base_start_date = range[0]
         settings = _create_settings(base_start_date, output, mode, **kwargs, )
@@ -186,15 +186,15 @@
     return start_date + num_leading, column_data, slice(num_leading, num_rows-num_trailing, )
     #]
 
 
 def _create_settings(
     base_start_date: _dates.Date,
     output: str,
-    mode: Literal["mult"] | Literal["add"] | Literal["pseudoadd"] | Literal["logadd"],
+    mode: Literal["mult", "add", "pseudoadd", "logadd", ],
     /,
     transform_function: str = "none",
 ) ->  dict[str, str]:
     """
     """
     #[
     if str(mode) == "mult" and str(transform_function) == "none":
```

### Comparing `irispie-0.8.1/src/irispie/series/main.py` & `irispie-0.9.0/src/irispie/series/main.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/tests/series/shift_test.py` & `irispie-0.9.0/tests/series/shift_test.py`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/LICENCE` & `irispie-0.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.8.1/pyproject.toml` & `irispie-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.8.1"
+    version = "0.9.0"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
```

### Comparing `irispie-0.8.1/PKG-INFO` & `irispie-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.8.1
+Version: 0.9.0
 Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
 Keywords: dsge,economics,forecasting,macroeconomics,modeling,simulation
 Classifier: License :: OSI Approved :: MIT License
```

