# Comparing `tmp/dsigma-0.7.2.tar.gz` & `tmp/dsigma-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsigma-0.7.2.tar", last modified: Fri Jun  2 19:17:12 2023, max compression
+gzip compressed data, was "dsigma-1.0.0.tar", last modified: Sun May 26 20:24:26 2024, max compression
```

## Comparing `dsigma-0.7.2.tar` & `dsigma-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.957168 dsigma-0.7.2/
--rw-r--r--   0 research  (1001) research  (1001)     2232 2023-06-02 18:56:14.000000 dsigma-0.7.2/CHANGELOG.md
--rw-r--r--   0 research  (1001) research  (1001)     1107 2023-04-26 17:55:50.000000 dsigma-0.7.2/LICENSE
--rw-r--r--   0 research  (1001) research  (1001)      115 2023-04-26 17:55:50.000000 dsigma-0.7.2/MANIFEST.in
--rw-r--r--   0 research  (1001) research  (1001)     3880 2023-06-02 19:17:12.957168 dsigma-0.7.2/PKG-INFO
--rw-r--r--   0 research  (1001) research  (1001)     2251 2023-04-26 17:55:50.000000 dsigma-0.7.2/README.md
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.955168 dsigma-0.7.2/dsigma/
--rw-r--r--   0 research  (1001) research  (1001)      366 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/__init__.py
--rw-r--r--   0 research  (1001) research  (1001)     7528 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/helpers.py
--rw-r--r--   0 research  (1001) research  (1001)     8721 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/jackknife.py
--rw-r--r--   0 research  (1001) research  (1001)    10075 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/physics.py
--rw-r--r--   0 research  (1001) research  (1001)    20046 2023-04-28 20:13:07.000000 dsigma-0.7.2/dsigma/precompute.py
--rw-r--r--   0 research  (1001) research  (1001)   968246 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma/precompute_engine.c
--rw-r--r--   0 research  (1001) research  (1001)    10368 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/precompute_engine.pyx
--rw-r--r--   0 research  (1001) research  (1001)    18468 2023-04-28 20:18:19.000000 dsigma-0.7.2/dsigma/stacking.py
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.956168 dsigma-0.7.2/dsigma/surveys/
--rw-r--r--   0 research  (1001) research  (1001)       81 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/__init__.py
--rw-r--r--   0 research  (1001) research  (1001)      715 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/cfhtls.py
--rw-r--r--   0 research  (1001) research  (1001)     6238 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/des.py
--rw-r--r--   0 research  (1001) research  (1001)     4601 2023-04-26 17:55:50.000000 dsigma-0.7.2/dsigma/surveys/hsc.py
--rw-r--r--   0 research  (1001) research  (1001)     3783 2023-06-02 19:03:36.000000 dsigma-0.7.2/dsigma/surveys/kids.py
-drwxr-xr-x   0 research  (1001) research  (1001)        0 2023-06-02 19:17:12.956168 dsigma-0.7.2/dsigma.egg-info/
--rw-r--r--   0 research  (1001) research  (1001)     3880 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/PKG-INFO
--rw-r--r--   0 research  (1001) research  (1001)      505 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/SOURCES.txt
--rw-r--r--   0 research  (1001) research  (1001)        1 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/dependency_links.txt
--rw-r--r--   0 research  (1001) research  (1001)       54 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/requires.txt
--rw-r--r--   0 research  (1001) research  (1001)        7 2023-06-02 19:17:12.000000 dsigma-0.7.2/dsigma.egg-info/top_level.txt
--rw-r--r--   0 research  (1001) research  (1001)      643 2023-06-02 19:01:10.000000 dsigma-0.7.2/pyproject.toml
--rw-r--r--   0 research  (1001) research  (1001)       38 2023-06-02 19:17:12.957168 dsigma-0.7.2/setup.cfg
--rw-r--r--   0 research  (1001) research  (1001)      248 2023-04-26 17:55:50.000000 dsigma-0.7.2/setup.py
+drwxr-xr-x   0 university  (1002) university  (1002)        0 2024-05-26 20:24:26.800975 dsigma-1.0.0/
+-rw-r--r--   0 university  (1002) university  (1002)     2730 2024-05-26 20:17:38.000000 dsigma-1.0.0/CHANGELOG.md
+-rw-r--r--   0 university  (1002) university  (1002)     1107 2024-05-19 20:46:55.000000 dsigma-1.0.0/LICENSE
+-rw-r--r--   0 university  (1002) university  (1002)      166 2024-05-26 20:24:08.000000 dsigma-1.0.0/MANIFEST.in
+-rw-r--r--   0 university  (1002) university  (1002)     4312 2024-05-26 20:24:26.800975 dsigma-1.0.0/PKG-INFO
+-rw-r--r--   0 university  (1002) university  (1002)     2251 2024-05-20 02:51:38.000000 dsigma-1.0.0/README.md
+drwxr-xr-x   0 university  (1002) university  (1002)        0 2024-05-26 20:24:26.796975 dsigma-1.0.0/dsigma/
+-rw-r--r--   0 university  (1002) university  (1002)      310 2024-05-26 20:18:00.000000 dsigma-1.0.0/dsigma/__init__.py
+-rw-r--r--   0 university  (1002) university  (1002)     7528 2024-05-20 02:51:38.000000 dsigma-1.0.0/dsigma/helpers.py
+-rw-r--r--   0 university  (1002) university  (1002)     8805 2024-05-24 18:19:50.000000 dsigma-1.0.0/dsigma/jackknife.py
+-rw-r--r--   0 university  (1002) university  (1002)    10329 2024-05-24 20:26:26.000000 dsigma-1.0.0/dsigma/physics.py
+-rw-r--r--   0 university  (1002) university  (1002)    20597 2024-05-24 20:18:16.000000 dsigma-1.0.0/dsigma/precompute.py
+-rw-r--r--   0 university  (1002) university  (1002)    10534 2024-05-24 13:46:10.000000 dsigma-1.0.0/dsigma/precompute_engine.pyx
+-rw-r--r--   0 university  (1002) university  (1002)    18584 2024-05-24 22:53:20.000000 dsigma-1.0.0/dsigma/stacking.py
+drwxr-xr-x   0 university  (1002) university  (1002)        0 2024-05-26 20:24:26.799975 dsigma-1.0.0/dsigma/surveys/
+-rw-r--r--   0 university  (1002) university  (1002)       81 2024-05-19 20:46:55.000000 dsigma-1.0.0/dsigma/surveys/__init__.py
+-rw-r--r--   0 university  (1002) university  (1002)      715 2024-05-20 02:51:38.000000 dsigma-1.0.0/dsigma/surveys/cfhtls.py
+-rw-r--r--   0 university  (1002) university  (1002)     6238 2024-05-20 02:51:38.000000 dsigma-1.0.0/dsigma/surveys/des.py
+-rw-r--r--   0 university  (1002) university  (1002)     4601 2024-05-20 02:51:38.000000 dsigma-1.0.0/dsigma/surveys/hsc.py
+-rw-r--r--   0 university  (1002) university  (1002)     3783 2024-05-20 02:51:38.000000 dsigma-1.0.0/dsigma/surveys/kids.py
+drwxr-xr-x   0 university  (1002) university  (1002)        0 2024-05-26 20:24:26.799975 dsigma-1.0.0/dsigma.egg-info/
+-rw-r--r--   0 university  (1002) university  (1002)     4312 2024-05-26 20:24:26.000000 dsigma-1.0.0/dsigma.egg-info/PKG-INFO
+-rw-r--r--   0 university  (1002) university  (1002)      478 2024-05-26 20:24:26.000000 dsigma-1.0.0/dsigma.egg-info/SOURCES.txt
+-rw-r--r--   0 university  (1002) university  (1002)        1 2024-05-26 20:24:26.000000 dsigma-1.0.0/dsigma.egg-info/dependency_links.txt
+-rw-r--r--   0 university  (1002) university  (1002)       54 2024-05-26 20:24:26.000000 dsigma-1.0.0/dsigma.egg-info/requires.txt
+-rw-r--r--   0 university  (1002) university  (1002)        7 2024-05-26 20:24:26.000000 dsigma-1.0.0/dsigma.egg-info/top_level.txt
+-rw-r--r--   0 university  (1002) university  (1002)      944 2024-05-20 23:55:24.000000 dsigma-1.0.0/pyproject.toml
+-rw-r--r--   0 university  (1002) university  (1002)       38 2024-05-26 20:24:26.800975 dsigma-1.0.0/setup.cfg
+-rw-r--r--   0 university  (1002) university  (1002)      408 2024-05-20 23:46:46.000000 dsigma-1.0.0/setup.py
```

### Comparing `dsigma-0.7.2/CHANGELOG.md` & `dsigma-1.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 # Changelog
 Notable changes to dsigma will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
