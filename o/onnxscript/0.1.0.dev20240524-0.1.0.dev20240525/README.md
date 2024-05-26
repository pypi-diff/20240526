# Comparing `tmp/onnxscript-0.1.0.dev20240524.tar.gz` & `tmp/onnxscript-0.1.0.dev20240525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240524.tar", last modified: Fri May 24 00:01:25 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240525.tar", last modified: Sat May 25 00:00:57 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240524.tar` & `onnxscript-0.1.0.dev20240525.tar`

### file list

```diff
@@ -1,222 +1,223 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.146366 onnxscript-0.1.0.dev20240524/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-24 00:01:25.146366 onnxscript-0.1.0.dev20240524/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.106366 onnxscript-0.1.0.dev20240524/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.106366 onnxscript-0.1.0.dev20240524/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.106366 onnxscript-0.1.0.dev20240524/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36693 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.106366 onnxscript-0.1.0.dev20240524/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.110366 onnxscript-0.1.0.dev20240524/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.098366 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.110366 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.122366 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.098366 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.098366 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.122366 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.126366 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.126366 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27429 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.126366 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   291013 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.130366 onnxscript-0.1.0.dev20240524/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2750 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10936 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94051 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2962 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20997 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/_type_casting.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.130366 onnxscript-0.1.0.dev20240524/onnxscript/ir/passes/
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/passes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8468 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/passes/_pass_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    59696 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19877 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.130366 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.138366 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.138366 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4393 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2114 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.142366 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1516 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1517 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7351 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26504 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.142366 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2154 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.142366 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/bfloat16_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5499 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.142366 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1674 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29584 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44529 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.142366 onnxscript-0.1.0.dev20240524/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.146366 onnxscript-0.1.0.dev20240524/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-24 00:01:25.146366 onnxscript-0.1.0.dev20240524/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-24 00:01:25.000000 onnxscript-0.1.0.dev20240524/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8302 2024-05-24 00:01:25.000000 onnxscript-0.1.0.dev20240524/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-24 00:01:25.000000 onnxscript-0.1.0.dev20240524/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-24 00:01:25.000000 onnxscript-0.1.0.dev20240524/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-24 00:01:25.000000 onnxscript-0.1.0.dev20240524/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-24 00:01:25.146366 onnxscript-0.1.0.dev20240524/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-24 00:00:57.000000 onnxscript-0.1.0.dev20240524/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.655320 onnxscript-0.1.0.dev20240525/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    11097 2024-05-25 00:00:57.655320 onnxscript-0.1.0.dev20240525/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.611317 onnxscript-0.1.0.dev20240525/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.615317 onnxscript-0.1.0.dev20240525/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.615317 onnxscript-0.1.0.dev20240525/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36693 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.615317 onnxscript-0.1.0.dev20240525/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.615317 onnxscript-0.1.0.dev20240525/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.607316 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.619317 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.635318 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.607316 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.607316 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.635318 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.635318 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1637 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.639319 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27429 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.639319 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   291013 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.643319 onnxscript-0.1.0.dev20240525/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2866 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14092 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    95688 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4301 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2962 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20997 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2775 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/_type_casting.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.643319 onnxscript-0.1.0.dev20240525/onnxscript/ir/passes/
+-rw-r--r--   0 vsts      (1001) docker     (127)      597 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/passes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5545 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/passes/_pass_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    59903 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2954 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/ir/traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19877 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.643319 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.647319 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.647319 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4393 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2633 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1516 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1517 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7351 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26504 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2154 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/bfloat16_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5499 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1674 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29584 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44529 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-25 00:00:57.651320 onnxscript-0.1.0.dev20240525/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11097 2024-05-25 00:00:57.000000 onnxscript-0.1.0.dev20240525/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8329 2024-05-25 00:00:57.000000 onnxscript-0.1.0.dev20240525/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-25 00:00:57.000000 onnxscript-0.1.0.dev20240525/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       45 2024-05-25 00:00:57.000000 onnxscript-0.1.0.dev20240525/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-25 00:00:57.000000 onnxscript-0.1.0.dev20240525/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6474 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-25 00:00:57.655320 onnxscript-0.1.0.dev20240525/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-25 00:00:35.000000 onnxscript-0.1.0.dev20240525/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240524/LICENSE` & `onnxscript-0.1.0.dev20240525/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/PKG-INFO` & `onnxscript-0.1.0.dev20240525/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240524
+Version: 0.1.0.dev20240525
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/d31670646cc2c886048336f6da52932e008e8c1b
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/19f4e26b2296416af647de66271db6d76b9afa81
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
@@ -42,14 +42,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: onnx>=1.16
 Requires-Dist: typing_extensions
+Requires-Dist: ml_dtypes
 
 # ONNX Script
 
 [![CI](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml/badge.svg)](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml)
 [![Dev Release](https://aiinfra.visualstudio.com/ONNX%20Converters/_apis/build/status%2Fonnxscript-release-dev?branchName=main&label=Dev%20Release)](https://aiinfra.visualstudio.com/ONNX%20Converters/_build/latest?definitionId=1258&branchName=main)
 [![PyPI - Version](https://img.shields.io/pypi/v/onnxscript.svg)](https://pypi.org/project/onnxscript)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/onnxscript.svg)](https://pypi.org/project/onnxscript)
```

