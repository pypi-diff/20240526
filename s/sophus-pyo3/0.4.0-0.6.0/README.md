# Comparing `tmp/sophus_pyo3-0.4.0.tar.gz` & `tmp/sophus_pyo3-0.6.0.tar.gz`

## Comparing `sophus_pyo3-0.4.0.tar` & `sophus_pyo3-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,54 @@
--rw-r--r--   0     1001      127      462 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/Cargo.toml
--rw-r--r--   0     1001      127    18633 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/dual/dual_matrix.rs
--rw-r--r--   0     1001      127    15009 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/dual/dual_scalar.rs
--rw-r--r--   0     1001      127    12885 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/dual/dual_vector.rs
--rw-r--r--   0     1001      127      117 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/dual.rs
--rw-r--r--   0     1001      127      369 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/lib.rs
--rw-r--r--   0     1001      127     2390 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/manifold/traits.rs
--rw-r--r--   0     1001      127       35 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/manifold.rs
--rw-r--r--   0     1001      127     5015 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/maps/curves.rs
--rw-r--r--   0     1001      127     7163 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/maps/matrix_valued_maps.rs
--rw-r--r--   0     1001      127     5335 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/maps/scalar_valued_maps.rs
--rw-r--r--   0     1001      127     7624 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/maps/vector_valued_maps.rs
--rw-r--r--   0     1001      127      390 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/maps.rs
--rw-r--r--   0     1001      127      990 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/points.rs
--rw-r--r--   0     1001      127     8577 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/region.rs
--rw-r--r--   0     1001      127    11810 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/spline/spline_segment.rs
--rw-r--r--   0     1001      127     8205 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/spline.rs
--rw-r--r--   0     1001      127     4998 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/types/matrix.rs
--rw-r--r--   0     1001      127      884 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/types/params.rs
--rw-r--r--   0     1001      127     2565 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/types/scalar.rs
--rw-r--r--   0     1001      127     3403 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/types/vector.rs
--rw-r--r--   0     1001      127      737 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_calculus/src/types.rs
--rw-r--r--   0     1001      127       56 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/README.md
--rw-r--r--   0     1001      127      439 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/Cargo.toml
--rw-r--r--   0     1001      127     1308 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/isometry2.rs
--rw-r--r--   0     1001      127     1599 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/isometry3.rs
--rw-r--r--   0     1001      127      321 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/lib.rs
--rw-r--r--   0     1001      127    32412 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/lie_group.rs
--rw-r--r--   0     1001      127       35 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/pyo3.rs
--rw-r--r--   0     1001      127     9791 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/rotation2.rs
--rw-r--r--   0     1001      127    20009 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/rotation3.rs
--rw-r--r--   0     1001      127     8866 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/traits.rs
--rw-r--r--   0     1001      127    16452 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_lie/src/translation_product_product.rs
--rw-r--r--   0     1001      127      485 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/Cargo.toml
--rw-r--r--   0     1001      127    21976 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/arc_tensor.rs
--rw-r--r--   0     1001      127     8843 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/element.rs
--rw-r--r--   0     1001      127     8147 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/layout.rs
--rw-r--r--   0     1001      127      228 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/lib.rs
--rw-r--r--   0     1001      127    20440 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/mut_tensor.rs
--rw-r--r--   0     1001      127     9679 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/mut_view.rs
--rw-r--r--   0     1001      127    17854 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_tensor/src/view.rs
--rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 sophus_pyo3-0.4.0/crates/sophus_pyo3/Cargo.toml
--rw-r--r--   0     1001      127      596 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_pyo3/src/lib.rs
--rw-r--r--   0     1001      127     6563 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_pyo3/src/pyo3/lie_groups.rs
--rw-r--r--   0     1001      127       35 2024-03-24 06:37:44.000000 sophus_pyo3-0.4.0/crates/sophus_pyo3/src/pyo3.rs
--rw-r--r--   0     1001      127   118398 2024-03-24 06:37:50.000000 sophus_pyo3-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 sophus_pyo3-0.4.0/Cargo.toml
--rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 sophus_pyo3-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 sophus_pyo3-0.4.0/PKG-INFO
+-rw-r--r--   0     1001      127      507 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/Cargo.toml
+-rw-r--r--   0     1001      127    48009 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_matrix.rs
+-rw-r--r--   0     1001      127    46150 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_scalar.rs
+-rw-r--r--   0     1001      127    36168 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual/dual_vector.rs
+-rw-r--r--   0     1001      127      485 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/dual.rs
+-rw-r--r--   0     1001      127       35 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/manifold.rs
+-rw-r--r--   0     1001      127     7425 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/curves.rs
+-rw-r--r--   0     1001      127    10602 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/matrix_valued_maps.rs
+-rw-r--r--   0     1001      127     7706 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/scalar_valued_maps.rs
+-rw-r--r--   0     1001      127    11249 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/vector_valued_maps.rs
+-rw-r--r--   0     1001      127     1035 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps.rs
+-rw-r--r--   0     1001      127    11449 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/region.rs
+-rw-r--r--   0     1001      127    12753 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline/spline_segment.rs
+-rw-r--r--   0     1001      127     8135 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline.rs
+-rw-r--r--   0     1001      127      531 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/calculus.rs
+-rw-r--r--   0     1001      127     1787 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/lib.rs
+-rw-r--r--   0     1001      127     1562 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/bool_mask.rs
+-rw-r--r--   0     1001      127    12433 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/matrix.rs
+-rw-r--r--   0     1001      127    16897 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/scalar.rs
+-rw-r--r--   0     1001      127     9619 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg/vector.rs
+-rw-r--r--   0     1001      127     3245 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/linalg.rs
+-rw-r--r--   0     1001      127     1532 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/manifold/traits.rs
+-rw-r--r--   0     1001      127       30 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/manifold.rs
+-rw-r--r--   0     1001      127     1509 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/params.rs
+-rw-r--r--   0     1001      127     2871 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/points.rs
+-rw-r--r--   0     1001      127    15058 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/arc_tensor.rs
+-rw-r--r--   0     1001      127     4747 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/element.rs
+-rw-r--r--   0     1001      127    18816 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor.rs
+-rw-r--r--   0     1001      127     9210 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor_view.rs
+-rw-r--r--   0     1001      127    14599 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/tensor_view.rs
+-rw-r--r--   0     1001      127      441 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_core/src/tensor.rs
+-rw-r--r--   0     1001      127      329 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/README.md
+-rw-r--r--   0     1001      127      432 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/Cargo.toml
+-rw-r--r--   0     1001      127     6405 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/factor_lie_group.rs
+-rw-r--r--   0     1001      127     1636 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry2.rs
+-rw-r--r--   0     1001      127     1619 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry3.rs
+-rw-r--r--   0     1001      127    11299 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/rotation2.rs
+-rw-r--r--   0     1001      127    22900 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/rotation3.rs
+-rw-r--r--   0     1001      127    16984 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/translation_product_product.rs
+-rw-r--r--   0     1001      127      202 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/groups.rs
+-rw-r--r--   0     1001      127      780 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/lib.rs
+-rw-r--r--   0     1001      127    11209 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/lie_group.rs
+-rw-r--r--   0     1001      127     2970 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/lie_group_manifold.rs
+-rw-r--r--   0     1001      127    22904 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/real_lie_group.rs
+-rw-r--r--   0     1001      127     9193 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_lie/src/traits.rs
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      693 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1249 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3/errors.rs
+-rw-r--r--   0     1001      127    15284 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3/lie_groups.rs
+-rw-r--r--   0     1001      127       70 2024-05-26 00:38:39.000000 sophus_pyo3-0.6.0/crates/sophus_pyo3/src/pyo3.rs
+-rw-r--r--   0     1001      127   123832 2024-05-26 00:38:59.000000 sophus_pyo3-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/Cargo.toml
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 sophus_pyo3-0.6.0/PKG-INFO
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_calculus/src/manifold/traits.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/manifold/traits.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-use crate::points::example_points;
-use crate::types::params::HasParams;
-use crate::types::params::ParamsImpl;
-use crate::types::scalar::IsScalar;
-use crate::types::VecF64;
+use crate::linalg::VecF64;
+use crate::params::ParamsImpl;
+use crate::prelude::*;
 
 /// A tangent implementation.
 pub trait TangentImpl<S: IsScalar<BATCH_SIZE>, const DOF: usize, const BATCH_SIZE: usize> {
     /// Examples of tangent vectors.
     fn tangent_examples() -> Vec<S::Vector<DOF>>;
 }
 
@@ -38,48 +36,20 @@
     fn params(&self) -> &S::Vector<PARAMS>;
     /// o-plus operation
     fn oplus(&self, tangent: &S::Vector<DOF>) -> Self;
     /// o-minus operation
     fn ominus(&self, rhs: &Self) -> S::Vector<DOF>;
 }
 
-impl<const N: usize> ParamsImpl<f64, N, 1> for VecF64<N> {
-    fn are_params_valid(_params: &<f64 as IsScalar<1>>::Vector<N>) -> bool {
-        true
-    }
-
-    fn params_examples() -> Vec<<f64 as IsScalar<1>>::Vector<N>> {
-        example_points::<f64, N>()
-    }
-
-    fn invalid_params_examples() -> Vec<<f64 as IsScalar<1>>::Vector<N>> {
-        vec![]
-    }
-}
-
-impl<const N: usize> HasParams<f64, N, 1> for VecF64<N> {
-    fn from_params(params: &<f64 as IsScalar<1>>::Vector<N>) -> Self {
-        *params
-    }
-
-    fn set_params(&mut self, params: &<f64 as IsScalar<1>>::Vector<N>) {
-        *self = *params
-    }
-
-    fn params(&self) -> &<f64 as IsScalar<1>>::Vector<N> {
-        self
-    }
-}
-
 impl<const N: usize> IsManifold<f64, N, N, 1> for VecF64<N> {
-    fn oplus(&self, tangent: &<f64 as IsScalar<1>>::Vector<N>) -> Self {
+    fn oplus(&self, tangent: &VecF64<N>) -> Self {
         self + tangent
     }
 
-    fn ominus(&self, rhs: &Self) -> <f64 as IsScalar<1>>::Vector<N> {
+    fn ominus(&self, rhs: &Self) -> VecF64<N> {
         self - rhs
     }
 
-    fn params(&self) -> &<f64 as IsScalar<1>>::Vector<N> {
+    fn params(&self) -> &VecF64<N> {
         self
     }
 }
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_calculus/src/maps/vector_valued_maps.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/maps/vector_valued_maps.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,315 @@
-use crate::dual::dual_matrix::DualM;
-use crate::dual::dual_vector::DualV;
-use crate::types::MatF64;
-use crate::types::VecF64;
-
-use sophus_tensor::mut_tensor::MutTensorDDR;
-use sophus_tensor::mut_tensor::MutTensorDR;
-use sophus_tensor::mut_view::IsMutTensorLike;
-use sophus_tensor::view::IsTensorLike;
-
+use crate::linalg::SVec;
+use crate::prelude::*;
+use crate::tensor::mut_tensor::MutTensorDDR;
+use crate::tensor::mut_tensor::MutTensorDR;
 use std::marker::PhantomData;
 
 /// Vector-valued map on a vector space.
 ///
 /// This is a function which takes a vector and returns a vector:
 ///
 ///  f: ℝᵐ -> ℝʳ
 ///
-/// These functions are also called vector fields (on vector space x s).
+/// These functions are also called vector fields (on vector space).
 ///
-pub struct VectorValuedMapFromVector;
+pub struct VectorValuedMapFromVector<S: IsScalar<BATCH>, const BATCH: usize> {
+    phantom: std::marker::PhantomData<S>,
+}
 
-impl VectorValuedMapFromVector {
+impl<S: IsRealScalar<BATCH, RealScalar = S>, const BATCH: usize>
+    VectorValuedMapFromVector<S, BATCH>
+{
     /// Finite difference quotient of the vector-valued map.
     ///
     /// The derivative is a matrix or rank-2 tensor with shape (Rₒ x Rᵢ).
     ///
     /// For efficiency reasons, we return the transpose Rᵢ x (Rₒ)
     ///
     pub fn sym_diff_quotient<TFn, const OUTROWS: usize, const INROWS: usize>(
         vector_valued: TFn,
-        a: VecF64<INROWS>,
+        a: S::RealVector<INROWS>,
         eps: f64,
-    ) -> MutTensorDR<f64, OUTROWS>
+    ) -> MutTensorDR<S, OUTROWS>
     where
-        TFn: Fn(VecF64<INROWS>) -> VecF64<OUTROWS>,
+        TFn: Fn(S::RealVector<INROWS>) -> SVec<S, OUTROWS>,
+        SVec<S, OUTROWS>: IsVector<S, OUTROWS, BATCH>,
     {
-        let mut out = MutTensorDR::<f64, OUTROWS>::from_shape([INROWS]);
+        let mut out = MutTensorDR::<S, OUTROWS>::from_shape([INROWS]);
+        let eps_v = S::RealScalar::from_f64(eps);
 
         for r in 0..INROWS {
             let mut a_plus = a;
-            a_plus[r] += eps;
+            a_plus[r] += eps_v;
 
             let mut a_minus = a;
-            a_minus[r] -= eps;
+            a_minus[r] -= eps_v;
+            let d = (vector_valued(a_plus) - vector_valued(a_minus))
+                .scaled(S::from_f64(1.0 / (2.0 * eps)));
 
-            out.get_mut([r])
-                .copy_from(&((vector_valued(a_plus) - vector_valued(a_minus)) / (2.0 * eps)));
+            out.get_mut([r]).copy_from(&d);
         }
         out
     }
 
-    /// Auto differentiation of the vector-valued map.
-    pub fn fw_autodiff<TFn, const OUTROWS: usize, const INROWS: usize>(
-        vector_valued: TFn,
-        a: VecF64<INROWS>,
-    ) -> MutTensorDR<f64, OUTROWS>
-    where
-        TFn: Fn(DualV<INROWS>) -> DualV<OUTROWS>,
-    {
-        let d = vector_valued(DualV::v(a)).dij_val;
-        if d.is_none() {
-            return MutTensorDR::from_shape([INROWS]);
-        }
-
-        MutTensorDR {
-            mut_array: d.unwrap().mut_array.into_shape([INROWS]).unwrap(),
-            phantom: PhantomData,
-        }
-    }
-
     /// Finite difference quotient of the vector-valued map.
     ///
     /// The derivative is a matrix or rank-2 tensor with shape (Rₒ x Rᵢ).
     ///
     pub fn static_sym_diff_quotient<TFn, const OUTROWS: usize, const INROWS: usize>(
         vector_valued: TFn,
-        a: VecF64<INROWS>,
+        a: S::RealVector<INROWS>,
         eps: f64,
-    ) -> MatF64<OUTROWS, INROWS>
+    ) -> S::RealMatrix<OUTROWS, INROWS>
     where
-        TFn: Fn(VecF64<INROWS>) -> VecF64<OUTROWS>,
+        TFn: Fn(S::RealVector<INROWS>) -> SVec<S, OUTROWS>,
+        SVec<S, OUTROWS>: IsVector<S, OUTROWS, BATCH>,
     {
         let jac = Self::sym_diff_quotient(vector_valued, a, eps);
-        let mut sjac = MatF64::<OUTROWS, INROWS>::zeros();
+        let mut sjac = S::RealMatrix::<OUTROWS, INROWS>::zeros();
 
         for r in 0..INROWS {
             let v = jac.get([r]);
-            sjac.fixed_view_mut::<OUTROWS, 1>(0, r).copy_from(&v);
+            for c in 0..OUTROWS {
+                sjac[(c, r)] = v[c];
+            }
         }
 
         sjac
+
+        // todo!()
+    }
+}
+
+impl<D: IsDualScalar<BATCH, DualScalar = D>, const BATCH: usize>
+    VectorValuedMapFromVector<D, BATCH>
+{
+    /// Auto differentiation of the vector-valued map.
+    pub fn fw_autodiff<TFn, const OUTROWS: usize, const INROWS: usize>(
+        vector_valued: TFn,
+        a: D::RealVector<INROWS>,
+    ) -> MutTensorDR<D::RealScalar, OUTROWS>
+    where
+        TFn: Fn(D::DualVector<INROWS>) -> D::DualVector<OUTROWS>,
+    {
+        let v = vector_valued(D::vector_with_dij(a));
+        let d = v.dij_val();
+        if d.is_none() {
+            return MutTensorDR::from_shape([INROWS]);
+        }
+
+        MutTensorDR {
+            mut_array: d.unwrap().mut_array.into_shape([INROWS]).unwrap(),
+            phantom: PhantomData,
+        }
     }
 
     /// Auto differentiation of the vector-valued map.
     pub fn static_fw_autodiff<TFn, const OUTROWS: usize, const INROWS: usize>(
         vector_valued: TFn,
-        a: VecF64<INROWS>,
-    ) -> MatF64<OUTROWS, INROWS>
+        a: D::RealVector<INROWS>,
+    ) -> D::RealMatrix<OUTROWS, INROWS>
     where
-        TFn: Fn(DualV<INROWS>) -> DualV<OUTROWS>,
+        TFn: Fn(D::DualVector<INROWS>) -> D::DualVector<OUTROWS>,
     {
         let jac = Self::fw_autodiff(vector_valued, a);
-        let mut sjac = MatF64::<OUTROWS, INROWS>::zeros();
+        let mut sjac = D::RealMatrix::<OUTROWS, INROWS>::zeros();
 
         for r in 0..INROWS {
             let v = jac.get([r]);
-            sjac.fixed_view_mut::<OUTROWS, 1>(0, r).copy_from(&v);
+            for c in 0..OUTROWS {
+                sjac[(c, r)] = v[c];
+            }
         }
 
         sjac
     }
 }
 
 /// Vector-valued map on a product space (= space of matrices).
 ///
 /// This is a function which takes a matrix and returns a vector:
 ///
 ///  f: ℝᵐ x ℝⁿ -> ℝʳ
 ///
 /// This type of function is also called a vector field (on product spaces).
 ///
-pub struct VectorValuedMapFromMatrix;
+pub struct VectorValuedMapFromMatrix<S: IsScalar<BATCH>, const BATCH: usize> {
+    phantom: std::marker::PhantomData<S>,
+}
 
-impl VectorValuedMapFromMatrix {
+impl<S: IsRealScalar<BATCH>, const BATCH: usize> VectorValuedMapFromMatrix<S, BATCH> {
     /// Finite difference quotient of the vector-valued map.
     ///
     /// The derivative is a matrix or rank-3 tensor with shape (Rₒ x Rᵢ x Cᵢ).
     ///
     /// For efficiency reasons, we return Rᵢ x Cᵢ x (Rₒ)
     ///
     pub fn sym_diff_quotient<TFn, const OUTROWS: usize, const INROWS: usize, const INCOLS: usize>(
         vector_valued: TFn,
-        a: MatF64<INROWS, INCOLS>,
+        a: S::RealMatrix<INROWS, INCOLS>,
         eps: f64,
-    ) -> MutTensorDDR<f64, OUTROWS>
+    ) -> MutTensorDDR<S, OUTROWS>
     where
-        TFn: Fn(MatF64<INROWS, INCOLS>) -> VecF64<OUTROWS>,
+        TFn: Fn(S::RealMatrix<INROWS, INCOLS>) -> SVec<S, OUTROWS>,
+        SVec<S, OUTROWS>: IsVector<S, OUTROWS, BATCH>,
     {
-        let mut out = MutTensorDDR::<f64, OUTROWS>::from_shape([INROWS, INCOLS]);
+        let mut out = MutTensorDDR::<S, OUTROWS>::from_shape([INROWS, INCOLS]);
+        let eps_b = S::RealScalar::from_f64(eps);
 
         for c in 0..INCOLS {
             for r in 0..INROWS {
                 let mut a_plus = a;
 
-                a_plus[(r, c)] += eps;
+                a_plus[(r, c)] += eps_b;
 
                 let mut a_minus = a;
 
-                a_minus[(r, c)] -= eps;
+                a_minus[(r, c)] -= eps_b;
 
-                let vv = (vector_valued(a_plus) - vector_valued(a_minus)) / (2.0 * eps);
+                let vv = (vector_valued(a_plus) - vector_valued(a_minus))
+                    .scaled(S::from_f64(1.0 / (2.0 * eps)));
                 *out.mut_view().get_mut([r, c]) = vv;
             }
         }
         out
     }
+}
 
+impl<D: IsDualScalar<BATCH, DualScalar = D>, const BATCH: usize>
+    VectorValuedMapFromMatrix<D, BATCH>
+{
     /// Auto differentiation of the vector-valued map.
     pub fn fw_autodiff<TFn, const OUTROWS: usize, const INROWS: usize, const INCOLS: usize>(
         vector_valued: TFn,
-        a: MatF64<INROWS, INCOLS>,
-    ) -> MutTensorDDR<f64, OUTROWS>
+        a: D::RealMatrix<INROWS, INCOLS>,
+    ) -> MutTensorDDR<D::RealScalar, OUTROWS>
     where
-        TFn: Fn(DualM<INROWS, INCOLS>) -> DualV<OUTROWS>,
+        TFn: Fn(D::DualMatrix<INROWS, INCOLS>) -> D::DualVector<OUTROWS>,
     {
-        vector_valued(DualM::v(a)).dij_val.unwrap()
+        vector_valued(D::matrix_with_dij(a)).dij_val().unwrap()
     }
 }
 
