# Comparing `tmp/cfgrib-0.9.9.0.tar.gz` & `tmp/cfgrib-0.9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgrib-0.9.9.0.tar", last modified: Fri Apr  9 09:56:12 2021, max compression
+gzip compressed data, was "cfgrib-0.9.9.1.tar", last modified: Wed Sep 29 09:08:47 2021, max compression
```

## Comparing `cfgrib-0.9.9.0.tar` & `cfgrib-0.9.9.1.tar`

### file list

```diff
@@ -1,120 +1,117 @@
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.684836 cfgrib-0.9.9.0/
--rw-r--r--   0 amici      (501) staff       (20)      118 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/.dockerignore
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.649241 cfgrib-0.9.9.0/.github/
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.660125 cfgrib-0.9.9.0/.github/workflows/
--rw-r--r--   0 amici      (501) staff       (20)     3084 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/.github/workflows/on-push.yml
--rw-r--r--   0 amici      (501) staff       (20)     1344 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/.github/workflows/weekly.yml
--rw-r--r--   0 amici      (501) staff       (20)      857 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/.gitignore
--rw-r--r--   0 amici      (501) staff       (20)    11295 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/CHANGELOG.rst
--rw-r--r--   0 amici      (501) staff       (20)     4334 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/CONTRIBUTING.rst
--rw-r--r--   0 amici      (501) staff       (20)      607 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/Dockerfile
--rw-r--r--   0 amici      (501) staff       (20)    11357 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/LICENSE
--rw-r--r--   0 amici      (501) staff       (20)      497 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/MANIFEST.in
--rw-r--r--   0 amici      (501) staff       (20)     2697 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/Makefile
--rw-r--r--   0 amici      (501) staff       (20)    56466 2021-04-09 09:56:12.685156 cfgrib-0.9.9.0/PKG-INFO
--rw-r--r--   0 amici      (501) staff       (20)    34729 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/README.rst
--rw-r--r--   0 amici      (501) staff       (20)      289 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/appveyor.yml
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.661027 cfgrib-0.9.9.0/cf2cdm/
--rw-r--r--   0 amici      (501) staff       (20)      751 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cf2cdm/__init__.py
--rw-r--r--   0 amici      (501) staff       (20)     6599 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cf2cdm/cfcoords.py
--rw-r--r--   0 amici      (501) staff       (20)     2485 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cf2cdm/cfunits.py
--rw-r--r--   0 amici      (501) staff       (20)     1850 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cf2cdm/datamodels.py
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.663087 cfgrib-0.9.9.0/cfgrib/
--rw-r--r--   0 amici      (501) staff       (20)     1046 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/__init__.py
--rw-r--r--   0 amici      (501) staff       (20)     2973 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/__main__.py
--rw-r--r--   0 amici      (501) staff       (20)     5747 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/cfmessage.py
--rw-r--r--   0 amici      (501) staff       (20)    26633 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/dataset.py
--rw-r--r--   0 amici      (501) staff       (20)    15974 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/messages.py
--rw-r--r--   0 amici      (501) staff       (20)     5177 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/xarray_plugin.py
--rw-r--r--   0 amici      (501) staff       (20)     4219 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/xarray_store.py
--rw-r--r--   0 amici      (501) staff       (20)    10560 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/cfgrib/xarray_to_grib.py
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.664851 cfgrib-0.9.9.0/cfgrib.egg-info/
--rw-r--r--   0 amici      (501) staff       (20)    56466 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/PKG-INFO
--rw-r--r--   0 amici      (501) staff       (20)     3022 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/SOURCES.txt
--rw-r--r--   0 amici      (501) staff       (20)        1 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/dependency_links.txt
--rw-r--r--   0 amici      (501) staff       (20)      118 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/entry_points.txt
--rw-r--r--   0 amici      (501) staff       (20)      124 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/requires.txt
--rw-r--r--   0 amici      (501) staff       (20)       14 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/top_level.txt
--rw-r--r--   0 amici      (501) staff       (20)        1 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/cfgrib.egg-info/zip-safe
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.667436 cfgrib-0.9.9.0/ci/
--rw-r--r--   0 amici      (501) staff       (20)     3150 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/install_python.ps1
--rw-r--r--   0 amici      (501) staff       (20)      123 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-dev.txt
--rw-r--r--   0 amici      (501) staff       (20)       27 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-docs.in
--rw-r--r--   0 amici      (501) staff       (20)     1342 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-docs.txt
--rw-r--r--   0 amici      (501) staff       (20)      145 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-docs.yml
--rw-r--r--   0 amici      (501) staff       (20)      265 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-py36-old.yml
--rw-r--r--   0 amici      (501) staff       (20)      276 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-py36-qc.yml
--rw-r--r--   0 amici      (501) staff       (20)      212 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-py36-without-xarray.yml
--rw-r--r--   0 amici      (501) staff       (20)      242 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-py37.yml
--rw-r--r--   0 amici      (501) staff       (20)       97 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-tests.in
--rw-r--r--   0 amici      (501) staff       (20)     1265 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/ci/requirements-tests.txt
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.669010 cfgrib-0.9.9.0/docs/
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.669229 cfgrib-0.9.9.0/docs/_static/
--rw-r--r--   0 amici      (501) staff       (20)        0 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/_static/.gitkeep
--rw-r--r--   0 amici      (501) staff       (20)       95 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/cfmessage.rst
--rw-r--r--   0 amici      (501) staff       (20)     5408 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/conf.py
--rw-r--r--   0 amici      (501) staff       (20)       93 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/dataset.rst
--rw-r--r--   0 amici      (501) staff       (20)     2469 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/index.rst
--rw-r--r--   0 amici      (501) staff       (20)       86 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/messages.rst
--rw-r--r--   0 amici      (501) staff       (20)      110 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/xarray_store.rst
--rw-r--r--   0 amici      (501) staff       (20)       84 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/docs/xarray_to_grib.rst
--rw-r--r--   0 amici      (501) staff       (20)      128 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/environment-minimal.in.yml
--rw-r--r--   0 amici      (501) staff       (20)      185 2021-04-09 09:56:11.000000 cfgrib-0.9.9.0/environment.in.yml
--rw-r--r--   0 amici      (501) staff       (20)  2361600 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/era5-levels-members.grib
--rw-r--r--   0 amici      (501) staff       (20)  1200165 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/nam.t00z.awp21100.tm00.grib2
--rw-r--r--   0 amici      (501) staff       (20)      218 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/pyproject.toml
--rw-r--r--   0 amici      (501) staff       (20)      159 2021-04-09 09:56:12.685600 cfgrib-0.9.9.0/setup.cfg
--rw-r--r--   0 amici      (501) staff       (20)     2926 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/setup.py
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.674965 cfgrib-0.9.9.0/tests/
--rw-r--r--   0 amici      (501) staff       (20)      903 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/cds_test_00_sync_sample_data.py
--rw-r--r--   0 amici      (501) staff       (20)     3379 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/cds_test_10_era5.py
--rw-r--r--   0 amici      (501) staff       (20)     5421 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/cds_test_20_sf_ecmwf.py
--rw-r--r--   0 amici      (501) staff       (20)     5060 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/cds_test_20_sf_meteo_france.py
--rw-r--r--   0 amici      (501) staff       (20)     4964 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/cds_test_20_sf_ukmo.py
--rw-r--r--   0 amici      (501) staff       (20)      824 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/cdscommon.py
--rw-r--r--   0 amici      (501) staff       (20)     1117 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-macos-3.8.yml
--rw-r--r--   0 amici      (501) staff       (20)     1131 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-ubuntu-3.6.yml
--rw-r--r--   0 amici      (501) staff       (20)     1131 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-ubuntu-3.7.yml
--rw-r--r--   0 amici      (501) staff       (20)     1130 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-ubuntu-3.8.yml
--rw-r--r--   0 amici      (501) staff       (20)     1047 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-ubuntu-3.9-minimal.yml
--rw-r--r--   0 amici      (501) staff       (20)     1712 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-ubuntu-3.9.yml
--rw-r--r--   0 amici      (501) staff       (20)     1012 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/environment-windows-3.8.yml
-drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-04-09 09:56:12.684592 cfgrib-0.9.9.0/tests/sample-data/
--rw-r--r--   0 amici      (501) staff       (20)    44136 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/era5-levels-corrupted.grib
--rw-r--r--   0 amici      (501) staff       (20)  2361600 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/era5-levels-members.grib
--rw-r--r--   0 amici      (501) staff       (20)     9960 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/fields_with_missing_values.grib
--rw-r--r--   0 amici      (501) staff       (20)    80640 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/forecast_monthly_ukmo.grib
--rw-r--r--   0 amici      (501) staff       (20)    20400 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/hpa_and_pa.grib
--rw-r--r--   0 amici      (501) staff       (20)    56880 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/lambert_grid.grib
--rw-r--r--   0 amici      (501) staff       (20)   103680 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/multi_param_on_multi_dims.grib
--rw-r--r--   0 amici      (501) staff       (20)    13680 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/reduced_gg.grib
--rw-r--r--   0 amici      (501) staff       (20)    14244 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_gg_ml.grib
--rw-r--r--   0 amici      (501) staff       (20)   311400 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_gg_ml_g2.grib
--rw-r--r--   0 amici      (501) staff       (20)    18600 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_gg_pl.grib
--rw-r--r--   0 amici      (501) staff       (20)    18600 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_gg_sfc.grib
--rw-r--r--   0 amici      (501) staff       (20)    55475 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_gg_wrong_increment.grib
--rw-r--r--   0 amici      (501) staff       (20)   114212 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_ll_msl.grib
--rw-r--r--   0 amici      (501) staff       (20)     2772 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_ll_sfc.grib
--rw-r--r--   0 amici      (501) staff       (20)     8171 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/regular_ll_wrong_increment.grib
--rw-r--r--   0 amici      (501) staff       (20)     8100 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/scanning_mode_64.grib
--rw-r--r--   0 amici      (501) staff       (20)     1440 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/single_gridpoint.grib
--rw-r--r--   0 amici      (501) staff       (20)     9360 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/spherical_harmonics.grib
--rw-r--r--   0 amici      (501) staff       (20)     8160 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/t_analysis_and_fc_0.grib
--rw-r--r--   0 amici      (501) staff       (20)     4080 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/t_on_different_level_types.grib
--rw-r--r--   0 amici      (501) staff       (20)     7200 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/tp_on_different_grid_resolutions.grib
--rw-r--r--   0 amici      (501) staff       (20)    23040 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/sample-data/uv_on_different_levels.grib
--rw-r--r--   0 amici      (501) staff       (20)      309 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_10_cfunits.py
--rw-r--r--   0 amici      (501) staff       (20)     4987 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_20_cfcoords.py
--rw-r--r--   0 amici      (501) staff       (20)      367 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_20_main.py
--rw-r--r--   0 amici      (501) staff       (20)     1334 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_20_main_commands.py
--rw-r--r--   0 amici      (501) staff       (20)     6879 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_20_messages.py
--rw-r--r--   0 amici      (501) staff       (20)     2376 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_25_cfmessage.py
--rw-r--r--   0 amici      (501) staff       (20)     7608 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_30_dataset.py
--rw-r--r--   0 amici      (501) staff       (20)     2348 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_40_xarray_store.ipynb
--rw-r--r--   0 amici      (501) staff       (20)     3295 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_40_xarray_store.py
--rw-r--r--   0 amici      (501) staff       (20)     2092 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_40_xarray_to_grib_regular_ll.py
--rw-r--r--   0 amici      (501) staff       (20)     1805 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_50_datamodels.py
--rw-r--r--   0 amici      (501) staff       (20)     2519 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_50_sample_data.py
--rw-r--r--   0 amici      (501) staff       (20)     2267 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_50_xarray_getitem.py
--rw-r--r--   0 amici      (501) staff       (20)      962 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tests/test_50_xarray_plugin.py
--rw-r--r--   0 amici      (501) staff       (20)      703 2021-04-09 09:56:12.000000 cfgrib-0.9.9.0/tox.ini
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.965138 cfgrib-0.9.9.1/
+-rw-r--r--   0 amici      (501) staff       (20)      118 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/.dockerignore
+-rw-r--r--   0 amici      (501) staff       (20)    11665 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/CHANGELOG.rst
+-rw-r--r--   0 amici      (501) staff       (20)     4334 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 amici      (501) staff       (20)      607 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/Dockerfile
+-rw-r--r--   0 amici      (501) staff       (20)    11357 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/LICENSE
+-rw-r--r--   0 amici      (501) staff       (20)      497 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/MANIFEST.in
+-rw-r--r--   0 amici      (501) staff       (20)     2697 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/Makefile
+-rw-r--r--   0 amici      (501) staff       (20)    57062 2021-09-29 09:08:47.965452 cfgrib-0.9.9.1/PKG-INFO
+-rw-r--r--   0 amici      (501) staff       (20)    34859 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/README.rst
+-rw-r--r--   0 amici      (501) staff       (20)      289 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/appveyor.yml
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.937528 cfgrib-0.9.9.1/cf2cdm/
+-rw-r--r--   0 amici      (501) staff       (20)      751 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cf2cdm/__init__.py
+-rw-r--r--   0 amici      (501) staff       (20)     6599 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cf2cdm/cfcoords.py
+-rw-r--r--   0 amici      (501) staff       (20)     2485 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cf2cdm/cfunits.py
+-rw-r--r--   0 amici      (501) staff       (20)     1850 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cf2cdm/datamodels.py
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.940129 cfgrib-0.9.9.1/cfgrib/
+-rw-r--r--   0 amici      (501) staff       (20)     1046 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/__init__.py
+-rw-r--r--   0 amici      (501) staff       (20)     2973 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/__main__.py
+-rw-r--r--   0 amici      (501) staff       (20)      513 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/abc.py
+-rw-r--r--   0 amici      (501) staff       (20)     5666 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/cfmessage.py
+-rw-r--r--   0 amici      (501) staff       (20)    27160 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/dataset.py
+-rw-r--r--   0 amici      (501) staff       (20)    15924 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/messages.py
+-rw-r--r--   0 amici      (501) staff       (20)     5261 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/xarray_plugin.py
+-rw-r--r--   0 amici      (501) staff       (20)     4219 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/xarray_store.py
+-rw-r--r--   0 amici      (501) staff       (20)    10537 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib/xarray_to_grib.py
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.941846 cfgrib-0.9.9.1/cfgrib.egg-info/
+-rw-r--r--   0 amici      (501) staff       (20)    57062 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/PKG-INFO
+-rw-r--r--   0 amici      (501) staff       (20)     3019 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/SOURCES.txt
+-rw-r--r--   0 amici      (501) staff       (20)        1 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/dependency_links.txt
+-rw-r--r--   0 amici      (501) staff       (20)      118 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/entry_points.txt
+-rw-r--r--   0 amici      (501) staff       (20)      127 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/requires.txt
+-rw-r--r--   0 amici      (501) staff       (20)       14 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/top_level.txt
+-rw-r--r--   0 amici      (501) staff       (20)        1 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/cfgrib.egg-info/zip-safe
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.944461 cfgrib-0.9.9.1/ci/
+-rw-r--r--   0 amici      (501) staff       (20)     3150 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/install_python.ps1
+-rw-r--r--   0 amici      (501) staff       (20)      123 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-dev.txt
+-rw-r--r--   0 amici      (501) staff       (20)       27 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-docs.in
+-rw-r--r--   0 amici      (501) staff       (20)     1342 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-docs.txt
+-rw-r--r--   0 amici      (501) staff       (20)      145 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-docs.yml
+-rw-r--r--   0 amici      (501) staff       (20)      265 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-py36-old.yml
+-rw-r--r--   0 amici      (501) staff       (20)      276 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-py36-qc.yml
+-rw-r--r--   0 amici      (501) staff       (20)      212 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-py36-without-xarray.yml
+-rw-r--r--   0 amici      (501) staff       (20)      242 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-py37.yml
+-rw-r--r--   0 amici      (501) staff       (20)       97 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-tests.in
+-rw-r--r--   0 amici      (501) staff       (20)     1265 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/ci/requirements-tests.txt
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.945991 cfgrib-0.9.9.1/docs/
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.946205 cfgrib-0.9.9.1/docs/_static/
+-rw-r--r--   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/_static/.gitkeep
+-rw-r--r--   0 amici      (501) staff       (20)       95 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/cfmessage.rst
+-rw-r--r--   0 amici      (501) staff       (20)     5408 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/conf.py
+-rw-r--r--   0 amici      (501) staff       (20)       93 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/dataset.rst
+-rw-r--r--   0 amici      (501) staff       (20)     2469 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/index.rst
+-rw-r--r--   0 amici      (501) staff       (20)       86 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/messages.rst
+-rw-r--r--   0 amici      (501) staff       (20)      110 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/xarray_store.rst
+-rw-r--r--   0 amici      (501) staff       (20)       84 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/docs/xarray_to_grib.rst
+-rw-r--r--   0 amici      (501) staff       (20)      144 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/environment-minimal.in.yml
+-rw-r--r--   0 amici      (501) staff       (20)      202 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/environment-minver.in.yml
+-rw-r--r--   0 amici      (501) staff       (20)      225 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/environment.in.yml
+-rw-r--r--   0 amici      (501) staff       (20)  2361600 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/era5-levels-members.grib
+-rw-r--r--   0 amici      (501) staff       (20)  1200165 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/nam.t00z.awp21100.tm00.grib2
+-rw-r--r--   0 amici      (501) staff       (20)      218 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/pyproject.toml
+-rw-r--r--   0 amici      (501) staff       (20)      178 2021-09-29 09:08:47.965967 cfgrib-0.9.9.1/setup.cfg
+-rw-r--r--   0 amici      (501) staff       (20)     2929 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/setup.py
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.953094 cfgrib-0.9.9.1/tests/
+-rw-r--r--   0 amici      (501) staff       (20)      903 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/cds_test_00_sync_sample_data.py
+-rw-r--r--   0 amici      (501) staff       (20)     3379 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/cds_test_10_era5.py
+-rw-r--r--   0 amici      (501) staff       (20)     5421 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/cds_test_20_sf_ecmwf.py
+-rw-r--r--   0 amici      (501) staff       (20)     5060 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/cds_test_20_sf_meteo_france.py
+-rw-r--r--   0 amici      (501) staff       (20)     4964 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/cds_test_20_sf_ukmo.py
+-rw-r--r--   0 amici      (501) staff       (20)      914 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/cdscommon.py
+-rw-r--r--   0 amici      (501) staff       (20)     1576 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/environment-macos-3.8.yml
+-rw-r--r--   0 amici      (501) staff       (20)     1480 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/environment-ubuntu-3.6-minver.yml
+-rw-r--r--   0 amici      (501) staff       (20)     1668 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/environment-ubuntu-3.7.yml
+-rw-r--r--   0 amici      (501) staff       (20)     1638 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/environment-ubuntu-3.8.yml
+-rw-r--r--   0 amici      (501) staff       (20)     1350 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/environment-ubuntu-3.9-minimal.yml
+-rw-r--r--   0 amici      (501) staff       (20)     1545 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/environment-windows-3.8.yml
+drwxr-xr-x   0 amici      (501) staff       (20)        0 2021-09-29 09:08:47.964840 cfgrib-0.9.9.1/tests/sample-data/
+-rw-r--r--   0 amici      (501) staff       (20)    44136 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/era5-levels-corrupted.grib
+-rw-r--r--   0 amici      (501) staff       (20)  2361600 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/era5-levels-members.grib
+-rw-r--r--   0 amici      (501) staff       (20)    48840 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/era5-single-level-scalar-time.grib
+-rw-r--r--   0 amici      (501) staff       (20)     9960 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/fields_with_missing_values.grib
+-rw-r--r--   0 amici      (501) staff       (20)    80640 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/forecast_monthly_ukmo.grib
+-rw-r--r--   0 amici      (501) staff       (20)    20400 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/hpa_and_pa.grib
+-rw-r--r--   0 amici      (501) staff       (20)    56880 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/lambert_grid.grib
+-rw-r--r--   0 amici      (501) staff       (20)   103680 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/multi_param_on_multi_dims.grib
+-rw-r--r--   0 amici      (501) staff       (20)    13680 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/reduced_gg.grib
+-rw-r--r--   0 amici      (501) staff       (20)    14244 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_gg_ml.grib
+-rw-r--r--   0 amici      (501) staff       (20)   311400 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_gg_ml_g2.grib
+-rw-r--r--   0 amici      (501) staff       (20)    18600 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_gg_pl.grib
+-rw-r--r--   0 amici      (501) staff       (20)    18600 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_gg_sfc.grib
+-rw-r--r--   0 amici      (501) staff       (20)    55475 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_gg_wrong_increment.grib
+-rw-r--r--   0 amici      (501) staff       (20)   114212 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_ll_msl.grib
+-rw-r--r--   0 amici      (501) staff       (20)     2772 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_ll_sfc.grib
+-rw-r--r--   0 amici      (501) staff       (20)     8171 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/regular_ll_wrong_increment.grib
+-rw-r--r--   0 amici      (501) staff       (20)     8100 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/scanning_mode_64.grib
+-rw-r--r--   0 amici      (501) staff       (20)     1440 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/single_gridpoint.grib
+-rw-r--r--   0 amici      (501) staff       (20)     9360 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/spherical_harmonics.grib
+-rw-r--r--   0 amici      (501) staff       (20)     8160 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/t_analysis_and_fc_0.grib
+-rw-r--r--   0 amici      (501) staff       (20)     4080 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/t_on_different_level_types.grib
+-rw-r--r--   0 amici      (501) staff       (20)     7200 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/tp_on_different_grid_resolutions.grib
+-rw-r--r--   0 amici      (501) staff       (20)    23040 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/sample-data/uv_on_different_levels.grib
+-rw-r--r--   0 amici      (501) staff       (20)      317 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_10_cfunits.py
+-rw-r--r--   0 amici      (501) staff       (20)     5141 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_20_cfcoords.py
+-rw-r--r--   0 amici      (501) staff       (20)      375 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_20_main.py
+-rw-r--r--   0 amici      (501) staff       (20)     6990 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_20_messages.py
+-rw-r--r--   0 amici      (501) staff       (20)     2402 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_25_cfmessage.py
+-rw-r--r--   0 amici      (501) staff       (20)     8160 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_30_dataset.py
+-rw-r--r--   0 amici      (501) staff       (20)     2348 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_40_xarray_store.ipynb
+-rw-r--r--   0 amici      (501) staff       (20)     3351 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_40_xarray_store.py
+-rw-r--r--   0 amici      (501) staff       (20)     2352 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_40_xarray_to_grib_regular_ll.py
+-rw-r--r--   0 amici      (501) staff       (20)     1821 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_50_datamodels.py
+-rw-r--r--   0 amici      (501) staff       (20)     3154 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_50_sample_data.py
+-rw-r--r--   0 amici      (501) staff       (20)     2337 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_50_xarray_getitem.py
+-rw-r--r--   0 amici      (501) staff       (20)      986 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_50_xarray_plugin.py
+-rw-r--r--   0 amici      (501) staff       (20)     1375 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tests/test_60_main_commands.py
+-rw-r--r--   0 amici      (501) staff       (20)      703 2021-09-29 09:08:47.000000 cfgrib-0.9.9.1/tox.ini
```

### Comparing `cfgrib-0.9.9.0/CHANGELOG.rst` & `cfgrib-0.9.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 
 Changelog for cfgrib
 ====================
 