### Comparing `onnxscript-0.1.0.dev20240524/README.md` & `onnxscript-0.1.0.dev20240525/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240525/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240525/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240525/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240525/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240525/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,39 +11,45 @@
 
 
 def _load_boolean_flag(
     name: str,
     *,
     this_will: str,
     deprecated: bool = False,
+    default: bool = False,
 ) -> bool:
     """Load a boolean flag from environment variable.
 
     Args:
         name: The name of the environment variable.
         this_will: A string that describes what this flag will do.
         deprecated: Whether this flag is deprecated.
+        default: The default value if envvar not defined.
     """
+    undefined = os.getenv(name) is None
     state = os.getenv(name) == "1"
     if state:
         if deprecated:
             logger.error(
                 "Experimental flag %s is deprecated. Please remove it from your environment.",
                 name,
             )
         else:
             logger.warning("Experimental flag %s is enabled. This will %s.", name, this_will)
+    if undefined:
+        state = default
     return state
 
 
 EXPERIMENTAL_INITIALIZERS_AS_INPUTS: bool = _load_boolean_flag(
     "TORCHLIB_EXPERIMENTAL_INITIALIZERS_AS_INPUTS",
     this_will="make initializers as inputs to the model graph",
 )
 EXPERIMENTAL_PREFER_TRACING: bool = _load_boolean_flag(
     "TORCHLIB_EXPERIMENTAL_PREFER_TRACING",
     this_will="trace all traceable functions to fold if branches and collapse constant expressions",
+    default=True,
 )
 EXPERIMENTAL_USE_IR: bool = _load_boolean_flag(
     "TORCHLIB_EXPERIMENTAL_USE_IR",
     this_will="use the ONNX IR instead of the PyTorch Graph for graph building",
 )
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240525/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,19 +64,23 @@
     # Types
     "OperatorIdentifier",
     # Protobuf compatible types
     "TensorProtoTensor",
     # Conversion functions
     "from_proto",
     "to_proto",
+    # IR Tensor initializer
+    "tensor",
     # Pass infrastructure
     "passes",
+    "traversal",
 ]
 
