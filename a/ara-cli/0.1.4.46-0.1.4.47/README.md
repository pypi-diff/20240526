# Comparing `tmp/ara_cli-0.1.4.46.tar.gz` & `tmp/ara_cli-0.1.4.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ara_cli-0.1.4.46.tar", last modified: Tue May 21 07:36:03 2024, max compression
+gzip compressed data, was "ara_cli-0.1.4.47.tar", last modified: Sun May 26 19:59:49 2024, max compression
```

## Comparing `ara_cli-0.1.4.46.tar` & `ara_cli-0.1.4.47.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/MANIFEST.in
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3962 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/README.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.230291 ara_cli-0.1.4.46/ara_cli/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    11473 2024-05-21 07:35:01.000000 ara_cli-0.1.4.46/ara_cli/__main__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/ara_config.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_deleter.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3643 2024-05-18 20:11:16.000000 ara_cli-0.1.4.46/ara_cli/chat.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/classifier_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/file_classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/filename_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1759 2024-05-18 21:13:35.000000 ara_cli-0.1.4.46/ara_cli/prompt_chat.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5966 2024-05-21 07:26:18.000000 ara_cli-0.1.4.46/ara_cli/prompt_extractor.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15579 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/prompt_handler.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/prompt_rag.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/run_file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/template_manager.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.230291 ara_cli-0.1.4.46/ara_cli/templates/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/agile.artefacts
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.226291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.238291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1060 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      797 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1413 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      836 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      807 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/empty_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1425 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/error_fixing_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1611 2024-05-19 20:39:37.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/feature_file_update_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      832 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      932 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      684 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.238291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/classify_task_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/empty_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/error_fixing_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      126 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_fix_steps_for_scenario_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      155 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_formulation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       92 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_reverse_formulation_from_code_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      201 2024-05-18 21:20:54.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-19 21:21:55.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_update_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      140 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_scenario_outline_extension_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      163 2024-05-19 21:13:03.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_update_formulation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      264 2024-05-19 21:13:39.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/fibonacci_example_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      207 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/js_implementation_from_task_description_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      247 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/js_steps_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/python_cli_implementation_with_test_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/python_code_understanding_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      351 2024-05-19 21:22:51.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/task_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-19 21:18:05.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/task_stepwise_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      866 2024-05-19 21:29:15.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rename.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/empty_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1024 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      971 2024-05-18 19:10:04.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/gherkin_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      814 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/product_owner_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.step.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.businessgoal
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.businessgoal_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.capability
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.capability_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.epic
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.epic_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.example
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.example_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.feature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.feature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.issue
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.keyfeature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.keyfeature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.steps_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      442 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.task
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.task_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.userstory
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.userstory_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.vision
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.vision_exploration.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/ara_cli/tests/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_file_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_template_manager.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2330 2024-05-19 21:36:29.000000 ara_cli-0.1.4.46/ara_cli/update_config_prompt.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/vectorDB.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-21 07:20:12.000000 ara_cli-0.1.4.46/ara_cli/version.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.230291 ara_cli-0.1.4.46/ara_cli.egg-info/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     7111 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/entry_points.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/requires.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/top_level.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/setup.cfg
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/setup.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/MANIFEST.in
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3962 2024-05-21 09:27:22.000000 ara_cli-0.1.4.47/README.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.189013 ara_cli-0.1.4.47/ara_cli/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    11473 2024-05-21 07:35:01.000000 ara_cli-0.1.4.47/ara_cli/__main__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/ara_config.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/artefact.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/artefact_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/artefact_deleter.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/artefact_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3769 2024-05-26 19:59:05.000000 ara_cli-0.1.4.47/ara_cli/chat.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/classifier_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/file_classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/filename_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1759 2024-05-18 21:13:35.000000 ara_cli-0.1.4.47/ara_cli/prompt_chat.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5966 2024-05-21 07:26:18.000000 ara_cli-0.1.4.47/ara_cli/prompt_extractor.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15579 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/prompt_handler.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/prompt_rag.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/run_file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/template_manager.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.193013 ara_cli-0.1.4.47/ara_cli/templates/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/agile.artefacts
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.185013 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.193013 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.193013 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/prompts/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.197013 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.197013 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.197013 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1060 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      797 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1413 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      836 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      807 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/empty_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1425 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/error_fixing_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1611 2024-05-19 20:39:37.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/feature_file_update_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      832 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      932 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/refactoring_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      684 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/classify_task_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/empty_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/error_fixing_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      126 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_fix_steps_for_scenario_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      155 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_formulation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       92 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_reverse_formulation_from_code_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      201 2024-05-18 21:20:54.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-19 21:21:55.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_update_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      140 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_scenario_outline_extension_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      163 2024-05-19 21:13:03.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/feature_update_formulation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      264 2024-05-19 21:13:39.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/fibonacci_example_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      207 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/js_implementation_from_task_description_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      247 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/js_steps_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/python_cli_implementation_with_test_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/python_code_understanding_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      351 2024-05-19 21:22:51.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/task_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-19 21:18:05.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/prompts/task_stepwise_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      866 2024-05-19 21:29:15.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rename.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/empty_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1024 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      971 2024-05-18 19:10:04.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/gherkin_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      814 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/product_owner_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.concept.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.customer.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.persona.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.step.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.technology.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.businessgoal
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.businessgoal_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.capability
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.capability_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.epic
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.epic_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.example
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.example_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.feature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.feature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.issue
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.keyfeature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.keyfeature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.steps_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      442 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.task
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.task_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.userstory
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.userstory_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.vision
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/templates/template.vision_exploration.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/ara_cli/tests/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/tests/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/tests/test_artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/tests/test_artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/tests/test_directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/tests/test_file_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/tests/test_template_manager.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2553 2024-05-21 13:09:34.000000 ara_cli-0.1.4.47/ara_cli/update_config_prompt.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/ara_cli/vectorDB.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-26 19:23:05.000000 ara_cli-0.1.4.47/ara_cli/version.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-26 19:59:49.189013 ara_cli-0.1.4.47/ara_cli.egg-info/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-26 19:59:49.000000 ara_cli-0.1.4.47/ara_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     7111 2024-05-26 19:59:49.000000 ara_cli-0.1.4.47/ara_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-26 19:59:49.000000 ara_cli-0.1.4.47/ara_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-26 19:59:49.000000 ara_cli-0.1.4.47/ara_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-26 19:59:49.000000 ara_cli-0.1.4.47/ara_cli.egg-info/requires.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-26 19:59:49.000000 ara_cli-0.1.4.47/ara_cli.egg-info/top_level.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-26 19:59:49.201013 ara_cli-0.1.4.47/setup.cfg
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-18 17:21:46.000000 ara_cli-0.1.4.47/setup.py
```

### Comparing `ara_cli-0.1.4.46/README.md` & `ara_cli-0.1.4.47/README.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/__main__.py` & `ara_cli-0.1.4.47/ara_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/ara_config.py` & `ara_cli-0.1.4.47/ara_cli/ara_config.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/artefact.py` & `ara_cli-0.1.4.47/ara_cli/artefact.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/artefact_creator.py` & `ara_cli-0.1.4.47/ara_cli/artefact_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/artefact_deleter.py` & `ara_cli-0.1.4.47/ara_cli/artefact_deleter.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/artefact_link_updater.py` & `ara_cli-0.1.4.47/ara_cli/artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/artefact_lister.py` & `ara_cli-0.1.4.47/ara_cli/artefact_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/artefact_renamer.py` & `ara_cli-0.1.4.47/ara_cli/artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/chat.py` & `ara_cli-0.1.4.47/ara_cli/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from os import sys
 from ara_cli.prompt_handler import send_prompt
 
 class Chat:
     def __init__(self, chat_name):
         self.chat_name = self.setup_chat(chat_name)
         self.chat_history = []
 
