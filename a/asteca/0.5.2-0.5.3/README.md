# Comparing `tmp/asteca-0.5.2.tar.gz` & `tmp/asteca-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asteca-0.5.2.tar", max compression
+gzip compressed data, was "asteca-0.5.3.tar", max compression
```

## Comparing `asteca-0.5.2.tar` & `asteca-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0     1071 2024-04-18 20:24:11.112496 asteca-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     1140 2024-04-18 20:24:11.112496 asteca-0.5.2/README.md
--rw-r--r--   0        0        0     1093 2024-05-05 14:37:26.025497 asteca-0.5.2/asteca/__init__.py
--rw-r--r--   0        0        0     5978 2024-05-06 15:23:31.088325 asteca-0.5.2/asteca/cluster.py
--rw-r--r--   0        0        0     6814 2024-05-06 20:00:05.721149 asteca-0.5.2/asteca/isochrones.py
--rw-r--r--   0        0        0     3088 2024-05-05 14:39:38.802627 asteca-0.5.2/asteca/likelihood.py
--rw-r--r--   0        0        0        0 2024-04-18 20:24:11.116496 asteca-0.5.2/asteca/modules/__init__.py
--rw-r--r--   0        0        0     3727 2024-05-05 14:39:38.878630 asteca-0.5.2/asteca/modules/imfs.py
--rw-r--r--   0        0        0    12359 2024-05-06 12:12:01.145323 asteca-0.5.2/asteca/modules/isochrones_priv.py
--rw-r--r--   0        0        0    10054 2024-05-05 14:39:39.214643 asteca-0.5.2/asteca/modules/likelihood_priv.py
--rw-r--r--   0        0        0     7833 2024-05-05 14:39:39.054636 asteca-0.5.2/asteca/modules/mass_binary.py
--rw-r--r--   0        0        0    35104 2024-05-06 20:09:09.279994 asteca-0.5.2/asteca/modules/synth_cluster_priv.py
--rw-r--r--   0        0        0    19706 2024-05-06 20:21:49.518241 asteca-0.5.2/asteca/synthetic.py
--rw-r--r--   0        0        0      617 2024-05-07 19:21:12.421026 asteca-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 asteca-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-18 20:24:11.112496 asteca-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0     1140 2024-04-18 20:24:11.112496 asteca-0.5.3/README.md
+-rw-r--r--   0        0        0     1132 2024-05-26 14:15:22.989696 asteca-0.5.3/asteca/__init__.py
+-rw-r--r--   0        0        0    10533 2024-05-26 14:16:14.807546 asteca-0.5.3/asteca/cluster.py
+-rw-r--r--   0        0        0     7167 2024-05-16 18:42:51.627432 asteca-0.5.3/asteca/isochrones.py
+-rw-r--r--   0        0        0     3087 2024-05-17 19:17:16.890054 asteca-0.5.3/asteca/likelihood.py
+-rw-r--r--   0        0        0     4545 2024-05-26 14:16:14.807546 asteca-0.5.3/asteca/membership.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:24:11.116496 asteca-0.5.3/asteca/modules/__init__.py
+-rw-r--r--   0        0        0     9103 2024-05-26 14:16:14.811546 asteca-0.5.3/asteca/modules/bayesian_da.py
+-rw-r--r--   0        0        0     6635 2024-05-26 14:16:14.811546 asteca-0.5.3/asteca/modules/cluster_priv.py
+-rw-r--r--   0        0        0    23189 2024-05-26 14:16:14.811546 asteca-0.5.3/asteca/modules/fastmp.py
+-rw-r--r--   0        0        0     3727 2024-05-07 19:32:15.248574 asteca-0.5.3/asteca/modules/imfs.py
+-rw-r--r--   0        0        0    12356 2024-05-26 14:16:14.811546 asteca-0.5.3/asteca/modules/isochrones_priv.py
+-rw-r--r--   0        0        0    10054 2024-05-07 19:32:15.252575 asteca-0.5.3/asteca/modules/likelihood_priv.py
+-rw-r--r--   0        0        0     7833 2024-05-07 19:32:15.252575 asteca-0.5.3/asteca/modules/mass_binary.py
+-rw-r--r--   0        0        0    35161 2024-05-17 19:17:17.542076 asteca-0.5.3/asteca/modules/synth_cluster_priv.py
+-rw-r--r--   0        0        0    19908 2024-05-25 13:34:36.464385 asteca-0.5.3/asteca/synthetic.py
+-rw-r--r--   0        0        0      617 2024-05-26 14:20:54.629643 asteca-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 asteca-0.5.3/PKG-INFO
```

### Comparing `asteca-0.5.2/LICENSE.txt` & `asteca-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asteca-0.5.2/README.md` & `asteca-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `asteca-0.5.2/asteca/__init__.py` & `asteca-0.5.3/asteca/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from .cluster import cluster as cluster
+from . import membership as membership
 from .isochrones import isochrones as isochrones
 from .synthetic import synthetic as synthetic
-from .cluster import cluster as cluster
 from .likelihood import likelihood as likelihood
 
 from contextlib import suppress
 import importlib.metadata
 from pathlib import Path
```

