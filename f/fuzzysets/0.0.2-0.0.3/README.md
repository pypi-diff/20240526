# Comparing `tmp/fuzzysets-0.0.2.tar.gz` & `tmp/fuzzysets-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\repositories\fuzzysets\dist\tmpe0ieh3hm\fuzzysets-0.0.2.tar", last modified: Fri Feb 19 10:43:33 2021, max compression
+gzip compressed data, was "C:\Stiliyan\repositories\fuzzy-sets\dist\tmphwktn03w\fuzzysets-0.0.3.tar", last modified: Sun May 26 09:41:48 2024, max compression
```

## Comparing `fuzzysets-0.0.2.tar` & `fuzzysets-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/
-drwxrwxrwx   0        0        0        0 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets/
--rw-rw-rw-   0        0        0     9211 2021-02-18 20:06:46.000000 fuzzysets-0.0.2/fuzzysets/plot.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets/sets/
--rw-rw-rw-   0        0        0    11196 2021-02-15 17:09:52.000000 fuzzysets-0.0.2/fuzzysets/sets/base.py
--rw-rw-rw-   0        0        0     4295 2021-02-15 17:12:09.000000 fuzzysets-0.0.2/fuzzysets/sets/continuous.py
--rw-rw-rw-   0        0        0     1901 2021-02-15 15:27:34.000000 fuzzysets-0.0.2/fuzzysets/sets/finite.py
--rw-rw-rw-   0        0        0        0 2021-02-14 10:03:11.000000 fuzzysets-0.0.2/fuzzysets/sets/__init__.py
--rw-rw-rw-   0        0        0     8765 2021-02-14 17:28:50.000000 fuzzysets-0.0.2/fuzzysets/tfn.py
--rw-rw-rw-   0        0        0      776 2021-02-15 15:23:38.000000 fuzzysets-0.0.2/fuzzysets/utils.py
--rw-rw-rw-   0        0        0      452 2021-02-18 20:08:08.000000 fuzzysets-0.0.2/fuzzysets/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets.egg-info/
--rw-rw-rw-   0        0        0        1 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    18646 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets.egg-info/requires.txt
--rw-rw-rw-   0        0        0      378 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/fuzzysets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18646 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      110 2021-02-18 20:37:40.000000 fuzzysets-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0    15115 2021-02-18 21:39:24.000000 fuzzysets-0.0.2/README.md
--rw-rw-rw-   0        0        0      661 2021-02-19 10:43:33.000000 fuzzysets-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets/
+-rw-rw-rw-   0        0        0     9505 2024-05-24 11:23:43.000000 fuzzysets-0.0.3/fuzzysets/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets/sets/
+-rw-rw-rw-   0        0        0    12852 2024-05-25 09:54:01.000000 fuzzysets-0.0.3/fuzzysets/sets/base.py
+-rw-rw-rw-   0        0        0     4901 2024-05-25 09:54:48.000000 fuzzysets-0.0.3/fuzzysets/sets/continuous.py
+-rw-rw-rw-   0        0        0     2272 2024-05-25 09:44:38.000000 fuzzysets-0.0.3/fuzzysets/sets/finite.py
+-rw-rw-rw-   0        0        0        0 2022-09-22 11:31:55.000000 fuzzysets-0.0.3/fuzzysets/sets/__init__.py
+-rw-rw-rw-   0        0        0    10205 2024-05-24 10:52:26.000000 fuzzysets-0.0.3/fuzzysets/tfn.py
+-rw-rw-rw-   0        0        0      977 2024-05-24 10:52:26.000000 fuzzysets-0.0.3/fuzzysets/utils.py
+-rw-rw-rw-   0        0        0      452 2022-09-22 11:31:55.000000 fuzzysets-0.0.3/fuzzysets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    15666 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      582 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/fuzzysets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2024-05-24 10:52:26.000000 fuzzysets-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    15666 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      110 2024-05-26 09:38:29.000000 fuzzysets-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0    15036 2024-05-26 09:17:50.000000 fuzzysets-0.0.3/README.md
+-rw-rw-rw-   0        0        0      810 2024-05-26 09:41:48.000000 fuzzysets-0.0.3/setup.cfg
```

### Comparing `fuzzysets-0.0.2/fuzzysets/plot.py` & `fuzzysets-0.0.3/fuzzysets/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,38 @@
+from typing import (
+    Callable,
+    Tuple,
+    TypeVar,
+)
+
 import matplotlib.pyplot as plt
 import numpy as np
 
 from fuzzysets import utils
 from fuzzysets.sets.base import FuzzySet
 from fuzzysets.sets.continuous import ContinuousFuzzySet
 from fuzzysets.sets.finite import FiniteFuzzySet
 from fuzzysets.tfn import TriangularFuzzyNumber as TFN
 
 