@@ -11,15 +12,15 @@
             return self.handle_existing_chat(chat_name)
         if chat_name == "chat" and os.path.exists("chat.md"):
             return self.handle_existing_chat("chat.md")
         return self.initialize_new_chat(chat_name)
 
     def handle_existing_chat(self, chat_name):
         if not os.path.exists(chat_name):
-            print("Couldn't continue existing chat. Provided chat file doesn't exist in this directory.")
+            print(f"Given chat file {chat_name} does not exist. Provide an existing chat file or create a new chat with its chat name only 'ara chat <chat_name>'. A file extension is not needed for a chat file!")
             sys.exit(1)
         self.chat_history = self.load_chat_history(chat_name)
         print(f"Reloaded {chat_name} content:")
         return chat_name
 
     def initialize_new_chat(self, chat_name):
         if chat_name != "chat":
```

### Comparing `ara_cli-0.1.4.46/ara_cli/classifier.py` & `ara_cli-0.1.4.47/ara_cli/classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/directory_navigator.py` & `ara_cli-0.1.4.47/ara_cli/directory_navigator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/file_classifier.py` & `ara_cli-0.1.4.47/ara_cli/file_classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/file_lister.py` & `ara_cli-0.1.4.47/ara_cli/file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/prompt_chat.py` & `ara_cli-0.1.4.47/ara_cli/prompt_chat.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/prompt_extractor.py` & `ara_cli-0.1.4.47/ara_cli/prompt_extractor.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/prompt_handler.py` & `ara_cli-0.1.4.47/ara_cli/prompt_handler.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/prompt_rag.py` & `ara_cli-0.1.4.47/ara_cli/prompt_rag.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/run_file_lister.py` & `ara_cli-0.1.4.47/ara_cli/run_file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/template_manager.py` & `ara_cli-0.1.4.47/ara_cli/template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/agile.artefacts` & `ara_cli-0.1.4.47/ara_cli/templates/agile.artefacts`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_businessgoal.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_capability.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_epic.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_feature.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_keyfeature.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_task.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_userstory.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_vision.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/commands/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_businessgoal.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_capability.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_epic.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_feature.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_keyfeature.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_task.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_userstory.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_vision.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-creation/rules/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/empty_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/empty_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/error_fixing_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/error_fixing_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/feature_file_update_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/feature_file_update_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/refactoring_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rename.py` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rename.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/gherkin_expert_rules.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/gherkin_expert_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/product_owner_rules.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/product_owner_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md` & `ara_cli-0.1.4.47/ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.concept.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.customer.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.persona.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.step.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.step.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.technology.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md` & `ara_cli-0.1.4.47/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.businessgoal` & `ara_cli-0.1.4.47/ara_cli/templates/template.businessgoal`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.capability` & `ara_cli-0.1.4.47/ara_cli/templates/template.capability`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.epic` & `ara_cli-0.1.4.47/ara_cli/templates/template.epic`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.feature` & `ara_cli-0.1.4.47/ara_cli/templates/template.feature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.issue` & `ara_cli-0.1.4.47/ara_cli/templates/template.issue`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.keyfeature` & `ara_cli-0.1.4.47/ara_cli/templates/template.keyfeature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.userstory` & `ara_cli-0.1.4.47/ara_cli/templates/template.userstory`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/templates/template.vision` & `ara_cli-0.1.4.47/ara_cli/templates/template.vision`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/tests/test_artefact_link_updater.py` & `ara_cli-0.1.4.47/ara_cli/tests/test_artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/tests/test_artefact_renamer.py` & `ara_cli-0.1.4.47/ara_cli/tests/test_artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/tests/test_file_creator.py` & `ara_cli-0.1.4.47/ara_cli/tests/test_file_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/tests/test_template_manager.py` & `ara_cli-0.1.4.47/ara_cli/tests/test_template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli/update_config_prompt.py` & `ara_cli-0.1.4.47/ara_cli/update_config_prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,10 +65,15 @@
     
     updated_content2 = update_items_in_file(content2, checked_items)
     
     write_file(input2, updated_content2)
     
     # Overwrite input1 with input2 and delete input2
     os.replace(input2, input1)
-    os.remove(input2)
-    
+
+    # Ensure the tmp file exists before attempting to delete
+    if os.path.exists(input2):
+        os.remove(input2)
+        print(f"Debug: Deleted temporary file {input2}")
+    else:
+        print(f"Debug: Temporary file {input2} does not exist")
     print("Update process completed.")
```

### Comparing `ara_cli-0.1.4.46/ara_cli/vectorDB.py` & `ara_cli-0.1.4.47/ara_cli/vectorDB.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/ara_cli.egg-info/SOURCES.txt` & `ara_cli-0.1.4.47/ara_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.46/setup.py` & `ara_cli-0.1.4.47/setup.py`

 * *Files identical despite different names*

