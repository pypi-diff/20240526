# Comparing `tmp/breedgym-0.0.1a0.tar.gz` & `tmp/breedgym-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breedgym-0.0.1a0.tar", last modified: Thu Nov 23 00:39:09 2023, max compression
+gzip compressed data, was "breedgym-0.0.2a0.tar", last modified: Sun May 26 18:10:54 2024, max compression
```

## Comparing `breedgym-0.0.1a0.tar` & `breedgym-0.0.2a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.438622 breedgym-0.0.1a0/
--rw-r--r--   0 omar       (501) staff       (20)     1501 2023-11-23 00:23:42.000000 breedgym-0.0.1a0/LICENSE
--rw-r--r--   0 omar       (501) staff       (20)       37 2023-11-23 00:30:23.000000 breedgym-0.0.1a0/MANIFEST.in
--rw-r--r--   0 omar       (501) staff       (20)     1002 2023-11-23 00:39:09.438470 breedgym-0.0.1a0/PKG-INFO
--rw-r--r--   0 omar       (501) staff       (20)      128 2023-11-22 06:03:20.000000 breedgym-0.0.1a0/README.md
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.418748 breedgym-0.0.1a0/breedgym/
--rw-r--r--   0 omar       (501) staff       (20)      643 2023-11-23 00:23:42.000000 breedgym-0.0.1a0/breedgym/__init__.py
--rw-r--r--   0 omar       (501) staff       (20)     8330 2023-11-23 00:30:16.000000 breedgym-0.0.1a0/breedgym/breedgym.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.419805 breedgym-0.0.1a0/breedgym/data/
--rw-r--r--   0 omar       (501) staff       (20)  7400128 2023-11-22 06:03:20.000000 breedgym-0.0.1a0/breedgym/data/small_geno.npy
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.433905 breedgym-0.0.1a0/breedgym/utils/
--rw-r--r--   0 omar       (501) staff       (20)        0 2023-11-22 06:29:24.000000 breedgym-0.0.1a0/breedgym/utils/__init__.py
--rw-r--r--   0 omar       (501) staff       (20)     3640 2023-11-22 06:18:09.000000 breedgym-0.0.1a0/breedgym/utils/index_functions.py
--rw-r--r--   0 omar       (501) staff       (20)      252 2023-11-22 23:01:36.000000 breedgym-0.0.1a0/breedgym/utils/paths.py
--rw-r--r--   0 omar       (501) staff       (20)     1480 2023-11-22 23:01:36.000000 breedgym-0.0.1a0/breedgym/utils/plot_utils.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.436416 breedgym-0.0.1a0/breedgym/vector/
--rw-r--r--   0 omar       (501) staff       (20)      279 2023-11-22 23:01:36.000000 breedgym-0.0.1a0/breedgym/vector/__init__.py
--rw-r--r--   0 omar       (501) staff       (20)     2680 2023-11-22 06:16:43.000000 breedgym-0.0.1a0/breedgym/vector/breeding_programs_env.py
--rw-r--r--   0 omar       (501) staff       (20)     8052 2023-11-23 00:29:42.000000 breedgym-0.0.1a0/breedgym/vector/vec_env.py
--rw-r--r--   0 omar       (501) staff       (20)     5367 2023-11-23 00:23:42.000000 breedgym-0.0.1a0/breedgym/vector/vec_wrappers.py
--rw-r--r--   0 omar       (501) staff       (20)     4129 2023-11-22 06:41:25.000000 breedgym-0.0.1a0/breedgym/wrappers.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.419642 breedgym-0.0.1a0/breedgym.egg-info/
--rw-r--r--   0 omar       (501) staff       (20)     1002 2023-11-23 00:39:09.000000 breedgym-0.0.1a0/breedgym.egg-info/PKG-INFO
--rw-r--r--   0 omar       (501) staff       (20)      605 2023-11-23 00:39:09.000000 breedgym-0.0.1a0/breedgym.egg-info/SOURCES.txt
--rw-r--r--   0 omar       (501) staff       (20)        1 2023-11-23 00:39:09.000000 breedgym-0.0.1a0/breedgym.egg-info/dependency_links.txt
--rw-r--r--   0 omar       (501) staff       (20)      105 2023-11-23 00:39:09.000000 breedgym-0.0.1a0/breedgym.egg-info/requires.txt
--rw-r--r--   0 omar       (501) staff       (20)        9 2023-11-23 00:39:09.000000 breedgym-0.0.1a0/breedgym.egg-info/top_level.txt
--rw-r--r--   0 omar       (501) staff       (20)     1515 2023-11-22 22:56:53.000000 breedgym-0.0.1a0/pyproject.toml
--rw-r--r--   0 omar       (501) staff       (20)       38 2023-11-23 00:39:09.438693 breedgym-0.0.1a0/setup.cfg
--rw-r--r--   0 omar       (501) staff       (20)       72 2023-11-22 22:48:32.000000 breedgym-0.0.1a0/setup.py
-drwxr-xr-x   0 omar       (501) staff       (20)        0 2023-11-23 00:39:09.437949 breedgym-0.0.1a0/tests/
--rw-r--r--   0 omar       (501) staff       (20)     2701 2023-11-22 06:16:43.000000 breedgym-0.0.1a0/tests/test_env.py
--rw-r--r--   0 omar       (501) staff       (20)     6060 2023-11-23 00:23:42.000000 breedgym-0.0.1a0/tests/test_vec.py
--rw-r--r--   0 omar       (501) staff       (20)     2515 2023-11-22 06:51:57.000000 breedgym-0.0.1a0/tests/test_wrappers.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.440273 breedgym-0.0.2a0/
+-rw-r--r--   0 omar       (501) staff       (20)     1501 2023-11-23 00:23:42.000000 breedgym-0.0.2a0/LICENSE
+-rw-r--r--   0 omar       (501) staff       (20)       37 2023-11-23 00:30:23.000000 breedgym-0.0.2a0/MANIFEST.in
+-rw-r--r--   0 omar       (501) staff       (20)     2906 2024-05-26 18:10:54.440139 breedgym-0.0.2a0/PKG-INFO
+-rw-r--r--   0 omar       (501) staff       (20)     2031 2024-05-26 17:11:58.000000 breedgym-0.0.2a0/README.md
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.426593 breedgym-0.0.2a0/breedgym/
+-rw-r--r--   0 omar       (501) staff       (20)      643 2023-11-23 00:23:42.000000 breedgym-0.0.2a0/breedgym/__init__.py
+-rw-r--r--   0 omar       (501) staff       (20)     8330 2024-05-26 17:53:45.000000 breedgym-0.0.2a0/breedgym/breedgym.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.427410 breedgym-0.0.2a0/breedgym/data/
+-rw-r--r--   0 omar       (501) staff       (20)  7400128 2023-11-22 06:03:20.000000 breedgym-0.0.2a0/breedgym/data/small_geno.npy
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.438498 breedgym-0.0.2a0/breedgym/utils/
+-rw-r--r--   0 omar       (501) staff       (20)        0 2023-11-22 06:29:24.000000 breedgym-0.0.2a0/breedgym/utils/__init__.py
+-rw-r--r--   0 omar       (501) staff       (20)     3640 2023-11-22 06:18:09.000000 breedgym-0.0.2a0/breedgym/utils/index_functions.py
+-rw-r--r--   0 omar       (501) staff       (20)      252 2023-11-22 23:01:36.000000 breedgym-0.0.2a0/breedgym/utils/paths.py
+-rw-r--r--   0 omar       (501) staff       (20)     1480 2023-11-22 23:01:36.000000 breedgym-0.0.2a0/breedgym/utils/plot_utils.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.439091 breedgym-0.0.2a0/breedgym/vector/
+-rw-r--r--   0 omar       (501) staff       (20)      279 2023-11-22 23:01:36.000000 breedgym-0.0.2a0/breedgym/vector/__init__.py
+-rw-r--r--   0 omar       (501) staff       (20)     2686 2024-05-26 17:53:11.000000 breedgym-0.0.2a0/breedgym/vector/breeding_programs_env.py
+-rw-r--r--   0 omar       (501) staff       (20)     8030 2024-05-26 17:17:32.000000 breedgym-0.0.2a0/breedgym/vector/vec_env.py
+-rw-r--r--   0 omar       (501) staff       (20)     5470 2024-05-26 17:17:05.000000 breedgym-0.0.2a0/breedgym/vector/vec_wrappers.py
+-rw-r--r--   0 omar       (501) staff       (20)     4132 2024-05-26 17:52:38.000000 breedgym-0.0.2a0/breedgym/wrappers.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.427261 breedgym-0.0.2a0/breedgym.egg-info/
+-rw-r--r--   0 omar       (501) staff       (20)     2906 2024-05-26 18:10:54.000000 breedgym-0.0.2a0/breedgym.egg-info/PKG-INFO
+-rw-r--r--   0 omar       (501) staff       (20)      605 2024-05-26 18:10:54.000000 breedgym-0.0.2a0/breedgym.egg-info/SOURCES.txt
+-rw-r--r--   0 omar       (501) staff       (20)        1 2024-05-26 18:10:54.000000 breedgym-0.0.2a0/breedgym.egg-info/dependency_links.txt
+-rw-r--r--   0 omar       (501) staff       (20)      105 2024-05-26 18:10:54.000000 breedgym-0.0.2a0/breedgym.egg-info/requires.txt
+-rw-r--r--   0 omar       (501) staff       (20)        9 2024-05-26 18:10:54.000000 breedgym-0.0.2a0/breedgym.egg-info/top_level.txt
+-rw-r--r--   0 omar       (501) staff       (20)     1516 2024-05-26 18:00:48.000000 breedgym-0.0.2a0/pyproject.toml
+-rw-r--r--   0 omar       (501) staff       (20)       38 2024-05-26 18:10:54.440319 breedgym-0.0.2a0/setup.cfg
+-rw-r--r--   0 omar       (501) staff       (20)       72 2024-05-26 18:05:17.000000 breedgym-0.0.2a0/setup.py
+drwxr-xr-x   0 omar       (501) staff       (20)        0 2024-05-26 18:10:54.439790 breedgym-0.0.2a0/tests/
+-rw-r--r--   0 omar       (501) staff       (20)     2785 2024-05-26 17:48:32.000000 breedgym-0.0.2a0/tests/test_env.py
+-rw-r--r--   0 omar       (501) staff       (20)     6062 2024-05-26 17:43:26.000000 breedgym-0.0.2a0/tests/test_vec.py
+-rw-r--r--   0 omar       (501) staff       (20)     2542 2024-05-26 18:03:37.000000 breedgym-0.0.2a0/tests/test_wrappers.py
```

### Comparing `breedgym-0.0.1a0/LICENSE` & `breedgym-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/breedgym/__init__.py` & `breedgym-0.0.2a0/breedgym/__init__.py`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/breedgym/breedgym.py` & `breedgym-0.0.2a0/breedgym/breedgym.py`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/breedgym/data/small_geno.npy` & `breedgym-0.0.2a0/breedgym/data/small_geno.npy`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/breedgym/utils/index_functions.py` & `breedgym-0.0.2a0/breedgym/utils/index_functions.py`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/breedgym/utils/plot_utils.py` & `breedgym-0.0.2a0/breedgym/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/breedgym/vector/breeding_programs_env.py` & `breedgym-0.0.2a0/breedgym/vector/breeding_programs_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
     @partial(jax.vmap, in_axes=(None, 0))
     def _double_haploid(self, pop):
         return self.simulator.double_haploid(pop, n_offspring=self.plant_per_line)
 
     @partial(jax.vmap, in_axes=(None, 0))
     def _select_line(self, pop):