+FuzzySetT = TypeVar("FuzzySetT", bound=FuzzySet)
+
+
+NormFunction = Callable[[float, float], float]
+
+
 _X_LIMITS = (0., 10.)
 
 
 _Y_LABEL = "μ(x)"
 
 
-def plot_tfn_operations(first_name="A",
-                        second_name="B",
-                        x_lim=_X_LIMITS):
+def plot_tfn_operations(first_name: str = "A",
+                        second_name: str = "B",
+                        x_lim: Tuple[float, float] = _X_LIMITS) -> None:
     """
     Reads two TFNs as input and plots the results of their addition,
     subtraction, multiplication and division.
 
     :param first_name: a str - the name for the first TFN. Defaults to
     'A'.
     :param second_name: a str - the name for the second TFN. Defaults
@@ -152,30 +164,32 @@
     axes.set_xlim(*x_lim)
     axes.set_ylim(0., 1.)
     axes.set_title(title)
     axes.set_xlabel(x_label)
     axes.set_ylabel(y_label)
 
 
-def plot_tfn(tfn, name="A"):
+def plot_tfn(tfn: TFN, name: str = "A") -> None:
     """
     :param tfn: an instance of TriangularFuzzyNumber.
     :param name: a str - the name of the TFN. Defaults to 'A'.
     """
     _, axes = plt.subplots()
     _set_up_and_plot_on(axes, tfn, name)
 
 
-def plot_fuzzy_set_operations(a,
-                              b,
-                              a_name="A",
-                              b_name="B",
-                              t_norm=min,
-                              s_norm=max,
-                              comp=utils.complement):
+def plot_fuzzy_set_operations(
+    a: FuzzySetT,
+    b: FuzzySetT,
+    a_name: str = "A",
+    b_name: str = "B",
+    t_norm: NormFunction = min,
+    s_norm: NormFunction = max,
+    comp: Callable[[float], float] = utils.complement
+) -> None:
     """
     Plots the complements, t-norm and s-norm of two fuzzy sets of the
     same type.
 
     :param a: a FuzzySet.
     :param b: a FuzzySet whose type is the same as `a`'s.
     :param a_name: a str - the name of the first set. Defaults to 'A'.
@@ -265,15 +279,18 @@
              xs,
              np.array(list(norm.range)),
              label=norm_set_name,
              add_legend=True,
              connect=connect)
 
 
-def plot_fuzzy_set(s, title="", x_label="x", y_label=_Y_LABEL):
+def plot_fuzzy_set(s: FuzzySet,
+                   title: str = "",
+                   x_label: str = "x",
+                   y_label: str = _Y_LABEL) -> None:
     """
     :param s: an instance of FuzzySet.
     :param title: an optional str - the title of the plot.
     :param x_label: a str - the label for the x axis of the plot.
     Defaults to 'x'.
     :param y_label: a str - the label for the y axis of the plot.
     Defaults to Y_LABEL.
```

### Comparing `fuzzysets-0.0.2/fuzzysets/sets/base.py` & `fuzzysets-0.0.3/fuzzysets/sets/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,176 +1,202 @@
 import abc
 import operator
+from typing import (
+    Any,
+    Callable,
+    FrozenSet,
+    Iterable,
+    Iterator,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+)
+
+import numpy as np
 
 from fuzzysets import utils
 
 
+T = TypeVar("T")
+
+FuzzySetT = TypeVar("FuzzySetT", bound="FuzzySet")
+
+NormFunction = Callable[[float, float], float]
+
+
 class Domain(abc.ABC):
     """
     An abstract class for domain of a fuzzy set.
     """
     @abc.abstractmethod
-    def __iter__(self):
+    def __iter__(self) -> Iterator[T]:
         """
         :returns: a generator which yields the elements of the domain.
         The order of the elements is the same in each call.
         """
         pass
 
     @abc.abstractmethod
-    def __contains__(self, item):
+    def __contains__(self, item: Any) -> bool:
         pass
 
     @abc.abstractmethod
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         pass
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         return not self == other
 
 
 class FuzzySet(abc.ABC):
     """
     An abstract class for fuzzy set.
     """
-    def __init__(self, domain, degrees):
+    def __init__(self, domain: Domain, degrees: np.ndarray) -> None:
         """
         :param domain: an instance of type Domain.
         :param degrees: a NumPy array of floats in the range [0, 1] -
         the corresponding membership degrees.
 
         :raises ValueError: if the degrees are invalid.
         """
         self.__set_degrees(degrees)
         self.__domain = domain
         self.__core = None
         self.__support = None
         self.__cross_over_points = None
 
-    def __set_degrees(self, degrees):
+    def __set_degrees(self, degrees: np.ndarray) -> None:
         if (utils.is_membership_degree_v(degrees).all()):
             self.__degrees = degrees
         else:
             raise ValueError("Membership degrees must be "
                              "floats between 0 and 1!")
 
-    def _degree_at(self, i):
+    def _degree_at(self, i: int) -> float:
         return self.__degrees[i]
 
     @abc.abstractmethod
-    def mu(self, x):
+    def mu(self, x: Any) -> float:
         """
         :param x: an element of the domain.
         :returns: the membership degree of `x`, if it is within the
         domain, otherwise 0.
         """
         pass
 
     @property
-    def domain(self):
+    def domain(self) -> Domain:
         """
         :returns: an instance of type Domain - the set's domain.
         """
         return self.__domain
 
     @property
-    def range(self):
+    def range(self) -> Iterator[float]:
         """
         :returns: a generator of floats in the range [0, 1] - the set's
         range.
         """
         return (i for i in self.__degrees)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Tuple[T, float]]:
         """