### Comparing `asteca-0.5.2/asteca/isochrones.py` & `asteca-0.5.3/asteca/isochrones.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,71 +3,75 @@
 from dataclasses import dataclass
 from typing import Optional
 from .modules import isochrones_priv
 
 
 @dataclass
 class isochrones:
-    r"""Define an ``isochrones`` object.
+    """Define an :class:`isochrones` object.
 
     This object contains the loaded theoretical isochrones used by the
-    :py:mod:`asteca.synthetic` class to generate synthetic clusters.
+    :py:class:`asteca.synthetic` class to generate synthetic clusters.
     See :ref:`isochronesload` for more details.
 
-    Parameters
-    ----------
-    model : str, {"PARSEC", "MIST", "BASTI"}
-        The model must be one of the supported isochrone services:
-        `PARSEC <http://stev.oapd.inaf.it/cgi-bin/cmd_3.7>`_,
-        `MIST <https://waps.cfa.harvard.edu/MIST/>`_, or
-        `BASTI <http://basti-iac.oa-abruzzo.inaf.it/isocs.html>`_.
-    isochs_path : str
-        Path to the folder that contains the files for the theoretical isochrones.
-    magnitude : str
-        Magnitude's filter name as defined in the theoretical isochrones.
-        Example for Gaia's ``G`` magnitude: ``"Gmag"``.
-    color : tuple
-        Tuple containing the filter names that generate the first color defined.
-        The correct format is: ``("filter1", "filter2")``, where ``filter1``
+    :param model: The model must be one of the supported isochrone services:
+        `PARSEC <http://stev.oapd.inaf.it/cgi-bin/cmd_3.7>`__,
+        `MIST <https://waps.cfa.harvard.edu/MIST/>`__, or
+        `BASTI <http://basti-iac.oa-abruzzo.inaf.it/isocs.html>`__.
+    :type model: str: ``PARSEC, MIST, BASTI``
+    :param isochs_path: Path to the folder that contains the files for the theoretical
+        isochrones
+    :type isochs_path: str
+    :param magnitude: Magnitude's filter name as defined in the theoretical isochrones.
+        Example for Gaia's ``G`` magnitude: ``"Gmag"``
+    :type magnitude: str
+    :param color: Tuple containing the filter names that generate the first color
+        defined. The correct format is: ``("filter1", "filter2")``, where ``filter1``
         and ``filter2`` are the names of the filters that are combined to generate
         the color. The order is important because the color will be generated as:
         ``filter1-filter2``. Example for Gaia's 'BP-RP' color:
