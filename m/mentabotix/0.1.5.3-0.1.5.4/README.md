# Comparing `tmp/mentabotix-0.1.5.3.tar.gz` & `tmp/mentabotix-0.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.3.tar", last modified: Sun May 26 04:18:11 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.4.tar", last modified: Sun May 26 15:19:34 2024, max compression
```

## Comparing `mentabotix-0.1.5.3.tar` & `mentabotix-0.1.5.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-05-26 04:17:47.880594 mentabotix-0.1.5.3/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-26 04:17:47.880594 mentabotix-0.1.5.3/README.md
--rw-r--r--   0        0        0      613 2024-05-26 04:18:11.900529 mentabotix-0.1.5.3/pyproject.toml
--rw-r--r--   0        0        0     1198 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    73553 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20809 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0        0 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_botix.py
--rw-r--r--   0        0        0     2525 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_case_registry.py
--rw-r--r--   0        0        0    11417 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_menta.py
--rw-r--r--   0        0        0     9251 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_moving_state.py
--rw-r--r--   0        0        0     7475 2024-05-26 04:17:47.884594 mentabotix-0.1.5.3/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/README.md
+-rw-r--r--   0        0        0      613 2024-05-26 15:19:34.993597 mentabotix-0.1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1198 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    76370 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    20809 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0      867 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/src/mentabotix/tools/selectors.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_botix.py
+-rw-r--r--   0        0        0     2525 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_case_registry.py
+-rw-r--r--   0        0        0    11417 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_menta.py
+-rw-r--r--   0        0        0     9975 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.4/PKG-INFO
```

### Comparing `mentabotix-0.1.5.3/LICENSE` & `mentabotix-0.1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/README.md` & `mentabotix-0.1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/pyproject.toml` & `mentabotix-0.1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.3"
+version = "0.1.5.4"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5.3/src/mentabotix/__init__.py` & `mentabotix-0.1.5.4/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.4/src/mentabotix/modules/botix.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 )
 
 import numpy as np
 from bdmc import CloseLoopController
 from numpy.random import random
 from terminaltables import SingleTable
 
+from mentabotix.tools.selectors import make_weighted_selector
 from .exceptions import StructuralError, TokenizeError
+from .logger import _logger
 from ..tools.generators import NameGenerator
 
 T_EXPR = TypeVar("T_EXPR", str, list)
-
 Expression: TypeAlias = str | int
 
 FullPattern: TypeAlias = Tuple[int]
 LRPattern: TypeAlias = Tuple[int, int]
 IndividualPattern: TypeAlias = Tuple[int, int, int, int]
 FullExpressionPattern: TypeAlias = str
 LRExpressionPattern: TypeAlias = Tuple[Expression, Expression]
@@ -412,16 +413,21 @@
             cls: Class method convention parameter, referring to the current class.
             con: CloseLoopController object, representing the instance to which the random turning control is applied.
             turn_speed: Turning speed, positive for turning right, negative for turning left.
             used_ctx_varname: Context variable name used to represent the turn direction, defaults to "direction".
             turn_left_prob: Probability of turning left, defaults to 0.5, meaning equal chance of turning left or right.
 
         Returns:
-            None
+            Self: A new instance of the class with a random turn direction and speed.
         """
+        if turn_speed < 0:
+            _logger.warn(
+                f"Turn speed must be positive, got {turn_speed}, "
+                f"if you 'd like to turn right, lower the value of turn_left_prob instead."
+            )
 
         def _dir() -> int:
             """
             Internal function to randomly decide the turn direction.
 
             Returns:
                 int: 1 for turning left, -1 for turning right.
@@ -443,54 +449,90 @@
         cls,
         con: CloseLoopController,
         direction: Literal["l", "r"],
         turn_speeds: Sequence[int],
         weights: Optional[Sequence[float | int]] = None,
         used_ctx_varname: str = "rand_speed",
     ) -> Self:
+        """
+        Generates a random turning behavior for a CloseLoopController.
+
+        Parameters:
+            cls: Class method convention parameter, referring to the current class.
+            con: The CloseLoopController object to apply the random turning behavior to.
+            direction: Turning direction, either "l" (left) or "r" (right).
+            turn_speeds: A sequence of turning speeds to randomly select from.
+            weights: An optional sequence of weights corresponding to turn_speeds for weighted selection.
+            used_ctx_varname: The variable name to use in the context to store the selected turning speed. Default is "rand_speed".
 
-        from random import uniform, choice
+        Returns:
+            Self: An instance of the class configured with the random turning behavior.
+        """
+        if any(num < 0 for num in turn_speeds):
+            _logger.warn(
+                f"All turn speeds should be positive, got {turn_speeds}. "
+                f"Since you should not using the turn left with negative speed to represent turn right."
+            )
+        from random import choice
 
         match direction:
             case "l":
-                direction = -1
-            case "r":
                 direction = 1
+            case "r":
+                direction = -1
             case _:
                 raise ValueError("Invalid Direction. Must be one of ['l','r']")