-        :returns: an generator of pairs (x, d), where x is an element
+        :returns: a generator of pairs (x, d), where x is an element
         of the domain and d is its membership degree.
         """
         return zip(self.domain, self.range)
 
     @property
-    def core(self):
+    def core(self) -> FrozenSet[T]:
         """
         :returns: an immutable set of all the elements whose membership
         degree is 1.
         """
         if (self.__core is None):
             self.__core = frozenset(x for x, d in self if (d == 1.))
 
         return self.__core
 
     @property
-    def support(self):
+    def support(self) -> FrozenSet[T]:
         """
         :returns: an immutable set of all the elements whose membership
         degree is positive.
         """
         if (self.__support is None):
             self.__support = frozenset(x for x, d in self if (d > 0.))
 
         return self.__support
 
     @property
-    def cross_over_points(self):
+    def cross_over_points(self) -> FrozenSet[T]:
         """
         :returns: an immutable set of all the elements whose membership
         degree is 0.5.
         """
         if (self.__cross_over_points is None):
             self.__cross_over_points = frozenset(
                 x for x, d in self if (d == 0.5)
             )
 
         return self.__cross_over_points
 
-    def alpha_cut(self, alpha):
+    def alpha_cut(self, alpha: float) -> Set[T]:
         """
         :param alpha: a float between 0 and 1.
         :returns: a set of the elements whose membership degree is
         greater or equal to `alpha`.
         """
         alpha = utils.to_float_if_int(alpha)
         utils.validate_alpha(alpha)
 
         return {x for x, d in self if (d >= alpha)}
 
     @property
-    def height(self):
+    def height(self) -> float:
         """
         :returns: the highest membership degree in the set, 0.0 if it is
         empty.
         """
         return self.__degrees.max(initial=0.0)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """
         :param other: a value.
         :returns: a boolean value indicating whether `other` is a fuzzy
         set of the same type which has the same domain and membership
         degrees.
         """
         return (isinstance(other, self.__class__) and
                 self.__pointwise_comparison(other, operator.eq))
 
-    def __pointwise_comparison(self, other, p, reduction=all):
+    def __pointwise_comparison(
+        self: FuzzySetT,
+        other: FuzzySetT,
+        p: Callable[[float, float], bool],
+        reduction: Callable[[Iterable[bool]], bool] = all
+    ) -> bool:
         return (self.domain == other.domain and
                 reduction(p(self.mu(x), other.mu(x))
                           for x in self._select_between_domains(other)))
 
-    def _select_between_domains(self, other):
+    def _select_between_domains(self: FuzzySetT,
+                                other: FuzzySetT) -> Domain:
         """
         This method is invoked whenever two FS's have equal domains and
         one of them is needed, in case it matters which one it is.
         """
         return self.domain
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         return not self == other
 
-    def __lt__(self, other):
+    def __lt__(self: FuzzySetT, other: FuzzySetT) -> bool:
         """
         Checks whether the fuzzy set is a proper subset of `other`.
 
         :param other: an instance of the same FuzzySet subclass.
         :returns: a boolean value indicating whether `other` has the
         same domain and its membership degrees are greater or equal
         to the fuzzy set's membership degrees, with at least one of them