-from onnxscript.ir import passes, serde
+from onnxscript.ir import passes, serde, traversal
+from onnxscript.ir._convenience import tensor
 from onnxscript.ir._core import (
     Attr,
     AttrFloat32,
     AttrFloat32s,
     AttrGraph,
     AttrGraphs,
     AttrInt64,
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_convenience.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,20 +12,25 @@
 
 __all__ = [
     "convert_attribute",
     "convert_attributes",
     "replace_all_uses_with",
 ]
 
+import typing
 from typing import Mapping, Sequence, Union
 
+import numpy as np
 import onnx
 
 from onnxscript.ir import _core, _enums, _protocols, serde
 
+if typing.TYPE_CHECKING:
+    import numpy.typing as npt
+
 SupportedAttrTypes = Union[
     str,
     int,
     float,
     Sequence[int],
     Sequence[float],
     Sequence[str],
@@ -281,7 +286,87 @@
     if not isinstance(replacements, Sequence):
         replacements = (replacements,)
     if len(values) != len(replacements):
         raise ValueError("The number of values and replacements must match.")
     for value, replacement in zip(values, replacements):
         for user_node, index in tuple(value.uses()):
             user_node.replace_input_with(index, replacement)
+
+
+def tensor(
+    value: npt.ArrayLike
+    | onnx.TensorProto
+    | _protocols.DLPackCompatible
+    | _protocols.ArrayCompatible,
+    dtype: _enums.DataType | None = None,
+    name: str | None = None,
+    doc_string: str | None = None,
+) -> _protocols.TensorProtocol:
+    """Create a tensor value from an ArrayLike object or a TensorProto.
+
+    The dtype must match the value. Reinterpretation of the value is
+    not supported, unless if the value is a plain Python object, in which case
+    it is converted to a numpy array with the given dtype.
+
+    :param:`value` can be a numpy array, a plain Python object, or a TensorProto.
+
+    Example::
+
+        >>> from onnxscript import ir
+        >>> import numpy as np
+        >>> import ml_dtypes
+        >>> import onnx
+        >>> ir.tensor(np.array([1, 2, 3], dtype=np.int16))
+        Tensor<INT16,[3]>(array([1, 2, 3], dtype=int16), name=None)
+        >>> ir.tensor([1, 2, 3], dtype=ir.DataType.BFLOAT16)
+        Tensor<BFLOAT16,[3]>(array([1, 2, 3], dtype=bfloat16), name=None)
+        >>> tp_tensor = ir.tensor(onnx.helper.make_tensor("tensor", onnx.TensorProto.FLOAT, dims=[], vals=[0.5]))
+        >>> tp_tensor.numpy()
+        array(0.5, dtype=float32)
+
+    Args:
+        value: The numpy array to create the tensor from.
+        dtype: The data type of the tensor.
+        name: The name of the tensor.
+        doc_string: The documentation string of the tensor.
+
+    Returns:
+        A tensor value.
+
+    Raises:
+        ValueError: If the dtype does not match the value when value is not a plain Python
+            object like ``list[int]``.
+    """
+    if isinstance(value, _protocols.TensorProtocol):
+        if dtype is not None and dtype != value.dtype:
+            raise ValueError(
+                f"The dtype must match the value when value is a Tensor. dtype={dtype}, value.dtype={value.dtype}. "
+                "You do not have to specify the dtype when value is a Tensor."
+            )
+        return value
+    if isinstance(value, onnx.TensorProto):
+        tensor_ = serde.deserialize_tensor(value)
+        if name is not None:
+            tensor_.name = name
+        if doc_string is not None:
+            tensor_.doc_string = doc_string
+        if dtype is not None and dtype != tensor_.dtype:
+            raise ValueError(
+                f"The dtype must match the value when value is a TensorProto. dtype={dtype}, value.data_type={tensor_.dtype}"
+                "You do not have to specify the dtype when value is a TensorProto."
+            )
+    elif isinstance(value, (_protocols.DLPackCompatible, _protocols.ArrayCompatible)):
+        tensor_ = _core.Tensor(value, dtype=dtype, name=name, doc_string=name)
+    else:
+        if dtype is not None:
+            numpy_dtype = dtype.numpy()
+        else:
+            numpy_dtype = None
+        array = np.array(value, dtype=numpy_dtype)
+        tensor_ = _core.Tensor(
+            array,
+            dtype=dtype,
+            shape=_core.Shape(array.shape),
+            name=name,
+            doc_string=name,
+        )
+    return tensor_
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Iterable,
     Iterator,
     OrderedDict,
     Sequence,
     Union,
 )
 
+import ml_dtypes
 import numpy as np
 
 import onnxscript
 from onnxscript.ir import (
     _display,
     _enums,
     _linked_list,
@@ -180,34 +181,41 @@
 
     When the dtype is not one of the numpy native dtypes, the value needs need to be:
 
     - ``int8`` or ``uint8`` for int4, with the sign bit extended to 8 bits.
     - ``uint8`` for uint4.
     - ``uint8`` for 8-bit data types.
     - ``uint16`` for bfloat16
+
+    or corresponding dtypes from the ``ml_dtype`` package.
     """
     if dtype in _NON_NUMPY_NATIVE_TYPES:
-        if dtype.itemsize == 2 and array.dtype != np.uint16:
-            # TODO(justinchuby): Support the storage dtypes like uint16 for bfloat16.
+        if dtype.itemsize == 2 and array.dtype not in (np.uint16, ml_dtypes.bfloat16):
             raise TypeError(
-                f"The numpy array dtype must be uint16 (not {array.dtype}) for IR data type {dtype}."
+                f"The numpy array dtype must be uint16 or ml_dtypes.bfloat16 (not {array.dtype}) for IR data type {dtype}."
             )
-        if dtype.itemsize == 1 and array.dtype != np.uint8:
+        if dtype.itemsize == 1 and array.dtype not in (
+            np.uint8,
+            ml_dtypes.float8_e4m3b11fnuz,
+            ml_dtypes.float8_e4m3fn,
+            ml_dtypes.float8_e5m2fnuz,
+            ml_dtypes.float8_e5m2,
+        ):
             raise TypeError(
-                f"The numpy array dtype must be uint8 (not {array.dtype}) for IR data type {dtype}."
+                f"The numpy array dtype must be uint8 or ml_dtypes.float8* (not {array.dtype}) for IR data type {dtype}."
             )
         if dtype == _enums.DataType.INT4:
-            if array.dtype not in (np.int8, np.uint8):
+            if array.dtype not in (np.int8, np.uint8, ml_dtypes.int4):
                 raise TypeError(
-                    f"The numpy array dtype must be int8 or uint8 (not {array.dtype}) for IR data type {dtype}."
+                    f"The numpy array dtype must be int8 or uint8 or ml_dtypes.int4 (not {array.dtype}) for IR data type {dtype}."
                 )
         if dtype == _enums.DataType.UINT4:
-            if array.dtype != np.uint8:
+            if array.dtype not in (np.uint8, ml_dtypes.uint4):
                 raise TypeError(
-                    f"The numpy array dtype must be uint8 (not {array.dtype}) for IR data type {dtype}."
+                    f"The numpy array dtype must be uint8 or or ml_dtypes.uint4 (not {array.dtype}) for IR data type {dtype}."
                 )
         return
 
     try:
         dtype_numpy = _enums.DataType.from_numpy(array.dtype)
     except TypeError as e:
         raise TypeError(
@@ -218,14 +226,43 @@
 
     if dtype_numpy != dtype:
         raise TypeError(
             f"The numpy array dtype {array.dtype} does not match the IR data type {dtype}."
         )
 
 
+def _maybe_view_np_array_with_ml_dtypes(
+    array: np.ndarray, dtype: _enums.DataType
+) -> np.ndarray:
+    """Reinterpret the array when it is a bit representation of a dtype not supported by numpy.
+
+    Args:
+        array: The numpy array to reinterpret.
+        dtype: The data type to reinterpret the array as.
+
+    Returns:
+        The array reinterpreted as the dtype.
+    """
+    if dtype == _enums.DataType.BFLOAT16:
+        return array.view(ml_dtypes.bfloat16)
+    if dtype == _enums.DataType.FLOAT8E4M3FN:
+        return array.view(ml_dtypes.float8_e4m3fn)
+    if dtype == _enums.DataType.FLOAT8E4M3FNUZ:
+        return array.view(ml_dtypes.float8_e4m3fnuz)
+    if dtype == _enums.DataType.FLOAT8E5M2:
+        return array.view(ml_dtypes.float8_e5m2)
+    if dtype == _enums.DataType.FLOAT8E5M2FNUZ:
+        return array.view(ml_dtypes.float8_e5m2fnuz)
+    if dtype == _enums.DataType.INT4:
+        return array.view(ml_dtypes.int4)
+    if dtype == _enums.DataType.UINT4:
+        return array.view(ml_dtypes.uint4)
+    return array
+
+
 class Tensor(TensorBase, _protocols.TensorProtocol, Generic[TArrayCompatible]):  # pylint: disable=too-many-ancestors
     """An immutable concrete tensor.
 
     This class is a wrapper around the raw tensor data. The raw tensor data can be a numpy array
     compatible object (e.g. ``np.ndarray``, ``torch.Tensor``) or a ``DLPack`` compatible object.
     The tensor is immutable and the data is not copied at initialization.
 
@@ -323,14 +360,19 @@
         else:
             if isinstance(value, np.ndarray):
                 # Make sure the dtype matches the value
                 _check_numpy_representation_type(value, dtype)
             # Users are responsible for making sure the dtype matches the value
             # when value is not a numpy array
             self._dtype = dtype
+
+        # View the bfloat16, float8 and int4 types using ml_dtypes
+        if isinstance(value, np.ndarray):
+            value = _maybe_view_np_array_with_ml_dtypes(value, self._dtype)  # type: ignore[assignment]
+
         self._raw = value
         self.name = name
         self.doc_string = doc_string
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props = metadata_props
 
     def __array__(self, dtype: Any = None) -> np.ndarray:
@@ -368,21 +410,17 @@
     def raw(self) -> TArrayCompatible:
         """Backing data of the tensor. Immutable."""
         return self._raw  # type: ignore[return-value]
 
     def numpy(self) -> np.ndarray:
         """Return the tensor as a numpy array.
 
-        When the data type is not supported by numpy, the value is the bit representation
-        of the dtype:
-
-        - ``int8`` for int4, with the sign bit extended to 8 bits.
-        - ``uint8`` for uint4.
-        - ``uint8`` for 8-bit data types like float8.
-        - ``uint16`` for bfloat16.
+        When the data type is not supported by numpy, the dtypes from the ``ml_dtype``
+        package are used. The values can be reinterpreted as bit representations
+        using the ``.view()`` method.
         """
         if isinstance(self._raw, np.ndarray):
             return self._raw
         # We do not cache the value to save memory
         return self.__array__()
 
     def tobytes(self) -> bytes:
@@ -524,14 +562,16 @@
                 f.fileno(),
                 0,
                 access=mmap.ACCESS_READ,
             )
         # Handle the byte order correctly by always using little endian
         dt = np.dtype(self.dtype.numpy()).newbyteorder("<")
         if self.dtype in {_enums.DataType.INT4, _enums.DataType.UINT4}:
+            # Use uint8 to read in the full byte. Otherwise ml_dtypes.int4 will clip the values
+            dt = np.dtype(np.uint8).newbyteorder("<")
             count = self.size // 2 + self.size % 2
         else:
             count = self.size
         self._array = np.frombuffer(self.raw, dtype=dt, offset=self.offset or 0, count=count)
         shape = self.shape.numpy()
         if self.dtype == _enums.DataType.INT4:
             # Unpack the int4 arrays
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # --------------------------------------------------------------------------
 """ONNX IR enums that matches the ONNX spec."""
 
 from __future__ import annotations
 
 import enum
 
+import ml_dtypes
 import numpy as np
 
 
 class AttributeType(enum.IntEnum):
     """Enum for the types of ONNX attributes."""
 
     UNDEFINED = 0
@@ -121,14 +122,15 @@
     DataType.FLOAT8E5M2: 1,
     DataType.FLOAT8E5M2FNUZ: 1,
     DataType.UINT4: 0.5,
     DataType.INT4: 0.5,
 }
 
 