-        ``("G_BPmag", "G_RPmag")``.
-    color2 : tuple, optional, default=None
-        Optional second color to use in the analysis. Same format as that used by the
-        ``color`` parameter.
-    magnitude_effl : float, optional, default=None
-        Effective lambda (in Angstrom) for the magnitude filter.
-    color_effl : tuple, optional, default=None
-        Effective lambdas for the filters that make up the ``color`` defined in the
-        :py:mod:`asteca.isochrones` object. E.g.: ``(1111.11, 2222.22)`` where
-        ``1111.11`` and ``2222.22`` are the effective lambdas (in Angstrom) for each
-        filter, in the same order as ``color``.
-    color2_effl : tuple, optional, default=None
-        Same as ``color_effl`` but for a second (optional) color defined.
-    z_to_FeH : float, optional, default=None
-        If ``None``, the default ``z`` values in the isochrones will be used to
-        generate the synthetic clusters. If ``float``, it must represent the solar
-        metallicity for these isochrones. The metallicity values will then be converted
-        to ``[FeH]`` values, to be used by the :meth:`synthetic.generate()` method.
-    N_interp : int, default=2500
-        Number of interpolation points used to ensure that all isochrones are the
-        same shape.
-    column_names : dict, optional, default=None
-        Column names for the initial mass, metallicity, and age for the photometric
-        system's isochrones files. Example:
+        ``("G_BPmag", "G_RPmag")``
+    :type color: tuple
+    :param color2: Optional second color to use in the analysis. Same format as that
+        used by the ``color`` parameter, defaults to ``None``
+    :type color2: tuple, optional
+    :param magnitude_effl: Effective lambda (in Angstrom) for the magnitude filter,
+        defaults to ``None``
+    :type magnitude_effl: float, optional
+    :param color_effl: Effective lambdas for the filters that make up the ``color``
+        defined in the :py:class:`asteca.isochrones` object. E.g.:
+        ``(1111.11, 2222.22)`` where ``1111.11`` and ``2222.22`` are the effective
+        lambdas (in Angstrom) for each filter, in the same order as ``color``, defaults
+        to ``None``
+    :type color_effl: tuple, optional
+    :param color2_effl: Same as ``color_effl`` but for a second (optional) color
+        defined, defaults to ``None``
+    :type color2_effl: tuple, optional
+    :param z_to_FeH: If ``None``, the default ``z`` values in the isochrones will be
+        used to generate the synthetic clusters. If ``float``, it must represent the
+        solar metallicity for these isochrones. The metallicity values will then be
+        converted to ``[FeH]`` values, to be used by the
+        :py:meth:`synthetic.generate() <asteca.synthetic.synthetic.generate>` method,
+        defaults to ``None``
+    :type z_to_FeH: float, optional
+    :param N_interp: Number of interpolation points used to ensure that all isochrones
+        are the same shape, defaults to ``2500``
+    :type N_interp: int
+    :param column_names: Column names for the initial mass, metallicity, and age for
+        the photometric system's isochrones files. Example:
         ``{"mass_col": "Mini", "met_col": "Zini", "age_col": "logAge"}``.
         This dictionary is defined internally in `ASteCA` and should only be given
         by the user if the isochrone service changes its format and the `isochrones`
-        class fails to load the files.
-    parsec_rm_stage_9 : boll, optional, default=True
-        If the isochrones are PARSEC, this argument set to ``True`` will remove the
-        *post_AGB* stage (label=9) which are still
-        "`in preparation <http://stev.oapd.inaf.it/cmd_3.7/faq.html>`_".
-
+        class fails to load the files, defaults to ``None``
+    :type column_names: dict, optional
+    :param parsec_rm_stage_9: If the isochrones are PARSEC, this argument set to
+        ``True`` will remove the *post_AGB* stage (label=9) which are still
+        "`in preparation <http://stev.oapd.inaf.it/cmd_3.7/faq.html>`__", defaults
+        to ``True``
+    :type parsec_rm_stage_9: bool, optional
     """
 
     model: str
     isochs_path: str
     magnitude: str
     color: tuple
     color2: Optional[tuple] = None
@@ -126,36 +130,34 @@
         print(f"Magnitude      : {self.magnitude}")
         print(f"Color          : {self.color[0]}-{self.color[1]}")
         if self.color2 is not None:
             print(f"Color2         : {self.color2[0]}-{self.color2[1]}")
         print("Isochrone object generated\n")
 
     def _func_z_to_FeH(self, z_to_FeH):
-        r"""Convert z to FeH"""
+        """Convert z to FeH"""
         feh = np.log10(self.met_age_dict["met"] / z_to_FeH)
         N_old = len(feh)
         round_n = 4
         while True:
             feh_r = np.round(feh, round_n)
             N_new = len(set(feh_r))
             # If no duplicated values exist after rounding
             if N_old == N_new:
                 break
             round_n += 1
         # Replace old values
         self.met_age_dict["met"] = feh_r
 
     def _min_max(self) -> tuple[float]:
-        r"""Return the minimum and maximum values for the metallicity and age defined
+        """Return the minimum and maximum values for the metallicity and age defined
         in the theoretical isochrones.
 
-        Returns
-        -------
-        tuple[float]
-            Tuple of (minimum_metallicity, maximum_metallicity, minimum_age, maximum_age)
-
+        :return: Tuple of (minimum_metallicity, maximum_metallicity, minimum_age,
+            maximum_age)
+        :rtype: tuple[float]
         """
         zmin = self.met_age_dict["met"].min()
         zmax = self.met_age_dict["met"].max()
         amin = self.met_age_dict["loga"].min()
         amax = self.met_age_dict["loga"].max()
         return zmin, zmax, amin, amax
