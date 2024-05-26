# Comparing `tmp/thztools-0.4.0.tar.gz` & `tmp/thztools-0.4.1.tar.gz`

## Comparing `thztools-0.4.0.tar` & `thztools-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 thztools-0.4.0/.gitattributes
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 thztools-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 thztools-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/other.xml
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 thztools-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 thztools-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.4.0/logo/make_logo.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 thztools-0.4.0/paper/paper.bib
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 thztools-0.4.0/paper/paper.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.4.0/src/thztools/__about__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 thztools-0.4.0/src/thztools/__init__.py
--rw-r--r--   0        0        0    64696 2020-02-02 00:00:00.000000 thztools-0.4.0/src/thztools/thztools.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.4.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.4.0/LICENSE
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 thztools-0.4.0/README.md
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 thztools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 thztools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 thztools-0.4.1/.gitattributes
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 thztools-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 thztools-0.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/modules.xml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/other.xml
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 thztools-0.4.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 thztools-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.4.1/logo/make_logo.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 thztools-0.4.1/paper/paper.bib
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 thztools-0.4.1/paper/paper.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.4.1/src/thztools/__about__.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 thztools-0.4.1/src/thztools/__init__.py
+-rw-r--r--   0        0        0    71632 2020-02-02 00:00:00.000000 thztools-0.4.1/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 thztools-0.4.1/README.md
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 thztools-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7977 2020-02-02 00:00:00.000000 thztools-0.4.1/PKG-INFO
```

### Comparing `thztools-0.4.0/CHANGELOG.md` & `thztools-0.4.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,42 @@
 # Changelog
 
 [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
 
 Please follow the guidelines at [Common Changelog](https://common-changelog.org)
 for maintaining this file.
 
-## [0.4.0] - 2024-05-09
+## [0.4.1] - 2024-05-25
+
+### Changed
+
+- Refactor `options`
+- Use explicit `dt` keyword option instead of global option in examples
+- Change hatch doctest script from Sphinx to PyTest
+- Change signature of `fit`
+- Revise documentation for `fit`, `FitResult`, `get_option`, `set_option`,
+  `transfer`
+- Refactor `_costfuntls`
+
+### Added
+
+- Add version badges for pip and Anaconda
+- Add conda installation instructions
+- Add `FitResult` dataclass and use it to return `fit` output
+- Add `autouse` fixture to reset `sampling_time` option to default before each
+  test
+- Add Python 3.12 to testing workflow
+- Add global doctest imports explicitly to docstrings
+- Add `numpy_sign_convention` parameter to `fit`
+
+### Fixed
+
+- Fix scaling error in `_parse_noisefit_output`
+
+## [0.4.0] - 2024-05-10
 
 ### Changed
 
 - Rename module constant `global_options` as `options`
 - Rename `tdnoisefit` as `noisefit`
 - Rename `NoiseModel` attributes `alpha`, `beta` and `tau` as `sigma_alpha`,
   `sigma_beta` and `sigma_tau`, respectively
@@ -48,16 +75,14 @@
 - Add `paper` directory with bib-file and stub for JOSS paper
 - Add `draft-pdf.yml` GitHub Action to autogenerate JOSS paper; update
   deprecated `upload-artifact` Action in workflow
 - Add Contributing and Examples pages to documentation
 - Add Code of Conduct
 - Add gallery of Jupyter notebook examples to documentation using `nbsphinx`
 
-### Removed
-
 ### Fixed
 
 - Fix error in units of `NoiseModel.sigma_tau` in `noisefit`
 - Fix bug related to `eta` scaling in `noisefit`
 
 ## [0.3.6] - 2023-11-12
 
@@ -154,14 +179,15 @@
 - Add `fit` function (#25) (Alireza)
 - Add pytest classes for all functions (Steve)
 
 ### Removed
 
 - Remove `tdtf`
 
+[0.4.1]: https://github.com/dodge-research-group/thztools/releases/tag/v0.4.1
 [0.4.0]: https://github.com/dodge-research-group/thztools/releases/tag/v0.4.0
 [0.3.6]: https://github.com/dodge-research-group/thztools/releases/tag/v0.3.6
 [0.3.5]: https://github.com/dodge-research-group/thztools/releases/tag/v0.3.5
 [0.3.4]: https://github.com/dodge-research-group/thztools/releases/tag/v0.3.4
 [0.3.3]: https://github.com/dodge-research-group/thztools/releases/tag/v0.3.3
 [0.3.2]: https://github.com/dodge-research-group/thztools/releases/tag/v0.3.2
 [0.3.1]: https://github.com/dodge-research-group/thztools/releases/tag/v0.3.1
```

### Comparing `thztools-0.4.0/CODE_OF_CONDUCT.md` & `thztools-0.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/.idea/thztools.iml` & `thztools-0.4.1/.idea/thztools.iml`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.4.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/logo/make_logo.py` & `thztools-0.4.1/logo/make_logo.py`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/paper/paper.bib` & `thztools-0.4.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/paper/paper.md` & `thztools-0.4.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/src/thztools/__init__.py` & `thztools-0.4.1/src/thztools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+"""
+THzTools provides data analysis software tools for terahertz time-domain
+spectroscopy (THz-TDS).
+"""
 from thztools.__about__ import __version__
 from thztools.thztools import (
+    FitResult,
     GlobalOptions,
     NoiseModel,
     NoiseResult,
     fit,
     get_option,
     noisefit,
     options,
     scaleshift,
     set_option,
     timebase,
     transfer,
     wave,
 )
 
-set_option("sampling_time", None)
-
 __all__ = [
+    "FitResult",
     "GlobalOptions",
     "NoiseModel",
     "NoiseResult",
     "fit",
     "get_option",
     "noisefit",
     "options",
```

### Comparing `thztools-0.4.0/src/thztools/thztools.py` & `thztools-0.4.1/src/thztools/thztools.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 import numpy as np
 import scipy.linalg as la
 import scipy.optimize as opt
 from numpy.fft import irfft, rfft, rfftfreq
 from numpy.random import default_rng
 from numpy.typing import ArrayLike, NDArray
 from scipy import signal
-from scipy.optimize import OptimizeResult, minimize
-from scipy.optimize import approx_fprime as fprime
+from scipy.linalg import sqrtm
+from scipy.optimize import OptimizeResult, approx_fprime, minimize
 
 NUM_NOISE_PARAMETERS = 3
 NUM_NOISE_DATA_DIMENSIONS = 2
 
 
 @dataclass
 class GlobalOptions:
     r"""
-    Class for global options.
+    Class for storing global options.
 
     Attributes
     ----------
     sampling_time : float | None, optional
         Global sampling time, normally in picoseconds. When set to None, the
         default, times and frequencies are treated as dimensionless quantities
         that are scaled by the (undetermined) sampling time.
     """
-    sampling_time: float | None
+    sampling_time: float | None = None
 
 
-options = GlobalOptions
+#: Instance of ``GlobalOptions`` that stores global options.
+options = GlobalOptions()
 
 
 def set_option(key: str, value: Any) -> None:
     r"""
     Set global option.
 
     Parameters
@@ -47,14 +48,32 @@
     value : object
         Option value.
 
     Returns
     -------
     None
         No return value.
+
+    Notes
+    -----
+    Available options, with descriptions:
+
+    sampling_time : float | None
+        Global sampling time, normally in picoseconds. When set to None, the
+        default, times and frequencies are treated as dimensionless quantities
+        that are scaled by the (undetermined) sampling time.
+
+    Examples
+    --------
+    >>> import thztools as thz
+    >>> thz.set_option("sampling_time", 0.05)
+    >>> thz.get_option("sampling_time")
+    0.05
+    >>> thz.set_option("sampling_time", None)
+    >>> thz.get_option("sampling_time")
     """
     setattr(options, key, value)
 
 
 def get_option(key: str) -> Any:
     r"""
     Get global option.
@@ -64,14 +83,32 @@
     key : str
         Option name.
 
     Returns
     -------
     val : object
         Option value.
+
+    Notes
+    -----
+    Available options, with descriptions:
+
+    sampling_time : float | None
+        Global sampling time, normally in picoseconds. When set to None, the
+        default, times and frequencies are treated as dimensionless quantities
+        that are scaled by the (undetermined) sampling time.
+
+    Examples
+    --------
+    >>> import thztools as thz
+    >>> thz.set_option("sampling_time", 0.05)
+    >>> thz.get_option("sampling_time")
+    0.05
+    >>> thz.set_option("sampling_time", None)
+    >>> thz.get_option("sampling_time")
     """
     return getattr(options, key)
 
 
 def _assign_sampling_time(dt: float | None) -> float:
     dt_out = 1.0
     if dt is None and get_option("sampling_time") is not None:
@@ -149,20 +186,19 @@
     simulated signal :math:`\mu(t)`. The signal amplitude is normalized to
     its peak magnitude, :math:`\mu_0`. The noise variance is normalized to
     :math:`(\sigma_\beta\mu_0)^2`.
 
     >>> import thztools as thz
     >>> from matplotlib import pyplot as plt
     >>> n, dt = 256, 0.05
-    >>> thz.set_option("sampling_time", dt)
-    >>> t = thz.timebase(n)
+    >>> t = thz.timebase(n, dt=dt)
     >>> mu = thz.wave(n)
     >>> alpha, beta, tau = 1e-4, 1e-2, 1e-3
     >>> noise_model = thz.NoiseModel(sigma_alpha=alpha, sigma_beta=beta,
-    ...  sigma_tau=tau)
+    ...  sigma_tau=tau, dt=dt)
     >>> noise_variance = noise_model.noise_var(mu)
 
     >>> _, axs = plt.subplots(2, 1, sharex=True, layout="constrained")
     >>> axs[0].plot(t, noise_variance / beta**2)
     >>> axs[0].set_ylabel(r"$\sigma^2/(\sigma_\beta\mu_0)^2$")
     >>> axs[1].plot(t, mu)
     >>> axs[1].set_ylabel(r"$\mu/\mu_0$")
@@ -222,20 +258,19 @@
         simulated signal :math:`\mu(t)`. The signal amplitude is normalized to
         its peak magnitude, :math:`\mu_0`. The noise variance is normalized to
         :math:`(\sigma_\beta\mu_0)^2`.
 
         >>> import thztools as thz
         >>> from matplotlib import pyplot as plt
         >>> n, dt = 256, 0.05
-        >>> thz.set_option("sampling_time", dt)
-        >>> t = thz.timebase(n)
-        >>> mu = thz.wave(n)
+        >>> t = thz.timebase(n, dt=dt)
+        >>> mu = thz.wave(n, dt=dt)
         >>> alpha, beta, tau = 1e-4, 1e-2, 1e-3
         >>> noise_model = thz.NoiseModel(sigma_alpha=alpha, sigma_beta=beta,
-        ... sigma_tau=tau)
+        ... sigma_tau=tau, dt=dt)
         >>> noise_variance = noise_model.noise_var(mu)
 
         >>> _, axs = plt.subplots(2, 1, sharex=True, layout="constrained")
         >>> axs[0].plot(t, noise_variance / beta**2)
         >>> axs[0].set_ylabel(r"$\sigma^2/(\sigma_\beta\mu_0)^2$")
         >>> axs[1].plot(t, mu)
         >>> axs[1].set_ylabel(r"$\mu/\mu_0$")
@@ -313,20 +348,19 @@
         simulated signal :math:`\mu(t)`. The signal amplitude is normalized to
         its peak magnitude, :math:`\mu_0`. The noise amplitude is normalized to
         :math:`\sigma_\beta\mu_0`.
 
         >>> import thztools as thz
         >>> from matplotlib import pyplot as plt
         >>> n, dt = 256, 0.05
-        >>> thz.set_option("sampling_time", dt)
-        >>> t = thz.timebase(n)
-        >>> mu = thz.wave(n)
+        >>> t = thz.timebase(n, dt=dt)
+        >>> mu = thz.wave(n, dt=dt)
         >>> alpha, beta, tau = 1e-4, 1e-2, 1e-3
         >>> noise_model = thz.NoiseModel(sigma_alpha=alpha, sigma_beta=beta,
-        ... sigma_tau=tau)
+        ... sigma_tau=tau, dt=dt)
         >>> noise_amplitude = noise_model.noise_amp(mu)
 
         >>> _, axs = plt.subplots(2, 1, sharex=True, layout="constrained")
         >>> axs[0].plot(t, noise_amplitude / beta)
         >>> axs[0].set_ylabel(r"$\sigma/(\sigma_\beta\mu_0)$")
         >>> axs[1].plot(t, mu)
         >>> axs[1].set_ylabel(r"$\mu/\mu_0$")
@@ -387,20 +421,19 @@
         :math:`\sigma_\mu(t_k)\epsilon(t_k)` for noise parameters
         :math:`\sigma_\alpha = 10^{-4}`, :math:`\sigma_\beta = 10^{-2}`,
         :math:`\sigma_\tau = 10^{-3}` and the simulated signal :math:`\mu(t)`.
 
         >>> import thztools as thz
         >>> from matplotlib import pyplot as plt
         >>> n, dt = 256, 0.05
-        >>> thz.set_option("sampling_time", dt)
-        >>> t = thz.timebase(n)
-        >>> mu = thz.wave(n)
+        >>> t = thz.timebase(n, dt=dt)
+        >>> mu = thz.wave(n, dt=dt)
         >>> alpha, beta, tau = 1e-4, 1e-2, 1e-3
         >>> noise_model = thz.NoiseModel(sigma_alpha=alpha, sigma_beta=beta,
-        ... sigma_tau=tau)
+        ... sigma_tau=tau, dt=dt)
         >>> noise = noise_model.noise_sim(mu, seed=1234)
 
         >>> _, axs = plt.subplots(2, 1, sharex=True, layout="constrained")
         >>> axs[0].plot(t, noise / beta)
         >>> axs[0].set_ylabel(r"$\sigma_\mu\epsilon/(\sigma_\beta\mu_0)$")
         >>> axs[1].plot(t, mu)
         >>> axs[1].set_ylabel(r"$\mu/\mu_0$")
