# Comparing `tmp/pysersic-0.1.4.tar.gz` & `tmp/pysersic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysersic-0.1.4.tar", last modified: Thu Apr 18 19:37:58 2024, max compression
+gzip compressed data, was "pysersic-0.1.5.tar", last modified: Sun May 26 18:05:26 2024, max compression
```

## Comparing `pysersic-0.1.4.tar` & `pysersic-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.071461 pysersic-0.1.4/
--rw-r--r--   0 ipasha     (501) staff       (20)     1065 2023-01-18 18:39:41.000000 pysersic-0.1.4/LICENSE
--rw-r--r--   0 ipasha     (501) staff       (20)     1810 2024-04-18 19:37:58.071277 pysersic-0.1.4/PKG-INFO
--rw-r--r--   0 ipasha     (501) staff       (20)     5310 2024-01-30 18:45:38.000000 pysersic-0.1.4/README.md
--rw-r--r--   0 ipasha     (501) staff       (20)      709 2024-04-18 18:01:53.000000 pysersic-0.1.4/pyproject.toml
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.069141 pysersic-0.1.4/pysersic/
--rw-r--r--   0 ipasha     (501) staff       (20)      289 2024-04-18 18:01:51.000000 pysersic-0.1.4/pysersic/__init__.py
--rw-r--r--   0 ipasha     (501) staff       (20)      204 2023-08-10 18:12:29.000000 pysersic-0.1.4/pysersic/exceptions.py
--rw-r--r--   0 ipasha     (501) staff       (20)     6804 2023-06-06 01:01:14.000000 pysersic-0.1.4/pysersic/galfit.py
--rw-r--r--   0 ipasha     (501) staff       (20)    11326 2024-01-30 18:45:38.000000 pysersic-0.1.4/pysersic/loss.py
--rw-r--r--   0 ipasha     (501) staff       (20)    21344 2024-01-30 18:45:38.000000 pysersic-0.1.4/pysersic/multiband.py
--rw-r--r--   0 ipasha     (501) staff       (20)    36198 2024-04-18 19:37:28.000000 pysersic-0.1.4/pysersic/priors.py
--rw-r--r--   0 ipasha     (501) staff       (20)    27213 2024-04-18 19:37:28.000000 pysersic-0.1.4/pysersic/pysersic.py
--rw-r--r--   0 ipasha     (501) staff       (20)    33668 2024-04-18 19:37:28.000000 pysersic-0.1.4/pysersic/rendering.py
--rw-r--r--   0 ipasha     (501) staff       (20)    19587 2024-04-18 18:01:53.000000 pysersic-0.1.4/pysersic/results.py
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.069982 pysersic-0.1.4/pysersic.egg-info/
--rw-r--r--   0 ipasha     (501) staff       (20)     1810 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/PKG-INFO
--rw-r--r--   0 ipasha     (501) staff       (20)      494 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/SOURCES.txt
--rw-r--r--   0 ipasha     (501) staff       (20)        1 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/dependency_links.txt
--rw-r--r--   0 ipasha     (501) staff       (20)      112 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/requires.txt
--rw-r--r--   0 ipasha     (501) staff       (20)        9 2024-04-18 19:37:58.000000 pysersic-0.1.4/pysersic.egg-info/top_level.txt
--rw-r--r--   0 ipasha     (501) staff       (20)       38 2024-04-18 19:37:58.071499 pysersic-0.1.4/setup.cfg
--rw-r--r--   0 ipasha     (501) staff       (20)       38 2024-01-30 18:45:38.000000 pysersic-0.1.4/setup.py
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-04-18 19:37:58.070923 pysersic-0.1.4/tests/
--rw-r--r--   0 ipasha     (501) staff       (20)     7002 2024-04-18 18:01:53.000000 pysersic-0.1.4/tests/test_fitters.py
--rw-r--r--   0 ipasha     (501) staff       (20)      676 2023-06-06 01:01:14.000000 pysersic-0.1.4/tests/test_loss.py
--rw-r--r--   0 ipasha     (501) staff       (20)     2588 2024-04-18 18:01:53.000000 pysersic-0.1.4/tests/test_multiband.py
--rw-r--r--   0 ipasha     (501) staff       (20)     4090 2024-01-30 18:45:38.000000 pysersic-0.1.4/tests/test_priors.py
--rw-r--r--   0 ipasha     (501) staff       (20)     3524 2024-01-30 18:45:38.000000 pysersic-0.1.4/tests/test_renderers.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-05-26 18:05:26.265910 pysersic-0.1.5/
+-rw-r--r--   0 ipasha     (501) staff       (20)     1065 2023-01-18 18:39:41.000000 pysersic-0.1.5/LICENSE
+-rw-r--r--   0 ipasha     (501) staff       (20)     1810 2024-05-26 18:05:26.265708 pysersic-0.1.5/PKG-INFO
+-rw-r--r--   0 ipasha     (501) staff       (20)     5310 2024-01-30 18:45:38.000000 pysersic-0.1.5/README.md
+-rw-r--r--   0 ipasha     (501) staff       (20)      709 2024-05-26 17:40:27.000000 pysersic-0.1.5/pyproject.toml
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-05-26 18:05:26.263231 pysersic-0.1.5/pysersic/
+-rw-r--r--   0 ipasha     (501) staff       (20)      289 2024-04-18 18:01:51.000000 pysersic-0.1.5/pysersic/__init__.py
+-rw-r--r--   0 ipasha     (501) staff       (20)      204 2023-08-10 18:12:29.000000 pysersic-0.1.5/pysersic/exceptions.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     6804 2023-06-06 01:01:14.000000 pysersic-0.1.5/pysersic/galfit.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    11326 2024-01-30 18:45:38.000000 pysersic-0.1.5/pysersic/loss.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    21344 2024-01-30 18:45:38.000000 pysersic-0.1.5/pysersic/multiband.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    36658 2024-04-29 20:24:47.000000 pysersic-0.1.5/pysersic/priors.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    27239 2024-05-26 17:40:53.000000 pysersic-0.1.5/pysersic/pysersic.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    34755 2024-04-29 20:24:47.000000 pysersic-0.1.5/pysersic/rendering.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    19587 2024-04-18 18:01:53.000000 pysersic-0.1.5/pysersic/results.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-05-26 18:05:26.265486 pysersic-0.1.5/pysersic.egg-info/
+-rw-r--r--   0 ipasha     (501) staff       (20)     1810 2024-05-26 18:05:26.000000 pysersic-0.1.5/pysersic.egg-info/PKG-INFO
+-rw-r--r--   0 ipasha     (501) staff       (20)      494 2024-05-26 18:05:26.000000 pysersic-0.1.5/pysersic.egg-info/SOURCES.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)        1 2024-05-26 18:05:26.000000 pysersic-0.1.5/pysersic.egg-info/dependency_links.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)      112 2024-05-26 18:05:26.000000 pysersic-0.1.5/pysersic.egg-info/requires.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)        9 2024-05-26 18:05:26.000000 pysersic-0.1.5/pysersic.egg-info/top_level.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)       38 2024-05-26 18:05:26.265950 pysersic-0.1.5/setup.cfg
+-rw-r--r--   0 ipasha     (501) staff       (20)       38 2024-01-30 18:45:38.000000 pysersic-0.1.5/setup.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2024-05-26 18:05:26.265180 pysersic-0.1.5/tests/
+-rw-r--r--   0 ipasha     (501) staff       (20)     7002 2024-04-18 18:01:53.000000 pysersic-0.1.5/tests/test_fitters.py
+-rw-r--r--   0 ipasha     (501) staff       (20)      676 2023-06-06 01:01:14.000000 pysersic-0.1.5/tests/test_loss.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     2588 2024-04-18 18:01:53.000000 pysersic-0.1.5/tests/test_multiband.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     4090 2024-01-30 18:45:38.000000 pysersic-0.1.5/tests/test_priors.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     3524 2024-01-30 18:45:38.000000 pysersic-0.1.5/tests/test_renderers.py
```

### Comparing `pysersic-0.1.4/LICENSE` & `pysersic-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/PKG-INFO` & `pysersic-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysersic
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Tool for fitting sersic profiles in python
 Author-email: Imad Pasha <imad.pasha@yale.edu>, Tim Miller <timothy.miller@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2023 pysersic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysersic-0.1.4/README.md` & `pysersic-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/pyproject.toml` & `pysersic-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         'numpyro',
         'arviz',
         'tqdm',
         'asdf',
         'equinox>=0.11',
         'interpax',
         ]
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.setuptools]
 packages = ['pysersic']
