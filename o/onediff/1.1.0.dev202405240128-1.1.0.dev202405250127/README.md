# Comparing `tmp/onediff-1.1.0.dev202405240128.tar.gz` & `tmp/onediff-1.1.0.dev202405250127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.1.0.dev202405240128.tar", last modified: Fri May 24 01:28:19 2024, max compression
+gzip compressed data, was "onediff-1.1.0.dev202405250127.tar", last modified: Sat May 25 01:27:38 2024, max compression
```

## Comparing `onediff-1.1.0.dev202405240128.tar` & `onediff-1.1.0.dev202405250127.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.719182 onediff-1.1.0.dev202405240128/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-24 01:28:19.719182 onediff-1.1.0.dev202405240128/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:28:19.719182 onediff-1.1.0.dev202405240128/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.703182 onediff-1.1.0.dev202405240128/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.707182 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.707182 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.707182 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.707182 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.707182 onediff-1.1.0.dev202405240128/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.707182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.711182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.711182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/nexfort/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/nexfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/nexfort/nexfort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.711182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/param_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.715182 onediff-1.1.0.dev202405240128/src/onediff/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/torch_utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/torch_utils/module_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.719182 onediff-1.1.0.dev202405240128/src/onediff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/src/onediff/utils/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.719182 onediff-1.1.0.dev202405240128/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-24 01:28:19.000000 onediff-1.1.0.dev202405240128/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-24 01:28:19.000000 onediff-1.1.0.dev202405240128/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:28:19.000000 onediff-1.1.0.dev202405240128/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 01:28:19.000000 onediff-1.1.0.dev202405240128/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 01:28:19.000000 onediff-1.1.0.dev202405240128/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:19.719182 onediff-1.1.0.dev202405240128/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-24 01:28:11.000000 onediff-1.1.0.dev202405240128/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.784312 onediff-1.1.0.dev202405250127/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-25 01:27:38.784312 onediff-1.1.0.dev202405250127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 01:27:38.784312 onediff-1.1.0.dev202405250127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.768312 onediff-1.1.0.dev202405250127/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.772312 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.772312 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77125 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24024 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61005 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.772312 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.772312 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.772312 onediff-1.1.0.dev202405250127/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.772312 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.776311 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.776311 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/nexfort/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/nexfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/nexfort/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/nexfort/nexfort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.776311 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.776311 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/param_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/torch_utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/torch_utils/module_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/src/onediff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/src/onediff/utils/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.784312 onediff-1.1.0.dev202405250127/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-25 01:27:38.000000 onediff-1.1.0.dev202405250127/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-25 01:27:38.000000 onediff-1.1.0.dev202405250127/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:27:38.000000 onediff-1.1.0.dev202405250127/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-25 01:27:38.000000 onediff-1.1.0.dev202405250127/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 01:27:38.000000 onediff-1.1.0.dev202405250127/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:27:38.780312 onediff-1.1.0.dev202405250127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-25 01:27:33.000000 onediff-1.1.0.dev202405250127/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.1.0.dev202405240128/LICENSE` & `onediff-1.1.0.dev202405250127/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/PKG-INFO` & `onediff-1.1.0.dev202405250127/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405240128
+Version: 1.1.0.dev202405250127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405240128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405250127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405240128/README.md` & `onediff-1.1.0.dev202405250127/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/setup.py` & `onediff-1.1.0.dev202405250127/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.1.0.dev202405250127/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/compiler.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/nexfort/deployable_module.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/nexfort/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/nexfort/nexfort.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/nexfort/nexfort.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import dataclasses
 import torch
 from ..registry import register_backend
 
 
 @register_backend("nexfort")
 def compile(torch_module: torch.nn.Module, *, options=None):
-    from nexfort.utils.memory_format import apply_memory_format
     from nexfort.compilers import nexfort_compile
-    from .deployable_module import NexfortDeployableModule
-    from ..options import CompileOptions
+    if isinstance(options, str):
+        import json
 
-    options = options if options is not None else CompileOptions()
-    nexfort_options = options.nexfort
+        # TODO(): using jsonschema to define the options schema
+        options = json.loads(options)
+
+    nexfort_options = options if options is not None else dict()
     compiled_model = nexfort_compile(torch_module, **nexfort_options)