```

### Comparing `asteca-0.5.2/asteca/likelihood.py` & `asteca-0.5.3/asteca/likelihood.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 import numpy as np
 from .cluster import cluster
 from .modules import likelihood_priv as lpriv
 
 
 @dataclass
 class likelihood:
-    r"""Define a ``likelihood`` object.
+    """Define a :class:`likelihood` object.
 
     This object is used to assess how similar your observed cluster is, stored in
     a :py:class:`cluster` object,  compared to a given synthetic cluster, generated by
     the :py:meth:`synthetic.generate()` method.
 
-    Parameters
-    ----------
-    my_cluster : :class:`cluster`
-         :py:mod:`asteca.cluster` object with the loaded data for the observed cluster.
-    lkl_name : str, {"plr"}, default="plr"
-        Currently only the Poisson likelihood ratio defined in
-        `Tremmel et al. (2013) <https://ui.adsabs.harvard.edu/abs/2013ApJ...766...19T/abstract)>`_
-        is accepted.
-    bin_method: str, {"knuth", "fixed", "bayes_blocks", "manual"}, default="knuth"
-        Bin method used to split the color-magnitude diagram into cells
-        (`Hess diagram <https://en.wikipedia.org/wiki/Hess_diagram>`_). If ``manual``
+    :param my_cluster: :py:class:`asteca.cluster` object with the loaded data for the
+        observed cluster
+    :type my_cluster: :class:`cluster`
+    :param lkl_name: Currently only the Poisson likelihood ratio defined in
+        `Tremmel et al. (2013) <https://ui.adsabs.harvard.edu/abs/2013ApJ...766...19T/abstract)>`__
+        is accepted, defaults to ``plr``
+    :type lkl_name: str
+    :param bin_method: Bin method used to split the color-magnitude diagram into cells
+        (`Hess diagram <https://en.wikipedia.org/wiki/Hess_diagram>`__). If ``manual``
         is selected, a list containing an array of edge values for the magnitude,
         followed by one or two arrays (depending on the number of colors defined) for
-        the color(s), also with edge values.
-
+        the color(s), also with edge values,  defaults to ``knuth``
+    :type bin_method: str: ``knuth, fixed, bayes_blocks, manual``
     """
 
     my_cluster: cluster
     lkl_name: str = "plr"
     bin_method: str = "knuth"
 
     def __post_init__(self):
@@ -54,29 +52,25 @@
         self.max_lkl = self.get(
             np.array([self.my_cluster.mag_p, *self.my_cluster.colors_p])
         )
 
         print("Likelihood object generated\n")
 
     def get(self, synth_clust):
-        r"""Evaluate the selected likelihood function.
+        """Evaluate the selected likelihood function.
+
 
-        Parameters
-        ----------
-        synth_clust : array
-            ``np.array`` containing the synthetic cluster. The shape of this array must
-            be: ``[magnitude, color1, (color2)]``, where ``magnitude`` and ``color``
-            are arrays with the magnitude and color photometric data (``color2`` is the
-            optional second color defined).
-
-        Returns
-        -------
-        float
-            Likelihood value.
+        :param synth_clust:  Numpy array containing the synthetic cluster. The shape of
+            this array must be: ``[magnitude, color1, (color2)]``, where ``magnitude``
+            and ``color`` are arrays with the magnitude and color photometric data
+            (``color2`` is the optional second color defined)
+        :type synth_clust: array
 
+        :return: Likelihood value
+        :rtype: float
         """
         if self.lkl_name == "plr":
             return lpriv.tremmel(self, synth_clust)
         if self.lkl_name == "visual":
             return lpriv.visual(self, synth_clust)
         if self.lkl_name == "mean_dist":
             return lpriv.mean_dist(self, synth_clust)