+## [1.0.0] - 2024-05-26
 
-## [0.7.2] - 2023-06-02
+### Added
+- added `dsigma.stacking.mean_critical_surface_density`
 
 ### Changed
+- photometric redshift correction now always applied when computing the mean source redshift
+- `dsigma.stacking.lens_magnification_bias` now uses `dsigma.stacking.mean_critical_surface_density` to estimate the critical surface density and not calculate it based on the mean lens and source redshift
+- `dsigma.physics.lens_magnification_shear_bias` can now use angles expressed with `astropy` units
+
+## [0.7.2] - 2023-06-02
+
+### Added
 
 - `dsigma.stacking.lens_magnification_bias` can now be used to compute the bias in the tangential shear
+
+### Changed
+
 - mean source redshift now takes into account n(z)'s passed to `dsigma.precompute.precompute`
 
 ### Fixed
 
 - incompatibility with numpy 1.24
 - bug in `dsigma.stacking.tangential_shear` when `random_subtraction=True`
 - error in tomographic redshift bin assignment for KiDS, sources with photo-z's at the bin edges were assigned to the wrong tomographic bin, this biased KiDS lensing measurements by order 2%
```

### Comparing `dsigma-0.7.2/LICENSE` & `dsigma-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.2/README.md` & `dsigma-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.2/dsigma/helpers.py` & `dsigma-1.0.0/dsigma/helpers.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.2/dsigma/jackknife.py` & `dsigma-1.0.0/dsigma/jackknife.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     continous field. The centers are defined in cartesian coordinates on a unit
     sphere.
 
     Parameters
     ----------
     table : astropy.table.Table
         Catalog containing objects. The catalog needs to have coordinates and