+# We use ml_dtypes to support dtypes that are not in numpy.
 _NP_TYPE_TO_DATA_TYPE = {
     np.dtype("bool"): DataType.BOOL,
     np.dtype("complex128"): DataType.COMPLEX128,
     np.dtype("complex64"): DataType.COMPLEX64,
     np.dtype("float16"): DataType.FLOAT16,
     np.dtype("float32"): DataType.FLOAT,
     np.dtype("float64"): DataType.DOUBLE,
@@ -137,23 +139,18 @@
     np.dtype("int64"): DataType.INT64,
     np.dtype("int8"): DataType.INT8,
     np.dtype("object"): DataType.STRING,
     np.dtype("uint16"): DataType.UINT16,
     np.dtype("uint32"): DataType.UINT32,
     np.dtype("uint64"): DataType.UINT64,
     np.dtype("uint8"): DataType.UINT8,
+    np.dtype(ml_dtypes.bfloat16): DataType.BFLOAT16,
+    np.dtype(ml_dtypes.float8_e4m3fn): DataType.FLOAT8E4M3FN,
+    np.dtype(ml_dtypes.float8_e4m3fnuz): DataType.FLOAT8E4M3FNUZ,
+    np.dtype(ml_dtypes.float8_e5m2): DataType.FLOAT8E5M2,
+    np.dtype(ml_dtypes.float8_e5m2fnuz): DataType.FLOAT8E5M2FNUZ,
+    np.dtype(ml_dtypes.int4): DataType.INT4,
+    np.dtype(ml_dtypes.uint4): DataType.UINT4,
 }
 
