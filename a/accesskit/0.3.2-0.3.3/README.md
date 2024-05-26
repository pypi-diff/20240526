# Comparing `tmp/accesskit-0.3.2.tar.gz` & `tmp/accesskit-0.3.3.tar.gz`

## Comparing `accesskit-0.3.2.tar` & `accesskit-0.3.3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
--rw-r--r--   0     1001      127     1294 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/Cargo.toml
--rw-r--r--   0     1001      127    11644 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/CHANGELOG.md
--rw-r--r--   0     1001      127      487 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/README.md
--rw-r--r--   0     1001      127     6935 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/adapter.rs
--rw-r--r--   0     1001      127    13572 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/bus.rs
--rw-r--r--   0     1001      127     6053 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/accessible.rs
--rw-r--r--   0     1001      127     1473 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/action.rs
--rw-r--r--   0     1001      127     1096 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/application.rs
--rw-r--r--   0     1001      127     2195 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/component.rs
--rw-r--r--   0     1001      127      945 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/mod.rs
--rw-r--r--   0     1001      127     1459 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/interfaces/value.rs
--rw-r--r--   0     1001      127      404 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/mod.rs
--rw-r--r--   0     1001      127     1224 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/object_address.rs
--rw-r--r--   0     1001      127     2185 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/atspi/object_id.rs
--rw-r--r--   0     1001      127     8048 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/context.rs
--rw-r--r--   0     1001      127     4885 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/executor.rs
--rw-r--r--   0     1001      127     1005 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/lib.rs
--rw-r--r--   0     1001      127     1389 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/unix/src/util.rs
--rw-r--r--   0     1001      127      942 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/Cargo.toml
--rw-r--r--   0     1001      127    16025 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/CHANGELOG.md
--rw-r--r--   0     1001      127      183 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/README.md
--rw-r--r--   0     1001      127     9554 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/adapter.rs
--rw-r--r--   0     1001      127     2731 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/context.rs
--rw-r--r--   0     1001      127     8399 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/event.rs
--rw-r--r--   0     1001      127      282 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/filters.rs
--rw-r--r--   0     1001      127      557 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/lib.rs
--rw-r--r--   0     1001      127    32713 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/node.rs
--rw-r--r--   0     1001      127     3146 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/patch.rs
--rw-r--r--   0     1001      127     9523 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/subclass.rs
--rw-r--r--   0     1001      127     2819 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/macos/src/util.rs
--rw-r--r--   0     1001      127      705 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/Cargo.toml
--rw-r--r--   0     1001      127    15163 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/CHANGELOG.md
--rw-r--r--   0     1001      127      740 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/README.md
--rw-r--r--   0     1001      127    22792 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/src/geometry.rs
--rw-r--r--   0     1001      127    78839 2024-05-13 21:02:49.000000 accesskit-0.3.2/common/src/lib.rs
--rw-r--r--   0     1001      127      956 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/Cargo.toml
--rw-r--r--   0     1001      127    26348 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/CHANGELOG.md
--rw-r--r--   0     1001      127      172 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/README.md
--rw-r--r--   0     1001      127    11651 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/examples/hello_world.rs
--rw-r--r--   0     1001      127    15277 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/adapter.rs
--rw-r--r--   0     1001      127     1850 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/context.rs
--rw-r--r--   0     1001      127      356 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/filters.rs
--rw-r--r--   0     1001      127      482 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/lib.rs
--rw-r--r--   0     1001      127    36973 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/node.rs
--rw-r--r--   0     1001      127     6179 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/subclass.rs
--rw-r--r--   0     1001      127    11438 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/tests/mod.rs
--rw-r--r--   0     1001      127     6937 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/tests/simple.rs
--rw-r--r--   0     1001      127     3536 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/tests/subclassed.rs
--rw-r--r--   0     1001      127    19711 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/text.rs
--rw-r--r--   0     1001      127     6500 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/windows/src/util.rs
--rw-r--r--   0     1001      127      435 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/Cargo.toml
--rw-r--r--   0     1001      127    18903 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/CHANGELOG.md
--rw-r--r--   0     1001      127      207 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/README.md
--rw-r--r--   0     1001      127      958 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/filters.rs
--rw-r--r--   0     1001      127    25410 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/iterators.rs
--rw-r--r--   0     1001      127     6057 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/lib.rs
--rw-r--r--   0     1001      127    31830 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/node.rs
--rw-r--r--   0     1001      127    64423 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/text.rs
--rw-r--r--   0     1001      127    25493 2024-05-13 21:02:49.000000 accesskit-0.3.2/consumer/src/tree.rs
--rw-r--r--   0     1001      127      670 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/Cargo.toml
--rw-r--r--   0     1001      127     4126 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/CHANGELOG.md
--rw-r--r--   0     1001      127      317 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/README.md
--rw-r--r--   0     1001      127      432 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/action.rs
--rw-r--r--   0     1001      127    12926 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/adapter.rs
--rw-r--r--   0     1001      127      583 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/callback.rs
--rw-r--r--   0     1001      127     3414 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/context.rs
--rw-r--r--   0     1001      127      541 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/error.rs
--rw-r--r--   0     1001      127     1036 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/events.rs
--rw-r--r--   0     1001      127      282 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/filters.rs
--rw-r--r--   0     1001      127      753 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/lib.rs
--rw-r--r--   0     1001      127    37868 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/node.rs
--rw-r--r--   0     1001      127      898 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/rect.rs
--rw-r--r--   0     1001      127    13107 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/simplified.rs
--rw-r--r--   0     1001      127     1157 2024-05-13 21:02:49.000000 accesskit-0.3.2/platforms/atspi-common/src/util.rs
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 accesskit-0.3.2/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      224 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/.cargo/config.toml
--rw-r--r--   0     1001      127     5568 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127      981 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/README.md
--rw-r--r--   0     1001      127     3078 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/.gitignore
--rw-r--r--   0     1001      127      367 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/README.md
--rw-r--r--   0     1001      127     6979 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/hello_world.py
--rw-r--r--   0     1001      127       24 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/examples/pygame/requirements.txt
--rw-r--r--   0     1001      127    24191 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/common.rs
--rw-r--r--   0     1001      127     4784 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/geometry.rs
--rw-r--r--   0     1001      127     2818 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     7316 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/macos.rs
--rw-r--r--   0     1001      127     1506 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/unix.rs
--rw-r--r--   0     1001      127     4126 2024-05-13 21:02:49.000000 accesskit-0.3.2/bindings/python/src/windows.rs
--rw-r--r--   0     1001      127    75008 2024-05-13 21:02:49.000000 accesskit-0.3.2/Cargo.lock
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.2/Cargo.toml
--rw-r--r--   0     1001      127     1043 2024-05-13 21:02:49.000000 accesskit-0.3.2/pyproject.toml
--rw-r--r--   0     1001      127     9723 2024-05-13 21:02:49.000000 accesskit-0.3.2/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-05-13 21:02:49.000000 accesskit-0.3.2/LICENSE-MIT
--rw-r--r--   0     1001      127     1559 2024-05-13 21:02:49.000000 accesskit-0.3.2/LICENSE.chromium
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.2/PKG-INFO
+-rw-r--r--   0     1001      127      942 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/Cargo.toml
+-rw-r--r--   0     1001      127    16504 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/CHANGELOG.md
+-rw-r--r--   0     1001      127      183 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/README.md
+-rw-r--r--   0     1001      127     9554 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/adapter.rs
+-rw-r--r--   0     1001      127     2731 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/context.rs
+-rw-r--r--   0     1001      127     8399 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/event.rs
+-rw-r--r--   0     1001      127      282 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/filters.rs
+-rw-r--r--   0     1001      127      557 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/lib.rs
+-rw-r--r--   0     1001      127    33207 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/node.rs
+-rw-r--r--   0     1001      127     3146 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/patch.rs
+-rw-r--r--   0     1001      127     9523 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/subclass.rs
+-rw-r--r--   0     1001      127     2819 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/macos/src/util.rs
+-rw-r--r--   0     1001      127      705 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/Cargo.toml
+-rw-r--r--   0     1001      127    15163 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/CHANGELOG.md
+-rw-r--r--   0     1001      127      740 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/README.md
+-rw-r--r--   0     1001      127    22792 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/src/geometry.rs
+-rw-r--r--   0     1001      127    78839 2024-05-26 10:52:10.000000 accesskit-0.3.3/common/src/lib.rs
+-rw-r--r--   0     1001      127      435 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/Cargo.toml
+-rw-r--r--   0     1001      127    20361 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/CHANGELOG.md
+-rw-r--r--   0     1001      127      207 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/README.md
+-rw-r--r--   0     1001      127      958 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/filters.rs
+-rw-r--r--   0     1001      127    25548 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/iterators.rs
+-rw-r--r--   0     1001      127     7678 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/lib.rs
+-rw-r--r--   0     1001      127    31990 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/node.rs
+-rw-r--r--   0     1001      127    71808 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/text.rs
+-rw-r--r--   0     1001      127    27118 2024-05-26 10:52:10.000000 accesskit-0.3.3/consumer/src/tree.rs
+-rw-r--r--   0     1001      127      956 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/Cargo.toml
+-rw-r--r--   0     1001      127    26831 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/CHANGELOG.md
+-rw-r--r--   0     1001      127      172 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/README.md
+-rw-r--r--   0     1001      127    11651 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/examples/hello_world.rs
+-rw-r--r--   0     1001      127    15277 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/adapter.rs
+-rw-r--r--   0     1001      127     1850 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/context.rs
+-rw-r--r--   0     1001      127      356 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/filters.rs
+-rw-r--r--   0     1001      127      482 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/lib.rs
+-rw-r--r--   0     1001      127    37084 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/node.rs
+-rw-r--r--   0     1001      127     6179 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/subclass.rs
+-rw-r--r--   0     1001      127    11438 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/tests/mod.rs
+-rw-r--r--   0     1001      127     6937 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/tests/simple.rs
+-rw-r--r--   0     1001      127     3536 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/tests/subclassed.rs
+-rw-r--r--   0     1001      127    19711 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/text.rs
+-rw-r--r--   0     1001      127     6500 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/windows/src/util.rs
+-rw-r--r--   0     1001      127     1295 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/Cargo.toml
+-rw-r--r--   0     1001      127    12315 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/CHANGELOG.md
+-rw-r--r--   0     1001      127      487 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/README.md
+-rw-r--r--   0     1001      127     6935 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/adapter.rs
+-rw-r--r--   0     1001      127    16200 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/bus.rs
+-rw-r--r--   0     1001      127     6218 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/accessible.rs
+-rw-r--r--   0     1001      127     1473 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/action.rs
+-rw-r--r--   0     1001      127     1096 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/application.rs
+-rw-r--r--   0     1001      127     2195 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/component.rs
+-rw-r--r--   0     1001      127      979 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/mod.rs
+-rw-r--r--   0     1001      127     4767 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/text.rs
+-rw-r--r--   0     1001      127     1459 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/interfaces/value.rs
+-rw-r--r--   0     1001      127      404 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/mod.rs
+-rw-r--r--   0     1001      127     1224 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/object_address.rs
+-rw-r--r--   0     1001      127     2185 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/atspi/object_id.rs
+-rw-r--r--   0     1001      127     8048 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/context.rs
+-rw-r--r--   0     1001      127     4885 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/executor.rs
+-rw-r--r--   0     1001      127     1005 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/lib.rs
+-rw-r--r--   0     1001      127     1616 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/unix/src/util.rs
+-rw-r--r--   0     1001      127      670 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/Cargo.toml
+-rw-r--r--   0     1001      127     5243 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/CHANGELOG.md
+-rw-r--r--   0     1001      127      317 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/README.md
+-rw-r--r--   0     1001      127      432 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/action.rs
+-rw-r--r--   0     1001      127    18429 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/adapter.rs
+-rw-r--r--   0     1001      127      583 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/callback.rs
+-rw-r--r--   0     1001      127     3414 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/context.rs
+-rw-r--r--   0     1001      127      677 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/error.rs
+-rw-r--r--   0     1001      127     1278 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/events.rs
+-rw-r--r--   0     1001      127      282 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/filters.rs
+-rw-r--r--   0     1001      127      785 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/lib.rs
+-rw-r--r--   0     1001      127    47783 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/node.rs
+-rw-r--r--   0     1001      127      898 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/rect.rs
+-rw-r--r--   0     1001      127    20319 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/simplified.rs
+-rw-r--r--   0     1001      127     4041 2024-05-26 10:52:10.000000 accesskit-0.3.3/platforms/atspi-common/src/util.rs
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 accesskit-0.3.3/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/.cargo/config.toml
+-rw-r--r--   0     1001      127     5791 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127      981 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/README.md
+-rw-r--r--   0     1001      127     3078 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/.gitignore
+-rw-r--r--   0     1001      127      367 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/README.md
+-rw-r--r--   0     1001      127     6979 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/hello_world.py
+-rw-r--r--   0     1001      127       24 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/examples/pygame/requirements.txt
+-rw-r--r--   0     1001      127    24191 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/common.rs
+-rw-r--r--   0     1001      127     4784 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/geometry.rs
+-rw-r--r--   0     1001      127     2818 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     7316 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/macos.rs
+-rw-r--r--   0     1001      127     1506 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/unix.rs
+-rw-r--r--   0     1001      127     4126 2024-05-26 10:52:10.000000 accesskit-0.3.3/bindings/python/src/windows.rs
+-rw-r--r--   0     1001      127    73418 2024-05-26 10:52:10.000000 accesskit-0.3.3/Cargo.lock
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.3/Cargo.toml
+-rw-r--r--   0     1001      127     1043 2024-05-26 10:52:10.000000 accesskit-0.3.3/pyproject.toml
+-rw-r--r--   0     1001      127     9723 2024-05-26 10:52:10.000000 accesskit-0.3.3/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-05-26 10:52:10.000000 accesskit-0.3.3/LICENSE-MIT
+-rw-r--r--   0     1001      127     1559 2024-05-26 10:52:10.000000 accesskit-0.3.3/LICENSE.chromium
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.3/PKG-INFO
```

### Comparing `accesskit-0.3.2/platforms/unix/Cargo.toml` & `accesskit-0.3.3/platforms/unix/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_unix"
-version = "0.9.2"
+version = "0.10.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Linux adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -14,15 +14,15 @@
 [features]
 default = ["async-io"]
 async-io = ["dep:async-channel", "dep:async-executor", "dep:async-task", "dep:futures-util", "atspi/async-std", "zbus/async-io"]
 tokio = ["dep:tokio", "dep:tokio-stream", "atspi/tokio", "zbus/tokio"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_atspi_common = { version = "0.4.2", path = "../atspi-common" }
+accesskit_atspi_common = { version = "0.5.0", path = "../atspi-common" }
 atspi = { version = "0.19", default-features = false }
 futures-lite = "1.13"
 serde = "1.0"
 zbus = { version = "3.14", default-features = false }
 
 # async-io support
 async-channel = { version = "2.1.1", optional = true }
```

### Comparing `accesskit-0.3.2/platforms/unix/CHANGELOG.md` & `accesskit-0.3.3/platforms/unix/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,29 @@
   * dependencies
     * accesskit_atspi_common bumped from 0.4.0 to 0.4.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_atspi_common bumped from 0.4.1 to 0.4.2
 
+## [0.10.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.9.2...accesskit_unix-v0.10.0) (2024-05-26)
+
+
+### Features
+
+* Add basic text support on Unix ([#362](https://github.com/AccessKit/accesskit/issues/362)) ([52540f8](https://github.com/AccessKit/accesskit/commit/52540f82cf9fc148358351ed486bab3e7e91f1d6))
+* Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_atspi_common bumped from 0.4.2 to 0.5.0
+
 ## [0.9.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.8.0...accesskit_unix-v0.9.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Force a semver-breaking release ([#398](https://github.com/AccessKit/accesskit/issues/398))
```

### Comparing `accesskit-0.3.2/platforms/unix/src/adapter.rs` & `accesskit-0.3.3/platforms/unix/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/bus.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/bus.rs`

 * *Files 22% similar despite different names*

```diff
@@ -120,14 +120,18 @@
         if new_interfaces.contains(Interface::Component) {
             self.register_interface(
                 &path,
                 ComponentInterface::new(bus_name.clone(), node.clone()),
             )
             .await?;
         }
+        if new_interfaces.contains(Interface::Text) {
+            self.register_interface(&path, TextInterface::new(node.clone()))
+                .await?;
+        }
         if new_interfaces.contains(Interface::Value) {
             self.register_interface(&path, ValueInterface::new(node.clone()))
                 .await?;
         }
 
         Ok(())
     }
@@ -161,14 +165,17 @@
         if old_interfaces.contains(Interface::Action) {
             self.unregister_interface::<ActionInterface>(&path).await?;
         }
         if old_interfaces.contains(Interface::Component) {
             self.unregister_interface::<ComponentInterface>(&path)
                 .await?;
         }
+        if old_interfaces.contains(Interface::Text) {
+            self.unregister_interface::<TextInterface>(&path).await?;
+        }
         if old_interfaces.contains(Interface::Value) {
             self.unregister_interface::<ValueInterface>(&path).await?;
         }
 
         Ok(())
     }
 
@@ -197,17 +204,20 @@
             NodeIdOrRoot::Root => ObjectId::Root,
         };
         let interface = "org.a11y.atspi.Event.Object";
         let signal = match event {
             ObjectEvent::ActiveDescendantChanged(_) => "ActiveDescendantChanged",
             ObjectEvent::Announcement(_, _) => "Announcement",
             ObjectEvent::BoundsChanged(_) => "BoundsChanged",
+            ObjectEvent::CaretMoved(_) => "TextCaretMoved",
             ObjectEvent::ChildAdded(_, _) | ObjectEvent::ChildRemoved(_) => "ChildrenChanged",
             ObjectEvent::PropertyChanged(_) => "PropertyChange",
             ObjectEvent::StateChanged(_, _) => "StateChanged",
+            ObjectEvent::TextInserted { .. } | ObjectEvent::TextRemoved { .. } => "TextChanged",
+            ObjectEvent::TextSelectionChanged => "TextSelectionChanged",
         };
         let properties = HashMap::new();
         match event {
             ObjectEvent::ActiveDescendantChanged(child) => {
                 let child = ObjectId::Node {
                     adapter: adapter_id,
                     node: child,
@@ -252,14 +262,29 @@
                         detail2: 0,
                         any_data: Value::from(bounds),
                         properties,
                     },
                 )
                 .await
             }