@@ -510,17 +543,17 @@
         sampling time is set to ``1.0``. In this case, the angular frequency
         ``omega`` must be given in units of radians per sampling time, and any
         parameters in ``args`` must be expressed with the sampling time as the
         unit of time.
     numpy_sign_convention : bool, optional
         Adopt NumPy sign convention for harmonic time dependence, e.g, express
         a harmonic function with frequency :math:`\omega` as
-        :math:`x(t) = a e^{i\omega t}`. Default is ``True``. Uses the
-        convention more common in physics, :math:`x(t) = a e^{-i\omega t}`,
-        when set to ``False``.
+        :math:`x(t) = a e^{i\omega t}`. Default is ``True``. When set to
+        ``False``, uses the convention more common in physics,
+        :math:`x(t) = a e^{-i\omega t}`.
     args : tuple, optional
         Extra arguments passed to the transfer function.
 
     Returns
     -------
     y : ndarray
         Result of applying the transfer function to ``x``.
@@ -559,53 +592,51 @@
     If the transfer function is expressed using the :math:`e^{-i\omega t}`
     representation, more common in physics,
 
     .. math:: H(\omega) = a\exp(i\omega\tau),
 
     set ``fft_sign=False``.
 
+    >>> import numpy as np
     >>> import thztools as thz
     >>> from matplotlib import pyplot as plt
     >>> n, dt = 256, 0.05