-# ONNX DataType to Numpy dtype. This mapping does not capture ONNX data
-# types that are not supported by numpy.
+# ONNX DataType to Numpy dtype.
 _DATA_TYPE_TO_NP_TYPE = {v: k for k, v in _NP_TYPE_TO_DATA_TYPE.items()}
-_DATA_TYPE_TO_NP_TYPE.update(
-    {
-        DataType.FLOAT8E4M3FN: np.dtype("uint8"),
-        DataType.FLOAT8E4M3FNUZ: np.dtype("uint8"),
-        DataType.FLOAT8E5M2: np.dtype("uint8"),
-        DataType.FLOAT8E5M2FNUZ: np.dtype("uint8"),
-        DataType.UINT4: np.dtype("uint8"),
-        DataType.INT4: np.dtype("int8"),
-        DataType.BFLOAT16: np.dtype("uint16"),
-    }
-)
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/_type_casting.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/_type_casting.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 # TODO(justinchuby): Upstream the logic to onnx
 
 from __future__ import annotations
 
 import typing
 from typing import Sequence
 
+import ml_dtypes
 import numpy as np
 
 if typing.TYPE_CHECKING:
     import numpy.typing as npt
 
 
 def pack_int4(array: np.ndarray) -> npt.NDArray[np.uint8]:
     """Convert a numpy array to flatten, packed int4/uint4. Elements must be in the correct range."""
     # Create a 1D copy