-        return self.simulator.select(pop, k=self.k_per_line)
+        return self.simulator.select(pop, k=self.k_per_line)[0]
 
     def step(self, actions):
         actions = self._convert_actions(actions)
         arange_envs = np.arange(self.num_envs)[:, None, None]
         parents = self.populations[arange_envs, actions]
         pop = self.cross(parents)
         assert pop.shape[1] == self.n_lines
         pop = self._double_haploid(pop)
         pop = self._select_line(pop)
         pop = pop.reshape(pop.shape[0], pop.shape[1] * pop.shape[2], *pop.shape[3:])
-        self.env.populations = self.simulator.select(pop, k=self.individual_per_gen)
+        self.env.populations, _ = self.simulator.select(pop, k=self.individual_per_gen)
 
         self.env.step_idx += 1
         infos = self.get_info()
         done = self.env.step_idx == self.num_generations
         if self.reward_shaping or done:
             rews = np.max(infos["GEBV"], axis=(1, 2))
             rews = np.asarray(rews)
```

### Comparing `breedgym-0.0.1a0/breedgym/vector/vec_env.py` & `breedgym-0.0.2a0/breedgym/vector/vec_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 GENOME_FILE = DATA_PATH.joinpath("small_geno.npy")
 
 
 @partial(jax.jit, static_argnums=1)
 @partial(jax.vmap, in_axes=(None, None, 0))
 def _random_selection(
-    germplasm: Population["n"], length: int, key: jax.random.PRNGKeyArray
+    germplasm: Population["n"], length: int, key: jax.Array
 ) -> Population["length"]:
     return jax.random.choice(key, germplasm, shape=(length,), replace=False)
 
 
 class VecBreedGym(VectorEnv):
     def __init__(
         self,
@@ -108,18 +108,18 @@
 
     def reset(
         self, seed: Optional[int] = None, options: Optional[dict] = None
     ) -> Tuple[Population["envs n"], dict]:
         self.step_idx = 0
         if seed is not None:
             self.simulator.set_seed(seed)
-            self.random_key = jax.random.PRNGKey(seed)
+            self.random_key = jax.random.key(seed)
         elif self.random_key is None:
             seed = np.random.randint(2**32)
-            self.random_key = jax.random.PRNGKey(seed)
+            self.random_key = jax.random.key(seed)
 
         keys = jax.random.split(self.random_key, num=self.num_envs + 1)
         self.random_key = keys[0]
 
         if options is not None and "individual_per_gen" in options.keys():
             self.individual_per_gen = options["individual_per_gen"]
```

### Comparing `breedgym-0.0.1a0/breedgym/vector/vec_wrappers.py` & `breedgym-0.0.2a0/breedgym/vector/vec_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         self.action_space = spaces.Box(
             -1e5, 1e5, shape=(self.num_envs, self.individual_per_gen)
         )
 
     @partial(jax.vmap, in_axes=(None, 0, 0))
     def _convert_actions(
-        self, action: Float[Array, "n"], random_key: jax.random.PRNGKeyArray
+        self, action: Float[Array, "n"], random_key: jax.Array
     ) -> Int[Array, "n 2"]:
         _, best_pop = jax.lax.top_k(action, self.k)
         diallel_indices = self.simulator._diallel_indices(best_pop)
 
         random_select_idx = jax.random.choice(
             random_key, len(diallel_indices), shape=(self.n_crosses,), replace=False
         )
@@ -117,15 +117,17 @@
         Population["envs n"],
         Float[Array, "envs"],
         Bool[Array, "envs"],
         Bool[Array, "envs"],
         dict,
     ]:
         low_level_actions = self._convert_actions(actions)