```

### Comparing `asteca-0.5.2/asteca/modules/imfs.py` & `asteca-0.5.3/asteca/modules/imfs.py`

 * *Files identical despite different names*

### Comparing `asteca-0.5.2/asteca/modules/isochrones_priv.py` & `asteca-0.5.3/asteca/modules/isochrones_priv.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 ) -> tuple[list, list]:
     """ """
 
     group_col = {"PARSEC": met_col, "MIST": age_col, "BASTI": None}
 
     isochrones = {}
     for file_path in f_paths:
-
         # Extract columns names and full header
         col_names, full_header = get_header(file_path)
 
         # Columns to keep for this photometric system
         cols_keep_ps = list(set(col_names) & set(cols_keep))
 
         # Group file in blocks as required
@@ -132,15 +131,14 @@
 
         if model == "PARSEC":
             # Process metallicity blocks
             for _, met_df in df_blocks:
                 # Group by age
                 age_blocks = met_df.groupby(age_col, sort=False)
                 for _, df in age_blocks:
-
                     zinit = df[met_col].values[0]
                     try:
                         isochrones[zinit]
                     except KeyError:
                         isochrones[zinit] = {}
 
                     # Remove post-AGB stage
@@ -159,15 +157,14 @@
             try:
                 isochrones[zinit]
             except KeyError:
                 isochrones[zinit] = {}
 
             # Process age blocks
             for _, df in df_blocks:
-
                 age = df[age_col].values[0]
                 # Interpolated isochrone
                 isochrones = interp_df(
                     N_interp, cols_keep_ps, df, isochrones, zinit, age
                 )
 
         elif model == "BASTI":
```

### Comparing `asteca-0.5.2/asteca/modules/likelihood_priv.py` & `asteca-0.5.3/asteca/modules/likelihood_priv.py`

 * *Files identical despite different names*

### Comparing `asteca-0.5.2/asteca/modules/mass_binary.py` & `asteca-0.5.3/asteca/modules/mass_binary.py`

 * *Files identical despite different names*

### Comparing `asteca-0.5.2/asteca/modules/synth_cluster_priv.py` & `asteca-0.5.3/asteca/modules/synth_cluster_priv.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,19 +205,24 @@
         # Effective wavelength in Armstrong.
         eff_wave = self.isochs.magnitude_effl
         # Effective wavelength in inverse microns.
         ext_coefs[0] = ccmo_model(10000.0 / eff_wave)
 
         # For colors.
         eff_wave1, eff_wave2 = self.isochs.color_effl
-        ext_coefs[1] = [ccmo_model(10000.0 / eff_wave1), ccmo_model(10000.0 / eff_wave2)]
+        ext_coefs[1] = [
+            ccmo_model(10000.0 / eff_wave1),
+            ccmo_model(10000.0 / eff_wave2),
+        ]
 
     if self.isochs.color2_effl is not None:
         eff_wave1, eff_wave2 = self.isochs.color2_effl