```

### Comparing `pysersic-0.1.4/pysersic/galfit.py` & `pysersic-0.1.5/pysersic/galfit.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/pysersic/loss.py` & `pysersic-0.1.5/pysersic/loss.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/pysersic/multiband.py` & `pysersic-0.1.5/pysersic/multiband.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/pysersic/priors.py` & `pysersic-0.1.5/pysersic/priors.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     ymid = float(Y.shape[0] / 2.0)
     return back + (X - xmid) * x_sl + (Y - ymid) * y_sl
 
 
 base_profile_types = [
     "sersic",
     "doublesersic",
+    "sersic_exp",
     "sersic_pointsource",
     "pointsource",
     "exp",
     "dev",
 ]
 base_profile_params = dict(
     zip(
@@ -59,14 +60,26 @@
                 "n_1",
                 "ellip_1",
                 "r_eff_2",
                 "n_2",
                 "ellip_2",
                 "theta",
             ],
+            [
+                "xc",
+                "yc",
+                "flux",
+                "f_1",
+                "r_eff_1",
+                "n",
+                "ellip_1",
+                "r_eff_2",
+                "ellip_2",
+                "theta",
+            ],
             ["xc", "yc", "flux", "f_ps", "r_eff", "n", "ellip", "theta"],
             ["xc", "yc", "flux"],
             ["xc", "yc", "flux", "r_eff", "ellip", "theta"],
             ["xc", "yc", "flux", "r_eff", "ellip", "theta"],
         ],
     )
 )