-        return super().step(low_level_actions)
+        obs, rew, ter, tru, infos = super().step(low_level_actions)
+        infos["low_level_actions"] = low_level_actions
+        return obs, rew, ter, tru, infos
 
 
 class RavelIndex(VectorWrapper):
     def __init__(self, vec_env: VecBreedGym):
         super().__init__(vec_env)
         self.action_shape = self.single_action_space.shape
         n_elems = prod(self.action_shape)
```

### Comparing `breedgym-0.0.1a0/breedgym/wrappers.py` & `breedgym-0.0.2a0/breedgym/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         n_offspring = ceil(self.individual_per_gen / n_crosses)
 
         if n_bests < 2:
             raise ValueError("n_bests must be higher or equal to 2")
         if n_crosses > self.individual_per_gen:
             raise ValueError("n_crosses must be lower or equal to individual_per_gen")
 
-        self.unwrapped.population = self.simulator.select(
+        self.unwrapped.population, _ = self.simulator.select(
             population=self.env.population, k=n_bests, f_index=self.f_index
         )
 
         best_idx = np.arange(n_bests)
         diallel_indices = self.simulator._diallel_indices(best_idx)
         random_select_idx = self.np_random.choice(
             len(diallel_indices), n_crosses, replace=False
```

### Comparing `breedgym-0.0.1a0/breedgym.egg-info/SOURCES.txt` & `breedgym-0.0.2a0/breedgym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `breedgym-0.0.1a0/pyproject.toml` & `breedgym-0.0.2a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "breedgym"
 description = "Suite of Gymnasium environments for optimizing breeding programs"
 readme = "README.md"
-requires-python = ">= 3.8"
+requires-python = ">= 3.9"
 authors = [{ name = "Omar G. Younis", email = "omar.g.younis@gmail.com" }]
 license = { text = "BSD-3-Clause" }
 keywords = ["Reinforcement Learning", "Breeding", "genetics", "bioinformatics"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     'Intended Audience :: Science/Research',
 ]
 dependencies = ["numpy", "pandas", "matplotlib", "chromax", "gymnasium>=0.29", "jax", "jaxtyping"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 testing = ["pytest"]
```

### Comparing `breedgym-0.0.1a0/tests/test_env.py` & `breedgym-0.0.2a0/tests/test_env.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pytest
 from chromax.sample_data import genetic_map, genome
 
 
 def test_reset_population():
     env = gym.make(
-        "BreedGym",
+        "breedgym:BreedGym",
         initial_population=genome,
         genetic_map=genetic_map,
     )
 
     pop, _ = env.reset()
     init_pop = np.copy(pop)
 
@@ -18,58 +18,58 @@
     pop, _ = env.reset()
     assert np.all(init_pop == pop)
 
 
 @pytest.mark.parametrize("n", [1, 5, 10])
 def test_num_progenies(n):
     env = gym.make(
-        "BreedGym",
+        "breedgym:BreedGym",
         initial_population=genome,
         genetic_map=genetic_map,
     )
     pop, _ = env.reset()
 
     action = np.random.randint(len(pop), size=(n, 2))
     env.step(action)
 
     assert len(env.population) == n
 
 
 def test_caching():
     env = gym.make(
-        "BreedGym",
+        "breedgym:BreedGym",
         initial_population=genome,
         genetic_map=genetic_map,
     )
     env.reset()
 
-    GEBV = env.GEBV
+    GEBV = env.unwrapped.GEBV
     GEBV_copy = np.copy(GEBV)
-    GEBV2 = env.GEBV
+    GEBV2 = env.unwrapped.GEBV
     assert id(GEBV) == id(GEBV2)
     assert np.all(GEBV_copy == GEBV2)
 
     corrcoef = env.corrcoef
     corrcoef_copy = np.copy(corrcoef)
     corrcoef2 = env.corrcoef
     assert id(corrcoef) == id(corrcoef2)
     assert np.all(corrcoef_copy == corrcoef2)
 
     action = np.array([[1, 3], [4, 2]])
     env.step(action)
 
-    GEBV3 = env.GEBV
+    GEBV3 = env.unwrapped.GEBV
     corrcoef3 = env.corrcoef
     assert id(corrcoef) != id(corrcoef3)
     assert id(GEBV) != id(GEBV3)
 
 
 def test_reward_shaping():
     env = gym.make(
-        "BreedGym",
+        "breedgym:BreedGym",
         initial_population=genome,
         genetic_map=genetic_map,
         reward_shaping=False,
     )
 
     pop, _ = env.reset()
 
@@ -83,37 +83,37 @@
     action = np.asarray(env.action_space.sample()) % len(pop)
     _, reward, _, truncated, _ = env.step(action)
 
     assert reward != 0
     assert truncated
 
     env2 = gym.make(
-        "BreedGym",
+        "breedgym:BreedGym",
         initial_population=genome,
         genetic_map=genetic_map,
         reward_shaping=True,
     )
 
     pop, _ = env2.reset()
     action = np.asarray(env2.action_space.sample()) % len(pop)
     _, reward, _, _, _ = env2.step(action)
 
     assert reward != 0
 
 
 def test_deterministic():
     env = gym.make(
-        "BreedGym",
+        "breedgym:BreedGym",
         initial_population=genome,
         genetic_map=genetic_map,
         reward_shaping=False,
     )
 
     env.reset(seed=7)
     action = np.array(
         [[1, 2], [1, 5], [1, 7], [2, 5], [2, 9], [4, 7], [4, 8], [5, 9], [6, 8], [6, 9]]
     )
 
     for _ in range(10):
         _, r, _, _, _ = env.step(action)
 
-    assert abs(r - (1.6602371)) < 1e-6
+    assert abs(r - (1.8197979)) < 1e-6
```

### Comparing `breedgym-0.0.1a0/tests/test_vec.py` & `breedgym-0.0.2a0/tests/test_vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     np.random.seed(seed=7)
     pop, _ = env.reset(seed=7)
     for _ in range(20):
         action = np.random.randint(len(pop), size=(num_envs, individual_per_gen, 2))
         pop, rews, _, _, _ = env.step(action)
 
-    expected_result = np.array([11.618341, 11.29245, 13.47926, 10.03809])
+    expected_result = np.array([10.844662, 8.436224, 8.759013, 9.1480465])
     assert np.allclose(rews, expected_result)
 
 
 def test_vec_gebv_policy():
     num_envs = 4
     individual_per_gen = 200
     env = gym.make(
@@ -146,15 +146,15 @@
         trait_names=["Yield"],
     )
 
     _, infos = env.reset(seed=7)
     for _ in range(10):
         _, rews, _, _, infos = env.step(infos["GEBV"].squeeze())
 
-    expected_result = np.array([20.43854, 21.59488, 20.503202, 21.617622])
+    expected_result = np.array([18.514063, 19.428415, 19.090204, 19.841211])
     assert np.allclose(rews, expected_result)
 
 
 def test_vec_wrapper_n_crosses():
     num_envs = 4
     individual_per_gen = 200
     env = VecBreedGym(
@@ -196,9 +196,9 @@
 
     _, infos = env.reset(seed=7)
     for _ in range(10):
         gebvs = infos["GEBV"].squeeze()
         gebvs_matrix_sum = np.add.outer(gebvs, gebvs)
         _, rews, _, _, infos = env.step(gebvs_matrix_sum)
 
-    expected_result = np.array([13.162314, 10.155096, 12.45827, 12.093216])
+    expected_result = np.array([8.650201, 9.414795, 8.115064, 10.0190525])
     assert np.allclose(rews, expected_result)
```

### Comparing `breedgym-0.0.1a0/tests/test_wrappers.py` & `breedgym-0.0.2a0/tests/test_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 from chromax.sample_data import genetic_map, genome
 
 
 def test_simplified_env():
     individual_per_gen = 200
     env = gym.make(
-        "SimplifiedBreedGym",
+        "breedgym:SimplifiedBreedGym",
         individual_per_gen=individual_per_gen,
         initial_population=genome,
         genetic_map=genetic_map,
     )
 
     obs, _ = env.reset()
     assert len(obs["GEBV"]) == individual_per_gen
@@ -42,15 +42,15 @@
     with pytest.raises(Exception):
         env.step({"n_bests": 500, "n_crosses": 10})
 
 
 def test_kbest_env():
     individual_per_gen = 200
     env = gym.make(
-        "KBestBreedGym",
+        "breedgym:KBestBreedGym",
         individual_per_gen=individual_per_gen,
         initial_population=genome,
         genetic_map=genetic_map,
     )
     obs, _ = env.reset()
     assert len(obs["GEBV"]) == individual_per_gen
     assert len(obs["corrcoef"]) == individual_per_gen
@@ -69,20 +69,20 @@
     with pytest.raises(Exception):
         env.step(21)
 
 
 def test_gebv_policy():
     individual_per_gen = 200
     env = gym.make(
-        "KBestBreedGym",
+        "breedgym:KBestBreedGym",
         individual_per_gen=individual_per_gen,
         initial_population=genome,
         genetic_map=genetic_map,
         trait_names=["Yield"],
     )
     env.reset(seed=7)
     action = 10
 
     for _ in range(10):
         _, r, _, _, _ = env.step(action)
 
-    assert abs(r - 20.315035) < 1e-5
+    assert abs(r - 18.826467) < 1e-5
```