-        ext_coefs += [[ccmo_model(10000.0 / eff_wave1), ccmo_model(10000.0 / eff_wave2)]]
+        ext_coefs += [
+            [ccmo_model(10000.0 / eff_wave1), ccmo_model(10000.0 / eff_wave2)]
+        ]
 
     return ext_coefs
 
 
 def ccmo_model(mw: float) -> list:
     """Cardelli, Clayton, and Mathis (1989 ApJ. 345, 245) model for extinction
     coefficients with updated coefficients for near-UV from O'Donnell
```

### Comparing `asteca-0.5.2/asteca/synthetic.py` & `asteca-0.5.3/asteca/synthetic.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,44 +7,47 @@
 from .isochrones import isochrones
 from .modules import synth_cluster_priv as scp
 from .modules import mass_binary as mb
 
 
 @dataclass
 class synthetic:
-    r"""Define a ``synthetic`` object.
+    """Define a :class:`synthetic` object.
 
-    Use the isochrones loaded in the :py:mod:`asteca.isochrones` object to generate a
-    :py:mod:`asteca.synthetic` object. This object is used to generate synthetic clusters
-    given a :py:mod:`asteca.cluster` object  and a set of input fundamental parameters
-    (metallicity, age, distance, extinction, etc.).
+    Use the isochrones loaded in the :py:class:`asteca.isochrones` object to generate a
+    :py:class:`asteca.synthetic` object. This object is used to generate synthetic
+    clusters given a :py:class:`asteca.cluster` object and a set of input fundamental
+    parameters (metallicity, age, distance, extinction, etc.).
 
     See the :ref:`synth_clusters` section for more details.
 
-    Parameters
-    ----------
-    isochs : :class:`isochrones`
-         :py:mod:`asteca.isochrones` object with the loaded files for the theoretical isochrones.
-    ext_law : str, {"CCMO", "GAIADR3"}, default="CCMO"
-        Extinction law. If "*GAIADR3*" is selected, the magnitude and first color defined
-        in :class:`isochrones` and :class:`cluster` are assumed to be Gaia's
-        (E)DR3 **G** and **(BP-RP)** respectively. The second color (if defined) will
-        always be affected by the "*CCMO*" model.
-    DR_distribution : str, {"uniform", "normal"}, default="uniform"
-        Distribution function for the differential reddening.
-    IMF_name : str, {"salpeter_1955", "kroupa_2001", "chabrier_2014"}, default="chabrier_2014"
-        Name of the initial mass function used to populate the isochrones.
-    max_mass : int, default=100_000
-        Maximum total initial mass. Should be large enough to allow generating as many
-        synthetic stars as observed stars.
-    gamma : str, float, {"D&K", "fisher_stepped", "fisher_peaked", "raghavan"}, default="D&K"
-        Distribution function for the mass ratio of the binary systems.
-    seed: int, optional, default=None
-        Random seed. If ``None`` a random integer will be generated and used.
-
+    :param isochs: :py:class:`asteca.isochrones` object with the loaded files for the
+        theoretical isochrones
+    :type isochs: :class:`isochrones`
+    :param ext_law: Extinction law. if ``GAIADR3`` is selected, the magnitude and first
+        color defined in :py:class:`asteca.isochrones` and :py:class:`asteca.cluster`
+        are assumed to be Gaia's (E)DR3 **G** and **(BP-RP)** respectively. The second
+        color (if defined) will always be affected by the ``CCMO`` model, defaults to
+        ``CCMO``
+    :type ext_law: str: ``CCMO, GAIADR3``
+    :param DR_distribution: Distribution function for the differential reddening,
+        defaults to ``uniform``
+    :type DR_distribution: str: ``uniform, normal``
+    :param IMF_name: Name of the initial mass function used to populate the isochrones,
+        defaults to ``chabrier_2014``
+    :type IMF_name: str: ``salpeter_1955, kroupa_2001, chabrier_2014``
+    :param max_mass: Maximum total initial mass. Should be large enough to allow
+        generating as many synthetic stars as observed stars, defaults to ``100_000``
+    :type max_mass: int
+    :param gamma: Distribution function for the mass ratio of the binary systems,
+        defaults to ``D&K``
+    :type gamma: str: ``D&K, fisher_stepped, fisher_peaked, raghavan``, float
+    :param seed: Random seed. If ``None`` a random integer will be generated and used,
+        defaults to ``None``
+    :type seed: int, optional
     """
 
     isochs: isochrones
     ext_law: str = "CCMO"
     DR_distribution: str = "uniform"
     IMF_name: str = "chabrier_2014"
     max_mass: int = 100_000
@@ -122,33 +125,31 @@
         print(f"Gamma distribution     : {self.gamma}")
         print(f"Extinction law         : {self.ext_law}")
         print(f"Differential reddening : {self.DR_distribution}")
         print(f"Random seed            : {self.seed}")
         print("Synthetic clusters object generated\n")
 
     def calibrate(self, cluster, fix_params: dict = {}):
-        r"""Calibrate a :py:mod:`asteca.synthetic` object based on a
-        :py:mod:`asteca.cluster` object and a dictionary of fixed fundamental parameters
-        (``fix_params``).
+        """Calibrate a :py:class:`asteca.synthetic` object based on a
+        :py:class:`asteca.cluster` object and a dictionary of fixed fundamental
+        parameters (``fix_params``).
 
         Use the data obtained from your observed cluster stored in the