@@ -180,76 +206,85 @@
         class.
         """
         self.__class__.__verify_has_same_class(other)
         return (self.__pointwise_comparison(other, operator.le) and
                 self.__pointwise_comparison(other, operator.lt, any))
 
     @classmethod
-    def __verify_has_same_class(cls, other):
+    def __verify_has_same_class(cls, other: Any) -> None:
         if (not isinstance(other, cls)):
             raise TypeError(
                 f"Expected an instance of {cls.__name__!r}!"
             )
 
-    def __gt__(self, other):
+    def __gt__(self: FuzzySetT, other: FuzzySetT) -> bool:
         """
         Checks whether the fuzzy set is a proper superset of `other`.
 
         :raises TypeError: if `other` is not an instance of the same
         class.
         """
         self.__class__.__verify_has_same_class(other)
         return other < self
 
-    def __le__(self, other):
+    def __le__(self: FuzzySetT, other: FuzzySetT) -> bool:
         """
         Checks whether the fuzzy set is a subset of `other`.
 
         :raises TypeError: if `other` is not an instance of the same
         class.
         """
         self.__class__.__verify_has_same_class(other)
         return self.__pointwise_comparison(other, operator.le)
 
-    def __ge__(self, other):
+    def __ge__(self: FuzzySetT, other: FuzzySetT) -> bool:
         """
         Checks whether the fuzzy set is a superset of `other`.
 
         :raises TypeError: if `other` is not an instance of the same
         class.
         """
         self.__class__.__verify_has_same_class(other)
         return other <= self
 
-    def __norm(self, other, norm):
+    def __norm(self: FuzzySetT,
+               other: FuzzySetT,
+               norm: NormFunction) -> FuzzySetT:
         self.__verify_has_same_class_and_domain(other)
 
         return self.__class__._from_domain(
             self._select_between_domains(other),
             mu=lambda x: norm(self.mu(x), other.mu(x))
         )
 
-    def __verify_has_same_class_and_domain(self, other):
+    def __verify_has_same_class_and_domain(
+        self: FuzzySetT,
+        other: FuzzySetT
+    ) -> None:
         self.__class__.__verify_has_same_class(other)
 
         if (self.domain != other.domain):
             raise ValueError(f"Domains differ: {self.domain} "
                              f"!= {other.domain}")
 
     @classmethod
     @abc.abstractmethod
-    def _from_domain(cls, domain, mu):
+    def _from_domain(cls: Type[FuzzySetT],
+                     domain: Domain,
+                     mu: Callable[[T], float]) -> FuzzySetT:
         """
         :param domain: an instance of Domain.
         :param mu: a callable that takes elements of `domain` and
         returns floats in the range [0, 1] (not assumed).
         """
         pass
 
-    def t_norm(self, other, norm=min):
+    def t_norm(self: FuzzySetT,
+               other: FuzzySetT,
+               norm: NormFunction = min) -> FuzzySetT:
         """
         Finds the t-norm of the fuzzy set and `other`.
 
         :param other: an instance of the same FuzzySet class.
         :param norm: a callable that takes two membership degrees
         (floats between 0 and 1) and returns a membership degree. This
         callable (denoted by I below) must also satisfy the following
@@ -268,15 +303,17 @@
         :raises TypeError: if `other` is not an instance of the same
         class.
         :raises ValueError: if the supplied callable does not return
         membership degrees.
         """
         return self.__norm(other, norm)
 
-    def s_norm(self, other, norm=max):
+    def s_norm(self: FuzzySetT,
+               other: FuzzySetT,
+               norm: NormFunction = max) -> FuzzySetT:
         """
         Finds the s-norm of the fuzzy set and `other`.
 
         :param other: an instance of the same FuzzySet class.
         :param norm: a callable that takes two membership degrees
         (floats between 0 and 1) and returns a membership degree. This
         callable (denoted by U below) must also satisfy the following