+            ObjectEvent::CaretMoved(offset) => {
+                self.emit_event(
+                    target,
+                    interface,
+                    signal,
+                    EventBody {
+                        kind: "",
+                        detail1: offset,
+                        detail2: 0,
+                        any_data: "".into(),
+                        properties,
+                    },
+                )
+                .await
+            }
             ObjectEvent::ChildAdded(index, child) => {
                 let child = ObjectId::Node {
                     adapter: adapter_id,
                     node: child,
                 };
                 self.emit_event(
                     target,
@@ -341,14 +366,67 @@
                         detail2: 0,
                         any_data: 0i32.into(),
                         properties,
                     },
                 )
                 .await
             }
+            ObjectEvent::TextInserted {
+                start_index,
+                length,
+                content,
+            } => {
+                self.emit_event(
+                    target,
+                    interface,
+                    signal,
+                    EventBody {
+                        kind: "insert",
+                        detail1: start_index,
+                        detail2: length,
+                        any_data: content.into(),
+                        properties,
+                    },
+                )
+                .await
+            }
+            ObjectEvent::TextRemoved {
+                start_index,
+                length,
+                content,
+            } => {
+                self.emit_event(
+                    target,
+                    interface,
+                    signal,
+                    EventBody {
+                        kind: "delete",
+                        detail1: start_index,
+                        detail2: length,
+                        any_data: content.into(),
+                        properties,
+                    },
+                )
+                .await
+            }
+            ObjectEvent::TextSelectionChanged => {
+                self.emit_event(
+                    target,
+                    interface,
+                    signal,
+                    EventBody {
+                        kind: "",
+                        detail1: 0,
+                        detail2: 0,
+                        any_data: "".into(),
+                        properties,
+                    },
+                )
+                .await
+            }
         }
     }
 
     pub(crate) async fn emit_window_event(
         &self,
         adapter_id: usize,
         target: NodeId,
```

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/accessible.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/accessible.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
+use std::collections::HashMap;
+
 use accesskit_atspi_common::{NodeIdOrRoot, PlatformNode, PlatformRoot};
 use atspi::{Interface, InterfaceSet, Role, StateSet};
 use zbus::{fdo, names::OwnedUniqueName};
 
 use super::map_root_error;
 use crate::atspi::{ObjectId, OwnedObjectAddress};
 
@@ -105,14 +107,18 @@
         self.node.localized_role_name().map_err(self.map_error())
     }
 
     fn get_state(&self) -> StateSet {
         self.node.state()
     }
 
+    fn get_attributes(&self) -> fdo::Result<HashMap<&str, String>> {
+        self.node.attributes().map_err(self.map_error())
+    }
+
     fn get_application(&self) -> (OwnedObjectAddress,) {
         (ObjectId::Root.to_address(self.bus_name.clone()),)
     }
 
     fn get_interfaces(&self) -> fdo::Result<InterfaceSet> {
         self.node.interfaces().map_err(self.map_error())
     }
```

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/action.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/action.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/application.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/application.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/component.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/component.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/mod.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 mod accessible;
 mod action;
 mod application;
 mod component;
+mod text;
 mod value;
 
 use crate::atspi::{ObjectId, OwnedObjectAddress};
 use zbus::{fdo, names::OwnedUniqueName};
 
 fn map_root_error(error: accesskit_atspi_common::Error) -> fdo::Error {
     crate::util::map_error(ObjectId::Root, error)
@@ -27,8 +28,9 @@
     }
 }
 
 pub(crate) use accessible::*;
 pub(crate) use action::*;
 pub(crate) use application::*;
 pub(crate) use component::*;
+pub(crate) use text::*;
 pub(crate) use value::*;
```

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/interfaces/value.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/interfaces/value.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/object_address.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/object_address.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/atspi/object_id.rs` & `accesskit-0.3.3/platforms/unix/src/atspi/object_id.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/context.rs` & `accesskit-0.3.3/platforms/unix/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/executor.rs` & `accesskit-0.3.3/platforms/unix/src/executor.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/lib.rs` & `accesskit-0.3.3/platforms/unix/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/unix/src/util.rs` & `accesskit-0.3.3/platforms/unix/src/util.rs`

 * *Files 15% similar despite different names*

```diff
@@ -26,13 +26,17 @@
 pub(crate) fn map_error(source: ObjectId, error: InternalError) -> FdoError {
     match error {
         InternalError::Defunct | InternalError::UnsupportedInterface => {
             FdoError::UnknownObject(source.path().to_string())
         }
         InternalError::TooManyChildren => FdoError::Failed("Too many children.".into()),
         InternalError::IndexOutOfRange => FdoError::Failed("Index is too big.".into()),
+        InternalError::TooManyCharacters => FdoError::Failed("Too many characters.".into()),
+        InternalError::UnsupportedTextGranularity => {
+            FdoError::Failed("Unsupported text granularity.".into())
+        }
     }
 }
 
 pub(crate) fn map_error_from_node(source: &PlatformNode, error: InternalError) -> FdoError {
     map_error(ObjectId::from(source), error)
 }
```