-    >>> thz.set_option("sampling_time", dt)
-    >>> t = thz.timebase(n)
-    >>> x = thz.wave(n)
+    >>> t = thz.timebase(n, dt=dt)
+    >>> x = thz.wave(n, dt=dt)
     >>> def shiftscale(_w, _a, _tau):
     ...     return _a * np.exp(-1j * _w * _tau)
     >>>
-    >>> y = thz.transfer(shiftscale, x,
+    >>> y = thz.transfer(shiftscale, x, dt=dt,
     ...                  numpy_sign_convention=True,
     ...                  args=(0.5, 1))
 
     >>> _, ax = plt.subplots()
     >>>
     >>> ax.plot(t, x, label='x')
     >>> ax.plot(t, y, label='y')
-    >>>
     >>> ax.legend()
     >>> ax.set_xlabel('t (ps)')
     >>> ax.set_ylabel('Amplitude (arb. units)')
-    >>>
     >>> plt.show()
 
     >>> def shiftscale_phys(_w, _a, _tau):
     ...     return _a * np.exp(1j * _w * _tau)
     >>>
     >>> y_p = thz.transfer(shiftscale_phys, x,
     ...                    numpy_sign_convention=False,
     ...                    args=(0.5, 1))
 
     >>> _, ax = plt.subplots()
     >>>
-    >>> ax.plot(t, x, label='x');
-    >>> ax.plot(t, y_p, label='y');
+    >>> ax.plot(t, x, label='x')
+    >>> ax.plot(t, y_p, label='y')
     >>>
-    >>> ax.legend();
-    >>> ax.set_xlabel('t (ps)');
-    >>> ax.set_ylabel('Amplitude (arb. units)');
+    >>> ax.legend()
+    >>> ax.set_xlabel('t (ps)')
+    >>> ax.set_ylabel('Amplitude (arb. units)')
     >>>
     >>> plt.show()
     """
     x = np.asarray(x, dtype=np.float64)
     if x.ndim != 1:
         msg = "x must be a one-dimensional array"
         raise ValueError(msg)
@@ -665,14 +696,15 @@
 
     Examples
     --------
     The following example computes the timebase with different methods for
     assigning the sampling time.
 
     >>> import thztools as thz
+    >>> thz.set_option("sampling_time", None)
     >>> n, dt, t_init = 256, 0.05, 2.5
     >>> t_1 = thz.timebase(n)
     >>> t_2 = thz.timebase(n, dt=dt)
     >>> thz.set_option("sampling_time", dt)
     >>> t_3 = thz.timebase(n)
     >>> t_4 = thz.timebase(n, t_init=t_init)
     >>> print(t_1[:3])
@@ -758,22 +790,21 @@
     --------
     The following example shows the simulated signal :math:`\mu(t)` normalized
     to its peak magnitude, :math:`\mu_0`.
 
     >>> import thztools as thz
     >>> from matplotlib import pyplot as plt
     >>> n, dt = 256, 0.05
-    >>> thz.set_option("sampling_time", dt)
-    >>> t = thz.timebase(n)
-    >>> mu = thz.wave(n)
+    >>> t = thz.timebase(n, dt=dt)
+    >>> mu = thz.wave(n, dt=dt)
 
     >>> _, ax = plt.subplots(layout="constrained")
-    >>> ax.plot(t, mu);
-    >>> ax.set_xlabel("t (ps)");
-    >>> ax.set_ylabel(r"$\mu/\mu_0$");
+    >>> ax.plot(t, mu)
+    >>> ax.set_xlabel("t (ps)")
+    >>> ax.set_ylabel(r"$\mu/\mu_0$")
     >>> plt.show()
     """
     dt = _assign_sampling_time(dt)
     if t0 is None:
         t0 = 0.3 * n * dt
 
     if taur is None:
@@ -846,30 +877,30 @@
     Examples
     --------
     The following example makes an array with 4 identical copies of the
     signal ``mu`` returned by :func:`wave`. It then uses :func:`scaleshift` to
     rescale each copy by ``a = [1.0, 0.5, 0.25, 0.125]`` and shift it by
     ``eta = [0.0, 1.0, 2.0, 3.0]``.
 
+    >>> import numpy as np
     >>> import thztools as thz
     >>> from matplotlib import pyplot as plt
     >>> n, dt = 256, 0.05
-    >>> thz.set_option("sampling_time", dt)
-    >>> t = thz.timebase(n)
-    >>> mu = thz.wave(n)
+    >>> t = thz.timebase(n, dt=dt)
+    >>> mu = thz.wave(n, dt=dt)
     >>> m = 4
     >>> x = np.repeat(np.atleast_2d(mu), m, axis=0)
     >>> a = 0.5**np.arange(m)
     >>> eta = np.arange(m)
     >>> x_adj = thz.scaleshift(x, a=a, eta=eta, dt=dt)
 
-    >>> plt.plot(t, x_adj.T, label=[f"{k=}" for k in range(4)]);
-    >>> plt.legend();
-    >>> plt.xlabel("t (ps)");
-    >>> plt.ylabel(r"$x_{\mathrm{adj}, k}$");
+    >>> plt.plot(t, x_adj.T, label=[f"{k=}" for k in range(4)])
+    >>> plt.legend()
+    >>> plt.xlabel("t (ps)")
+    >>> plt.ylabel(r"$x_{\mathrm{adj}, k}$")
     >>> plt.show()
     """
     x = np.asarray(x, dtype=np.float64)
     if x.size == 0:
         return np.empty(x.shape)
 
     dt = _assign_sampling_time(dt)
@@ -978,21 +1009,18 @@
     x = np.asarray(x, dtype=np.float64)
     y = np.asarray(y, dtype=np.float64)
     sigma_x = np.asarray(sigma_x, dtype=np.float64)
     sigma_y = np.asarray(sigma_y, dtype=np.float64)
 
     dt = _assign_sampling_time(dt)
 
-    n = x.shape[-1]
-    delta_norm = (x - mu) / sigma_x
-    w = 2 * np.pi * rfftfreq(n) / dt
-    h_f = fun(theta, w)
-
-    eps_norm = (y - irfft(rfft(mu) * h_f, n=n)) / sigma_y
+    psi = transfer(lambda omega: fun(theta, omega), mu, dt=dt)
 
+    delta_norm = (x - mu) / sigma_x
+    eps_norm = (y - psi) / sigma_y
     res = np.concatenate((delta_norm, eps_norm))
 
     return res
 
 
 def _costfun_noisefit(
     x: NDArray[np.float64],
@@ -1339,40 +1367,41 @@
     Examples
     --------
     In basic usage, it should be possible to call ``noisefit`` with just
     the data array. In the code below, we simulate ``m = 50`` noisy waveforms
     with ``n = 256`` time points each, then verify that the fit results are
     consistent with the true noise parameters.
 
+    >>> import numpy as np
     >>> import thztools as thz
     >>> from matplotlib import pyplot as plt
     >>> rng = np.random.default_rng(0)
     >>> n, m, dt = 256, 50, 0.05
-    >>> thz.set_option("sampling_time", dt)
-    >>> t = thz.timebase(n)
-    >>> mu = thz.wave(n)
-    >>> alpha, beta, tau = 1e-5, 1e-2, 1e-3
+    >>> t = thz.timebase(n, dt=dt)
+    >>> mu = thz.wave(n, dt=dt)
+    >>> alpha, beta, tau = 1e-4, 1e-2, 1e-3
     >>> noise_model = thz.NoiseModel(sigma_alpha=alpha, sigma_beta=beta,
-    ...  sigma_tau=tau)
+    ...  sigma_tau=tau, dt=dt)
     >>> a = 1.0 + 1e-2 * np.concatenate(([0.0],
     ...                                 rng.standard_normal(m - 1)))
     >>> eta = 1e-3 * np.concatenate(([0.0], rng.standard_normal(m - 1)))
-    >>> z = thz.scaleshift(np.repeat(np.atleast_2d(mu), m, axis=0),
+    >>> z = thz.scaleshift(np.repeat(np.atleast_2d(mu), m, axis=0), dt=dt,
     ...                    a=a, eta=eta).T  # Orient the array columnwise
     >>> x = z + noise_model.noise_sim(z, axis=1, seed=1234)
-    >>> noise_res = thz.noisefit(x)
+    >>> noise_res = thz.noisefit(x, sigma_alpha0=alpha, sigma_beta0=beta,
+    ...  sigma_tau0=tau, dt=dt)
     >>> noise_res.noise_model  #doctest: +NORMALIZE_WHITESPACE
-    NoiseModel(sigma_alpha=1.000...e-05, sigma_beta=0.009609...,
-    sigma_tau=0.0009243..., dt=0.05)
+    NoiseModel(sigma_alpha=9.9...e-05, sigma_beta=0.0096...,
+    sigma_tau=4.27...e-06, dt=0.05)
 
     >>> plt.plot(t, np.std(thz.scaleshift(x, a=1 / noise_res.a,
     ... eta=-noise_res.eta, axis=0), axis=1), "-",
     ... label="Data")
     >>> plt.plot(t, noise_res.noise_model.noise_amp(noise_res.mu)
-    ...  * np.sqrt(m / (m + 1)), "--", label="Fit")
+    ...  * np.sqrt(m / (m - 1)), "--", label="Fit")
     >>> plt.legend()
     >>> plt.xlabel("t (ps)")
     >>> plt.ylabel(r"$\sigma(t)$")
     >>> plt.show()
     """
     x = np.asarray(x, dtype=np.float64)
     dt = _assign_sampling_time(dt)
@@ -1689,15 +1718,15 @@
         beta = sigma_beta0
     else:
         beta = np.exp(x_out[0] / 2) * scale_sigma_beta
         x_out = x_out[1:]
     if fix_sigma_tau:
         tau = sigma_tau0
     else:
-        tau = np.exp(x_out[0] / 2) * scale_sigma_tau * dt
+        tau = np.exp(x_out[0] / 2) * scale_sigma_tau
         x_out = x_out[1:]
     # noinspection PyArgumentList
     noise_model = NoiseModel(alpha, beta, tau, dt=dt)
 
     if fix_mu:
         mu_out = mu0
     else:
@@ -1797,177 +1826,308 @@
         err_mu,
         err_a,
         err_eta,
         diagnostic,
     )
 
 