-        field IDs.
+        field IDs. The jackknife field for each galaxy will be added in the
+        `field_jk` column.
     centers : int or numpy.ndarray
         If int, total number of jackknife fields. Otherwise, the centers
         returned from a previous call to that function. This allows for
         different samples to have the same jackknife fields.
     distance_threshold : float, optional
         The angular separation in degrees used to link points and calculate
         continous fields before running KMeans. Default is 1.
```

### Comparing `dsigma-0.7.2/dsigma/physics.py` & `dsigma-1.0.0/dsigma/physics.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,16 +196,17 @@
                                   k_max=1e3):
     r"""Compute the lens magnification bias to the mean tangential shear.
 
     This function is based on equations (13) and (14) in Unruh et al. (2020).
 
     Parameters
     ----------
-    theta : float
-        Angular separation :math:`\theta` from the lens sample in radians.
+    theta : float or astropy.units.quantity.Quantity
+        Angular separation :math:`\theta` from the lens sample. If not quantity
+        is given, the separation is assumed to be in radians.
     alpha_l : float
         Local slope of the flux distribution of lenses near the flux limit.
     z_l : float
         Redshift of lens.
     z_s : float
         Redshift of source.
     camb_results : camb.results.CAMBdata
@@ -234,14 +235,19 @@
     et_lm : float
         Bias in the mean tangential shear due to lens magnification effects.
 
     """
     camb_interp = camb_results.get_matter_power_interpolator(
         hubble_units=False, k_hunit=False)
 