-        :py:mod:`asteca.cluster` object, to calibrate a :py:mod:`asteca.synthetic`
+        :py:class:`asteca.cluster` object, to calibrate a :py:class:`asteca.synthetic`
         object. Additionally, a dictionary of fixed fundamental parameters
         (metallicity, age, distance, extinction, etc.) can be passed.
 
         See the :ref:`synth_clusters` section for more details.
 
-        Parameters
-        ----------
-        cluster : :class:`cluster`
-             :py:mod:`asteca.cluster` object with the processed data from your observed
-             cluster.
-        fix_params : dict, optional, default={}
-            Dictionary with the values for the fixed parameters (if any).
-
+        :param cluster: :py:class:`asteca.cluster` object with the processed data from
+            your observed cluster
+        :type cluster: :py:class:`asteca.cluster`
+        :param fix_params: Dictionary with the values for the fixed parameters (if any),
+            defaults to ``{}``
+        :type fix_params: dict, optional
         """
         # Check that the number of colors match
         if self.isochs.color2_effl is not None and cluster.color2 is None:
             raise ValueError(
                 "Two colors were defined in 'synthetic' but a single color\n"
                 + "was defined in 'cluster'."
             )
@@ -188,35 +189,29 @@
                     )
 
         # # Remove low masses if required
         # if dm_min is not None:
         #     self._rm_low_masses(dm_min)
 
     def generate(self, fit_params: dict) -> np.ndarray:
-        r"""Generate a synthetic cluster.
+        """Generate a synthetic cluster.
 
         The synthetic cluster is generated according to the parameters given in
         the ``fit_params`` dictionary and the already calibrated
-        :py:mod:`asteca.synthetic` object.
+        :py:class:`asteca.synthetic` object.
 
-        Parameters
-        ----------
-        fit_params : dict
-            Dictionary with the values for the fundamental parameters that were **not**
-            included in the ``fix_params`` dictionary when the
-            :py:mod:`asteca.synthetic` object was calibrated
+        :param fit_params: Dictionary with the values for the fundamental parameters
+            that were **not** included in the ``fix_params`` dictionary when the
+            :py:class:`asteca.synthetic` object was calibrated
             (:meth:`synthetic.calibrate()` method).
-
-        Returns
-        -------
-        array[mag, c1, (c2)]
-            Return a ``np.array`` containing a synthetic cluster with the shape
+        :type fit_params: dict
+        :return: Return a ``np.array`` containing a synthetic cluster with the shape
             ``[mag, c1, (c2)]``, where ``mag`` is the magnitude dimension, and
             ``c1`` and ``c2`` (last one is optional) are the color dimension(s).
-
+        :rtype: array[mag, c1, (c2)]
         """
 
         # Return proper values for fixed parameters and parameters required
         # for the (z, log(age)) isochrone averaging.
         met, loga, alpha, beta, av, dr, rv, dm, ml, mh, al, ah = scp.properModel(
             self.met_age_dict, self.fix_params, fit_params
         )
@@ -279,39 +274,34 @@
         synth_clust = scp.add_errors(
             isoch_binar, self.err_dist, self.rand_floats["norm"][1]
         )
 
         return synth_clust[: self.m_ini_idx]
 
     def synthplot(self, ax, fit_params, color_idx=0, isochplot=False):
-        r"""Generate a color-magnitude plot for a synthetic cluster.
+        """Generate a color-magnitude plot for a synthetic cluster.
 
         The synthetic cluster is generated using the fundamental parameter values
         given in the ``fit_params`` dictionary.
 
-        Parameters
-        ----------
-        ax : matplotlib.axis, optional, default=None
-            Matplotlib axis where to draw the plot.
-        fit_params : dict
-            Dictionary with the values for the fundamental parameters that were **not**
-            included in the ``fix_params`` dictionary when the
-            :py:mod:`asteca.synthetic` object was calibrated
+        :param ax: Matplotlib axis where to draw the plot, defaults to ``None``
+        :type ax: matplotlib.axis, optional
+        :param fit_params: Dictionary with the values for the fundamental parameters
+            that were **not** included in the ``fix_params`` dictionary when the
+            :py:class:`asteca.synthetic` object was calibrated
             (:meth:`synthetic.calibrate()` method).