+@dataclass
+class FitResult:
+    r"""
+    Dataclass for the output of :func:`fit`.
+
+    Parameters
+    ----------
+    p_opt : array_like
+        Optimal fit parameters.
+    p_var : array_like
+        Variance of p_opt.
+    mu_opt : array_like
+        Optimal underlying waveform.
+    mu_var : array_like
+        Variance of mu_opt.
+    resnorm : float
+        The value of chi-squared.
+    delta : array_like
+        Residuals of the input waveform ``x``, defined as ``x - mu_opt``.
+    epsilon : array_like
+        Residuals of the output waveform ``y``, defined as ``y - psi_opt``,
+        where ``psi_opt = thztools.transfer(tfun_opt, mu, dt=dt)`` and
+        ``tfun_opt`` is the parameterized transfer function evaluated at
+        ``p_opt``.
+    r_tls : array_like
+        Total least-squares residuals.
+    success : bool
+        True if one of the convergence criteria is satisfied.
+
+    See Also
+    --------
+    fit : Fit a transfer function to time-domain data.
+    """
+    p_opt: NDArray[np.float64]
+    p_var: NDArray[np.float64]
+    mu_opt: NDArray[np.float64]
+    mu_var: NDArray[np.float64]
+    resnorm: float
+    delta: NDArray[np.float64]
+    epsilon: NDArray[np.float64]
+    r_tls: NDArray[np.float64]
+    success: bool
+
+
 def fit(
     fun: Callable,
+    xdata: ArrayLike,
+    ydata: ArrayLike,
     p0: ArrayLike,
-    x: ArrayLike,
-    y: ArrayLike,
+    noise_parms: ArrayLike | None = None,
     *,
     dt: float | None = None,
-    sigma_parms: ArrayLike = (1.0, 0.0, 0.0),
-    f_bounds: ArrayLike = (0.0, np.inf),
+    numpy_sign_convention: bool = True,
+    f_bounds: ArrayLike | None = None,
     p_bounds: ArrayLike | None = None,
     jac: Callable | None = None,
-    args: ArrayLike = (),
-    kwargs: dict | None = None,
-) -> dict:
+) -> FitResult:
     r"""
     Fit a transfer function to time-domain data.
 
-    Computes the noise on the input ``x`` and output ``y`` time series using
-    a given ``NoiseModel``. Uses the total residuals generated by
-    ``_costfuntls`` to fit the input and output to the transfer function.
+    Determines the total least-squares fit to ``xdata`` and ``ydata``, given
+    the parameterized transfer function relationship ``fun`` and noise model
+    parameters ``noise_parms``.
 
     Parameters
     ----------
     fun : callable
-        Transfer function.
-
-            ``fun(p, w, *args, **kwargs) -> ndarray``
-
-        Assumes the :math:`+i\omega t` convention for harmonic time dependence.
-    p0 : array_like
-        Initial guess for ``p``.
-    x : array_like
+        Transfer function with signature ``fun(omega, *p, *args, **kwargs)``
+        that returns an ``ndarray``. Assumes the :math:`+i\omega t` convention
+        for harmonic time dependence when ``numpy_sign_convention`` is
+        ``True``, the default.
+    xdata : array_like
         Measured input signal.
-    y : array_like
+    ydata : array_like
         Measured output signal.
+    p0 : array_like
+        Initial guess for the parameters ``p``.
+    noise_parms : array_like or None, optional
+        Noise parameters ``(sigma_alpha, sigma_beta, sigma_tau)`` used to
+        define the :class:``NoiseModel`` for the fit. Default is ``None``,
+        which sets ``noise_parms`` to ``(1.0, 0.0, 0.0)``.
     dt : float or None, optional
-        Sampling time, normally in picoseconds. Default is None, which sets
-        the sampling time to ``thztools.options.sampling_time``. If both
-        ``dt`` and ``thztools.options.sampling_time`` are ``None``, the
-        sampling time is set to ``1.0``. In this case, the angular frequency
-        ``omega`` must be given in units of radians per sampling time, and any
-        parameters in ``args`` must be expressed with the sampling time as the
-        unit of time.
-    sigma_parms : None or array_like, optional
-        Noise parameters with size (3,), expressed as standard deviation
-        amplitudes.
+        Sampling time, normally in picoseconds. Default is ``None``, which sets
+        ``dt`` to ``thztools.options.sampling_time``. If both ``dt`` and
+        ``thztools.options.sampling_time`` are ``None``, ``dt`` is set to
+        ``1.0``. In this case, the angular frequency ``omega`` must be given in
+        units of radians per sampling time, and any parameters in ``args`` must
+        be expressed with ``dt`` as the unit of time.
+    numpy_sign_convention : bool, optional
+        Adopt NumPy sign convention for harmonic time dependence, e.g, express
+        a harmonic function with frequency :math:`\omega` as
+        :math:`x(t) = a e^{i\omega t}`. Default is ``True``. When set to
+        ``False``, uses the convention more common in physics,
+        :math:`x(t) = a e^{-i\omega t}`.
     f_bounds : array_like, optional
-        Frequency bounds.
+        Frequency bounds. Default is ``None``, which sets ``f_bounds`` to
+        ``(0.0, np.inf)``.
     p_bounds : None, 2-tuple of array_like, or Bounds, optional
-        Lower and upper bounds on fit parameter(s).
+        Lower and upper bounds on fit parameter(s). Default is ``None``, which
+        sets all parameter bounds to ``(-np.inf, np.inf)``.
     jac : None or callable, optional
-        Method of calculating derivative of the output signal residuals
-        with respect to the fit parameter(s), theta.
-    args : tuple, optional
-        Additional arguments passed to ``fun`` and ``jac``.
-    kwargs : dict, optional
-        Additional keyword arguments passed to ``fun`` and ``jac``.
+        Jacobian of the residuals with respect to the fit parameters, with
+        signature ``jac(p, w, *args, **kwargs)``. Default is ``None``, which
+        uses :func:`scipy.optimize.approx_fprime`.
 
     Returns
     -------
-    p : dict
-        Output parameter dictionary containing:
+    res : FitResult
+        Fit result represented as a :class:`FitResult` object. Important
+        attributes are: ``p_opt``, the optimal fit parameter values; ``p_cov``,
+        the parameter covariance matrix estimated from fit; ``resnorm``,
+        the value of the total least-squares cost function for the fit;
+        ``r_tls``, and ``success``, which is `True` when the fit converges. See
+        the *Notes* section below and the :class:`FitResult` documentation for
+        more details and for a description of other attributes.
 
-            p_opt : array_like
-                Optimal fit parameters.
-            p_cov : array_like
-                Variance of p_opt.
-            mu_opt : array_like
-                Optimal underlying waveform.
-            mu_var : array_like
-                Variance of mu_opt.
-            resnorm : float
-                The value of chi-squared.
-            delta : array_like
-                Residuals of the input waveform ``x``.
-            epsilon : array_like
-                Resiuals of the output waveform ``y``.
-            success : bool
-                True if one of the convergence criteria is satisfied.
+    Raises
+    ------
+    ValueError
+        If ``noise_parms`` does not have 3 elements.
 
     Warns
     -----
     UserWarning
         If ``thztools.options.sampling_time`` and the ``dt`` parameter
         are both not ``None`` and are set to different ``float`` values, the
         function will set the sampling time to ``dt`` and raise a
         :class:`UserWarning`.
+
+    See Also
+    --------
+    NoiseModel : Noise model class.
+
+    Notes
+    -----
+    This function computes the maximum-likelihood estimate for the parameters
+    :math:`\boldsymbol{\theta}` in the transfer function model
+    :math:`H(\omega; \boldsymbol{\theta})` by minimizing
+    the total least-squares cost function
+
+    .. math:: Q_\text{TLS}(\boldsymbol{\theta}) \
+        = \sum_{k=0}^{N-1}\left[ \
+        \frac{(x_k - \mu_k)^2}{\sigma_{\mathbf{x},k}^2} \
+        + \frac{(y_k - \psi_k)^2}{\sigma_{\mathbf{y},k}^2} \
+        \right],
+
+    where :math:`\mathbf{x}` is the input signal array, :math:`\mathbf{y}`
+    is the output signal array, and :math:`\boldsymbol{\sigma}_{\mathbf{y}}`,
+    :math:`\boldsymbol{\sigma}_{\mathbf{y}}` are their associated noise
+    amplitudes. The arrays :math:`\boldsymbol{\mu}` and
+    :math:`\boldsymbol{\psi}` are the ideal input and output signal arrays,
+    respectively, which are related by the constraint
+
+    .. math:: [\mathcal{F}\boldsymbol{\psi}]_k = \
+        [H(\omega_k; \boldsymbol{\theta})] \
+        [\mathcal{F}\boldsymbol{\mu}]_k
+
+    at all discrete Fourier transform frequencies :math:`\omega_k` within
+    the frequency bounds.
+
+    The optimization step uses :func:`scipy.optimize.least_squares` with ``p``
+    and ``mu`` as free parameters. It minimizes the Euclidean norm of the
+    residual vector ``np.concat((delta / sigma_x, epsilon / sigma_y)``, where
+    ``delta = xdata - mu``, ``epsilon = ydata - psi``,
+    ``sigma_x = NoiseModel(*noise_parms, dt=dt).noise_amp(xdata)``,
+    ``sigma_y = NoiseModel(*noise_parms, dt=dt).noise_amp(ydata)``, and
+    ``psi = thz.transfer(fun(omega, *p, *args, **kwargs), mu, dt=dt)``.
+
+    References
+    ----------
+    .. [1] Laleh Mohtashemi, Paul Westlund, Derek G. Sahota, Graham B. Lea,
+        Ian Bushfield, Payam Mousavi, and J. Steven Dodge, "Maximum-
+        likelihood parameter estimation in terahertz time-domain
+        spectroscopy," Opt. Express **29**, 4912-4926 (2021),
+        `<https://doi.org/10.1364/OE.417724>`_.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import thztools as thz
+    >>> from matplotlib import pyplot as plt
+    >>> n, dt = 256, 0.05
+    >>> t = thz.timebase(n, dt=dt)
+    >>> mu = thz.wave(n, dt=dt)
+    >>> alpha, beta, tau = 1e-4, 1e-2, 1e-3
+    >>> noise_model = thz.NoiseModel(sigma_alpha=alpha, sigma_beta=beta,
+    ...  sigma_tau=tau, dt=dt)
+
+    >>> def tfun(p, w):
+    ...    return p[0] * np.exp(1j * p[1] * w)
+    >>>
+    >>> p0 = (0.5, 1.0)
+    >>> psi = thz.transfer(lambda omega: tfun(p0, omega), mu, dt=dt)
+    >>> xdata = mu + noise_model.noise_sim(mu, seed=0)
+    >>> ydata = psi + noise_model.noise_sim(psi, seed=1)
+    >>> result = thz.fit(tfun, xdata, ydata, p0, (alpha, beta, tau), dt=dt)
+    >>> result.p_opt
+    array([0.499..., 1.000...])
+    >>> result.resnorm
+    198.300...
+
+    >>> _, ax = plt.subplots()
+    >>> ax.plot(t, result.r_tls, '.')
+    >>> ax.set_xlabel("t (ps)")
+    >>> ax.set_ylabel(r"$r_\mathrm{TLS}$")
+    >>> plt.show()
     """
     fit_method = "trf"
 
     p0 = np.asarray(p0, dtype=np.float64)