+    if not isinstance(theta, u.quantity.Quantity):
+        theta = theta * u.rad
+
+    theta = theta.to(u.rad).value
+
     ell_min = 0
     ell_max = np.amax(jn_zeros(2, bessel_function_zeros)) / theta
     z_min = 0
     z_max = min(z_l, z_s)
 
     z, w_z = np.polynomial.legendre.leggauss(n_z)
     z = (z_max - z_min) / 2.0 * z + (z_max + z_min) / 2.0
@@ -279,8 +285,8 @@
 
     gamma = np.sum(int_z * int_ell * int_z_ell * w_z * w_ell)
     gamma = ((gamma * u.Mpc**3) * 9 * camb_results.Params.H0**3 * u.km**3 /
              u.s**3 / u.Mpc**3 *
              (camb_results.Params.omch2 + camb_results.Params.ombh2)**2 /
              (camb_results.Params.H0 / 100)**4 / 4 / c.c**3)
 
-    return 2 * (alpha_l - 1) * gamma
+    return 2 * (alpha_l - 1) * gamma.to(u.dimensionless_unscaled).value
```

### Comparing `dsigma-0.7.2/dsigma/precompute.py` & `dsigma-1.0.0/dsigma/precompute.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,22 +188,27 @@
 
     Parameters
     ----------
     table_l : astropy.table.Table
         Catalog of lenses.
     table_s : astropy.table.Table
         Catalog of sources.
-    bins : numpy.ndarray or u.quantity.Quantity
+    bins : numpy.ndarray or astropy.units.quantity.Quantity
         Bins in radius to use for the stacking. If a numpy array, bins are
         assumed to be in Mpc. If an astropy quantity, one can pass both length
         units, e.g. kpc and Mpc, as well as angular units, i.e. deg and rad.
     table_c : astropy.table.Table, optional
-        Additional photometric redshift calibration catalog. Default is None.
+        Additional photometric redshift calibration catalog. If provided, this
+        will be used to statistically correct the photometric source redshifts
+        and critical surface densities. Default is None.
     table_n : astropy.table.Table, optional
-        Source redshift distributions. Default is None.
+        Source redshift distributions. If provided, this will be used to
+        compute mean source redshifts and critical surface densities. These
+        mean quantities would be used instead the individual photometric
+        redshift estimates. Default is None.
     cosmology : astropy.cosmology, optional
         Cosmology to assume for calculations. Default is a flat LambdaCDM
         cosmology with h=1 and Om0=0.3.
     comoving : boolean, optional
         Whether to use comoving or physical quantities for radial bins (if
         given in physical units) and the excess surface density. Default is
         True.
@@ -384,15 +389,15 @@
         raise ValueError('table_c and table_n cannot both be given.')
 
     # Create arrays that will hold the final results.
     table_engine_r = {}
     n_results = len(table_l) * (len(bins) - 1)
 
     key_list = ['sum 1', 'sum w_ls', 'sum w_ls e_t', 'sum w_ls z_s',
-                'sum w_ls e_t sigma_crit']
+                'sum w_ls e_t sigma_crit', 'sum w_ls sigma_crit']
 
     if 'm' in table_s.colnames:
         key_list.append('sum w_ls m')
 
     if 'e_rms' in table_s.colnames:
         key_list.append('sum w_ls (1 - e_rms^2)')
 
@@ -465,20 +470,23 @@
     for key in table_engine_r.keys():
         table_l[key] = np.array(table_engine_r[key]).reshape(
             len(table_l), len(bins) - 1)[inv_argsort_pix_l]
 
     table_l['sum w_ls z_l'] = table_l['z'][:, np.newaxis] * table_l['sum w_ls']
 
     if 'f_bias' in table_engine_l.keys():