-    # return NexfortDeployableModule(compiled_model, torch_module)
     return compiled_model
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/deployable_module.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/dual_module.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/dual_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def oneflow_module(self):
         if self._oneflow_module is not None:
             return self._oneflow_module
 
         logger.debug(f"Convert {type(self._torch_module)} ...")
         self._oneflow_module = torch2oflow(self._torch_module)
         logger.debug(f"Convert {type(self._torch_module)} done!")
+
         return self._oneflow_module
 
     @oneflow_module.deleter
     def oneflow_module(self):
         if self._oneflow_module:
             del self._oneflow_module
             setattr(self, "_oneflow_module", None)
@@ -95,22 +96,29 @@
         else:
             return oneflow_attr if oneflow_exec_mode_enabled() else torch_attr
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in ["_torch_module", "_oneflow_module"]:
             super().__setattr__(name, value)
         else:  # TODO: aviod memory up when set attr
+            _torch_module: torch.nn.Module = self._torch_module
+            if (
+                hasattr(_torch_module, "_disable_param_update")
+                and _torch_module._disable_param_update
+            ):
+                return
+
             if self._oneflow_module is not None:
                 v = torch2oflow(value)
                 if isinstance(v, flow.Tensor):
                     obj = getattr(self._oneflow_module, name)
                     obj.copy_(v)
                 else:
                     setattr(self._oneflow_module, name, v)
-            setattr(self._torch_module, name, value)
+            setattr(_torch_module, name, value)
 
     def extra_repr(self) -> str:
         return self._torch_module.extra_repr()
 
 
 class DualModuleList(torch.nn.ModuleList):
     def __init__(self, torch_modules, oneflow_modules):
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/env_var.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/env_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional
 
 from onediff.utils import set_boolean_env_var, set_integer_env_var
 
 
 @dataclasses.dataclass
 class OneflowCompileOptions:
+    dynamic: bool = True
     use_graph: bool = True
     debug_level: int = -1
     max_cached_graph_size: int = 9
     graph_file: str = None
     graph_file_device: torch.device = None
 
     # Optimization related environment variables
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/graph.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/import_tools/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/oneflow.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/oneflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,51 +5,52 @@
 
 @register_backend("oneflow")
 def compile(torch_module: torch.nn.Module, *, options=None):
     """
     Transform a torch nn.Module to oneflow.nn.Module, then optimize it with oneflow.nn.Graph.
     Args:
        model (torch.nn.Module): Module to optimize
-       options (CompileOptions): Compilation options to pass to the compiler:
+       options (OneflowCompileOptions): Compilation options to pass to the compiler:
         - 'dynamic': When this is True, we will generate one graph and reuse it to avoid recompilations when
                      input shape change.  This may not always work as some operations/optimizations break the contition of
                      reusing. When this is False, we will generate a graph for each new input shape, and will always specialize.
                      default True.
         - 'use_graph' whether to optimize with oneflow.nn.Graph, default True.
         - 'debug' which config the nn.Graph debug level, default -1(no debug info), max 3(max debug info).
         - 'size' which config the cache size when cache is enabled. Note that after onediff v0.12, cache is default disabled.
         - 'graph_file' (None) generates a compilation cache file. If the file exists, loading occurs; if not, the compilation result is saved after the first run.
         - 'graph_file_device' (None) sets the device for the graph file, default None.  If set, the compilation result will be converted to the specified device.
     """
     from .deployable_module import OneflowDeployableModule, get_mixed_deployable_module
-    from .env_var import set_oneflow_default_env_vars, set_oneflow_env_vars
-    from ..options import CompileOptions
+    from .env_var import (
+        set_oneflow_default_env_vars,
+        set_oneflow_env_vars,
+        OneflowCompileOptions,
+    )
     from .param_utils import (
         state_update_hook,
         init_state_update_attr,
         forward_pre_check_and_update_state_hook,
         forward_generate_constant_folding_info_hook,
     )
     from .transform.custom_transform import set_default_registry
 
     set_oneflow_default_env_vars()
     set_default_registry()
 
-    options = options if options is not None else CompileOptions()
-    set_oneflow_env_vars(options.oneflow)
+    options = options if options is not None else OneflowCompileOptions()
+    set_oneflow_env_vars(options)
 
     def wrap_module(module):
         if isinstance(module, OneflowDeployableModule):
             assert not module._is_raw_deployable_module