-    x = np.asarray(x, dtype=np.float64)
-    y = np.asarray(y, dtype=np.float64)
-    sigma_parms = np.asarray(sigma_parms, dtype=np.float64)
+    xdata = np.asarray(xdata, dtype=np.float64)
+    ydata = np.asarray(ydata, dtype=np.float64)
+    if noise_parms is None:
+        noise_parms = np.asarray((1.0, 0.0, 0.0), dtype=np.float64)
+    else:
+        noise_parms = np.asarray(noise_parms, dtype=np.float64)
+
+    if noise_parms.size != NUM_NOISE_PARAMETERS:
+        msg = f"sigma_parms must be a tuple of length {NUM_NOISE_PARAMETERS:d}"
+        raise ValueError(msg)
 
     dt = _assign_sampling_time(dt)
 
-    n = y.shape[-1]
+    n = ydata.shape[-1]
     n_p = len(p0)
 
+    if f_bounds is None:
+        f_bounds = np.array((0.0, np.inf), dtype=np.float64)
+
     if p_bounds is None:
         p_bounds = (-np.inf, np.inf)
         fit_method = "lm"
     else:
         p_bounds = np.asarray(p_bounds, dtype=np.float64)
         if p_bounds.shape[0] == 2:  # noqa: PLR2004
             p_bounds = (
                 np.concatenate((p_bounds[0], np.full((n,), -np.inf))),
                 np.concatenate((p_bounds[1], np.full((n,), np.inf))),
             )
         else:
             msg = "`bounds` must contain 2 elements."
             raise ValueError(msg)
 
