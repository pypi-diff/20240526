# Comparing `tmp/mentabotix-0.1.5.2.tar.gz` & `tmp/mentabotix-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.2.tar", last modified: Fri May 24 13:02:01 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.3.tar", last modified: Sun May 26 04:18:11 2024, max compression
```

## Comparing `mentabotix-0.1.5.2.tar` & `mentabotix-0.1.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-24 13:01:36.791462 mentabotix-0.1.5.2/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-24 13:01:36.791462 mentabotix-0.1.5.2/README.md
--rw-r--r--   0        0        0      613 2024-05-24 13:02:01.955751 mentabotix-0.1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1198 2024-05-24 13:01:36.791462 mentabotix-0.1.5.2/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    73476 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20809 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0        0 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/test_botix.py
--rw-r--r--   0        0        0     2525 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/test_case_registry.py
--rw-r--r--   0        0        0    11417 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/test_menta.py
--rw-r--r--   0        0        0     9251 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/test_moving_state.py
--rw-r--r--   0        0        0     6505 2024-05-24 13:01:36.795462 mentabotix-0.1.5.2/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-26 04:17:47.880594 mentabotix-0.1.5.3/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-26 04:17:47.880594 mentabotix-0.1.5.3/README.md
+-rw-r--r--   0        0        0      613 2024-05-26 04:18:11.900529 mentabotix-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1198 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    73553 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    20809 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0        0 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_botix.py
+-rw-r--r--   0        0        0     2525 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_case_registry.py
+-rw-r--r--   0        0        0    11417 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_menta.py
+-rw-r--r--   0        0        0     9251 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.3/PKG-INFO
```

### Comparing `mentabotix-0.1.5.2/LICENSE` & `mentabotix-0.1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/README.md` & `mentabotix-0.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/pyproject.toml` & `mentabotix-0.1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.2"
+version = "0.1.5.3"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5.2/src/mentabotix/__init__.py` & `mentabotix-0.1.5.3/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.3/src/mentabotix/modules/botix.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,39 +455,42 @@
                 direction = -1
             case "r":
                 direction = 1
             case _:
                 raise ValueError("Invalid Direction. Must be one of ['l','r']")
         if weights:
 
+            total_weight = sum(weights)
+            norm_weights = tuple(weight / total_weight for weight in weights)
+            pack = list(zip(turn_speeds, norm_weights))
+
             def _spd() -> int:
                 # 计算权重总和并检查是否有负权重
-                total_weight = sum(weights)
 
                 # 生成一个随机数用于选择
                 rand_num = uniform(0, 1)
                 cum_weight = 0.0
 
                 # 遍历归一化后的权重，累加权重直到超过随机数，从而确定选择的索引
-                for i, weight in enumerate(weight / total_weight for weight in weights):
+                for index, weight in pack:
                     cum_weight += weight
-                    if rand_num <= cum_weight:
-                        return turn_speeds[i]
+                    if rand_num < cum_weight:
+                        return index
 
         else:
             _spd = lambda: choice(turn_speeds)
 
         # Register a context updater to update the turn direction before entering this behavior.
 
         _updater = con.register_context_updater(_spd, output_keys=[used_ctx_varname], input_keys=[])
 
         # Set speed expressions and actions before entering, implementing random turning.
 
         return cls(
-            speed_expressions=(f"{direction}*{used_ctx_varname}", f"{direction*-1}*{used_ctx_varname}"),
+            speed_expressions=(f"{direction}*{used_ctx_varname}", f"{direction * -1}*{used_ctx_varname}"),
             used_context_variables=[used_ctx_varname],
             before_entering=[_updater],
         )
 
     @classmethod
     def drift(cls, fixed_axis: Literal["fl", "rl", "rr", "fr"], speed: int) -> Self:
         """
```

### Comparing `mentabotix-0.1.5.2/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.3/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.3/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.3/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.3/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/find_tests.py` & `mentabotix-0.1.5.3/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/test_botix.py` & `mentabotix-0.1.5.3/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/test_case_registry.py` & `mentabotix-0.1.5.3/tests/test_case_registry.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/test_composer.py` & `mentabotix-0.1.5.3/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/test_menta.py` & `mentabotix-0.1.5.3/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/test_moving_state.py` & `mentabotix-0.1.5.3/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.2/tests/test_moving_transition.py` & `mentabotix-0.1.5.3/tests/test_moving_transition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import unittest
 from unittest.mock import patch
 
-from mentabotix.modules.botix import MovingTransition, MovingState
+from bdmc.modules.controller import CloseLoopController, MotorInfo
+
+from mentabotix.modules.botix import MovingTransition, MovingState, Botix
 
 
 # Define a mock MovingState class for testing purposes
 
 
 class TestMovingTransition(unittest.TestCase):
 
@@ -130,10 +132,43 @@
         )
 
     def test_hash(self):
         transition1 = MovingTransition(self.default_duration, None, None, None, None)
         transition2 = MovingTransition(self.default_duration, None, None, None, None)
         self.assertNotEqual(hash(transition1), hash(transition2))
 
+    def test_som(self):
+        state_a = MovingState(100, -100)
+
+        end_state = MovingState(0)
+
+        state_b = MovingState(5000)
+
+        state_c = MovingState(
+            speed_expressions=("var1", "var2"),
+            used_context_variables=["var1", "var2"],
+        )
+
+        import random
+
+        con = CloseLoopController(
+            [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
+        ).start_msg_sending()
+
+        def breaker() -> int:
+            return random.randint(0, 2)
+
+        trans = MovingTransition(
+            2.0,
+            to_states={0: end_state, 1: state_b, 2: state_c},
+            from_states=state_a,
+            breaker=breaker,
+        )
+        botix = Botix(con)
+        botix.token_pool.append(trans)
+        func = botix.compile(False)
+
+        print(f"is callable {callable(func)}")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.5.2/PKG-INFO` & `mentabotix-0.1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