+        table_l['sum w_ls sigma_crit f_bias'] = (
+            np.array(table_engine_l['f_bias'])[inv_argsort_pix_l][
+                :, np.newaxis] * table_l['sum w_ls sigma_crit'])
         table_l['sum w_ls e_t sigma_crit f_bias'] = (
             np.array(table_engine_l['f_bias'])[inv_argsort_pix_l][
                 :, np.newaxis] * table_l['sum w_ls e_t sigma_crit'])
 
     if 'delta z_s' in table_engine_l.keys():
-        table_l['sum w_ls (z_s - delta z_s)'] = (
+        table_l['sum w_ls z_s'] = (
             table_l['sum w_ls z_s'] - table_l['sum w_ls'] * np.array(
                 table_engine_l['delta z_s'])[inv_argsort_pix_l][:, np.newaxis])
 
     table_l.meta['bins'] = bins
     table_l.meta['comoving'] = comoving
     table_l.meta['H0'] = cosmology.H0.value
     table_l.meta['Ok0'] = cosmology.Ok0
```

### Comparing `dsigma-0.7.2/dsigma/precompute_engine.pyx` & `dsigma-1.0.0/dsigma/precompute_engine.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
     cdef double[::1] dist_3d_sq_bins = dist_3d_sq_bins_in
 
     cdef long[::1] sum_1 = table_r['sum 1']
     cdef double[::1] sum_w_ls = table_r['sum w_ls']
     cdef double[::1] sum_w_ls_e_t = table_r['sum w_ls e_t']
     cdef double[::1] sum_w_ls_e_t_sigma_crit = table_r['sum w_ls e_t sigma_crit']
+    cdef double[::1] sum_w_ls_sigma_crit = table_r['sum w_ls sigma_crit']
     cdef double[::1] sum_w_ls_z_s = table_r['sum w_ls z_s']
     cdef double[::1] sum_w_ls_m
     if has_m:
         sum_w_ls_m = table_r['sum w_ls m']
     cdef double[::1] sum_w_ls_1_minus_e_rms_sq
     if has_e_rms:
         sum_w_ls_1_minus_e_rms_sq = table_r['sum w_ls (1 - e_rms^2)']
@@ -199,15 +200,15 @@
 
                     if w_s[i_s] == 0:
                         continue
 
                     if has_sigma_crit_eff:
                         sigma_crit = sigma_crit_eff[
                             i_l * n_z_bins + z_bin[i_s]]
-                    elif z_l[i_l] < z_s[i_s]:
+                    elif d_com_l[i_l] < d_com_s[i_s]:
                         sigma_crit = (sigma_crit_factor * (1 + z_l[i_l]) *
                             d_com_s[i_s] / d_com_l[i_l] /
                             (d_com_s[i_s] - d_com_l[i_l]))
                         if comoving:
                             sigma_crit /= (1.0 + z_l[i_l]) * (1.0 + z_l[i_l])
                     else:
                         if weighting < 0:
@@ -246,14 +247,15 @@
                     summand = w_ls
                     sum_w_ls[offset_result + i_bin] += summand
                     summand *= e_t
                     sum_w_ls_e_t[offset_result + i_bin] += summand
                     summand *= sigma_crit
                     sum_w_ls_e_t_sigma_crit[offset_result + i_bin] += summand
                     sum_w_ls_z_s[offset_result + i_bin] += w_ls * z_s[i_s]
+                    sum_w_ls_sigma_crit[offset_result + i_bin] += w_ls * sigma_crit
                     if has_m:
                         sum_w_ls_m[offset_result + i_bin] += w_ls * m[i_s]
                     if has_e_rms:
                         sum_w_ls_1_minus_e_rms_sq[offset_result + i_bin] += (
                             w_ls * (1 - e_rms[i_s] * e_rms[i_s]))
                     if has_R_2 and R_2[i_s] <= 0.31:
                         sum_w_ls_A_p_R_2[offset_result + i_bin] += (
```

### Comparing `dsigma-0.7.2/dsigma/stacking.py` & `dsigma-1.0.0/dsigma/stacking.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import numpy as np
 from astropy import units as u
 from astropy.table import Table
 from astropy.cosmology import FlatLambdaCDM
 from astropy.units import UnitConversionError
 from . import surveys
 from .physics import mpc_per_degree, lens_magnification_shear_bias
-from .physics import critical_surface_density
 
 __all__ = ['number_of_pairs', 'raw_tangential_shear',
            'raw_excess_surface_density', 'photo_z_dilution_factor',
            'boost_factor', 'scalar_shear_response_factor',
            'matrix_shear_response_factor', 'shear_responsivity_factor',
            'mean_lens_redshift', 'mean_source_redshift',
+           'mean_critical_surface_density', 'lens_magnification_bias',
            'tangential_shear', 'excess_surface_density']
 
 
 def number_of_pairs(table_l):
     """Compute the number of lens-source pairs per bin.
 
     Parameters
@@ -204,58 +204,78 @@
 
     """
     return (
         np.sum(table_l['sum w_ls z_l'] * table_l['w_sys'][:, None], axis=0) /
         np.sum(table_l['sum w_ls'] * table_l['w_sys'][:, None], axis=0))
 
 
-def mean_source_redshift(table_l, photo_z_correction=False):
+def mean_source_redshift(table_l):
     """Compute the weighted-average source redshift.
 
     Parameters
     ----------
     table_l : astropy.table.Table
         Precompute results for the lenses.
-    photo_z_correction : boolean, optional
-        By default, this function returns the average photometric source
-        redshift. If True and a calibration catalog or source redshift
-        distribution has been provided at the precompute stage, estimate the
-        intrinsic source redshift distribution. Default is False.
 
     Returns
     -------
     z_s : numpy.ndarray
         Mean source redshift in each bin.
 
     """
-    if not photo_z_correction:
-        key_num = 'sum w_ls z_s'
-    else:
-        key_num = 'sum w_ls (z_s - delta z_s)'
+    return (
+        np.sum(table_l['sum w_ls z_s'] * table_l['w_sys'][:, None], axis=0) /
+        np.sum(table_l['sum w_ls'] * table_l['w_sys'][:, None], axis=0))
+
+
+def mean_critical_surface_density(table_l, photo_z_dilution_correction=False):
+    """Compute the weighted-average (effective) critical surface density.
+
+    Parameters
+    ----------
+    table_l : astropy.table.Table
+        Precompute results for the lenses.
+    photo_z_dilution_correction : boolean, optional
+        If True, correct for photo-z biases. This can only be done if a
+        calibration catalog has been provided in the Precomputation phase.
+        Default is False.
+
+    Returns
+    -------
+    sigma_crit : numpy.ndarray
+        Mean (effective) critical surface density.
 
+    """
+    if photo_z_dilution_correction:
+        key = 'sum w_ls sigma_crit f_bias'
+    else:
+        key = 'sum w_ls sigma_crit'
     return (
-        np.sum(table_l[key_num] * table_l['w_sys'][:, None], axis=0) /
+        np.sum(table_l[key] * table_l['w_sys'][:, None], axis=0) /
         np.sum(table_l['sum w_ls'] * table_l['w_sys'][:, None], axis=0))
 
 
 def lens_magnification_bias(table_l, alpha_l, camb_results,
-                            photo_z_correction=True, shear=False):
+                            photo_z_dilution_correction=False, shear=False):
     """Estimate the additive lens magnification bias.
 
     Parameters
     ----------
     table_l : astropy.table.Table
         Precompute results for the lenses.
     alpha_l : float
         The response of the lenses to magnification.
     camb_results : camb.results.CAMBdata
         CAMB results object that contains information on cosmology and the
         matter power spectrum.
-    photo_z_correction : boolean, optional
-        Whether to correct for photo-z dilution and offsets. Default is True.
+    photo_z_dilution_correction : boolean, optional
+        If True, correct the mean critical surface density for photo-z biases.
+        Not used if `shear` is True. This should be consistent with what is
+        used for calculating the total excess surface density. Default is
+        False.
     shear : boolean, optional
         If True, return bias of the mean tangential shear. Otherwise, return
         an estimate for the bias of the excess surface density. Default is
         False.
 
     Returns
     -------
@@ -263,45 +283,32 @@
         The lens magnification bias in each radial bin.
 
     """
     cosmology = FlatLambdaCDM(H0=table_l.meta['H0'], Om0=table_l.meta['Om0'])
 
     z_l = mean_lens_redshift(table_l)
     z_s = mean_source_redshift(table_l)
-    if photo_z_correction:
-        z_s_true = mean_source_redshift(table_l, photo_z_correction=True)
-        try:
-            sigma_crit = critical_surface_density(
-                z_l, z_s, cosmology, comoving=table_l.meta['comoving'])
-            sigma_crit *= photo_z_dilution_factor(table_l)
-        except KeyError:
-            sigma_crit = critical_surface_density(
-                z_l, z_s_true, cosmology, comoving=table_l.meta['comoving'])
-    else:
-        sigma_crit = critical_surface_density(
-            z_l, z_s, cosmology, comoving=table_l.meta['comoving'])
-        z_s_true = z_s
-
     bins = table_l.meta['bins']
     d = 2.0 / 3.0 * np.diff(bins**3) / np.diff(bins**2)
 
     try:
         theta = d.to(u.rad).value
     except UnitConversionError:
         theta = np.deg2rad(d.to(u.Mpc).value / mpc_per_degree(
             z_l, cosmology=cosmology, comoving=table_l.meta['comoving']))
 
     gt = np.array([lens_magnification_shear_bias(
-        theta[i], alpha_l, z_l[i], z_s_true[i], camb_results) for i in
+        theta[i], alpha_l, z_l[i], z_s[i], camb_results) for i in
         range(len(theta))])
 
     if shear:
         return gt
     else:
-        return gt * sigma_crit
+        return gt * mean_critical_surface_density(
+            table_l, photo_z_dilution_correction=photo_z_dilution_correction)
 
 
 def tangential_shear(table_l, table_r=None, boost_correction=False,
                      scalar_shear_response_correction=False,
                      matrix_shear_response_correction=False,
                      shear_responsivity_correction=False,
                      hsc_selection_bias_correction=False,
@@ -420,15 +427,15 @@
     ----------
     table_l : astropy.table.Table
         Precompute results for the lenses.
     table_r : astropy.table.Table, optional
         Precompute results for random lenses. Default is None.
     photo_z_dilution_correction : boolean, optional
         If True, correct for photo-z biases. This can only be done if a
-        calibration catalog has been provided in the Precomputation phase.
+        calibration catalog has been provided in the precomputation phase.
         Default is False.
     boost_correction : boolean, optional
         If true, calculate and apply a boost factor correction. This can only
         be done if a random catalog is provided. Default is False.
     scalar_shear_response_correction : boolean or string, optional
         Whether to correct for the multiplicative shear bias (scalar form).
         Default is False.
```

### Comparing `dsigma-0.7.2/dsigma/surveys/cfhtls.py` & `dsigma-1.0.0/dsigma/surveys/cfhtls.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.2/dsigma/surveys/des.py` & `dsigma-1.0.0/dsigma/surveys/des.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.2/dsigma/surveys/hsc.py` & `dsigma-1.0.0/dsigma/surveys/hsc.py`

 * *Files identical despite different names*

### Comparing `dsigma-0.7.2/dsigma/surveys/kids.py` & `dsigma-1.0.0/dsigma/surveys/kids.py`

 * *Files identical despite different names*