-    if kwargs is None:
-        kwargs = {}
-
     w = 2 * np.pi * rfftfreq(n, dt)
     w_bounds = 2 * np.pi * np.asarray(f_bounds, dtype=np.float64)
     w_below_idx = w <= w_bounds[0]
     w_above_idx = w > w_bounds[1]
     w_in_idx = np.invert(w_below_idx) * np.invert(w_above_idx)
     n_f = len(w)
 
-    alpha, beta, tau = sigma_parms
+    alpha, beta, tau = noise_parms
     # noinspection PyArgumentList
     noise_model = NoiseModel(alpha, beta, tau, dt=dt)
-    sigma_x = noise_model.noise_amp(x)
-    sigma_y = noise_model.noise_amp(y)
+    sigma_x = noise_model.noise_amp(xdata)
+    sigma_y = noise_model.noise_amp(ydata)
     p0_est = np.concatenate((p0, np.zeros(n)))
 
     def etfe(_x, _y):
-        return rfft(_y) / rfft(_x)
+        h = rfft(_y) / rfft(_x)
+        if numpy_sign_convention:
+            h = np.conj(h)
+        return h
 
     def function(_theta, _w):
-        _h = etfe(x, y)
+        _h = etfe(xdata, ydata)
         _w_in = _w[w_in_idx]