@@ -295,15 +332,18 @@
         :raises TypeError: if `other` is not an instance of the same
         class.
         :raises ValueError: if the supplied callable does not return
         membership degrees.
         """
         return self.__norm(other, norm)
 
-    def complement(self, comp=utils.complement):
+    def complement(
+        self: FuzzySetT,
+        comp: Callable[[float], float] = utils.complement
+    ) -> FuzzySetT:
         """
         Finds the complement of the fuzzy set.
 
         :param comp: a callable that takes a membership degree (float
         between 0 and 1) and returns a membership degree. This callable
         (denoted by C below) must also satisfy the following axioms:
          1) boundary condition:
@@ -316,46 +356,53 @@
         membership degrees.
         """
         return self.__class__._from_domain(
             self.domain,
             mu=lambda x: comp(self.mu(x))
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.domain})"
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         :returns: a str in the format:
         <x 0>/<d 0> + ... + <x n>/<d n>
         where <x i> and <d i> are the elements of the set and their
         membership degrees, respectively.
         """
         return " + ".join(f"{x}/{d:.2f}" for x, d in self)
 
 
-def t_norm(a, b, norm=min):
+def t_norm(a: FuzzySetT,
+           b: FuzzySetT,
+           norm: NormFunction = min) -> FuzzySetT:
     """
     Equivalent to `a.t_norm(b, norm)`.
     """
     return a.t_norm(b, norm)
 
 
-def s_norm(a, b, norm=max):
+def s_norm(a: FuzzySetT,
+           b: FuzzySetT,
+           norm: NormFunction = max) -> FuzzySetT:
     """
     Equivalent to `a.s_norm(b, norm)`.
     """
     return a.s_norm(b, norm)
 
 
-def complement(a, comp=utils.complement):
+def complement(
+    a: FuzzySetT,
+    comp: Callable[[float], float] = utils.complement
+) -> FuzzySetT:
     """
     Equivalent to `a.complement(comp)`.
     """
     return a.complement(comp)
 
 
-def alpha_cut(a, alpha):
+def alpha_cut(a: FuzzySet, alpha: float) -> Set[T]:
     """
     Equivalent to `a.alpha_cut(alpha)`.
     """
     return a.alpha_cut(alpha)
```

### Comparing `fuzzysets-0.0.2/fuzzysets/sets/continuous.py` & `fuzzysets-0.0.3/fuzzysets/sets/continuous.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+from typing import (
+    Any,
+    Callable,
+    Iterator,
+    Type,
+)
+
 import numpy as np
 
 from fuzzysets import utils
 from fuzzysets.sets import base
 
 
 _STEP = 0.1
 
 
 class ContinuousDomain(base.Domain):
     """
     Represents the domain of a continuous fuzzy set - a range of real
     numbers: [start, end].
     """
-    def __init__(self, start, end, step=_STEP):
+    def __init__(self,
+                 start: float,
+                 end: float,
+                 step: float = _STEP) -> None:
         """
         :param start: a float - the range start.
         :param end: a float - the range end.
         :param step: a float - the step to use when iterating the range,
         for example when the domain object is being iterated. Defaults
         to `STEP`.
 
@@ -33,60 +43,66 @@
             step > 0.):
             self.__start = start
             self.__end = end
             self.__step = step
         else:
             raise ValueError("Invalid range!")
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[float]:
         current = self.__start
 
         while current <= self.__end:
             yield current
             current += self.__step
 
-    def __contains__(self, item):
+    def __contains__(self, item: Any) -> bool:
         item = utils.to_float_if_int(item)
 
         return (isinstance(item, float) and
                 self.__start <= item <= self.__end)
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) ->  bool:
         return (isinstance(other, self.__class__) and
                 self.__start == other.__start and
                 self.__end == other.__end)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (f"{self.__class__.__name__}("
                 f"start={self.__start}, "
                 f"end={self.__end}, "
                 f"step={self.__step})")
 
     @property
-    def start(self):
+    def start(self) -> float:
         return self.__start
 
     @property
-    def end(self):
+    def end(self) -> float:
         return self.__end
 
     @property
-    def step(self):
+    def step(self) -> float:
         return self.__step
 
 
 class ContinuousFuzzySet(base.FuzzySet):
     """
     Represents a fuzzy set whose domain is an interval of real numbers.
     """
     @classmethod
-    def _from_domain(cls, domain, mu):
+    def _from_domain(
+        cls: Type[base.FuzzySetT],
+        domain: ContinuousDomain,
+        mu: Callable[[float], float]
+    ) -> base.FuzzySetT:
         return cls(domain, mu)
 
-    def __init__(self, domain, mu):
+    def __init__(self,
+                 domain: ContinuousDomain,
+                 mu: Callable[[float], float]) -> None:
         """
         :param domain: an instance of ContinuousDomain.
         :param mu: a callable that takes elements of `domain` and
         returns floats in the range [0, 1] - the membership function
         of the set.
 
         :raises ValueError: if the degrees returned by `mu` are invalid.