@@ -977,15 +990,15 @@
             prior.set_uniform_prior("theta", 0.0, 2.0 * np.pi)
 
             if "sersic" in profile_type:
                 prior.set_uniform_prior("n", 0.65, 8)
                 if profile_type == "sersic_pointsource":
                     prior.set_uniform_prior("f_ps", 0.0, 1.0)
 
-        elif profile_type == "doublesersic":
+        elif profile_type in ["doublesersic", "sersic_exp"]:
             prior.set_uniform_prior("f_1", 0.0, 1.0)
 
             # prior.set_custom_prior('theta',
             #                       dist.VonMises(loc = self.theta_guess,concentration=2),
             #                       reparam= infer.reparam.CircularReparam() )
             prior.set_uniform_prior("theta", 0.0, 2.0 * np.pi)
 
@@ -999,17 +1012,19 @@
             r_eff_guess_err2 = jnp.sqrt(self.r_eff_guess * 1.5)
             prior.set_truncated_gaussian_prior(
                 "r_eff_2", r_loc2, r_eff_guess_err2, low=0.5
             )
 
             prior.set_uniform_prior("ellip_1", 0, 0.9)
             prior.set_uniform_prior("ellip_2", 0, 0.9)
-
-            prior.set_truncated_gaussian_prior("n_1", 4, 1, low=0.65, high=8)
-            prior.set_truncated_gaussian_prior("n_2", 1, 1, low=0.65, high=8)
+            if profile_type == "doublesersic":
+                prior.set_truncated_gaussian_prior("n_1", 4, 1, low=0.65, high=8)
+                prior.set_truncated_gaussian_prior("n_2", 1, 1, low=0.65, high=8)
+            else:
+                prior.set_truncated_gaussian_prior("n", 4, 1, low=0.65, high=8)
 
         return prior
 
     def visualize(
         self,
         figsize: Tuple[float, float] = (6.0, 6.0),
         cmap: str = "gray",
```

### Comparing `pysersic-0.1.4/pysersic/pysersic.py` & `pysersic-0.1.5/pysersic/pysersic.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,15 +664,15 @@
     return SVIRunResult(svi_class.get_params(best_state), svi_state, losses)
 
 
 def parse_mask(mask: ArrayLike = None, data: ArrayLike = None):
     if mask is None:
         return jnp.ones_like(data).astype(jnp.bool_)
     else:
-        return jnp.logical_not(jnp.array(mask.astype(int))).astype(jnp.bool_)
+        return jnp.logical_not(jnp.array(mask.astype(float))).astype(jnp.bool_)
 
 
 def check_input_data(
     data: ArrayLike, rms: ArrayLike, psf: ArrayLike, mask: ArrayLike = None
 ):
     """Check input data for certain conditions and raise warnings or exceptions if needed
 
@@ -718,7 +718,10 @@
         if jnp.sum(mask) / jnp.prod(jnp.array(mask.shape)) < 0.7:
             warnings.warn(
                 "More than 70 percent of input image is masked. Is this correct? (Pysersic treats True/1 as masked; you may need to flip your boolean array.) "
             )
         if mask.shape != data.shape:
             raise ShapeMatchError("Mask ndims must match input data ndims.")
     return True
+
+
+__version__ = "0.1.5"
```

### Comparing `pysersic-0.1.4/pysersic/rendering.py` & `pysersic-0.1.5/pysersic/rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from scipy.special import comb
 
 from .exceptions import *
 
 base_profile_types = [
     "sersic",
     "doublesersic",
+    "sersic_exp",
     "sersic_pointsource",
     "pointsource",
     "exp",
     "dev",
 ]
 base_profile_params = dict(
     zip(
@@ -33,14 +34,26 @@
                 "n_1",
                 "ellip_1",
                 "r_eff_2",
                 "n_2",
                 "ellip_2",
                 "theta",
             ],
+            [
+                "xc",
+                "yc",
+                "flux",
+                "f_1",
+                "r_eff_1",
+                "ellip_1",
+                "r_eff_2",
+                "n",
+                "ellip_2",
+                "theta",
+            ],
             ["xc", "yc", "flux", "f_ps", "r_eff", "n", "ellip", "theta"],
             ["xc", "yc", "flux"],
             ["xc", "yc", "flux", "r_eff", "ellip", "theta"],
             ["xc", "yc", "flux", "r_eff", "ellip", "theta"],
         ],
     )
 )
@@ -164,14 +177,37 @@
             "r_eff": params["r_eff_2"],
         }
         F1, im_int_1, im_obs_1 = self.render_sersic(dict_1)
         F2, im_int_2, im_obs_2 = self.render_sersic(dict_2)
 
         return F1 + F2, im_int_1 + im_int_2, im_obs_1 + im_obs_2
 
+    def render_sersic_exp(self, params: dict):
+        dict_1 = {
+            "xc": params["xc"],
+            "yc": params["yc"],
+            "flux": params["flux"] * params["f_1"],
+            "n": params["n"],
+            "ellip": params["ellip_1"],
+            "theta": params["theta"],
+            "r_eff": params["r_eff_1"],
+        }
+        dict_2 = {
+            "xc": params["xc"],
+            "yc": params["yc"],
+            "flux": params["flux"] * (1.0 - params["f_1"]),
+            "ellip": params["ellip_2"],
+            "theta": params["theta"],
+            "r_eff": params["r_eff_2"],
+        }
+        F1, im_int_1, im_obs_1 = self.render_sersic(dict_1)
+        F2, im_int_2, im_obs_2 = self.render_exp(dict_2)
+
+        return F1 + F2, im_int_1 + im_int_2, im_obs_1 + im_obs_2
+
     def render_sersic_pointsource(self, params: dict):
         pointsource_dict = {}
         sersic_dict = params.copy()
 
         sersic_dict["flux"] = (1.0 - params["f_ps"]) * params["flux"]
         pointsource_dict["flux"] = sersic_dict.pop("f_ps") * params["flux"]
         pointsource_dict["xc"] = sersic_dict["xc"]
```

### Comparing `pysersic-0.1.4/pysersic/results.py` & `pysersic-0.1.5/pysersic/results.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/pysersic.egg-info/PKG-INFO` & `pysersic-0.1.5/pysersic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysersic
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Tool for fitting sersic profiles in python
 Author-email: Imad Pasha <imad.pasha@yale.edu>, Tim Miller <timothy.miller@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2023 pysersic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysersic-0.1.4/tests/test_fitters.py` & `pysersic-0.1.5/tests/test_fitters.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/tests/test_loss.py` & `pysersic-0.1.5/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/tests/test_multiband.py` & `pysersic-0.1.5/tests/test_multiband.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/tests/test_priors.py` & `pysersic-0.1.5/tests/test_priors.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.4/tests/test_renderers.py` & `pysersic-0.1.5/tests/test_renderers.py`

 * *Files identical despite different names*