-    array_flat = array.ravel().astype(np.uint8)
+    array_flat = array.ravel().view(np.uint8).copy()
     size = array.size
     odd_sized = size % 2 == 1
     if odd_sized:
         array_flat.resize([size + 1], refcheck=False)
     array_flat &= 0x0F
     array_flat[1::2] <<= 4
     return array_flat[0::2] | array_flat[1::2]  # type: ignore[return-type]
 
 
-def unpack_uint4(data: npt.NDArray[np.uint8], dims: Sequence[int]) -> npt.NDArray[np.uint8]:
+def _unpack_uint4_as_uint8(
+    data: npt.NDArray[np.uint8], dims: Sequence[int]
+) -> npt.NDArray[np.uint8]:
     """Convert a packed uint4 array to unpacked uint4 array represented as uint8.
 
     Args:
         data: A numpy array.
         dims: The dimensions are used to reshape the unpacked buffer.
 
     Returns:
@@ -44,41 +47,43 @@
     if result.size == np.prod(dims) + 1:
         # handle single-element padding due to odd number of elements
         result = result[:-1]
     result.resize(dims, refcheck=False)
     return result
 
 
-def _int4_to_int8(x: npt.NDArray[np.uint8]) -> npt.NDArray[np.int8]:
+def unpack_uint4(
+    data: npt.NDArray[np.uint8], dims: Sequence[int]
+) -> npt.NDArray[ml_dtypes.uint4]:
+    """Convert a packed uint4 array to unpacked uint4 array represented as uint8.
+
+    Args:
+        data: A numpy array.
+        dims: The dimensions are used to reshape the unpacked buffer.
+
+    Returns:
+        A numpy array of int8/uint8 reshaped to dims.
+    """
+    return _unpack_uint4_as_uint8(data, dims).view(ml_dtypes.uint4)
+
+
+def _extend_int4_sign_bits(x: npt.NDArray[np.uint8]) -> npt.NDArray[np.int8]:
     """Extend 4-bit signed integer to 8-bit signed integer."""
     return np.where((x >> 3) == 0, x, x | 0xF0).astype(np.int8)
 
 
-def unpack_int4(data: npt.NDArray[np.uint8], dims: Sequence[int]) -> npt.NDArray[np.int8]:
+def unpack_int4(
+    data: npt.NDArray[np.uint8], dims: Sequence[int]
+) -> npt.NDArray[ml_dtypes.int4]:
     """Convert a packed (signed) int4 array to unpacked int4 array represented as int8.
 
     The sign bit is extended to the most significant bit of the int8.
 
     Args:
         data: A numpy array.
         dims: The dimensions are used to reshape the unpacked buffer.
 
     Returns:
         A numpy array of int8 reshaped to dims.
     """
-    unpacked = unpack_uint4(data, dims)
-    return _int4_to_int8(unpacked)
-
-
-def float32_to_bfloat16(array: npt.NDArray[np.float32]) -> npt.NDArray[np.uint16]:
-    """Convert a numpy array to uint16 representation of bfloat16."""
-    bfloat16_array = array.astype(np.float32).view(np.uint32)
-    # Drop bottom 16-bits
-    # Round remaining bits using round-to-nearest-even
-    rounded = bfloat16_array >> 16
-    rounded &= 1
-    rounded += 0x7FFF
-    bfloat16_array += rounded  # type: ignore[arg-type]
-    bfloat16_array >>= 16
-    # NaN requires at least 1 significant bit set
-    bfloat16_array[np.isnan(array)] = 0x7FC0  # sign=0, exp=all-ones, sig=0b1000000
-    return bfloat16_array.astype(np.uint16)
+    unpacked = _unpack_uint4_as_uint8(data, dims)
+    return _extend_int4_sign_bits(unpacked).view(ml_dtypes.int4)
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240525/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,21 +218,17 @@
 
         This is an improved version of onnx.numpy_helper.to_array.
         It first reads the data using the dtype corresponding to the tensor
         proto data field, then converts it to the correct dtype and shape.
         Special cases are bfloat16, complex and int4 where we need to
         reinterpret the data. Other types can simply be casted.
 
-        When the data type is not supported by numpy, the value is the bit representation
-        of the dtype:
-
-        - ``int8`` for int4, with the sign bit extended to 8 bits.
-        - ``uint8`` for uint4.
-        - ``uint8`` for 8-bit data types like float8.
-        - ``uint16`` for bfloat16.
+        When the data type is not supported by numpy, the dtypes from the ``ml_dtype``
+        package are used. The values can be reinterpreted as bit representations
+        using the ``.view()`` method.
 
         When the data type is a string, this method returns a numpy array
         of bytes instead of a numpy array of strings, to follow the ONNX
         specification.
 
         External tensors are not supported by this class. Use
         :class:`onnxscript.ir.ExternalTensor` instead.
@@ -252,17 +248,24 @@
         if self._proto.HasField("raw_data"):
             array = np.frombuffer(self._proto.raw_data, dtype=dtype.numpy().newbyteorder("<"))
             # Cannot return now, because we may need to unpack 4bit tensors
         elif dtype == _enums.DataType.STRING:
             return np.array(self._proto.string_data).reshape(self._proto.dims)
         elif self._proto.int32_data:
             array = np.array(self._proto.int32_data, dtype=_little_endian_dtype(np.int32))
-            if dtype == _enums.DataType.FLOAT16:
-                # Reinterpret the int32 as float16; bfloat16 is handled on the last line
-                array = array.astype(np.uint16).view(np.float16)
+            if dtype in {_enums.DataType.FLOAT16, _enums.DataType.BFLOAT16}:
+                # Reinterpret the int32 as float16 or bfloat16
+                array = array.astype(np.uint16).view(dtype.numpy())
+            elif dtype in {
+                _enums.DataType.FLOAT8E4M3FN,
+                _enums.DataType.FLOAT8E4M3FNUZ,
+                _enums.DataType.FLOAT8E5M2,
+                _enums.DataType.FLOAT8E5M2FNUZ,
+            }:
+                array = array.astype(np.uint8).view(dtype.numpy())
         elif self._proto.int64_data:
             array = np.array(self._proto.int64_data, dtype=_little_endian_dtype(np.int64))
         elif self._proto.uint64_data:
             array = np.array(self._proto.uint64_data, dtype=_little_endian_dtype(np.uint64))
         elif self._proto.float_data:
             array = np.array(self._proto.float_data, dtype=_little_endian_dtype(np.float32))
             if dtype == _enums.DataType.COMPLEX64:
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240525/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/main.py` & `onnxscript-0.1.0.dev20240525/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240525/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/remove_unused_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,74 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from __future__ import annotations
 
 import logging
+from typing import TypeVar
 
 import onnx
 
 from onnxscript import ir
 
 logger = logging.getLogger(__name__)
 
 
-class UnusedFunctionRemover(ir.passes.NodeTransformer):
+TModel = TypeVar("TModel", ir.Model, onnx.ModelProto)
+
+
+def _clean_up_unused_functions(model: ir.Model, unused: set[ir.OperatorIdentifier]) -> None:
+    """Removes unused functions from the model."""
+    for op_identifier in unused:
+        del model.functions[op_identifier]
+
+    logger.info("Removed %s unused functions", len(unused))
+    logger.debug("Functions left: %s", list(model.functions))
+    logger.debug("Functions removed: %s", unused)
+
+
+class RemoveUnusedFunctionPass(ir.passes.PassBase):
     def __init__(self):
         super().__init__()
-        self.used: set[ir.OperatorIdentifier] = set()
+        self.used: set[ir.OperatorIdentifier] | None = None
+
+    def call(self, model: ir.Model) -> ir.passes.PassResult:
+        self.used = set()
+        for node in ir.traversal.RecursiveGraphIterator(model.graph):
+            self._call_node(model, node)
+
+        # Update the model to remove unused functions
+        unused = set(model.functions) - self.used
+        if not unused:
+            logger.info("No unused functions to remove")
+            return ir.passes.PassResult(model, modified=False)
 
-    def _call_function(self, function: ir.Function) -> None:
+        _clean_up_unused_functions(model, unused)
+        self.used = None
+        return ir.passes.PassResult(model, modified=True)
+
+    def _call_function(self, model: ir.Model, function: ir.Function) -> None:
+        assert self.used is not None
         if function.identifier() in self.used:
             # The function and its nodes are already recorded as used
             return
         self.used.add(function.identifier())
-        for node in function:
-            self.call_node_recursive(node)
+        for node in ir.traversal.RecursiveGraphIterator(function):
+            self._call_node(model, node)
 
-    def call_node(self, node: ir.Node) -> None:
+    def _call_node(self, model: ir.Model, node: ir.Node) -> None:
         op_identifier = node.op_identifier()
-        if op_identifier in self.model.functions:
-            self._call_function(self.model.functions[op_identifier])
-        else:
-            self.used.add(op_identifier)
-
-    def exit_pass(self) -> None:
-        # Update the model to remove unused functions
-        unused = set(self.model.functions) - self.used
-        if not unused:
-            logger.info("No unused functions to remove")
-            self.modified = False
+        if op_identifier not in model.functions:
             return
-        for op_identifier in unused:
-            if op_identifier not in self.used:
-                del self.model.functions[op_identifier]
-        self.modified = True
-        logger.info("Removed %s unused functions", len(unused))
-        logger.debug("Functions left: %s", list(self.model.functions))
-        logger.debug("Functions removed: %s", unused)
+        self._call_function(model, model.functions[op_identifier])
 
 
-def remove_unused_functions(model_proto: onnx.ModelProto) -> onnx.ModelProto:
+def remove_unused_functions(model: TModel) -> TModel:
     """Removes unused function protos from the model."""
-    # TODO(justinchuby): Update this to accept an ir.Model
-    model = ir.serde.deserialize_model(model_proto)
-    UnusedFunctionRemover()(model)
-    model_proto = ir.serde.serialize_model(model)
 
-    return model_proto
+    if isinstance(model, ir.Model):
+        return RemoveUnusedFunctionPass()(model).model  # type: ignore[return-value]
+
+    model_ = ir.serde.deserialize_model(model)
+    result = RemoveUnusedFunctionPass()(model_)
+    return ir.serde.serialize_model(result.model)
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240525/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240525/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240525/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240525/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240525/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240525/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240525/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript/values.py` & `onnxscript-0.1.0.dev20240525/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240525/onnxscript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240524
+Version: 0.1.0.dev20240525
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/d31670646cc2c886048336f6da52932e008e8c1b
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/19f4e26b2296416af647de66271db6d76b9afa81
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
@@ -42,14 +42,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: onnx>=1.16
 Requires-Dist: typing_extensions
+Requires-Dist: ml_dtypes
 
 # ONNX Script
 
 [![CI](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml/badge.svg)](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml)
 [![Dev Release](https://aiinfra.visualstudio.com/ONNX%20Converters/_apis/build/status%2Fonnxscript-release-dev?branchName=main&label=Dev%20Release)](https://aiinfra.visualstudio.com/ONNX%20Converters/_build/latest?definitionId=1258&branchName=main)
 [![PyPI - Version](https://img.shields.io/pypi/v/onnxscript.svg)](https://pypi.org/project/onnxscript)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/onnxscript.svg)](https://pypi.org/project/onnxscript)
```

### Comparing `onnxscript-0.1.0.dev20240524/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240525/onnxscript.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 onnxscript/ir/_graph_comparison.py
 onnxscript/ir/_linked_list.py
 onnxscript/ir/_metadata.py
 onnxscript/ir/_name_authority.py
 onnxscript/ir/_protocols.py
 onnxscript/ir/_type_casting.py
 onnxscript/ir/serde.py
+onnxscript/ir/traversal.py
 onnxscript/ir/passes/__init__.py
 onnxscript/ir/passes/_pass_infra.py
 onnxscript/onnx_opset/__init__.py
 onnxscript/onnx_opset/_impl/opset1.py
 onnxscript/onnx_opset/_impl/opset10.py
 onnxscript/onnx_opset/_impl/opset11.py
 onnxscript/onnx_opset/_impl/opset12.py
```

### Comparing `onnxscript-0.1.0.dev20240524/pyproject.toml` & `onnxscript-0.1.0.dev20240525/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "License :: OSI Approved :: MIT License",
 ]
-dependencies = ["numpy", "onnx>=1.16", "typing_extensions"]
+dependencies = ["numpy", "onnx>=1.16", "typing_extensions", "ml_dtypes"]
 
 [tool.setuptools.packages.find]
 include = ["onnxscript*"]
 
 [tool.setuptools.package-data]
 onnxscript = ["py.typed"]
 onnx = ["py.typed"]
```

### Comparing `onnxscript-0.1.0.dev20240524/setup.py` & `onnxscript-0.1.0.dev20240525/setup.py`

 * *Files identical despite different names*