@@ -96,51 +112,54 @@
         index = np.array(list(domain))
         degrees = mu(index)
         super().__init__(domain, degrees)
         self.__index = index
         self.__mu = mu
 
     @staticmethod
-    def __validate_domain(d):
+    def __validate_domain(d: Any) -> None:
         if (not isinstance(d, ContinuousDomain)):
             raise ValueError("Invalid domain!")
 
-    def mu(self, x):
+    def mu(self, x: float) -> float:
         """
         :param x: a float - an element of the domain.
         :returns: the membership degree of `x`, if it is within the
         domain, otherwise 0.
         """
         x = utils.to_float_if_int(x)
 
         return (
             self.__mu_for(x)
             if (isinstance(x, float) and
                 self.__index[0] <= x <= self.__index[-1])
             else 0.
         )
 
-    def __mu_for(self, x):
+    def __mu_for(self, x: float) -> float:
         i = self.__index_for(x)
 
         return (self._degree_at(i)
                 if (self.__index[i] == x)
                 else self.__calculate_mu(x, i))
 
-    def __index_for(self, x):
+    def __index_for(self, x: float) -> int:
         assert self.__index[0] <= x <= self.__index[-1]
         return np.searchsorted(self.__index, x, side="left")
 
-    def __calculate_mu(self, x, i):
+    def __calculate_mu(self, x: float, i: int) -> float:
         try:
             return self.__mu(x).item()
         except Exception:
             return (self._degree_at(i - 1) + self._degree_at(i)) / 2.
 
-    def _select_between_domains(self, other):
+    def _select_between_domains(
+        self: base.FuzzySetT,
+        other: base.FuzzySetT
+    ) -> ContinuousDomain:
         """
         This method is invoked whenever two FS's have equal domains and
         one of them is needed, in case it matters which one it is.
         """
         return (self.domain
                 if (self.domain.step < other.domain.step)
                 else other.domain)
```

### Comparing `fuzzysets-0.0.2/fuzzysets/sets/finite.py` & `fuzzysets-0.0.3/fuzzysets/sets/finite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,64 @@
+from typing import (
+    Any,
+    Callable,
+    Iterable,
+    Iterator,
+    Mapping,
+    Type,
+    TypeVar,
+)
+
 import numpy as np
 
 from fuzzysets.sets import base
 
 
+T = TypeVar("T")
+
+
 class FiniteDomain(base.Domain):
     """
     Represents the domain of a finite fuzzy set.
     """
-    def __init__(self, items):
+    def __init__(self, items: Iterable[T]) -> None:
         """
         :param items: an iterable of hashable items.
         """
         self.__items = set(items)
         self.__sequenced_items = list(self.__items)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[T]:
         return iter(self.__sequenced_items)
 
-    def __contains__(self, item):
+    def __contains__(self, item: Any) -> bool:
         return item in self.__items
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         return (isinstance(other, self.__class__) and
                 self.__items == other.__items)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.__items})"
 
 
 class FiniteFuzzySet(base.FuzzySet):
     """
     Represents a fuzzy set with a finite domain.
     """
     @classmethod
-    def _from_domain(cls, domain, mu):
+    def _from_domain(cls: Type[base.FuzzySetT],
+                     domain: FiniteDomain,
+                     mu: Callable[[T], float]) -> base.FuzzySetT:
         return cls({
             x: mu(x)
             for x in domain
         })
 
-    def __init__(self, elements):
+    def __init__(self, elements: Mapping[T, float]) -> None:
         """
         :param elements: an instance of abc.Mapping (like dict) whose
         keys are the set's elements and whose values are their
         corresponding membership degrees (floats between 0 and 1).
 
         :raises ValueError: if the degrees are invalid.
         """
@@ -52,15 +67,15 @@
         super().__init__(domain, degrees)
 
         self.__indexes = {
             x: i
             for i, x in enumerate(domain)
         }
 
-    def mu(self, x):
+    def mu(self, x: T) -> float:
         """
         :param x: an element of the domain.
         :returns: the membership degree of `x`, if it is within the
         domain, otherwise 0.
         """
         index = self.__indexes.get(x)
```