### Comparing `accesskit-0.3.2/platforms/macos/Cargo.toml` & `accesskit-0.3.3/platforms/macos/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_macos"
-version = "0.13.2"
+version = "0.14.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: macOS adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -12,15 +12,15 @@
 rust-version.workspace = true
 
 [package.metadata.docs.rs]
 default-target = "x86_64-apple-darwin"
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.20.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.21.0", path = "../../consumer" }
 once_cell = "1.13.0"
 objc2 = "0.5.1"
 objc2-foundation = { version = "0.2.0", features = [
     "NSArray",
     "NSDictionary",
     "NSValue",
     "NSThread",
```

### Comparing `accesskit-0.3.2/platforms/macos/CHANGELOG.md` & `accesskit-0.3.3/platforms/macos/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,28 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_consumer bumped from 0.19.0 to 0.19.1
 
+## [0.14.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.13.2...accesskit_macos-v0.14.0) (2024-05-26)
+
+
+### Features
+
+* Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.20.0 to 0.21.0
+
 ## [0.13.2](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.13.1...accesskit_macos-v0.13.2) (2024-05-13)
 
 
 ### Bug Fixes
 
 * Fix platform adapters to support copy-on-write tree snapshots again ([#411](https://github.com/AccessKit/accesskit/issues/411)) ([d3a130a](https://github.com/AccessKit/accesskit/commit/d3a130a5ec8ae1d9edf0bf85a44f35f0e365242c))
```

### Comparing `accesskit-0.3.2/platforms/macos/src/adapter.rs` & `accesskit-0.3.3/platforms/macos/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/macos/src/context.rs` & `accesskit-0.3.3/platforms/macos/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/macos/src/event.rs` & `accesskit-0.3.3/platforms/macos/src/event.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/macos/src/lib.rs` & `accesskit-0.3.3/platforms/macos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/macos/src/node.rs` & `accesskit-0.3.3/platforms/macos/src/node.rs`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,18 @@
         self.name()
     }
 
     pub(crate) fn description(&self) -> Option<String> {
         self.0.description()
     }
 
+    pub(crate) fn placeholder(&self) -> Option<String> {
+        self.0.placeholder()
+    }
+
     pub(crate) fn value(&self) -> Option<Value> {
         let state = self.0;
         if let Some(toggled) = state.toggled() {
             return Some(Value::Bool(toggled != Toggled::False));
         }
         if let Some(value) = self.node_value() {
             return Some(Value::String(value));
@@ -409,14 +413,23 @@
             self.resolve(|node| {
                 let wrapper = NodeWrapper(node);
                 wrapper.description().map(|description| NSString::from_str(&description))
             })
             .flatten()
         }
 
+        #[method_id(accessibilityPlaceholderValue)]
+        fn placeholder(&self) -> Option<Id<NSString>> {
+            self.resolve(|node| {
+                let wrapper = NodeWrapper(node);
+                wrapper.placeholder().map(|placeholder| NSString::from_str(&placeholder))
+            })
+            .flatten()
+        }
+
         #[method_id(accessibilityValue)]
         fn value(&self) -> Option<Id<NSObject>> {
             self.resolve(|node| {
                 let wrapper = NodeWrapper(node);
                 wrapper.value().map(|value| match value {
                     Value::Bool(value) => {
                         Id::into_super(Id::into_super(NSNumber::new_bool(value)))
@@ -748,14 +761,15 @@
                     || selector == sel!(accessibilityChildren)
                     || selector == sel!(accessibilityChildrenInNavigationOrder)
                     || selector == sel!(accessibilityFrame)
                     || selector == sel!(accessibilityRole)
                     || selector == sel!(accessibilityRoleDescription)
                     || selector == sel!(accessibilityTitle)
                     || selector == sel!(accessibilityHelp)
+                    || selector == sel!(accessibilityPlaceholderValue)
                     || selector == sel!(accessibilityValue)
                     || selector == sel!(accessibilityMinValue)
                     || selector == sel!(accessibilityMaxValue)
                     || selector == sel!(isAccessibilityElement)
                     || selector == sel!(isAccessibilityFocused)
                     || selector == sel!(accessibilityNotifiesWhenDestroyed)
                     || selector == sel!(isAccessibilitySelectorAllowed:)
```

### Comparing `accesskit-0.3.2/platforms/macos/src/patch.rs` & `accesskit-0.3.3/platforms/macos/src/patch.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/macos/src/subclass.rs` & `accesskit-0.3.3/platforms/macos/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/macos/src/util.rs` & `accesskit-0.3.3/platforms/macos/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/common/Cargo.toml` & `accesskit-0.3.3/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/common/CHANGELOG.md` & `accesskit-0.3.3/common/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/common/README.md` & `accesskit-0.3.3/common/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/common/src/geometry.rs` & `accesskit-0.3.3/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/common/src/lib.rs` & `accesskit-0.3.3/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/Cargo.toml` & `accesskit-0.3.3/platforms/windows/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "accesskit_windows"
-version = "0.18.2"
+version = "0.19.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Windows adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.20.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.21.0", path = "../../consumer" }
 paste = "1.0"
 static_assertions = "1.1.0"
 
 [dependencies.windows]
 version = "0.54"
 features = [
     "implement",
```

### Comparing `accesskit-0.3.2/platforms/windows/CHANGELOG.md` & `accesskit-0.3.3/platforms/windows/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,28 @@
     * accesskit_consumer bumped from 0.15.1 to 0.15.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.19.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.18.2...accesskit_windows-v0.19.0) (2024-05-26)
+
+
+### Features
+
+* Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.20.0 to 0.21.0
+
 ## [0.18.2](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.18.1...accesskit_windows-v0.18.2) (2024-05-13)
 
 
 ### Bug Fixes
 
 * Fix platform adapters to support copy-on-write tree snapshots again ([#411](https://github.com/AccessKit/accesskit/issues/411)) ([d3a130a](https://github.com/AccessKit/accesskit/commit/d3a130a5ec8ae1d9edf0bf85a44f35f0e365242c))
```

### Comparing `accesskit-0.3.2/platforms/windows/examples/hello_world.rs` & `accesskit-0.3.3/platforms/windows/examples/hello_world.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/adapter.rs` & `accesskit-0.3.3/platforms/windows/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/context.rs` & `accesskit-0.3.3/platforms/windows/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/node.rs` & `accesskit-0.3.3/platforms/windows/src/node.rs`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,18 @@
         self.0.name()
     }
 
     fn description(&self) -> Option<String> {
         self.0.description()
     }
 
+    fn placeholder(&self) -> Option<String> {
+        self.0.placeholder()
+    }
+
     fn is_content_element(&self) -> bool {
         filter(self.0) == FilterResult::Include
     }
 
     fn is_enabled(&self) -> bool {
         !self.0.is_disabled()
     }
@@ -848,14 +852,15 @@
 }
 
 properties! {
     (ControlType, control_type),
     (LocalizedControlType, localized_control_type),
     (Name, name),
     (FullDescription, description),
+    (HelpText, placeholder),
     (IsContentElement, is_content_element),
     (IsControlElement, is_content_element),
     (IsEnabled, is_enabled),
     (IsKeyboardFocusable, is_focusable),
     (HasKeyboardFocus, is_focused),
     (LiveSetting, live_setting),
     (ClassName, class_name)
```

### Comparing `accesskit-0.3.2/platforms/windows/src/subclass.rs` & `accesskit-0.3.3/platforms/windows/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/tests/mod.rs` & `accesskit-0.3.3/platforms/windows/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/tests/simple.rs` & `accesskit-0.3.3/platforms/windows/src/tests/simple.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/tests/subclassed.rs` & `accesskit-0.3.3/platforms/windows/src/tests/subclassed.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/text.rs` & `accesskit-0.3.3/platforms/windows/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/windows/src/util.rs` & `accesskit-0.3.3/platforms/windows/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/consumer/CHANGELOG.md` & `accesskit-0.3.3/consumer/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,30 @@
   * dependencies
     * accesskit bumped from 0.11.1 to 0.11.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
 
+## [0.21.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.20.0...accesskit_consumer-v0.21.0) (2024-05-26)
+
+
+### Features
+
+* Add basic text support on Unix ([#362](https://github.com/AccessKit/accesskit/issues/362)) ([52540f8](https://github.com/AccessKit/accesskit/commit/52540f82cf9fc148358351ed486bab3e7e91f1d6))
+* Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
+
+
+### Bug Fixes
+
+* Clamp character indices when converting a text selection to a range ([#416](https://github.com/AccessKit/accesskit/issues/416)) ([5c550af](https://github.com/AccessKit/accesskit/commit/5c550af7afc81b3a32c30d31327ff95b93718545))
+* Fix a logic error that sometimes caused filtered traversal to stop prematurely ([#412](https://github.com/AccessKit/accesskit/issues/412)) ([9946d38](https://github.com/AccessKit/accesskit/commit/9946d38b9d13489517713f43284cf6b96d88cb8c))
+* Go back to detecting unchanged nodes when processing tree updates ([#415](https://github.com/AccessKit/accesskit/issues/415)) ([489302d](https://github.com/AccessKit/accesskit/commit/489302db7143a016605145682b989ab18583d59c))
+* Update minimum version of immutable-chunkmap ([#419](https://github.com/AccessKit/accesskit/issues/419)) ([893f688](https://github.com/AccessKit/accesskit/commit/893f68845dd322da5f3ae4d39fc2b1cc01f88888))
+
 ## [0.20.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.19.1...accesskit_consumer-v0.20.0) (2024-05-13)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Restore full copy-on-write tree snapshots, now using `immutable-chunkmap` ([#365](https://github.com/AccessKit/accesskit/issues/365))
```

### Comparing `accesskit-0.3.2/consumer/src/filters.rs` & `accesskit-0.3.3/consumer/src/filters.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/consumer/src/iterators.rs` & `accesskit-0.3.3/consumer/src/iterators.rs`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     while let Some(current) = next {
         if let Some(Some(child)) = consider_children.then(|| current.children().next()) {
             let result = filter(&child);
             next = Some(child);
             if result == FilterResult::Include {
                 return next;
             }
+            consider_children = result == FilterResult::ExcludeNode;
         } else if let Some(sibling) = current.following_siblings().next() {
             let result = filter(&sibling);
             next = Some(sibling);
             if result == FilterResult::Include {
                 return next;
             }
             if result == FilterResult::ExcludeNode {
@@ -225,14 +226,15 @@
     while let Some(current) = previous {
         if let Some(Some(child)) = consider_children.then(|| current.children().next_back()) {
             let result = filter(&child);
             previous = Some(child);
             if result == FilterResult::Include {
                 return previous;
             }
+            consider_children = result == FilterResult::ExcludeNode;
         } else if let Some(sibling) = current.preceding_siblings().next() {
             let result = filter(&sibling);
             previous = Some(sibling);
             if result == FilterResult::Include {
                 return previous;
             }
             if result == FilterResult::ExcludeNode {
@@ -625,15 +627,15 @@
             .state()
             .root()
             .following_filtered_siblings(test_tree_filter)
             .next()
             .is_none());
         assert_eq!(
             [
-                STATIC_TEXT_1_0_ID,
+                STATIC_TEXT_1_1_ID,
                 PARAGRAPH_2_ID,
                 STATIC_TEXT_3_1_0_ID,
                 BUTTON_3_2_ID
             ],
             tree.state()
                 .node_by_id(PARAGRAPH_0_ID)
                 .unwrap()
@@ -669,15 +671,15 @@
             .next_back()
             .is_none());
         assert_eq!(
             [
                 BUTTON_3_2_ID,
                 STATIC_TEXT_3_1_0_ID,
                 PARAGRAPH_2_ID,
-                STATIC_TEXT_1_0_ID
+                STATIC_TEXT_1_1_ID
             ],
             tree.state()
                 .node_by_id(PARAGRAPH_0_ID)
                 .unwrap()
                 .following_filtered_siblings(test_tree_filter)
                 .rev()
                 .map(|node| node.id())
@@ -708,24 +710,24 @@
         assert!(tree
             .state()
             .root()
             .preceding_filtered_siblings(test_tree_filter)
             .next()
             .is_none());
         assert_eq!(
-            [PARAGRAPH_2_ID, STATIC_TEXT_1_0_ID, PARAGRAPH_0_ID],
+            [PARAGRAPH_2_ID, STATIC_TEXT_1_1_ID, PARAGRAPH_0_ID],
             tree.state()
                 .node_by_id(PARAGRAPH_3_IGNORED_ID)
                 .unwrap()
                 .preceding_filtered_siblings(test_tree_filter)
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
         assert_eq!(
-            [PARAGRAPH_2_ID, STATIC_TEXT_1_0_ID, PARAGRAPH_0_ID],
+            [PARAGRAPH_2_ID, STATIC_TEXT_1_1_ID, PARAGRAPH_0_ID],
             tree.state()
                 .node_by_id(STATIC_TEXT_3_1_0_ID)
                 .unwrap()
                 .preceding_filtered_siblings(test_tree_filter)
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
@@ -744,25 +746,25 @@
         assert!(tree
             .state()
             .root()
             .preceding_filtered_siblings(test_tree_filter)
             .next_back()
             .is_none());
         assert_eq!(
-            [PARAGRAPH_0_ID, STATIC_TEXT_1_0_ID, PARAGRAPH_2_ID],
+            [PARAGRAPH_0_ID, STATIC_TEXT_1_1_ID, PARAGRAPH_2_ID],
             tree.state()
                 .node_by_id(PARAGRAPH_3_IGNORED_ID)
                 .unwrap()
                 .preceding_filtered_siblings(test_tree_filter)
                 .rev()
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
         );
         assert_eq!(
-            [PARAGRAPH_0_ID, STATIC_TEXT_1_0_ID, PARAGRAPH_2_ID],
+            [PARAGRAPH_0_ID, STATIC_TEXT_1_1_ID, PARAGRAPH_2_ID],
             tree.state()
                 .node_by_id(STATIC_TEXT_3_1_0_ID)
                 .unwrap()
                 .preceding_filtered_siblings(test_tree_filter)
                 .rev()
                 .map(|node| node.id())
                 .collect::<Vec<NodeId>>()[..]
@@ -778,15 +780,15 @@
 
     #[test]
     fn filtered_children() {
         let tree = test_tree();
         assert_eq!(
             [
                 PARAGRAPH_0_ID,
-                STATIC_TEXT_1_0_ID,
+                STATIC_TEXT_1_1_ID,
                 PARAGRAPH_2_ID,
                 STATIC_TEXT_3_1_0_ID,
                 BUTTON_3_2_ID
             ],
             tree.state()
                 .root()
                 .filtered_children(test_tree_filter)
@@ -813,15 +815,15 @@
     fn filtered_children_reversed() {
         let tree = test_tree();
         assert_eq!(
             [
                 BUTTON_3_2_ID,
                 STATIC_TEXT_3_1_0_ID,
                 PARAGRAPH_2_ID,
-                STATIC_TEXT_1_0_ID,
+                STATIC_TEXT_1_1_ID,
                 PARAGRAPH_0_ID
             ],
             tree.state()
                 .root()
                 .filtered_children(test_tree_filter)
                 .rev()
                 .map(|node| node.id())
```

### Comparing `accesskit-0.3.2/consumer/src/lib.rs` & `accesskit-0.3.3/consumer/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -26,23 +26,27 @@
 
     use crate::FilterResult;
 
     pub const ROOT_ID: NodeId = NodeId(0);
     pub const PARAGRAPH_0_ID: NodeId = NodeId(1);
     pub const STATIC_TEXT_0_0_IGNORED_ID: NodeId = NodeId(2);
     pub const PARAGRAPH_1_IGNORED_ID: NodeId = NodeId(3);
-    pub const STATIC_TEXT_1_0_ID: NodeId = NodeId(4);
-    pub const PARAGRAPH_2_ID: NodeId = NodeId(5);
-    pub const STATIC_TEXT_2_0_ID: NodeId = NodeId(6);
-    pub const PARAGRAPH_3_IGNORED_ID: NodeId = NodeId(7);
-    pub const EMPTY_CONTAINER_3_0_IGNORED_ID: NodeId = NodeId(8);
-    pub const LINK_3_1_IGNORED_ID: NodeId = NodeId(9);
-    pub const STATIC_TEXT_3_1_0_ID: NodeId = NodeId(10);
-    pub const BUTTON_3_2_ID: NodeId = NodeId(11);
-    pub const EMPTY_CONTAINER_3_3_IGNORED_ID: NodeId = NodeId(12);
+    pub const BUTTON_1_0_HIDDEN_ID: NodeId = NodeId(4);
+    pub const CONTAINER_1_0_0_HIDDEN_ID: NodeId = NodeId(5);
+    pub const STATIC_TEXT_1_1_ID: NodeId = NodeId(6);
+    pub const BUTTON_1_2_HIDDEN_ID: NodeId = NodeId(7);
+    pub const CONTAINER_1_2_0_HIDDEN_ID: NodeId = NodeId(8);
+    pub const PARAGRAPH_2_ID: NodeId = NodeId(9);
+    pub const STATIC_TEXT_2_0_ID: NodeId = NodeId(10);
+    pub const PARAGRAPH_3_IGNORED_ID: NodeId = NodeId(11);
+    pub const EMPTY_CONTAINER_3_0_IGNORED_ID: NodeId = NodeId(12);
+    pub const LINK_3_1_IGNORED_ID: NodeId = NodeId(13);
+    pub const STATIC_TEXT_3_1_0_ID: NodeId = NodeId(14);
+    pub const BUTTON_3_2_ID: NodeId = NodeId(15);
+    pub const EMPTY_CONTAINER_3_3_IGNORED_ID: NodeId = NodeId(16);
 
     pub fn test_tree() -> crate::tree::Tree {
         let root = {
             let mut builder = NodeBuilder::new(Role::RootWebArea);
             builder.set_children(vec![
                 PARAGRAPH_0_ID,
                 PARAGRAPH_1_IGNORED_ID,
@@ -66,26 +70,54 @@
             builder.set_transform(Affine::translate(Vec2::new(10.0, 40.0)));
             builder.set_bounds(Rect {
                 x0: 0.0,
                 y0: 0.0,
                 x1: 800.0,
                 y1: 40.0,
             });
-            builder.set_children(vec![STATIC_TEXT_1_0_ID]);
+            builder.set_children(vec![
+                BUTTON_1_0_HIDDEN_ID,
+                STATIC_TEXT_1_1_ID,
+                BUTTON_1_2_HIDDEN_ID,
+            ]);
+            builder.build()
+        };
+        let button_1_0_hidden = {
+            let mut builder = NodeBuilder::new(Role::Button);
+            builder.set_name("button_1_0_hidden");
+            builder.set_hidden();
+            builder.set_children(vec![CONTAINER_1_0_0_HIDDEN_ID]);
+            builder.build()
+        };
+        let container_1_0_0_hidden = {
+            let mut builder = NodeBuilder::new(Role::GenericContainer);
+            builder.set_hidden();
             builder.build()
         };
-        let static_text_1_0 = {
+        let static_text_1_1 = {
             let mut builder = NodeBuilder::new(Role::StaticText);
             builder.set_bounds(Rect {
                 x0: 10.0,
                 y0: 10.0,
                 x1: 90.0,
                 y1: 30.0,
             });
-            builder.set_name("static_text_1_0");
+            builder.set_name("static_text_1_1");
+            builder.build()
+        };
+        let button_1_2_hidden = {
+            let mut builder = NodeBuilder::new(Role::Button);
+            builder.set_name("button_1_2_hidden");
+            builder.set_hidden();
+            builder.set_children(vec![CONTAINER_1_2_0_HIDDEN_ID]);
+            builder.build()
+        };
+        let container_1_2_0_hidden = {
+            let mut builder = NodeBuilder::new(Role::GenericContainer);
+            builder.set_hidden();
             builder.build()
         };
         let paragraph_2 = {
             let mut builder = NodeBuilder::new(Role::Paragraph);
             builder.set_children(vec![STATIC_TEXT_2_0_ID]);
             builder.build()
         };
@@ -124,15 +156,19 @@
         let empty_container_3_3_ignored = NodeBuilder::new(Role::GenericContainer).build();
         let initial_update = TreeUpdate {
             nodes: vec![
                 (ROOT_ID, root),
                 (PARAGRAPH_0_ID, paragraph_0),
                 (STATIC_TEXT_0_0_IGNORED_ID, static_text_0_0_ignored),
                 (PARAGRAPH_1_IGNORED_ID, paragraph_1_ignored),
-                (STATIC_TEXT_1_0_ID, static_text_1_0),
+                (BUTTON_1_0_HIDDEN_ID, button_1_0_hidden),
+                (CONTAINER_1_0_0_HIDDEN_ID, container_1_0_0_hidden),
+                (STATIC_TEXT_1_1_ID, static_text_1_1),
+                (BUTTON_1_2_HIDDEN_ID, button_1_2_hidden),
+                (CONTAINER_1_2_0_HIDDEN_ID, container_1_2_0_hidden),
                 (PARAGRAPH_2_ID, paragraph_2),
                 (STATIC_TEXT_2_0_ID, static_text_2_0),
                 (PARAGRAPH_3_IGNORED_ID, paragraph_3_ignored),
                 (EMPTY_CONTAINER_3_0_IGNORED_ID, empty_container_3_0_ignored),
                 (LINK_3_1_IGNORED_ID, link_3_1_ignored),
                 (STATIC_TEXT_3_1_0_ID, static_text_3_1_0),
                 (BUTTON_3_2_ID, button_3_2),
@@ -142,15 +178,17 @@
             focus: ROOT_ID,
         };
         crate::tree::Tree::new(initial_update, false)
     }
 
     pub fn test_tree_filter(node: &crate::Node) -> FilterResult {
         let id = node.id();
-        if id == STATIC_TEXT_0_0_IGNORED_ID
+        if node.is_hidden() {
+            FilterResult::ExcludeSubtree
+        } else if id == STATIC_TEXT_0_0_IGNORED_ID
             || id == PARAGRAPH_1_IGNORED_ID
             || id == PARAGRAPH_3_IGNORED_ID
             || id == EMPTY_CONTAINER_3_0_IGNORED_ID
             || id == LINK_3_1_IGNORED_ID
             || id == EMPTY_CONTAINER_3_3_IGNORED_ID
         {
             FilterResult::ExcludeNode
```

### Comparing `accesskit-0.3.2/consumer/src/node.rs` & `accesskit-0.3.3/consumer/src/node.rs`

 * *Files 1% similar despite different names*

```diff
@@ -507,14 +507,20 @@
 
     pub fn description(&self) -> Option<String> {
         self.data()
             .description()
             .map(|description| description.to_string())
     }
 
+    pub fn placeholder(&self) -> Option<String> {
+        self.data()
+            .placeholder()
+            .map(|placeholder| placeholder.to_string())
+    }
+
     pub fn value(&self) -> Option<String> {
         if let Some(value) = &self.data().value() {
             Some(value.to_string())
         } else if self.supports_text_ranges() && !self.is_multiline() {
             Some(self.document_range().text())
         } else {
             None
@@ -705,15 +711,15 @@
 
     #[test]
     fn filtered_parent() {
         let tree = test_tree();
         assert_eq!(
             ROOT_ID,
             tree.state()
-                .node_by_id(STATIC_TEXT_1_0_ID)
+                .node_by_id(STATIC_TEXT_1_1_ID)
                 .unwrap()
                 .filtered_parent(&test_tree_filter)
                 .unwrap()
                 .id()
         );
         assert!(tree
             .state()
@@ -867,37 +873,37 @@
             Some(Rect {
                 x0: 20.0,
                 y0: 50.0,
                 x1: 100.0,
                 y1: 70.0,
             }),
             tree.state()
-                .node_by_id(STATIC_TEXT_1_0_ID)
+                .node_by_id(STATIC_TEXT_1_1_ID)
                 .unwrap()
                 .bounding_box()
         );
     }
 
     #[test]
     fn node_at_point() {
         let tree = test_tree();
         assert!(tree
             .state()
             .root()
             .node_at_point(Point::new(10.0, 40.0), &test_tree_filter)
             .is_none());
         assert_eq!(
-            Some(STATIC_TEXT_1_0_ID),
+            Some(STATIC_TEXT_1_1_ID),
             tree.state()
                 .root()
                 .node_at_point(Point::new(20.0, 50.0), &test_tree_filter)
                 .map(|node| node.id())
         );
         assert_eq!(
-            Some(STATIC_TEXT_1_0_ID),
+            Some(STATIC_TEXT_1_1_ID),
             tree.state()
                 .root()
                 .node_at_point(Point::new(50.0, 60.0), &test_tree_filter)
                 .map(|node| node.id())
         );
         assert!(tree
             .state()
```

### Comparing `accesskit-0.3.2/consumer/src/text.rs` & `accesskit-0.3.3/consumer/src/text.rs`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,28 @@
         }
         Some(Self {
             node,
             character_index,
         })
     }
 
+    fn clamped_upgrade(tree_state: &'a TreeState, weak: WeakPosition) -> Option<Self> {
+        let node = tree_state.node_by_id(weak.node)?;
+        if node.role() != Role::InlineTextBox {
+            return None;
+        }
+        let character_index = weak
+            .character_index
+            .min(node.data().character_lengths().len());
+        Some(Self {
+            node,
+            character_index,
+        })
+    }
+
     fn is_word_start(&self) -> bool {
         let mut total_length = 0usize;
         for length in self.node.data().word_lengths().iter() {
             if total_length == self.character_index {
                 return true;
             }
             total_length += *length as usize;
@@ -230,14 +244,32 @@
         self.inner.is_document_end(&self.root_node)
     }
 
     pub fn to_degenerate_range(&self) -> Range<'a> {
         Range::new(self.root_node, self.inner, self.inner)
     }
 
+    pub fn to_global_usv_index(&self) -> usize {
+        let mut total_length = 0usize;
+        for node in self.root_node.inline_text_boxes() {
+            let node_text = node.data().value().unwrap();
+            if node.id() == self.inner.node.id() {
+                let character_lengths = node.data().character_lengths();
+                let slice_end = character_lengths[..self.inner.character_index]
+                    .iter()
+                    .copied()
+                    .map(usize::from)
+                    .sum::<usize>();
+                return total_length + node_text[..slice_end].chars().count();
+            }
+            total_length += node_text.chars().count();
+        }
+        panic!("invalid position")
+    }
+
     pub fn to_global_utf16_index(&self) -> usize {
         let mut total_length = 0usize;
         for node in self.root_node.inline_text_boxes() {
             let node_text = node.data().value().unwrap();
             if node.id() == self.inner.node.id() {
                 let character_lengths = node.data().character_lengths();
                 let slice_end = character_lengths[..self.inner.character_index]
@@ -868,16 +900,16 @@
 
     pub fn has_text_selection(&self) -> bool {
         self.data().text_selection().is_some()
     }
 
     pub fn text_selection(&self) -> Option<Range> {
         self.data().text_selection().map(|selection| {
-            let anchor = InnerPosition::upgrade(self.tree_state, selection.anchor).unwrap();
-            let focus = InnerPosition::upgrade(self.tree_state, selection.focus).unwrap();
+            let anchor = InnerPosition::clamped_upgrade(self.tree_state, selection.anchor).unwrap();
+            let focus = InnerPosition::clamped_upgrade(self.tree_state, selection.focus).unwrap();
             Range::new(*self, anchor, focus)
         })
     }
 
     pub fn text_selection_focus(&self) -> Option<Position> {
         self.data().text_selection().map(|selection| {
             let focus = InnerPosition::upgrade(self.tree_state, selection.focus).unwrap();
@@ -978,14 +1010,56 @@
             pos
         } else {
             pos.forward_to_line_end()
         };
         Some(Range::new(*self, pos.inner, end.inner))
     }
 
+    pub fn text_position_from_global_usv_index(&self, index: usize) -> Option<Position> {
+        let mut total_length = 0usize;
+        for node in self.inline_text_boxes() {
+            let node_text = node.data().value().unwrap();
+            let node_text_length = node_text.chars().count();
+            let new_total_length = total_length + node_text_length;
+            if index >= total_length && index < new_total_length {
+                let index = index - total_length;
+                let mut utf8_length = 0usize;
+                let mut usv_length = 0usize;
+                for (character_index, utf8_char_length) in
+                    node.data().character_lengths().iter().enumerate()
+                {
+                    let new_utf8_length = utf8_length + (*utf8_char_length as usize);
+                    let char_str = &node_text[utf8_length..new_utf8_length];
+                    let usv_char_length = char_str.chars().count();
+                    let new_usv_length = usv_length + usv_char_length;
+                    if index >= usv_length && index < new_usv_length {
+                        return Some(Position {
+                            root_node: *self,
+                            inner: InnerPosition {
+                                node,
+                                character_index,
+                            },
+                        });
+                    }
+                    utf8_length = new_utf8_length;
+                    usv_length = new_usv_length;
+                }
+                panic!("index out of range");
+            }
+            total_length = new_total_length;
+        }
+        if index == total_length {
+            return Some(Position {
+                root_node: *self,
+                inner: self.document_end(),
+            });
+        }
+        None
+    }
+
     pub fn text_position_from_global_utf16_index(&self, index: usize) -> Option<Position> {
         let mut total_length = 0usize;
         for node in self.inline_text_boxes() {
             let node_text = node.data().value().unwrap();
             let node_text_length = node_text.chars().map(char::len_utf16).sum::<usize>();
             let new_total_length = total_length + node_text_length;
             if index >= total_length && index < new_total_length {
@@ -1230,14 +1304,29 @@
             focus: TextPosition {
                 node: NodeId(7),
                 character_index: 0,
             },
         }
     }
 
+    fn multiline_past_end_selection() -> TextSelection {
+        use accesskit::TextPosition;
+
+        TextSelection {
+            anchor: TextPosition {
+                node: NodeId(7),
+                character_index: 3,
+            },
+            focus: TextPosition {
+                node: NodeId(7),
+                character_index: 3,
+            },
+        }
+    }
+
     fn multiline_wrapped_line_end_selection() -> TextSelection {
         use accesskit::TextPosition;
 
         TextSelection {
             anchor: TextPosition {
                 node: NodeId(2),
                 character_index: 38,
@@ -1659,14 +1748,39 @@
         {
             let pos = node.text_position_at_point(Point::new(250.0, 122.0));
             assert!(pos.is_document_end());
         }
     }
 
     #[test]
+    fn to_global_usv_index() {
+        let tree = main_multiline_tree(None);
+        let state = tree.state();
+        let node = state.node_by_id(NodeId(1)).unwrap();
+
+        {
+            let range = node.document_range();
+            assert_eq!(range.start().to_global_usv_index(), 0);
+            assert_eq!(range.end().to_global_usv_index(), 97);
+        }
+
+        {
+            let range = node.document_range();
+            let pos = range.start().forward_to_line_end();
+            assert_eq!(pos.to_global_usv_index(), 38);
+            let pos = range.start().forward_to_line_start();
+            assert_eq!(pos.to_global_usv_index(), 38);
+            let pos = pos.forward_to_character_start();
+            assert_eq!(pos.to_global_usv_index(), 39);
+            let pos = pos.forward_to_line_start();
+            assert_eq!(pos.to_global_usv_index(), 55);
+        }
+    }
+
+    #[test]
     fn to_global_utf16_index() {
         let tree = main_multiline_tree(None);
         let state = tree.state();
         let node = state.node_by_id(NodeId(1)).unwrap();
 
         {
             let range = node.document_range();
@@ -1749,14 +1863,93 @@
             assert_eq!(range.text(), "");
         }
 
         assert!(node.line_range_from_index(6).is_none());
     }
 
     #[test]
+    fn text_position_from_global_usv_index() {
+        let tree = main_multiline_tree(None);
+        let state = tree.state();
+        let node = state.node_by_id(NodeId(1)).unwrap();
+
+        {
+            let pos = node.text_position_from_global_usv_index(0).unwrap();
+            assert!(pos.is_document_start());
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(17).unwrap();
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "\u{a0}");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(18).unwrap();
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "l");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(37).unwrap();
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), " ");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(38).unwrap();
+            assert!(!pos.is_paragraph_start());
+            assert!(pos.is_line_start());
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "t");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(54).unwrap();
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "\n");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(55).unwrap();
+            assert!(pos.is_paragraph_start());
+            assert!(pos.is_line_start());
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "A");
+        }
+
+        for i in 94..=95 {
+            let pos = node.text_position_from_global_usv_index(i).unwrap();
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "\u{1f44d}\u{1f3fb}");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(96).unwrap();
+            let mut range = pos.to_degenerate_range();
+            range.set_end(pos.forward_to_character_end());
+            assert_eq!(range.text(), "\n");
+        }
+
+        {
+            let pos = node.text_position_from_global_usv_index(97).unwrap();
+            assert!(pos.is_document_end());
+        }
+
+        assert!(node.text_position_from_global_usv_index(98).is_none());
+    }
+
+    #[test]
     fn text_position_from_global_utf16_index() {
         let tree = main_multiline_tree(None);
         let state = tree.state();
         let node = state.node_by_id(NodeId(1)).unwrap();
 
         {
             let pos = node.text_position_from_global_utf16_index(0).unwrap();
@@ -1826,8 +2019,16 @@
         {
             let pos = node.text_position_from_global_utf16_index(99).unwrap();
             assert!(pos.is_document_end());
         }
 
         assert!(node.text_position_from_global_utf16_index(100).is_none());
     }
+
+    #[test]
+    fn multiline_selection_clamping() {
+        let tree = main_multiline_tree(Some(multiline_past_end_selection()));
+        let state = tree.state();
+        let node = state.node_by_id(NodeId(1)).unwrap();
+        let _ = node.text_selection().unwrap();
+    }
 }
```

### Comparing `accesskit-0.3.2/consumer/src/tree.rs` & `accesskit-0.3.3/consumer/src/tree.rs`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,14 @@
 
     fn update(
         &mut self,
         update: TreeUpdate,
         is_host_focused: bool,
         mut changes: Option<&mut InternalChanges>,
     ) {
-        // First, if we're collecting changes, collect the IDS of any nodes
-        // in the update that were in the previous state.
-        if let Some(changes) = &mut changes {
-            for (node_id, _) in &update.nodes {
-                if self.nodes.get(node_id).is_some() {
-                    changes.updated_node_ids.insert(*node_id);
-                }
-            }
-        }
-
         let mut orphans = HashSet::new();
 
         if let Some(tree) = update.tree {
             if tree.root != self.data.root {
                 orphans.insert(self.data.root);
             }
             self.data = tree;
@@ -119,15 +109,20 @@
                     node_state.parent_and_index = None;
                 }
                 for child_id in node_state.data.children().iter() {
                     if !seen_child_ids.contains(child_id) {
                         orphans.insert(*child_id);
                     }
                 }
-                node_state.data = Arc::new(node_data);
+                if *node_state.data != node_data {
+                    node_state.data = Arc::new(node_data);
+                    if let Some(changes) = &mut changes {
+                        changes.updated_node_ids.insert(node_id);
+                    }
+                }
             } else if let Some(parent_and_index) = pending_children.remove(&node_id) {
                 add_node(
                     &mut self.nodes,
                     &mut changes,
                     Some(parent_and_index),
                     node_id,
                     node_data,
@@ -730,8 +725,57 @@
         tree.update_and_process_changes(second_update, &mut handler);
         assert!(handler.got_updated_child_node);
         assert_eq!(
             Some("bar".into()),
             tree.state().node_by_id(NodeId(1)).unwrap().name()
         );
     }
+
+    // Verify that if an update consists entirely of node data and tree data
+    // that's the same as before, no changes are reported. This is useful
+    // for a provider that constructs a fresh tree every time, such as
+    // an immediate-mode GUI.
+    #[test]
+    fn no_change_update() {
+        let update = TreeUpdate {
+            nodes: vec![
+                (NodeId(0), {
+                    let mut builder = NodeBuilder::new(Role::Window);
+                    builder.set_children(vec![NodeId(1)]);
+                    builder.build()
+                }),
+                (NodeId(1), {
+                    let mut builder = NodeBuilder::new(Role::Button);
+                    builder.set_name("foo");
+                    builder.build()
+                }),
+            ],
+            tree: Some(Tree::new(NodeId(0))),
+            focus: NodeId(0),
+        };
+        let mut tree = super::Tree::new(update.clone(), false);
+        struct Handler;
+        fn unexpected_change() {
+            panic!("expected no changes");
+        }
+        impl super::ChangeHandler for Handler {
+            fn node_added(&mut self, _node: &crate::Node) {
+                unexpected_change();
+            }
+            fn node_updated(&mut self, _old_node: &crate::Node, _new_node: &crate::Node) {
+                unexpected_change();
+            }
+            fn focus_moved(
+                &mut self,
+                _old_node: Option<&crate::Node>,
+                _new_node: Option<&crate::Node>,
+            ) {
+                unexpected_change();
+            }
+            fn node_removed(&mut self, _node: &crate::Node) {
+                unexpected_change();
+            }
+        }
+        let mut handler = Handler {};
+        tree.update_and_process_changes(update, &mut handler);
+    }
 }
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/Cargo.toml` & `accesskit-0.3.3/platforms/atspi-common/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "accesskit_atspi_common"
-version = "0.4.2"
+version = "0.5.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: core AT-SPI translation layer"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.20.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.21.0", path = "../../consumer" }
 atspi-common = { version = "0.3.0", default-features = false }
 serde = "1.0"
 thiserror = "1.0.39"
 zvariant = { version = "3", default-features = false }
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/CHANGELOG.md` & `accesskit-0.3.3/platforms/atspi-common/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,35 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_consumer bumped from 0.19.0 to 0.19.1
 
+## [0.5.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.4.2...accesskit_atspi_common-v0.5.0) (2024-05-26)
+
+
+### Features
+
+* Add basic text support on Unix ([#362](https://github.com/AccessKit/accesskit/issues/362)) ([52540f8](https://github.com/AccessKit/accesskit/commit/52540f82cf9fc148358351ed486bab3e7e91f1d6))
+* Expose the `placeholder` property ([#417](https://github.com/AccessKit/accesskit/issues/417)) ([8f4a0a1](https://github.com/AccessKit/accesskit/commit/8f4a0a1c10f83fcc8580a37d8013fec2d110865b))
+
+
+### Bug Fixes
+
+* Don't fire events for filtered children on Unix ([#414](https://github.com/AccessKit/accesskit/issues/414)) ([2bcb1b6](https://github.com/AccessKit/accesskit/commit/2bcb1b63e88b801b194a4db50059fa063efbee64))
+* Improve how coordinates are computed on Unix ([#420](https://github.com/AccessKit/accesskit/issues/420)) ([fc5125e](https://github.com/AccessKit/accesskit/commit/fc5125e27f8f4f655e1de5049d0d53536284d9a0))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.20.0 to 0.21.0
+
 ## [0.4.2](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.4.1...accesskit_atspi_common-v0.4.2) (2024-05-13)
 
 
 ### Bug Fixes
 
 * Fix platform adapters to support copy-on-write tree snapshots again ([#411](https://github.com/AccessKit/accesskit/issues/411)) ([d3a130a](https://github.com/AccessKit/accesskit/commit/d3a130a5ec8ae1d9edf0bf85a44f35f0e365242c))
 * Return to handling focus events directly, after generic node changes ([#409](https://github.com/AccessKit/accesskit/issues/409)) ([cd2e35e](https://github.com/AccessKit/accesskit/commit/cd2e35e43817405199ae6acd64ef90aee445be0b))
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/adapter.rs` & `accesskit-0.3.3/platforms/atspi-common/src/adapter.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
+// Derived from Chromium's accessibility abstraction.
+// Copyright 2017 The Chromium Authors. All rights reserved.
+// Use of this source code is governed by a BSD-style license that can be
+// found in the LICENSE.chromium file.
+
 use accesskit::{ActionHandler, NodeId, Role, TreeUpdate};
 use accesskit_consumer::{FilterResult, Node, Tree, TreeChangeHandler, TreeState};
 use atspi_common::{InterfaceSet, Live, State};
-use std::sync::{
-    atomic::{AtomicUsize, Ordering},
-    Arc, RwLock,
+use std::{
+    collections::HashSet,
+    sync::{
+        atomic::{AtomicUsize, Ordering},
+        Arc, RwLock,
+    },
 };
 
 use crate::{
     context::{ActionHandlerNoMut, ActionHandlerWrapper, AppContext, Context},
     filters::filter,
     node::{NodeIdOrRoot, NodeWrapper, PlatformNode, PlatformRoot},
     util::WindowBounds,
     AdapterCallback, Event, ObjectEvent, WindowEvent,
 };
 
 struct AdapterChangeHandler<'a> {
     adapter: &'a Adapter,
+    text_changed: HashSet<NodeId>,
 }
 
-impl AdapterChangeHandler<'_> {
+impl<'a> AdapterChangeHandler<'a> {
+    fn new(adapter: &'a Adapter) -> Self {
+        Self {
+            adapter,
+            text_changed: HashSet::new(),
+        }
+    }
+
     fn add_node(&mut self, node: &Node) {
         let role = node.role();
         let is_root = node.is_root();
         let node = NodeWrapper(node);
         let interfaces = node.interfaces();
         self.adapter.register_interfaces(node.id(), interfaces);
         if is_root && role == Role::Window {
@@ -57,24 +73,154 @@
             self.adapter.window_destroyed(node.id());
         }
         self.adapter
             .emit_object_event(node.id(), ObjectEvent::StateChanged(State::Defunct, true));
         self.adapter
             .unregister_interfaces(node.id(), node.interfaces());
     }
+
+    fn emit_text_change_if_needed_parent(&mut self, old_node: &Node, new_node: &Node) {
+        if !new_node.supports_text_ranges() || !old_node.supports_text_ranges() {
+            return;
+        }
+        let id = new_node.id();
+        if self.text_changed.contains(&id) {
+            return;
+        }
+        let old_text = old_node.document_range().text();
+        let new_text = new_node.document_range().text();
+
+        let mut old_chars = old_text.chars();
+        let mut new_chars = new_text.chars();
+        let mut prefix_usv_count = 0;
+        let mut prefix_byte_count = 0;
+        loop {
+            match (old_chars.next(), new_chars.next()) {
+                (Some(old_char), Some(new_char)) if old_char == new_char => {
+                    prefix_usv_count += 1;
+                    prefix_byte_count += new_char.len_utf8();
+                }
+                (None, None) => return,
+                _ => break,
+            }
+        }
+
+        let suffix_byte_count = old_text
+            .chars()
+            .rev()
+            .zip(new_text.chars().rev())
+            .take_while(|(old_char, new_char)| old_char == new_char)
+            .fold(0, |count, (c, _)| count + c.len_utf8());
+
+        let old_content = &old_text[prefix_byte_count..old_text.len() - suffix_byte_count];
+        if let Ok(length) = old_content.chars().count().try_into() {
+            if length > 0 {
+                self.adapter.emit_object_event(
+                    id,
+                    ObjectEvent::TextRemoved {
+                        start_index: prefix_usv_count,
+                        length,
+                        content: old_content.to_string(),
+                    },
+                );
+            }
+        }
+
+        let new_content = &new_text[prefix_byte_count..new_text.len() - suffix_byte_count];
+        if let Ok(length) = new_content.chars().count().try_into() {
+            if length > 0 {
+                self.adapter.emit_object_event(
+                    id,
+                    ObjectEvent::TextInserted {
+                        start_index: prefix_usv_count,
+                        length,
+                        content: new_content.to_string(),
+                    },
+                );
+            }
+        }
+
+        self.text_changed.insert(id);
+    }
+
+    fn emit_text_change_if_needed(&mut self, old_node: &Node, new_node: &Node) {
+        if let Role::InlineTextBox | Role::GenericContainer = new_node.role() {
+            if let (Some(old_parent), Some(new_parent)) = (
+                old_node.filtered_parent(&filter),
+                new_node.filtered_parent(&filter),
+            ) {
+                self.emit_text_change_if_needed_parent(&old_parent, &new_parent);
+            }
+        } else {
+            self.emit_text_change_if_needed_parent(old_node, new_node);
+        }
+    }
+
+    fn emit_text_selection_change(&self, old_node: Option<&Node>, new_node: &Node) {
+        if !new_node.supports_text_ranges() {
+            return;
+        }
+        let Some(old_node) = old_node else {
+            if let Some(selection) = new_node.text_selection() {
+                if !selection.is_degenerate() {
+                    self.adapter
+                        .emit_object_event(new_node.id(), ObjectEvent::TextSelectionChanged);
+                }
+            }
+            if let Some(selection_focus) = new_node.text_selection_focus() {
+                if let Ok(offset) = selection_focus.to_global_usv_index().try_into() {
+                    self.adapter
+                        .emit_object_event(new_node.id(), ObjectEvent::CaretMoved(offset));
+                }
+            }
+            return;
+        };
+        if !old_node.is_focused() || new_node.raw_text_selection() == old_node.raw_text_selection()
+        {
+            return;
+        }
+
+        if let Some(selection) = new_node.text_selection() {
+            if !selection.is_degenerate()
+                || old_node
+                    .text_selection()
+                    .map(|selection| !selection.is_degenerate())
+                    .unwrap_or(false)
+            {
+                self.adapter
+                    .emit_object_event(new_node.id(), ObjectEvent::TextSelectionChanged);
+            }
+        }
+
+        let old_caret_position = old_node
+            .raw_text_selection()
+            .map(|selection| selection.focus);
+        let new_caret_position = new_node
+            .raw_text_selection()
+            .map(|selection| selection.focus);
+        if old_caret_position != new_caret_position {
+            if let Some(selection_focus) = new_node.text_selection_focus() {
+                if let Ok(offset) = selection_focus.to_global_usv_index().try_into() {
+                    self.adapter
+                        .emit_object_event(new_node.id(), ObjectEvent::CaretMoved(offset));
+                }
+            }
+        }
+    }
 }
 
 impl TreeChangeHandler for AdapterChangeHandler<'_> {
     fn node_added(&mut self, node: &Node) {
         if filter(node) == FilterResult::Include {
             self.add_node(node);
         }
     }
 
     fn node_updated(&mut self, old_node: &Node, new_node: &Node) {
+        self.emit_text_change_if_needed(old_node, new_node);
         let filter_old = filter(old_node);
         let filter_new = filter(new_node);
         if filter_new != filter_old {
             if filter_new == FilterResult::Include {
                 self.add_node(new_node);
             } else if filter_old == FilterResult::Include {
                 self.remove_node(old_node);
@@ -87,14 +233,15 @@
             let kept_interfaces = old_interfaces & new_interfaces;
             self.adapter
                 .unregister_interfaces(new_wrapper.id(), old_interfaces ^ kept_interfaces);
             self.adapter
                 .register_interfaces(new_node.id(), new_interfaces ^ kept_interfaces);
             let bounds = *self.adapter.context.read_root_window_bounds();
             new_wrapper.notify_changes(&bounds, self.adapter, &old_wrapper);
+            self.emit_text_selection_change(Some(old_node), new_node);
         }
     }
 
     fn focus_moved(&mut self, old_node: Option<&Node>, new_node: Option<&Node>) {
         if let (None, Some(new_node)) = (old_node, new_node) {
             if let Some(root_window) = root_window(new_node.tree_state) {
                 self.adapter.window_activated(&NodeWrapper(&root_window));
@@ -103,14 +250,15 @@
             if let Some(root_window) = root_window(old_node.tree_state) {
                 self.adapter.window_deactivated(&NodeWrapper(&root_window));
             }
         }
         if let Some(node) = new_node {
             self.adapter
                 .emit_object_event(node.id(), ObjectEvent::StateChanged(State::Focused, true));
+            self.emit_text_selection_change(None, node);
         }
         if let Some(node) = old_node {
             self.adapter
                 .emit_object_event(node.id(), ObjectEvent::StateChanged(State::Focused, false));
         }
     }
 
@@ -275,21 +423,21 @@
 
     pub fn set_root_window_bounds(&mut self, new_bounds: WindowBounds) {
         let mut bounds = self.context.root_window_bounds.write().unwrap();
         *bounds = new_bounds;
     }
 
     pub fn update(&mut self, update: TreeUpdate) {
-        let mut handler = AdapterChangeHandler { adapter: self };
+        let mut handler = AdapterChangeHandler::new(self);
         let mut tree = self.context.tree.write().unwrap();
         tree.update_and_process_changes(update, &mut handler);
     }
 
     pub fn update_window_focus_state(&mut self, is_focused: bool) {
-        let mut handler = AdapterChangeHandler { adapter: self };
+        let mut handler = AdapterChangeHandler::new(self);
         let mut tree = self.context.tree.write().unwrap();
         tree.update_host_focus_state_and_process_changes(is_focused, &mut handler);
     }
 
     fn window_created(&self, adapter_index: usize, window: NodeId) {
         self.emit_root_object_event(ObjectEvent::ChildAdded(adapter_index, window));
     }
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/callback.rs` & `accesskit-0.3.3/platforms/atspi-common/src/callback.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/context.rs` & `accesskit-0.3.3/platforms/atspi-common/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/events.rs` & `accesskit-0.3.3/platforms/atspi-common/src/events.rs`

 * *Files 17% similar despite different names*

```diff
@@ -32,18 +32,30 @@
 
 #[allow(clippy::enum_variant_names)]
 #[derive(Debug)]
 pub enum ObjectEvent {
     ActiveDescendantChanged(NodeId),
     Announcement(String, Live),
     BoundsChanged(Rect),
+    CaretMoved(i32),
     ChildAdded(usize, NodeId),
     ChildRemoved(NodeId),
     PropertyChanged(Property),
     StateChanged(State, bool),
+    TextInserted {
+        start_index: i32,
+        length: i32,
+        content: String,
+    },
+    TextRemoved {
+        start_index: i32,
+        length: i32,
+        content: String,
+    },
+    TextSelectionChanged,
 }
 
 #[derive(Debug)]
 pub enum WindowEvent {
     Activated,
     Deactivated,
 }
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/lib.rs` & `accesskit-0.3.3/platforms/atspi-common/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 mod events;
 mod filters;
 mod node;
 mod rect;
 pub mod simplified;
 mod util;
 
-pub use atspi_common::{CoordType, InterfaceSet, Layer, Role, State, StateSet};
+pub use atspi_common::{
+    CoordType, Granularity, InterfaceSet, Layer, Role, ScrollType, State, StateSet,
+};
 
 pub use action::*;
 pub use adapter::{next_adapter_id, Adapter};
 pub use callback::AdapterCallback;
 pub use context::{ActionHandlerNoMut, ActionHandlerWrapper, AppContext};
 pub use error::*;
 pub use events::*;
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/node.rs` & `accesskit-0.3.3/platforms/atspi-common/src/node.rs`

 * *Files 16% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 
 use accesskit::{
     Action, ActionData, ActionRequest, Affine, DefaultActionVerb, Live, NodeId, Point, Rect, Role,
     Toggled,
 };
 use accesskit_consumer::{FilterResult, Node, TreeState};
 use atspi_common::{
-    CoordType, Interface, InterfaceSet, Layer, Live as AtspiLive, Role as AtspiRole, State,
-    StateSet,
+    CoordType, Granularity, Interface, InterfaceSet, Layer, Live as AtspiLive, Role as AtspiRole,
+    ScrollType, State, StateSet,
 };
 use std::{
+    collections::HashMap,
     hash::{Hash, Hasher},
     iter::FusedIterator,
     sync::{Arc, RwLock, RwLockReadGuard, Weak},
 };
 
 use crate::{
     adapter::Adapter,
     context::{AppContext, Context},
     filters::filter,
-    util::WindowBounds,
+    util::*,
     Action as AtspiAction, Error, ObjectEvent, Property, Rect as AtspiRect, Result,
 };
 
 pub(crate) struct NodeWrapper<'a>(pub(crate) &'a Node<'a>);
 
 impl<'a> NodeWrapper<'a> {
     pub(crate) fn name(&self) -> Option<String> {
@@ -46,23 +47,14 @@
         self.0.parent_id()
     }
 
     pub(crate) fn id(&self) -> NodeId {
         self.0.id()
     }
 
-    fn child_ids(
-        &self,
-    ) -> impl DoubleEndedIterator<Item = NodeId>
-           + ExactSizeIterator<Item = NodeId>
-           + FusedIterator<Item = NodeId>
-           + '_ {
-        self.0.child_ids()
-    }
-
     fn filtered_child_ids(
         &self,
     ) -> impl DoubleEndedIterator<Item = NodeId> + FusedIterator<Item = NodeId> + '_ {
         self.0.filtered_children(&filter).map(|child| child.id())
     }
 
     pub(crate) fn role(&self) -> AtspiRole {
@@ -287,14 +279,17 @@
     pub(crate) fn state(&self, is_window_focused: bool) -> StateSet {
         let state = self.0;
         let atspi_role = self.role();
         let mut atspi_state = StateSet::empty();
         if state.parent_id().is_none() && state.role() == Role::Window && is_window_focused {
             atspi_state.insert(State::Active);
         }
+        if state.is_text_input() && !state.is_read_only() {
+            atspi_state.insert(State::Editable);
+        }
         // TODO: Focus and selection.
         if state.is_focusable() {
             atspi_state.insert(State::Focusable);
         }
         let filter_result = filter(self.0);
         if filter_result == FilterResult::Include {
             atspi_state.insert(State::Visible | State::Showing);
@@ -342,38 +337,53 @@
         if self.is_focused() {
             atspi_state.insert(State::Focused);
         }
 
         atspi_state
     }
 
+    fn attributes(&self) -> HashMap<&'static str, String> {
+        let mut attributes = HashMap::new();
+        if let Some(placeholder) = self.0.placeholder() {
+            attributes.insert("placeholder-text", placeholder);
+        }
+        attributes
+    }
+
     fn is_root(&self) -> bool {
         self.0.is_root()
     }
 
     fn supports_action(&self) -> bool {
         self.0.default_action_verb().is_some()
     }
 
     fn supports_component(&self) -> bool {
         self.0.raw_bounds().is_some() || self.is_root()
     }
 
+    fn supports_text(&self) -> bool {
+        self.0.supports_text_ranges()
+    }
+
     fn supports_value(&self) -> bool {
         self.current_value().is_some()
     }
 
     pub(crate) fn interfaces(&self) -> InterfaceSet {
         let mut interfaces = InterfaceSet::new(Interface::Accessible);
         if self.supports_action() {
             interfaces.insert(Interface::Action);
         }
         if self.supports_component() {
             interfaces.insert(Interface::Component);
         }
+        if self.supports_text() {
+            interfaces.insert(Interface::Text);
+        }
         if self.supports_value() {
             interfaces.insert(Interface::Value);
         }
         interfaces
     }
 
     pub(crate) fn live(&self) -> AtspiLive {
@@ -412,30 +422,26 @@
     }
 
     fn raw_bounds_and_transform(&self) -> (Option<Rect>, Affine) {
         let state = self.0;
         (state.raw_bounds(), state.direct_transform())
     }
 
-    fn extents(&self, window_bounds: &WindowBounds) -> AtspiRect {
-        if self.is_root() {
-            return window_bounds.outer.into();
-        }
-        self.0.bounding_box().map_or_else(
-            || AtspiRect::INVALID,
-            |bounds| {
-                let window_top_left = window_bounds.inner.origin();
-                let node_origin = bounds.origin();
-                let new_origin = Point::new(
-                    window_top_left.x + node_origin.x,
-                    window_top_left.y + node_origin.y,
+    fn extents(&self, window_bounds: &WindowBounds, coord_type: CoordType) -> Option<Rect> {
+        self.is_root()
+            .then(|| window_bounds.inner.with_origin(Point::ZERO))
+            .or_else(|| self.0.bounding_box())
+            .map(|bounds| {
+                let new_origin = window_bounds.accesskit_point_to_atspi_point(
+                    bounds.origin(),
+                    self.0.filtered_parent(&filter),
+                    coord_type,
                 );
-                bounds.with_origin(new_origin).into()
-            },
-        )
+                bounds.with_origin(new_origin)
+            })
     }
 
     fn current_value(&self) -> Option<f64> {
         self.0.numeric_value()
     }
 
     pub(crate) fn notify_changes(
@@ -520,31 +526,30 @@
     fn notify_bounds_changes(
         &self,
         window_bounds: &WindowBounds,
         adapter: &Adapter,
         old: &NodeWrapper<'_>,
     ) {
         if self.raw_bounds_and_transform() != old.raw_bounds_and_transform() {
-            adapter.emit_object_event(
-                self.id(),
-                ObjectEvent::BoundsChanged(self.extents(window_bounds)),
-            );
+            if let Some(extents) = self.extents(window_bounds, CoordType::Window) {
+                adapter.emit_object_event(self.id(), ObjectEvent::BoundsChanged(extents.into()));
+            }
         }
     }
 
     fn notify_children_changes(&self, adapter: &Adapter, old: &NodeWrapper<'_>) {
-        let old_children = old.child_ids().collect::<Vec<NodeId>>();
-        let filtered_children = self.filtered_child_ids().collect::<Vec<NodeId>>();
-        for (index, child) in filtered_children.iter().enumerate() {
-            if !old_children.contains(child) {
+        let old_filtered_children = old.filtered_child_ids().collect::<Vec<NodeId>>();
+        let new_filtered_children = self.filtered_child_ids().collect::<Vec<NodeId>>();
+        for (index, child) in new_filtered_children.iter().enumerate() {
+            if !old_filtered_children.contains(child) {
                 adapter.emit_object_event(self.id(), ObjectEvent::ChildAdded(index, *child));
             }
         }
-        for child in old_children.into_iter() {
-            if !filtered_children.contains(&child) {
+        for child in old_filtered_children.into_iter() {
+            if !new_filtered_children.contains(&child) {
                 adapter.emit_object_event(self.id(), ObjectEvent::ChildRemoved(child));
             }
         }
     }
 }
 
 #[derive(Clone)]
@@ -603,21 +608,42 @@
                 f(node, context)
             } else {
                 Err(Error::Defunct)
             }
         })
     }
 
+    fn resolve_for_text_with_context<F, T>(&self, f: F) -> Result<T>
+    where
+        for<'a> F: FnOnce(Node<'a>, &Context) -> Result<T>,
+    {
+        self.resolve_with_context(|node, context| {
+            let wrapper = NodeWrapper(&node);
+            if wrapper.supports_text() {
+                f(node, context)
+            } else {
+                Err(Error::UnsupportedInterface)
+            }
+        })
+    }
+
     fn resolve<F, T>(&self, f: F) -> Result<T>
     where
         for<'a> F: FnOnce(Node<'a>) -> Result<T>,
     {
         self.resolve_with_context(|node, _| f(node))
     }
 
+    fn resolve_for_text<F, T>(&self, f: F) -> Result<T>
+    where
+        for<'a> F: FnOnce(Node<'a>) -> Result<T>,
+    {
+        self.resolve_for_text_with_context(|node, _| f(node))
+    }
+
     fn do_action_internal<F>(&self, f: F) -> Result<()>
     where
         F: FnOnce(&TreeState, &Context) -> ActionRequest,
     {
         let context = self.upgrade_context()?;
         let tree = context.read_tree();
         if tree.state().has_node(self.id) {
@@ -735,28 +761,42 @@
         self.resolve_with_context(|node, context| {
             let wrapper = NodeWrapper(&node);
             Ok(wrapper.state(context.read_tree().state().focus_id().is_some()))
         })
         .unwrap_or(State::Defunct.into())
     }
 
+    pub fn attributes(&self) -> Result<HashMap<&'static str, String>> {
+        self.resolve(|node| {
+            let wrapper = NodeWrapper(&node);
+            Ok(wrapper.attributes())
+        })
+    }
+
     pub fn supports_action(&self) -> Result<bool> {
         self.resolve(|node| {
             let wrapper = NodeWrapper(&node);
             Ok(wrapper.supports_action())
         })
     }
 
     pub fn supports_component(&self) -> Result<bool> {
         self.resolve(|node| {
             let wrapper = NodeWrapper(&node);
             Ok(wrapper.supports_component())
         })
     }
 
+    pub fn supports_text(&self) -> Result<bool> {
+        self.resolve(|node| {
+            let wrapper = NodeWrapper(&node);
+            Ok(wrapper.supports_text())
+        })
+    }
+
     pub fn supports_value(&self) -> Result<bool> {
         self.resolve(|node| {
             let wrapper = NodeWrapper(&node);
             Ok(wrapper.supports_value())
         })
     }
 
@@ -808,70 +848,48 @@
         })?;
         Ok(true)
     }
 
     pub fn contains(&self, x: i32, y: i32, coord_type: CoordType) -> Result<bool> {
         self.resolve_with_context(|node, context| {
             let window_bounds = context.read_root_window_bounds();
-            let bounds = match node.bounding_box() {
-                Some(node_bounds) => {
-                    let top_left = window_bounds.top_left(coord_type, node.is_root());
-                    let new_origin =
-                        Point::new(top_left.x + node_bounds.x0, top_left.y + node_bounds.y0);
-                    node_bounds.with_origin(new_origin)
-                }
-                None if node.is_root() => {
-                    let bounds = window_bounds.outer;
-                    match coord_type {
-                        CoordType::Screen => bounds,
-                        CoordType::Window => bounds.with_origin(Point::ZERO),
-                        _ => unimplemented!(),
-                    }
-                }
-                _ => return Err(Error::UnsupportedInterface),
-            };
-            Ok(bounds.contains(Point::new(x.into(), y.into())))
+            let wrapper = NodeWrapper(&node);
+            if let Some(extents) = wrapper.extents(&window_bounds, coord_type) {
+                Ok(extents.contains(Point::new(x.into(), y.into())))
+            } else {
+                Ok(false)
+            }
         })
     }
 
     pub fn accessible_at_point(
         &self,
         x: i32,
         y: i32,
         coord_type: CoordType,
     ) -> Result<Option<NodeId>> {
         self.resolve_with_context(|node, context| {
             let window_bounds = context.read_root_window_bounds();
-            let top_left = window_bounds.top_left(coord_type, node.is_root());
-            let point = Point::new(f64::from(x) - top_left.x, f64::from(y) - top_left.y);
+            let point = window_bounds.atspi_point_to_accesskit_point(
+                Point::new(x.into(), y.into()),
+                Some(node),
+                coord_type,
+            );
             let point = node.transform().inverse() * point;
             Ok(node.node_at_point(point, &filter).map(|node| node.id()))
         })
     }
 
     pub fn extents(&self, coord_type: CoordType) -> Result<AtspiRect> {
         self.resolve_with_context(|node, context| {
             let window_bounds = context.read_root_window_bounds();
-            match node.bounding_box() {
-                Some(node_bounds) => {
-                    let top_left = window_bounds.top_left(coord_type, node.is_root());
-                    let new_origin =
-                        Point::new(top_left.x + node_bounds.x0, top_left.y + node_bounds.y0);
-                    Ok(node_bounds.with_origin(new_origin).into())
-                }
-                None if node.is_root() => {
-                    let bounds = window_bounds.outer;
-                    Ok(match coord_type {
-                        CoordType::Screen => bounds.into(),
-                        CoordType::Window => bounds.with_origin(Point::ZERO).into(),
-                        _ => unimplemented!(),
-                    })
-                }
-                _ => Err(Error::UnsupportedInterface),
-            }
+            let wrapper = NodeWrapper(&node);
+            Ok(wrapper
+                .extents(&window_bounds, coord_type)
+                .map_or(AtspiRect::INVALID, AtspiRect::from))
         })
     }
 
     pub fn layer(&self) -> Result<Layer> {
         self.resolve(|node| {
             let wrapper = NodeWrapper(&node);
             if wrapper.role() == AtspiRole::Window {
@@ -888,28 +906,310 @@
             target: self.id,
             data: None,
         })?;
         Ok(true)
     }
 
     pub fn scroll_to_point(&self, coord_type: CoordType, x: i32, y: i32) -> Result<bool> {
-        self.do_action_internal(|tree_state, context| {
+        self.resolve_with_context(|node, context| {
             let window_bounds = context.read_root_window_bounds();
-            let is_root = self.id == tree_state.root_id();
-            let top_left = window_bounds.top_left(coord_type, is_root);
-            let point = Point::new(f64::from(x) - top_left.x, f64::from(y) - top_left.y);
-            ActionRequest {
+            let point = window_bounds.atspi_point_to_accesskit_point(
+                Point::new(x.into(), y.into()),
+                node.filtered_parent(&filter),
+                coord_type,
+            );
+            context.do_action(ActionRequest {
                 action: Action::ScrollToPoint,
                 target: self.id,
                 data: Some(ActionData::ScrollToPoint(point)),
-            }
+            });
+            Ok(())
         })?;
         Ok(true)
     }
 
+    pub fn character_count(&self) -> Result<i32> {
+        self.resolve_for_text(|node| {
+            node.document_range()
+                .end()
+                .to_global_usv_index()
+                .try_into()
+                .map_err(|_| Error::TooManyCharacters)
+        })
+    }
+
+    pub fn caret_offset(&self) -> Result<i32> {
+        self.resolve_for_text(|node| {
+            node.text_selection_focus().map_or(Ok(-1), |focus| {
+                focus
+                    .to_global_usv_index()
+                    .try_into()
+                    .map_err(|_| Error::TooManyCharacters)
+            })
+        })
+    }
+
+    pub fn string_at_offset(
+        &self,
+        offset: i32,
+        granularity: Granularity,
+    ) -> Result<(String, i32, i32)> {
+        self.resolve_for_text(|node| {
+            let range = text_range_from_offset(&node, offset, granularity)?;
+            let text = range.text();
+            let start = range
+                .start()
+                .to_global_usv_index()
+                .try_into()
+                .map_err(|_| Error::TooManyCharacters)?;
+            let end = range
+                .end()
+                .to_global_usv_index()
+                .try_into()
+                .map_err(|_| Error::TooManyCharacters)?;
+
+            Ok((text, start, end))
+        })
+    }
+
+    pub fn text(&self, start_offset: i32, end_offset: i32) -> Result<String> {
+        self.resolve_for_text(|node| {
+            let range = text_range_from_offsets(&node, start_offset, end_offset)
+                .ok_or(Error::IndexOutOfRange)?;
+            Ok(range.text())
+        })
+    }
+
+    pub fn set_caret_offset(&self, offset: i32) -> Result<bool> {
+        self.resolve_for_text_with_context(|node, context| {
+            let offset = text_position_from_offset(&node, offset).ok_or(Error::IndexOutOfRange)?;
+            context.do_action(ActionRequest {
+                action: Action::SetTextSelection,
+                target: node.id(),
+                data: Some(ActionData::SetTextSelection(
+                    offset.to_degenerate_range().to_text_selection(),
+                )),
+            });
+            Ok(true)
+        })
+    }
+
+    pub fn text_attribute_value(&self, _offset: i32, _attribute_name: &str) -> Result<String> {
+        // TODO: Implement rich text.
+        Err(Error::UnsupportedInterface)
+    }
+
+    pub fn text_attributes(&self, _offset: i32) -> Result<(HashMap<String, String>, i32, i32)> {
+        // TODO: Implement rich text.
+        Err(Error::UnsupportedInterface)
+    }
+
+    pub fn default_text_attributes(&self) -> Result<HashMap<String, String>> {
+        // TODO: Implement rich text.
+        Err(Error::UnsupportedInterface)
+    }
+
+    pub fn character_extents(&self, offset: i32, coord_type: CoordType) -> Result<AtspiRect> {
+        self.resolve_for_text_with_context(|node, context| {
+            let range = text_range_from_offset(&node, offset, Granularity::Char)?;
+            if let Some(bounds) = range.bounding_boxes().first() {
+                let window_bounds = context.read_root_window_bounds();
+                let new_origin = window_bounds.accesskit_point_to_atspi_point(
+                    bounds.origin(),
+                    Some(node),
+                    coord_type,
+                );
+                Ok(bounds.with_origin(new_origin).into())
+            } else {
+                Ok(AtspiRect::INVALID)
+            }
+        })
+    }
+
+    pub fn offset_at_point(&self, x: i32, y: i32, coord_type: CoordType) -> Result<i32> {
+        self.resolve_for_text_with_context(|node, context| {
+            let window_bounds = context.read_root_window_bounds();
+            let point = window_bounds.atspi_point_to_accesskit_point(
+                Point::new(x.into(), y.into()),
+                Some(node),
+                coord_type,
+            );
+            let point = node.transform().inverse() * point;
+            node.text_position_at_point(point)
+                .to_global_usv_index()
+                .try_into()
+                .map_err(|_| Error::TooManyCharacters)
+        })
+    }
+
+    pub fn n_selections(&self) -> Result<i32> {
+        self.resolve_for_text(|node| {
+            match node.text_selection().filter(|range| !range.is_degenerate()) {
+                Some(_) => Ok(1),
+                None => Ok(0),
+            }
+        })
+    }
+
+    pub fn selection(&self, selection_num: i32) -> Result<(i32, i32)> {
+        if selection_num != 0 {
+            return Ok((-1, -1));
+        }
+
+        self.resolve_for_text(|node| {
+            node.text_selection()
+                .filter(|range| !range.is_degenerate())
+                .map_or(Ok((-1, -1)), |range| {
+                    let start = range
+                        .start()
+                        .to_global_usv_index()
+                        .try_into()
+                        .map_err(|_| Error::TooManyCharacters)?;
+                    let end = range
+                        .end()
+                        .to_global_usv_index()
+                        .try_into()
+                        .map_err(|_| Error::TooManyCharacters)?;
+
+                    Ok((start, end))
+                })
+        })
+    }
+
+    pub fn add_selection(&self, start_offset: i32, end_offset: i32) -> Result<bool> {
+        // We only support one selection.
+        self.set_selection(0, start_offset, end_offset)
+    }
+
+    pub fn remove_selection(&self, selection_num: i32) -> Result<bool> {
+        if selection_num != 0 {
+            return Ok(false);
+        }
+
+        self.resolve_for_text_with_context(|node, context| {
+            // Simply collapse the selection to the position of the caret if a caret is
+            // visible, otherwise set the selection to 0.
+            let selection_end = node
+                .text_selection_focus()
+                .unwrap_or_else(|| node.document_range().start());
+            context.do_action(ActionRequest {
+                action: Action::SetTextSelection,
+                target: node.id(),
+                data: Some(ActionData::SetTextSelection(
+                    selection_end.to_degenerate_range().to_text_selection(),
+                )),
+            });
+            Ok(true)
+        })
+    }
+
+    pub fn set_selection(
+        &self,
+        selection_num: i32,
+        start_offset: i32,
+        end_offset: i32,
+    ) -> Result<bool> {
+        if selection_num != 0 {
+            return Ok(false);
+        }
+
+        self.resolve_for_text_with_context(|node, context| {
+            let range = text_range_from_offsets(&node, start_offset, end_offset)
+                .ok_or(Error::IndexOutOfRange)?;
+            context.do_action(ActionRequest {
+                action: Action::SetTextSelection,
+                target: node.id(),
+                data: Some(ActionData::SetTextSelection(range.to_text_selection())),
+            });
+            Ok(true)
+        })
+    }
+
+    pub fn range_extents(
+        &self,
+        start_offset: i32,
+        end_offset: i32,
+        coord_type: CoordType,
+    ) -> Result<AtspiRect> {
+        self.resolve_for_text_with_context(|node, context| {
+            if let Some(rect) = text_range_bounds_from_offsets(&node, start_offset, end_offset) {
+                let window_bounds = context.read_root_window_bounds();
+                let new_origin = window_bounds.accesskit_point_to_atspi_point(
+                    rect.origin(),
+                    Some(node),
+                    coord_type,
+                );
+                Ok(rect.with_origin(new_origin).into())
+            } else {
+                Ok(AtspiRect::INVALID)
+            }
+        })
+    }
+
+    pub fn text_attribute_run(
+        &self,
+        _offset: i32,
+        _include_defaults: bool,
+    ) -> Result<(HashMap<String, String>, i32, i32)> {
+        // TODO: Implement rich text.
+        // For now, just report a range spanning the entire text with no attributes,
+        // this is required by Orca to announce selection content and caret movements.
+        let character_count = self.character_count()?;
+        Ok((HashMap::new(), 0, character_count))
+    }
+
+    pub fn scroll_substring_to(
+        &self,
+        start_offset: i32,
+        end_offset: i32,
+        _: ScrollType,
+    ) -> Result<bool> {
+        self.resolve_for_text_with_context(|node, context| {
+            if let Some(rect) = text_range_bounds_from_offsets(&node, start_offset, end_offset) {
+                context.do_action(ActionRequest {
+                    action: Action::ScrollIntoView,
+                    target: node.id(),
+                    data: Some(ActionData::ScrollTargetRect(rect)),
+                });
+                Ok(true)
+            } else {
+                Ok(false)
+            }
+        })
+    }
+
+    pub fn scroll_substring_to_point(
+        &self,
+        start_offset: i32,
+        end_offset: i32,
+        coord_type: CoordType,
+        x: i32,
+        y: i32,
+    ) -> Result<bool> {
+        self.resolve_for_text_with_context(|node, context| {
+            let window_bounds = context.read_root_window_bounds();
+            let target_point = window_bounds.atspi_point_to_accesskit_point(
+                Point::new(x.into(), y.into()),
+                Some(node),
+                coord_type,
+            );
+
+            if let Some(rect) = text_range_bounds_from_offsets(&node, start_offset, end_offset) {
+                let point = Point::new(target_point.x - rect.x0, target_point.y - rect.y0);
+                context.do_action(ActionRequest {
+                    action: Action::ScrollToPoint,
+                    target: node.id(),
+                    data: Some(ActionData::ScrollToPoint(point)),
+                });
+                return Ok(true);
+            }
+            Ok(false)
+        })
+    }
+
     pub fn minimum_value(&self) -> Result<f64> {
         self.resolve(|node| Ok(node.min_numeric_value().unwrap_or(f64::MIN)))
     }
 
     pub fn maximum_value(&self) -> Result<f64> {
         self.resolve(|node| Ok(node.max_numeric_value().unwrap_or(f64::MAX)))
     }
```

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/rect.rs` & `accesskit-0.3.3/platforms/atspi-common/src/rect.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/platforms/atspi-common/src/simplified.rs` & `accesskit-0.3.3/platforms/atspi-common/src/simplified.rs`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 //! API that corresponds more closely to the libatspi client API,
 //! intended to be used by bindings to languages with less rich
 //! type systems.
 
+use std::collections::HashMap;
+
 use crate::{
     Adapter, Event as EventEnum, NodeIdOrRoot, ObjectEvent, PlatformNode, PlatformRoot, Property,
     WindowEvent,
 };
 
-pub use crate::{CoordType, Error, Layer, Rect, Result, Role, StateSet};
+pub use crate::{CoordType, Error, Granularity, Layer, Rect, Result, Role, ScrollType, StateSet};
 
 #[derive(Clone, Hash, PartialEq)]
 pub enum Accessible {
     Node(PlatformNode),
     Root(PlatformRoot),
 }
 
@@ -52,14 +54,21 @@
     pub fn state(&self) -> StateSet {
         match self {
             Self::Node(node) => node.state(),
             Self::Root(_) => StateSet::empty(),
         }
     }
 
+    pub fn attributes(&self) -> Result<HashMap<&'static str, String>> {
+        match self {
+            Self::Node(node) => node.attributes(),
+            Self::Root(_) => Ok(HashMap::new()),
+        }
+    }
+
     pub fn parent(&self) -> Result<Option<Self>> {
         match self {
             Self::Node(node) => match node.parent()? {
                 NodeIdOrRoot::Node(id) => Ok(Some(Self::Node(node.relative(id)))),
                 NodeIdOrRoot::Root => node.root().map(|root| Some(Self::Root(root))),
             },
             Self::Root(_) => Ok(None),
@@ -202,14 +211,186 @@
     pub fn scroll_to_point(&self, coord_type: CoordType, x: i32, y: i32) -> Result<bool> {
         match self {
             Self::Node(node) => node.scroll_to_point(coord_type, x, y),
             Self::Root(_) => Err(Error::UnsupportedInterface),
         }
     }
 
+    pub fn supports_text(&self) -> Result<bool> {
+        match self {
+            Self::Node(node) => node.supports_text(),
+            Self::Root(_) => Ok(false),
+        }
+    }
+
+    pub fn character_count(&self) -> Result<i32> {
+        match self {
+            Self::Node(node) => node.character_count(),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn caret_offset(&self) -> Result<i32> {
+        match self {
+            Self::Node(node) => node.caret_offset(),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn string_at_offset(
+        &self,
+        offset: i32,
+        granularity: Granularity,
+    ) -> Result<(String, i32, i32)> {
+        match self {
+            Self::Node(node) => node.string_at_offset(offset, granularity),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn text(&self, start_offset: i32, end_offset: i32) -> Result<String> {
+        match self {
+            Self::Node(node) => node.text(start_offset, end_offset),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn set_caret_offset(&self, offset: i32) -> Result<bool> {
+        match self {
+            Self::Node(node) => node.set_caret_offset(offset),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn text_attribute_value(&self, offset: i32, attribute_name: &str) -> Result<String> {
+        match self {
+            Self::Node(node) => node.text_attribute_value(offset, attribute_name),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn text_attributes(&self, offset: i32) -> Result<(HashMap<String, String>, i32, i32)> {
+        match self {
+            Self::Node(node) => node.text_attributes(offset),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn default_text_attributes(&self) -> Result<HashMap<String, String>> {
+        match self {
+            Self::Node(node) => node.default_text_attributes(),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn character_extents(&self, offset: i32, coord_type: CoordType) -> Result<Rect> {
+        match self {
+            Self::Node(node) => node.character_extents(offset, coord_type),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn offset_at_point(&self, x: i32, y: i32, coord_type: CoordType) -> Result<i32> {
+        match self {
+            Self::Node(node) => node.offset_at_point(x, y, coord_type),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn n_selections(&self) -> Result<i32> {
+        match self {
+            Self::Node(node) => node.n_selections(),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn selection(&self, selection_num: i32) -> Result<(i32, i32)> {
+        match self {
+            Self::Node(node) => node.selection(selection_num),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn add_selection(&self, start_offset: i32, end_offset: i32) -> Result<bool> {
+        match self {
+            Self::Node(node) => node.add_selection(start_offset, end_offset),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn remove_selection(&self, selection_num: i32) -> Result<bool> {
+        match self {
+            Self::Node(node) => node.remove_selection(selection_num),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn set_selection(
+        &self,
+        selection_num: i32,
+        start_offset: i32,
+        end_offset: i32,
+    ) -> Result<bool> {
+        match self {
+            Self::Node(node) => node.set_selection(selection_num, start_offset, end_offset),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn range_extents(
+        &self,
+        start_offset: i32,
+        end_offset: i32,
+        coord_type: CoordType,
+    ) -> Result<Rect> {
+        match self {
+            Self::Node(node) => node.range_extents(start_offset, end_offset, coord_type),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn text_attribute_run(
+        &self,
+        offset: i32,
+        include_defaults: bool,
+    ) -> Result<(HashMap<String, String>, i32, i32)> {
+        match self {
+            Self::Node(node) => node.text_attribute_run(offset, include_defaults),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn scroll_substring_to(
+        &self,
+        start_offset: i32,
+        end_offset: i32,
+        scroll_type: ScrollType,
+    ) -> Result<bool> {
+        match self {
+            Self::Node(node) => node.scroll_substring_to(start_offset, end_offset, scroll_type),
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
+    pub fn scroll_substring_to_point(
+        &self,
+        start_offset: i32,
+        end_offset: i32,
+        coord_type: CoordType,
+        x: i32,
+        y: i32,
+    ) -> Result<bool> {
+        match self {
+            Self::Node(node) => {
+                node.scroll_substring_to_point(start_offset, end_offset, coord_type, x, y)
+            }
+            Self::Root(_) => Err(Error::UnsupportedInterface),
+        }
+    }
+
     pub fn supports_value(&self) -> Result<bool> {
         match self {
             Self::Node(node) => node.supports_value(),
             Self::Root(_) => Ok(false),
         }
     }
 
@@ -296,14 +477,21 @@
                     ObjectEvent::BoundsChanged(bounds) => Self {
                         kind: "object:bounds-changed".into(),
                         source,
                         detail1: 0,
                         detail2: 0,
                         data: Some(EventData::Rect(bounds)),
                     },
+                    ObjectEvent::CaretMoved(offset) => Self {
+                        kind: "object:text-caret-moved".into(),
+                        source,
+                        detail1: offset,
+                        detail2: 0,
+                        data: None,
+                    },
                     ObjectEvent::ChildAdded(index, child) => {
                         let child = Accessible::Node(adapter.platform_node(child));
                         Self {
                             kind: "object:children-changed:add".into(),
                             source,
                             detail1: index as i32,
                             detail2: 0,
@@ -353,14 +541,43 @@
                     ObjectEvent::StateChanged(state, value) => Self {
                         kind: format!("object:state-changed:{}", String::from(state)),
                         source,
                         detail1: value as i32,
                         detail2: 0,
                         data: None,
                     },
+                    ObjectEvent::TextInserted {
+                        start_index,
+                        length,
+                        content,
+                    } => Self {
+                        kind: "object:text-changed:insert".into(),
+                        source,
+                        detail1: start_index,
+                        detail2: length,
+                        data: Some(EventData::String(content)),
+                    },
+                    ObjectEvent::TextRemoved {
+                        start_index,
+                        length,
+                        content,
+                    } => Self {
+                        kind: "object:text-changed:delete".into(),
+                        source,
+                        detail1: start_index,
+                        detail2: length,
+                        data: Some(EventData::String(content)),
+                    },
+                    ObjectEvent::TextSelectionChanged => Self {
+                        kind: "object:text-selection-changed".into(),
+                        source,
+                        detail1: 0,
+                        detail2: 0,
+                        data: None,
+                    },
                 }
             }
             EventEnum::Window {
                 target,
                 name,
                 event,
             } => {
```

### Comparing `accesskit-0.3.2/bindings/python/Cargo.toml` & `accesskit-0.3.3/bindings/python/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_python"
-version = "0.3.2"
+version = "0.3.3"
 authors.workspace = true
 license.workspace = true
 description = "Python bindings to the AccessKit library"
 readme = "README.md"
 publish = false
 edition.workspace = true
 
@@ -17,14 +17,14 @@
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common", features = ["pyo3"] }
 pyo3 = { version = "0.20", features = ["abi3-py38", "multiple-pymethods"] }
 
 [target.'cfg(target_os = "windows")'.dependencies]
-accesskit_windows = { version = "0.18.2", path = "../../platforms/windows" }
+accesskit_windows = { version = "0.19.0", path = "../../platforms/windows" }
 
 [target.'cfg(target_os = "macos")'.dependencies]
-accesskit_macos = { version = "0.13.2", path = "../../platforms/macos" }
+accesskit_macos = { version = "0.14.0", path = "../../platforms/macos" }
 
 [target.'cfg(any(target_os = "linux", target_os = "dragonfly", target_os = "freebsd", target_os = "openbsd", target_os = "netbsd"))'.dependencies]
-accesskit_unix = { version = "0.9.2", path = "../../platforms/unix" }
+accesskit_unix = { version = "0.10.0", path = "../../platforms/unix" }
```

### Comparing `accesskit-0.3.2/bindings/python/CHANGELOG.md` & `accesskit-0.3.3/bindings/python/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_windows bumped from 0.18.1 to 0.18.2
     * accesskit_macos bumped from 0.13.1 to 0.13.2
     * accesskit_unix bumped from 0.9.1 to 0.9.2
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_windows bumped from 0.18.2 to 0.19.0
+    * accesskit_macos bumped from 0.13.2 to 0.14.0
+    * accesskit_unix bumped from 0.9.2 to 0.10.0
+
 ## [0.3.1](https://github.com/AccessKit/accesskit/compare/accesskit_python-v0.3.0...accesskit_python-v0.3.1) (2024-05-11)
 
 
 ### Bug Fixes
 
 * Fix dead code warning on Unix platforms ([#403](https://github.com/AccessKit/accesskit/issues/403)) ([09d9157](https://github.com/AccessKit/accesskit/commit/09d91577dd88743e379a1fdea34b25a94726d0fb))
```

### Comparing `accesskit-0.3.2/bindings/python/README.md` & `accesskit-0.3.3/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/examples/pygame/.gitignore` & `accesskit-0.3.3/bindings/python/examples/pygame/.gitignore`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/examples/pygame/hello_world.py` & `accesskit-0.3.3/bindings/python/examples/pygame/hello_world.py`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/src/common.rs` & `accesskit-0.3.3/bindings/python/src/common.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/src/geometry.rs` & `accesskit-0.3.3/bindings/python/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/src/lib.rs` & `accesskit-0.3.3/bindings/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/src/macos.rs` & `accesskit-0.3.3/bindings/python/src/macos.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/src/unix.rs` & `accesskit-0.3.3/bindings/python/src/unix.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/bindings/python/src/windows.rs` & `accesskit-0.3.3/bindings/python/src/windows.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/Cargo.lock` & `accesskit-0.3.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -26,69 +26,69 @@
  "pyo3",
  "schemars",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_atspi_common"
-version = "0.4.2"
+version = "0.5.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "atspi-common",
  "serde",
  "thiserror",
  "zvariant",
 ]
 
 [[package]]
 name = "accesskit_c"
-version = "0.10.1"
+version = "0.10.2"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "paste",
 ]
 
 [[package]]
 name = "accesskit_consumer"
-version = "0.20.0"
+version = "0.21.0"
 dependencies = [
  "accesskit",
  "immutable-chunkmap",
 ]
 
 [[package]]
 name = "accesskit_macos"
-version = "0.13.2"
+version = "0.14.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "objc2",
  "objc2-app-kit",
  "objc2-foundation",
  "once_cell",
 ]
 
 [[package]]
 name = "accesskit_python"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "pyo3",
 ]
 
 [[package]]
 name = "accesskit_unix"
-version = "0.9.2"
+version = "0.10.0"
 dependencies = [
  "accesskit",
  "accesskit_atspi_common",
  "async-channel 2.1.1",
  "async-executor",
  "async-task",
  "atspi",
@@ -98,29 +98,29 @@
  "tokio",
  "tokio-stream",
  "zbus",
 ]
 
 [[package]]
 name = "accesskit_windows"
-version = "0.18.2"
+version = "0.19.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "once_cell",
  "paste",
  "scopeguard",
  "static_assertions",
  "windows",
  "winit",
 ]
 
 [[package]]
 name = "accesskit_winit"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
@@ -428,26 +428,14 @@
 [[package]]
 name = "bitflags"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
 
 [[package]]
-name = "bitvec"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
-dependencies = [
- "funty",
- "radium",
- "tap",
- "wyz",
-]
-
-[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
@@ -839,20 +827,14 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
 
 [[package]]
-name = "funty"
-version = "2.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
-
-[[package]]
 name = "futures-core"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
 
 [[package]]
 name = "futures-io"
@@ -974,21 +956,19 @@
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "immutable-chunkmap"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374b75d1b5a9df2c4d9392f21a9e821113543ffc49571b3428d8e161802f8cc7"
+checksum = "4419f022e55cc63d5bbd6b44b71e1d226b9c9480a47824c706e9d54e5c40c5eb"
 dependencies = [
  "arrayvec",
- "packed_struct",
- "packed_struct_codegen",
 ]
 
 [[package]]
 name = "indexmap"
 version = "1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
@@ -1369,35 +1349,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e25e9fb15717794fae58ab55c26e044103aad13186fbb625893f9a3bbcc24228"
 dependencies = [
  "ttf-parser",
 ]
 
 [[package]]
-name = "packed_struct"
-version = "0.10.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36b29691432cc9eff8b282278473b63df73bea49bc3ec5e67f31a3ae9c3ec190"
-dependencies = [
- "bitvec",
- "packed_struct_codegen",
-]
-
-[[package]]
-name = "packed_struct_codegen"
-version = "0.10.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cd6706dfe50d53e0f6aa09e12c034c44faacd23e966ae5a209e8bdb8f179f98"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "parking"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
 
 [[package]]
 name = "parking_lot"
@@ -1604,20 +1563,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
-name = "radium"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
-
-[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
@@ -1993,20 +1946,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "tap"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
-
-[[package]]
 name = "target-lexicon"
 version = "0.12.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
 
 [[package]]
 name = "tempfile"
@@ -2771,23 +2718,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "wyz"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
-dependencies = [
- "tap",
-]
-
-[[package]]
 name = "x11-dl"
 version = "2.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38735924fedd5314a6e548792904ed8c6de6636285cb9fec04d5b1db85c1516f"
 dependencies = [
  "libc",
  "once_cell",
```

### Comparing `accesskit-0.3.2/pyproject.toml` & `accesskit-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/LICENSE-APACHE` & `accesskit-0.3.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/LICENSE-MIT` & `accesskit-0.3.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/LICENSE.chromium` & `accesskit-0.3.3/LICENSE.chromium`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.2/PKG-INFO` & `accesskit-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: accesskit
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