-mod test {
-
-    #[test]
-    fn test_batched_vector_valued_map_from_vector() {
-        use crate::maps::vector_valued_maps::VectorValuedMapFromVector;
-        use crate::types::scalar::IsScalar;
-        use crate::types::vector::IsVector;
-        use crate::types::VecF64;
-        use sophus_tensor::view::IsTensorLike;
-
-        let a = VecF64::<3>::new(0.6, 2.2, 1.1);
-
-        //       [[ x ]]   [[ x / z ]]
-        //  proj [[ y ]] = [[       ]]
-        //       [[ z ]]   [[ y / z ]]
-        fn proj_fn<S: IsScalar<1>, V2: IsVector<S, 2, 1>, V3: IsVector<S, 3, 1>>(v: V3) -> V2 {
-            let x = v.get(0);
-            let y = v.get(1);
-            let z = v.get(2);
-
-            V2::from_array([x / z.clone(), y / z])
-        }
-
-        let finite_diff = VectorValuedMapFromVector::sym_diff_quotient(proj_fn, a, 1e-6);
-        let auto_grad = VectorValuedMapFromVector::fw_autodiff(proj_fn, a);
-        for i in 0..2 {
-            approx::assert_abs_diff_eq!(finite_diff.get([i]), auto_grad.get([i]), epsilon = 0.0001);
-        }
-
-        let sfinite_diff = VectorValuedMapFromVector::static_sym_diff_quotient(proj_fn, a, 1e-6);
-        let sauto_grad = VectorValuedMapFromVector::static_fw_autodiff(proj_fn, a);
-        approx::assert_abs_diff_eq!(sfinite_diff, sauto_grad, epsilon = 0.0001);
+#[test]
+fn vector_valued_map_from_vector_tests() {
+    use crate::calculus::dual::dual_scalar::DualBatchScalar;
+    use crate::calculus::dual::dual_scalar::DualScalar;
+    use crate::calculus::maps::vector_valued_maps::VectorValuedMapFromMatrix;
+    use crate::calculus::maps::vector_valued_maps::VectorValuedMapFromVector;
+
+    use crate::linalg::vector::IsVector;
+    use crate::linalg::BatchScalarF64;
+    use crate::tensor::tensor_view::IsTensorLike;
+
+    #[cfg(test)]
+    trait Test {
+        fn run();
     }
 
-    #[test]
-    fn test_batched_vector_valued_map_from_matrix() {
-        use crate::maps::vector_valued_maps::VectorValuedMapFromMatrix;
-        use crate::types::matrix::IsMatrix;
-        use crate::types::scalar::IsScalar;
-        use crate::types::vector::IsVector;
-        use crate::types::MatF64;
-        use sophus_tensor::view::IsTensorLike;
-
-        fn f<S: IsScalar<1>, M32: IsMatrix<S, 3, 2, 1>, V4: IsVector<S, 4, 1>>(x: M32) -> V4 {
-            let a = x.get((0, 0));
-            let b = x.get((0, 1));
-            let c = x.get((1, 0));
-            let d = x.get((1, 1));
-            let e = x.get((2, 0));
-            let f = x.get((2, 1));
-
-            V4::from_array([a + b, c + d, e + f, S::c(1.0)])
-        }
-
-        let mut mat = MatF64::<3, 2>::zeros();
-        mat[(0, 0)] = -4.6;
-        mat[(0, 1)] = -1.6;
-        mat[(1, 0)] = 0.6;
-        mat[(1, 1)] = 1.6;
-        mat[(2, 0)] = -1.6;
-        mat[(2, 1)] = 0.2;
-
-        let finite_diff = VectorValuedMapFromMatrix::sym_diff_quotient(f, mat, 1e-6);
-        let auto_grad = VectorValuedMapFromMatrix::fw_autodiff(f, mat);
-        approx::assert_abs_diff_eq!(
-            finite_diff.elem_view(),
-            auto_grad.elem_view(),
-            epsilon = 0.0001
-        );
+    macro_rules! def_test_template {
+        ( $scalar:ty, $dual_scalar: ty, $batch:literal
+    ) => {
+            #[cfg(test)]
+            impl Test for $scalar {
+                fn run() {
+                    {
+                        let a = <$scalar as IsScalar<$batch>>::RealVector::<3>::new(
+                            <$scalar>::from_f64(0.6),
+                            <$scalar>::from_f64(2.2),
+                            <$scalar>::from_f64(1.1),
+                        );
+
+                        //       [[ x ]]   [[ x / z ]]
+                        //  proj [[ y ]] = [[       ]]
+                        //       [[ z ]]   [[ y / z ]]
+                        fn proj_fn<S: IsScalar<BATCH>, const BATCH: usize>(
+                            v: S::Vector<3>,
+                        ) -> S::Vector<2> {
+                            let x = IsVector::get_elem(&v, 0);
+                            let y = IsVector::get_elem(&v, 1);
+                            let z = IsVector::get_elem(&v, 2);
+                            S::Vector::<2>::from_array([x / z.clone(), y / z])
+                        }
+
+                        let finite_diff =
+                            VectorValuedMapFromVector::<$scalar, $batch>::sym_diff_quotient(
+                                proj_fn::<$scalar, $batch>,
+                                a,
+                                1e-6,
+                            );
+                        let auto_grad =
+                            VectorValuedMapFromVector::<$dual_scalar, $batch>::fw_autodiff(
+                                proj_fn::<$dual_scalar, $batch>,
+                                a,
+                            );
+                        for i in 0..2 {
+                            approx::assert_abs_diff_eq!(
+                                finite_diff.get([i]),
+                                auto_grad.get([i]),
+                                epsilon = 0.0001
+                            );
+                        }
+
+                        let sfinite_diff =
+                            VectorValuedMapFromVector::<$scalar, $batch>::static_sym_diff_quotient(
+                                proj_fn::<$scalar, $batch>,
+                                a,
+                                1e-6,
+                            );
+                        let sauto_grad =
+                            VectorValuedMapFromVector::<$dual_scalar, $batch>::static_fw_autodiff(
+                                proj_fn::<$dual_scalar, $batch>,
+                                a,
+                            );
+                        approx::assert_abs_diff_eq!(sfinite_diff, sauto_grad, epsilon = 0.0001);
+                    }
+
+                    fn f<S: IsScalar<BATCH>, const BATCH: usize>(
+                        x: S::Matrix<3, 2>,
+                    ) -> S::Vector<4> {
+                        let a = x.get_elem([0, 0]);
+                        let b = x.get_elem([0, 1]);
+                        let c = x.get_elem([1, 0]);
+                        let d = x.get_elem([1, 1]);
+                        let e = x.get_elem([2, 0]);
+                        let f = x.get_elem([2, 1]);
+
+                        S::Vector::<4>::from_array([a + b, c + d, e + f, S::from_f64(1.0)])
+                    }
+
+                    let mut mat = <$scalar as IsScalar<$batch>>::RealMatrix::<3, 2>::zeros();
+                    mat[(0, 0)] = <$scalar>::from_f64(-4.6);
+                    mat[(0, 1)] = <$scalar>::from_f64(-1.6);
+                    mat[(1, 0)] = <$scalar>::from_f64(0.6);
+                    mat[(1, 1)] = <$scalar>::from_f64(1.6);
+                    mat[(2, 0)] = <$scalar>::from_f64(-1.6);
+                    mat[(2, 1)] = <$scalar>::from_f64(0.2);
+
+                    let finite_diff =
+                        VectorValuedMapFromMatrix::<$scalar, $batch>::sym_diff_quotient(
+                            f::<$scalar, $batch>,
+                            mat,
+                            1e-6,
+                        );
+                    let auto_grad = VectorValuedMapFromMatrix::<$dual_scalar, $batch>::fw_autodiff(
+                        f::<$dual_scalar, $batch>,
+                        mat,
+                    );
+                    approx::assert_abs_diff_eq!(
+                        finite_diff.elem_view(),
+                        auto_grad.elem_view(),
+                        epsilon = 0.0001
+                    );
+                }
+            }
+        };
     }
+
+    def_test_template!(f64, DualScalar, 1);
+    def_test_template!(BatchScalarF64<2>, DualBatchScalar<2>, 2);
+    def_test_template!(BatchScalarF64<4>, DualBatchScalar<4>, 4);
+
+    f64::run();
+    BatchScalarF64::<2>::run();
+    BatchScalarF64::<4>::run();
 }
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_calculus/src/spline/spline_segment.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/calculus/spline/spline_segment.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,83 @@
-use crate::types::matrix::IsMatrix;
-use crate::types::scalar::IsScalar;
-use crate::types::vector::IsVector;
-use crate::types::vector::IsVectorLike;
-
+use crate::prelude::*;
 use std::marker::PhantomData;
 
 /// cubic basis function
 pub struct CubicBasisFunction<S> {
     phantom: PhantomData<S>,
 }
 
-impl<S: IsScalar<1>> CubicBasisFunction<S> {
+impl<S: IsSingleScalar> CubicBasisFunction<S> {
     /// C matrix
-    pub fn c() -> S::Matrix<3, 4> {
-        S::Matrix::<3, 4>::from_c_array2([
+    pub fn c() -> S::SingleMatrix<3, 4> {
+        S::SingleMatrix::<3, 4>::from_f64_array2([
             [5.0 / 6.0, 3.0 / 6.0, -3.0 / 6.0, 1.0 / 6.0],
             [1.0 / 6.0, 3.0 / 6.0, 3.0 / 6.0, -2.0 / 6.0],
             [0.0, 0.0, 0.0, 1.0 / 6.0],
         ])
     }
 
     /// B(u) matrix
-    pub fn b(u: S) -> S::Vector<3> {
+    pub fn b(u: S) -> S::SingleVector<3> {
         let u_sq = u.clone() * u.clone();
-        Self::c() * S::Vector::<4>::from_array([1.0.into(), u.clone(), u_sq.clone(), u_sq * u])
+        let m34 = Self::c();
+        let v4 =
+            S::SingleVector::<4>::from_array([S::from_f64(1.0), u.clone(), u_sq.clone(), u_sq * u]);
+
+        m34 * v4
     }
 
     /// derivative of B(u) matrix with respect to u
-    pub fn du_b(u: S, delta_t: S) -> S::Vector<3> {
+    pub fn du_b(u: S, delta_t: S) -> S::SingleVector<3> {
         let u_sq = u.clone() * u.clone();
-        Self::c().scaled(S::c(1.0) / delta_t)
-            * S::Vector::<4>::from_array([S::c(0.0), S::c(1.0), S::c(2.0) * u, S::c(3.0) * u_sq])
+        Self::c().scaled(S::from_f64(1.0) / delta_t)
+            * S::SingleVector::<4>::from_array([
+                S::from_f64(0.0),
+                S::from_f64(1.0),
+                S::from_f64(2.0) * u,
+                S::from_f64(3.0) * u_sq,
+            ])
     }
 
     /// second derivative of B(u) matrix with respect to u
-    pub fn du2_b(u: S, delta_t: S) -> S::Vector<3> {
-        Self::c().scaled(S::c(1.0) / (delta_t.clone() * delta_t))
-            * S::Vector::<4>::from_array([S::c(0.0), S::c(0.0), S::c(2.0), S::c(6.0) * u])
+    pub fn du2_b(u: S, delta_t: S) -> S::SingleVector<3> {
+        Self::c().scaled(S::from_f64(1.0) / (delta_t.clone() * delta_t))
+            * S::SingleVector::<4>::from_array([
+                S::from_f64(0.0),
+                S::from_f64(0.0),
+                S::from_f64(2.0),
+                S::from_f64(6.0) * u,
+            ])
     }
 }
 
 /// cubic B-spline function
-pub struct CubicBSplineFn<S: IsScalar<1>, const DIMS: usize> {
+pub struct CubicBSplineFn<S: IsSingleScalar, const DIMS: usize> {
     phantom: PhantomData<S>,
 }
 
-impl<S: IsScalar<1>, const DIMS: usize> CubicBSplineFn<S, DIMS> {
+impl<S: IsSingleScalar, const DIMS: usize> CubicBSplineFn<S, DIMS> {
     fn interpolate(
-        control_point: S::Vector<DIMS>,
-        control_points: [S::Vector<DIMS>; 3],
+        control_point: S::SingleVector<DIMS>,
+        control_points: [S::SingleVector<DIMS>; 3],
         u: S,
-    ) -> S::Vector<DIMS> {
+    ) -> S::SingleVector<DIMS> {
         let b = CubicBasisFunction::<S>::b(u);
         control_point
-            + control_points[0].scaled(b.get(0))
-            + control_points[1].scaled(b.get(1))
-            + control_points[2].scaled(b.get(2))
+            + control_points[0].scaled(b.get_elem(0))
+            + control_points[1].scaled(b.get_elem(1))
+            + control_points[2].scaled(b.get_elem(2))
     }
 
-    fn dxi_interpolate(u: S, quadruple_idx: usize) -> S::Matrix<DIMS, DIMS> {
+    fn dxi_interpolate(u: S, quadruple_idx: usize) -> S::SingleMatrix<DIMS, DIMS> {
         let b = CubicBasisFunction::<S>::b(u.clone());
         if quadruple_idx == 0 {
-            S::Matrix::<DIMS, DIMS>::identity()
+            S::SingleMatrix::<DIMS, DIMS>::identity()
         } else {
-            S::Matrix::<DIMS, DIMS>::identity().scaled(b.get(quadruple_idx - 1))
+            S::SingleMatrix::<DIMS, DIMS>::identity().scaled(b.get_elem(quadruple_idx - 1))
         }
     }
 }
 
 /// Segment case
 #[derive(Clone, Debug, Copy)]
 pub enum SegmentCase {
@@ -77,27 +87,27 @@
     Normal,
     /// Last segment
     Last,
 }
 
 /// Cubic B-spline segment
 #[derive(Clone, Debug)]
-pub struct CubicBSplineSegment<S: IsScalar<1>, const DIMS: usize> {
+pub struct CubicBSplineSegment<S: IsSingleScalar, const DIMS: usize> {
     pub(crate) case: SegmentCase,
-    pub(crate) control_points: [S::Vector<DIMS>; 4],
+    pub(crate) control_points: [S::SingleVector<DIMS>; 4],
 }
 
-impl<S: IsScalar<1>, const DIMS: usize> CubicBSplineSegment<S, DIMS> {
+impl<S: IsSingleScalar, const DIMS: usize> CubicBSplineSegment<S, DIMS> {
     /// Interpolate
-    pub fn interpolate(&self, u: S) -> S::Vector<DIMS> {
+    pub fn interpolate(&self, u: S) -> S::SingleVector<DIMS> {
         match self.case {
             SegmentCase::First => CubicBSplineFn::interpolate(
                 self.control_points[1].clone(),
                 [
-                    S::Vector::<DIMS>::zero(),
+                    S::SingleVector::<DIMS>::zeros(),
                     self.control_points[2].clone() - self.control_points[1].clone(),
                     self.control_points[3].clone() - self.control_points[2].clone(),
                 ],
                 u,
             ),
             SegmentCase::Normal => CubicBSplineFn::interpolate(
                 self.control_points[0].clone(),
@@ -109,27 +119,27 @@
                 u,
             ),
             SegmentCase::Last => CubicBSplineFn::interpolate(
                 self.control_points[0].clone(),
                 [
                     self.control_points[1].clone() - self.control_points[0].clone(),
                     self.control_points[2].clone() - self.control_points[1].clone(),
-                    S::Vector::<DIMS>::zero(),
+                    S::SingleVector::<DIMS>::zeros(),
                 ],
                 u,
             ),
         }
     }
 
     /// Derivative of the interpolation with respect to u
-    pub fn dxi_interpolate(&self, u: S, quadruple_idx: usize) -> S::Matrix<DIMS, DIMS> {
+    pub fn dxi_interpolate(&self, u: S, quadruple_idx: usize) -> S::SingleMatrix<DIMS, DIMS> {
         match self.case {
             SegmentCase::First => {
                 if quadruple_idx == 0 {
-                    S::Matrix::<DIMS, DIMS>::zero()
+                    S::SingleMatrix::<DIMS, DIMS>::zeros()
                 } else if quadruple_idx == 1 {
                     CubicBSplineFn::dxi_interpolate(u.clone(), 0)
                         - CubicBSplineFn::dxi_interpolate(u.clone(), 2)
                 } else if quadruple_idx == 2 {
                     CubicBSplineFn::dxi_interpolate(u.clone(), 2)
                         - CubicBSplineFn::dxi_interpolate(u.clone(), 3)
                 } else {
@@ -156,117 +166,124 @@
                         - CubicBSplineFn::dxi_interpolate(u.clone(), 1)
                 } else if quadruple_idx == 1 {
                     CubicBSplineFn::dxi_interpolate(u.clone(), 1)
                         - CubicBSplineFn::dxi_interpolate(u.clone(), 2)
                 } else if quadruple_idx == 2 {
                     CubicBSplineFn::dxi_interpolate(u.clone(), 2)
                 } else {
-                    S::Matrix::<DIMS, DIMS>::zero()
+                    S::SingleMatrix::<DIMS, DIMS>::zeros()
                 }
             }
         }
     }
 }
 
 mod test {
 
     #[test]
     fn test_spline_basis_fn() {
-        use crate::dual::dual_scalar::Dual;
-        use crate::dual::dual_vector::DualV;
-        use crate::maps::vector_valued_maps::VectorValuedMapFromVector;
+        use crate::calculus::dual::dual_scalar::DualScalar;
+        use crate::calculus::dual::dual_vector::DualVector;
+        use crate::calculus::maps::vector_valued_maps::VectorValuedMapFromVector;
+        use crate::calculus::spline::spline_segment::CubicBSplineFn;
+        use crate::linalg::scalar::IsScalar;
+        use crate::linalg::vector::IsVector;
+        use crate::linalg::VecF64;
         use crate::points::example_points;
-        use crate::spline::spline_segment::CubicBSplineFn;
-        use crate::types::scalar::IsScalar;
-        use crate::types::vector::IsVector;
-        use crate::types::vector::IsVectorLike;
-        use crate::types::VecF64;
+        use num_traits::Zero;
 
-        let points = &example_points::<f64, 3>();
+        let points = &example_points::<f64, 3, 1>();
         assert!(points.len() >= 8);
 
         let mut u = 0.0;
         loop {
             if u >= 1.0 {
                 break;
             }
 
             for p_idx in 0..points.len() - 4 {
                 let first_control_point = points[p_idx];
-                let first_control_point_dual = DualV::c(points[p_idx]);
+                let first_control_point_dual = DualVector::from_real_vector(points[p_idx]);
                 let mut segment_control_points = [VecF64::<3>::zeros(); 3];
-                let mut segment_control_points_dual =
-                    [DualV::<3>::zero(), DualV::<3>::zero(), DualV::<3>::zero()];
+                let mut segment_control_points_dual = [
+                    DualVector::<3>::zero(),
+                    DualVector::<3>::zero(),
+                    DualVector::<3>::zero(),
+                ];
                 for i in 0..3 {
                     segment_control_points[i] = points[p_idx + 1];
-                    segment_control_points_dual[i] = DualV::c(segment_control_points[i]);
+                    segment_control_points_dual[i] =
+                        DualVector::from_real_vector(segment_control_points[i]);
                 }
 
-                let f0 = |x| -> DualV<3> {
-                    CubicBSplineFn::<Dual, 3>::interpolate(
+                let f0 = |x| -> DualVector<3> {
+                    CubicBSplineFn::<DualScalar, 3>::interpolate(
                         x,
                         segment_control_points_dual.clone(),
-                        Dual::c(u),
+                        DualScalar::from_real_scalar(u),
                     )
                 };
-                let auto_dx0 =
-                    VectorValuedMapFromVector::static_fw_autodiff(f0, first_control_point);
+                let auto_dx0 = VectorValuedMapFromVector::<DualScalar, 1>::static_fw_autodiff(
+                    f0,
+                    first_control_point,
+                );
                 let analytic_dx0 = CubicBSplineFn::<f64, 3>::dxi_interpolate(u, 0);
                 approx::assert_abs_diff_eq!(auto_dx0, analytic_dx0, epsilon = 0.0001);
 
                 for i in 0..3 {
-                    let fi = |x| -> DualV<3> {
+                    let fi = |x| -> DualVector<3> {
                         let mut seg = segment_control_points_dual.clone();
                         seg[i] = x;
-                        CubicBSplineFn::<Dual, 3>::interpolate(
+                        CubicBSplineFn::<DualScalar, 3>::interpolate(
                             first_control_point_dual.clone(),
                             seg,
-                            Dual::c(u),
+                            DualScalar::from_real_scalar(u),
                         )
                     };
-                    let auto_dxi = VectorValuedMapFromVector::static_fw_autodiff(
+                    let auto_dxi = VectorValuedMapFromVector::<DualScalar, 1>::static_fw_autodiff(
                         fi,
                         segment_control_points[i],
                     );
                     let analytic_dxi = CubicBSplineFn::<f64, 3>::dxi_interpolate(u, i + 1);
                     approx::assert_abs_diff_eq!(auto_dxi, analytic_dxi, epsilon = 0.0001);
                 }
             }
             u += 0.1;
         }
     }
 
     #[test]
     fn test_spline_segment() {
-        use crate::dual::dual_scalar::Dual;
-        use crate::dual::dual_vector::DualV;
-        use crate::maps::vector_valued_maps::VectorValuedMapFromVector;
+        use crate::calculus::dual::dual_scalar::DualScalar;
+        use crate::calculus::dual::dual_vector::DualVector;
+        use crate::calculus::maps::vector_valued_maps::VectorValuedMapFromVector;
+        use crate::calculus::spline::spline_segment::CubicBSplineSegment;
+        use crate::calculus::spline::spline_segment::SegmentCase;
+        use crate::linalg::scalar::IsScalar;
+        use crate::linalg::vector::IsVector;
+        use crate::linalg::VecF64;
         use crate::points::example_points;
-        use crate::spline::spline_segment::CubicBSplineSegment;
-        use crate::spline::spline_segment::SegmentCase;
-        use crate::types::scalar::IsScalar;
-        use crate::types::vector::IsVector;
-        use crate::types::vector::IsVectorLike;
-        use crate::types::VecF64;
+        use num_traits::Zero;
 
-        let points = &example_points::<f64, 3>();
+        let points = &example_points::<f64, 3, 1>();
         assert!(points.len() >= 8);
 
         for p_idx in 0..points.len() - 4 {
             let mut segment_control_points = [VecF64::<3>::zeros(); 4];
             let mut segment_control_points_dual = [
-                DualV::<3>::zero(),
-                DualV::<3>::zero(),
-                DualV::<3>::zero(),
-                DualV::<3>::zero(),
+                DualVector::<3>::zero(),
+                DualVector::<3>::zero(),
+                DualVector::<3>::zero(),
+                DualVector::<3>::zero(),
             ];
 
             for i in 0..4 {
                 segment_control_points[i] = points[p_idx];
-                segment_control_points_dual[i] = DualV::c(segment_control_points[i]);
+                segment_control_points_dual[i] =
+                    DualVector::from_real_vector(segment_control_points[i]);
             }
 
             for case in [SegmentCase::First, SegmentCase::Normal, SegmentCase::Last] {
                 let base = CubicBSplineSegment::<f64, 3> {
                     case,
                     control_points: segment_control_points,
                 };
@@ -284,25 +301,29 @@
                             base_copy.interpolate(u)
                         };
 
                         let num_dx = VectorValuedMapFromVector::static_sym_diff_quotient(
                             f, points[0], 0.0001,
                         );
 
-                        let f = |v: DualV<3>| {
-                            let mut base_dual = CubicBSplineSegment::<Dual, 3> {
+                        let f = |v: DualVector<3>| {
+                            let mut base_dual = CubicBSplineSegment::<DualScalar, 3> {
                                 case,
                                 control_points: segment_control_points_dual.clone(),
                             };
 
                             base_dual.control_points[i] = v;
-                            base_dual.interpolate(Dual::c(u))
+                            base_dual.interpolate(DualScalar::from_real_scalar(u))
                         };
 
-                        let auto_dx = VectorValuedMapFromVector::static_fw_autodiff(f, points[i]);
+                        let auto_dx =
+                            VectorValuedMapFromVector::<DualScalar, 1>::static_fw_autodiff(
+                                f,
+                                segment_control_points[i],
+                            );
 
                         approx::assert_abs_diff_eq!(analytic_dx, num_dx, epsilon = 0.0001);
                         approx::assert_abs_diff_eq!(analytic_dx, auto_dx, epsilon = 0.0001);
                     }
                     u += 0.1;
                 }
             }
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_calculus/src/types/params.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/params.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,53 @@
-use crate::types::scalar::IsScalar;
+use crate::linalg::VecF64;
+use crate::points::example_points;
+use crate::prelude::*;
 
 /// Parameter implementation.
 pub trait ParamsImpl<S: IsScalar<BATCH_SIZE>, const PARAMS: usize, const BATCH_SIZE: usize> {
     /// Is the parameter vector valid?
-    fn are_params_valid(params: &S::Vector<PARAMS>) -> bool;
+    fn are_params_valid(params: &S::Vector<PARAMS>) -> S::Mask;
     /// Examples of valid parameter vectors.
     fn params_examples() -> Vec<S::Vector<PARAMS>>;
     /// Examples of invalid parameter vectors.
     fn invalid_params_examples() -> Vec<S::Vector<PARAMS>>;
 }
 
-/// A trait for types that have parameters.
+/// A trait for linalg that have parameters.
 pub trait HasParams<S: IsScalar<BATCH_SIZE>, const PARAMS: usize, const BATCH_SIZE: usize>:
     ParamsImpl<S, PARAMS, BATCH_SIZE>
 {
     /// Create from parameters.
     fn from_params(params: &S::Vector<PARAMS>) -> Self;
     /// Set parameters.
     fn set_params(&mut self, params: &S::Vector<PARAMS>);
     /// Get parameters.
     fn params(&self) -> &S::Vector<PARAMS>;
 }
+
+impl<const N: usize> ParamsImpl<f64, N, 1> for VecF64<N> {
+    fn are_params_valid(_params: &VecF64<N>) -> bool {
+        true
+    }
+
+    fn params_examples() -> Vec<VecF64<N>> {
+        example_points::<f64, N, 1>()
+    }
+
+    fn invalid_params_examples() -> Vec<VecF64<N>> {
+        vec![]
+    }
+}
+
+impl<const N: usize> HasParams<f64, N, 1> for VecF64<N> {
+    fn from_params(params: &VecF64<N>) -> Self {
+        *params
+    }
+
+    fn set_params(&mut self, params: &VecF64<N>) {
+        *self = *params
+    }
+
+    fn params(&self) -> &VecF64<N> {
+        self
+    }
+}
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_lie/src/isometry2.rs` & `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/isometry3.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-use super::{
-    lie_group::LieGroup, rotation2::Rotation2Impl,
-    translation_product_product::TranslationProductGroupImpl,
-};
-use crate::rotation2::Rotation2;
-use crate::traits::IsTranslationProductGroup;
-use sophus_calculus::types::scalar::IsScalar;
+use super::rotation3::Rotation3Impl;
+use super::translation_product_product::TranslationProductGroupImpl;
+use crate::lie_group::LieGroup;
+use crate::prelude::*;
+use crate::Rotation3;
+
+/// 3D isometry group implementation struct - SE(3)
+pub type Isometry3Impl<S, const BATCH: usize> =
+    TranslationProductGroupImpl<S, 6, 7, 3, 4, 3, 4, BATCH, Rotation3Impl<S, BATCH>>;
+/// 3d isometry group - SE(3)
+pub type Isometry3<S, const BATCH: usize> = LieGroup<S, 6, 7, 3, 4, BATCH, Isometry3Impl<S, BATCH>>;
 
-/// 2D isometry group implementation struct - SE(2)
-pub type Isometry2Impl<S> = TranslationProductGroupImpl<S, 3, 4, 2, 3, 1, 2, Rotation2Impl<S>>;
-
-/// 2D isometry group - SE(2)
-pub type Isometry2<S> = LieGroup<S, 3, 4, 2, 3, 1, Isometry2Impl<S>>;
-
-impl<S: IsScalar<1>> Isometry2<S> {
+impl<S: IsScalar<BATCH>, const BATCH: usize> Isometry3<S, BATCH> {
     /// create isometry from translation and rotation
     pub fn from_translation_and_rotation(
-        translation: &<S as IsScalar<1>>::Vector<2>,
-        rotation: &Rotation2<S>,
+        translation: &S::Vector<3>,
+        rotation: &Rotation3<S, BATCH>,
     ) -> Self {
         Self::from_translation_and_factor(translation, rotation)
     }
 
     /// set rotation
-    pub fn set_rotation(&mut self, rotation: &Rotation2<S>) {
+    pub fn set_rotation(&mut self, rotation: &Rotation3<S, BATCH>) {
         self.set_factor(rotation)
     }
 
     /// get rotation
-    pub fn rotation(&self) -> Rotation2<S> {
+    pub fn rotation(&self) -> Rotation3<S, BATCH> {
         self.factor()
     }
 }
 
-mod tests {
+#[test]
+fn isometry3_prop_tests() {
+    use crate::real_lie_group::RealLieGroupTest;
+    use sophus_core::calculus::dual::dual_scalar::DualBatchScalar;
+    use sophus_core::calculus::dual::dual_scalar::DualScalar;
+    use sophus_core::linalg::BatchScalarF64;
+
+    Isometry3::<f64, 1>::test_suite();
+    Isometry3::<BatchScalarF64<8>, 8>::test_suite();
+    Isometry3::<DualScalar, 1>::test_suite();
+    Isometry3::<DualBatchScalar<8>, 8>::test_suite();
 
-    #[test]
-    fn isometry2_prop_tests() {
-        use super::Isometry2;
-        use sophus_calculus::dual::dual_scalar::Dual;
-
-        Isometry2::<f64>::test_suite();
-        Isometry2::<Dual>::test_suite();
-        Isometry2::<f64>::real_test_suite();
-    }
+    Isometry3::<f64, 1>::run_real_tests();
+    Isometry3::<BatchScalarF64<8>, 8>::run_real_tests();
 }
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_lie/src/traits.rs` & `sophus_pyo3-0.6.0/crates/sophus_lie/src/traits.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,12 @@
+use crate::prelude::*;
+use sophus_core::manifold::traits::TangentImpl;
+use sophus_core::params::ParamsImpl;
 use std::fmt::Debug;
 
-use sophus_calculus::dual::dual_scalar::Dual;
-use sophus_calculus::manifold::traits::TangentImpl;
-use sophus_calculus::manifold::{self};
-use sophus_calculus::types::params::HasParams;
-use sophus_calculus::types::params::ParamsImpl;
-use sophus_calculus::types::scalar::IsScalar;
-use sophus_calculus::types::MatF64;
-use sophus_calculus::types::VecF64;
-
 /// Lie Group implementation trait
 ///
 /// Here, the actual manifold is represented by as a N-dimensional parameter tuple.
 /// See LieGroup struct for the concrete implementation.
 ///
 /// DOF: Degrees of freedom
 /// NUM_PARAMS:
@@ -21,26 +15,22 @@
 pub trait IsLieGroupImpl<
     S: IsScalar<BATCH_SIZE>,
     const DOF: usize,
     const PARAMS: usize,
     const POINT: usize,
     const AMBIENT: usize,
     const BATCH_SIZE: usize,
->:
-    ParamsImpl<S, PARAMS, BATCH_SIZE>
-    + manifold::traits::TangentImpl<S, DOF, BATCH_SIZE>
-    + Clone
-    + Debug
+>: ParamsImpl<S, PARAMS, BATCH_SIZE> + TangentImpl<S, DOF, BATCH_SIZE> + Clone + Debug
 {
     /// Generic scalar, real scalar, and dual scalar
     type GenG<S2: IsScalar<BATCH_SIZE>>: IsLieGroupImpl<S2, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
     /// Real scalar
-    type RealG: IsLieGroupImpl<f64, DOF, PARAMS, POINT, AMBIENT, 1>;
-    /// Dual scalar - for automatic differentiation
-    type DualG: IsLieGroupImpl<Dual, DOF, PARAMS, POINT, AMBIENT, 1>;
+    type RealG: IsLieGroupImpl<S::RealScalar, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
+    /// DualScalar scalar - for automatic differentiation
+    type DualG: IsLieGroupImpl<S::DualScalar, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
 
     /// is transformation origin preserving?
     const IS_ORIGIN_PRESERVING: bool;
     /// is transformation axis direction preserving?
     const IS_AXIS_DIRECTION_PRESERVING: bool;
     /// is transformation direction vector preserving?
     const IS_DIRECTION_VECTOR_PRESERVING: bool;
@@ -52,17 +42,14 @@
     const IS_PARALLEL_LINE_PRESERVING: bool;
 
     /// identity parameters
     fn identity_params() -> S::Vector<PARAMS>;
 
     // Manifold / Lie Group concepts
 
-    /// are there multiple shortest paths to the identity?
-    fn has_shortest_path_ambiguity(params: &S::Vector<PARAMS>) -> bool;
-
     /// group adjoint
     fn adj(params: &S::Vector<PARAMS>) -> S::Matrix<DOF, DOF>;
 
     /// algebra adjoint
     fn ad(tangent: &S::Vector<DOF>) -> S::Matrix<DOF, DOF>;
 
     /// exponential map
@@ -97,38 +84,43 @@
     fn compact(params: &S::Vector<PARAMS>) -> S::Matrix<POINT, AMBIENT>;
 
     /// return square matrix representation
     fn matrix(params: &S::Vector<PARAMS>) -> S::Matrix<AMBIENT, AMBIENT>;
 }
 
 /// Lie Group implementation trait for real scalar, f64
-pub trait IsF64LieGroupImpl<
+pub trait IsRealLieGroupImpl<
+    S: IsRealScalar<BATCH_SIZE>,
     const DOF: usize,
     const PARAMS: usize,
     const POINT: usize,
     const AMBIENT: usize,
->: IsLieGroupImpl<f64, DOF, PARAMS, POINT, AMBIENT, 1>
+    const BATCH_SIZE: usize,
+>: IsLieGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>
 {
     /// derivative of group multiplication with respect to the first argument
-    fn da_a_mul_b(a: &VecF64<PARAMS>, b: &VecF64<PARAMS>) -> MatF64<PARAMS, PARAMS>;
+    fn da_a_mul_b(a: &S::Vector<PARAMS>, b: &S::Vector<PARAMS>) -> S::Matrix<PARAMS, PARAMS>;
 
     /// derivative of group multiplication with respect to the second argument
-    fn db_a_mul_b(a: &VecF64<PARAMS>, b: &VecF64<PARAMS>) -> MatF64<PARAMS, PARAMS>;
+    fn db_a_mul_b(a: &S::Vector<PARAMS>, b: &S::Vector<PARAMS>) -> S::Matrix<PARAMS, PARAMS>;
 
     /// derivative of exponential map
-    fn dx_exp(tangent: &VecF64<DOF>) -> MatF64<PARAMS, DOF>;
+    fn dx_exp(tangent: &S::Vector<DOF>) -> S::Matrix<PARAMS, DOF>;
 
     /// derivative of exponential map at the identity
-    fn dx_exp_x_at_0() -> MatF64<PARAMS, DOF>;
+    fn dx_exp_x_at_0() -> S::Matrix<PARAMS, DOF>;
 
     /// derivative of logarithmic map
-    fn dx_log_x(params: &VecF64<PARAMS>) -> MatF64<DOF, PARAMS>;
+    fn dx_log_x(params: &S::Vector<PARAMS>) -> S::Matrix<DOF, PARAMS>;
 
     /// derivative of exponential map times a point at the identity
-    fn dx_exp_x_times_point_at_0(point: VecF64<POINT>) -> MatF64<POINT, DOF>;
+    fn dx_exp_x_times_point_at_0(point: S::Vector<POINT>) -> S::Matrix<POINT, DOF>;
+
+    /// are there multiple shortest paths to the identity?
+    fn has_shortest_path_ambiguity(params: &S::Vector<PARAMS>) -> S::Mask;
 }
 
 /// Lie Factor Group
 ///
 /// Can be a factor of a semi-direct product group
 pub trait IsLieFactorGroupImpl<
     S: IsScalar<BATCH_SIZE>,
@@ -143,17 +135,17 @@
         S2,
         DOF,
         PARAMS,
         POINT,
         BATCH_SIZE,
     >;
     /// Real scalar
-    type RealFactorG: IsLieFactorGroupImpl<f64, DOF, PARAMS, POINT, 1>;
-    /// Dual scalar - for automatic differentiation
-    type DualFactorG: IsLieFactorGroupImpl<Dual, DOF, PARAMS, POINT, 1>;
+    type RealFactorG: IsLieFactorGroupImpl<S::RealScalar, DOF, PARAMS, POINT, BATCH_SIZE>;
+    /// DualScalar scalar - for automatic differentiation
+    type DualFactorG: IsLieFactorGroupImpl<S::DualScalar, DOF, PARAMS, POINT, BATCH_SIZE>;
 
     /// V matrix - used by semi-direct product exponential
     fn mat_v(tangent: &S::Vector<DOF>) -> S::Matrix<POINT, POINT>;
 
     /// V matrix inverse - used by semi-direct product logarithm
     fn mat_v_inverse(tangent: &S::Vector<DOF>) -> S::Matrix<POINT, POINT>;
 
@@ -164,30 +156,36 @@
     ) -> S::Matrix<POINT, DOF>;
 
     /// algebra adjoint of translation
     fn ad_of_translation(point: &S::Vector<POINT>) -> S::Matrix<POINT, DOF>;
 }
 
 /// Lie Factor Group implementation trait for real scalar, f64
-pub trait IsF64LieFactorGroupImpl<const DOF: usize, const PARAMS: usize, const POINT: usize>:
-    IsLieGroupImpl<f64, DOF, PARAMS, POINT, POINT, 1>
-    + IsLieFactorGroupImpl<f64, DOF, PARAMS, POINT, 1>
-    + IsF64LieGroupImpl<DOF, PARAMS, POINT, POINT>
+pub trait IsRealLieFactorGroupImpl<
+    S: IsRealScalar<BATCH_SIZE>,
+    const DOF: usize,
+    const PARAMS: usize,
+    const POINT: usize,
+    const BATCH_SIZE: usize,
+>:
+    IsLieGroupImpl<S, DOF, PARAMS, POINT, POINT, BATCH_SIZE>
+    + IsLieFactorGroupImpl<S, DOF, PARAMS, POINT, BATCH_SIZE>
+    + IsRealLieGroupImpl<S, DOF, PARAMS, POINT, POINT, BATCH_SIZE>
 {
     /// derivative of V matrix
-    fn dx_mat_v(tangent: &VecF64<DOF>) -> [MatF64<POINT, POINT>; DOF];
+    fn dx_mat_v(tangent: &S::Vector<DOF>) -> [S::Matrix<POINT, POINT>; DOF];
 
     /// derivative of V matrix inverse
-    fn dx_mat_v_inverse(tangent: &VecF64<DOF>) -> [MatF64<POINT, POINT>; DOF];
+    fn dx_mat_v_inverse(tangent: &S::Vector<DOF>) -> [S::Matrix<POINT, POINT>; DOF];
 
     /// derivative of group transformation times a point with respect to the group parameters
     fn dparams_matrix_times_point(
-        params: &VecF64<PARAMS>,
-        point: &VecF64<POINT>,
-    ) -> MatF64<POINT, PARAMS>;
+        params: &S::Vector<PARAMS>,
+        point: &S::Vector<POINT>,
+    ) -> S::Matrix<POINT, PARAMS>;
 }
 
 /// Lie Group trait
 pub trait IsLieGroup<
     S: IsScalar<BATCH_SIZE>,
     const DOF: usize,
     const PARAMS: usize,
@@ -197,31 +195,40 @@
 >: TangentImpl<S, DOF, BATCH_SIZE> + HasParams<S, PARAMS, BATCH_SIZE>
 {
     /// This is the actual Lie Group implementation
     type G: IsLieGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
     /// Lie Group implementation with generic scalar, real scalar, and dual scalar
     type GenG<S2: IsScalar<BATCH_SIZE>>: IsLieGroupImpl<S2, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
     /// Lie Group implementation- with real scalar
-    type RealG: IsLieGroupImpl<f64, DOF, PARAMS, POINT, AMBIENT, 1>;
+    type RealG: IsLieGroupImpl<S::RealScalar, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
     /// Lie Group implementation with dual scalar - for automatic differentiation
-    type DualG: IsLieGroupImpl<Dual, DOF, PARAMS, POINT, AMBIENT, 1>;
+    type DualG: IsLieGroupImpl<S::DualScalar, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
+
+    /// degree of freedom
+    const DOF: usize;
+    /// number of parameters
+    const PARAMS: usize;
+    /// point dimension
+    const POINT: usize;
+    /// ambient dimension
+    const AMBIENT: usize;
 
     /// Get the Lie Group
     type GenGroup<S2: IsScalar<BATCH_SIZE>, G2: IsLieGroupImpl<S2, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>>: IsLieGroup<
         S2,
         DOF,
         PARAMS,
         POINT,
         AMBIENT,
         BATCH_SIZE
     >;
     /// Lie Group with real scalar
-    type RealGroup: IsLieGroup<f64, DOF, PARAMS, POINT, AMBIENT, 1>;
+    type RealGroup: IsLieGroup<S::RealScalar, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
     /// Lie Group with dual scalar - for automatic differentiation
-    type DualGroup: IsLieGroup<Dual, DOF, PARAMS, POINT, AMBIENT, 1>;
+    type DualGroup: IsLieGroup<S::DualScalar, DOF, PARAMS, POINT, AMBIENT, BATCH_SIZE>;
 }
 
 /// Lie Group trait for real scalar, f64
 pub trait IsTranslationProductGroup<
     S: IsScalar<BATCH_SIZE>,
     const DOF: usize,
     const PARAMS: usize,
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_lie/src/translation_product_product.rs` & `sophus_pyo3-0.6.0/crates/sophus_lie/src/groups/translation_product_product.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,102 @@
-use std::vec;
-
-use super::lie_group::LieGroup;
-use super::traits::IsF64LieFactorGroupImpl;
-use super::traits::IsF64LieGroupImpl;
-use super::traits::IsLieFactorGroupImpl;
-
-use super::traits::IsLieGroupImpl;
-use super::traits::IsTranslationProductGroup;
-use sophus_calculus::dual::dual_scalar::Dual;
-use sophus_calculus::manifold;
-use sophus_calculus::points::example_points;
-use sophus_calculus::types::matrix::IsMatrix;
-use sophus_calculus::types::params::HasParams;
-use sophus_calculus::types::params::ParamsImpl;
-use sophus_calculus::types::scalar::IsScalar;
-use sophus_calculus::types::vector::IsVector;
-use sophus_calculus::types::vector::IsVectorLike;
-use sophus_calculus::types::MatF64;
-use sophus_calculus::types::VecF64;
+use crate::lie_group::LieGroup;
+use crate::prelude::*;
+use crate::traits::IsLieFactorGroupImpl;
+use crate::traits::IsLieGroupImpl;
+use crate::traits::IsRealLieFactorGroupImpl;
+use crate::traits::IsRealLieGroupImpl;
+use sophus_core::manifold::traits::TangentImpl;
+use sophus_core::params::ParamsImpl;
+use sophus_core::points::example_points;
 
 /// implementation of a translation product group
 ///
 /// It is a semi-direct product of the commutative translation group (Euclidean vector space) and a factor group.
-#[derive(Debug, Copy, Clone)]
+#[derive(Debug, Copy, Clone, Default)]
 pub struct TranslationProductGroupImpl<
-    S: IsScalar<1>,
+    S: IsScalar<BATCH>,
     const DOF: usize,
     const PARAMS: usize,
     const POINT: usize,
     const AMBIENT: usize,
     const SDOF: usize,
     const SPARAMS: usize,
-    F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, 1>,
+    const BATCH: usize,
+    F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
 > {
     phantom: std::marker::PhantomData<(S, F)>,
 }
 
 impl<
-        S: IsScalar<1>,
+        S: IsScalar<BATCH>,
         const DOF: usize,
         const PARAMS: usize,
         const POINT: usize,
         const AMBIENT: usize,
         const SDOF: usize,
         const SPARAMS: usize,
-        F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, 1>,
-    > TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, F>
+        const BATCH: usize,
+        F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
+    > TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, BATCH, F>
 {
     /// translation part of the group parameters
     pub fn translation(params: &S::Vector<PARAMS>) -> S::Vector<POINT> {
-        params.get_fixed_rows::<POINT>(0)
+        params.get_fixed_subvec::<POINT>(0)
     }
 
     /// factor part of the group parameters
     pub fn factor_params(params: &S::Vector<PARAMS>) -> S::Vector<SPARAMS> {
-        params.get_fixed_rows::<SPARAMS>(POINT)
+        params.get_fixed_subvec::<SPARAMS>(POINT)
     }
 
     /// create group parameters from translation and factor parameters
     pub fn params_from(
         translation: &S::Vector<POINT>,
         factor_params: &S::Vector<SPARAMS>,
     ) -> S::Vector<PARAMS> {
         S::Vector::block_vec2(translation.clone(), factor_params.clone())
     }
 
     /// translation part of the tangent vector
     fn translation_tangent(tangent: &S::Vector<DOF>) -> S::Vector<POINT> {
-        tangent.get_fixed_rows::<POINT>(0)
+        tangent.get_fixed_subvec::<POINT>(0)
     }
 
     /// factor part of the tangent vector
     fn factor_tangent(tangent: &S::Vector<DOF>) -> S::Vector<SDOF> {
-        tangent.get_fixed_rows::<SDOF>(POINT)
+        tangent.get_fixed_subvec::<SDOF>(POINT)
     }
 
     /// create tangent vector from translation and factor tangent
     fn tangent_from(
         translation: &S::Vector<POINT>,
         factor_tangent: &S::Vector<SDOF>,
     ) -> S::Vector<DOF> {
         S::Vector::block_vec2(translation.clone(), factor_tangent.clone())
     }
 
     fn translation_examples() -> Vec<S::Vector<POINT>> {
-        example_points::<S, POINT>()
+        example_points::<S, POINT, BATCH>()
     }
 }
 
 impl<
-        S: IsScalar<1>,
+        S: IsScalar<BATCH>,
         const DOF: usize,
         const PARAMS: usize,
         const POINT: usize,
         const AMBIENT: usize,
         const SDOF: usize,
         const SPARAMS: usize,
-        F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, 1>,
-    > ParamsImpl<S, PARAMS, 1>
-    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, F>
+        const BATCH: usize,
+        F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
+    > ParamsImpl<S, PARAMS, BATCH>
+    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, BATCH, F>
 {
-    fn are_params_valid(params: &S::Vector<PARAMS>) -> bool {
+    fn are_params_valid(params: &S::Vector<PARAMS>) -> S::Mask {
         F::are_params_valid(&Self::factor_params(params))
     }
 
     fn params_examples() -> Vec<S::Vector<PARAMS>> {
         let mut examples = vec![];
         for factor_params in F::params_examples() {
             for translation in Self::translation_examples() {
@@ -112,80 +104,80 @@
             }
         }
         examples
     }
 
     fn invalid_params_examples() -> Vec<S::Vector<PARAMS>> {
         vec![Self::params_from(
-            &S::Vector::zero(),
+            &S::Vector::zeros(),
             &F::invalid_params_examples()[0],
         )]
     }
 }
 
 impl<
-        S: IsScalar<1>,
+        S: IsScalar<BATCH>,
         const DOF: usize,
         const PARAMS: usize,
         const POINT: usize,
         const AMBIENT: usize,
         const SDOF: usize,
         const SPARAMS: usize,
-        F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, 1>,
-    > manifold::traits::TangentImpl<S, DOF, 1>
-    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, F>
+        const BATCH: usize,
+        F: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
+    > TangentImpl<S, DOF, BATCH>
+    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, BATCH, F>
 {
     fn tangent_examples() -> Vec<S::Vector<DOF>> {
         let mut examples = vec![];
         for group_tangent in F::tangent_examples() {
             for translation_tangent in Self::translation_examples() {
                 examples.push(Self::tangent_from(&translation_tangent, &group_tangent));
             }
         }
         examples
     }
 }
 
-// TODO : Port to Rust
-
 impl<
-        S: IsScalar<1>,
+        S: IsScalar<BATCH>,
         const DOF: usize,
         const PARAMS: usize,
         const POINT: usize,
         const AMBIENT: usize,
         const SDOF: usize,
         const SPARAMS: usize,
-        Factor: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, 1>,
-    > IsLieGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, 1>
-    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, Factor>
+        const BATCH: usize,
+        Factor: IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
+    > IsLieGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, BATCH>
+    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, BATCH, Factor>
 {
     const IS_ORIGIN_PRESERVING: bool = false;
     const IS_AXIS_DIRECTION_PRESERVING: bool = Factor::IS_AXIS_DIRECTION_PRESERVING;
     const IS_DIRECTION_VECTOR_PRESERVING: bool = Factor::IS_DIRECTION_VECTOR_PRESERVING;
     const IS_SHAPE_PRESERVING: bool = Factor::IS_SHAPE_PRESERVING;
     const IS_DISTANCE_PRESERVING: bool = Factor::IS_DISTANCE_PRESERVING;
     const IS_PARALLEL_LINE_PRESERVING: bool = true;
 
     fn identity_params() -> S::Vector<PARAMS> {
-        Self::params_from(&S::Vector::zero(), &Factor::identity_params())
+        Self::params_from(&S::Vector::zeros(), &Factor::identity_params())
     }
 
     //    Manifold / Lie Group concepts
 
     fn adj(params: &S::Vector<PARAMS>) -> S::Matrix<DOF, DOF> {
         let factor_params = Self::factor_params(params);
         let translation = Self::translation(params);
 
         S::Matrix::block_mat2x2::<POINT, SDOF, POINT, SDOF>(
             (
                 Factor::matrix(&factor_params),
                 Factor::adj_of_translation(&factor_params, &translation),
             ),
-            (S::Matrix::zero(), Factor::adj(&factor_params)),
+            (S::Matrix::zeros(), Factor::adj(&factor_params)),
         )
     }
 
     fn exp(omega: &S::Vector<DOF>) -> S::Vector<PARAMS> {
         let translation = Self::translation_tangent(omega);
         let factor_params = Factor::exp(&Self::factor_tangent(omega));
 
@@ -207,15 +199,15 @@
 
     fn hat(omega: &S::Vector<DOF>) -> S::Matrix<AMBIENT, AMBIENT> {
         S::Matrix::block_mat2x2::<POINT, 1, POINT, 1>(
             (
                 Factor::hat(&Self::factor_tangent(omega)),
                 Self::translation_tangent(omega).to_mat(),
             ),
-            (S::Matrix::zero(), S::Matrix::zero()),
+            (S::Matrix::zeros(), S::Matrix::zeros()),
         )
     }
 
     fn vee(hat: &S::Matrix<AMBIENT, AMBIENT>) -> S::Vector<DOF> {
         let factor_tangent = Factor::vee(&hat.get_fixed_submat::<POINT, POINT>(0, 0));
         let translation_tangent = hat.get_fixed_submat::<POINT, 1>(0, POINT);
         Self::tangent_from(&translation_tangent.get_col_vec(0), &factor_tangent)
@@ -245,15 +237,15 @@
     fn transform(params: &S::Vector<PARAMS>, point: &S::Vector<POINT>) -> S::Vector<POINT> {
         let factor_params = Self::factor_params(params);
         let translation = Self::translation(params);
         Factor::transform(&factor_params, point) + translation
     }
 
     fn to_ambient(params: &S::Vector<POINT>) -> S::Vector<AMBIENT> {
-        S::Vector::block_vec2(params.clone(), S::Vector::<1>::zero())
+        S::Vector::block_vec2(params.clone(), S::Vector::<1>::zeros())
     }
 
     fn compact(params: &S::Vector<PARAMS>) -> S::Matrix<POINT, AMBIENT> {
         S::Matrix::block_mat1x2::<POINT, 1>(
             Factor::matrix(&Self::factor_params(params)),
             Self::translation(params).to_mat(),
         )
@@ -261,229 +253,260 @@
 
     fn matrix(params: &S::Vector<PARAMS>) -> S::Matrix<AMBIENT, AMBIENT> {
         S::Matrix::block_mat2x2::<POINT, 1, POINT, 1>(
             (
                 Factor::matrix(&Self::factor_params(params)),
                 Self::translation(params).to_mat(),
             ),
-            (S::Matrix::<1, POINT>::zero(), S::Matrix::<1, 1>::identity()),
+            (
+                S::Matrix::<1, POINT>::zeros(),
+                S::Matrix::<1, 1>::identity(),
+            ),
         )
     }
 
     fn ad(tangent: &S::Vector<DOF>) -> S::Matrix<DOF, DOF> {
-        let o = S::Matrix::<SDOF, POINT>::zero();
+        let o = S::Matrix::<SDOF, POINT>::zeros();
         S::Matrix::block_mat2x2::<POINT, SDOF, POINT, SDOF>(
             (
                 Factor::hat(&Self::factor_tangent(tangent)),
                 Factor::ad_of_translation(&Self::translation_tangent(tangent)),
             ),
             (o, Factor::ad(&Self::factor_tangent(tangent))),
         )
     }
 
-    type GenG<S2: IsScalar<1>> = TranslationProductGroupImpl<
+    type GenG<S2: IsScalar<BATCH>> = TranslationProductGroupImpl<
         S2,
         DOF,
         PARAMS,
         POINT,
         AMBIENT,
         SDOF,
         SPARAMS,
+        BATCH,
         Factor::GenFactorG<S2>,
     >;
 
     type RealG = TranslationProductGroupImpl<
-        f64,
+        S::RealScalar,
         DOF,
         PARAMS,
         POINT,
         AMBIENT,
         SDOF,
         SPARAMS,
-        Factor::GenFactorG<f64>,
+        BATCH,
+        Factor::GenFactorG<S::RealScalar>,
     >;
 
     type DualG = TranslationProductGroupImpl<
-        Dual,
+        S::DualScalar,
         DOF,
         PARAMS,
         POINT,
         AMBIENT,
         SDOF,
         SPARAMS,
-        Factor::GenFactorG<Dual>,
+        BATCH,
+        Factor::GenFactorG<S::DualScalar>,
     >;
-
-    fn has_shortest_path_ambiguity(params: &<S as IsScalar<1>>::Vector<PARAMS>) -> bool {
-        Factor::has_shortest_path_ambiguity(&Self::factor_params(params))
-    }
 }
 
 impl<
+        S: IsRealScalar<BATCH>,
         const DOF: usize,
         const PARAMS: usize,
         const POINT: usize,
         const AMBIENT: usize,
         const SDOF: usize,
         const SPARAMS: usize,
-        Factor: IsF64LieFactorGroupImpl<SDOF, SPARAMS, POINT>,
-    > IsF64LieGroupImpl<DOF, PARAMS, POINT, AMBIENT>
-    for TranslationProductGroupImpl<f64, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, Factor>
+        const BATCH: usize,
+        Factor: IsRealLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
+    > IsRealLieGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, BATCH>
+    for TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, BATCH, Factor>
 {
-    fn dx_exp_x_at_0() -> MatF64<PARAMS, DOF> {
-        MatF64::block_mat2x2::<POINT, SPARAMS, POINT, SDOF>(
+    fn dx_exp_x_at_0() -> S::Matrix<PARAMS, DOF> {
+        S::Matrix::block_mat2x2::<POINT, SPARAMS, POINT, SDOF>(
+            (
+                S::Matrix::<POINT, POINT>::identity(),
+                S::Matrix::<POINT, SDOF>::zeros(),
+            ),
             (
-                MatF64::<POINT, POINT>::identity(),
-                MatF64::<POINT, SDOF>::zero(),
+                S::Matrix::<SPARAMS, POINT>::zeros(),
+                Factor::dx_exp_x_at_0(),
             ),
-            (MatF64::<SPARAMS, POINT>::zero(), Factor::dx_exp_x_at_0()),
         )
     }
 
-    fn dx_exp_x_times_point_at_0(point: VecF64<POINT>) -> MatF64<POINT, DOF> {
-        MatF64::block_mat1x2(
-            MatF64::<POINT, POINT>::identity(),
+    fn dx_exp_x_times_point_at_0(point: S::Vector<POINT>) -> S::Matrix<POINT, DOF> {
+        S::Matrix::block_mat1x2(
+            S::Matrix::<POINT, POINT>::identity(),
             Factor::dx_exp_x_times_point_at_0(point),
         )
     }
 
-    fn dx_exp(tangent: &VecF64<DOF>) -> MatF64<PARAMS, DOF> {
+    fn dx_exp(tangent: &S::Vector<DOF>) -> S::Matrix<PARAMS, DOF> {
         let factor_tangent = &Self::factor_tangent(tangent);
         let trans_tangent = &Self::translation_tangent(tangent);
 
         let dx_mat_v = Factor::dx_mat_v(factor_tangent);
-        let mut dx_mat_v_tangent = MatF64::<POINT, SDOF>::zero();
+        let mut dx_mat_v_tangent = S::Matrix::<POINT, SDOF>::zeros();
 
         for i in 0..SDOF {
-            dx_mat_v_tangent
-                .fixed_columns_mut::<1>(i)
-                .copy_from(&(dx_mat_v[i] * trans_tangent));
+            dx_mat_v_tangent.set_col_vec(i, dx_mat_v[i].clone() * trans_tangent.clone());
         }
 
-        MatF64::block_mat2x2::<POINT, SPARAMS, POINT, SDOF>(
+        S::Matrix::block_mat2x2::<POINT, SPARAMS, POINT, SDOF>(
             (Factor::mat_v(factor_tangent), dx_mat_v_tangent),
             (
-                MatF64::<SPARAMS, POINT>::zero(),
+                S::Matrix::<SPARAMS, POINT>::zeros(),
                 Factor::dx_exp(factor_tangent),
             ),
         )
     }
 
-    fn dx_log_x(params: &VecF64<PARAMS>) -> MatF64<DOF, PARAMS> {
+    fn dx_log_x(params: &S::Vector<PARAMS>) -> S::Matrix<DOF, PARAMS> {
         let factor_params = &Self::factor_params(params);
         let trans = &Self::translation(params);
         let factor_tangent = Factor::log(factor_params);
 
         let dx_log_x = Factor::dx_log_x(factor_params);
         let dx_mat_v_inverse = Factor::dx_mat_v_inverse(&factor_tangent);
 
-        let mut dx_mat_v_inv_tangent = MatF64::<POINT, SPARAMS>::zero();
+        let mut dx_mat_v_inv_tangent = S::Matrix::<POINT, SPARAMS>::zeros();
 
         for i in 0..SDOF {
-            let v = dx_mat_v_inverse[i] * trans;
-            let r = dx_log_x.row(i);
-            dx_mat_v_inv_tangent += v * r;
+            let v: S::Vector<POINT> = dx_mat_v_inverse[i].clone() * trans.clone();
+            let r: S::Vector<SPARAMS> = dx_log_x.get_row_vec(i);
+
+            let m = v.outer(r);
+            dx_mat_v_inv_tangent = dx_mat_v_inv_tangent + m;
         }
 
-        MatF64::block_mat2x2::<POINT, SDOF, POINT, SPARAMS>(
+        S::Matrix::block_mat2x2::<POINT, SDOF, POINT, SPARAMS>(
             (Factor::mat_v_inverse(&factor_tangent), dx_mat_v_inv_tangent),
-            (MatF64::<SDOF, POINT>::zero(), dx_log_x),
+            (S::Matrix::<SDOF, POINT>::zeros(), dx_log_x),
         )
     }
 
-    fn da_a_mul_b(a: &VecF64<PARAMS>, b: &VecF64<PARAMS>) -> MatF64<PARAMS, PARAMS> {
+    fn da_a_mul_b(a: &S::Vector<PARAMS>, b: &S::Vector<PARAMS>) -> S::Matrix<PARAMS, PARAMS> {
         let a_factor_params = &Self::factor_params(a);
         let b_factor_params = &Self::factor_params(b);
 
         let b_trans = &Self::translation(b);
 
-        MatF64::block_mat2x2::<POINT, SPARAMS, POINT, SPARAMS>(
+        S::Matrix::block_mat2x2::<POINT, SPARAMS, POINT, SPARAMS>(
             (
-                MatF64::<POINT, POINT>::identity(),
+                S::Matrix::<POINT, POINT>::identity(),
                 Factor::dparams_matrix_times_point(a_factor_params, b_trans),
             ),
             (
-                MatF64::<SPARAMS, POINT>::zero(),
+                S::Matrix::<SPARAMS, POINT>::zeros(),
                 Factor::da_a_mul_b(a_factor_params, b_factor_params),
             ),
         )
     }
 
-    fn db_a_mul_b(a: &VecF64<PARAMS>, b: &VecF64<PARAMS>) -> MatF64<PARAMS, PARAMS> {
+    fn db_a_mul_b(a: &S::Vector<PARAMS>, b: &S::Vector<PARAMS>) -> S::Matrix<PARAMS, PARAMS> {
         let a_factor_params = &Self::factor_params(a);
         let b_factor_params = &Self::factor_params(b);
 
-        MatF64::block_mat2x2::<POINT, SPARAMS, POINT, SPARAMS>(
+        S::Matrix::block_mat2x2::<POINT, SPARAMS, POINT, SPARAMS>(
             (
                 Factor::matrix(a_factor_params),
-                MatF64::<POINT, SPARAMS>::zero(),
+                S::Matrix::<POINT, SPARAMS>::zeros(),
             ),
             (
-                MatF64::<SPARAMS, POINT>::zero(),
+                S::Matrix::<SPARAMS, POINT>::zeros(),
                 Factor::db_a_mul_b(a_factor_params, b_factor_params),
             ),
         )
     }
+
+    fn has_shortest_path_ambiguity(params: &<S>::Vector<PARAMS>) -> <S>::Mask {
+        Factor::has_shortest_path_ambiguity(&Self::factor_params(params))
+    }
 }
 
 impl<
-        S: IsScalar<1>,
+        S: IsScalar<BATCH>,
         const DOF: usize,
         const PARAMS: usize,
         const POINT: usize,
         const AMBIENT: usize,
         const SDOF: usize,
         const SPARAMS: usize,
-        FactorImpl: crate::traits::IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, 1>,
+        const BATCH: usize,
+        FactorImpl: crate::traits::IsLieFactorGroupImpl<S, SDOF, SPARAMS, POINT, BATCH>,
     >
     IsTranslationProductGroup<
         S,
         DOF,
         PARAMS,
         POINT,
         AMBIENT,
         SDOF,
         SPARAMS,
-        1,
-        LieGroup<S, SDOF, SPARAMS, POINT, POINT, 1, FactorImpl>,
+        BATCH,
+        LieGroup<S, SDOF, SPARAMS, POINT, POINT, BATCH, FactorImpl>,
     >
     for crate::lie_group::LieGroup<
         S,
         DOF,
         PARAMS,
         POINT,
         AMBIENT,
-        1,
-        TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, FactorImpl>,
+        BATCH,
+        TranslationProductGroupImpl<
+            S,
+            DOF,
+            PARAMS,
+            POINT,
+            AMBIENT,
+            SDOF,
+            SPARAMS,
+            BATCH,
+            FactorImpl,
+        >,
     >
 {
-    type Impl =
-        TranslationProductGroupImpl<S, DOF, PARAMS, POINT, AMBIENT, SDOF, SPARAMS, FactorImpl>;
+    type Impl = TranslationProductGroupImpl<
+        S,
+        DOF,
+        PARAMS,
+        POINT,
+        AMBIENT,
+        SDOF,
+        SPARAMS,
+        BATCH,
+        FactorImpl,
+    >;
 
     fn from_translation_and_factor(
-        translation: &<S as IsScalar<1>>::Vector<POINT>,
-        factor: &LieGroup<S, SDOF, SPARAMS, POINT, POINT, 1, FactorImpl>,
+        translation: &<S as IsScalar<BATCH>>::Vector<POINT>,
+        factor: &LieGroup<S, SDOF, SPARAMS, POINT, POINT, BATCH, FactorImpl>,
     ) -> Self {
         let params = Self::Impl::params_from(translation, factor.params());
         Self::from_params(&params)
     }
 
-    fn from_t(translation: &<S as IsScalar<1>>::Vector<POINT>) -> Self {
+    fn from_t(translation: &<S as IsScalar<BATCH>>::Vector<POINT>) -> Self {
         Self::from_translation_and_factor(translation, &LieGroup::identity())
     }
 
-    fn set_translation(&mut self, translation: &<S as IsScalar<1>>::Vector<POINT>) {
+    fn set_translation(&mut self, translation: &<S as IsScalar<BATCH>>::Vector<POINT>) {
         self.set_params(&Self::G::params_from(translation, self.factor().params()))
     }
 
-    fn translation(&self) -> <S as IsScalar<1>>::Vector<POINT> {
+    fn translation(&self) -> <S as IsScalar<BATCH>>::Vector<POINT> {
         Self::Impl::translation(self.params())
     }
 
-    fn set_factor(&mut self, factor: &LieGroup<S, SDOF, SPARAMS, POINT, POINT, 1, FactorImpl>) {
+    fn set_factor(&mut self, factor: &LieGroup<S, SDOF, SPARAMS, POINT, POINT, BATCH, FactorImpl>) {
         self.set_params(&Self::G::params_from(&self.translation(), factor.params()))
     }
 
-    fn factor(&self) -> LieGroup<S, SDOF, SPARAMS, POINT, POINT, 1, FactorImpl> {
+    fn factor(&self) -> LieGroup<S, SDOF, SPARAMS, POINT, POINT, BATCH, FactorImpl> {
         LieGroup::from_params(&Self::Impl::factor_params(self.params()))
     }
 }
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_tensor/src/mut_tensor.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,30 @@
-use crate::arc_tensor::ArcTensor;
-use crate::element::BatchMat;
-use crate::element::BatchScalar;
-use crate::element::BatchVec;
-use crate::element::IsStaticTensor;
-use crate::element::IsTensorScalar;
-use crate::element::SMat;
-use crate::element::SVec;
-use crate::mut_view::IsMutTensorLike;
-use crate::mut_view::MutTensorView;
-use crate::view::IsTensorLike;
-use crate::view::IsTensorView;
-use crate::view::TensorView;
-
+use crate::linalg::SMat;
+use crate::linalg::SVec;
+use crate::prelude::*;
+use crate::tensor::ArcTensor;
+use crate::tensor::MutTensorView;
+use crate::tensor::TensorView;
 use ndarray::Dim;
 use ndarray::Ix;
 use std::fmt::Debug;
 use std::marker::PhantomData;
 
 /// mutable tensor
 ///
 /// See TensorView for more details of the tensor structure
 #[derive(Default, Debug, Clone)]
 pub struct MutTensor<
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
-    Scalar: IsTensorScalar + 'static,
-    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS, BATCH_SIZE> + 'static,
+    Scalar: IsCoreScalar + 'static,
+    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS> + 'static,
     const ROWS: usize,
     const COLS: usize,
-    const BATCH_SIZE: usize,
 > where
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
 {
     /// ndarray of the static tensors with shape [D1, D2, ...]
     pub mut_array: ndarray::Array<STensor, Dim<[Ix; DRANK]>>,
     /// phantom data
     pub phantom: PhantomData<(Scalar, STensor)>,
@@ -42,18 +33,18 @@
 /// Converting a tensor of vectors to a tensor of Rx1 matrices
 pub trait InnerVecToMat<
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     const HYBER_RANK_PLUS1: usize,
     const SRANK_PLUS1: usize,
-    Scalar: IsTensorScalar + 'static,
+    Scalar: IsCoreScalar + 'static,
     const ROWS: usize,
 > where
-    SVec<Scalar, ROWS>: IsStaticTensor<Scalar, SRANK_PLUS1, ROWS, 1, 1>,
+    SVec<Scalar, ROWS>: IsStaticTensor<Scalar, SRANK_PLUS1, ROWS, 1>,
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
 {
     /// The output tensor
     type Output;
 
     /// Convert to a tensor of Rx1 matrices
     fn inner_vec_to_mat(self) -> Self::Output;
@@ -62,166 +53,124 @@
 /// Converting a tensor of scalars to a tensor of 1-vectors
 pub trait InnerScalarToVec<
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     const HYBER_RANK_PLUS1: usize,
     const SRANK_PLUS1: usize,
-    Scalar: IsTensorScalar + 'static,
+    Scalar: IsCoreScalar + 'static,
 > where
-    SVec<Scalar, 1>: IsStaticTensor<Scalar, SRANK_PLUS1, 1, 1, 1>,
+    SVec<Scalar, 1>: IsStaticTensor<Scalar, SRANK_PLUS1, 1, 1>,
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
 {
     /// The output tensor
     type Output;
 
     /// Convert to a tensor of 1-vectors
     fn inner_scalar_to_vec(self) -> Self::Output;
 }
 
-impl<Scalar: IsTensorScalar + 'static, const ROWS: usize> InnerVecToMat<3, 1, 2, 4, 2, Scalar, ROWS>
+impl<Scalar: IsCoreScalar + 'static, const ROWS: usize> InnerVecToMat<3, 1, 2, 4, 2, Scalar, ROWS>
     for MutTensorXR<3, 2, 1, Scalar, ROWS>
 {
     type Output = MutTensorXRC<4, 2, 2, Scalar, ROWS, 1>;
 
     fn inner_vec_to_mat(self) -> MutTensorXRC<4, 2, 2, Scalar, ROWS, 1> {
         MutTensorXRC::<4, 2, 2, Scalar, ROWS, 1> {
             mut_array: self.mut_array,
             phantom: PhantomData,
         }
     }
 }
 
-impl<Scalar: IsTensorScalar + 'static> InnerScalarToVec<2, 0, 2, 3, 1, Scalar>
+impl<Scalar: IsCoreScalar + 'static> InnerScalarToVec<2, 0, 2, 3, 1, Scalar>
     for MutTensorX<2, Scalar>
 {
     type Output = MutTensorXR<3, 2, 1, Scalar, 1>;
 
     fn inner_scalar_to_vec(self) -> MutTensorXR<3, 2, 1, Scalar, 1> {
         MutTensorXR::<3, 2, 1, Scalar, 1> {
-            mut_array: self.mut_array.map(|x| SVec::<Scalar, 1>::new(*x)),
+            mut_array: self.mut_array.map(|x| SVec::<Scalar, 1>::new(x.clone())),
             phantom: PhantomData,
         }
     }
 }
 
 /// Mutable tensor of scalars
-pub type MutTensorX<const DRANK: usize, Scalar> =
-    MutTensor<DRANK, DRANK, 0, Scalar, Scalar, 1, 1, 1>;
-
-/// Mutable tensor of batched scalars
-pub type MutTensorXB<
-    const TOTAL_RANK: usize,
-    const DRANK: usize,
-    const SRANK: usize,
-    Scalar,
-    const B: usize,
-> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, BatchScalar<Scalar, B>, 1, 1, B>;
+pub type MutTensorX<const DRANK: usize, Scalar> = MutTensor<DRANK, DRANK, 0, Scalar, Scalar, 1, 1>;
 
 /// Mutable tensor of vectors with shape R
 pub type MutTensorXR<
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     Scalar,
     const R: usize,
-> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, SVec<Scalar, R>, R, 1, 1>;
-
-/// Mutable tensor of batched vectors with shape [R x B]
-pub type MutTensorXRB<
-    const TOTAL_RANK: usize,
-    const DRANK: usize,
-    const SRANK: usize,
-    Scalar,
-    const R: usize,
-    const B: usize,
-> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, BatchVec<Scalar, R, B>, R, 1, B>;
+> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, SVec<Scalar, R>, R, 1>;
 
 /// Mutable tensor of matrices with shape [R x C]
 pub type MutTensorXRC<
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     Scalar,
     const R: usize,
     const C: usize,
-> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, SMat<Scalar, R, C>, R, C, 1>;
-
-/// Mutable tensor of batched matrices with shape [R x C x B]
-pub type MutTensorXRCB<
-    const TOTAL_RANK: usize,
-    const DRANK: usize,
-    const SRANK: usize,
-    Scalar,
-    const R: usize,
-    const C: usize,
-    const B: usize,
-> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, BatchMat<Scalar, R, C, B>, R, C, B>;
+> = MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, SMat<Scalar, R, C>, R, C>;
 
 /// rank-1 mutable tensor of scalars with shape D0
 pub type MutTensorD<Scalar> = MutTensorX<1, Scalar>;
 
 /// rank-2 mutable tensor of scalars with shape [D0 x D1]
 pub type MutTensorDD<Scalar> = MutTensorX<2, Scalar>;
 
-/// rank-2 mutable tensor of batched scalars with shape [D0 x B]
-pub type MutTensorDB<Scalar, const B: usize> = MutTensorXB<2, 1, 1, Scalar, B>;
-
 /// rank-2 mutable tensor of vectors with shape [D0 x R]
 pub type MutTensorDR<Scalar, const R: usize> = MutTensorXR<2, 1, 1, Scalar, R>;
 
 /// rank-3 mutable tensor of scalars with shape [D0 x D1 x D2]
 pub type MutTensorDDD<Scalar> = MutTensorX<3, Scalar>;
 
-/// rank-3 mutable tensor of batched scalars with shape [D0 x D1 x B]
-pub type MutTensorDDB<Scalar, const B: usize> = MutTensorXB<3, 2, 1, Scalar, B>;
-
 /// rank-3 mutable tensor of vectors with shape [D0 x D1 x R]
 pub type MutTensorDDR<Scalar, const R: usize> = MutTensorXR<3, 2, 1, Scalar, R>;
 
-/// rank-3 mutable tensor of batched vectors with shape [D0 x R x B]
-pub type MutTensorDRB<Scalar, const R: usize, const B: usize> = MutTensorXRB<3, 1, 2, Scalar, R, B>;
-
 /// rank-3 mutable tensor of matrices with shape [D0 x R x C]
 pub type MutTensorDRC<Scalar, const R: usize, const C: usize> = MutTensorXRC<3, 1, 2, Scalar, R, C>;
 
 /// rank-4 mutable tensor of scalars with shape [D0 x D1 x D2 x D3]
 pub type MutTensorDDDD<Scalar> = MutTensorX<4, Scalar>;
 
-/// rank-4 mutable tensor of batched scalars with shape [D0 x D1 x D2 x B]
-pub type MutTensorDDDB<Scalar, const B: usize> = MutTensorXB<4, 3, 1, Scalar, B>;
-
 /// rank-4 mutable tensor of vectors with shape [D0 x D1 x D2 x R]
 pub type MutTensorDDDR<Scalar, const R: usize> = MutTensorXR<4, 3, 1, Scalar, R>;
 
-/// rank-4 mutable tensor of batched vectors with shape [D0 x D1 x R x B]
-pub type MutTensorDDRB<Scalar, const R: usize, const B: usize> =
-    MutTensorXRB<4, 2, 2, Scalar, R, B>;
-
-/// rank-4 mutable tensor of matrices with shape [D0 x R x C x B]
+/// rank-4 mutable tensor of matrices with shape [D0 x D1 x R x C]
 pub type MutTensorDDRC<Scalar, const R: usize, const C: usize> =
     MutTensorXRC<4, 2, 2, Scalar, R, C>;
 
-/// rank-4 mutable tensor of batched matrices with shape [D0 x R x C x B]
-pub type MutTensorDRCB<Scalar, const R: usize, const C: usize, const B: usize> =
-    MutTensorXRCB<4, 1, 3, Scalar, R, C, B>;
+/// rank-5 mutable tensor of scalars with shape [D0 x D1 x D2 x D3 x D4]
+pub type MutTensorDDDDD<Scalar> = MutTensorX<5, Scalar>;
+
+/// rank-5 mutable tensor of vectors with shape [D0 x D1 x D2 x D3 x R]
+pub type MutTensorDDDDR<Scalar, const R: usize> = MutTensorXR<5, 4, 1, Scalar, R>;
+
+/// rank-5 mutable tensor of matrices with shape [D0 x D1 x D2 x R x C]
+pub type MutTensorDDDRC<Scalar, const R: usize, const C: usize> =
+    MutTensorXRC<5, 3, 2, Scalar, R, C>;
 
 macro_rules! mut_tensor_is_view {
     ($scalar_rank:literal, $srank:literal, $drank:literal) => {
 
 
         impl<
         'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
-            > IsTensorLike<'a, $scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS, BATCH_SIZE>
-            for MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS, BATCH_SIZE>
+            > IsTensorLike<'a, $scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS>
+            for MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS>
         {
             fn elem_view<'b:'a>(
                 &'b self,
             ) -> ndarray::ArrayView<'a, STensor, ndarray::Dim<[ndarray::Ix; $drank]>> {
                 self.view().elem_view
             }
 
@@ -245,36 +194,36 @@
 
             fn scalar_dims(&self) -> [usize; $scalar_rank] {
                 self.view().scalar_dims()
             }
 
             fn to_mut_tensor(
                 &self,
-            ) -> MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS, BATCH_SIZE> {
+            ) -> MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS> {
                 MutTensor {
                     mut_array: self.elem_view().to_owned(),
                     phantom: PhantomData::default(),
                 }
             }
         }
 
         impl<
         'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
+
             >
             IsMutTensorLike<'a,
                 $scalar_rank, $drank, $srank,
                 Scalar, STensor,
-                ROWS, COLS, BATCH_SIZE
+                ROWS, COLS
             >
-            for MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            for MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
             fn elem_view_mut<'b:'a>(
                 &'b mut self,
             ) -> ndarray::ArrayViewMut<'a, STensor, ndarray::Dim<[ndarray::Ix; $drank]>>{
                 self.mut_view().elem_view_mut
             }
             fn get_mut(& mut self, idx: [usize; $drank]) -> &mut STensor{
@@ -284,57 +233,130 @@
             fn scalar_view_mut<'b:'a>(
                 &'b mut self,
             ) -> ndarray::ArrayViewMut<'a, Scalar, ndarray::Dim<[ndarray::Ix; $scalar_rank]>>{
                 self.mut_view().scalar_view_mut
             }
         }
 
-        impl<'a,  Scalar: IsTensorScalar+ 'static,
-                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS, BATCH_SIZE> + 'static,
+        impl<'a,  Scalar: IsCoreScalar+ 'static,
+        STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
+        const ROWS: usize,
+        const COLS: usize,
+
+        > PartialEq for
+            MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
+        {
+            fn eq(&self, other: &Self) -> bool {
+                self.view().scalar_view == other.view().scalar_view
+            }
+        }
+
+        impl<'a,  Scalar: IsCoreScalar+ 'static,
+                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
+
         >
-            MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
+        {
+
+            /// create a new tensor from a shape - filled with zeros
+            pub fn from_shape(size: [usize; $drank]) -> Self {
+                MutTensor::<$scalar_rank, $drank, $srank, Scalar, STensor,
+                            ROWS, COLS>::from_shape_and_val(
+                    size, num_traits::Zero::zero()
+                )
+            }
+
+             /// create a new mutable tensor by applying a binary operator to each element of two
+            /// other tensors
+            pub fn from_map2<
+                'b,
+                const OTHER_HRANK: usize, const OTHER_SRANK: usize,
+                OtherScalar: IsCoreScalar + 'static,
+                OtherSTensor: IsStaticTensor<
+                    OtherScalar, OTHER_SRANK, OTHER_ROWS, OTHER_COLS
+                > + 'static,
+                const OTHER_ROWS: usize, const OTHER_COLS: usize,
+            V : IsTensorView::<'b,
+                OTHER_HRANK, $drank, OTHER_SRANK,
+                OtherScalar, OtherSTensor,
+                OTHER_ROWS, OTHER_COLS
+            >,
+            const OTHER_HRANK2: usize, const OTHER_SRANK2: usize,
+            OtherScalar2: IsCoreScalar + 'static,
+            OtherSTensor2: IsStaticTensor<
+                OtherScalar2, OTHER_SRANK2, OTHER_ROWS2, OTHER_COLS2,
+            > + 'static,
+            const OTHER_ROWS2: usize, const OTHER_COLS2: usize,
+            V2 : IsTensorView::<'b,
+                OTHER_HRANK2, $drank, OTHER_SRANK2,
+                OtherScalar2, OtherSTensor2,
+                OTHER_ROWS2, OTHER_COLS2
+            >,
+            F: FnMut(&OtherSTensor, &OtherSTensor2)->STensor
+            >(
+                view: &'b V,
+                view2: &'b V2,
+                mut op: F,
+            )
+            -> Self
+            where
+                ndarray::Dim<[ndarray::Ix; OTHER_HRANK]>: ndarray::Dimension,
+                ndarray::Dim<[ndarray::Ix; OTHER_HRANK2]>: ndarray::Dimension
+
+            {
+                let mut out  = Self::from_shape(view.dims());
+                ndarray::Zip::from(&mut out.elem_view_mut())
+                .and(&view.elem_view())
+                .and(&view2.elem_view())
+                .for_each(
+                    |out, v, v2|{
+                      *out = op(v,v2);
+                    });
+                out
+            }
+        }
+
+        impl<'a,  Scalar: IsCoreScalar+ 'static,
+                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS> + 'static,
+                const ROWS: usize,
+                const COLS: usize,
+
+        >
+            MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
 
 
             /// returns a mutable view of the tensor
             pub fn mut_view<'b: 'a>(
                 &'b mut self,
             ) -> MutTensorView<'a,
                                $scalar_rank, $drank, $srank,
                                Scalar, STensor,
-                               ROWS, COLS, BATCH_SIZE>
+                               ROWS, COLS>
             {
                 MutTensorView::<
                     'a,
                     $scalar_rank, $drank, $srank,
-                    Scalar, STensor, ROWS, COLS, BATCH_SIZE>::new
+                    Scalar, STensor, ROWS, COLS>::new
                 (
                     self.mut_array.view_mut()
                 )
             }
 
             /// returns a view of the tensor
             pub fn view<'b: 'a>(&'b self
             ) -> TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor,
-                            ROWS, COLS, BATCH_SIZE> {
+                            ROWS, COLS> {
                 TensorView::<'a, $scalar_rank, $drank, $srank, Scalar, STensor,
-                             ROWS, COLS, BATCH_SIZE>::new(
+                             ROWS, COLS>::new(
                     self.mut_array.view())
             }
 
-            /// create a new tensor from a shape - filled with zeros
-            pub fn from_shape(size: [usize; $drank]) -> Self {
-                MutTensor::<$scalar_rank, $drank, $srank, Scalar, STensor,
-                            ROWS, COLS, BATCH_SIZE>::from_shape_and_val(
-                    size, STensor::zero()
-                )
-            }
 
             /// create a new tensor from a shape and a value
             pub fn from_shape_and_val
             (
                 shape: [usize; $drank],
                 val: STensor,
             ) -> Self
@@ -343,47 +365,47 @@
                     mut_array: ndarray::Array::<STensor, Dim<[Ix; $drank]>>::from_elem(shape, val),
                     phantom: PhantomData::default()
                 }
             }
 
             /// create a new mutable tensor by copying from another tensor
             pub fn make_copy_from(
-                v: &TensorView<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+                v: &TensorView<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
             ) -> Self
             {
                 IsTensorLike::to_mut_tensor(v)
             }
 
             /// return ArcTensor copy of the mutable tensor
             pub fn to_shared(self)
-                -> ArcTensor::<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS, BATCH_SIZE>
+                -> ArcTensor::<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS>
             {
                 ArcTensor::<
                     $scalar_rank,
                     $drank, $srank,
                     Scalar, STensor,
-                    ROWS, COLS, BATCH_SIZE>::from_mut_tensor(self)
+                    ROWS, COLS>::from_mut_tensor(self)
             }
 
             /// create a new mutable tensor by applying a unary operator to each element of another
             /// tensor
             pub fn from_map<
                 'b,
                 const OTHER_HRANK: usize, const OTHER_SRANK: usize,
-                OtherScalar: IsTensorScalar+ 'static,
+                OtherScalar: IsCoreScalar+ 'static,
                 OtherSTensor: IsStaticTensor<
                     OtherScalar, OTHER_SRANK,
-                    OTHER_ROWS, OTHER_COLS, OTHER_BATCHES
+                    OTHER_ROWS, OTHER_COLS
                 > + 'static,
-                const OTHER_ROWS: usize, const OTHER_COLS: usize, const OTHER_BATCHES: usize,
+                const OTHER_ROWS: usize, const OTHER_COLS: usize,
                 V : IsTensorView::<
                     'b,
                     OTHER_HRANK, $drank, OTHER_SRANK,
                     OtherScalar, OtherSTensor,
-                    OTHER_ROWS, OTHER_COLS, OTHER_BATCHES
+                    OTHER_ROWS, OTHER_COLS
                 >,
                 F: FnMut(&OtherSTensor)-> STensor
             > (
                 view:  &'b V,
                 op: F,
             )
             -> Self where
@@ -392,113 +414,61 @@
             {
                 Self {
                     mut_array: view.elem_view().map(op),
                     phantom: PhantomData::default()
                 }
             }
 
-            /// create a new mutable tensor by applying a binary operator to each element of two
-            /// other tensors
-            pub fn from_map2<
-                'b,
-                const OTHER_HRANK: usize, const OTHER_SRANK: usize,
-                OtherScalar: IsTensorScalar + 'static,
-                OtherSTensor: IsStaticTensor<
-                    OtherScalar, OTHER_SRANK, OTHER_ROWS, OTHER_COLS, OTHER_BATCHES
-                > + 'static,
-                const OTHER_ROWS: usize, const OTHER_COLS: usize, const OTHER_BATCHES: usize,
-            V : IsTensorView::<'b,
-                OTHER_HRANK, $drank, OTHER_SRANK,
-                OtherScalar, OtherSTensor,
-                OTHER_ROWS, OTHER_COLS, OTHER_BATCHES
-            >,
-            const OTHER_HRANK2: usize, const OTHER_SRANK2: usize,
-            OtherScalar2: IsTensorScalar + 'static,
-            OtherSTensor2: IsStaticTensor<
-                OtherScalar2, OTHER_SRANK2, OTHER_ROWS2, OTHER_COLS2, OTHER_BATCHES2,
-            > + 'static,
-            const OTHER_ROWS2: usize, const OTHER_COLS2: usize, const OTHER_BATCHES2: usize,
-            V2 : IsTensorView::<'b,
-                OTHER_HRANK2, $drank, OTHER_SRANK2,
-                OtherScalar2, OtherSTensor2,
-                OTHER_ROWS2, OTHER_COLS2, OTHER_BATCHES2
-            >,
-            F: FnMut(&OtherSTensor, &OtherSTensor2)->STensor
-            >(
-                view: &'b V,
-                view2: &'b V2,
-                mut op: F,
-            )
-            -> Self
-            where
-                ndarray::Dim<[ndarray::Ix; OTHER_HRANK]>: ndarray::Dimension,
-                ndarray::Dim<[ndarray::Ix; OTHER_HRANK2]>: ndarray::Dimension
 
-            {
-                let mut out  = Self::from_shape(view.dims());
-                ndarray::Zip::from(&mut out.elem_view_mut())
-                .and(&view.elem_view())
-                .and(&view2.elem_view())
-                .for_each(
-                    |out, v, v2|{
-                      *out = op(v,v2);
-                    });
-                out
-            }
         }
     };
 }
 
 mut_tensor_is_view!(1, 0, 1);
 mut_tensor_is_view!(2, 0, 2);
 mut_tensor_is_view!(2, 1, 1);
 mut_tensor_is_view!(3, 0, 3);
 mut_tensor_is_view!(3, 1, 2);
 mut_tensor_is_view!(3, 2, 1);
 mut_tensor_is_view!(4, 0, 4);
 mut_tensor_is_view!(4, 1, 3);
 mut_tensor_is_view!(4, 2, 2);
-mut_tensor_is_view!(4, 3, 1);
-
-#[cfg(test)]
-mod tests {
-    use simba::simd::AutoSimd;
-
-    use super::*;
-
-    #[test]
-    fn empty_image() {
-        {
-            let _rank1_tensor = MutTensorD::<u8>::default();
-            //assert!(rank1_tensor.is_empty());
-            let shape = [2];
-            let tensor_f32 = MutTensorD::from_shape_and_val(shape, 0.0);
-            //assert!(!tensor_f32.is_empty());
-            assert_eq!(tensor_f32.view().dims(), shape);
-        }
-        {
-            let _rank2_tensor = MutTensorDD::<u8>::default();
-            //assert!(rank2_tensor.is_empty());
-            let shape = [3, 2];
-            let tensor_f32 = MutTensorDD::<f32>::from_shape(shape);
-            // assert!(!tensor_f32.is_empty());
-            assert_eq!(tensor_f32.view().dims(), shape);
-        }
-        {
-            let _rank3_tensor = MutTensorDDD::<u8>::default();
-            // assert!(rank3_tensor.is_empty());
-            let shape = [3, 2, 4];
-            let tensor_f32 = MutTensorDDD::<f32>::from_shape(shape);
-            //  assert!(!tensor_f32.is_empty());
-            assert_eq!(tensor_f32.view().dims(), shape);
-        }
+mut_tensor_is_view!(5, 0, 5);
+mut_tensor_is_view!(5, 1, 4);
+mut_tensor_is_view!(5, 2, 3);
+
+#[test]
+fn mut_tensor_tests() {
+    use crate::linalg::BatchMatF64;
+    {
+        let _rank1_tensor = MutTensorD::<u8>::default();
+        //assert!(rank1_tensor.is_empty());
+        let shape = [2];
+        let tensor_f32 = MutTensorD::from_shape_and_val(shape, 0.0);
+        //assert!(!tensor_f32.is_empty());
+        assert_eq!(tensor_f32.view().dims(), shape);
     }
-
-    #[test]
-    pub fn transform() {
+    {
+        let _rank2_tensor = MutTensorDD::<u8>::default();
+        //assert!(rank2_tensor.is_empty());
+        let shape = [3, 2];
+        let tensor_f32 = MutTensorDD::<f32>::from_shape(shape);
+        // assert!(!tensor_f32.is_empty());
+        assert_eq!(tensor_f32.view().dims(), shape);
+    }
+    {
+        let _rank3_tensor = MutTensorDDD::<u8>::default();
+        // assert!(rank3_tensor.is_empty());
+        let shape = [3, 2, 4];
+        let tensor_f32 = MutTensorDDD::<f32>::from_shape(shape);
+        //  assert!(!tensor_f32.is_empty());
+        assert_eq!(tensor_f32.view().dims(), shape);
+    }
+    //transform
+    {
         let shape = [3];
         {
             let tensor_f32 = MutTensorD::from_shape_and_val(shape, 1.0);
             let op = |v: &f32| {
                 let mut value = SVec::<f32, 3>::default();
                 value[0] = *v;
                 value[1] = 0.2 * *v;
@@ -539,30 +509,30 @@
             };
             let pattern = MutTensorDDDR::from_map(&tensor_f32.view(), op);
             println!("p :{}", pattern.mut_array);
             println!("p :{}", pattern.view().scalar_view());
         }
     }
 
-    #[test]
-    pub fn types() {
+    //linalg
+    {
         let shape = [3];
 
         let _tensor_u8 = MutTensorD::from_shape_and_val(shape, 0);
-        let _tensor_f32 = MutTensorDRC::from_shape_and_val(shape, SMat::<f32, 4, 4>::zeros());
+        let _tensor_f64 = MutTensorDRC::from_shape_and_val(shape, SMat::<f64, 4, 4>::zeros());
         let _tensor_batched_f32 =
-            MutTensorDRCB::from_shape_and_val(shape, SMat::<AutoSimd<[f32; 8]>, 4, 4>::zeros());
+            MutTensorDRC::from_shape_and_val(shape, BatchMatF64::<2, 3, 4>::zeros());
     }
 
-    #[test]
-    pub fn from_raw_data() {
+    //from_raw_data
+    {
         let shape = [1];
         let data = [1.0, 2.0, 3.0, 4.0, 5.0, 6.0];
         let data_mat = SMat::<f32, 3, 2>::from_vec(data.to_vec());
-        let tensor_f32 = MutTensorDRC::from_shape_and_val(shape, data_mat); // CxWxH
+        let tensor_f32 = MutTensorDRC::from_shape_and_val(shape, data_mat);
         assert_eq!(tensor_f32.dims(), shape);
         assert_eq!(tensor_f32.view().scalar_get([0, 0, 0]), data[0]);
         assert_eq!(tensor_f32.view().scalar_get([0, 1, 0]), data[1]);
         assert_eq!(tensor_f32.view().scalar_get([0, 2, 0]), data[2]);
         assert_eq!(tensor_f32.view().scalar_get([0, 0, 1]), data[3]);
         assert_eq!(tensor_f32.view().scalar_get([0, 1, 1]), data[4]);
         assert_eq!(tensor_f32.view().scalar_get([0, 2, 1]), data[5]);
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_tensor/src/mut_view.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/mut_tensor_view.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-use crate::mut_tensor::MutTensor;
-use crate::view::IsTensorLike;
-use crate::view::IsTensorView;
-use crate::view::TensorView;
+use crate::prelude::*;
+use crate::tensor::MutTensor;
+use crate::tensor::TensorView;
 use concat_arrays::concat_arrays;
-
-use crate::element::IsStaticTensor;
-use crate::element::IsTensorScalar;
 use std::marker::PhantomData;
 
 /// Mutable tensor view
 ///
 /// See TensorView for more details of the tensor structure
 #[derive(Debug, PartialEq, Eq)]
 pub struct MutTensorView<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
-    Scalar: IsTensorScalar + 'static,
-    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS, BATCH_SIZE> + 'static,
+    Scalar: IsCoreScalar + 'static,
+    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS> + 'static,
     const ROWS: usize,
     const COLS: usize,
-    const BATCH_SIZE: usize,
 > where
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
     ndarray::Dim<[ndarray::Ix; TOTAL_RANK]>: ndarray::Dimension,
 {
     /// mutable ndarray view of the static tensors with shape [D1, D2, ...]
     pub elem_view_mut: ndarray::ArrayViewMut<'a, STensor, ndarray::Dim<[ndarray::Ix; DRANK]>>,
     /// mutable ndarray view of the scalars with shape [D1, D2, ..., S0, S1, ...]
@@ -34,20 +29,19 @@
 
 /// A mutable tensor like object
 pub trait IsMutTensorLike<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
-    Scalar: IsTensorScalar + 'static,
-    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS, BATCH_SIZE> + 'static,
+    Scalar: IsCoreScalar + 'static,
+    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS> + 'static,
     const ROWS: usize,
     const COLS: usize,
-    const BATCH_SIZE: usize,
->: IsTensorLike<'a, TOTAL_RANK, DRANK, SRANK, Scalar, STensor, ROWS, COLS, BATCH_SIZE> where
+>: IsTensorLike<'a, TOTAL_RANK, DRANK, SRANK, Scalar, STensor, ROWS, COLS> where
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
     ndarray::Dim<[ndarray::Ix; TOTAL_RANK]>: ndarray::Dimension,
 {
     /// mutable ndarray view of the static tensors with shape [D1, D2, ...]
     fn elem_view_mut<'b: 'a>(
         &'b mut self,
     ) -> ndarray::ArrayViewMut<'a, STensor, ndarray::Dim<[ndarray::Ix; DRANK]>>;
@@ -62,26 +56,25 @@
 }
 
 macro_rules! mut_view_is_view {
     ($scalar_rank:literal, $srank:literal, $drank:literal) => {
 
         impl<
                 'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
-            > MutTensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            > MutTensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
 
             /// Returns a tensor view
             pub fn view(
                 & self,
-            ) -> TensorView<'_, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            ) -> TensorView<'_, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
             {
                let v =  TensorView {
                     elem_view: self.elem_view_mut.view(),
                     scalar_view: self.scalar_view_mut.view(),
                 };
                 v
             }
@@ -91,28 +84,30 @@
                 elem_view_mut: ndarray::ArrayViewMut<
                     'a,
                     STensor,
                     ndarray::Dim<[ndarray::Ix; $drank]>,
                 >,
             ) -> Self {
                 let dims: [usize; $drank] = elem_view_mut.shape().try_into().unwrap();
+                #[allow(clippy::drop_non_drop)]
                 let shape: [usize; $scalar_rank] = concat_arrays!(dims, STensor::sdims());
 
                 let dstrides: [isize; $drank] = elem_view_mut.strides().try_into().unwrap();
                 let mut dstrides: [usize; $drank] = dstrides.map(|x| x as usize);
                 let num_scalars = STensor::num_scalars();
                 for d in dstrides.iter_mut() {
                     *d *= num_scalars;
                 }
+                #[allow(clippy::drop_non_drop)]
                 let strides = concat_arrays!(dstrides, STensor::strides());
 
                 let ptr = elem_view_mut.as_ptr() as *mut Scalar;
                 use ndarray::ShapeBuilder;
                 assert_eq!(std::mem::size_of::<STensor>(),
-                    std::mem::size_of::<Scalar>() * ROWS * COLS* BATCH_SIZE
+                    std::mem::size_of::<Scalar>() * ROWS * COLS
                 );
 
                 let scalar_view_mut =
                     unsafe { ndarray::ArrayViewMut::from_shape_ptr(shape.strides(strides), ptr) };
 
                 Self {
                     elem_view_mut,
@@ -126,35 +121,32 @@
             }
 
             /// fills self using a unary operator applied to the elements of another tensor
             pub fn map<
                 'b,
                 const OTHER_HRANK: usize,
                 const OTHER_SRANK: usize,
-                OtherScalar: IsTensorScalar + 'static,
+                OtherScalar: IsCoreScalar + 'static,
                 OtherSTensor: IsStaticTensor<
                     OtherScalar,
                     OTHER_SRANK,
                     OTHER_ROWS,
                     OTHER_COLS,
-                    OTHER_BATCHES,
                 > + 'static,
                 const OTHER_ROWS: usize,
                 const OTHER_COLS: usize,
-                const OTHER_BATCHES: usize,
                 V : IsTensorView::<
                     'b,
                     OTHER_HRANK,
                     $drank,
                     OTHER_SRANK,
                     OtherScalar,
                     OtherSTensor,
                     OTHER_ROWS,
                     OTHER_COLS,
-                    OTHER_BATCHES,
                 >,
                 F: FnMut(&mut STensor, &OtherSTensor)
             >(
                 &'a mut self,
                 view: &'b V,
                 op: F,
             ) where
@@ -165,31 +157,29 @@
         }
 
 
 
 
         impl<
         'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
-            > IsTensorLike<'a, $scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS, BATCH_SIZE>
+            > IsTensorLike<'a, $scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS>
             for MutTensorView<
                 'a,
                 $scalar_rank,
                 $drank,
                 $srank,
                 Scalar,
                 STensor,
                 ROWS,
-                COLS,
-                BATCH_SIZE>
-        {
+                COLS
+>        {
             fn elem_view<'b:'a>(
                 &'b self,
             ) -> ndarray::ArrayView<'a, STensor, ndarray::Dim<[ndarray::Ix; $drank]>> {
                 self.view().elem_view
             }
 
             fn get(& self, idx: [usize; $drank]) -> STensor {
@@ -212,46 +202,43 @@
 
             fn scalar_dims(&self) -> [usize; $scalar_rank] {
                 self.view().scalar_dims()
             }
 
             fn to_mut_tensor(
                 &self,
-            ) -> MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS, BATCH_SIZE> {
+            ) -> MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor,  ROWS, COLS> {
                 MutTensor {
                     mut_array: self.view().elem_view.to_owned(),
                     phantom: PhantomData::default(),
                 }
             }
         }
 
         impl<
         'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank,  ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
             >
             IsMutTensorLike<'a,
                 $scalar_rank,
                 $drank, $srank,
                 Scalar, STensor,
                 ROWS,
-                COLS,
-                BATCH_SIZE
-            >
+                COLS            >
             for MutTensorView<'a,
                 $scalar_rank,
                 $drank,
                 $srank,
                 Scalar,
                 STensor,
-                ROWS, COLS,
-                BATCH_SIZE
+                ROWS,
+                COLS,
             >
         {
             fn elem_view_mut<'b:'a>(
                 &'b mut self,
             ) -> ndarray::ArrayViewMut<'a, STensor, ndarray::Dim<[ndarray::Ix; $drank]>>{
                 self.elem_view_mut.view_mut()
             }
@@ -276,8 +263,10 @@
 mut_view_is_view!(2, 1, 1);
 mut_view_is_view!(3, 0, 3);
 mut_view_is_view!(3, 1, 2);
 mut_view_is_view!(3, 2, 1);
 mut_view_is_view!(4, 0, 4);
 mut_view_is_view!(4, 1, 3);
 mut_view_is_view!(4, 2, 2);
-mut_view_is_view!(4, 3, 1);
+mut_view_is_view!(5, 0, 5);
+mut_view_is_view!(5, 1, 4);
+mut_view_is_view!(5, 2, 3);
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_tensor/src/view.rs` & `sophus_pyo3-0.6.0/crates/sophus_core/src/tensor/tensor_view.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-use crate::element::BatchMat;
-use crate::element::BatchScalar;
-use crate::element::BatchVec;
-use crate::element::IsStaticTensor;
-use crate::element::IsTensorScalar;
-use crate::element::SMat;
-use crate::element::SVec;
-use crate::mut_tensor::MutTensor;
-
+use crate::linalg::SMat;
+use crate::linalg::SVec;
+use crate::prelude::*;
+use crate::tensor::MutTensor;
 use concat_arrays::concat_arrays;
 use std::marker::PhantomData;
 
 /// Tensor view
 ///
 /// There are two ways of describing the tensor (TensorView as well as its siblings ArcTensor,
 /// MutTensor and MutTensorView):
@@ -19,173 +14,110 @@
 ///    * The dynamic tensor is of rank DRANK
 ///      - ``self.dims()`` is used to access its dynamic dimensions of type
 ///        ``[usize: DRANK]``.
 ///      - an individual element (= static tensor) can be accessed with
 ///        ``self.get(idx)``, where idx is f type ``[usize: DRANK]``.
 ///      - Each element is of type ``STensor``.
 ///    * Each static tensor is of SRANK. In particular we have.
-///      - rank 0: scalars of type ``Scalar`` (such as ``f64`` or ``u8``).
+///      - rank 0: scalars of type ``Scalar`` (such as ``u8`` or BatchF64<8>).
 ///      - rank 1:
-///         * A batch scalar of type ``BatchScalar<Scalar, BATCH>`` with static
-///           batch size of BATCH_SIZE.
 ///         * A column vector ``SVec<Scalar, ROWS>`` aka ``nalgebra::SVector<Scalar, ROWS>`` with
 ///           number of ROWS.
 ///      - rank 2:
-///         * A batch vector of type ``BatchVector<Scalar, BATCH_SIZE>`` with static
-///           shape (ROWS x BATCH_SIZE).
 ///         * A matrix ``SMat<Scalar, ROWS, COLS>`` aka ``nalgebra::SMatrix<Scalar, ROWS, COLS>``
 ///           with static shape (ROWS x COLS).
-///       - rank 3:
-///         * A batch matrix of type ``BatchMatrix<Scalar, ROWS, COLS, BATCH>`` with static
-///           shape (BATCH_SIZE x ROWS .x COLS).
 ///  2. A scalar tensor of TOTAL_RANK = DRANK + SRANK.
 ///    *  ``self.scalar_dims()`` is used to access its dimensions of type
 ///        ``[usize: TOTAL_RANK]`` at runtime.
 ///    *  - an individual element (= static tensor) can be accessed with
 ///        ``self.scalar_get(idx)``, where idx is of type ``[usize: DRANK]``.
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub struct TensorView<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
-    Scalar: IsTensorScalar + 'static,
-    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS, BATCH_SIZE> + 'static,
+    Scalar: IsCoreScalar + 'static,
+    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS> + 'static,
     const ROWS: usize,
     const COLS: usize,
-    const BATCH_SIZE: usize,
 > where
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
     ndarray::Dim<[ndarray::Ix; TOTAL_RANK]>: ndarray::Dimension,
 {
     /// Element view - an ndarray of static tensors with shape [D0, D1, ...]
     pub elem_view: ndarray::ArrayView<'a, STensor, ndarray::Dim<[ndarray::Ix; DRANK]>>,
     /// Scalar view - an ndarray of scalars with shape [D0, D1, ..., S0, S1, ...]
     pub scalar_view: ndarray::ArrayView<'a, Scalar, ndarray::Dim<[ndarray::Ix; TOTAL_RANK]>>,
 }
 
 /// Tensor view of scalars
 pub type TensorViewX<'a, const DRANK: usize, Scalar> =
-    TensorView<'a, DRANK, DRANK, 0, Scalar, Scalar, 1, 1, 1>;
-
-/// Tensor view of batched scalars
-pub type TensorViewXB<
-    'a,
-    const TOTAL_RANK: usize,
-    const DRANK: usize,
-    const SRANK: usize,
-    Scalar,
-    const B: usize,
-> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, BatchScalar<Scalar, B>, 1, 1, B>;
+    TensorView<'a, DRANK, DRANK, 0, Scalar, Scalar, 1, 1>;
 
 /// Tensor view of vectors with shape R
 pub type TensorViewXR<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     Scalar,
     const R: usize,
-> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, SVec<Scalar, R>, R, 1, 1>;
-
-/// Tensor view of batched vectors with shape [R x B]
-pub type TensorViewXRB<
-    'a,
-    const TOTAL_RANK: usize,
-    const DRANK: usize,
-    const SRANK: usize,
-    Scalar,
-    const R: usize,
-    const B: usize,
-> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, BatchVec<Scalar, R, B>, R, 1, B>;
+> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, SVec<Scalar, R>, R, 1>;
 
 /// Tensor view of matrices with shape [R x C]
 pub type TensorViewXRC<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
     Scalar,
     const R: usize,
     const C: usize,
-> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, SMat<Scalar, R, C>, R, C, 1>;
-
-/// Tensor view of batched matrices with shape [R x C x B]
-pub type TensorViewXRCB<
-    'a,
-    const TOTAL_RANK: usize,
-    const DRANK: usize,
-    const SRANK: usize,
-    Scalar,
-    const R: usize,
-    const C: usize,
-    const B: usize,
-> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, BatchMat<Scalar, R, C, B>, R, C, B>;
+> = TensorView<'a, TOTAL_RANK, DRANK, SRANK, Scalar, SMat<Scalar, R, C>, R, C>;
 
 /// rank-1 tensor view of scalars with shape D0
 pub type TensorViewD<'a, Scalar> = TensorViewX<'a, 1, Scalar>;
 
 /// rank-2 tensor view of scalars with shape [D0 x D1]
 pub type TensorViewDD<'a, Scalar> = TensorViewX<'a, 2, Scalar>;
 
-/// rank-2 tensor view of batched scalars with shape [D0 x B]
-pub type TensorViewDB<'a, Scalar, const B: usize> = TensorViewXB<'a, 2, 1, 1, Scalar, B>;
-
 /// rank-2 tensor view of vectors with shape [D0 x R]
 pub type TensorViewDR<'a, Scalar, const R: usize> = TensorViewXR<'a, 2, 1, 1, Scalar, R>;
 
 /// rank-3 tensor view of scalars with shape [D0 x R x B]
 pub type TensorViewDDD<'a, Scalar> = TensorViewX<'a, 3, Scalar>;
 
-/// rank-3 tensor view of batched scalars with shape [D0 x D1 x B]
-pub type TensorViewDDB<'a, Scalar, const B: usize> = TensorViewXB<'a, 3, 2, 1, Scalar, B>;
-
 /// rank-3 tensor view of vectors with shape [D0 x D1 x R]
 pub type TensorViewDDR<'a, Scalar, const R: usize> = TensorViewXR<'a, 3, 2, 1, Scalar, R>;
 
-/// rank-3 tensor view of batched vectors with shape [D0 x R x B]
-pub type TensorViewDRB<'a, Scalar, const R: usize, const B: usize> =
-    TensorViewXRB<'a, 3, 1, 2, Scalar, R, B>;
-
 /// rank-3 tensor view of matrices with shape [D0 x R x C]
 pub type TensorViewDRC<'a, Scalar, const R: usize, const C: usize> =
     TensorViewXRC<'a, 3, 1, 2, Scalar, R, C>;
 
 /// rank-4 tensor view of scalars with shape [D0 x D1 x D2 x D3]
 pub type TensorViewDDDD<'a, Scalar> = TensorViewX<'a, 4, Scalar>;
 
-/// rank-4 tensor view of batched scalars with shape [D0 x D1 x D2 x B]
-pub type TensorViewDDDB<'a, Scalar, const B: usize> = TensorViewXB<'a, 4, 3, 1, Scalar, B>;
-
 /// rank-4 tensor view of vectors with shape [D0 x D1 x D2 x R]
 pub type TensorViewDDDR<'a, Scalar, const R: usize> = TensorViewXR<'a, 4, 3, 1, Scalar, R>;
 
-/// rank-4 tensor view of batched vectors with shape [D0 x D1 x R x B]
-pub type TensorViewDDRB<'a, Scalar, const R: usize, const B: usize> =
-    TensorViewXRB<'a, 4, 2, 2, Scalar, R, B>;
-
 /// rank-4 tensor view of matrices with shape [D0 x R x C x B]
 pub type TensorViewDDRC<'a, Scalar, const R: usize, const C: usize> =
     TensorViewXRC<'a, 4, 2, 2, Scalar, R, C>;
 
-/// rank-4 tensor view of batched matrices with shape [D0 x R x C x B]
-pub type TensorViewDRCB<'a, Scalar, const R: usize, const C: usize, const B: usize> =
-    TensorViewXRCB<'a, 4, 1, 3, Scalar, R, C, B>;
-
 /// Is a tensor-like object
 pub trait IsTensorLike<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
-    Scalar: IsTensorScalar + 'static,
-    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS, BATCH_SIZE> + 'static,
+    Scalar: IsCoreScalar + 'static,
+    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS> + 'static,
     const ROWS: usize,
     const COLS: usize,
-    const BATCH_SIZE: usize,
 > where
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
     ndarray::Dim<[ndarray::Ix; TOTAL_RANK]>: ndarray::Dimension,
 {
     /// Element view - that is a tensor view of static tensors
     fn elem_view<'b: 'a>(
         &'b self,
@@ -205,70 +137,68 @@
     /// Get the scalar at index idx
     fn scalar_get(&'a self, idx: [usize; TOTAL_RANK]) -> Scalar;
 
     /// Get the dimensions of the scalar view [D0, D1, ..., S0, S1, ...]
     fn scalar_dims(&self) -> [usize; TOTAL_RANK];
 
     /// Convert to a mutable tensor - this will copy the tensor
-    fn to_mut_tensor(
-        &self,
-    ) -> MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, STensor, ROWS, COLS, BATCH_SIZE>;
+    fn to_mut_tensor(&self) -> MutTensor<TOTAL_RANK, DRANK, SRANK, Scalar, STensor, ROWS, COLS>;
 }
 
 /// Is a tensor view like object
 pub trait IsTensorView<
     'a,
     const TOTAL_RANK: usize,
     const DRANK: usize,
     const SRANK: usize,
-    Scalar: IsTensorScalar + 'static,
-    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS, BATCH_SIZE> + 'static,
+    Scalar: IsCoreScalar + 'static,
+    STensor: IsStaticTensor<Scalar, SRANK, ROWS, COLS> + 'static,
     const ROWS: usize,
     const COLS: usize,
-    const BATCH_SIZE: usize,
->: IsTensorLike<'a, TOTAL_RANK, DRANK, SRANK, Scalar, STensor, ROWS, COLS, BATCH_SIZE> where
+>: IsTensorLike<'a, TOTAL_RANK, DRANK, SRANK, Scalar, STensor, ROWS, COLS> where
     ndarray::Dim<[ndarray::Ix; DRANK]>: ndarray::Dimension,
     ndarray::Dim<[ndarray::Ix; TOTAL_RANK]>: ndarray::Dimension,
 {
     /// return tensor view
     fn view<'b: 'a>(&'b self) -> Self;
 }
 
 macro_rules! tensor_view_is_view {
     ($scalar_rank:literal, $srank:literal, $drank:literal) => {
         impl<
                 'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS, BATCH_SIZE>,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS>,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
-            > TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            > TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
             /// Create a new tensor view from an ndarray of static tensors
             pub fn new(
                 elem_view: ndarray::ArrayView<'a, STensor, ndarray::Dim<[ndarray::Ix; $drank]>>,
             ) -> Self {
                 let dims: [usize; $drank] = elem_view.shape().try_into().unwrap();
+                #[allow(clippy::drop_non_drop)]
                 let shape: [usize; $scalar_rank] = concat_arrays!(dims, STensor::sdims());
 
                 let dstrides: [isize; $drank] = elem_view.strides().try_into().unwrap();
                 let mut dstrides: [usize; $drank] = dstrides.map(|x| x as usize);
                 let num_scalars = STensor::num_scalars();
                 for d in dstrides.iter_mut() {
                     *d *= num_scalars;
                 }
+                #[allow(clippy::drop_non_drop)]
                 let strides = concat_arrays!(dstrides, STensor::strides());
 
                 let ptr = elem_view.as_ptr() as *const Scalar;
                 use ndarray::ShapeBuilder;
 
                 assert_eq!(
                     std::mem::size_of::<STensor>(),
-                    std::mem::size_of::<Scalar>() * ROWS * COLS * BATCH_SIZE
+                    std::mem::size_of::<Scalar>() * ROWS * COLS
                 );
                 let scalar_view =
                     unsafe { ndarray::ArrayView::from_shape_ptr(shape.strides(strides), ptr) };
 
                 Self {
                     elem_view,
                     scalar_view,
@@ -280,201 +210,192 @@
                 let elem_view = ndarray::ArrayView::from_shape(shape, slice).unwrap();
                 Self::new(elem_view)
             }
         }
 
         impl<
                 'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
-            > IsTensorLike<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
-            for TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            > IsTensorLike<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
+            for TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
             fn elem_view<'b: 'a>(
                 &'b self,
             ) -> ndarray::ArrayView<'a, STensor, ndarray::Dim<[ndarray::Ix; $drank]>> {
                 self.elem_view
             }
 
             fn get(&self, idx: [usize; $drank]) -> STensor {
-                self.elem_view[idx]
+                self.elem_view[idx].clone()
             }
 
             fn dims(&self) -> [usize; $drank] {
                 self.elem_view.shape().try_into().unwrap()
             }
 
             fn scalar_view<'b: 'a>(
                 &'b self,
             ) -> ndarray::ArrayView<'a, Scalar, ndarray::Dim<[ndarray::Ix; $scalar_rank]>> {
                 self.scalar_view
             }
 
             fn scalar_get(&'a self, idx: [usize; $scalar_rank]) -> Scalar {
-                self.scalar_view[idx]
+                self.scalar_view[idx].clone()
             }
 
             fn scalar_dims(&self) -> [usize; $scalar_rank] {
                 self.scalar_view.shape().try_into().unwrap()
             }
 
             fn to_mut_tensor(
                 &self,
-            ) -> MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE> {
+            ) -> MutTensor<$scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS> {
                 MutTensor {
                     mut_array: self.elem_view.to_owned(),
                     phantom: PhantomData::default(),
                 }
             }
         }
 
         impl<
                 'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS, BATCH_SIZE> + 'static,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-                const BATCH_SIZE: usize,
-            > IsTensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
-            for TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            > IsTensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
+            for TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
             fn view<'b: 'a>(
                 &'b self,
-            ) -> TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
-            {
-                *self
+            ) -> TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS> {
+                self.clone()
             }
         }
 
         impl<
                 'a,
-                Scalar: IsTensorScalar + 'static,
-                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS, BATCH_SIZE> + 'static,
-                const BATCH_SIZE: usize,
+                Scalar: IsCoreScalar + 'static,
+                STensor: IsStaticTensor<Scalar, $srank, ROWS, COLS> + 'static,
                 const ROWS: usize,
                 const COLS: usize,
-            > TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS, BATCH_SIZE>
+            > TensorView<'a, $scalar_rank, $drank, $srank, Scalar, STensor, ROWS, COLS>
         {
         }
     };
 }
 
 tensor_view_is_view!(1, 0, 1);
 tensor_view_is_view!(2, 0, 2);
 tensor_view_is_view!(2, 1, 1);
 tensor_view_is_view!(3, 0, 3);
 tensor_view_is_view!(3, 1, 2);
 tensor_view_is_view!(3, 2, 1);
 tensor_view_is_view!(4, 0, 4);
 tensor_view_is_view!(4, 1, 3);
 tensor_view_is_view!(4, 2, 2);
-tensor_view_is_view!(4, 3, 1);
-
-#[cfg(test)]
-mod tests {
-
-    #[test]
-    fn view() {
-        use super::*;
-        use ndarray::ShapeBuilder;
-        {
-            let rank1_shape = [3];
-            let arr: [u8; 3] = [5, 6, 7];
-
-            let ndview =
-                ndarray::ArrayView::from_shape(rank1_shape.strides([1]), &arr[..]).unwrap();
-            assert!(ndview.is_standard_layout());
-            let view = TensorViewD::new(ndview);
+tensor_view_is_view!(5, 0, 5);
+tensor_view_is_view!(5, 1, 4);
+tensor_view_is_view!(5, 2, 3);
+
+#[test]
+fn tensor_view_tests() {
+    use ndarray::ShapeBuilder;
+    {
+        let rank1_shape = [3];
+        let arr: [u8; 3] = [5, 6, 7];
+
+        let ndview = ndarray::ArrayView::from_shape(rank1_shape.strides([1]), &arr[..]).unwrap();
+        assert!(ndview.is_standard_layout());
+        let view = TensorViewD::new(ndview);
 
-            for i in 0..view.dims()[0] {
-                assert_eq!(arr[i], view.get([i]));
+        for i in 0..view.dims()[0] {
+            assert_eq!(arr[i], view.get([i]));
+        }
+    }
+    {
+        const ROWS: usize = 2;
+        const COLS: usize = 3;
+
+        type Mat2x3 = SMat<f32, 2, 3>;
+
+        let a = Mat2x3::new(0.1, 0.56, 0.77, 2.0, 5.1, 7.0);
+        let b = Mat2x3::new(0.6, 0.5, 0.78, 2.0, 5.2, 7.1);
+        let c = Mat2x3::new(0.9, 0.58, 0.7, 2.0, 5.3, 7.2);
+        let d = Mat2x3::new(0.9, 0.50, 0.9, 2.0, 5.0, 7.3);
+
+        let rank2_shape = [4, 2];
+        let arr = [a, a, b, c, d, c, b, b];
+
+        let strides = [2, 1];
+        let ndview = ndarray::ArrayView::from_shape(rank2_shape.strides([2, 1]), &arr[..]).unwrap();
+        assert!(ndview.is_standard_layout());
+        let view = TensorViewDDRC::new(ndview);
+
+        println!("{}", view.elem_view);
+        for d0 in 0..view.dims()[0] {
+            for d1 in 0..view.dims()[1] {
+                assert_eq!(view.get([d0, d1]), arr[strides[0] * d0 + strides[1] * d1]);
             }
         }
-        {
-            const ROWS: usize = 2;
-            const COLS: usize = 3;
-
-            type Mat2x3 = SMat<f32, 2, 3>;
 
-            let a = Mat2x3::new(0.1, 0.56, 0.77, 2.0, 5.1, 7.0);
-            let b = Mat2x3::new(0.6, 0.5, 0.78, 2.0, 5.2, 7.1);
-            let c = Mat2x3::new(0.9, 0.58, 0.7, 2.0, 5.3, 7.2);
-            let d = Mat2x3::new(0.9, 0.50, 0.9, 2.0, 5.0, 7.3);
-
-            let rank2_shape = [4, 2];
-            let arr = [a, a, b, c, d, c, b, b];
-
-            let strides = [2, 1];
-            let ndview =
-                ndarray::ArrayView::from_shape(rank2_shape.strides([2, 1]), &arr[..]).unwrap();
-            assert!(ndview.is_standard_layout());
-            let view = TensorViewDDRC::new(ndview);
-
-            println!("{}", view.elem_view);
-            for d0 in 0..view.dims()[0] {
-                for d1 in 0..view.dims()[1] {
-                    assert_eq!(view.get([d0, d1]), arr[strides[0] * d0 + strides[1] * d1]);
+        println!("{:?}", view.scalar_view);
+        assert!(!view.scalar_view.is_standard_layout());
+        for d0 in 0..view.scalar_dims()[0] {
+            for d1 in 0..view.scalar_dims()[1] {
+                for c in 0..COLS {
+                    for r in 0..ROWS {
+                        assert_eq!(
+                            view.scalar_get([d0, d1, r, c]),
+                            arr[strides[0] * d0 + strides[1] * d1][c * ROWS + r]
+                        );
+                    }
                 }
             }
+        }
+    }
 
-            println!("{:?}", view.scalar_view);
-            assert!(!view.scalar_view.is_standard_layout());
-            for d0 in 0..view.scalar_dims()[0] {
-                for d1 in 0..view.scalar_dims()[1] {
-                    for c in 0..COLS {
-                        for r in 0..ROWS {
-                            assert_eq!(
-                                view.scalar_get([d0, d1, r, c]),
-                                arr[strides[0] * d0 + strides[1] * d1][c * ROWS + r]
-                            );
-                        }
-                    }
+    {
+        let rank3_shape = [4, 2, 3];
+        let raw_arr = [
+            4, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27,
+            28,
+        ];
+
+        let arr = raw_arr.map(SVec::<u8, 1>::new);
+
+        let strides = [6, 3, 1];
+        let ndview =
+            ndarray::ArrayView::from_shape(rank3_shape.strides(strides), &arr[..]).unwrap();
+        assert!(ndview.is_standard_layout());
+        let view = TensorViewDDDR::new(ndview);
+
+        println!("{}", view.elem_view);
+        for d0 in 0..view.dims()[0] {
+            for d1 in 0..view.dims()[1] {
+                for d2 in 0..view.dims()[2] {
+                    assert_eq!(
+                        view.get([d0, d1, d2]),
+                        arr[strides[0] * d0 + strides[1] * d1 + strides[2] * d2]
+                    );
                 }
             }
         }
 
-        {
-            let rank3_shape = [4, 2, 3];
-            let raw_arr = [
-                4, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26,
-                27, 28,
-            ];
-
-            let arr = raw_arr.map(SVec::<u8, 1>::new);
-
-            let strides = [6, 3, 1];
-            let ndview =
-                ndarray::ArrayView::from_shape(rank3_shape.strides(strides), &arr[..]).unwrap();
-            assert!(ndview.is_standard_layout());
-            let view = TensorViewDDDR::new(ndview);
-
-            println!("{}", view.elem_view);
-            for d0 in 0..view.dims()[0] {
-                for d1 in 0..view.dims()[1] {
-                    for d2 in 0..view.dims()[2] {
+        println!("{:?}", view.scalar_view);
+        for d0 in 0..view.scalar_dims()[0] {
+            for d1 in 0..view.scalar_dims()[1] {
+                for d2 in 0..view.scalar_dims()[2] {
+                    for r in 0..1 {
                         assert_eq!(
-                            view.get([d0, d1, d2]),
-                            arr[strides[0] * d0 + strides[1] * d1 + strides[2] * d2]
+                            view.scalar_get([d0, d1, d2, r]),
+                            arr[strides[0] * d0 + strides[1] * d1 + strides[2] * d2][r]
                         );
                     }
                 }
             }
-
-            println!("{:?}", view.scalar_view);
-            for d0 in 0..view.scalar_dims()[0] {
-                for d1 in 0..view.scalar_dims()[1] {
-                    for d2 in 0..view.scalar_dims()[2] {
-                        for r in 0..1 {
-                            assert_eq!(
-                                view.scalar_get([d0, d1, d2, r]),
-                                arr[strides[0] * d0 + strides[1] * d1 + strides[2] * d2][r]
-                            );
-                        }
-                    }
-                }
-            }
         }
     }
 }
```

### Comparing `sophus_pyo3-0.4.0/crates/sophus_pyo3/Cargo.toml` & `sophus_pyo3-0.6.0/crates/sophus_pyo3/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 include.workspace = true
 keywords.workspace = true
 license.workspace = true
 repository.workspace = true
 version.workspace = true
 
 [dependencies]
-sophus_calculus.workspace = true
+sophus_core.workspace = true
 sophus_lie.workspace = true
-sophus_tensor.workspace = true
 
 nalgebra.workspace = true
 numpy.workspace = true
 
 [dependencies.pyo3]
-version = "0.20.0"
+version = "0.21.2"
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
-features = ["abi3-py38", "multiple-pymethods"]
+features = ["abi3-py38"]
```

### Comparing `sophus_pyo3-0.4.0/Cargo.lock` & `sophus_pyo3-0.6.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ab_glyph"
-version = "0.2.23"
+version = "0.2.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80179d7dd5d7e8c285d67c4a1e652972a92de7475beddfb92028c76463b13225"
+checksum = "2e53b0a3d5760cd2ba9b787ae0c6440ad18ee294ff71b05e3381c900a7d16cfd"
 dependencies = [
  "ab_glyph_rasterizer",
  "owned_ttf_parser",
 ]
 
 [[package]]
 name = "ab_glyph_rasterizer"
@@ -129,17 +129,17 @@
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "android-activity"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee91c0c2905bae44f84bfa4e044536541df26b7703fd0888deeb9060fcc44289"
 dependencies = [
@@ -171,55 +171,56 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "approx"
@@ -228,25 +229,24 @@
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "arboard"
-version = "3.3.2"
+version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2041f1943049c7978768d84e6d0fd95de98b76d6c4727b09e78ec253d29fa58"
+checksum = "9fb4009533e8ff8f1450a5bcbc30f4242a1d34442221f72314bea1f5dc9c7f89"
 dependencies = [
  "clipboard-win",
  "log",
- "objc",
- "objc-foundation",
- "objc_id",
+ "objc2 0.5.2",
+ "objc2-app-kit",
+ "objc2-foundation",
  "parking_lot",
- "thiserror",
  "x11rb",
 ]
 
 [[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -293,35 +293,33 @@
 dependencies = [
  "event-listener 2.5.3",
  "futures-core",
 ]
 
 [[package]]
 name = "async-channel"
-version = "2.2.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f28243a43d821d11341ab73c80bed182dc015c514b951616cf79bd4af39af0c3"
+checksum = "89b47800b0be77592da0afd425cc03468052844aff33b84e33cc696f64e77b6a"
 dependencies = [
  "concurrent-queue",
- "event-listener 5.2.0",
- "event-listener-strategy 0.5.0",
+ "event-listener-strategy 0.5.2",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.8.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ae5ebefcc48e7452b4987947920dac9450be1110cadf34d1b8c116bdbaf97c"
+checksum = "c8828ec6e544c02b0d6691d21ed9f9218d0384a82542855073c2a3f58304aaf0"
 dependencies = [
- "async-lock 3.3.0",
  "async-task",
  "concurrent-queue",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-lite 2.3.0",
  "slab",
 ]
 
 [[package]]
 name = "async-fs"
 version = "1.6.0"
@@ -362,16 +360,16 @@
 dependencies = [
  "async-lock 3.3.0",
  "cfg-if",
  "concurrent-queue",
  "futures-io",
  "futures-lite 2.3.0",
  "parking",
- "polling 3.6.0",
- "rustix 0.38.32",
+ "polling 3.7.0",
+ "rustix 0.38.34",
  "slab",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-lock"
@@ -408,62 +406,62 @@
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-signal",
  "blocking",
  "cfg-if",
  "event-listener 3.1.0",
  "futures-lite 1.13.0",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-recursion"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30c5ef0ede93efbf733c1a727f3b6b5a1060bbedd5600183e66f6e4be4af0ec5"
+checksum = "3b43422f69d8ff38f95f1b2bb76517c91589a924d1559a0e935d7c8ce0274c11"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "async-signal"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e47d90f65a225c4527103a8d747001fc56e375203592b25ad103e1ca13124c5"
+checksum = "afe66191c335039c7bb78f99dc7520b0cbb166b3a1cb33a03f53d8a1c6f2afda"
 dependencies = [
  "async-io 2.3.2",
- "async-lock 2.8.0",
+ "async-lock 3.3.0",
  "atomic-waker",
  "cfg-if",
  "futures-core",
  "futures-io",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "signal-hook-registry",
  "slab",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.7.0"
+version = "4.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbb36e985947064623dbd357f727af08ffd077f93d696782f3c56365fa2e2799"
+checksum = "8b75356056920673b02621b35afd0f7dda9306d03c79a30f5c56c44cf256e3de"
 
 [[package]]
 name = "async-trait"
-version = "0.1.79"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
@@ -514,17 +512,17 @@
  "atspi-common",
  "serde",
  "zbus",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -590,15 +588,15 @@
 
 [[package]]
 name = "block-sys"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae85a0696e7ea3b835a453750bf002770776609115e6d25c6d2ff28a8200f7e7"
 dependencies = [
- "objc-sys 0.3.2",
+ "objc-sys 0.3.5",
 ]
 
 [[package]]
 name = "block2"
 version = "0.2.0-alpha.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8dd9e63c1744f755c2f60332b88de39d341e5e86239014ad839bd71c106dec42"
@@ -614,53 +612,60 @@
 checksum = "15b55663a85f33501257357e6421bb33e769d5c9ffb5ba0921c975a123e35e68"
 dependencies = [
  "block-sys 0.2.1",
  "objc2 0.4.1",
 ]
 
 [[package]]
+name = "block2"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c132eebf10f5cad5289222520a4a058514204aed6d791f1cf4fe8088b82d15f"
+dependencies = [
+ "objc2 0.5.2",
+]
+
+[[package]]
 name = "blocking"
-version = "1.5.1"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a37913e8dc4ddcc604f0c6d3bf2887c995153af3611de9e23c352b44c1b9118"
+checksum = "495f7104e962b7356f0aeb34247aca1fe7d2e783b346582db7f2904cb5717e88"
 dependencies = [
  "async-channel",
  "async-lock 3.3.0",
  "async-task",
- "fastrand 2.0.2",
  "futures-io",
  "futures-lite 2.3.0",
  "piper",
- "tracing",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
+checksum = "369cfaf2a5bed5d8f8202073b2e093c9f508251de1551a0deb4253e4c7d80909"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -675,40 +680,41 @@
 name = "calloop"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
  "bitflags 2.5.0",
  "log",
- "polling 3.6.0",
- "rustix 0.38.32",
+ "polling 3.7.0",
+ "rustix 0.38.34",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "calloop-wayland-source"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f0ea9b9476c7fad82841a8dbb380e2eae480c21910feba80725b46931ed8f02"
 dependencies = [
  "calloop",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "wayland-backend",
  "wayland-client",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
@@ -732,17 +738,17 @@
 checksum = "0ced0551234e87afee12411d535648dd89d2e7f34c78b753395567aff3d447ff"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "clipboard-win"
-version = "5.3.0"
+version = "5.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d517d4b86184dbb111d3556a10f1c8a04da7428d2987bf1081602bf11c3aa9ee"
+checksum = "79f4473f5144e20d9aceaf2972478f06ddf687831eafeeb434fbaf0acc4144ad"
 dependencies = [
  "error-code",
 ]
 
 [[package]]
 name = "cocoa"
 version = "0.25.0"
@@ -793,17 +799,17 @@
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "colored"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cbf2150cce219b664a8a70df7a1f933836724b503f8a413af9365b4dcc4d90b8"
 dependencies = [
@@ -840,17 +846,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "combine"
-version = "4.6.6"
+version = "4.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
+checksum = "ba5a308b75df32fe02788e748662718f03fde005016435c444eea572398219fd"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "concat-arrays"
@@ -861,17 +867,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
+checksum = "4ca0197aee26d1ae37445ee532fefce43251d24cc7c166799f4d46817f1d3973"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "convert_case"
 version = "0.6.0"
@@ -895,17 +901,17 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "core-graphics"
-version = "0.23.1"
+version = "0.23.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "970a29baf4110c26fedbc7f82107d42c23f7e88e404c4577ed73fe99ff85a212"
+checksum = "c07782be35f9e1140080c6b96f0d44b739e2278479f64e02fdab4e32dfd8b081"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-graphics-types",
  "foreign-types",
  "libc",
 ]
@@ -928,17 +934,17 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -956,17 +962,17 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -977,14 +983,24 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "ctrlc"
+version = "3.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "672465ae37dc1bc6380a6547a8883d5dd397b0f1faaad4f265726cc7042a5345"
+dependencies = [
+ "nix 0.28.0",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "cursor-icon"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96a6ac251f4a2aca6b3f91340350eab87ae57c3f127ffeb585e92bd336717991"
 
 [[package]]
 name = "d3d12"
@@ -1045,18 +1061,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
 dependencies = [
  "litrs",
 ]
 
 [[package]]
+name = "doubled"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f60f472d90e6b0aa29ba7e63aef46fa5441a4a852d36d950648b5468adfe3a3"
+
+[[package]]
 name = "downcast-rs"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
+checksum = "75b325c5dbd37f80359721ad39aca5a29fb04c89279657cffdda8736d0c0b9d2"
 
 [[package]]
 name = "drawille"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64e461c3f1e69d99372620640b3fd5f0309eeda2e26e4af69f6760c0e1df845"
 dependencies = [
@@ -1078,27 +1100,27 @@
 dependencies = [
  "bytemuck",
  "reborrow",
 ]
 
 [[package]]
 name = "ecolor"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03cfe80b1890e1a8cdbffc6044d6872e814aaf6011835a2a5e2db0e5c5c4ef4e"
+checksum = "20930a432bbd57a6d55e07976089708d4893f3d556cf42a0d79e9e321fa73b10"
 dependencies = [
  "bytemuck",
  "serde",
 ]
 
 [[package]]
 name = "eframe"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c456c1bb6d13bf68b780257484703d750c70a23ff891ba35f4d6e23a4dbdf26f"
+checksum = "020e2ccef6bbcec71dbc542f7eed64a5846fc3076727f5746da8fd307c91bab2"
 dependencies = [
  "bytemuck",
  "cocoa",
  "document-features",
  "egui",
  "egui-wgpu",
  "egui-winit",
@@ -1110,45 +1132,45 @@
  "js-sys",
  "log",
  "objc",
  "parking_lot",
  "percent-encoding",
  "pollster",
  "raw-window-handle 0.5.2",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "static_assertions",
  "thiserror",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "web-time",
  "wgpu",
  "winapi",
  "winit",
 ]
 
 [[package]]
 name = "egui"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180f595432a5b615fc6b74afef3955249b86cfea72607b40740a4cd60d5297d0"
+checksum = "584c5d1bf9a67b25778a3323af222dbe1a1feb532190e103901187f92c7fe29a"
 dependencies = [
  "accesskit",
  "ahash",
  "epaint",
  "log",
  "nohash-hasher",
  "serde",
 ]
 
 [[package]]
 name = "egui-wgpu"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f2d75e1e70228e7126f828bac05f9fe0e7ea88e9660c8cebe609bb114c61d4"
+checksum = "469ff65843f88a702b731a1532b7d03b0e8e96d283e70f3a22b0e06c46cb9b37"
 dependencies = [
  "bytemuck",
  "document-features",
  "egui",
  "epaint",
  "log",
  "thiserror",
@@ -1156,84 +1178,84 @@
  "web-time",
  "wgpu",
  "winit",
 ]
 
 [[package]]
 name = "egui-winit"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa4d44f8d89f70d4480545eb2346b76ea88c3022e9f4706cebc799dbe8b004a2"
+checksum = "2e3da0cbe020f341450c599b35b92de4af7b00abde85624fd16f09c885573609"
 dependencies = [
  "accesskit_winit",
  "arboard",
  "egui",
  "log",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "smithay-clipboard",
  "web-time",
  "webbrowser",
  "winit",
 ]
 
 [[package]]
 name = "egui_extras"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f4a6962241a76da5be5e64e41b851ee1c95fda11f76635522a3c82b119b5475"
+checksum = "1b78779f35ded1a853786c9ce0b43fe1053e10a21ea3b23ebea411805ce41593"
 dependencies = [
  "egui",
  "enum-map",
  "log",
  "mime_guess2",
  "serde",
 ]
 
 [[package]]
 name = "egui_glow"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a08e3be8728b4c59493dbfec041c657e6725bdeafdbd49aef3f1dbb9e551fa01"
+checksum = "e0e5d975f3c86edc3d35b1db88bb27c15dde7c55d3b5af164968ab5ede3f44ca"
 dependencies = [
  "bytemuck",
  "egui",
  "glow",
  "log",
- "memoffset 0.9.0",
+ "memoffset 0.9.1",
  "wasm-bindgen",
  "web-sys",
  "winit",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "emath"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6916301ecf80448f786cdf3eb51d9dbdd831538732229d49119e2d4312eaaf09"
+checksum = "e4c3a552cfca14630702449d35f41c84a0d15963273771c6059175a803620f3f"
 dependencies = [
  "bytemuck",
  "serde",
 ]
 
 [[package]]
 name = "enum-as-inner"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "enum-map"
 version = "2.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6866f3bfdf8207509a033af1a75a7b08abda06bbaaeae6669323fd5a097df2e9"
@@ -1246,15 +1268,15 @@
 name = "enum-map-derive"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f282cfdfe92516eb26c2af8589c274c7c17681f5ecc03c18255fe741c6aa64eb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "enumflags2"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3278c9d5fb675e0a51dabcf4c0d355f692b064171535ba72361be1528a9d8e8d"
@@ -1267,26 +1289,26 @@
 name = "enumflags2_derive"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "enumn"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "env_filter"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a009aa4810eb158359dda09d0c87378e4bbb89b5a801f016885a4707ba24f7ea"
@@ -1306,17 +1328,17 @@
  "env_filter",
  "humantime",
  "log",
 ]
 
 [[package]]
 name = "epaint"
-version = "0.26.2"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77b9fdf617dd7f58b0c8e6e9e4a1281f730cde0831d40547da446b2bb76a47af"
+checksum = "b381f8b149657a4acf837095351839f32cd5c4aec1817fc4df84e18d76334176"
 dependencies = [
  "ab_glyph",
  "ahash",
  "bytemuck",
  "ecolor",
  "emath",
  "log",
@@ -1338,28 +1360,28 @@
 name = "equator-macro"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60d08acb9849f7fb4401564f251be5a526829183a3645a90197dea8e786cf3ae"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "error-code"
@@ -1393,17 +1415,17 @@
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener"
-version = "5.2.0"
+version = "5.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b5fb89194fa3cad959b833185b3063ba881dbfc7030680b314250779fb4cc91"
+checksum = "6d9944b8ca13534cdfb2800775f8dd4902ff3fc75a50101466decadfdf322a24"
 dependencies = [
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -1414,19 +1436,19 @@
 dependencies = [
  "event-listener 4.0.3",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener-strategy"
-version = "0.5.0"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "feedafcaa9b749175d5ac357452a9d41ea2911da598fde46ce1fe02c37751291"
+checksum = "0f214dc438f977e6d4e3500aaa277f5ad94ca83fbbd9b1a15713ce2344ccc5a1"
 dependencies = [
- "event-listener 5.2.0",
+ "event-listener 5.3.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "faer"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1475,17 +1497,17 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fdeflate"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
 dependencies = [
@@ -1496,17 +1518,17 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -1528,15 +1550,15 @@
 name = "foreign-types-macros"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "foreign-types-shared"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
@@ -1579,15 +1601,15 @@
 
 [[package]]
 name = "futures-lite"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52527eb5074e35e9339c6b4e8d12600c7128b68fb25dcb9fa9dec18f7c25f3a5"
 dependencies = [
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-core",
  "futures-io",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -1754,17 +1776,17 @@
 dependencies = [
  "libc",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -1917,29 +1939,29 @@
 name = "grid"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d196ffc1627db18a531359249b2bf8416178d84b729f3cebeb278f285fb9b58c"
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "bytemuck",
  "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
 ]
 
 [[package]]
 name = "hassle-rs"
@@ -1978,42 +2000,46 @@
 name = "hexf-parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfa686283ad6dd069f105e5ab091b04c62850d3e4cf5d67debad1933f55023df"
 
 [[package]]
 name = "hollywood"
-version = "0.5.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "878086335e7a512c1ebe2dcd425df83c1891649aee552a1dc3d8a7762f0b81a4"
+checksum = "42eae5b3191aee3d75f6bca5b99cbed091324017c8b73dcc4c25186aabfd1565"
 dependencies = [
  "async-trait",
+ "ctrlc",
  "drawille",
  "eframe",
  "env_logger",
  "grid",
  "hollywood_macros",
+ "linear_type",
  "nalgebra",
  "petgraph",
  "rand",
  "rand_distr",
  "tokio",
  "tokio-stream",
+ "tracing",
+ "tracing-subscriber",
 ]
 
 [[package]]
 name = "hollywood_macros"
-version = "0.5.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b953d105fc9668630761a7ac38b138224e922bd8454d9085e067e8cd5f706be6"
+checksum = "665d28f7187cb6b3e3724d79edbde37f15693d8291b255e620858ba88e477e54"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "home"
 version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
@@ -2075,39 +2101,39 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+checksum = "e0242819d153cba4b4b05a5a8f2a7e9bbf97b6055b2a002b395c96b5ff3c0222"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "inventory"
-version = "0.3.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
-
-[[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "jni"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a87aa2bb7d2af34197c04845522473242e1aa17c12f4935d5856491a7fb8c97"
 dependencies = [
  "cesu8",
  "cfg-if",
@@ -2123,17 +2149,17 @@
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -2164,17 +2190,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -2185,15 +2211,15 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
@@ -2206,36 +2232,42 @@
 dependencies = [
  "bitflags 2.5.0",
  "libc",
  "redox_syscall 0.4.1",
 ]
 
 [[package]]
+name = "linear_type"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe1b1db2093ba1db1b494c2f29526b6ee00c89343744210cad6c5a04466e8526"
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "litrs"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4ce301924b7887e9d637144fdade93f9dfff9b60981d4ac161db09720d39aa5"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -2276,17 +2308,17 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
@@ -2300,17 +2332,17 @@
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "metal"
 version = "0.27.0"
@@ -2340,17 +2372,17 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
 name = "mio"
@@ -2381,17 +2413,17 @@
  "termcolor",
  "thiserror",
  "unicode-xid",
 ]
 
 [[package]]
 name = "nalgebra"
-version = "0.32.4"
+version = "0.32.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4541eb06dce09c0241ebbaab7102f0a01a0c8994afed2e5d0d66775016e25ac2"
+checksum = "3ea4908d4f23254adda3daa60ffef0f1ac7b8c3e9a864cf3cc154b251908a2ef"
 dependencies = [
  "approx",
  "matrixmultiply",
  "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits",
@@ -2434,15 +2466,15 @@
 dependencies = [
  "bitflags 2.5.0",
  "jni-sys",
  "log",
  "ndk-sys",
  "num_enum",
  "raw-window-handle 0.5.2",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "thiserror",
 ]
 
 [[package]]
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2466,14 +2498,26 @@
  "bitflags 1.3.2",
  "cfg-if",
  "libc",
  "memoffset 0.7.1",
 ]
 
 [[package]]
+name = "nix"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab2156c4fce2f8df6c499cc1c763e4394b7482525bf2a9701c9d79d215f519e4"
+dependencies = [
+ "bitflags 2.5.0",
+ "cfg-if",
+ "cfg_aliases",
+ "libc",
+]
+
+[[package]]
 name = "nohash-hasher"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2bf50223579dc7cdcfb3bfcacf7069ff68243f8c363f62ffa99cf000a6b9c451"
 
 [[package]]
 name = "npyz"
@@ -2483,29 +2527,38 @@
 dependencies = [
  "byteorder",
  "num-bigint",
  "py_literal",
 ]
 
 [[package]]
+name = "nu-ansi-term"
+version = "0.46.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
+dependencies = [
+ "overload",
+ "winapi",
+]
+
+[[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "bytemuck",
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
@@ -2514,28 +2567,27 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -2561,22 +2613,22 @@
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
  "proc-macro-crate 3.1.0",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -2590,35 +2642,24 @@
 checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
 dependencies = [
  "malloc_buf",
  "objc_exception",
 ]
 
 [[package]]
-name = "objc-foundation"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1add1b659e36c9607c7aab864a76c7a4c2760cd0cd2e120f3fb8b952c7e22bf9"
-dependencies = [
- "block",
- "objc",
- "objc_id",
-]
-
-[[package]]
 name = "objc-sys"
 version = "0.2.0-beta.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df3b9834c1e95694a05a828b59f55fa2afec6288359cda67146126b3f90a55d7"
 
 [[package]]
 name = "objc-sys"
-version = "0.3.2"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7c71324e4180d0899963fc83d9d241ac39e699609fc1025a850aadac8257459"
+checksum = "cdb91bdd390c7ce1a8607f35f3ca7151b65afc0ff5ff3b34fa350f7d7c7e4310"
 
 [[package]]
 name = "objc2"
 version = "0.3.0-beta.3.patch-leaks.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e01640f9f2cb1220bbe80325e179e532cb3379ebcd1bf2279d703c19fe3a468"
 dependencies = [
@@ -2629,19 +2670,69 @@
 
 [[package]]
 name = "objc2"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "559c5a40fdd30eb5e344fbceacf7595a81e242529fb4e21cf5f43fb4f11ff98d"
 dependencies = [
- "objc-sys 0.3.2",
+ "objc-sys 0.3.5",
  "objc2-encode 3.0.0",
 ]
 
 [[package]]
+name = "objc2"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "46a785d4eeff09c14c487497c162e92766fbb3e4059a71840cecc03d9a50b804"
+dependencies = [
+ "objc-sys 0.3.5",
+ "objc2-encode 4.0.3",
+]
+
+[[package]]
+name = "objc2-app-kit"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4e89ad9e3d7d297152b17d39ed92cd50ca8063a89a9fa569046d41568891eff"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2 0.5.1",
+ "libc",
+ "objc2 0.5.2",
+ "objc2-core-data",
+ "objc2-core-image",
+ "objc2-foundation",
+ "objc2-quartz-core",
+]
+
+[[package]]
+name = "objc2-core-data"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "617fbf49e071c178c0b24c080767db52958f716d9eabdf0890523aeae54773ef"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2 0.5.1",
+ "objc2 0.5.2",
+ "objc2-foundation",
+]
+
+[[package]]
+name = "objc2-core-image"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55260963a527c99f1819c4f8e3b47fe04f9650694ef348ffd2227e8196d34c80"
+dependencies = [
+ "block2 0.5.1",
+ "objc2 0.5.2",
+ "objc2-foundation",
+ "objc2-metal",
+]
+
+[[package]]
 name = "objc2-encode"
 version = "2.0.0-pre.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abfcac41015b00a120608fdaa6938c44cb983fee294351cc4bac7638b4e50512"
 dependencies = [
  "objc-sys 0.2.0-beta.2",
 ]
@@ -2649,29 +2740,63 @@
 [[package]]
 name = "objc2-encode"
 version = "3.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
 
 [[package]]
-name = "objc_exception"
-version = "0.1.2"
+name = "objc2-encode"
+version = "4.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad970fb455818ad6cba4c122ad012fae53ae8b4795f86378bce65e4f6bab2ca4"
+checksum = "7891e71393cd1f227313c9379a26a584ff3d7e6e7159e988851f0934c993f0f8"
+
+[[package]]
+name = "objc2-foundation"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ee638a5da3799329310ad4cfa62fbf045d5f56e3ef5ba4149e7452dcf89d5a8"
 dependencies = [
- "cc",
+ "bitflags 2.5.0",
+ "block2 0.5.1",
+ "libc",
+ "objc2 0.5.2",
 ]
 
 [[package]]
-name = "objc_id"
-version = "0.1.1"
+name = "objc2-metal"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c92d4ddb4bd7b50d730c215ff871754d0da6b2178849f8a2a2ab69712d0c073b"
+checksum = "dd0cba1276f6023976a406a14ffa85e1fdd19df6b0f737b063b95f6c8c7aadd6"
 dependencies = [
- "objc",
+ "bitflags 2.5.0",
+ "block2 0.5.1",
+ "objc2 0.5.2",
+ "objc2-foundation",
+]
+
+[[package]]
+name = "objc2-quartz-core"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e42bee7bff906b14b167da2bac5efe6b6a07e6f7c0a21a7308d40c960242dc7a"
+dependencies = [
+ "bitflags 2.5.0",
+ "block2 0.5.1",
+ "objc2 0.5.2",
+ "objc2-foundation",
+ "objc2-metal",
+]
+
+[[package]]
+name = "objc_exception"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad970fb455818ad6cba4c122ad012fae53ae8b4795f86378bce65e4f6bab2ca4"
+dependencies = [
+ "cc",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
@@ -2701,138 +2826,144 @@
 checksum = "9aa2b01e1d916879f73a53d01d1d6cee68adbb31d6d9177a8cfce093cced1d50"
 dependencies = [
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "overload"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
+
+[[package]]
 name = "owned_ttf_parser"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4586edfe4c648c71797a74c84bacb32b52b212eff5dfe2bb9f2c599844023e7"
+checksum = "6b41438d2fc63c46c74a2203bf5ccd82c41ba04347b2fcf5754f230b167067d5"
 dependencies = [
  "ttf-parser",
 ]
 
 [[package]]
 name = "parking"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.4.1",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.8"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56f8023d0fb78c8e03784ea1c7f3fa36e68a723138990b8d5a47d916b651e7a8"
+checksum = "560131c633294438da9f7c4b08189194b20946c8274c6b9e38881a7874dc8ee8"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.7.8"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0d24f72393fd16ab6ac5738bc33cdb6a9aa73f8b902e8fe29cf4e67d7dd1026"
+checksum = "26293c9193fbca7b1a3bf9b79dc1e388e927e6cacaa78b4a3ab705a1d3d41459"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.7.8"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fdc17e2a6c7d0a492f0158d7a4bd66cc17280308bbaff78d5bef566dca35ab80"
+checksum = "3ec22af7d3fb470a85dd2ca96b7c577a1eb4ef6f1683a9fe9a8c16e136c04687"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.7.8"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "934cd7631c050f4674352a6e835d5f6711ffbfb9345c2fc0107155ac495ae293"
+checksum = "d7a240022f37c361ec1878d646fc5b7d7c4d28d5946e1a80ad5a7a4f4ca0bdcd"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
 name = "petgraph"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
+checksum = "b4c5cc86750666a3ed20bdaf5ca2a0344f9c67674cae0515bec2da16fbaa47db"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "piper"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "668d31b1c4eba19242f2088b2bf3316b82ca31082a8335764db4e083db7485d4"
+checksum = "464db0c665917b13ebb5d453ccdec4add5658ee1adc7affc7677615356a8afaf"
 dependencies = [
  "atomic-waker",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-io",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2865,23 +2996,23 @@
  "log",
  "pin-project-lite",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "polling"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0c976a60b2d7e99d6f229e414670a9b85d13ac305cc6d1e9c134de58c5aaaf6"
+checksum = "645493cf344456ef24219d02a768cf1fb92ddf8c92161679ae3d91b91a637be3"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
  "hermit-abi",
  "pin-project-lite",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "pollster"
 version = "0.3.0"
@@ -2923,32 +3054,32 @@
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
  "toml_edit 0.21.1",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "profiling"
 version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43d84d1d7a6ac92673717f9f6d1518374ef257669c24ebc5ac25d5033828be58"
 
 [[package]]
 name = "pulp"
-version = "0.18.9"
+version = "0.18.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03457ac216146f43f921500bac4e892d5cd32b0479b929cbfc90f95cd6c599c2"
+checksum = "0ec8d02258294f59e4e223b41ad7e81c874aa6b15bc4ced9ba3965826da0eed5"
 dependencies = [
  "bytemuck",
  "libm",
  "num-complex",
  "reborrow",
 ]
 
@@ -2963,90 +3094,89 @@
  "num-traits",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
- "inventory",
  "libc",
- "memoffset 0.9.0",
+ "memoffset 0.9.1",
  "parking_lot",
  "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -3106,17 +3236,17 @@
 name = "raw-window-handle"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
 name = "raw-window-handle"
-version = "0.6.0"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42a9830a0e1b9fb145ebb365b8bc4ccd75f290f98c0247deafbbe2c75cefb544"
+checksum = "20675572f6f24e9e76ef639bc5552774ed45f1c30e2951e1e99c59888861c539"
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
@@ -3161,14 +3291,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
@@ -3185,29 +3324,29 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "renderdoc-sys"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b30a45b0cd0bcca8037f3d0dc3421eaf95327a17cad11964fb8179b4fc4832"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -3223,22 +3362,22 @@
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
- "linux-raw-sys 0.4.13",
+ "linux-raw-sys 0.4.14",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "safe_arch"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3285,41 +3424,41 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.18"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
+checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sha1"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
@@ -3337,18 +3476,27 @@
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
+name = "sharded-slab"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
+dependencies = [
+ "lazy_static",
+]
+
+[[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simba"
 version = "0.8.1"
@@ -3374,14 +3522,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "sleef"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9fe16088049a19013d5736660a666dae8e1dbb78dd1ced530a396a7bab4ef47d"
+dependencies = [
+ "doubled",
+]
+
+[[package]]
 name = "slotmap"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dbff4acf519f630b3a3ddcfaea6c06b42174d9a44bc70c620e9ed1649d58b82a"
 dependencies = [
  "version_check",
 ]
@@ -3401,15 +3558,15 @@
  "bitflags 2.5.0",
  "calloop",
  "calloop-wayland-source",
  "cursor-icon",
  "libc",
  "log",
  "memmap2",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "thiserror",
  "wayland-backend",
  "wayland-client",
  "wayland-csd-frame",
  "wayland-cursor",
  "wayland-protocols",
  "wayland-protocols-wlr",
@@ -3426,17 +3583,17 @@
  "libc",
  "smithay-client-toolkit",
  "wayland-backend",
 ]
 
 [[package]]
 name = "smol_str"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6845563ada680337a52d43bb0b29f396f2d911616f6573012645b9e3d048a49"
+checksum = "dd538fb6910ac1099850255cf94a94df6551fbdd602454387d0adb2d1ca6dead"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "socket2"
 version = "0.4.10"
@@ -3445,134 +3602,146 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "sophus"
-version = "0.4.0"
+version = "0.6.0"
 dependencies = [
  "approx",
  "assertables",
  "bytemuck",
  "eframe",
  "egui_extras",
  "env_logger",
  "hollywood",
  "nalgebra",
  "ndarray",
- "sophus_calculus",
+ "sophus_core",
  "sophus_image",
  "sophus_lie",
  "sophus_opt",
+ "sophus_pyo3",
  "sophus_sensor",
- "sophus_tensor",
+ "sophus_viewer",
  "tokio",
  "wgpu",
 ]
 
 [[package]]
-name = "sophus_calculus"
-version = "0.4.0"
+name = "sophus_core"
+version = "0.6.0"
 dependencies = [
  "approx",
  "assertables",
+ "concat-arrays",
  "nalgebra",
+ "ndarray",
  "num-traits",
- "simba",
- "sophus_tensor",
+ "sleef",
+ "typenum",
 ]
 
 [[package]]
 name = "sophus_image"
-version = "0.4.0"
+version = "0.6.0"
 dependencies = [
  "approx",
  "assertables",
  "bytemuck",
  "nalgebra",
  "ndarray",
+ "num-traits",
  "png",
- "sophus_tensor",
+ "sophus_core",
 ]
 
 [[package]]
 name = "sophus_lie"
-version = "0.4.0"
+version = "0.6.0"
 dependencies = [
  "approx",
  "assertables",
  "nalgebra",
- "sophus_calculus",
- "sophus_tensor",
+ "num-traits",
+ "sophus_core",
 ]
 
 [[package]]
 name = "sophus_opt"
-version = "0.4.0"
+version = "0.6.0"
 dependencies = [
  "approx",
  "as-any",
  "assertables",
  "dyn-clone",
  "faer",
  "nalgebra",
  "ndarray",
  "rand",
- "sophus_calculus",
+ "sophus_core",
  "sophus_image",
  "sophus_lie",
  "sophus_sensor",
 ]
 
 [[package]]
 name = "sophus_pyo3"
-version = "0.4.0"
+version = "0.6.0"
 dependencies = [
  "nalgebra",
  "numpy",
  "pyo3",
- "sophus_calculus",
+ "sophus_core",
  "sophus_lie",
- "sophus_tensor",
 ]
 
 [[package]]
 name = "sophus_sensor"
-version = "0.4.0"
+version = "0.6.0"
 dependencies = [
  "approx",
  "assertables",
  "nalgebra",
  "ndarray",
- "sophus_calculus",
+ "num-traits",
+ "sophus_core",
  "sophus_image",
 ]
 
 [[package]]
-name = "sophus_tensor"
-version = "0.4.0"
+name = "sophus_viewer"
+version = "0.6.0"
 dependencies = [
+ "approx",
  "assertables",
- "concat-arrays",
+ "bytemuck",
+ "eframe",
+ "egui_extras",
+ "env_logger",
+ "hollywood",
  "nalgebra",
  "ndarray",
- "num-traits",
- "simba",
- "typenum",
+ "sophus_core",
+ "sophus_image",
+ "sophus_lie",
+ "sophus_sensor",
+ "tokio",
+ "wgpu",
 ]
 
 [[package]]
 name = "spirv"
 version = "0.3.0+sdk-1.3.268.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eda41003dc44290527a59b13432d4a0379379fa074b70174882adfbdfd917844"
@@ -3601,17 +3770,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3637,46 +3806,56 @@
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
- "fastrand 2.0.2",
- "rustix 0.38.32",
+ "fastrand 2.1.0",
+ "rustix 0.38.34",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "thread_local"
+version = "1.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
+dependencies = [
+ "cfg-if",
+ "once_cell",
 ]
 
 [[package]]
 name = "tiny-skia"
 version = "0.11.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83d13394d44dae3207b52a326c0c85a8bf87f1541f23b0d143811088497b09ab"
@@ -3713,40 +3892,40 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2 0.5.6",
+ "socket2 0.5.7",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "267ac89e0bec6e691e5813911606935d77c476ff49024f98abcea3e7b15e37af"
@@ -3754,17 +3933,17 @@
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 
 [[package]]
 name = "toml_edit"
 version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
@@ -3799,31 +3978,57 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
+ "valuable",
+]
+
+[[package]]
+name = "tracing-log"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
+dependencies = [
+ "log",
+ "once_cell",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-subscriber"
+version = "0.3.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
+dependencies = [
+ "nu-ansi-term",
+ "sharded-slab",
+ "smallvec",
+ "thread_local",
+ "tracing-core",
+ "tracing-log",
 ]
 
 [[package]]
 name = "ttf-parser"
-version = "0.20.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f77d76d837a7830fe1d4f12b7b4ba4192c1888001c7164257e4bc6d21d96b4"
+checksum = "2c591d83f69777866b9126b24c6dd9a18351f177e49d625920d19f989fd31cf8"
 
 [[package]]
 name = "type-map"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "deb68604048ff8fa93347f02441e4487594adc20bb8a084f9e564d2b827a0a9f"
 dependencies = [
@@ -3844,15 +4049,15 @@
 
 [[package]]
 name = "uds_windows"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89daebc3e6fd160ac4aa9fc8b3bf71e1f74fbf92367ae71fb83a037e8bf164b9"
 dependencies = [
- "memoffset 0.9.0",
+ "memoffset 0.9.1",
  "tempfile",
  "winapi",
 ]
 
 [[package]]
 name = "unicase"
 version = "2.7.0"
@@ -3887,17 +4092,17 @@
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
@@ -3921,24 +4126,30 @@
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
+name = "valuable"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "waker-fn"
-version = "1.1.1"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3c4517f54858c779bbcbf228f4fca63d121bf85fbecb2dc578cdf4a39395690"
+checksum = "317211a0dc0ceedd78fb2ca9a44aed3d7b9b26f81870d485c07122b4350673b7"
 
 [[package]]
 name = "walkdir"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
@@ -3969,15 +4180,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4003,15 +4214,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -4022,28 +4233,28 @@
 name = "wayland-backend"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d50fa61ce90d76474c87f5fc002828d81b32677340112b4ef08079a9d459a40"
 dependencies = [
  "cc",
  "downcast-rs",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "scoped-tls",
  "smallvec",
  "wayland-sys",
 ]
 
 [[package]]
 name = "wayland-client"
 version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
 dependencies = [
  "bitflags 2.5.0",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "wayland-backend",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-csd-frame"
 version = "0.3.0"
@@ -4057,15 +4268,15 @@
 
 [[package]]
 name = "wayland-cursor"
 version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "71ce5fa868dd13d11a0d04c5e2e65726d0897be8de247c0c5a65886e283231ba"
 dependencies = [
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "wayland-client",
  "xcursor",
 ]
 
 [[package]]
 name = "wayland-protocols"
 version = "0.31.2"
@@ -4145,85 +4356,85 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webbrowser"
-version = "0.8.13"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1b04c569c83a9bb971dd47ec6fd48753315f4bf989b9b04a2e7ca4d7f0dc950"
+checksum = "db67ae75a9405634f5882791678772c94ff5f16a66535aae186e26aa0841fc8b"
 dependencies = [
  "core-foundation",
  "home",
  "jni",
  "log",
  "ndk-context",
  "objc",
  "raw-window-handle 0.5.2",
  "url",
  "web-sys",
 ]
 
 [[package]]
 name = "wgpu"
-version = "0.19.3"
+version = "0.19.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4b1213b52478a7631d6e387543ed8f642bc02c578ef4e3b49aca2a29a7df0cb"
+checksum = "cbd7311dbd2abcfebaabf1841a2824ed7c8be443a0f29166e5d3c6a53a762c01"
 dependencies = [
  "arrayvec",
  "cfg-if",
  "cfg_aliases",
  "js-sys",
  "log",
  "naga",
  "parking_lot",
  "profiling",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "smallvec",
  "static_assertions",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "wgpu-core",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-core"
-version = "0.19.3"
+version = "0.19.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9f6b033c2f00ae0bc8ea872c5989777c60bc241aac4e58b24774faa8b391f78"
+checksum = "28b94525fc99ba9e5c9a9e24764f2bc29bad0911a7446c12f446a8277369bf3a"
 dependencies = [
  "arrayvec",
  "bit-vec",
  "bitflags 2.5.0",
  "cfg_aliases",
  "codespan-reporting",
  "indexmap",
  "log",
  "naga",
  "once_cell",
  "parking_lot",
  "profiling",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "rustc-hash",
  "smallvec",
  "thiserror",
  "web-sys",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-hal"
-version = "0.19.3"
+version = "0.19.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49f972c280505ab52ffe17e94a7413d9d54b58af0114ab226b9fc4999a47082e"
+checksum = "fc1a4924366df7ab41a5d8546d6534f1f33231aa5b3f72b9930e300f254e39c3"
 dependencies = [
  "android_system_properties",
  "arrayvec",
  "ash",
  "bit-set",
  "bitflags 2.5.0",
  "block",
@@ -4245,15 +4456,15 @@
  "naga",
  "ndk-sys",
  "objc",
  "once_cell",
  "parking_lot",
  "profiling",
  "range-alloc",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "renderdoc-sys",
  "rustc-hash",
  "smallvec",
  "thiserror",
  "wasm-bindgen",
  "web-sys",
  "wgpu-types",
@@ -4269,27 +4480,27 @@
  "bitflags 2.5.0",
  "js-sys",
  "web-sys",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.15"
+version = "0.7.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
+checksum = "cd8dc749a1b03f3c255a3064a4f5c0ee5ed09b7c6bc6d4525d31f779cd74d7fc"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "widestring"
-version = "1.0.2"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "653f141f39ec16bba3c5abe400a0c60da7468261cc2cbf36805022876bc721a8"
+checksum = "7219d36b6eac893fa81e84ebe06485e7dcbb616177469b142df14f1f4deb1311"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -4301,19 +4512,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -4332,24 +4543,24 @@
 [[package]]
 name = "windows"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-implement"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e2ee588991b9e7e6c8338edf3333fbe4da35dc72092643958ebb43f0ab2c49c"
@@ -4390,15 +4601,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -4425,25 +4636,26 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
@@ -4452,17 +4664,17 @@
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
@@ -4470,17 +4682,17 @@
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
@@ -4488,17 +4700,23 @@
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
@@ -4506,17 +4724,17 @@
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
@@ -4524,17 +4742,17 @@
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
@@ -4542,17 +4760,17 @@
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
@@ -4560,17 +4778,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winit"
 version = "0.29.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
 dependencies = [
@@ -4592,17 +4810,17 @@
  "ndk",
  "ndk-sys",
  "objc2 0.4.1",
  "once_cell",
  "orbclient",
  "percent-encoding",
  "raw-window-handle 0.5.2",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.2",
  "redox_syscall 0.3.5",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "sctk-adwaita",
  "smithay-client-toolkit",
  "smol_str",
  "unicode-segmentation",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wayland-backend",
@@ -4635,32 +4853,32 @@
  "libc",
  "once_cell",
  "pkg-config",
 ]
 
 [[package]]
 name = "x11rb"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
+checksum = "5d91ffca73ee7f68ce055750bf9f6eca0780b8c85eff9bc046a3b0da41755e12"
 dependencies = [
  "as-raw-xcb-connection",
  "gethostname",
  "libc",
  "libloading 0.8.3",
  "once_cell",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "x11rb-protocol",
 ]
 
 [[package]]
 name = "x11rb-protocol"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
+checksum = "ec107c4503ea0b4a98ef47356329af139c0a4f7750e621cf2973cd3385ebcb3d"
 
 [[package]]
 name = "xcursor"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a0ccd7b4a5345edfcd0c3535718a4e9ff7798ffc536bb5b5a0e26ff84732911"
 
@@ -4691,17 +4909,17 @@
 name = "xkeysym"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "054a8e68b76250b253f671d1268cb7f1ae089ec35e195b2efb2a4e9a836d0621"
 
 [[package]]
 name = "xml-rs"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fcb9cbac069e033553e8bb871be2fbdffcab578eb25bd0f7c508cedc6dcd75a"
+checksum = "791978798f0597cfc70478424c2b4fdc2b7a8024aaff78497ef00f24ef674193"
 
 [[package]]
 name = "zbus"
 version = "3.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "675d170b632a6ad49804c8cf2105d7c31eddd3312555cffd4b740e08e97c25e6"
 dependencies = [
@@ -4719,15 +4937,15 @@
  "derivative",
  "enumflags2",
  "event-listener 2.5.3",
  "futures-core",
  "futures-sink",
  "futures-util",
  "hex",
- "nix",
+ "nix 0.26.4",
  "once_cell",
  "ordered-stream",
  "rand",
  "serde",
  "serde_repr",
  "sha1",
  "static_assertions",
@@ -4763,30 +4981,30 @@
  "serde",
  "static_assertions",
  "zvariant",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zvariant"
 version = "3.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4eef2be88ba09b358d3b58aca6e41cd853631d44787f319a1383ca83424fb2db"
```

### Comparing `sophus_pyo3-0.4.0/Cargo.toml` & `sophus_pyo3-0.6.0/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -8,57 +8,51 @@
   "**/*.rs",
   "**/*.wgsl",
   "Cargo.toml",
 ]
 keywords = ["robotics", "optimization"]
 license = "MIT OR Apache-2.0"
 repository = "https://github.com/farm-ng/sophus-rs/"
-version = "0.4.0"
+version = "0.6.0"
 
 [workspace.dependencies]
-sophus = {path = "crates/sophus", version = "0.4.0"}
-sophus_calculus = {path = "crates/sophus_calculus", version = "0.4.0"}
-sophus_image = {path = "crates/sophus_image", version = "0.4.0"}
-sophus_lie = {path = "crates/sophus_lie", version = "0.4.0"}
-sophus_opt = {path = "crates/sophus_opt", version = "0.4.0"}
-sophus_sensor = {path = "crates/sophus_sensor", version = "0.4.0"}
-sophus_tensor = {path = "crates/sophus_tensor", version = "0.4.0"}
+sophus = {path = "crates/sophus", version = "0.6.0"}
+sophus_core = {path = "crates/sophus_core", version = "0.6.0"}
+sophus_image = {path = "crates/sophus_image", version = "0.6.0"}
+sophus_lie = {path = "crates/sophus_lie", version = "0.6.0"}
+sophus_opt = {path = "crates/sophus_opt", version = "0.6.0"}
+sophus_pyo3 = {path = "crates/sophus_pyo3", version = "0.6.0"}
+sophus_sensor = {path = "crates/sophus_sensor", version = "0.6.0"}
+sophus_viewer = {path = "crates/sophus_viewer", version = "0.6.0"}
 
-approx = {version = "0.5.1"}
-as-any = "0.3.1"
-assertables = "7.0.1"
-async-trait = "0.1.77"
-bytemuck = {version = "1.14.0", features = ["derive"]}
-concat-arrays = "0.1.2"
-dyn-clone = "1.0.16"
-eframe = {version = "0.26", features = ["wgpu"]}
-egui_extras = "0.26"
+approx = "0.5"
+as-any = "0.3"
+assertables = "7.0"
+async-trait = "0.1"
+bytemuck = {version = "1.14", features = ["derive"]}
+concat-arrays = "0.1"
+dyn-clone = "1.0"
+eframe = {version = "0.27", features = ["wgpu"]}
+egui_extras = "0.27"
 env_logger = "0.11"
 faer = "0.18"
-hollywood = "0.5.0"
+hollywood = {version = "0.7.0"}
 image = {version = "0.25", features = [
   "jpeg",
   "png",
-  "tga",
-  "gif",
-  "ico",
-  "bmp",
-  "hdr",
   "tiff",
-  "avif",
-  "webp",
 ]}
-log = "0.4.14"
+log = "0.4"
 nalgebra = {version = "0.32", features = ["rand"]}
-ndarray = {version = "0.15.4", features = ["approx-0_5"]}
-num-traits = "0.2.15"
-numpy = "0.20"
-png = "0.17.11"
-rand = "0.8.5"
-simba = "0.8.1"
+ndarray = {version = "0.15", features = ["approx-0_5"]}
+num-traits = "0.2"
+numpy = "0.21"
+png = "0.17"
+rand = "0.8"
+sleef = "0.3"
 tokio = {version = "1", features = ["full"]}
-typenum = {version = "1.17.0", features = ["const-generics"]}
+typenum = {version = "1.17", features = ["const-generics"]}
 wgpu = "0.19"
-winit = {version = "0.29", features = ["android-native-activity"]}
+winit = {version = "0.30", features = ["android-native-activity"]}
 
 [profile.release]
 debug = 1
```