-            return module.__class__.from_existing(
-                module, options.dynamic, options.oneflow
-            )
+            return module.__class__.from_existing(module, options.dynamic, options)
         else:
             return get_mixed_deployable_module(module.__class__)(
-                module, None, options.dynamic, options.oneflow
+                module, None, options.dynamic, options
             )
 
     model = wrap_module(torch_module)
     assert isinstance(model, OneflowDeployableModule)
     assert isinstance(model, torch_module.__class__)
 
     def state_dict_hook(module, state_dict, prefix, local_metadata):
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/online_quantization_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             seed,
             calibration_info=calibration_info,
         )
     module = OnlineQuantModule(calculator, False, inplace=inplace)
     in_args, in_kwargs = patch_input_adapter(input_args, input_kwargs)
     quantized_model, info = module.quantize_with_calibration(*in_args, **in_kwargs)
     status = module.collect_quantization_status(model, info)
+    for _, layer in quantized_model.named_modules():
+        layer._disable_param_update = True
 
     return quantized_model, status
 
 
 def quantize_and_deploy_wrapper(func):
     def wrapper(self: "DeployableModule", *args, **kwargs):
         torch_model = self._torch_module
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/param_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/manager.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/transform/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/oneflow/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.1.0.dev202405250127/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/optimization/attention_processor.py` & `onediff-1.1.0.dev202405250127/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/optimization/quant_optimizer.py` & `onediff-1.1.0.dev202405250127/src/onediff/optimization/quant_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import time
 import torch
 import torch.nn as nn
 from copy import deepcopy
 from onediff.utils import logger
-from onediff.infer_compiler.backends.oneflow.utils.version_util import is_quantization_enabled
+from onediff.infer_compiler.backends.oneflow.utils.version_util import (
+    is_quantization_enabled,
+)
 from onediff.infer_compiler.backends.oneflow.utils.cost_util import cost_cnt
 from onediff.infer_compiler.backends.oneflow.transform.manager import transform_mgr
 from onediff.torch_utils.module_operations import modify_sub_module
 
 
 __all__ = ["quantize_model", "varify_can_use_quantization"]
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.1.0.dev202405250127/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/quantization/load_quantized_model.py` & `onediff-1.1.0.dev202405250127/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.1.0.dev202405250127/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.1.0.dev202405250127/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/quantization/quantize_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/torch_utils/model_inplace_assign.py` & `onediff-1.1.0.dev202405250127/src/onediff/torch_utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/torch_utils/module_operations.py` & `onediff-1.1.0.dev202405250127/src/onediff/torch_utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/utils/env_var.py` & `onediff-1.1.0.dev202405250127/src/onediff/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff/utils/log_utils.py` & `onediff-1.1.0.dev202405250127/src/onediff/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/src/onediff.egg-info/PKG-INFO` & `onediff-1.1.0.dev202405250127/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405240128
+Version: 1.1.0.dev202405250127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405240128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405250127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405240128/src/onediff.egg-info/SOURCES.txt` & `onediff-1.1.0.dev202405250127/src/onediff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 src/onediff.egg-info/dependency_links.txt
 src/onediff.egg-info/requires.txt
 src/onediff.egg-info/top_level.txt
 src/onediff/infer_compiler/__init__.py
 src/onediff/infer_compiler/backends/__init__.py
 src/onediff/infer_compiler/backends/compiler.py
 src/onediff/infer_compiler/backends/deployable_module.py
-src/onediff/infer_compiler/backends/options.py
 src/onediff/infer_compiler/backends/registry.py
 src/onediff/infer_compiler/backends/nexfort/__init__.py
 src/onediff/infer_compiler/backends/nexfort/deployable_module.py
 src/onediff/infer_compiler/backends/nexfort/nexfort.py
 src/onediff/infer_compiler/backends/oneflow/__init__.py
 src/onediff/infer_compiler/backends/oneflow/args_tree_util.py
 src/onediff/infer_compiler/backends/oneflow/deployable_module.py
```

### Comparing `onediff-1.1.0.dev202405240128/tests/test_dual_module_list.py` & `onediff-1.1.0.dev202405250127/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.1.0.dev202405250127/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/tests/test_quantitative_quality.py` & `onediff-1.1.0.dev202405250127/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405240128/tests/test_quantize_custom_model.py` & `onediff-1.1.0.dev202405250127/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