+0.9.9.1 (2021-09-29)
+--------------------
+
+- Fix the plugin interface that was missing ``extra_coords``.
+  See `#231 <https://github.com/ecmwf/cfgrib/issues/231>`_.
+- Fix the crash when ``extra_coords`` return a scalar.
+  See `#238 <https://github.com/ecmwf/cfgrib/issues/238>`_.
+- Improve type-hints.
+  Needed by `#243 <https://github.com/ecmwf/cfgrib/issues/243>`_.
+
+
 0.9.9.0 (2021-04-09)
 --------------------
 
 - Depend on the ECMWF `eccodes python package <https://pypi.org/project/eccodes>`_ to access
   the low level ecCodes C-library, dropping all other GRIB decoding options.
   See: `#95 <https://github.com/ecmwf/cfgrib/issues/95>`_,
   `#14 <https://github.com/ecmwf/cfgrib/issues/14>`_.
```

### Comparing `cfgrib-0.9.9.0/CONTRIBUTING.rst` & `cfgrib-0.9.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/Dockerfile` & `cfgrib-0.9.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/LICENSE` & `cfgrib-0.9.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/Makefile` & `cfgrib-0.9.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/PKG-INFO` & `cfgrib-0.9.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgrib
-Version: 0.9.9.0
+Version: 0.9.9.1
 Summary: Python interface to map GRIB files to the NetCDF Common Data Model following the CF Convention using ecCodes.
 Home-page: https://github.com/ecmwf/cfgrib
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Description: cfgrib: A Python interface to map GRIB files to the NetCDF Common Data Model following the CF Convention using ecCodes
         ======================================================================================================================
@@ -99,15 +99,15 @@
         
         .. code-block: python
         
         >>> import xarray as xr
         >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
         >>> ds
         <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+        Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number         (number) int64 0 1 2 3 4 5 6 7 8 9
           * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step           timedelta64[ns] ...
           * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
           * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -163,15 +163,15 @@
         
         .. code-block: python
         
         >>> import cf2cdm
         >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
         >>> cf2cdm.translate_coords(ds, cf2cdm.ECMWF)
         <xarray.Dataset>
