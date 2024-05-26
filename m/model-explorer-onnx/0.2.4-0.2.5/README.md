# Comparing `tmp/model_explorer_onnx-0.2.4.tar.gz` & `tmp/model_explorer_onnx-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.2.4.tar", last modified: Wed May 22 03:00:19 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.2.5.tar", last modified: Sun May 26 18:44:35 2024, max compression
```

## Comparing `model_explorer_onnx-0.2.4.tar` & `model_explorer_onnx-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.288561 model_explorer_onnx-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/src/model_explorer_onnx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/src/model_explorer_onnx/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx/bin/onnxvis.py
--rw-r--r--   0 runner    (1001) docker     (127)    22798 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:44:35.190188 model_explorer_onnx-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 18:44:31.000000 model_explorer_onnx-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-26 18:44:35.190188 model_explorer_onnx-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-26 18:44:31.000000 model_explorer_onnx-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-26 18:44:31.000000 model_explorer_onnx-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:44:35.190188 model_explorer_onnx-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:44:35.186188 model_explorer_onnx-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:44:35.186188 model_explorer_onnx-0.2.5/src/model_explorer_onnx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:44:35.190188 model_explorer_onnx-0.2.5/src/model_explorer_onnx/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 18:44:31.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 18:44:31.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx/bin/onnxvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22968 2024-05-26 18:44:31.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:44:35.190188 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-26 18:44:35.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-26 18:44:35.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:44:35.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-26 18:44:35.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 18:44:35.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 18:44:35.000000 model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.2.4/LICENSE` & `model_explorer_onnx-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.2.4/PKG-INFO` & `model_explorer_onnx-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.4
+Version: 0.2.5
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Requires-Dist: numpy
 Requires-Dist: onnx
 Requires-Dist: onnxscript>=0.1.0.dev20240517
 Requires-Dist: ml_dtypes
 
 # Model Explorer ONNX Adapter
 