-        return np.concatenate(
-            (
-                _h[w_below_idx],
-                fun(_theta, _w_in, *args, **kwargs),
-                _h[w_above_idx],
-            )
-        )
+        h_lo = _h[w_below_idx]
+        h_in = fun(_theta, _w_in)
+        h_hi = _h[w_above_idx]
+        if not numpy_sign_convention:
+            h_in = np.conj(h_in)
+        return np.concatenate((h_lo, h_in, h_hi))
 
     def function_flat(_x):
         _tf = function(_x, w)
         return np.concatenate((np.real(_tf), np.imag(_tf)))
 
     def td_fun(_p, _x):
-        _h = irfft(rfft(_x) * function(_p, w), n=n)
+        if numpy_sign_convention:
+            _h = irfft(rfft(_x) * function(_p, w), n=n)
+        else:
+            _h = irfft(rfft(_x) * np.conj(function(_p, w)), n=n)
         return _h
 
     def jacobian(_p):
         if jac is None:
-            _tf_prime = fprime(_p, function_flat)
+            _tf_prime = approx_fprime(_p, function_flat)
             return _tf_prime[0:n_f] + 1j * _tf_prime[n_f:]
         else:
-            return jac(_p, w, *args, **kwargs)
+            return jac(_p, w)
 
     def jac_fun(_x):
         p_est = _x[:n_p]