-        if weights:
-
-            total_weight = sum(weights)
-            norm_weights = tuple(weight / total_weight for weight in weights)
-            pack = list(zip(turn_speeds, norm_weights))
-
-            def _spd() -> int:
-                # 计算权重总和并检查是否有负权重
-
-                # 生成一个随机数用于选择
-                rand_num = uniform(0, 1)
-                cum_weight = 0.0
-
-                # 遍历归一化后的权重，累加权重直到超过随机数，从而确定选择的索引
-                for index, weight in pack:
-                    cum_weight += weight
-                    if rand_num < cum_weight:
-                        return index
-
-        else:
-            _spd = lambda: choice(turn_speeds)
+        _spd = make_weighted_selector(turn_speeds, weights) if weights else lambda: choice(turn_speeds)
 
         # Register a context updater to update the turn direction before entering this behavior.
 
         _updater = con.register_context_updater(_spd, output_keys=[used_ctx_varname], input_keys=[])
 
         # Set speed expressions and actions before entering, implementing random turning.
 
         return cls(
-            speed_expressions=(f"{direction}*{used_ctx_varname}", f"{direction * -1}*{used_ctx_varname}"),
+            speed_expressions=(f"{-direction}*{used_ctx_varname}", f"{direction}*{used_ctx_varname}"),
+            used_context_variables=[used_ctx_varname],
+            before_entering=[_updater],
+        )
+
+    @classmethod
+    def rand_dir_spd_turn(
+        cls,
+        con: CloseLoopController,
+        turn_speeds: Sequence[int],
+        weights: Optional[Sequence[float | int]] = None,
+        used_ctx_varname: str = "rand_dir_speed",
+    ) -> Self:
+        """
+        Generates an instance of CloseLoopController that randomly selects a turning speed before entering the behavior.
+        It updates the context variable with the chosen speed.
+
+        Args:
+            con (CloseLoopController): The controller instance to modify.
+            turn_speeds (Sequence[int]): A sequence of turning speeds. positive means turn left, negative means turn right
+            weights (Optional[Sequence[float | int]], optional): Weights for each turning speed. If provided, speeds will be selected probabilistically. Defaults to None.
+            used_ctx_varname (str, optional): The name of the context variable to store the selected speed. Defaults to "rand_dir_speed".
+
+        Returns:
+            Self: An instance of the CloseLoopController class with the configured random turning behavior.
+        """
+        # Warn if all turn speeds have the same sign, suggesting the use of rand_spd_turn instead.
+        if all(num > 0 for num in turn_speeds) or all(num < 0 for num in turn_speeds):
+            _logger.warn("All speeds have the same sign, consider using rand_spd_turn")
+
+        # Select a turning speed based on given weights or randomly.
+        _spd = make_weighted_selector(turn_speeds, weights) if weights else lambda: choice(turn_speeds)
+
+        # Register a context updater to update the turn direction before entering this behavior.
+        _updater = con.register_context_updater(_spd, output_keys=[used_ctx_varname], input_keys=[])
+
+        # Set speed expressions and actions before entering, implementing random turning.
+        return cls(
+            speed_expressions=(f"-{used_ctx_varname}", f"{used_ctx_varname}"),
             used_context_variables=[used_ctx_varname],
             before_entering=[_updater],
         )
 
     @classmethod
     def drift(cls, fixed_axis: Literal["fl", "rl", "rr", "fr"], speed: int) -> Self:
         """
```

### Comparing `mentabotix-0.1.5.3/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.4/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.4/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.4/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.4/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/tests/find_tests.py` & `mentabotix-0.1.5.4/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/tests/test_botix.py` & `mentabotix-0.1.5.4/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/tests/test_case_registry.py` & `mentabotix-0.1.5.4/tests/test_case_registry.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/tests/test_composer.py` & `mentabotix-0.1.5.4/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/tests/test_menta.py` & `mentabotix-0.1.5.4/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/tests/test_moving_state.py` & `mentabotix-0.1.5.4/tests/test_moving_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,10 +227,30 @@
         fun = b.compile()
         for _ in range(20):
             fun()
             sleep(0.2)
         con.stop_msg_sending()
         con.serial_client.close()
 
+    def test_rand_turn_spd_dir_with_weights(self):
+        from mentabotix import MovingTransition, Botix
+
+        con = CloseLoopController(
+            [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
+        ).start_msg_sending()
+        state = MovingState.rand_dir_spd_turn(con, [500, 600, -700], weights=[10, 80, 10])
+        print(state)
+        end = MovingState(0)
+        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+
+        b = Botix(controller=con, token_pool=[trans])
+
+        fun = b.compile()
+        for _ in range(20):
+            fun()
+            sleep(0.2)
+        con.stop_msg_sending()
+        con.serial_client.close()
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.5.3/tests/test_moving_transition.py` & `mentabotix-0.1.5.4/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.3/PKG-INFO` & `mentabotix-0.1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.3
+Version: 0.1.5.4
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