-[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx)
+[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx) [![PyPI - Downloads](https://img.shields.io/pypi/dm/model-explorer-onnx)](https://pypi.org/project/model-explorer-onnx) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ONNX Adapter for [google-ai-edge/model-explorer](https://github.com/google-ai-edge/model-explorer)
 
 ## Installation
 
 ```bash
 pip install --upgrade model-explorer-onnx
@@ -46,18 +46,27 @@
 # Or as a shortcut
 onnxvis
 
 # Supply model path
 onnxvis model.onnx
 ```
 
+> [!NOTE]
+> Model Explorer only supports WSL on Windows.
+
+Read more on the [Model Explorer User Guide](https://github.com/google-ai-edge/model-explorer/wiki/2.-User-Guide).
+
 ## Notes on representation
 
 Graph input/output/initializers in ONNX are values (edges), not nodes. A node is displayed here for visualization. Graph inputs that are initialized by initializers are displayed as `InitializedInput`, and are displayed closer to nodes that use them.
 
+## Color Themes
+
+Get node color themes [here](./themes)
+
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

### Comparing `model_explorer_onnx-0.2.4/README.md` & `model_explorer_onnx-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Model Explorer ONNX Adapter
 
-[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx)
+[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx) [![PyPI - Downloads](https://img.shields.io/pypi/dm/model-explorer-onnx)](https://pypi.org/project/model-explorer-onnx) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ONNX Adapter for [google-ai-edge/model-explorer](https://github.com/google-ai-edge/model-explorer)
 
 ## Installation
 
 ```bash
 pip install --upgrade model-explorer-onnx
@@ -18,18 +18,27 @@
 # Or as a shortcut
 onnxvis
 
 # Supply model path
 onnxvis model.onnx
 ```
 
+> [!NOTE]
+> Model Explorer only supports WSL on Windows.
+
+Read more on the [Model Explorer User Guide](https://github.com/google-ai-edge/model-explorer/wiki/2.-User-Guide).
+
 ## Notes on representation
 
 Graph input/output/initializers in ONNX are values (edges), not nodes. A node is displayed here for visualization. Graph inputs that are initialized by initializers are displayed as `InitializedInput`, and are displayed closer to nodes that use them.
 
+## Color Themes
+
+Get node color themes [here](./themes)
+
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

### Comparing `model_explorer_onnx-0.2.4/pyproject.toml` & `model_explorer_onnx-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.2.4"
+version = "0.2.5"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["onnx", "model-explorer", "visualization"]
 classifiers = [
```

### Comparing `model_explorer_onnx-0.2.4/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.2.5/src/model_explorer_onnx/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,19 @@
 def set_type_shape_metadata(
     metadata: graph_builder.MetadataItem, value: ir.Value | ir.TensorProtocol
 ) -> None:
     # tensor_shape is a special key that is used to display the type and shape of the tensor
     set_attr(metadata, "tensor_shape", format_tensor_shape(value))
 
 
+def set_metadata_props(metadata: graph_builder.MetadataItem, value: ir.Value) -> None:
+    for prop_key, prop_value in value.metadata_props.items():
+        set_attr(metadata, f"[metadata] {prop_key}", prop_value)
+
+
 def add_inputs_metadata(
     onnx_node: ir.Node, node: graph_builder.GraphNode, opset_version: int
 ) -> None:
     if onnx.defs.has(onnx_node.op_type, max_inclusive_version=opset_version):
         schema = onnx.defs.get_schema(
             onnx_node.op_type, max_inclusive_version=opset_version
         )
@@ -170,16 +175,15 @@
     for i, input_value in enumerate(onnx_node.inputs):
         metadata = graph_builder.MetadataItem(id=str(i), attrs=[])
         if input_value is None:
             set_attr(metadata, "__tensor_tag", "None")
         else:
             set_attr(metadata, "__tensor_tag", input_value.name or "None")
             set_type_shape_metadata(metadata, input_value)
-            for prop_key, prop_value in input_value.metadata_props.items():
-                set_attr(metadata, f"[metadata] {prop_key}", prop_value)
+            set_metadata_props(metadata, input_value)
         if schema is not None:
             if (param_name := get_node_input_param_name(schema, i)) is not None:
                 set_attr(metadata, "param_name", param_name)
         node.inputsMetadata.append(metadata)
 
 
 def add_outputs_metadata(
@@ -191,16 +195,15 @@
         )
     else:
         schema = None
     for output_value in onnx_node.outputs:
         metadata = graph_builder.MetadataItem(id=str(output_value.index()), attrs=[])
         set_attr(metadata, "__tensor_tag", output_value.name or "None")
         set_type_shape_metadata(metadata, output_value)
-        for prop_key, prop_value in output_value.metadata_props.items():
-            set_attr(metadata, f"[metadata] {prop_key}", prop_value)
+        set_metadata_props(metadata, output_value)
         if len(output_value.uses()) == 0 and not output_value.is_graph_output():
             # The output is unused. Add a flag to indicate that.
             set_attr(metadata, "unused", "True")
         if schema is not None:
             output_index = output_value.index()
             assert output_index is not None
             if (
@@ -295,20 +298,29 @@
 
 def create_op_label(domain: str, op_type: str) -> str:
     if domain in {"", "ai.onnx"}:
         return op_type
     return f"{domain}::{op_type}"
 
 
-def parse_namespace(node_name: str) -> list[str]:
+def _parse_namespace(node_name: str) -> list[str]:
     """Parse the namespace from the node name if it is in the format of /namespace/node_name."""
     split = node_name.lstrip("/").rstrip("/").split("/")[0:-1]
     return [ns or "<anonymous>" for ns in split]
 
 
+def get_node_namespace(node: ir.Node) -> list[str]:
+    """Get the namespace from the node."""
+    if (metadata_namespace := node.metadata_props.get("namespace")) is not None:
+        return _parse_namespace(metadata_namespace)
+    if node.name:
+        return _parse_namespace(node.name)
+    return []
+
+
 def create_node(
     onnx_node: ir.Node,
     graph_inputs: set[ir.Value],
     namespace: str,
     all_function_ids: set[ir.OperatorIdentifier],
     opset_version: int,
     settings: Settings,
@@ -324,15 +336,15 @@
     """
     assert onnx_node.name, "Bug: Node name is required"
 
     if onnx_node.op_type == "Constant":
         # Move the constant closer to the user node's namespace
         namespace = get_constant_namespace(onnx_node.outputs[0], namespace)
     else:
-        embedded_namespace = parse_namespace(onnx_node.name)
+        embedded_namespace = get_node_namespace(onnx_node)
         if embedded_namespace:
             namespace = namespace + "/" + "/".join(embedded_namespace)
     node = graph_builder.GraphNode(
         id=onnx_node.name,
         label=create_op_label(onnx_node.domain, onnx_node.op_type),
         namespace=namespace,
     )
@@ -366,14 +378,15 @@
                     targetNodeInputId="0",
                 )
             )
         if type_ == "Input":
             metadata = graph_builder.MetadataItem(id="0", attrs=[])
             set_attr(metadata, "__tensor_tag", value.name or "")
             set_type_shape_metadata(metadata, value)
+            set_metadata_props(metadata, value)
             node.outputsMetadata.append(metadata)
         set_attr(node, "name", value.name or "")
         set_attr(node, "index", str(i))
         graph.nodes.append(node)
         # Record nodes for quick lookup
         all_nodes[node.id] = node
 
@@ -387,30 +400,24 @@
     user_nodes = tuple(set(node for node, _ in initializer.uses()))
     if not user_nodes:
         # The initializer is not used by any node. Keep it in the root namespace.
         return initializer_namespace
     if len(user_nodes) == 1:
         # If the initializer is used by a single node, move it to the same namespace as the node
         user_node = user_nodes[0]
-        assert (
-            user_node.name
-        ), "Bug: Node name is required and should have been assigned"
-        user_node_namespace = parse_namespace(user_node.name)
+        user_node_namespace = get_node_namespace(user_node)
         if user_node_namespace:
             initializer_namespace = (
                 initializer_namespace + "/" + "/".join(user_node_namespace)
             )
     else:
         # If there are multiple user nodes, find the common namespace
-        common_namespace = parse_namespace(user_nodes[0].name)  # type: ignore
+        common_namespace = get_node_namespace(user_nodes[0])
         for user_node in user_nodes:
-            assert (
-                user_node.name
-            ), "Bug: Node name is required and should have been assigned"
-            user_node_namespace = parse_namespace(user_node.name)
+            user_node_namespace = get_node_namespace(user_node)
             for i, (name_a, name_b) in enumerate(
                 zip(common_namespace, user_node_namespace)
             ):
                 if name_a != name_b:
                     # That's the end of the common namespace
                     common_namespace = common_namespace[:i]
                     break
@@ -473,14 +480,15 @@
             assert initializer.const_value is not None
             set_attr(
                 node,
                 "__value",
                 display_tensor_json(initializer.const_value, settings=settings),
             )
         set_attr(metadata, "value", display_tensor_repr(initializer.const_value))
+        set_metadata_props(metadata, initializer)
         # Note if the initializer is unused
         if not initializer.uses():
             set_attr(metadata, "unused", "True")
         node.outputsMetadata.append(metadata)
         graph.nodes.append(node)
```

### Comparing `model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.2.5/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.4
+Version: 0.2.5
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Requires-Dist: numpy
 Requires-Dist: onnx
 Requires-Dist: onnxscript>=0.1.0.dev20240517
 Requires-Dist: ml_dtypes
 
 # Model Explorer ONNX Adapter
 
-[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx)
+[![PyPI - Version](https://img.shields.io/pypi/v/model-explorer-onnx.svg)](https://pypi.org/project/model-explorer-onnx) [![PyPI - Downloads](https://img.shields.io/pypi/dm/model-explorer-onnx)](https://pypi.org/project/model-explorer-onnx) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ONNX Adapter for [google-ai-edge/model-explorer](https://github.com/google-ai-edge/model-explorer)
 
 ## Installation
 
 ```bash
 pip install --upgrade model-explorer-onnx
@@ -46,18 +46,27 @@
 # Or as a shortcut
 onnxvis
 
 # Supply model path
 onnxvis model.onnx
 ```
 
+> [!NOTE]
+> Model Explorer only supports WSL on Windows.
+
+Read more on the [Model Explorer User Guide](https://github.com/google-ai-edge/model-explorer/wiki/2.-User-Guide).
+
 ## Notes on representation
 
 Graph input/output/initializers in ONNX are values (edges), not nodes. A node is displayed here for visualization. Graph inputs that are initialized by initializers are displayed as `InitializedInput`, and are displayed closer to nodes that use them.
 
+## Color Themes
+
+Get node color themes [here](./themes)
+
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