-        color_idx : int, default=0
-            Index of the color to plot. If ``0`` (default), plot the first color. If
-            ``1`` plot the second color.
-        isochplot : bool, default=False
-            If ``True``, the accompanying isochrone will be plotted.
-
-        Returns
-        -------
-        matplotlib.axis
-            Matplotlib axis object
-
+        :type fit_params: dict
+        :param color_idx: Index of the color to plot. If ``0`` (default), plot the
+            first color. If ``1`` plot the second color. Defaults to ``0``
+        :type color_idx: int
+        :param isochplot: If ``True``, the accompanying isochrone will be plotted,
+            defaults to ``False``
+        :type isochplot: bool
+        :return: Matplotlib axis object
+        :rtype: matplotlib.axis
         """
         if color_idx > 1:
             raise ValueError(
                 f"Wrong 'color_idx' value ({color_idx}), should be one of: [0, 1]"
             )
 
         # Generate synthetic cluster.
@@ -367,36 +357,30 @@
         msk = (isochrone[c_idx] >= xmin) & (isochrone[c_idx] <= xmax)
         isochrone = isochrone[:, msk]
         ax.plot(isochrone[c_idx], isochrone[0], c="k")
 
         return ax
 
     def masses_binary_probs(self, model, model_std):
-        r"""Estimate individual masses for the observed stars, along with their binary
+        """Estimate individual masses for the observed stars, along with their binary
         probabilities (if binarity was estimated).
 
-        Parameters
-        ----------
-        model : dict
-            Dictionary with the values for the fundamental parameters that were **not**
-            included in the ``fix_params`` dictionary when the
-            :py:mod:`asteca.synthetic` object was calibrated
-            (:meth:`synthetic.calibrate()` method).
-        model_std : dict
-            Dictionary with the standard deviations for the fundamental parameters in
-            the ``model`` argument.
-
-        Returns
-        -------
-        pandas.DataFrame
-            Data frame containing per-star primary and secondary masses along with
-            their uncertainties, and their probability of being a binary system.
-        numpy.array
-            Distribution of total binary fraction values for the cluster.
-
+        :param model: Dictionary with the values for the fundamental parameters that
+            were **not** included in the ``fix_params`` dictionary when the
+            :py:class:`asteca.synthetic` object was calibrated
+            (:py:meth:`synthetic.calibrate()` method)
+        :type model: dict
+        :param model_std: Dictionary with the standard deviations for the fundamental
+            parameters in the ``model`` argument
+        :type model_std: dict
+        :return: Data frame containing per-star primary and secondary masses along with
+            their uncertainties, and their probability of being a binary system
+        :rtype: pandas.DataFrame
+        :return: Distribution of total binary fraction values for the cluster
+        :rtype: numpy.array
         """
         # Generate random models from the selected solution
         models = mb.ranModels(model, model_std, self.seed)
 
         # Observed photometry
         obs_phot = np.array([self.mag_p] + [_ for _ in self.colors_p])
         # Replace nans in mag and colors to avoid crashing KDTree()
@@ -454,17 +438,15 @@
                 + "These will be assigned 'nan' values\nfor masses and "
                 + "binarity probability"
             )
 
         return df, np.array(b_fr_all)
 
     def _get_masses(self, fit_params, model_std, ra_c, dec_c):
-        """
-        Estimate the different total masses for the observed cluster
-        """
+        """Estimate the different total masses for the observed cluster"""
         print("Estimating total initial and actual masses")
         # Generate random models from the selected solution
         models = mb.ranModels(fit_params, model_std, self.seed)
 
         masses_all = []
         for i, model in enumerate(models):
             isoch = scp.generate(self, model)
```

### Comparing `asteca-0.5.2/pyproject.toml` & `asteca-0.5.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asteca"
-version = "0.5.2"
+version = "0.5.3"
 description = "Stellar cluster analysis package"
 authors = ["Gabriel I Perren <gabrielperren@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["cluster", "astrophysics"]
 homepage = "https://asteca.github.io/"
 repository = "https://github.com/asteca/ASteCA"
```

### Comparing `asteca-0.5.2/PKG-INFO` & `asteca-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asteca
-Version: 0.5.2
+Version: 0.5.3
 Summary: Stellar cluster analysis package
 Home-page: https://asteca.github.io/
 License: MIT
 Keywords: cluster,astrophysics
 Author: Gabriel I Perren
 Author-email: gabrielperren@gmail.com
 Requires-Python: >=3.10,<4.0
```