-        mu_est = x[:] - _x[n_p:]
+        mu_est = xdata[:] - _x[n_p:]
         jac_tl = np.zeros((n, n_p))
         jac_tr = np.diag(1 / sigma_x)
         jac_bl = -(
             irfft(rfft(mu_est) * np.atleast_2d(jacobian(p_est)).T, n=n)
             / sigma_y
         ).T
         jac_br = (
@@ -1976,36 +2136,54 @@
         jac_tot = np.block([[jac_tl, jac_tr], [jac_bl, jac_br]])
         return jac_tot
 
     result = opt.least_squares(
         lambda _p: _costfuntls(
             function,
             _p[:n_p],
-            x[:] - _p[n_p:],
-            x[:],
-            y[:],
+            xdata[:] - _p[n_p:],
+            xdata[:],
+            ydata[:],
             sigma_x,
             sigma_y,
             dt,
         ),
         p0_est,
         jac=jac_fun,
         bounds=p_bounds,
         method=fit_method,
         x_scale=np.concatenate((np.ones(n_p), sigma_x)),
     )
 
     # Parse output
-    p = {}
-    p["p_opt"] = result.x[:n_p]
-    p["mu_opt"] = x - result.x[n_p:]
     _, s, vt = la.svd(result.jac, full_matrices=False)
     threshold = np.finfo(float).eps * max(result.jac.shape) * s[0]
     s = s[s > threshold]
     vt = vt[: s.size]
-    p["p_var"] = np.diag(np.dot(vt.T / s**2, vt))[:n_p]
-    p["mu_var"] = np.diag(np.dot(vt.T / s**2, vt))[n_p:]
-    p["resnorm"] = 2 * result.cost
-    p["delta"] = x - p["mu_opt"]
-    p["epsilon"] = y - irfft(rfft(p["mu_opt"]) * function(p["p_opt"], w), n=n)
-    p["success"] = result.success
-    return p
+
+    p_opt = result.x[:n_p]
+    p_var = np.diag(np.dot(vt.T / s**2, vt))[n_p:]
+    delta = result.x[n_p:]
+    mu_opt = xdata - delta
+    mu_var = np.diag(np.dot(vt.T / s**2, vt))[n_p:]
+    resnorm = 2 * result.cost
+    psi_opt = transfer(lambda _w: function(p_opt, _w), mu_opt, dt=dt)
+    epsilon = ydata - psi_opt
+
+    v_y = np.diag(sigma_y**2)
+    h_sigma_x = transfer(lambda _w: function(p_opt, _w), sigma_x, dt=dt)
+    u_x = h_sigma_x[:, np.newaxis] @ h_sigma_x[np.newaxis, :]
+    h_delta = transfer(lambda _w: function(p_opt, _w), delta, dt=dt)
+    r_tls = sqrtm(np.linalg.inv(v_y + u_x)) @ (epsilon - h_delta)
+
+    res = FitResult(
+        p_opt=p_opt,
+        p_var=p_var,
+        mu_opt=mu_opt,
+        mu_var=mu_var,
+        resnorm=resnorm,
+        delta=delta,
+        epsilon=epsilon,
+        r_tls=r_tls,
+        success=result.success,
+    )
+    return res
```

### Comparing `thztools-0.4.0/.gitignore` & `thztools-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/LICENSE` & `thztools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.4.0/README.md` & `thztools-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 electromagnetic waveforms that are acquired as a function of *time*, which users typically
 represent as a function of *frequency* for analysis. THzTools makes it easier for researchers
 to use statistically optimal methods for doing this analysis, as described in [L. Mohtashemi et al.,
  Opt. Express **29**, 4912 (2021)](https://doi.org/10.1364/OE.417724).
 
 This is *alpha* software that is currently under development.
 
-| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|:------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools)          |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+|:------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![PyPI - Version](https://img.shields.io/pypi/v/thztools) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/thztools/badges/version.svg)](https://anaconda.org/conda-forge/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools)                                                                                                                                                                                                        |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 
 The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

### Comparing `thztools-0.4.0/pyproject.toml` & `thztools-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -51,18 +51,21 @@
 
 [tool.hatch.version]
 path = "src/thztools/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
     "coverage[toml]>=6.5",
+    "grayskull",
     "jupyter",
     "matplotlib",
     "numdifftools",
     "pytest",
+    "pytest-cov",
+    "scipy-doctest",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
     "- coverage combine",
     "coverage report",
@@ -199,19 +202,20 @@
     "matplotlib",
     "nbsphinx",
     "numpydoc",
     "pydata-sphinx-theme",
     "sphinx",
     "sphinx-design",
     "sphinx-gallery",
+    "sphinx-tabs",
     "tomli",
 ]
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -v -b html docs/source docs/build/html"
-test = "sphinx-build -v -b doctest docs/source docs/doctest"
+test = "pytest -v src/thztools --doctest-modules"
 
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
 
 [[tool.mypy.overrides]]
 module = [
     "pytest",
```

### Comparing `thztools-0.4.0/PKG-INFO` & `thztools-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: thztools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Data analysis software tools for terahertz time-domain spectroscopy (THz-TDS)
 Project-URL: Documentation, https://dodge-research-group.github.io/thztools/
 Project-URL: Issues, https://github.com/dodge-research-group/thztools/issues
 Project-URL: Discussion, https://github.com/dodge-research-group/thztools/discussions
 Project-URL: Source, https://github.com/dodge-research-group/thztools
 Author-email: Jonathan Posada Loaiza <jonathan.posada1@udea.edu.co>, Santiago Higuera-Quintero <s.higuera@uniandes.edu.co>, Alireza Noori <alireza_noori@sfu.ca>, Laleh Mohtashemi <lalehmo@gmail.com>, "R. P. Hall" <rph4@sfu.ca>, Naod Ayalew Yimam <nayimam@gmail.com>, "J. Steven Dodge" <jsdodge@sfu.ca>
 Maintainer-email: Steve Dodge <jsdodge@sfu.ca>
@@ -41,15 +41,15 @@
 electromagnetic waveforms that are acquired as a function of *time*, which users typically
 represent as a function of *frequency* for analysis. THzTools makes it easier for researchers
 to use statistically optimal methods for doing this analysis, as described in [L. Mohtashemi et al.,
  Opt. Express **29**, 4912 (2021)](https://doi.org/10.1364/OE.417724).
 
 This is *alpha* software that is currently under development.
 
-| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-|:------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools)          |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+|:------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | [![DOI](https://zenodo.org/badge/569133241.svg)](https://zenodo.org/doi/10.5281/zenodo.10100093) ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![PyPI - Version](https://img.shields.io/pypi/v/thztools) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/thztools/badges/version.svg)](https://anaconda.org/conda-forge/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools)                                                                                                                                                                                                        |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 
 The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