-        Dimensions:     (latitude: 61, level: 2, longitude: 120, number: 10, time: 4)
+        Dimensions:     (number: 10, time: 4, level: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number      (number) int64 0 1 2 3 4 5 6 7 8 9
           * time        (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step        timedelta64[ns] ...
           * level       (level) float64 850.0 500.0
           * latitude    (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude   (longitude) float64 0.0 3.0 6.0 9.0 ... 348.0 351.0 354.0 357.0
@@ -191,15 +191,15 @@
         To translate to the Common Data Model of the Climate Data Store use:
         
         .. code-block: python
         
         >>> import cf2cdm
         >>> cf2cdm.translate_coords(ds, cf2cdm.CDS)
         <xarray.Dataset>
-        Dimensions:                  (forecast_reference_time: 4, lat: 61, lon: 120, plev: 2, realization: 10)
+        Dimensions:                  (realization: 10, forecast_reference_time: 4, plev: 2, lat: 61, lon: 120)
         Coordinates:
           * realization              (realization) int64 0 1 2 3 4 5 6 7 8 9
           * forecast_reference_time  (forecast_reference_time) datetime64[ns] 2017-01...
             leadtime                 timedelta64[ns] ...
           * plev                     (plev) float64 8.5e+04 5e+04
           * lat                      (lat) float64 -90.0 -87.0 -84.0 ... 84.0 87.0 90.0
           * lon                      (lon) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -243,23 +243,23 @@
         you can use:
         
         .. code-block: python
         
         >>> xr.open_dataset('nam.t00z.awp21100.tm00.grib2', engine='cfgrib',
         ...     backend_kwargs={'filter_by_keys': {'typeOfLevel': 'surface'}})
         <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] ...
             step        timedelta64[ns] ...
             surface     float64 ...
             latitude    (y, x) float64 ...
             longitude   (y, x) float64 ...
             valid_time  datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             gust        (y, x) float32 ...
             sp          (y, x) float32 ...
             orog        (y, x) float32 ...
             tp          (y, x) float32 ...
             acpcp       (y, x) float32 ...
             csnow       (y, x) float32 ...
@@ -276,23 +276,23 @@
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP...
             history:                 ...
         >>> xr.open_dataset('nam.t00z.awp21100.tm00.grib2', engine='cfgrib',
         ...     backend_kwargs={'filter_by_keys': {'typeOfLevel': 'heightAboveGround', 'level': 2}})
         <xarray.Dataset>
-        Dimensions:            (x: 93, y: 65)
+        Dimensions:            (y: 65, x: 93)
         Coordinates:
             time               datetime64[ns] ...
             step               timedelta64[ns] ...
             heightAboveGround  float64 ...
             latitude           (y, x) float64 ...
             longitude          (y, x) float64 ...
             valid_time         datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t2m                (y, x) float32 ...
             r2                 (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
@@ -309,293 +309,312 @@
         and returns a list of all valid ``xarray.Dataset``'s in the GRIB file.
         
         .. code-block: python
         
         >>> import cfgrib
         >>> cfgrib.open_datasets('nam.t00z.awp21100.tm00.grib2')
         [<xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:                (y: 65, x: 93)
+        Coordinates:
+            time                   datetime64[ns] 2018-09-17
+            step                   timedelta64[ns] 00:00:00
+            atmosphereSingleLayer  float64 0.0
+            latitude               (y, x) float64 ...
+            longitude              (y, x) float64 ...
+            valid_time             datetime64[ns] ...
+        Dimensions without coordinates: y, x
+        Data variables:
+            pwat                   (y, x) float32 ...
+        Attributes:
+            GRIB_edition:            2
+            GRIB_centre:             kwbc
+            GRIB_centreDescription:  US National Weather Service - NCEP...
+            GRIB_subCentre:          0
+            Conventions:             CF-1.7
+            institution:             US National Weather Service - NCEP , <xarray.Dataset>
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             cloudBase   float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pres        (y, x) float32 ...
             gh          (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             cloudTop    float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pres        (y, x) float32 ...
             t           (y, x) float32 ...
             gh          (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:            (x: 93, y: 65)
+        Dimensions:            (y: 65, x: 93)
         Coordinates:
             time               datetime64[ns] 2018-09-17
             step               timedelta64[ns] 00:00:00
             heightAboveGround  float64 10.0
             latitude           (y, x) float64 ...
             longitude          (y, x) float64 ...
             valid_time         datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             u10                (y, x) float32 ...
+            v10                (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:            (x: 93, y: 65)
+        Dimensions:            (y: 65, x: 93)
         Coordinates:
             time               datetime64[ns] 2018-09-17
             step               timedelta64[ns] 00:00:00
             heightAboveGround  float64 2.0
             latitude           (y, x) float64 12.19 12.39 12.58 ... 57.68 57.49 57.29
             longitude          (y, x) float64 226.5 227.2 227.9 ... 308.5 309.6 310.6
             valid_time         datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t2m                (y, x) float32 ...
             r2                 (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                 (heightAboveGroundLayer: 2, x: 93, y: 65)
+        Dimensions:                 (heightAboveGroundLayer: 2, y: 65, x: 93)
         Coordinates:
             time                    datetime64[ns] 2018-09-17
             step                    timedelta64[ns] 00:00:00
           * heightAboveGroundLayer  (heightAboveGroundLayer) float64 1e+03 3e+03
             latitude                (y, x) float64 ...
             longitude               (y, x) float64 ...
             valid_time              datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             hlcy                    (heightAboveGroundLayer, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 19, x: 93, y: 65)
+        Dimensions:        (isobaricInhPa: 19, y: 65, x: 93)
         Coordinates:
             time           datetime64[ns] 2018-09-17
             step           timedelta64[ns] 00:00:00
           * isobaricInhPa  (isobaricInhPa) float64 1e+03 950.0 900.0 ... 150.0 100.0
             latitude       (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude      (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time     datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t              (isobaricInhPa, y, x) float32 ...
             u              (isobaricInhPa, y, x) float32 ...
             v              (isobaricInhPa, y, x) float32 ...
             w              (isobaricInhPa, y, x) float32 ...
             gh             (isobaricInhPa, y, x) float32 ...
             r              (isobaricInhPa, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 5, x: 93, y: 65)
+        Dimensions:        (isobaricInhPa: 5, y: 65, x: 93)
         Coordinates:
             time           datetime64[ns] 2018-09-17
             step           timedelta64[ns] 00:00:00
           * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0 700.0 500.0 250.0
             latitude       (y, x) float64 ...
             longitude      (y, x) float64 ...
             valid_time     datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             absv           (isobaricInhPa, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:       (x: 93, y: 65)
+        Dimensions:       (y: 65, x: 93)
         Coordinates:
             time          datetime64[ns] 2018-09-17
             step          timedelta64[ns] 00:00:00
             isothermZero  float64 0.0
             latitude      (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude     (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time    datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             gh            (y, x) float32 ...
             r             (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             maxWind     float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pres        (y, x) float32 ...
             u           (y, x) float32 ...
             v           (y, x) float32 ...
             gh          (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             meanSea     float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             prmsl       (y, x) float32 ...
             mslet       (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (pressureFromGroundLayer: 2, x: 93, y: 65)
+        Dimensions:                  (pressureFromGroundLayer: 2, y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
           * pressureFromGroundLayer  (pressureFromGroundLayer) float64 9e+03 1.8e+04
             latitude                 (y, x) float64 12.19 12.39 12.58 ... 57.49 57.29
             longitude                (y, x) float64 226.5 227.2 227.9 ... 309.6 310.6
             valid_time               datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             cape                     (pressureFromGroundLayer, y, x) float32 ...
             cin                      (pressureFromGroundLayer, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (pressureFromGroundLayer: 5, x: 93, y: 65)
+        Dimensions:                  (pressureFromGroundLayer: 5, y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
           * pressureFromGroundLayer  (pressureFromGroundLayer) float64 3e+03 ... 1.5e+04
             latitude                 (y, x) float64 12.19 12.39 12.58 ... 57.49 57.29
             longitude                (y, x) float64 226.5 227.2 227.9 ... 309.6 310.6
             valid_time               datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t                        (pressureFromGroundLayer, y, x) float32 ...
             u                        (pressureFromGroundLayer, y, x) float32 ...
             v                        (pressureFromGroundLayer, y, x) float32 ...
             r                        (pressureFromGroundLayer, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (x: 93, y: 65)
+        Dimensions:                  (y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
             pressureFromGroundLayer  float64 3e+03
             latitude                 (y, x) float64 ...
             longitude                (y, x) float64 ...
             valid_time               datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pli                      (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (x: 93, y: 65)
+        Dimensions:                  (y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
             pressureFromGroundLayer  float64 1.8e+04
             latitude                 (y, x) float64 ...
             longitude                (y, x) float64 ...
             valid_time               datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             4lftx                    (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             surface     float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             cape        (y, x) float32 ...
             sp          (y, x) float32 ...
             acpcp       (y, x) float32 ...
             cin         (y, x) float32 ...
             orog        (y, x) float32 ...
             tp          (y, x) float32 ...
@@ -608,46 +627,28 @@
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             tropopause  float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
-            pres        (y, x) float32 ...
             t           (y, x) float32 ...
             u           (y, x) float32 ...
             v           (y, x) float32 ...
-        Attributes:
-            GRIB_edition:            2
-            GRIB_centre:             kwbc
-            GRIB_centreDescription:  US National Weather Service - NCEP...
-            GRIB_subCentre:          0
-            Conventions:             CF-1.7
-            institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
-        Coordinates:
-            time        datetime64[ns] 2018-09-17
-            step        timedelta64[ns] 00:00:00
-            level       float64 0.0
-            latitude    (y, x) float64 ...
-            longitude   (y, x) float64 ...
-            valid_time  datetime64[ns] ...
-        Dimensions without coordinates: x, y
-        Data variables:
-            pwat        (y, x) float32 ...
+            trpp        (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP ]
@@ -666,15 +667,15 @@
         
         .. code-block: python
         
         >>> from cfgrib.xarray_to_grib import to_grib
         >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
         >>> ds
         <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+        Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number         (number) int64 0 1 2 3 4 5 6 7 8 9
           * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step           timedelta64[ns] ...
           * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
           * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -689,15 +690,15 @@
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             European Centre for Medium-Range Weather Forecasts
             history:                 ...
         >>> to_grib(ds, 'out1.grib', grib_keys={'edition': 2})
         >>> xr.open_dataset('out1.grib', engine='cfgrib')
         <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+        Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number         (number) int64 0 1 2 3 4 5 6 7 8 9
           * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step           timedelta64[ns] ...
           * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
           * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -846,14 +847,25 @@
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
         Changelog for cfgrib
         ====================
         
+        0.9.9.1 (2021-09-29)
+        --------------------
+        
+        - Fix the plugin interface that was missing ``extra_coords``.
+          See `#231 <https://github.com/ecmwf/cfgrib/issues/231>`_.
+        - Fix the crash when ``extra_coords`` return a scalar.
+          See `#238 <https://github.com/ecmwf/cfgrib/issues/238>`_.
+        - Improve type-hints.
+          Needed by `#243 <https://github.com/ecmwf/cfgrib/issues/243>`_.
+        
+        
         0.9.9.0 (2021-04-09)
         --------------------
         
         - Depend on the ECMWF `eccodes python package <https://pypi.org/project/eccodes>`_ to access
           the low level ecCodes C-library, dropping all other GRIB decoding options.
           See: `#95 <https://github.com/ecmwf/cfgrib/issues/95>`_,
           `#14 <https://github.com/ecmwf/cfgrib/issues/14>`_.
@@ -1187,10 +1199,10 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Provides-Extra: xarray
 Provides-Extra: tests
```

### Comparing `cfgrib-0.9.9.0/README.rst` & `cfgrib-0.9.9.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 .. code-block: python
 
 >>> import xarray as xr
 >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
 >>> ds
 <xarray.Dataset>
-Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
 Coordinates:
   * number         (number) int64 0 1 2 3 4 5 6 7 8 9
   * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
     step           timedelta64[ns] ...
   * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
   * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
   * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -155,15 +155,15 @@
 
 .. code-block: python
 
 >>> import cf2cdm
 >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
 >>> cf2cdm.translate_coords(ds, cf2cdm.ECMWF)
 <xarray.Dataset>
-Dimensions:     (latitude: 61, level: 2, longitude: 120, number: 10, time: 4)
+Dimensions:     (number: 10, time: 4, level: 2, latitude: 61, longitude: 120)
 Coordinates:
   * number      (number) int64 0 1 2 3 4 5 6 7 8 9
   * time        (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
     step        timedelta64[ns] ...
   * level       (level) float64 850.0 500.0
   * latitude    (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
   * longitude   (longitude) float64 0.0 3.0 6.0 9.0 ... 348.0 351.0 354.0 357.0
@@ -183,15 +183,15 @@
 To translate to the Common Data Model of the Climate Data Store use:
 
 .. code-block: python
 
 >>> import cf2cdm
 >>> cf2cdm.translate_coords(ds, cf2cdm.CDS)
 <xarray.Dataset>
-Dimensions:                  (forecast_reference_time: 4, lat: 61, lon: 120, plev: 2, realization: 10)
+Dimensions:                  (realization: 10, forecast_reference_time: 4, plev: 2, lat: 61, lon: 120)
 Coordinates:
   * realization              (realization) int64 0 1 2 3 4 5 6 7 8 9
   * forecast_reference_time  (forecast_reference_time) datetime64[ns] 2017-01...
     leadtime                 timedelta64[ns] ...
   * plev                     (plev) float64 8.5e+04 5e+04
   * lat                      (lat) float64 -90.0 -87.0 -84.0 ... 84.0 87.0 90.0
   * lon                      (lon) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -235,23 +235,23 @@
 you can use:
 
 .. code-block: python
 
 >>> xr.open_dataset('nam.t00z.awp21100.tm00.grib2', engine='cfgrib',
 ...     backend_kwargs={'filter_by_keys': {'typeOfLevel': 'surface'}})
 <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] ...
     step        timedelta64[ns] ...
     surface     float64 ...
     latitude    (y, x) float64 ...
     longitude   (y, x) float64 ...
     valid_time  datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     gust        (y, x) float32 ...
     sp          (y, x) float32 ...
     orog        (y, x) float32 ...
     tp          (y, x) float32 ...
     acpcp       (y, x) float32 ...
     csnow       (y, x) float32 ...
@@ -268,23 +268,23 @@
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP...
     history:                 ...
 >>> xr.open_dataset('nam.t00z.awp21100.tm00.grib2', engine='cfgrib',
 ...     backend_kwargs={'filter_by_keys': {'typeOfLevel': 'heightAboveGround', 'level': 2}})
 <xarray.Dataset>
-Dimensions:            (x: 93, y: 65)
+Dimensions:            (y: 65, x: 93)
 Coordinates:
     time               datetime64[ns] ...
     step               timedelta64[ns] ...
     heightAboveGround  float64 ...
     latitude           (y, x) float64 ...
     longitude          (y, x) float64 ...
     valid_time         datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     t2m                (y, x) float32 ...
     r2                 (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
@@ -301,293 +301,312 @@
 and returns a list of all valid ``xarray.Dataset``'s in the GRIB file.
 
 .. code-block: python
 
 >>> import cfgrib
 >>> cfgrib.open_datasets('nam.t00z.awp21100.tm00.grib2')
 [<xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:                (y: 65, x: 93)
+Coordinates:
+    time                   datetime64[ns] 2018-09-17
+    step                   timedelta64[ns] 00:00:00
+    atmosphereSingleLayer  float64 0.0
+    latitude               (y, x) float64 ...
+    longitude              (y, x) float64 ...
+    valid_time             datetime64[ns] ...
+Dimensions without coordinates: y, x
+Data variables:
+    pwat                   (y, x) float32 ...
+Attributes:
+    GRIB_edition:            2
+    GRIB_centre:             kwbc
+    GRIB_centreDescription:  US National Weather Service - NCEP...
+    GRIB_subCentre:          0
+    Conventions:             CF-1.7
+    institution:             US National Weather Service - NCEP , <xarray.Dataset>
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] 2018-09-17
     step        timedelta64[ns] 00:00:00
     cloudBase   float64 0.0
     latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time  datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     pres        (y, x) float32 ...
     gh          (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] 2018-09-17
     step        timedelta64[ns] 00:00:00
     cloudTop    float64 0.0
     latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time  datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     pres        (y, x) float32 ...
     t           (y, x) float32 ...
     gh          (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:            (x: 93, y: 65)
+Dimensions:            (y: 65, x: 93)
 Coordinates:
     time               datetime64[ns] 2018-09-17
     step               timedelta64[ns] 00:00:00
     heightAboveGround  float64 10.0
     latitude           (y, x) float64 ...
     longitude          (y, x) float64 ...
     valid_time         datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     u10                (y, x) float32 ...
+    v10                (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:            (x: 93, y: 65)
+Dimensions:            (y: 65, x: 93)
 Coordinates:
     time               datetime64[ns] 2018-09-17
     step               timedelta64[ns] 00:00:00
     heightAboveGround  float64 2.0
     latitude           (y, x) float64 12.19 12.39 12.58 ... 57.68 57.49 57.29
     longitude          (y, x) float64 226.5 227.2 227.9 ... 308.5 309.6 310.6
     valid_time         datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     t2m                (y, x) float32 ...
     r2                 (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:                 (heightAboveGroundLayer: 2, x: 93, y: 65)
+Dimensions:                 (heightAboveGroundLayer: 2, y: 65, x: 93)
 Coordinates:
     time                    datetime64[ns] 2018-09-17
     step                    timedelta64[ns] 00:00:00
   * heightAboveGroundLayer  (heightAboveGroundLayer) float64 1e+03 3e+03
     latitude                (y, x) float64 ...
     longitude               (y, x) float64 ...
     valid_time              datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     hlcy                    (heightAboveGroundLayer, y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:        (isobaricInhPa: 19, x: 93, y: 65)
+Dimensions:        (isobaricInhPa: 19, y: 65, x: 93)
 Coordinates:
     time           datetime64[ns] 2018-09-17
     step           timedelta64[ns] 00:00:00
   * isobaricInhPa  (isobaricInhPa) float64 1e+03 950.0 900.0 ... 150.0 100.0
     latitude       (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude      (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time     datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     t              (isobaricInhPa, y, x) float32 ...
     u              (isobaricInhPa, y, x) float32 ...
     v              (isobaricInhPa, y, x) float32 ...
     w              (isobaricInhPa, y, x) float32 ...
     gh             (isobaricInhPa, y, x) float32 ...
     r              (isobaricInhPa, y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:        (isobaricInhPa: 5, x: 93, y: 65)
+Dimensions:        (isobaricInhPa: 5, y: 65, x: 93)
 Coordinates:
     time           datetime64[ns] 2018-09-17
     step           timedelta64[ns] 00:00:00
   * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0 700.0 500.0 250.0
     latitude       (y, x) float64 ...
     longitude      (y, x) float64 ...
     valid_time     datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     absv           (isobaricInhPa, y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:       (x: 93, y: 65)
+Dimensions:       (y: 65, x: 93)
 Coordinates:
     time          datetime64[ns] 2018-09-17
     step          timedelta64[ns] 00:00:00
     isothermZero  float64 0.0
     latitude      (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude     (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time    datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     gh            (y, x) float32 ...
     r             (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] 2018-09-17
     step        timedelta64[ns] 00:00:00
     maxWind     float64 0.0
     latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time  datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     pres        (y, x) float32 ...
     u           (y, x) float32 ...
     v           (y, x) float32 ...
     gh          (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] 2018-09-17
     step        timedelta64[ns] 00:00:00
     meanSea     float64 0.0
     latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time  datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     prmsl       (y, x) float32 ...
     mslet       (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:                  (pressureFromGroundLayer: 2, x: 93, y: 65)
+Dimensions:                  (pressureFromGroundLayer: 2, y: 65, x: 93)
 Coordinates:
     time                     datetime64[ns] 2018-09-17
     step                     timedelta64[ns] 00:00:00
   * pressureFromGroundLayer  (pressureFromGroundLayer) float64 9e+03 1.8e+04
     latitude                 (y, x) float64 12.19 12.39 12.58 ... 57.49 57.29
     longitude                (y, x) float64 226.5 227.2 227.9 ... 309.6 310.6
     valid_time               datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     cape                     (pressureFromGroundLayer, y, x) float32 ...
     cin                      (pressureFromGroundLayer, y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:                  (pressureFromGroundLayer: 5, x: 93, y: 65)
+Dimensions:                  (pressureFromGroundLayer: 5, y: 65, x: 93)
 Coordinates:
     time                     datetime64[ns] 2018-09-17
     step                     timedelta64[ns] 00:00:00
   * pressureFromGroundLayer  (pressureFromGroundLayer) float64 3e+03 ... 1.5e+04
     latitude                 (y, x) float64 12.19 12.39 12.58 ... 57.49 57.29
     longitude                (y, x) float64 226.5 227.2 227.9 ... 309.6 310.6
     valid_time               datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     t                        (pressureFromGroundLayer, y, x) float32 ...
     u                        (pressureFromGroundLayer, y, x) float32 ...
     v                        (pressureFromGroundLayer, y, x) float32 ...
     r                        (pressureFromGroundLayer, y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:                  (x: 93, y: 65)
+Dimensions:                  (y: 65, x: 93)
 Coordinates:
     time                     datetime64[ns] 2018-09-17
     step                     timedelta64[ns] 00:00:00
     pressureFromGroundLayer  float64 3e+03
     latitude                 (y, x) float64 ...
     longitude                (y, x) float64 ...
     valid_time               datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     pli                      (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:                  (x: 93, y: 65)
+Dimensions:                  (y: 65, x: 93)
 Coordinates:
     time                     datetime64[ns] 2018-09-17
     step                     timedelta64[ns] 00:00:00
     pressureFromGroundLayer  float64 1.8e+04
     latitude                 (y, x) float64 ...
     longitude                (y, x) float64 ...
     valid_time               datetime64[ns] ...
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     4lftx                    (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] 2018-09-17
     step        timedelta64[ns] 00:00:00
     surface     float64 0.0
     latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time  datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
     cape        (y, x) float32 ...
     sp          (y, x) float32 ...
     acpcp       (y, x) float32 ...
     cin         (y, x) float32 ...
     orog        (y, x) float32 ...
     tp          (y, x) float32 ...
@@ -600,46 +619,28 @@
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
+Dimensions:     (y: 65, x: 93)
 Coordinates:
     time        datetime64[ns] 2018-09-17
     step        timedelta64[ns] 00:00:00
     tropopause  float64 0.0
     latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
     longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
     valid_time  datetime64[ns] 2018-09-17
-Dimensions without coordinates: x, y
+Dimensions without coordinates: y, x
 Data variables:
-    pres        (y, x) float32 ...
     t           (y, x) float32 ...
     u           (y, x) float32 ...
     v           (y, x) float32 ...
-Attributes:
-    GRIB_edition:            2
-    GRIB_centre:             kwbc
-    GRIB_centreDescription:  US National Weather Service - NCEP...
-    GRIB_subCentre:          0
-    Conventions:             CF-1.7
-    institution:             US National Weather Service - NCEP , <xarray.Dataset>
-Dimensions:     (x: 93, y: 65)
-Coordinates:
-    time        datetime64[ns] 2018-09-17
-    step        timedelta64[ns] 00:00:00
-    level       float64 0.0
-    latitude    (y, x) float64 ...
-    longitude   (y, x) float64 ...
-    valid_time  datetime64[ns] ...
-Dimensions without coordinates: x, y
-Data variables:
-    pwat        (y, x) float32 ...
+    trpp        (y, x) float32 ...
 Attributes:
     GRIB_edition:            2
     GRIB_centre:             kwbc
     GRIB_centreDescription:  US National Weather Service - NCEP...
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             US National Weather Service - NCEP ]
@@ -658,15 +659,15 @@
 
 .. code-block: python
 
 >>> from cfgrib.xarray_to_grib import to_grib
 >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
 >>> ds
 <xarray.Dataset>
-Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
 Coordinates:
   * number         (number) int64 0 1 2 3 4 5 6 7 8 9
   * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
     step           timedelta64[ns] ...
   * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
   * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
   * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -681,15 +682,15 @@
     GRIB_subCentre:          0
     Conventions:             CF-1.7
     institution:             European Centre for Medium-Range Weather Forecasts
     history:                 ...
 >>> to_grib(ds, 'out1.grib', grib_keys={'edition': 2})
 >>> xr.open_dataset('out1.grib', engine='cfgrib')
 <xarray.Dataset>
-Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
 Coordinates:
   * number         (number) int64 0 1 2 3 4 5 6 7 8 9
   * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
     step           timedelta64[ns] ...
   * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
   * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
   * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
```

### Comparing `cfgrib-0.9.9.0/cf2cdm/__init__.py` & `cfgrib-0.9.9.1/cf2cdm/__init__.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/cf2cdm/cfcoords.py` & `cfgrib-0.9.9.1/cf2cdm/cfcoords.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/cf2cdm/cfunits.py` & `cfgrib-0.9.9.1/cf2cdm/cfunits.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/cf2cdm/datamodels.py` & `cfgrib-0.9.9.1/cf2cdm/datamodels.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/cfgrib/__init__.py` & `cfgrib-0.9.9.1/cfgrib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.9.9.0"
+__version__ = "0.9.9.1"
 
 # cfgrib core API depends on the ECMWF ecCodes C-library only
 from .cfmessage import CfMessage
 from .dataset import Dataset, DatasetBuildError, open_file, open_fileindex
 from .messages import FileStream, Message
 
 # NOTE: xarray is not a hard dependency, but let's provide helpers if it is available.
```

### Comparing `cfgrib-0.9.9.0/cfgrib/__main__.py` & `cfgrib-0.9.9.1/cfgrib/__main__.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/cfgrib/cfmessage.py` & `cfgrib-0.9.9.1/cfgrib/cfmessage.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 import datetime
 import functools
 import logging
 import typing as T
 
 import attr
-import numpy as np  # type: ignore
+import numpy as np
 
-from . import messages
+from . import abc, messages
 
 LOG = logging.getLogger(__name__)
 
 # taken from eccodes stepUnits.table
 GRIB_STEP_UNITS_TO_SECONDS = [
     60,
     3600,
@@ -49,15 +49,15 @@
     900,
     1800,
 ]  # type: T.List[T.Union[int, None]]
 DEFAULT_EPOCH = datetime.datetime(1970, 1, 1)
 
 
 def from_grib_date_time(message, date_key="dataDate", time_key="dataTime", epoch=DEFAULT_EPOCH):
-    # type: (T.Mapping[str, T.Any], str, str, datetime.datetime) -> int
+    # type: (abc.Message, str, str, datetime.datetime) -> int
     """
     Return the number of seconds since the ``epoch`` from the values of the ``message`` keys,
     using datetime.total_seconds().
 
     :param message: the target GRIB message
     :param date_key: the date key, defaults to "dataDate"
     :param time_key: the time key, defaults to "dataTime"
@@ -75,53 +75,53 @@
     # see: https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp
     return int((data_datetime - epoch).total_seconds())
 
 
 def to_grib_date_time(
     message, time_ns, date_key="dataDate", time_key="dataTime", epoch=DEFAULT_EPOCH
 ):
-    # type: (T.MutableMapping[str, T.Any], np.datetime64, str, str, datetime.datetime) -> None
+    # type: (abc.MutableMessage, int, str, str, datetime.datetime) -> None
     time_s = int(time_ns) * 1e-9
     time = epoch + datetime.timedelta(seconds=time_s)
     datetime_iso = str(time)
     message[date_key] = int(datetime_iso[:10].replace("-", ""))
     message[time_key] = int(datetime_iso[11:16].replace(":", ""))
 
 
 def from_grib_step(message, step_key="endStep", step_unit_key="stepUnits"):
-    # type: (T.Mapping[str, T.Any], str, str) -> float
+    # type: (abc.Message, str, str) -> float
     step_unit = message[step_unit_key]
     to_seconds = GRIB_STEP_UNITS_TO_SECONDS[step_unit]
     if to_seconds is None:
         raise ValueError("unsupported stepUnit %r" % step_unit)
     assert isinstance(to_seconds, int)  # mypy misses this
     return int(message[step_key]) * to_seconds / 3600.0
 
 
 def to_grib_step(message, step_ns, step_unit=1, step_key="endStep", step_unit_key="stepUnits"):
-    # type: (T.MutableMapping[str, T.Any], int, int, str, str) -> None
+    # type: (abc.MutableMessage, int, int, str, str) -> None
     step_s = step_ns * 1e-9
     to_seconds = GRIB_STEP_UNITS_TO_SECONDS[step_unit]
     if to_seconds is None:
         raise ValueError("unsupported stepUnit %r" % step_unit)
     message[step_key] = step_s / to_seconds
     message[step_unit_key] = step_unit
 
 
 def from_grib_month(message, verifying_month_key="verifyingMonth", epoch=DEFAULT_EPOCH):
-    # type: (T.Mapping[str, T.Any], str, datetime.datetime) -> int
+    # type: (abc.Message, str, datetime.datetime) -> int
     date = message[verifying_month_key]
     year = date // 100
     month = date % 100
     data_datetime = datetime.datetime(year, month, 1, 0, 0)
     return int((data_datetime - epoch).total_seconds())
 
 
 def to_grib_dummy(message, value):
-    # type: (T.MutableMapping[str, T.Any], T.Any) -> None
+    # type: (abc.MutableMessage, T.Any) -> None
     pass
 
 
 def build_valid_time(time, step):
     # type: (np.ndarray, np.ndarray) -> T.Tuple[T.Tuple[str, ...], np.ndarray]
     """
     Return dimensions and data of the valid_time corresponding to the given ``time`` and ``step``.
```

### Comparing `cfgrib-0.9.9.0/cfgrib/dataset.py` & `cfgrib-0.9.9.1/cfgrib/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 import datetime
 import json
 import logging
 import os
 import typing as T
 
 import attr
-import numpy as np  # type: ignore
+import numpy as np
 
-from . import __version__, cfmessage, messages
+from . import __version__, abc, cfmessage, messages
 
 LOG = logging.getLogger(__name__)
 
 #
 # Edition-independent keys in ecCodes namespaces. Documented in:
 #   https://software.ecmwf.int/wiki/display/ECC/GRIB%3A+Namespaces
 #
@@ -256,15 +256,15 @@
 
 class DatasetBuildError(ValueError):
     def __str__(self) -> str:
         return str(self.args[0])
 
 
 def enforce_unique_attributes(index, attributes_keys, filter_by_keys={}):
-    # type: (T.Mapping[str, T.Any], T.Sequence[str], T.Dict[str, T.Any]) -> T.Dict[str, T.Any]
+    # type: (T.Mapping[str, T.List[T.Any]], T.Sequence[str], T.Dict[str, T.Any]) -> T.Dict[str, T.Any]
     attributes = {}  # type: T.Dict[str, T.Any]
     for key in attributes_keys:
         values = index[key]
         if len(values) > 1:
             fbks = []
             for value in values:
                 fbk = {key: value}
@@ -273,15 +273,15 @@
             raise DatasetBuildError("multiple values for key %r" % key, key, fbks)
         if values and values[0] not in ("undef", "unknown"):
             attributes["GRIB_" + key] = values[0]
     return attributes
 
 
 @attr.attrs(auto_attribs=True, eq=False)
-class Variable(object):
+class Variable:
     dimensions: T.Tuple[str, ...]
     data: np.ndarray
     attributes: T.Dict[str, T.Any] = attr.attrib(default={}, repr=False)
 
     def __eq__(self, other):
         # type: (T.Any) -> bool
         if other.__class__ is not self.__class__:
@@ -302,15 +302,15 @@
             expanded_item.append([i])
         else:
             raise TypeError("Unsupported index type %r" % type(i))
     return tuple(expanded_item)
 
 
 @attr.attrs(auto_attribs=True)
-class OnDiskArray(object):
+class OnDiskArray:
     stream: messages.FileStream
     shape: T.Tuple[int, ...]
     offsets: T.Dict[T.Tuple[T.Any, ...], T.List[T.Union[int, T.Tuple[int, int]]]] = attr.attrib(
         repr=False
     )
     missing_value: float
     geo_ndim: int = attr.attrib(default=1, repr=False)
@@ -341,15 +341,15 @@
                 except KeyError:
                     continue
                 # NOTE: fill a single field as found in the message
                 message = self.stream.message_from_file(file, offset=offset[0])
                 values = message.message_get("values", float)
                 array_field.__getitem__(tuple(array_field_indexes)).flat[:] = values
 
-        array = array_field[(Ellipsis,) + item[-self.geo_ndim :]]
+        array = np.asarray(array_field[(Ellipsis,) + item[-self.geo_ndim :]])
         array[array == self.missing_value] = np.nan
         for i, it in reversed(list(enumerate(item[: -self.geo_ndim]))):
             if isinstance(it, int):
                 array = array[(slice(None, None, None),) * i + (0,)]
         return array
 
 
@@ -361,18 +361,15 @@
     "lambert_azimuthal_equal_area",
     "albers",
     "polar_stereographic",
 }
 
 
 def build_geography_coordinates(
-    first,  # type: messages.Message
-    encode_cf,  # type: T.Sequence[str]
-    errors,  # type: str
-    log=LOG,  # type: logging.Logger
+    first: abc.Message, encode_cf: T.Sequence[str], errors: str, log: logging.Logger = LOG,
 ):
     # type: (...) -> T.Tuple[T.Tuple[str, ...], T.Tuple[int, ...], T.Dict[str, Variable]]
     geo_coord_vars = {}  # type: T.Dict[str, Variable]
     grid_type = first["gridType"]
     if "geography" in encode_cf and grid_type in GRID_TYPES_DIMENSION_COORDS:
         geo_dims = ("latitude", "longitude")  # type: T.Tuple[str, ...]
         geo_shape = (first["Ny"], first["Nx"])  # type: T.Tuple[int, ...]
@@ -447,15 +444,15 @@
     else:
         coords_map.extend(DATA_TIME_KEYS)
     coords_map.extend(VERTICAL_KEYS)
     coords_map.extend(SPECTRA_KEYS)
     return coords_map
 
 
-def read_data_var_attrs(first: messages.Message, extra_keys: T.List[str]) -> T.Dict[str, T.Any]:
+def read_data_var_attrs(first: abc.Message, extra_keys: T.List[str]) -> T.Dict[str, T.Any]:
     attributes = {}
     for key in extra_keys:
         try:
             attributes["GRIB_" + key] = first[key]
         except:
             pass
     return attributes
@@ -517,21 +514,26 @@
     coord_vars.update(geo_coord_vars)
 
     offsets = {}  # type: T.Dict[T.Tuple[int, ...], T.List[T.Union[int, T.Tuple[int, int]]]]
     header_value_index = {}
     extra_coords_data: T.Dict[str, T.Dict[str, T.Any]] = {
         coord_name: {} for coord_name in extra_coords
     }
-    for dim in header_dimensions:
-        header_value_index[dim] = {v: i for i, v in enumerate(coord_vars[dim].data.tolist())}
+    extra_dims = tuple(extra_coords.values())
+    for dim in header_dimensions + extra_dims:
+        if np.isscalar(coord_vars[dim].data):
+            header_value_index[dim] = {coord_vars[dim].data.item(): 0}
+        else:
+            header_value_index[dim] = {v: i for i, v in enumerate(coord_vars[dim].data.tolist())}
     for header_values, offset in index.offsets:
         header_indexes = []  # type: T.List[int]
-        for dim in header_dimensions:
+        for dim in header_dimensions + extra_dims:
             header_value = header_values[index.index_keys.index(coord_name_key_map.get(dim, dim))]
-            header_indexes.append(header_value_index[dim][header_value])
+            if dim in header_dimensions:
+                header_indexes.append(header_value_index[dim][header_value])
             for coord_name in extra_coords:
                 coord_value = header_values[
                     index.index_keys.index(coord_name_key_map.get(coord_name, coord_name))
                 ]
                 if dim == extra_coords[coord_name]:
                     saved_coord_value = extra_coords_data[coord_name].get(
                         header_value, coord_value
@@ -542,15 +544,15 @@
                             f"found two '{coord_name}' distinct values ({saved_coord_value}, {coord_value}) "
                             f"for '{extra_coords[coord_name]}' value {header_value}."
                         )
 
                     extra_coords_data[coord_name][header_value] = coord_value
         offsets[tuple(header_indexes)] = offset
     missing_value = data_var_attrs.get("missingValue", 9999)
-    data = OnDiskArray(
+    on_disk_array = OnDiskArray(
         stream=index.filestream,
         shape=shape,
         offsets=offsets,
         missing_value=missing_value,
         geo_ndim=len(geo_dims),
     )
 
@@ -559,20 +561,25 @@
         time_dims, time_data = cfmessage.build_valid_time(
             coord_vars["time"].data, coord_vars["step"].data,
         )
         attrs = COORD_ATTRS["valid_time"]
         coord_vars["valid_time"] = Variable(dimensions=time_dims, data=time_data, attributes=attrs)
 
     for coord_name in extra_coords:
-        coord_vars[coord_name] = Variable(
-            dimensions=(extra_coords[coord_name],),
-            data=np.array(list(extra_coords_data[coord_name].values())),
-        )
+        coord_data = np.array(list(extra_coords_data[coord_name].values()))
+        if extra_coords[coord_name] not in header_dimensions:
+            coord_dimensions: T.Tuple[str, ...] = ()
+            coord_data = coord_data.reshape(())
+        else:
+            coord_dimensions = (extra_coords[coord_name],)
+        coord_vars[coord_name] = Variable(dimensions=coord_dimensions, data=coord_data,)
+
     data_var_attrs["coordinates"] = " ".join(coord_vars.keys())
-    data_var = Variable(dimensions=dimensions, data=data, attributes=data_var_attrs)
+    # OnDiskArray is close enough to np.ndarray to work, but not to make mypy happy
+    data_var = Variable(dimensions=dimensions, data=on_disk_array, attributes=data_var_attrs)  # type: ignore
     dims = {d: s for d, s in zip(dimensions, data_var.data.shape)}
     return dims, data_var, coord_vars
 
 
 def dict_merge(master, update):
     # type: (T.Dict[str, T.Any], T.Dict[str, T.Any]) -> None
     for key, value in update.items():
@@ -666,15 +673,15 @@
         "encode_cf": encode_cf,
     }
     attributes = build_dataset_attributes(index, filter_by_keys, encoding)
     return dimensions, variables, attributes, encoding
 
 
 @attr.attrs(auto_attribs=True)
-class Dataset(object):
+class Dataset:
     """
     Map a GRIB file to the NetCDF Common Data Model with CF Conventions.
     """
 
     dimensions: T.Dict[str, int]
     variables: T.Dict[str, Variable]
     attributes: T.Dict[str, T.Any]
```

### Comparing `cfgrib-0.9.9.0/cfgrib/messages.py` & `cfgrib-0.9.9.1/cfgrib/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 import logging
 import os
 import pickle
 import typing as T
 
 import attr
 import eccodes  # type: ignore
-import numpy as np  # type: ignore
+import numpy as np
+
+from . import abc
 
 eccodes_version = eccodes.codes_get_api_version()
 
 LOG = logging.getLogger(__name__)
 _MARKER = object()
 
 #
@@ -61,27 +63,31 @@
     "float": float,
     "int": int,
     "str": str,
     "": None,
 }
 
 
+OffsetType = T.Union[int, T.Tuple[int, int]]
+OffsetsType = T.List[T.Tuple[T.Tuple[T.Any, ...], T.List[OffsetType]]]
+
+
 @attr.attrs(auto_attribs=True)
-class Message(T.MutableMapping[str, T.Any]):
+class Message(abc.MutableMessage):
     """Dictionary-line interface to access Message headers."""
 
     codes_id: int
     encoding: str = "ascii"
     errors: str = attr.attrib(
         default="warn", validator=attr.validators.in_(["ignore", "warn", "raise"])
     )
 
     @classmethod
     def from_file(cls, file, offset=None, **kwargs):
-        # type: (T.IO[bytes], T.Union[int, T.Tuple[int ,int], None], T.Any) -> Message
+        # type: (T.IO[bytes], T.Optional[OffsetType], T.Any) -> Message
         field_in_message = 0
         if isinstance(offset, tuple):
             offset, field_in_message = offset
         if offset is not None:
             file.seek(offset)
         codes_id = None
         if field_in_message == 0:
@@ -174,16 +180,16 @@
     def __len__(self) -> int:
         return sum(1 for _ in self)
 
     def write(self, file: T.IO[bytes]) -> None:
         eccodes.codes_write(self.codes_id, file)
 
 
-GetterType = T.Callable[[Message], T.Any]
-SetterType = T.Callable[[Message, T.Any], None]
+GetterType = T.Callable[..., T.Any]
+SetterType = T.Callable[..., None]
 ComputedKeysType = T.Dict[str, T.Tuple[GetterType, SetterType]]
 
 
 @attr.attrs(auto_attribs=True)
 class ComputedKeysMessage(Message):
     """Extension of Message class for adding computed keys."""
 
@@ -210,15 +216,15 @@
             _, setter = self.computed_keys[item]
             return setter(self, value)
         else:
             return super(ComputedKeysMessage, self).__setitem__(item, value)
 
 
 @attr.attrs(auto_attribs=True)
-class FileStream(T.Iterable[T.MutableMapping[str, T.Any]]):
+class FileStream(T.Iterable[Message]):
     """Iterator-like access to a filestream of Messages."""
 
     path: str
     message_class: T.Type[Message] = attr.attrib(default=Message, repr=False)
     errors: str = attr.attrib(
         default="warn", validator=attr.validators.in_(["ignore", "warn", "raise"])
     )
@@ -241,15 +247,15 @@
                             pass
                         elif self.errors == "raise":
                             raise
                         else:
                             LOG.exception("skipping corrupted Message")
 
     def message_from_file(self, file, offset=None, **kwargs):
-        # type: (T.IO[bytes], T.Union[int, T.Tuple[int, int], None], T.Any) -> Message
+        # type: (T.IO[bytes], T.Optional[OffsetType], T.Any) -> Message
         return self.message_class.from_file(file, offset, **kwargs)
 
     def first(self) -> Message:
         for message in self:
             return message
         raise ValueError("index has no message")
 
@@ -267,20 +273,19 @@
             yield file
         except Exception:
             file.close()
             os.unlink(path)
             raise
 
 
-OffsetsType = T.List[T.Tuple[T.Tuple[T.Any, ...], T.List[T.Union[int, T.Tuple[int, int]]]]]
 ALLOWED_PROTOCOL_VERSION = "1"
 
 
 @attr.attrs(auto_attribs=True)
-class FileIndex(T.Mapping[str, T.List[T.Any]]):
+class FileIndex(abc.Index[OffsetType, Message]):
     filestream: FileStream
     index_keys: T.List[str]
     offsets: OffsetsType = attr.attrib(repr=False)
     filter_by_keys: T.Dict[str, T.Any] = {}
     index_protocol_version: str = ALLOWED_PROTOCOL_VERSION
 
     @classmethod
```

### Comparing `cfgrib-0.9.9.0/cfgrib/xarray_plugin.py` & `cfgrib-0.9.9.1/cfgrib/xarray_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,26 +90,28 @@
         indexpath: str = "{path}.{short_hash}.idx",
         filter_by_keys: T.Dict[str, T.Any] = {},
         read_keys: T.Iterable[str] = (),
         encode_cf: T.Sequence[str] = ("parameter", "time", "geography", "vertical"),
         squeeze: bool = True,
         time_dims: T.Iterable[str] = ("time", "step"),
         errors: str = "warn",
+        extra_coords: T.Dict[str, str] = {},
     ) -> xr.Dataset:
 
         store = CfGribDataStore(
             filename_or_obj,
             indexpath=indexpath,
             filter_by_keys=filter_by_keys,
             read_keys=read_keys,
             encode_cf=encode_cf,
             squeeze=squeeze,
             time_dims=time_dims,
             lock=lock,
             errors=errors,
+            extra_coords=extra_coords,
         )
         with xr.core.utils.close_on_error(store):
             vars, attrs = store.load()  # type: ignore
             encoding = store.get_encoding()
             vars, attrs, coord_names = xr.conventions.decode_cf_variables(
                 vars,
                 attrs,
```

### Comparing `cfgrib-0.9.9.0/cfgrib/xarray_store.py` & `cfgrib-0.9.9.1/cfgrib/xarray_store.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/cfgrib/xarray_to_grib.py` & `cfgrib-0.9.9.1/cfgrib/xarray_to_grib.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #
 
 import itertools
 import logging
 import typing as T
 import warnings
 
-import numpy as np  # type: ignore
+import numpy as np
 import xarray as xr
 
 from . import cfmessage, dataset, messages
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -57,15 +57,15 @@
     #   unless `units` is set before some other unknown key, this happens at random and only in
     #   Python 3.5, so it must be linked to dict key stability.
     "units",
 ]
 
 
 def regular_ll_params(values, min_value=-180.0, max_value=360.0):
-    # type: (T.Sequence[float], float, float) -> T.Tuple[float, float, int]
+    # type: (np.ndarray, float, float) -> T.Tuple[float, float, int]
     start, stop, num = float(values[0]), float(values[-1]), len(values)
     if min(start, stop) < min_value or max(start, stop) > max_value:
         raise ValueError("Unsupported spatial grid: out of bounds (%r, %r)" % (start, stop))
     check_values = np.linspace(start, stop, num)
     if not np.allclose(check_values, values):
         raise ValueError("Unsupported spatial grid: not regular %r" % (check_values,))
     return (start, stop, num)
```

### Comparing `cfgrib-0.9.9.0/cfgrib.egg-info/PKG-INFO` & `cfgrib-0.9.9.1/cfgrib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgrib
-Version: 0.9.9.0
+Version: 0.9.9.1
 Summary: Python interface to map GRIB files to the NetCDF Common Data Model following the CF Convention using ecCodes.
 Home-page: https://github.com/ecmwf/cfgrib
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Description: cfgrib: A Python interface to map GRIB files to the NetCDF Common Data Model following the CF Convention using ecCodes
         ======================================================================================================================
@@ -99,15 +99,15 @@
         
         .. code-block: python
         
         >>> import xarray as xr
         >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
         >>> ds
         <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+        Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number         (number) int64 0 1 2 3 4 5 6 7 8 9
           * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step           timedelta64[ns] ...
           * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
           * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -163,15 +163,15 @@
         
         .. code-block: python
         
         >>> import cf2cdm
         >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
         >>> cf2cdm.translate_coords(ds, cf2cdm.ECMWF)
         <xarray.Dataset>
-        Dimensions:     (latitude: 61, level: 2, longitude: 120, number: 10, time: 4)
+        Dimensions:     (number: 10, time: 4, level: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number      (number) int64 0 1 2 3 4 5 6 7 8 9
           * time        (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step        timedelta64[ns] ...
           * level       (level) float64 850.0 500.0
           * latitude    (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude   (longitude) float64 0.0 3.0 6.0 9.0 ... 348.0 351.0 354.0 357.0
@@ -191,15 +191,15 @@
         To translate to the Common Data Model of the Climate Data Store use:
         
         .. code-block: python
         
         >>> import cf2cdm
         >>> cf2cdm.translate_coords(ds, cf2cdm.CDS)
         <xarray.Dataset>
-        Dimensions:                  (forecast_reference_time: 4, lat: 61, lon: 120, plev: 2, realization: 10)
+        Dimensions:                  (realization: 10, forecast_reference_time: 4, plev: 2, lat: 61, lon: 120)
         Coordinates:
           * realization              (realization) int64 0 1 2 3 4 5 6 7 8 9
           * forecast_reference_time  (forecast_reference_time) datetime64[ns] 2017-01...
             leadtime                 timedelta64[ns] ...
           * plev                     (plev) float64 8.5e+04 5e+04
           * lat                      (lat) float64 -90.0 -87.0 -84.0 ... 84.0 87.0 90.0
           * lon                      (lon) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -243,23 +243,23 @@
         you can use:
         
         .. code-block: python
         
         >>> xr.open_dataset('nam.t00z.awp21100.tm00.grib2', engine='cfgrib',
         ...     backend_kwargs={'filter_by_keys': {'typeOfLevel': 'surface'}})
         <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] ...
             step        timedelta64[ns] ...
             surface     float64 ...
             latitude    (y, x) float64 ...
             longitude   (y, x) float64 ...
             valid_time  datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             gust        (y, x) float32 ...
             sp          (y, x) float32 ...
             orog        (y, x) float32 ...
             tp          (y, x) float32 ...
             acpcp       (y, x) float32 ...
             csnow       (y, x) float32 ...
@@ -276,23 +276,23 @@
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP...
             history:                 ...
         >>> xr.open_dataset('nam.t00z.awp21100.tm00.grib2', engine='cfgrib',
         ...     backend_kwargs={'filter_by_keys': {'typeOfLevel': 'heightAboveGround', 'level': 2}})
         <xarray.Dataset>
-        Dimensions:            (x: 93, y: 65)
+        Dimensions:            (y: 65, x: 93)
         Coordinates:
             time               datetime64[ns] ...
             step               timedelta64[ns] ...
             heightAboveGround  float64 ...
             latitude           (y, x) float64 ...
             longitude          (y, x) float64 ...
             valid_time         datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t2m                (y, x) float32 ...
             r2                 (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
@@ -309,293 +309,312 @@
         and returns a list of all valid ``xarray.Dataset``'s in the GRIB file.
         
         .. code-block: python
         
         >>> import cfgrib
         >>> cfgrib.open_datasets('nam.t00z.awp21100.tm00.grib2')
         [<xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:                (y: 65, x: 93)
+        Coordinates:
+            time                   datetime64[ns] 2018-09-17
+            step                   timedelta64[ns] 00:00:00
+            atmosphereSingleLayer  float64 0.0
+            latitude               (y, x) float64 ...
+            longitude              (y, x) float64 ...
+            valid_time             datetime64[ns] ...
+        Dimensions without coordinates: y, x
+        Data variables:
+            pwat                   (y, x) float32 ...
+        Attributes:
+            GRIB_edition:            2
+            GRIB_centre:             kwbc
+            GRIB_centreDescription:  US National Weather Service - NCEP...
+            GRIB_subCentre:          0
+            Conventions:             CF-1.7
+            institution:             US National Weather Service - NCEP , <xarray.Dataset>
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             cloudBase   float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pres        (y, x) float32 ...
             gh          (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             cloudTop    float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pres        (y, x) float32 ...
             t           (y, x) float32 ...
             gh          (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:            (x: 93, y: 65)
+        Dimensions:            (y: 65, x: 93)
         Coordinates:
             time               datetime64[ns] 2018-09-17
             step               timedelta64[ns] 00:00:00
             heightAboveGround  float64 10.0
             latitude           (y, x) float64 ...
             longitude          (y, x) float64 ...
             valid_time         datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             u10                (y, x) float32 ...
+            v10                (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:            (x: 93, y: 65)
+        Dimensions:            (y: 65, x: 93)
         Coordinates:
             time               datetime64[ns] 2018-09-17
             step               timedelta64[ns] 00:00:00
             heightAboveGround  float64 2.0
             latitude           (y, x) float64 12.19 12.39 12.58 ... 57.68 57.49 57.29
             longitude          (y, x) float64 226.5 227.2 227.9 ... 308.5 309.6 310.6
             valid_time         datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t2m                (y, x) float32 ...
             r2                 (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                 (heightAboveGroundLayer: 2, x: 93, y: 65)
+        Dimensions:                 (heightAboveGroundLayer: 2, y: 65, x: 93)
         Coordinates:
             time                    datetime64[ns] 2018-09-17
             step                    timedelta64[ns] 00:00:00
           * heightAboveGroundLayer  (heightAboveGroundLayer) float64 1e+03 3e+03
             latitude                (y, x) float64 ...
             longitude               (y, x) float64 ...
             valid_time              datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             hlcy                    (heightAboveGroundLayer, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 19, x: 93, y: 65)
+        Dimensions:        (isobaricInhPa: 19, y: 65, x: 93)
         Coordinates:
             time           datetime64[ns] 2018-09-17
             step           timedelta64[ns] 00:00:00
           * isobaricInhPa  (isobaricInhPa) float64 1e+03 950.0 900.0 ... 150.0 100.0
             latitude       (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude      (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time     datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t              (isobaricInhPa, y, x) float32 ...
             u              (isobaricInhPa, y, x) float32 ...
             v              (isobaricInhPa, y, x) float32 ...
             w              (isobaricInhPa, y, x) float32 ...
             gh             (isobaricInhPa, y, x) float32 ...
             r              (isobaricInhPa, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 5, x: 93, y: 65)
+        Dimensions:        (isobaricInhPa: 5, y: 65, x: 93)
         Coordinates:
             time           datetime64[ns] 2018-09-17
             step           timedelta64[ns] 00:00:00
           * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0 700.0 500.0 250.0
             latitude       (y, x) float64 ...
             longitude      (y, x) float64 ...
             valid_time     datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             absv           (isobaricInhPa, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:       (x: 93, y: 65)
+        Dimensions:       (y: 65, x: 93)
         Coordinates:
             time          datetime64[ns] 2018-09-17
             step          timedelta64[ns] 00:00:00
             isothermZero  float64 0.0
             latitude      (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude     (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time    datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             gh            (y, x) float32 ...
             r             (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             maxWind     float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pres        (y, x) float32 ...
             u           (y, x) float32 ...
             v           (y, x) float32 ...
             gh          (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             meanSea     float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             prmsl       (y, x) float32 ...
             mslet       (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (pressureFromGroundLayer: 2, x: 93, y: 65)
+        Dimensions:                  (pressureFromGroundLayer: 2, y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
           * pressureFromGroundLayer  (pressureFromGroundLayer) float64 9e+03 1.8e+04
             latitude                 (y, x) float64 12.19 12.39 12.58 ... 57.49 57.29
             longitude                (y, x) float64 226.5 227.2 227.9 ... 309.6 310.6
             valid_time               datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             cape                     (pressureFromGroundLayer, y, x) float32 ...
             cin                      (pressureFromGroundLayer, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (pressureFromGroundLayer: 5, x: 93, y: 65)
+        Dimensions:                  (pressureFromGroundLayer: 5, y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
           * pressureFromGroundLayer  (pressureFromGroundLayer) float64 3e+03 ... 1.5e+04
             latitude                 (y, x) float64 12.19 12.39 12.58 ... 57.49 57.29
             longitude                (y, x) float64 226.5 227.2 227.9 ... 309.6 310.6
             valid_time               datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             t                        (pressureFromGroundLayer, y, x) float32 ...
             u                        (pressureFromGroundLayer, y, x) float32 ...
             v                        (pressureFromGroundLayer, y, x) float32 ...
             r                        (pressureFromGroundLayer, y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (x: 93, y: 65)
+        Dimensions:                  (y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
             pressureFromGroundLayer  float64 3e+03
             latitude                 (y, x) float64 ...
             longitude                (y, x) float64 ...
             valid_time               datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             pli                      (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:                  (x: 93, y: 65)
+        Dimensions:                  (y: 65, x: 93)
         Coordinates:
             time                     datetime64[ns] 2018-09-17
             step                     timedelta64[ns] 00:00:00
             pressureFromGroundLayer  float64 1.8e+04
             latitude                 (y, x) float64 ...
             longitude                (y, x) float64 ...
             valid_time               datetime64[ns] ...
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             4lftx                    (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             surface     float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
             cape        (y, x) float32 ...
             sp          (y, x) float32 ...
             acpcp       (y, x) float32 ...
             cin         (y, x) float32 ...
             orog        (y, x) float32 ...
             tp          (y, x) float32 ...
@@ -608,46 +627,28 @@
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
+        Dimensions:     (y: 65, x: 93)
         Coordinates:
             time        datetime64[ns] 2018-09-17
             step        timedelta64[ns] 00:00:00
             tropopause  float64 0.0
             latitude    (y, x) float64 12.19 12.39 12.58 12.77 ... 57.68 57.49 57.29
             longitude   (y, x) float64 226.5 227.2 227.9 228.7 ... 308.5 309.6 310.6
             valid_time  datetime64[ns] 2018-09-17
-        Dimensions without coordinates: x, y
+        Dimensions without coordinates: y, x
         Data variables:
-            pres        (y, x) float32 ...
             t           (y, x) float32 ...
             u           (y, x) float32 ...
             v           (y, x) float32 ...
-        Attributes:
-            GRIB_edition:            2
-            GRIB_centre:             kwbc
-            GRIB_centreDescription:  US National Weather Service - NCEP...
-            GRIB_subCentre:          0
-            Conventions:             CF-1.7
-            institution:             US National Weather Service - NCEP , <xarray.Dataset>
-        Dimensions:     (x: 93, y: 65)
-        Coordinates:
-            time        datetime64[ns] 2018-09-17
-            step        timedelta64[ns] 00:00:00
-            level       float64 0.0
-            latitude    (y, x) float64 ...
-            longitude   (y, x) float64 ...
-            valid_time  datetime64[ns] ...
-        Dimensions without coordinates: x, y
-        Data variables:
-            pwat        (y, x) float32 ...
+            trpp        (y, x) float32 ...
         Attributes:
             GRIB_edition:            2
             GRIB_centre:             kwbc
             GRIB_centreDescription:  US National Weather Service - NCEP...
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             US National Weather Service - NCEP ]
@@ -666,15 +667,15 @@
         
         .. code-block: python
         
         >>> from cfgrib.xarray_to_grib import to_grib
         >>> ds = xr.open_dataset('era5-levels-members.grib', engine='cfgrib')
         >>> ds
         <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+        Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number         (number) int64 0 1 2 3 4 5 6 7 8 9
           * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step           timedelta64[ns] ...
           * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
           * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -689,15 +690,15 @@
             GRIB_subCentre:          0
             Conventions:             CF-1.7
             institution:             European Centre for Medium-Range Weather Forecasts
             history:                 ...
         >>> to_grib(ds, 'out1.grib', grib_keys={'edition': 2})
         >>> xr.open_dataset('out1.grib', engine='cfgrib')
         <xarray.Dataset>
-        Dimensions:        (isobaricInhPa: 2, latitude: 61, longitude: 120, number: 10, time: 4)
+        Dimensions:        (number: 10, time: 4, isobaricInhPa: 2, latitude: 61, longitude: 120)
         Coordinates:
           * number         (number) int64 0 1 2 3 4 5 6 7 8 9
           * time           (time) datetime64[ns] 2017-01-01 ... 2017-01-02T12:00:00
             step           timedelta64[ns] ...
           * isobaricInhPa  (isobaricInhPa) float64 850.0 500.0
           * latitude       (latitude) float64 90.0 87.0 84.0 81.0 ... -84.0 -87.0 -90.0
           * longitude      (longitude) float64 0.0 3.0 6.0 9.0 ... 351.0 354.0 357.0
@@ -846,14 +847,25 @@
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
         Changelog for cfgrib
         ====================
         
+        0.9.9.1 (2021-09-29)
+        --------------------
+        
+        - Fix the plugin interface that was missing ``extra_coords``.
+          See `#231 <https://github.com/ecmwf/cfgrib/issues/231>`_.
+        - Fix the crash when ``extra_coords`` return a scalar.
+          See `#238 <https://github.com/ecmwf/cfgrib/issues/238>`_.
+        - Improve type-hints.
+          Needed by `#243 <https://github.com/ecmwf/cfgrib/issues/243>`_.
+        
+        
         0.9.9.0 (2021-04-09)
         --------------------
         
         - Depend on the ECMWF `eccodes python package <https://pypi.org/project/eccodes>`_ to access
           the low level ecCodes C-library, dropping all other GRIB decoding options.
           See: `#95 <https://github.com/ecmwf/cfgrib/issues/95>`_,
           `#14 <https://github.com/ecmwf/cfgrib/issues/14>`_.
@@ -1187,10 +1199,10 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Provides-Extra: xarray
 Provides-Extra: tests
```

### Comparing `cfgrib-0.9.9.0/cfgrib.egg-info/SOURCES.txt` & `cfgrib-0.9.9.1/cfgrib.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 .dockerignore
-.gitignore
 CHANGELOG.rst
 CONTRIBUTING.rst
 Dockerfile
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 appveyor.yml
 environment-minimal.in.yml
+environment-minver.in.yml
 environment.in.yml
 era5-levels-members.grib
 nam.t00z.awp21100.tm00.grib2
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-.github/workflows/on-push.yml
-.github/workflows/weekly.yml
 cf2cdm/__init__.py
 cf2cdm/cfcoords.py
 cf2cdm/cfunits.py
 cf2cdm/datamodels.py
 cfgrib/__init__.py
 cfgrib/__main__.py
+cfgrib/abc.py
 cfgrib/cfmessage.py
 cfgrib/dataset.py
 cfgrib/messages.py
 cfgrib/xarray_plugin.py
 cfgrib/xarray_store.py
 cfgrib/xarray_to_grib.py
 cfgrib.egg-info/PKG-INFO
@@ -59,36 +58,36 @@
 tests/cds_test_00_sync_sample_data.py
 tests/cds_test_10_era5.py
 tests/cds_test_20_sf_ecmwf.py
 tests/cds_test_20_sf_meteo_france.py
 tests/cds_test_20_sf_ukmo.py
 tests/cdscommon.py
 tests/environment-macos-3.8.yml
-tests/environment-ubuntu-3.6.yml
+tests/environment-ubuntu-3.6-minver.yml
 tests/environment-ubuntu-3.7.yml
 tests/environment-ubuntu-3.8.yml
 tests/environment-ubuntu-3.9-minimal.yml
-tests/environment-ubuntu-3.9.yml
 tests/environment-windows-3.8.yml
 tests/test_10_cfunits.py
 tests/test_20_cfcoords.py
 tests/test_20_main.py
-tests/test_20_main_commands.py
 tests/test_20_messages.py
 tests/test_25_cfmessage.py
 tests/test_30_dataset.py
 tests/test_40_xarray_store.ipynb
 tests/test_40_xarray_store.py
 tests/test_40_xarray_to_grib_regular_ll.py
 tests/test_50_datamodels.py
 tests/test_50_sample_data.py
 tests/test_50_xarray_getitem.py
 tests/test_50_xarray_plugin.py
+tests/test_60_main_commands.py
 tests/sample-data/era5-levels-corrupted.grib
 tests/sample-data/era5-levels-members.grib
+tests/sample-data/era5-single-level-scalar-time.grib
 tests/sample-data/fields_with_missing_values.grib
 tests/sample-data/forecast_monthly_ukmo.grib
 tests/sample-data/hpa_and_pa.grib
 tests/sample-data/lambert_grid.grib
 tests/sample-data/multi_param_on_multi_dims.grib
 tests/sample-data/reduced_gg.grib
 tests/sample-data/regular_gg_ml.grib
```

### Comparing `cfgrib-0.9.9.0/ci/install_python.ps1` & `cfgrib-0.9.9.1/ci/install_python.ps1`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/ci/requirements-docs.txt` & `cfgrib-0.9.9.1/ci/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/ci/requirements-tests.txt` & `cfgrib-0.9.9.1/ci/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/docs/conf.py` & `cfgrib-0.9.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/docs/index.rst` & `cfgrib-0.9.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/era5-levels-members.grib` & `cfgrib-0.9.9.1/era5-levels-members.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/nam.t00z.awp21100.tm00.grib2` & `cfgrib-0.9.9.1/nam.t00z.awp21100.tm00.grib2`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/setup.py` & `cfgrib-0.9.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,19 @@
     long_description=read("README.rst") + read("CHANGELOG.rst"),
     author="European Centre for Medium-Range Weather Forecasts (ECMWF)",
     author_email="software.support@ecmwf.int",
     license="Apache License Version 2.0",
     url="https://github.com/ecmwf/cfgrib",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=["attrs>=19.2", "click", "eccodes", "numpy"],
-    python_requires=">=3.5",
+    install_requires=["attrs>=19.2", "click", "eccodes>=0.9.8", "numpy"],
+    python_requires=">=3.6",
     extras_require={
-        "xarray": ["xarray>=0.12.0"],
-        "tests": ["dask[array]", "flake8", "pytest", "pytest-cov", "scipy", "xarray>=0.12.0",],
+        "xarray": ["xarray>=0.15"],
+        "tests": ["dask[array]", "flake8", "pytest", "pytest-cov", "scipy", "xarray>=0.15",],
     },
     zip_safe=True,
     keywords="eccodes grib xarray",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `cfgrib-0.9.9.0/tests/cds_test_00_sync_sample_data.py` & `cfgrib-0.9.9.1/tests/cds_test_00_sync_sample_data.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/cds_test_10_era5.py` & `cfgrib-0.9.9.1/tests/cds_test_10_era5.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/cds_test_20_sf_ecmwf.py` & `cfgrib-0.9.9.1/tests/cds_test_20_sf_ecmwf.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/cds_test_20_sf_meteo_france.py` & `cfgrib-0.9.9.1/tests/cds_test_20_sf_meteo_france.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/cds_test_20_sf_ukmo.py` & `cfgrib-0.9.9.1/tests/cds_test_20_sf_ukmo.py`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/cdscommon.py` & `cfgrib-0.9.9.1/tests/cdscommon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import hashlib
 import os
 import shutil
+import typing as T
 
-import cdsapi
+import cdsapi  # type: ignore
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 EXTENSIONS = {"grib": ".grib", "netcdf": ".nc"}
 
 
 def ensure_data(dataset, request, folder=SAMPLE_DATA_FOLDER, name="{uuid}.grib"):
+    # type: (str, T.Dict[str, T.Any], str, str) -> str
     request_text = str(sorted(request.items())).encode("utf-8")
     uuid = hashlib.sha3_224(request_text).hexdigest()[:10]
     format = request.get("format", "grib")
     ext = EXTENSIONS.get(format, ".bin")
     name = name.format(**locals())
     path = os.path.join(SAMPLE_DATA_FOLDER, name)
     if not os.path.exists(path):
```

### Comparing `cfgrib-0.9.9.0/tests/environment-macos-3.8.yml` & `cfgrib-0.9.9.1/tests/environment-ubuntu-3.9-minimal.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,70 @@
-name: macos-3.8
+name: ubuntu-3.9-minimal
 channels:
   - defaults
   - conda-forge
 dependencies:
-  - attrs=20.3.0
-  - blas=2.108
-  - blas-devel=3.9.0
+  - _libgcc_mutex=0.1
+  - _openmp_mutex=4.5
+  - attrs=21.2.0
+  - blas=2.106
   - bzip2=1.0.8
-  - ca-certificates=2021.1.19
-  - certifi=2020.12.5
-  - cffi=1.14.5
-  - click=7.1.2
+  - ca-certificates=2021.7.5
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - click=8.0.1
+  - coverage=5.5
   - curl=7.71.1
   - eccodes=2.21.0
   - hdf4=4.2.13
   - hdf5=1.10.6
+  - importlib-metadata=3.10.0
+  - iniconfig=1.1.1
   - jasper=1.900.1
   - jpeg=9d
-  - krb5=1.18.2
+  - krb5=1.19.2
+  - ld_impl_linux-64=2.35.1
   - libaec=1.0.4
   - libblas=3.9.0
   - libcblas=3.9.0
   - libcurl=7.71.1
-  - libcxx=11.1.0
   - libedit=3.1.20210216
   - libffi=3.3
-  - libgfortran=5.0.0
+  - libgcc-ng=11.1.0
+  - libgfortran-ng=9.3.0
   - libgfortran5=9.3.0
   - liblapack=3.9.0
   - liblapacke=3.9.0
   - libnetcdf=4.7.4
   - libopenblas=0.3.12
   - libpng=1.6.37
   - libssh2=1.9.0
-  - llvm-openmp=11.1.0
+  - libstdcxx-ng=9.3.0
+  - llvm-openmp=12.0.1
+  - more-itertools=8.8.0
   - ncurses=6.2
-  - numpy=1.19.2
-  - numpy-base=1.19.2
-  - openblas=0.3.12
+  - nomkl=3.0
+  - numpy=1.20.3
+  - numpy-base=1.20.3
   - openssl=1.1.1k
-  - pandas=1.0.5
-  - pip=21.0.1
+  - packaging=21.0
+  - pip=21.1.3
+  - pluggy=0.13.1
+  - py=1.10.0
   - pycparser=2.20
-  - python=3.8.8
-  - python-dateutil=2.8.1
+  - pyparsing=2.4.7
+  - pytest=6.2.4
+  - pytest-cov=2.12.1
+  - python=3.9.5
   - python-eccodes=2021.03.0
-  - python_abi=3.8
-  - pytz=2021.1
+  - python_abi=3.9
   - readline=8.1
-  - scipy=1.6.2
   - setuptools=52.0.0
-  - six=1.15.0
-  - sqlite=3.35.2
+  - sqlite=3.36.0
   - tk=8.6.10
+  - toml=0.10.2
+  - tzdata=2021a
   - wheel=0.36.2
-  - xarray=0.17.0
   - xz=5.2.5
+  - zipp=3.5.0
   - zlib=1.2.11
-prefix: /usr/local/miniconda/envs/macos-3.8
+prefix: /usr/share/miniconda/envs/ubuntu-3.9-minimal
```

### Comparing `cfgrib-0.9.9.0/tests/environment-ubuntu-3.6.yml` & `cfgrib-0.9.9.1/tests/environment-ubuntu-3.6-minver.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,76 @@
-name: ubuntu-3.6
+name: ubuntu-3.6-minver
 channels:
   - defaults
   - conda-forge
 dependencies:
   - _libgcc_mutex=0.1
-  - attrs=20.3.0
+  - _openmp_mutex=4.5
+  - attrs=19.2.0
   - blas=1.0
   - bzip2=1.0.8
-  - ca-certificates=2021.1.19
-  - certifi=2020.12.5
-  - cffi=1.14.5
-  - click=7.1.2
+  - ca-certificates=2021.7.5
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - click=7.0
+  - coverage=5.5
   - curl=7.71.1
-  - eccodes=2.19.1
+  - eccodes=2.16.0
   - hdf4=4.2.13
-  - hdf5=1.10.6
-  - intel-openmp=2020.2
+  - hdf5=1.10.5
+  - importlib-metadata=3.10.0
+  - importlib_metadata=3.10.0
+  - iniconfig=1.1.1
+  - intel-openmp=2021.3.0
   - jasper=1.900.1
   - jpeg=9d
-  - krb5=1.18.2
-  - ld_impl_linux-64=2.33.1
+  - krb5=1.19.2
+  - ld_impl_linux-64=2.35.1
   - libaec=1.0.4
   - libcurl=7.71.1
   - libedit=3.1.20210216
   - libffi=3.3
-  - libgcc-ng=9.1.0
+  - libgcc-ng=9.3.0
   - libgfortran-ng=7.5.0
   - libgfortran4=7.5.0
-  - libnetcdf=4.7.4
+  - libgomp=9.3.0
+  - libnetcdf=4.7.3
   - libpng=1.6.37
   - libssh2=1.9.0
-  - libstdcxx-ng=9.1.0
-  - mkl=2020.2
-  - mkl-service=2.3.0
-  - mkl_fft=1.3.0
-  - mkl_random=1.1.1
+  - libstdcxx-ng=9.3.0
+  - mkl=2018.0.3
+  - mkl_fft=1.0.6
+  - mkl_random=1.0.1
+  - more-itertools=8.8.0
   - ncurses=6.2
-  - numpy=1.19.2
-  - numpy-base=1.19.2
+  - numpy=1.15.0
+  - numpy-base=1.15.0
   - openssl=1.1.1k
-  - pandas=1.0.5
-  - pip=21.0.1
+  - packaging=21.0
+  - pandas=0.25.0
+  - pip=21.1.3
+  - pluggy=0.13.1
+  - py=1.10.0
   - pycparser=2.20
+  - pyparsing=2.4.7
+  - pytest=6.2.4
+  - pytest-cov=2.12.1
   - python=3.6.13
-  - python-dateutil=2.8.1
-  - python-eccodes=2020.10.1
+  - python-dateutil=2.8.2
+  - python-eccodes=2020.06.0
   - python_abi=3.6
   - pytz=2021.1
   - readline=8.1
-  - scipy=1.5.2
   - setuptools=52.0.0
-  - six=1.15.0
-  - sqlite=3.35.2
+  - six=1.16.0
+  - sqlite=3.36.0
+  - tbb=2021.3.0
+  - tbb4py=2021.3.0
   - tk=8.6.10
+  - toml=0.10.2
+  - typing_extensions=3.10.0.0
   - wheel=0.36.2
-  - xarray=0.17.0
+  - xarray=0.15.0
   - xz=5.2.5
+  - zipp=3.5.0
   - zlib=1.2.11
-prefix: /usr/share/miniconda/envs/ubuntu-3.6
+prefix: /usr/share/miniconda/envs/ubuntu-3.6-minver
```

### Comparing `cfgrib-0.9.9.0/tests/environment-ubuntu-3.7.yml` & `cfgrib-0.9.9.1/tests/environment-ubuntu-3.7.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,86 @@
 name: ubuntu-3.7
 channels:
   - defaults
   - conda-forge
 dependencies:
   - _libgcc_mutex=0.1
-  - attrs=20.3.0
-  - blas=1.0
+  - _openmp_mutex=4.5
+  - attrs=21.2.0
+  - blas=2.106
   - bzip2=1.0.8
-  - ca-certificates=2021.1.19
-  - certifi=2020.12.5
-  - cffi=1.14.5
-  - click=7.1.2
-  - curl=7.71.1
-  - eccodes=2.19.1
+  - c-ares=1.17.1
+  - ca-certificates=2021.7.5
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - click=8.0.1
+  - coverage=5.5
+  - curl=7.78.0
+  - eccodes=2.22.1
   - hdf4=4.2.13
   - hdf5=1.10.6
-  - intel-openmp=2020.2
+  - importlib-metadata=3.10.0
+  - importlib_metadata=3.10.0
+  - iniconfig=1.1.1
   - jasper=1.900.1
   - jpeg=9d
-  - krb5=1.18.2
-  - ld_impl_linux-64=2.33.1
-  - libaec=1.0.4
-  - libcurl=7.71.1
+  - krb5=1.19.2
+  - ld_impl_linux-64=2.35.1
+  - libaec=1.0.5
+  - libblas=3.9.0
+  - libcblas=3.9.0
+  - libcurl=7.78.0
   - libedit=3.1.20210216
+  - libev=4.33
   - libffi=3.3
-  - libgcc-ng=9.1.0
-  - libgfortran-ng=7.5.0
-  - libgfortran4=7.5.0
-  - libnetcdf=4.7.4
+  - libgcc-ng=11.1.0
+  - libgfortran-ng=9.3.0
+  - libgfortran5=9.3.0
+  - liblapack=3.9.0
+  - liblapacke=3.9.0
+  - libnetcdf=4.8.0
+  - libnghttp2=1.43.0
+  - libopenblas=0.3.12
   - libpng=1.6.37
   - libssh2=1.9.0
-  - libstdcxx-ng=9.1.0
-  - mkl=2020.2
-  - mkl-service=2.3.0
-  - mkl_fft=1.3.0
-  - mkl_random=1.1.1
+  - libstdcxx-ng=9.3.0
+  - libzip=1.8.0
+  - llvm-openmp=12.0.1
+  - more-itertools=8.8.0
+  - mypy=0.812
+  - mypy_extensions=0.4.3
   - ncurses=6.2
-  - numpy=1.19.2
-  - numpy-base=1.19.2
+  - nomkl=3.0
+  - numpy=1.20.3
+  - numpy-base=1.20.3
   - openssl=1.1.1k
+  - packaging=21.0
   - pandas=1.0.5
-  - pip=21.0.1
+  - pip=21.1.3
+  - pluggy=0.13.1
+  - psutil=5.8.0
+  - py=1.10.0
   - pycparser=2.20
+  - pyparsing=2.4.7
+  - pytest=6.2.4
+  - pytest-cov=2.12.1
   - python=3.7.10
-  - python-dateutil=2.8.1
-  - python-eccodes=2020.10.1
+  - python-dateutil=2.8.2
+  - python-eccodes=2021.03.0
   - python_abi=3.7
   - pytz=2021.1
   - readline=8.1
-  - scipy=1.6.2
+  - scipy=1.7.0
   - setuptools=52.0.0
-  - six=1.15.0
-  - sqlite=3.35.2
+  - six=1.16.0
+  - sqlite=3.36.0
   - tk=8.6.10
+  - toml=0.10.2
+  - typed-ast=1.4.3
+  - typing-extensions=3.10.0.0
+  - typing_extensions=3.10.0.0
   - wheel=0.36.2
-  - xarray=0.17.0
+  - xarray=0.19.0
   - xz=5.2.5
+  - zipp=3.5.0
   - zlib=1.2.11
 prefix: /usr/share/miniconda/envs/ubuntu-3.7
```

### Comparing `cfgrib-0.9.9.0/tests/environment-ubuntu-3.8.yml` & `cfgrib-0.9.9.1/tests/environment-macos-3.8.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,83 @@
-name: ubuntu-3.8
+name: macos-3.8
 channels:
   - defaults
   - conda-forge
 dependencies:
-  - _libgcc_mutex=0.1
-  - attrs=20.3.0
-  - blas=1.0
+  - attrs=21.2.0
+  - blas=2.110
+  - blas-devel=3.9.0
   - bzip2=1.0.8
-  - ca-certificates=2021.1.19
-  - certifi=2020.12.5
-  - cffi=1.14.5
-  - click=7.1.2
-  - curl=7.71.1
-  - eccodes=2.19.1
+  - c-ares=1.17.1
+  - ca-certificates=2021.7.5
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - click=8.0.1
+  - coverage=5.5
+  - curl=7.78.0
+  - eccodes=2.22.1
   - hdf4=4.2.13
   - hdf5=1.10.6
-  - intel-openmp=2020.2
+  - importlib-metadata=3.10.0
+  - iniconfig=1.1.1
   - jasper=1.900.1
   - jpeg=9d
-  - krb5=1.18.2
-  - ld_impl_linux-64=2.33.1
-  - libaec=1.0.4
-  - libcurl=7.71.1
+  - krb5=1.19.2
+  - libaec=1.0.5
+  - libblas=3.9.0
+  - libcblas=3.9.0
+  - libcurl=7.78.0
+  - libcxx=12.0.1
   - libedit=3.1.20210216
+  - libev=4.33
   - libffi=3.3
-  - libgcc-ng=9.1.0
-  - libgfortran-ng=7.5.0
-  - libgfortran4=7.5.0
-  - libnetcdf=4.7.4
+  - libgfortran=5.0.0
+  - libgfortran5=9.3.0
+  - liblapack=3.9.0
+  - liblapacke=3.9.0
+  - libnetcdf=4.8.0
+  - libnghttp2=1.43.0
+  - libopenblas=0.3.17
   - libpng=1.6.37
   - libssh2=1.9.0
-  - libstdcxx-ng=9.1.0
-  - mkl=2020.2
-  - mkl-service=2.3.0
-  - mkl_fft=1.3.0
-  - mkl_random=1.1.1
+  - libzip=1.8.0
+  - llvm-openmp=12.0.1
+  - more-itertools=8.8.0
+  - mypy=0.812
+  - mypy_extensions=0.4.3
   - ncurses=6.2
-  - numpy=1.19.2
-  - numpy-base=1.19.2
+  - nomkl=3.0
+  - numpy=1.20.3
+  - numpy-base=1.20.3
+  - openblas=0.3.17
   - openssl=1.1.1k
+  - packaging=21.0
   - pandas=1.0.5
-  - pip=21.0.1
+  - pip=21.1.3
+  - pluggy=0.13.1
+  - psutil=5.8.0
+  - py=1.10.0
   - pycparser=2.20
-  - python=3.8.8
-  - python-dateutil=2.8.1
-  - python-eccodes=2020.10.1
+  - pyparsing=2.4.7
+  - pytest=6.2.4
+  - pytest-cov=2.12.1
+  - python=3.8.10
+  - python-dateutil=2.8.2
+  - python-eccodes=2021.03.0
   - python_abi=3.8
   - pytz=2021.1
   - readline=8.1
-  - scipy=1.6.2
+  - scipy=1.7.0
   - setuptools=52.0.0
-  - six=1.15.0
-  - sqlite=3.35.2
+  - six=1.16.0
+  - sqlite=3.36.0
   - tk=8.6.10
+  - toml=0.10.2
+  - typed-ast=1.4.3
+  - typing-extensions=3.10.0.0
+  - typing_extensions=3.10.0.0
   - wheel=0.36.2
-  - xarray=0.17.0
+  - xarray=0.19.0
   - xz=5.2.5
+  - zipp=3.5.0
   - zlib=1.2.11
-prefix: /usr/share/miniconda/envs/ubuntu-3.8
+prefix: /usr/local/miniconda/envs/macos-3.8
```

### Comparing `cfgrib-0.9.9.0/tests/environment-ubuntu-3.9.yml` & `cfgrib-0.9.9.1/tests/environment-ubuntu-3.8.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,85 @@
-name: ubuntu-3.9
+name: ubuntu-3.8
 channels:
   - defaults
   - conda-forge
 dependencies:
   - _libgcc_mutex=0.1
-  - attrs=20.3.0
-  - blas=1.0
-  - bokeh=2.2.3
+  - _openmp_mutex=4.5
+  - attrs=21.2.0
+  - blas=2.106
   - bzip2=1.0.8
-  - ca-certificates=2020.12.8
-  - certifi=2020.12.5
-  - cffi=1.14.4
-  - cftime=1.3.0
-  - click=7.1.2
-  - cloudpickle=1.6.0
-  - curl=7.71.1
-  - cytoolz=0.11.0
-  - dask=2020.12.0
-  - dask-core=2020.12.0
-  - distributed=2020.12.0
-  - eccodes=2.18.0
-  - freetype=2.10.4
-  - fsspec=0.8.3
+  - c-ares=1.17.1
+  - ca-certificates=2021.7.5
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - click=8.0.1
+  - coverage=5.5
+  - curl=7.78.0
+  - eccodes=2.22.1
   - hdf4=4.2.13
   - hdf5=1.10.6
-  - heapdict=1.0.1
-  - intel-openmp=2020.2
+  - importlib-metadata=3.10.0
+  - iniconfig=1.1.1
   - jasper=1.900.1
-  - jinja2=2.11.2
   - jpeg=9d
-  - krb5=1.18.2
-  - lcms2=2.11
-  - ld_impl_linux-64=2.33.1
-  - libaec=1.0.4
-  - libcurl=7.71.1
-  - libedit=3.1.20191231
+  - krb5=1.19.2
+  - ld_impl_linux-64=2.35.1
+  - libaec=1.0.5
+  - libblas=3.9.0
+  - libcblas=3.9.0
+  - libcurl=7.78.0
+  - libedit=3.1.20210216
+  - libev=4.33
   - libffi=3.3
-  - libgcc-ng=9.1.0
-  - libgfortran-ng=7.3.0
-  - libnetcdf=4.7.4
+  - libgcc-ng=11.1.0
+  - libgfortran-ng=9.3.0
+  - libgfortran5=9.3.0
+  - liblapack=3.9.0
+  - liblapacke=3.9.0
+  - libnetcdf=4.8.0
+  - libnghttp2=1.43.0
+  - libopenblas=0.3.12
   - libpng=1.6.37
   - libssh2=1.9.0
-  - libstdcxx-ng=9.1.0
-  - libtiff=4.1.0
-  - locket=0.2.0
-  - lz4-c=1.9.2
-  - markupsafe=1.1.1
-  - mkl=2020.2
-  - mkl-service=2.3.0
-  - mkl_fft=1.0.6
-  - mkl_random=1.0.2
-  - msgpack-python=1.0.1
+  - libstdcxx-ng=9.3.0
+  - libzip=1.8.0
+  - llvm-openmp=12.0.1
+  - more-itertools=8.8.0
+  - mypy=0.812
+  - mypy_extensions=0.4.3
   - ncurses=6.2
-  - netcdf4=1.5.4
-  - numpy=1.19.2
-  - numpy-base=1.19.2
-  - olefile=0.46
-  - openssl=1.1.1i
-  - packaging=20.8
+  - nomkl=3.0
+  - numpy=1.20.3
+  - numpy-base=1.20.3
+  - openssl=1.1.1k
+  - packaging=21.0
   - pandas=1.0.5
-  - partd=1.1.0
-  - pillow=8.0.1
-  - pip=20.3.3
-  - psutil=5.7.2
+  - pip=21.1.3
+  - pluggy=0.13.1
+  - psutil=5.8.0
+  - py=1.10.0
   - pycparser=2.20
   - pyparsing=2.4.7
-  - python=3.9.1
-  - python-dateutil=2.8.1
-  - python-eccodes=2020.10.0
-  - python_abi=3.9
-  - pytz=2020.5
-  - pyyaml=5.3.1
-  - readline=8.0
-  - setuptools=51.0.0
-  - six=1.15.0
-  - sortedcontainers=2.3.0
-  - sqlite=3.33.0
-  - tblib=1.7.0
+  - pytest=6.2.4
+  - pytest-cov=2.12.1
+  - python=3.8.10
+  - python-dateutil=2.8.2
+  - python-eccodes=2021.03.0
+  - python_abi=3.8
+  - pytz=2021.1
+  - readline=8.1
+  - scipy=1.7.0
+  - setuptools=52.0.0
+  - six=1.16.0
+  - sqlite=3.36.0
   - tk=8.6.10
-  - toolz=0.11.1
-  - tornado=6.1
-  - typing_extensions=3.7.4.3
+  - toml=0.10.2
+  - typed-ast=1.4.3
+  - typing-extensions=3.10.0.0
+  - typing_extensions=3.10.0.0
   - wheel=0.36.2
-  - xarray=0.16.2
+  - xarray=0.19.0
   - xz=5.2.5
-  - yaml=0.2.5
-  - zict=2.0.0
+  - zipp=3.5.0
   - zlib=1.2.11
-  - zstd=1.4.5
-prefix: /usr/share/miniconda/envs/ubuntu-3.9
+prefix: /usr/share/miniconda/envs/ubuntu-3.8
```

### Comparing `cfgrib-0.9.9.0/tests/environment-windows-3.8.yml` & `cfgrib-0.9.9.1/tests/environment-windows-3.8.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,78 @@
 name: windows-3.8
 channels:
   - defaults
   - conda-forge
 dependencies:
-  - attrs=20.3.0
-  - blas=1.0
+  - atomicwrites=1.4.0
+  - attrs=21.2.0
   - bzip2=1.0.8
-  - ca-certificates=2021.1.19
-  - certifi=2020.12.5
-  - cffi=1.14.5
-  - click=7.1.2
-  - curl=7.71.1
-  - eccodes=2.21.0
+  - ca-certificates=2021.7.5
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - click=8.0.1
+  - colorama=0.4.4
+  - coverage=5.5
+  - curl=7.78.0
+  - eccodes=2.22.1
   - hdf4=4.2.13
   - hdf5=1.10.6
-  - icc_rt=2019.0.0
-  - intel-openmp=2020.2
+  - importlib-metadata=3.10.0
+  - iniconfig=1.1.1
   - jpeg=9d
-  - krb5=1.18.2
-  - libcurl=7.71.1
-  - libnetcdf=4.7.4
+  - krb5=1.19.2
+  - libblas=3.9.0
+  - libcblas=3.9.0
+  - libcurl=7.78.0
+  - liblapack=3.9.0
+  - libnetcdf=4.8.0
   - libpng=1.6.37
   - libssh2=1.9.0
   - libtiff=4.2.0
+  - libzip=1.8.0
   - lz4-c=1.9.3
-  - mkl=2020.2
-  - mkl-service=2.3.0
-  - mkl_fft=1.3.0
-  - mkl_random=1.1.1
-  - numpy=1.19.2
-  - numpy-base=1.19.2
+  - m2w64-gcc-libgfortran=5.3.0
+  - m2w64-gcc-libs=5.3.0
+  - m2w64-gcc-libs-core=5.3.0
+  - m2w64-gmp=6.1.0
+  - m2w64-libwinpthread-git=5.0.0.4634.697f757
+  - more-itertools=8.8.0
+  - msys2-conda-epoch=20160418
+  - mypy=0.812
+  - mypy_extensions=0.4.3
+  - nomkl=1.0
+  - numpy=1.21.1
   - openjpeg=2.4.0
   - openssl=1.1.1k
+  - packaging=21.0
   - pandas=1.0.5
-  - pip=21.0.1
+  - pip=21.1.3
+  - pluggy=0.13.1
+  - psutil=5.8.0
+  - py=1.10.0
   - pycparser=2.20
-  - python=3.8.8
-  - python-dateutil=2.8.1
+  - pyparsing=2.4.7
+  - pytest=6.2.4
+  - pytest-cov=2.12.1
+  - python=3.8.10
+  - python-dateutil=2.8.2
   - python-eccodes=2021.03.0
   - python_abi=3.8
   - pytz=2021.1
-  - scipy=1.6.2
+  - scipy=1.7.0
   - setuptools=52.0.0
-  - six=1.15.0
-  - sqlite=3.35.2
+  - six=1.16.0
+  - sqlite=3.36.0
+  - toml=0.10.2
+  - typed-ast=1.4.3
+  - typing-extensions=3.10.0.0
+  - typing_extensions=3.10.0.0
   - vc=14.2
   - vs2015_runtime=14.27.29016
   - wheel=0.36.2
   - wincertstore=0.2
-  - xarray=0.17.0
+  - xarray=0.19.0
   - xz=5.2.5
+  - zipp=3.5.0
   - zlib=1.2.11
-  - zstd=1.4.5
+  - zstd=1.4.9
 prefix: C:\Miniconda\envs\windows-3.8
```

### Comparing `cfgrib-0.9.9.0/tests/sample-data/era5-levels-corrupted.grib` & `cfgrib-0.9.9.1/tests/sample-data/era5-levels-corrupted.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/era5-levels-members.grib` & `cfgrib-0.9.9.1/tests/sample-data/era5-levels-members.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/fields_with_missing_values.grib` & `cfgrib-0.9.9.1/tests/sample-data/fields_with_missing_values.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/forecast_monthly_ukmo.grib` & `cfgrib-0.9.9.1/tests/sample-data/forecast_monthly_ukmo.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/hpa_and_pa.grib` & `cfgrib-0.9.9.1/tests/sample-data/hpa_and_pa.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/lambert_grid.grib` & `cfgrib-0.9.9.1/tests/sample-data/lambert_grid.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/multi_param_on_multi_dims.grib` & `cfgrib-0.9.9.1/tests/sample-data/multi_param_on_multi_dims.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/reduced_gg.grib` & `cfgrib-0.9.9.1/tests/sample-data/reduced_gg.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_gg_ml.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_gg_ml.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_gg_ml_g2.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_gg_ml_g2.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_gg_pl.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_gg_pl.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_gg_sfc.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_gg_sfc.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_gg_wrong_increment.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_gg_wrong_increment.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_ll_msl.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_ll_msl.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_ll_sfc.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_ll_sfc.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/regular_ll_wrong_increment.grib` & `cfgrib-0.9.9.1/tests/sample-data/regular_ll_wrong_increment.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/scanning_mode_64.grib` & `cfgrib-0.9.9.1/tests/sample-data/scanning_mode_64.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/single_gridpoint.grib` & `cfgrib-0.9.9.1/tests/sample-data/single_gridpoint.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/spherical_harmonics.grib` & `cfgrib-0.9.9.1/tests/sample-data/spherical_harmonics.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/t_analysis_and_fc_0.grib` & `cfgrib-0.9.9.1/tests/sample-data/t_analysis_and_fc_0.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/t_on_different_level_types.grib` & `cfgrib-0.9.9.1/tests/sample-data/t_on_different_level_types.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/tp_on_different_grid_resolutions.grib` & `cfgrib-0.9.9.1/tests/sample-data/tp_on_different_grid_resolutions.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/sample-data/uv_on_different_levels.grib` & `cfgrib-0.9.9.1/tests/sample-data/uv_on_different_levels.grib`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/test_20_cfcoords.py` & `cfgrib-0.9.9.1/tests/test_20_cfcoords.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import sys
 import typing as T
 
-import numpy as np  # type: ignore
+import numpy as np
 import pytest
 
-xr = pytest.importorskip("xarray")  # noqa
+pytest.importorskip("xarray")  # noqa
+
+import xarray as xr
 
 from cf2cdm import cfcoords
 
 
 @pytest.fixture
-def da1():
+def da1() -> xr.Dataset:
     latitude = [0.5, 0.0]
     longitude = [10.0, 10.5]
     time = ["2017-12-01T00:00:00", "2017-12-01T12:00:00", "2017-12-02T00:00:00"]
     level = [950, 500]
     data = xr.DataArray(
         np.zeros((2, 2, 3, 2), dtype="float32"),
         coords=[
@@ -28,15 +30,15 @@
             ("level", np.array(level), {"units": "hPa"}),
         ],
     )
     return data.to_dataset(name="da1")
 
 
 @pytest.fixture
-def da2():
+def da2() -> xr.Dataset:
     latitude = [0.5, 0.0]
     longitude = [10.0, 10.5]
     time = ["2017-12-01T00:00:00", "2017-12-01T12:00:00", "2017-12-02T00:00:00"]
     level = [950, 500]
     data = xr.DataArray(
         np.zeros((2, 2, 3, 2), dtype="float32"),
         coords=[
@@ -46,15 +48,15 @@
             ("level", np.array(level), {"units": "hPa"}),
         ],
     )
     return data.to_dataset(name="da2")
 
 
 @pytest.fixture
-def da3():
+def da3() -> xr.Dataset:
     latitude = [0.5, 0.0]
     longitude = [10.0, 10.5]
     step = [0, 24, 48]
     time = ["2017-12-01T00:00:00", "2017-12-01T12:00:00"]
     level = [950, 500]
     data = xr.DataArray(
         np.zeros((2, 2, 3, 2, 2), dtype="float32"),
@@ -70,22 +72,22 @@
             ("time", np.array(level), {"units": "hPa"}),
         ],
     )
 
     return data.to_dataset(name="da3")
 
 
-def test_match_values():
+def test_match_values() -> None:
     mapping = {"callable": len, "int": 1}  # type: T.Dict[T.Hashable, T.Any]
     res = cfcoords.match_values(callable, mapping)
 
     assert res == ["callable"]
 
 
-def test_translate_coord_direction(da1):
+def test_translate_coord_direction(da1: xr.Dataset) -> None:
     res = cfcoords.translate_coord_direction(da1, "lat", "increasing")
     assert res.lat.values[-1] > res.lat.values[0]
 
     res = cfcoords.translate_coord_direction(da1, "lat", "decreasing")
     assert res.lat.values[-1] < res.lat.values[0]
 
     res = cfcoords.translate_coord_direction(da1, "lon", "decreasing")
@@ -97,15 +99,15 @@
     res = cfcoords.translate_coord_direction(da1.isel(lon=0), "lon", "increasing")
     assert len(res.lon.shape) == 0
 
     with pytest.raises(ValueError):
         cfcoords.translate_coord_direction(da1, "lat", "wrong")
 
 
-def test_coord_translator(da1):
+def test_coord_translator(da1: xr.Dataset) -> None:
     res = cfcoords.coord_translator("level", "hPa", "decreasing", lambda x: False, "lvl", da1)
     assert da1.equals(res)
 
     with pytest.raises(ValueError):
         cfcoords.coord_translator("level", "hPa", "decreasing", lambda x: True, "lvl", da1)
 
     res = cfcoords.coord_translator("level", "hPa", "decreasing", cfcoords.is_isobaric, "lvl", da1)
@@ -117,15 +119,15 @@
     res = cfcoords.coord_translator("level", "Pa", "decreasing", cfcoords.is_isobaric, "lvl", da1)
     assert not da1.equals(res)
 
     res = cfcoords.coord_translator("step", "h", "increasing", cfcoords.is_step, "step", da1)
     assert da1.equals(res)
 
 
-def test_translate_coords(da1, da2, da3):
+def test_translate_coords(da1: xr.Dataset, da2: xr.Dataset, da3: xr.Dataset) -> None:
     res = cfcoords.translate_coords(da1)
 
     assert "latitude" in res.coords
     assert "longitude" in res.coords
     assert "time" in res.coords
 
     res = cfcoords.translate_coords(da2)
@@ -136,15 +138,15 @@
 
     res = cfcoords.translate_coords(da3, errors="ignore")
     assert "latitude" in res.coords
     assert "longitude" in res.coords
 
 
 @pytest.mark.skipif(sys.version_info < (3, 6), reason="test needs stable dict's")
-def test_translate_coords_errors(da3):
+def test_translate_coords_errors(da3: xr.Dataset) -> None:
     cfcoords.translate_coords(da3)
     cfcoords.translate_coords(da3, errors="ignore")
     with pytest.raises(RuntimeError):
         cfcoords.translate_coords(da3, errors="raise")
 
     DATA_MODEL = {"config": {"preferred_time_dimension": "valid_time"}}
     cfcoords.translate_coords(da3, DATA_MODEL)
```

### Comparing `cfgrib-0.9.9.0/tests/test_20_main_commands.py` & `cfgrib-0.9.9.1/tests/test_60_main_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os.path
 
 import click.testing
+import py
 import pytest
 
 pytest.importorskip("scipy", reason="scpy not found")
 xr = pytest.importorskip("xarray")  # noqa
 
 from cfgrib import __main__
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 
 
-def test_cfgrib_cli_to_netcdf(tmpdir):
+def test_cfgrib_cli_to_netcdf(tmpdir: py.path.local) -> None:
     runner = click.testing.CliRunner()
 
     res = runner.invoke(__main__.cfgrib_cli, ["to_netcdf"])
 
     assert res.exit_code == 0
     assert res.output == ""
 
@@ -28,15 +29,15 @@
     out = tmpdir.join("tmp.nc")
     res = runner.invoke(__main__.cfgrib_cli, ["to_netcdf", TEST_DATA, "-o" + str(out), "-cCDS"])
 
     assert res.exit_code == 0
     assert res.output == ""
 
 
-def test_cfgrib_cli_dump():
+def test_cfgrib_cli_dump() -> None:
     runner = click.testing.CliRunner()
 
     res = runner.invoke(__main__.cfgrib_cli, ["dump"])
 
     assert res.exit_code == 0
     assert res.output == ""
```

### Comparing `cfgrib-0.9.9.0/tests/test_20_messages.py` & `cfgrib-0.9.9.1/tests/test_20_messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os.path
 
-import numpy as np  # type: ignore
+import numpy as np
+import py
 import pytest
 
 from cfgrib import messages
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 
 
-def test_Message_read():
+def test_Message_read() -> None:
     with open(TEST_DATA, "rb") as file:
         res1 = messages.Message.from_file(file)
 
     assert res1.message_get("paramId") == 129
     assert res1["paramId"] == 129
     assert isinstance(res1["paramId:float"], float)
     assert res1["centre"] == "ecmf"
@@ -38,15 +39,15 @@
 
     with open(TEST_DATA, "rb") as file:
         with pytest.raises(EOFError):
             while True:
                 messages.Message.from_file(file)
 
 
-def test_Message_write(tmpdir):
+def test_Message_write(tmpdir: py.path.local) -> None:
     res = messages.Message.from_sample_name("regular_ll_pl_grib2")
     assert res["gridType"] == "regular_ll"
 
     res.message_set("Ni", 20)
     assert res["Ni"] == 20
 
     res["iDirectionIncrementInDegrees"] = 1.0
@@ -78,15 +79,15 @@
         del res["gridType"]
 
     out = tmpdir.join("test.grib")
     with open(str(out), "wb") as file:
         res.write(file)
 
 
-def test_ComputedKeysMessage_read():
+def test_ComputedKeysMessage_read() -> None:
     computed_keys = {
         "ref_time": (lambda m: str(m["dataDate"]) + str(m["dataTime"]), None),
         "error_key": (lambda m: 1 / 0, None),
         "centre": (lambda m: -1, lambda m, v: None),
     }
     with open(TEST_DATA, "rb") as file:
         res = messages.ComputedKeysMessage.from_file(file, computed_keys=computed_keys)
@@ -96,15 +97,15 @@
     assert len(res) > 100
     assert res["centre"] == -1
 
     with pytest.raises(ZeroDivisionError):
         res["error_key"]
 
 
-def test_ComputedKeysMessage_write():
+def test_ComputedKeysMessage_write() -> None:
     computed_keys = {
         "ref_time": (lambda m: "%s%04d" % (m["dataDate"], m["dataTime"]), None),
         "error_key": (lambda m: 1 / 0, None),
         "centre": (lambda m: -1, lambda m, v: None),
     }
     res = messages.ComputedKeysMessage.from_sample_name(
         "regular_ll_pl_grib2", computed_keys=computed_keys
@@ -112,15 +113,15 @@
     res["dataDate"] = 20180101
     res["dataTime"] = 0
     assert res["ref_time"] == "201801010000"
 
     res["centre"] = 1
 
 
-def test_compat_create_exclusive(tmpdir):
+def test_compat_create_exclusive(tmpdir: py.path.local) -> None:
     test_file = tmpdir.join("file.grib.idx")
 
     try:
         with messages.compat_create_exclusive(str(test_file)):
             raise RuntimeError("Test remove")
     except RuntimeError:
         pass
@@ -129,15 +130,15 @@
         file.write(b"Hi!")
 
     with pytest.raises(OSError):
         with messages.compat_create_exclusive(str(test_file)) as file:
             pass  # pragma: no cover
 
 
-def test_FileIndex():
+def test_FileIndex() -> None:
     res = messages.FileIndex.from_filestream(messages.FileStream(TEST_DATA), ["paramId"])
     assert res["paramId"] == [129, 130]
     assert len(res) == 1
     assert list(res) == ["paramId"]
     assert res.first()
 
     with pytest.raises(ValueError):
@@ -149,15 +150,15 @@
     subres = res.subindex(paramId=130)
 
     assert subres.get("paramId") == [130]
     assert subres.getone("paramId") == 130
     assert len(subres) == 1
 
 
-def test_FileIndex_from_indexpath_or_filestream(tmpdir):
+def test_FileIndex_from_indexpath_or_filestream(tmpdir: py.path.local) -> None:
     grib_file = tmpdir.join("file.grib")
 
     with open(TEST_DATA, "rb") as file:
         grib_file.write_binary(file.read())
 
     # create index file
     res = messages.FileIndex.from_indexpath_or_filestream(
@@ -192,29 +193,29 @@
 
     res = messages.FileIndex.from_indexpath_or_filestream(
         messages.FileStream(str(grib_file)), ["paramId"]
     )
     assert isinstance(res, messages.FileIndex)
 
 
-def test_FileIndex_errors():
+def test_FileIndex_errors() -> None:
     class MyMessage(messages.ComputedKeysMessage):
         computed_keys = {
             "error_key": (lambda m: bool(1 / 0), lambda m, v: None)
         }  # pragma: no branch
 
     stream = messages.FileStream(TEST_DATA, message_class=MyMessage)
     res = messages.FileIndex.from_filestream(stream, ["paramId", "error_key"])
     assert res["paramId"] == [129, 130]
     assert len(res) == 2
     assert list(res) == ["paramId", "error_key"]
     assert res["error_key"] == ["undef"]
 
 
-def test_FileStream():
+def test_FileStream() -> None:
     res = messages.FileStream(TEST_DATA)
     leader = res.first()
     assert len(leader) > 100
     assert sum(1 for _ in res) == leader["count"]
     assert len(res.index(["paramId"])) == 1
 
     # __file__ is not a GRIB, but contains the "GRIB" string, so it is a very tricky corner case
```

### Comparing `cfgrib-0.9.9.0/tests/test_25_cfmessage.py` & `cfgrib-0.9.9.1/tests/test_25_cfmessage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import os.path
 import typing as T
 
-import numpy as np  # type: ignore
+import numpy as np
 import pytest
 
 from cfgrib import cfmessage
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 
 
-def test_from_grib_date_time():
+def test_from_grib_date_time() -> None:
     message = {"dataDate": 20160706, "dataTime": 1944}
     result = cfmessage.from_grib_date_time(message)
 
     assert result == 1467834240
 
 
-def test_to_grib_date_time():
+def test_to_grib_date_time() -> None:
     message = {}  # type: T.Dict[str, T.Any]
-    datetime_ns = int(np.datetime64("2001-10-11T01:01:00", "ns"))
+    datetime_ns = np.datetime64("2001-10-11T01:01:00", "ns").item()
 
     cfmessage.to_grib_date_time(message, datetime_ns)
 
     assert message["dataDate"] == 20011011
     assert message["dataTime"] == 101
 
 
-def test_from_grib_step():
+def test_from_grib_step() -> None:
     message = {"endStep": 1, "stepUnits": 1}
     step_seconds = cfmessage.from_grib_step(message)
 
     assert step_seconds == 1
 
 
-def test_to_grib_step():
+def test_to_grib_step() -> None:
     message = {}  # type: T.Dict[str, T.Any]
     step_ns = 3600 * 1_000_000_000
 
     cfmessage.to_grib_step(message, step_ns, step_unit=1)
 
     assert message["endStep"] == 1
     assert message["stepUnits"] == 1
 
     with pytest.raises(ValueError):
         cfmessage.to_grib_step(message, 0, step_unit=3)
 
 
-def test_build_valid_time():
+def test_build_valid_time() -> None:
     forecast_reference_time = np.array(0)
     forecast_period = np.array(0)
 
     dims, data = cfmessage.build_valid_time(forecast_reference_time, forecast_period)
 
     assert dims == ()
     assert data.shape == ()
```

### Comparing `cfgrib-0.9.9.0/tests/test_30_dataset.py` & `cfgrib-0.9.9.1/tests/test_30_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os.path
 import pathlib
+import typing as T
 
-import numpy as np  # type: ignore
+import numpy as np
 import pytest
 
 from cfgrib import cfmessage, dataset, messages
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 TEST_DATA_UKMO = os.path.join(SAMPLE_DATA_FOLDER, "forecast_monthly_ukmo.grib")
+TEST_DATA_SCALAR_TIME = os.path.join(SAMPLE_DATA_FOLDER, "era5-single-level-scalar-time.grib")
 
 
-def test_enforce_unique_attributes():
+def test_enforce_unique_attributes() -> None:
     assert dataset.enforce_unique_attributes({"key": [1]}, ["key"])
     assert not dataset.enforce_unique_attributes({"key": ["undef"]}, ["key"])
 
     with pytest.raises(dataset.DatasetBuildError):
         assert dataset.enforce_unique_attributes({"key": [1, 2]}, ["key"])
 
 
-def test_Variable():
+def test_Variable() -> None:
     res = dataset.Variable(dimensions=("lat",), data=np.array([0.0]), attributes={})
 
     assert res == res
     assert res != 1
 
 
 @pytest.mark.parametrize(
@@ -31,50 +33,50 @@
     [
         (([1, 5],), (10,), ([1, 5],)),
         ((np.array([1]),), (10,), ([1],)),
         ((slice(0, 3, 2),), (10,), ([0, 2],)),
         ((1,), (10,), ([1],)),
     ],
 )
-def test_expand_item(item, shape, expected):
+def test_expand_item(item: T.Any, shape: T.Any, expected: T.Any) -> None:
     assert dataset.expand_item(item, shape) == expected
 
 
-def test_expand_item_error():
+def test_expand_item_error() -> None:
     with pytest.raises(TypeError):
         dataset.expand_item((None,), (1,))
 
 
-def test_dict_merge():
+def test_dict_merge() -> None:
     master = {"one": 1}
     dataset.dict_merge(master, {"two": 2})
     assert master == {"one": 1, "two": 2}
     dataset.dict_merge(master, {"two": 2})
     assert master == {"one": 1, "two": 2}
 
     with pytest.raises(dataset.DatasetBuildError):
         dataset.dict_merge(master, {"two": 3})
 
 
-def test_encode_cf_first():
+def test_encode_cf_first() -> None:
     assert dataset.encode_cf_first({})
 
 
-def test_build_data_var_components_no_encode():
+def test_build_data_var_components_no_encode() -> None:
     index_keys = sorted(dataset.INDEX_KEYS + ["time", "step"])
     index = messages.FileStream(path=TEST_DATA).index(index_keys).subindex(paramId=130)
     dims, data_var, coord_vars = dataset.build_variable_components(index=index)
     assert dims == {"number": 10, "dataDate": 2, "dataTime": 2, "level": 2, "values": 7320}
     assert data_var.data.shape == (10, 2, 2, 2, 7320)
 
     # equivalent to not np.isnan without importing numpy
     assert data_var.data[:, :, :, :, :].mean() > 0.0
 
 
-def test_build_data_var_components_encode_cf_geography():
+def test_build_data_var_components_encode_cf_geography() -> None:
     stream = messages.FileStream(path=TEST_DATA, message_class=cfmessage.CfMessage)
     index_keys = sorted(dataset.INDEX_KEYS + ["time", "step"])
     index = stream.index(index_keys).subindex(paramId=130)
     dims, data_var, coord_vars = dataset.build_variable_components(
         index=index, encode_cf="geography"
     )
     assert dims == {
@@ -87,15 +89,15 @@
     }
     assert data_var.data.shape == (10, 2, 2, 2, 61, 120)
 
     # equivalent to not np.isnan without importing numpy
     assert data_var.data[:, :, :, :, :, :].mean() > 0.0
 
 
-def test_build_dataset_components_time_dims():
+def test_build_dataset_components_time_dims() -> None:
     index_keys = sorted(dataset.INDEX_KEYS + ["time", "step"])
     index = dataset.open_fileindex(TEST_DATA_UKMO, "warn", "{path}.{short_hash}.idx", index_keys)
     dims = dataset.build_dataset_components(index, read_keys=[])[0]
     assert dims == {
         "latitude": 6,
         "longitude": 11,
         "number": 28,
@@ -117,15 +119,15 @@
     time_dims = ["indexing_time", "step"]
     index_keys = sorted(dataset.INDEX_KEYS + time_dims)
     index = dataset.open_fileindex(TEST_DATA_UKMO, "warn", "{path}.{short_hash}.idx", index_keys)
     dims, *_ = dataset.build_dataset_components(index, read_keys=[], time_dims=time_dims)
     assert dims == {"number": 28, "indexing_time": 2, "step": 20, "latitude": 6, "longitude": 11}
 
 
-def test_Dataset():
+def test_Dataset() -> None:
     res = dataset.open_file(TEST_DATA)
     assert "Conventions" in res.attributes
     assert "institution" in res.attributes
     assert "history" in res.attributes
     assert res.attributes["GRIB_edition"] == 1
     assert tuple(res.dimensions.keys()) == (
         "number",
@@ -137,36 +139,36 @@
     assert len(res.variables) == 9
 
     res1 = dataset.open_file(pathlib.Path(TEST_DATA))
 
     assert res1 == res
 
 
-def test_Dataset_no_encode():
+def test_Dataset_no_encode() -> None:
     res = dataset.open_file(TEST_DATA, encode_cf=())
     assert "Conventions" in res.attributes
     assert "institution" in res.attributes
     assert "history" in res.attributes
     assert res.attributes["GRIB_edition"] == 1
     assert tuple(res.dimensions.keys()) == ("number", "dataDate", "dataTime", "level", "values")
     assert len(res.variables) == 9
 
 
-def test_Dataset_encode_cf_time():
+def test_Dataset_encode_cf_time() -> None:
     res = dataset.open_file(TEST_DATA, encode_cf=("time",))
     assert "history" in res.attributes
     assert res.attributes["GRIB_edition"] == 1
     assert tuple(res.dimensions.keys()) == ("number", "time", "level", "values")
     assert len(res.variables) == 9
 
     # equivalent to not np.isnan without importing numpy
     assert res.variables["t"].data[:, :, :, :].mean() > 0.0
 
 
-def test_Dataset_encode_cf_geography():
+def test_Dataset_encode_cf_geography() -> None:
     res = dataset.open_file(TEST_DATA, encode_cf=("geography",))
     assert "history" in res.attributes
     assert res.attributes["GRIB_edition"] == 1
     assert tuple(res.dimensions.keys()) == (
         "number",
         "dataDate",
         "dataTime",
@@ -176,46 +178,54 @@
     )
     assert len(res.variables) == 9
 
     # equivalent to not np.isnan without importing numpy
     assert res.variables["t"].data[:, :, :, :, :, :].mean() > 0.0
 
 
-def test_Dataset_encode_cf_vertical():
+def test_Dataset_encode_cf_vertical() -> None:
     res = dataset.open_file(TEST_DATA, encode_cf=("vertical",))
     assert "history" in res.attributes
     assert res.attributes["GRIB_edition"] == 1
     expected_dimensions = ("number", "dataDate", "dataTime", "isobaricInhPa", "values")
     assert tuple(res.dimensions.keys()) == expected_dimensions
     assert len(res.variables) == 9
 
     # equivalent to not np.isnan without importing numpy
     assert res.variables["t"].data[:, :, :, :, :].mean() > 0.0
 
 
-def test_Dataset_reguler_gg_surface():
+def test_Dataset_reguler_gg_surface() -> None:
     path = os.path.join(SAMPLE_DATA_FOLDER, "regular_gg_sfc.grib")
     res = dataset.open_file(path)
 
     assert res.dimensions == {"latitude": 96, "longitude": 192}
     assert np.allclose(res.variables["latitude"].data[:2], [88.57216851, 86.72253095])
 
 
-def test_Dataset_extra_coords():
+def test_Dataset_extra_coords() -> None:
     res = dataset.open_file(TEST_DATA, extra_coords={"experimentVersionNumber": "time"})
     assert "experimentVersionNumber" in res.variables
     assert res.variables["experimentVersionNumber"].dimensions == ("time",)
 
 
-def test_Dataet_extra_coords_error():
+def test_Dataset_scalar_extra_coords() -> None:
+    res = dataset.open_file(
+        TEST_DATA_SCALAR_TIME, extra_coords={"experimentVersionNumber": "time"}
+    )
+    assert "experimentVersionNumber" in res.variables
+    assert res.variables["experimentVersionNumber"].dimensions == ()
+
+
+def test_Dataset_extra_coords_error() -> None:
     with pytest.raises(ValueError):
         dataset.open_file(TEST_DATA, extra_coords={"validityDate": "number"})
 
 
-def test_OnDiskArray():
+def test_OnDiskArray() -> None:
     res = dataset.open_file(TEST_DATA).variables["t"]
 
     assert isinstance(res.data, dataset.OnDiskArray)
     assert np.allclose(
         res.data[2:4:2, [0, 3], 0, 0, 0], res.data.build_array()[2:4:2, [0, 3], 0, 0, 0]
     )
```

### Comparing `cfgrib-0.9.9.0/tests/test_40_xarray_store.ipynb` & `cfgrib-0.9.9.1/tests/test_40_xarray_store.ipynb`

 * *Files identical despite different names*

### Comparing `cfgrib-0.9.9.0/tests/test_40_xarray_store.py` & `cfgrib-0.9.9.1/tests/test_40_xarray_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 TEST_CORRUPTED = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-corrupted.grib")
 TEST_DATASETS = os.path.join(SAMPLE_DATA_FOLDER, "t_on_different_level_types.grib")
 TEST_IGNORE = os.path.join(SAMPLE_DATA_FOLDER, "uv_on_different_levels.grib")
 
 
-def test_open_dataset():
+def test_open_dataset() -> None:
     res = xarray_store.open_dataset(TEST_DATA)
 
     assert res.attrs["GRIB_edition"] == 1
 
     var = res["t"]
     assert var.attrs["GRIB_gridType"] == "regular_ll"
     assert var.attrs["units"] == "K"
@@ -34,71 +34,71 @@
     res = xarray_store.open_dataset(TEST_IGNORE, backend_kwargs={"errors": "ignore"})
     assert "isobaricInhPa" in res.dims
 
     with pytest.raises(ValueError):
         xarray_store.open_dataset(TEST_IGNORE, backend_kwargs={"errors": "raise"})
 
 
-def test_open_dataset_corrupted():
+def test_open_dataset_corrupted() -> None:
     res = xarray_store.open_dataset(TEST_CORRUPTED)
 
     assert res.attrs["GRIB_edition"] == 1
     assert len(res.data_vars) == 1
 
     with pytest.raises(Exception):
         xarray_store.open_dataset(TEST_CORRUPTED, backend_kwargs={"grib_errors": "raise"})
 
 
-def test_open_dataset_encode_cf_time():
+def test_open_dataset_encode_cf_time() -> None:
     backend_kwargs = {"encode_cf": ("time",)}
     res = xarray_store.open_dataset(TEST_DATA, backend_kwargs=backend_kwargs)
 
     assert res.attrs["GRIB_edition"] == 1
     assert res["t"].attrs["GRIB_gridType"] == "regular_ll"
     assert res["t"].attrs["GRIB_units"] == "K"
     assert res["t"].dims == ("number", "time", "level", "values")
 
     assert res["t"].mean() > 0.0
 
 
-def test_open_dataset_encode_cf_vertical():
+def test_open_dataset_encode_cf_vertical() -> None:
     backend_kwargs = {"encode_cf": ("vertical",)}
     res = xarray_store.open_dataset(TEST_DATA, backend_kwargs=backend_kwargs)
 
     var = res["t"]
     assert var.dims == ("number", "dataDate", "dataTime", "isobaricInhPa", "values")
 
     assert var.mean() > 0.0
 
 
-def test_open_dataset_encode_cf_geography():
+def test_open_dataset_encode_cf_geography() -> None:
     backend_kwargs = {"encode_cf": ("geography",)}
     res = xarray_store.open_dataset(TEST_DATA, backend_kwargs=backend_kwargs)
 
     assert res.attrs["GRIB_edition"] == 1
 
     var = res["t"]
     assert var.attrs["GRIB_gridType"] == "regular_ll"
     assert var.attrs["GRIB_units"] == "K"
     assert var.dims == ("number", "dataDate", "dataTime", "level", "latitude", "longitude")
 
     assert var.mean() > 0.0
 
 
-def test_open_dataset_eccodes():
+def test_open_dataset_eccodes() -> None:
     res = xarray_store.open_dataset(TEST_DATA)
 
     assert res.attrs["GRIB_edition"] == 1
 
     var = res["t"]
     assert var.attrs["GRIB_gridType"] == "regular_ll"
     assert var.attrs["units"] == "K"
     assert var.dims == ("number", "time", "isobaricInhPa", "latitude", "longitude")
 
     assert var.mean() > 0.0
 
 
-def test_open_datasets():
+def test_open_datasets() -> None:
     res = xarray_store.open_datasets(TEST_DATASETS)
 
     assert len(res) > 1
     assert res[0].attrs["GRIB_centre"] == "ecmf"
```

### Comparing `cfgrib-0.9.9.0/tests/test_40_xarray_to_grib_regular_ll.py` & `cfgrib-0.9.9.1/tests/test_40_xarray_to_grib_regular_ll.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,72 @@
-import numpy as np  # type: ignore
+import typing as T
+
+import numpy as np
+import py
 import pytest
 
 pd = pytest.importorskip("pandas")  # noqa
-xr = pytest.importorskip("xarray")  # noqa
+pytest.importorskip("xarray")  # noqa
+
+import xarray as xr
 
 from cfgrib import xarray_to_grib
 
 
 @pytest.fixture()
-def canonic_da():
+def canonic_da() -> xr.DataArray:
+    coords: T.List[T.Any] = [
+        pd.date_range("2018-01-01T00:00", "2018-01-02T12:00", periods=4),
+        pd.timedelta_range(0, "12h", periods=2),
+        [1000.0, 850.0, 500.0],
+        np.linspace(90.0, -90.0, 5),
+        np.linspace(0.0, 360.0, 6, endpoint=False),
+    ]
     da = xr.DataArray(
         np.zeros((4, 2, 3, 5, 6)),
-        coords=[
-            pd.date_range("2018-01-01T00:00", "2018-01-02T12:00", periods=4),
-            pd.timedelta_range(0, "12h", periods=2),
-            [1000.0, 850.0, 500.0],
-            np.linspace(90.0, -90.0, 5),
-            np.linspace(0.0, 360.0, 6, endpoint=False),
-        ],
+        coords=coords,
         dims=["time", "step", "isobaricInhPa", "latitude", "longitude"],
     )
     return da
 
 
-def test_canonical_dataarray_to_grib_with_grib_keys(canonic_da, tmpdir):
+def test_canonical_dataarray_to_grib_with_grib_keys(
+    canonic_da: xr.DataArray, tmpdir: py.path.local
+) -> None:
     out_path = tmpdir.join("res.grib")
     grib_keys = {"gridType": "regular_ll"}
     with open(str(out_path), "wb") as file:
         xarray_to_grib.canonical_dataarray_to_grib(canonic_da, file, grib_keys=grib_keys)
 
 
-def test_canonical_dataarray_to_grib_detect_grib_keys(canonic_da, tmpdir):
+def test_canonical_dataarray_to_grib_detect_grib_keys(
+    canonic_da: xr.DataArray, tmpdir: py.path.local
+) -> None:
     out_path = tmpdir.join("res.grib")
     with open(str(out_path), "wb") as file:
         xarray_to_grib.canonical_dataarray_to_grib(canonic_da, file)
 
 
-def test_canonical_dataarray_to_grib_conflicting_detect_grib_keys(canonic_da, tmpdir):
+def test_canonical_dataarray_to_grib_conflicting_detect_grib_keys(
+    canonic_da: xr.DataArray, tmpdir: py.path.local
+) -> None:
     out_path = tmpdir.join("res.grib")
     grib_keys = {"gridType": "reduced_ll"}
     with open(str(out_path), "wb") as file:
         with pytest.raises(ValueError):
             xarray_to_grib.canonical_dataarray_to_grib(canonic_da, file, grib_keys=grib_keys)
 
 
-def test_canonical_dataset_to_grib(canonic_da, tmpdir):
+def test_canonical_dataset_to_grib(canonic_da: xr.DataArray, tmpdir: py.path.local) -> None:
     out_path = tmpdir.join("res.grib")
     canonic_ds = canonic_da.to_dataset(name="t")
     with pytest.warns(FutureWarning):
         xarray_to_grib.canonical_dataset_to_grib(canonic_ds, str(out_path))
 
     xarray_to_grib.canonical_dataset_to_grib(canonic_ds, str(out_path), no_warn=True)
 
 
-def test_to_grib(canonic_da, tmpdir):
+def test_to_grib(canonic_da: xr.DataArray, tmpdir: py.path.local) -> None:
     out_path = tmpdir.join("res.grib")
     canonic_ds = canonic_da.to_dataset(name="t")
     with pytest.warns(FutureWarning):
         xarray_to_grib.to_grib(canonic_ds, str(out_path))
```

### Comparing `cfgrib-0.9.9.0/tests/test_50_datamodels.py` & `cfgrib-0.9.9.1/tests/test_50_datamodels.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cfgrib import xarray_store
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA1 = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 TEST_DATA2 = os.path.join(SAMPLE_DATA_FOLDER, "lambert_grid.grib")
 
 
-def test_cds():
+def test_cds() -> None:
     ds = xarray_store.open_dataset(TEST_DATA1)
 
     res = cfcoords.translate_coords(ds, coord_model=datamodels.CDS)
 
     assert set(res.dims) == {"forecast_reference_time", "lat", "lon", "plev", "realization"}
     assert set(res.coords) == {
         "forecast_reference_time",
@@ -39,15 +39,15 @@
         "lat",
         "leadtime",
         "lon",
         "time",
     }
 
 
-def test_ecmwf():
+def test_ecmwf() -> None:
     ds = xarray_store.open_dataset(TEST_DATA1)
 
     res = cfcoords.translate_coords(ds, coord_model=datamodels.ECMWF)
 
     assert set(res.dims) == {"latitude", "level", "longitude", "number", "time"}
     assert set(res.coords) == {
         "latitude",
```

### Comparing `cfgrib-0.9.9.0/tests/test_50_sample_data.py` & `cfgrib-0.9.9.1/tests/test_50_sample_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os.path
+import typing as T
 
+import py
 import pytest
 
 xr = pytest.importorskip("xarray")  # noqa
 
 from cfgrib import xarray_store, xarray_to_grib
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
@@ -24,40 +26,40 @@
         "regular_ll_msl",
         "scanning_mode_64",
         "single_gridpoint",
         "spherical_harmonics",
         "t_analysis_and_fc_0",
     ],
 )
-def test_open_dataset(grib_name):
+def test_open_dataset(grib_name: str) -> None:
     grib_path = os.path.join(SAMPLE_DATA_FOLDER, grib_name + ".grib")
     res = xarray_store.open_dataset(grib_path, cache=False)
     print(res)
 
 
 @pytest.mark.parametrize(
     "grib_name",
     [
         "hpa_and_pa",
         "t_on_different_level_types",
         "tp_on_different_grid_resolutions",
         "uv_on_different_levels",
     ],
 )
-def test_open_dataset_fail(grib_name):
+def test_open_dataset_fail(grib_name: str) -> None:
     grib_path = os.path.join(SAMPLE_DATA_FOLDER, grib_name + ".grib")
 
     with pytest.raises(ValueError):
         xarray_store.open_dataset(grib_path, cache=False, backend_kwargs={"errors": "raise"})
 
 
 @pytest.mark.parametrize(
     "grib_name", ["hpa_and_pa", "t_on_different_level_types", "tp_on_different_grid_resolutions"]
 )
-def test_open_datasets(grib_name):
+def test_open_datasets(grib_name: str) -> None:
     grib_path = os.path.join(SAMPLE_DATA_FOLDER, grib_name + ".grib")
 
     res = xarray_store.open_datasets(grib_path)
 
     assert len(res) > 1
 
 
@@ -75,17 +77,31 @@
         "regular_ll_sfc",
         "regular_ll_msl",
         "scanning_mode_64",
         pytest.param("spherical_harmonics", marks=pytest.mark.xfail),
         "t_analysis_and_fc_0",
     ],
 )
-def test_canonical_dataset_to_grib(grib_name, tmpdir):
+def test_canonical_dataset_to_grib(grib_name: str, tmpdir: py.path.local) -> None:
     grib_path = os.path.join(SAMPLE_DATA_FOLDER, grib_name + ".grib")
     out_path = str(tmpdir.join(grib_name + ".grib"))
 
     res = xarray_store.open_dataset(grib_path)
 
     with pytest.warns(FutureWarning):
         xarray_to_grib.canonical_dataset_to_grib(res, out_path)
     reread = xarray_store.open_dataset(out_path)
     assert res.equals(reread)
+
+
+@pytest.mark.parametrize(
+    "grib_name,ndims", [("era5-levels-members", 1), ("era5-single-level-scalar-time", 0),],
+)
+def test_open_dataset_extra_coords(grib_name: str, ndims: T.Any) -> None:
+    grib_path = os.path.join(SAMPLE_DATA_FOLDER, grib_name + ".grib")
+    res = xarray_store.open_dataset(
+        grib_path,
+        backend_kwargs={"extra_coords": {"experimentVersionNumber": "time"}},
+        cache=False,
+    )
+    assert "experimentVersionNumber" in res.coords
+    assert len(res["experimentVersionNumber"].dims) == ndims
```

### Comparing `cfgrib-0.9.9.0/tests/test_50_xarray_getitem.py` & `cfgrib-0.9.9.1/tests/test_50_xarray_getitem.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,56 +7,56 @@
 from cfgrib import xarray_store
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "era5-levels-members.grib")
 
 
 @pytest.mark.parametrize("cache", [True, False])
-def test_all(cache):
+def test_all(cache: bool) -> None:
     da = xarray_store.open_dataset(TEST_DATA, cache=cache).data_vars["t"]
     va = da.values[:]
 
     assert va.shape == (10, 4, 2, 61, 120)
 
     assert da.mean() == va.mean()
 
 
 @pytest.mark.parametrize("cache", [True, False])
-def test_getitem_int(cache):
+def test_getitem_int(cache: bool) -> None:
     da = xarray_store.open_dataset(TEST_DATA, cache=cache).data_vars["t"]
     va = da.values[:]
 
     assert da.isel(isobaricInhPa=1).values.shape == va[:, :, 1].shape
     assert da.isel(isobaricInhPa=1).mean() == va[:, :, 1].mean()
     assert da.sel(isobaricInhPa=500).mean() == va[:, :, 1].mean()
 
 
 @pytest.mark.parametrize("cache", [True, False])
-def test_getitem_slice(cache):
+def test_getitem_slice(cache: bool) -> None:
     da = xarray_store.open_dataset(TEST_DATA, cache=cache).data_vars["t"]
     va = da.values[:]
 
     assert da.isel(number=slice(2, 6)).mean() == va[2:6].mean()
     assert da.isel(number=slice(2, 6, 2)).mean() == va[2:6:2].mean()
     # NOTE: label based indexing in xarray is inclusive of both the start and stop bounds.
     assert da.sel(number=slice(2, 6)).mean() == va[2:7].mean()
     assert da.sel(number=slice(2, 6, 2)).mean() == va[2:7:2].mean()
 
 
 @pytest.mark.parametrize("cache", [True, False])
-def test_getitem_list(cache):
+def test_getitem_list(cache: bool) -> None:
     da = xarray_store.open_dataset(TEST_DATA, cache=cache).data_vars["t"]
     va = da.values[:]
 
     assert da.isel(number=[2, 3, 4, 5]).mean() == va[[2, 3, 4, 5]].mean()
     assert da.isel(number=[4, 3, 2, 5]).mean() == va[[4, 3, 2, 5]].mean()
     assert da.sel(number=[2, 3, 4, 5]).mean() == va[[2, 3, 4, 5]].mean()
     assert da.sel(number=[4, 3, 2, 5]).mean() == va[[4, 3, 2, 5]].mean()
 
 
 @pytest.mark.parametrize("cache", [True, False])
-def test_getitem_latlon(cache):
+def test_getitem_latlon(cache: bool) -> None:
     da = xarray_store.open_dataset(TEST_DATA, cache=cache).data_vars["t"]
     va = da.values[:]
 
     assert da.isel(latitude=slice(0, 3), longitude=slice(0, 33)).mean() == va[..., :3, :33].mean()
     assert da.sel(latitude=slice(90, 0), longitude=slice(0, 90)).mean() == va[..., :31, :31].mean()
```

### Comparing `cfgrib-0.9.9.0/tests/test_50_xarray_plugin.py` & `cfgrib-0.9.9.1/tests/test_50_xarray_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,32 @@
     "xarray", minversion="0.17.1.dev0", reason="required xarray>=0.18"
 )  # noqa
 
 SAMPLE_DATA_FOLDER = os.path.join(os.path.dirname(__file__), "sample-data")
 TEST_DATA = os.path.join(SAMPLE_DATA_FOLDER, "regular_ll_sfc.grib")
 
 
-def test_plugin():
+def test_plugin() -> None:
     engines = xr.backends.list_engines()
     cfgrib_entrypoint = engines["cfgrib"]
     assert cfgrib_entrypoint.__module__ == "cfgrib.xarray_plugin"
 
 
-def test_xr_open_dataset():
+def test_xr_open_dataset() -> None:
     expected = {
         "latitude": 37,
         "longitude": 72,
     }
 
     ds = xr.open_dataset(TEST_DATA, engine="cfgrib")
     assert ds.dims == expected
     assert list(ds.data_vars) == ["skt"]
 
 
-def test_read():
+def test_read() -> None:
     expected = {
         "latitude": 37,
         "longitude": 72,
     }
     import cfgrib.xarray_plugin
 
     opener = cfgrib.xarray_plugin.CfGribBackend()
```

### Comparing `cfgrib-0.9.9.0/tox.ini` & `cfgrib-0.9.9.1/tox.ini`

 * *Files identical despite different names*

