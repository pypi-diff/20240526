# Comparing `tmp/fermo_core-0.1.1.tar.gz` & `tmp/fermo_core-0.2.0.tar.gz`

## Comparing `fermo_core-0.1.1.tar` & `fermo_core-0.2.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fermo_core-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/__init__.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/__init__.py
--rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/class_default_settings.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/class_logger.py
--rw-r--r--   0        0        0    43465 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/__init__.py
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/class_analysis_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/__init__.py
--rw-r--r--   0        0        0    51559 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/blank_assigner/__init__.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/chrom_trace_calculator/__init__.py
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/feature_filter/__init__.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/feature_filter/class_feature_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_assigner/__init__.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_assigner/class_group_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_factor_assigner/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/__init__.py
--rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py
--rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/score_assigner/__init__.py
--rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/score_assigner/class_score_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/__init__.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py
--rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/__init__.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/class_repository.py
--rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/class_stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/__init__.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_feature_builder.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_general_feature_director.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_specific_feature_director.py
--rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/dataclass_feature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/__init__.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_sample_builder.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_samples_director.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/dataclass_sample.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/__init__.py
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/class_general_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/group_metadata_parser/__init__.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/msms_parser/__init__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/phenotype_parser/__init__.py
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/spec_library_parser/__init__.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/__init__.py
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/additional_module_parameter_managers.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_argparse_manager.py
--rw-r--r--   0        0        0    21122 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_export_manager.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_file_manager.py
--rw-r--r--   0        0        0    37024 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_parameter_manager.py
--rw-r--r--   0        0        0    20289 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_summary_writer.py
--rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_validation_manager.py
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/core_module_parameter_managers.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/input_file_parameter_managers.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/output_file_parameter_managers.py
--rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_bio_pos.csv
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_neg.csv
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_pos.csv
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_glycosides.csv
--rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_ribosomal.csv
--rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/mibig/mibig_cds_count.csv
--rw-r--r--   0        0        0  2878179 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/ms2deepscore/pos/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/ms2query/neg/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/ms2query/pos/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/utils/__init__.py
--rw-r--r--   0        0        0    12500 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/utils/utility_method_manager.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 fermo_core-0.1.1/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fermo_core-0.1.1/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 fermo_core-0.1.1/README.md
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fermo_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 fermo_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 fermo_core-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/__init__.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/config/__init__.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/config/class_default_settings.py
+-rw-r--r--   0        0        0    42886 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/config/schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/__init__.py
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/class_analysis_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/__init__.py
+-rw-r--r--   0        0        0    51559 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py
+-rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/blank_assigner/__init__.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/chrom_trace_calculator/__init__.py
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/feature_filter/__init__.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/feature_filter/class_feature_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_assigner/__init__.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_assigner/class_group_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_factor_assigner/__init__.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/__init__.py
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/score_assigner/__init__.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/score_assigner/class_score_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/__init__.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py
+-rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/class_repository.py
+-rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/class_stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/__init__.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_feature_builder.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_general_feature_director.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_specific_feature_director.py
+-rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_feature/dataclass_feature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/__init__.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_sample_builder.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_samples_director.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/builder_sample/dataclass_sample.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/__init__.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/class_general_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/group_metadata_parser/__init__.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/msms_parser/__init__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/phenotype_parser/__init__.py
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/spec_library_parser/__init__.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/__init__.py
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/additional_module_parameter_managers.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_argparse_manager.py
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_export_manager.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_file_manager.py
+-rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_parameter_manager.py
+-rw-r--r--   0        0        0    20145 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_summary_writer.py
+-rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/class_validation_manager.py
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/core_module_parameter_managers.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/input_file_parameter_managers.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/input_output/output_file_parameter_managers.py
+-rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_bio_pos.csv
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_neg.csv
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_pos.csv
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_glycosides.csv
+-rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_ribosomal.csv
+-rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/mibig/mibig_cds_count.csv
+-rw-r--r--   0        0        0  2878179 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/ms2deepscore/pos/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/ms2query/neg/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/libraries/ms2query/pos/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/utils/__init__.py
+-rw-r--r--   0        0        0    12500 2020-02-02 00:00:00.000000 fermo_core-0.2.0/fermo_core/utils/utility_method_manager.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 fermo_core-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fermo_core-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 fermo_core-0.2.0/README.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fermo_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 fermo_core-0.2.0/PKG-INFO
```

### Comparing `fermo_core-0.1.1/fermo_core/config/class_default_settings.py` & `fermo_core-0.2.0/fermo_core/config/class_default_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Organizes certain hardcoded default settings for easier access.
 
-Copyright (c) 2022-2023 Mitja Maximilian Zdouc, PhD
+Copyright (c) 2022 to present Mitja Maximilian Zdouc, PhD
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fermo_core-0.1.1/fermo_core/config/schema.json` & `fermo_core-0.2.0/fermo_core/config/schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998263888888889%*

 * *Differences: {"'properties'": "{'files': {'properties': {delete: ['output']}}}"}*

```diff
@@ -670,28 +670,14 @@
                     "required": [
                         "filepath",
                         "format"
                     ],
                     "title": "(Optional): file containing information of MS/MS spectra of molecular features in peaktable.",
                     "type": "object"
                 },
-                "output": {
-                    "additionalProperties": false,
-                    "properties": {
-                        "directory_path": {
-                            "title": "Specifies the directory path. Absolute paths are preferred.",
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "directory_path"
-                    ],
-                    "title": "(Optional): fermo_core output location.",
-                    "type": "object"
-                },
                 "peaktable": {
                     "additionalProperties": false,
                     "properties": {
                         "filepath": {
                             "title": "Specifies the filepath. Absolute paths are preferred.",
                             "type": "string"
                         },
```

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/class_analysis_manager.py` & `fermo_core-0.2.0/fermo_core/data_analysis/class_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py` & `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py` & `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py` & `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py` & `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py` & `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py` & `fermo_core-0.2.0/fermo_core/utils/utility_method_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""Runs the ms2query library annotation module.
+"""Organize general utility functions that are not specific for any other classes.
 
-Copyright (c) 2024 Mitja Maximilian Zdouc, PhD
+Copyright (c) 2022-2023 Mitja Maximilian Zdouc, PhD
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -17,269 +17,300 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import contextlib
 import logging
-import os
+import re
+import urllib.error
+import urllib.request
 from pathlib import Path
-from typing import Optional, Self
+from typing import Self
+from urllib.parse import urlparse
 
-import func_timeout
+import matchms
 import pandas as pd
-from matchms.exporting import save_as_mgf
-from ms2query.ms2library import MS2Library, create_library_object_from_one_dir
-from ms2query.run_ms2query import run_complete_folder
-from ms2query.utils import SettingsRunMS2Query
 from pydantic import BaseModel
 
 from fermo_core.config.class_default_settings import DefaultPaths
-from fermo_core.data_processing.builder_feature.dataclass_feature import (
-    Annotations,
-    Match,
-)
-from fermo_core.data_processing.class_repository import Repository
-from fermo_core.input_output.class_parameter_manager import ParameterManager
-from fermo_core.utils.utility_method_manager import UtilityMethodManager
 
 logger = logging.getLogger("fermo_core")
 
 
-class MS2QueryAnnotator(BaseModel):
-    """Pydantic-based class to organize calling and logging of ms2query lib matching
+class UtilityMethodManager(BaseModel):
+    """Pydantic-based base class to organize general utility methods for subclasses."""
 
-    Attributes:
-        features: Repository object, holds "General Feature" objects
-        params: User-provided parameters
-        active_features: a set of active features
-        cutoff: a float between 0 and 1 indicating the minimum accepted score
-        queries: a list of Spectra for which to perform matching
-    """
-
-    features: Repository
-    params: ParameterManager
-    active_features: set
-    cutoff: float
-    queries: Optional[list] = None
+    def check_ms2deepscore_req(self: Self, polarity: str):
+        """Checks if files required for ms2query functionality are present
 
-    def return_features(self: Self) -> Repository:
-        """Return the modified Feature objects as Repository object
+        Attributes:
+            polarity: the mass spectrometry data polarity
 
-        Returns:
-            A Repository object with modified Feature objects
+        Raises:
+            RuntimeError: unexpected polarity (currently only positive mode supported)
         """
-        return self.features
+        if polarity == "positive":
+            file = urlparse(DefaultPaths().url_ms2deepscore_pos).path.split("/")[-1]
+            if not DefaultPaths().dirpath_ms2deepscore_pos.joinpath(file).exists():
+                self.download_file(
+                    url=DefaultPaths().url_ms2deepscore_pos,
+                    location=DefaultPaths().dirpath_ms2deepscore_pos.joinpath(file),
+                    timeout=600,
+                )
+        else:
+            RuntimeError(
+                "'UtilityMethodManager': the MS2DeepScore algorithm currently only "
+                "supports positive ionization mode mass spectrometry data - SKIP"
+            )
 
-    def prepare_queries(self: Self):
-        """Prepare a filtered list of query spectra for matching
+    def check_ms2query_req(self: Self, polarity: str):
+        """Checks if files required for ms2query functionality are present
 
-        Raise:
-            RuntimeError: no query spectra collected (empty list)
+        Attributes:
+            polarity: the mass spectrometry data polarity
         """
-        query_spectra = []
-
-        for f_id in self.active_features:
-            feature = self.features.get(f_id)
-            if feature.Spectrum is None or len(feature.Spectrum.peaks.mz) == 0:
-                logger.debug(
-                    f"'AnnotationManager/MS2QueryAnnotator': feature with id "
-                    f"'{feature.f_id}' has no associated MS2 spectrum - SKIP"
-                )
-                continue
-            else:
-                query_spectra.append(feature.Spectrum)
-
-        if len(query_spectra) != 0:
-            self.queries = query_spectra
-            return
+        if polarity == "positive":
+            for url in DefaultPaths().url_ms2query_pos:
+                file = urlparse(url).path.split("/")[-1]
+                if not DefaultPaths().dirpath_ms2query_pos.joinpath(file).exists():
+                    self.download_file(
+                        url=url,
+                        location=DefaultPaths().dirpath_ms2query_pos.joinpath(file),
+                        timeout=600,
+                    )
         else:
-            raise RuntimeError(
-                "'AnnotationManager/MS2QueryAnnotator': no query spectra qualify for "
-                "matching - SKIP"
-            )
+            for url in DefaultPaths().url_ms2query_neg:
+                file = urlparse(url).path.split("/")[-1]
+                if not DefaultPaths().dirpath_ms2query_neg.joinpath(file).exists():
+                    self.download_file(
+                        url=url,
+                        location=DefaultPaths().dirpath_ms2query_neg.joinpath(file),
+                        timeout=600,
+                    )
 
-    def estimate_calc_time(self: Self):
-        """Estimates the approximate calculation time and aborts if set time too low
+    @staticmethod
+    def download_file(url: str, location: Path, timeout: int):
+        """Downloads from given URL into the designated location.
+
+        Arguments:
+            url: A URL string to download from
+            location: A Path pointing towards the designated file location
+            timeout: A timeout for the download
 
         Raises:
-            RuntimeError: no query spectra collected (None) or runtime too short
+            URLError: states the URL from where download failed
+
+        Notes:
+            `urlretrieve` considered legacy, therefore not used
         """
-        if self.queries is None:
-            raise RuntimeError(
-                "'AnnotationManager/MS2QueryAnnotator': 'self.queries' is None."
-                "Did you run 'self.prepare_queries()'?"
+        logger.info(
+            f"'UtilityMethodManager': attempt to download file from "
+            f"'{url}' to location '{location}' with a timeout of '{timeout}' seconds."
+        )
+        try:
+            with (
+                urllib.request.urlopen(url=url, timeout=timeout) as response,
+                open(location, "wb") as out,
+            ):
+                data = response.read()
+                out.write(data)
+            logger.info(
+                f"'UtilityMethodManager': successfully downloaded file from "
+                f"'{url}' to location '{location}'."
             )
-
-        if self.params.Ms2QueryAnnotationParameters.maximum_runtime != 0 and (
-            (len(self.queries) * 2.5)
-            > self.params.Ms2QueryAnnotationParameters.maximum_runtime
-        ):
-            raise RuntimeError(
-                f"'AnnotationManager/MS2QueryAnnotator': Estimated runtime of "
-                f"MS2Query for the "
-                f"annotation of "
-                f"'{len(self.queries)}' features is '{len(self.queries) * 2.5}' "
-                f"seconds. This exceeds the maximum allowed runtime of "
-                f"'{self.params.Ms2QueryAnnotationParameters.maximum_runtime}' "
-                f"seconds. Please increase the 'max_runtime' parameter or set to "
-                f"'0' for unlimited runtime - SKIP"
+        except urllib.error.URLError as e:
+            logger.error(
+                f"'UtilityMethodManager': could not download from url '{url}' - SKIP"
             )
+            raise e
 
     @staticmethod
-    def create_ms2query_dirs():
-        """Create ms2query helper directories"""
-        if not DefaultPaths().dirpath_ms2query_base.joinpath("queries").exists():
-            os.mkdir(DefaultPaths().dirpath_ms2query_base.joinpath("queries"))
+    def create_spectrum_object(data: dict, intensity_from: float) -> matchms.Spectrum:
+        """Create matchms Spectrum, add neutral losses, normalize and filter intensity
 
-        if not DefaultPaths().dirpath_ms2query_base.joinpath("results").exists():
-            os.mkdir(DefaultPaths().dirpath_ms2query_base.joinpath("results"))
+        Arguments:
+            data: a dict containing data to create a matchms Spectrum object.
+            intensity_from: a float between 0 and 1 to filter for MS2 rel intensity
 
-    @staticmethod
-    def remove_ms2query_temp_files():
-        """Remove queries and results files to clean up before run"""
+        Returns:
+            A matchms Spectrum object
+        """
+        spectrum = matchms.Spectrum(
+            mz=data["mz"],
+            intensities=data["intens"],
+            metadata={"precursor_mz": data["precursor_mz"], "id": data["f_id"]},
+            metadata_harmonization=False,
+        )
+        spectrum = matchms.filtering.add_precursor_mz(spectrum)
 
-        with contextlib.suppress(FileNotFoundError):
-            os.remove(
-                DefaultPaths().dirpath_ms2query_base.joinpath("queries/f_queries.mgf")
-            )
+        frag_before = len(spectrum.peaks.mz)
+        spectrum = matchms.filtering.remove_peaks_around_precursor_mz(
+            spectrum_in=spectrum, mz_tolerance=10
+        )
+        logger.debug(
+            f"'UtilityMethodManager': feature id '{data['f_id']}': removed MS2 "
+            f"fragments 10 Da around precursor m/z. '{len(spectrum.peaks.mz)}' "
+            f"fragments remaining (before: '{frag_before}')."
+        )
 
-        with contextlib.suppress(FileNotFoundError):
-            os.remove(
-                DefaultPaths().dirpath_ms2query_base.joinpath("results/f_queries.csv")
+        spectrum = matchms.filtering.normalize_intensities(spectrum)
+        if intensity_from > 0.0:
+            frag_before = len(spectrum.peaks.mz)
+            spectrum = matchms.filtering.select_by_relative_intensity(
+                spectrum, intensity_from=intensity_from
+            )
+            frag_diff = frag_before - len(spectrum.peaks.mz)
+            logger.debug(
+                f"'UtilityMethodManager': feature id '{data['f_id']}': removed '"
+                f"MS2 fragments with relative intensity lower than '"
+                f"{intensity_from}': {frag_diff}'. '{len(spectrum.peaks.mz)}' "
+                f"fragments remaining (before: '{frag_before}')."
             )
 
-    def assign_feature_info(self: Self, results_path: str | Path):
-        """Load ms2query results and add annotation to Feature objects
+        spectrum = matchms.filtering.add_losses(spectrum)
+
+        return spectrum
+
+    @staticmethod
+    def mass_deviation(m1: float, m2: float, f_id_m2: int | str) -> float:
+        """Calculate mass deviation in ppm between m1 and m2
 
         Arguments:
-            results_path: location of the ms2query results file
-        """
-        df = pd.read_csv(results_path)
-        df.fillna("unknown", inplace=True)
+            m1: an m/z ratio
+            m2: an m/z ratio
+            f_id_m2: the (feature) id of m2 for error reporting
 
-        for _, row in df.iterrows():
-            if int(row["id"]) not in self.active_features:
-                logger.debug(
-                    f"'AnnotationManager/MS2QueryAnnotator': in MS2Query results, "
-                    f"feature with ID "
-                    f"'{row['id']}' is not part of set of currently active features. "
-                    f"This feature might have been filtered out due to fermo_core "
-                    f"filter settings. Alternatively, the wrong MS2Query results file "
-                    f"was provided - SKIP"
-                )
-                continue
-            else:
-                if float(row["ms2query_model_prediction"]) >= self.cutoff:
-                    feature = self.features.get(int(row["id"]))
-
-                    if feature.Annotations is None:
-                        feature.Annotations = Annotations()
-                    if feature.Annotations.matches is None:
-                        feature.Annotations.matches = []
-
-                    feature.Annotations.matches.append(
-                        Match(
-                            id=row["analog_compound_name"],
-                            library="ms2query",
-                            algorithm="ms2query",
-                            score=float(row["ms2query_model_prediction"]),
-                            mz=float(row["precursor_mz_analog"]),
-                            diff_mz=float(row["precursor_mz_difference"]),
-                            module="ms2query_annotation",
-                            smiles=str(row["smiles"]),
-                            inchikey=str(row["inchikey"]),
-                            npc_class=str(row["npc_class_results"]),
-                        )
-                    )
-                    self.features.modify(int(row["id"]), feature)
+        Returns:
+            The mass deviation in ppm
 
-    def start_ms2query_algorithm(self: Self, library: MS2Library):
-        """Run ms2query algorithm with given library and timeout
+        Raises:
+            ZeroDivisionError: m2 is zero
+
+        Notes:
+            Taken from publication doi.org/10.1016/j.jasms.2010.06.006
+        """
+        try:
+            return abs(((m1 - m2) / m2) * 10**6)
+        except ZeroDivisionError as e:
+            logger.error(
+                f"'UtilityMethodManager': Division through zero in mass deviation "
+                f"calculation. Feature with id '{f_id_m2}' has a mass of '{m2}' - SKIP"
+            )
+            raise e
+
+    @staticmethod
+    def extract_as_kcb_results(as_results: Path, cutoff: float) -> dict:
+        """Extract MIBiG IDs from antiSMASH full results folder
 
         Arguments:
-            library: the generated MS2Library in positive or negative mode
+            as_results: a path pointing towards the antiSMASH results folder
+            cutoff: the coverage cutoff value to restrict spurious hits
+
+        Returns:
+            A dict of regions with detected MIBiG knownclusterblast matches
 
         Raises:
-            func_timeout.FunctionTimedOut
+            NotADirectoryError: the knownclusterblast directory was not found
         """
-        settings = SettingsRunMS2Query(additional_metadata_columns=("id",))
 
-        if self.params.Ms2QueryAnnotationParameters.maximum_runtime == 0:
-            logger.info(
-                "'AnnotationManager/MS2QueryAnnotator': Started MS2Query algorithm "
-                "with no timeout set."
+        def _extract_bgcs(content) -> list:
+            return re.findall(r"BGC\d{7}", content)
+
+        df_cds = pd.read_csv(
+            DefaultPaths().library_mibig_pos.parent.parent.joinpath(
+                "mibig_cds_count.csv"
             )
-            run_complete_folder(
-                ms2library=library,
-                folder_with_spectra=DefaultPaths().dirpath_ms2query_base.joinpath(
-                    "queries"
-                ),
-                results_folder=DefaultPaths().dirpath_ms2query_base.joinpath("results"),
-                settings=settings,
+        )
+
+        if not as_results.joinpath("knownclusterblast").is_dir():
+            raise NotADirectoryError(
+                f"'UtilityMethodManager': could not find the directory "
+                f"'knownclusterblast' in the antiSMASH result folder "
+                f"'{as_results.resolve()}' - SKIP"
             )
-        else:
-            try:
-                logger.info(
-                    f"'AnnotationManager/MS2QueryAnnotator': Started MS2Query "
-                    f"algorithm with a timeout "
-                    f"of '{self.params.Ms2QueryAnnotationParameters.maximum_runtime}' "
-                    f"seconds."
-                )
-                func_timeout.func_timeout(
-                    timeout=self.params.Ms2QueryAnnotationParameters.maximum_runtime,
-                    func=run_complete_folder,
-                    kwargs={
-                        "ms2library": library,
-                        "folder_with_spectra": DefaultPaths().dirpath_ms2query_base.joinpath(
-                            "queries"
-                        ),
-                        "results_folder": DefaultPaths().dirpath_ms2query_base.joinpath(
-                            "results"
-                        ),
-                        "settings": settings,
-                    },
-                )
-            except func_timeout.FunctionTimedOut as e:
-                logger.warning(
-                    f"'AnnotationManager/MS2QueryAnnotator': timeout of "
-                    f"MS2Query-based calculation:"
-                    f"took longer than maximum set time of '"
-                    f"{self.params.Ms2QueryAnnotationParameters.maximum_runtime}'. "
-                    f"seconds. For unlimited runtime, "
-                    f"set 'maximum_runtime' parameter to 0 (zero) - SKIP"
-                )
-                raise e
 
-    def run_ms2query(self: Self):
-        """Prepare dump/load locations and annotate features with ms2query"""
+        bgcs = {}
+        for f_path in as_results.joinpath("knownclusterblast").iterdir():
+            if f_path.is_file() and f_path.suffix == ".txt":
+                with open(f_path) as f_handle:
+                    data = f_handle.read()
+
+                    if len(_extract_bgcs(data)) == 0:
+                        logger.debug(
+                            f"'UtilityMethodManager': no significant "
+                            f"KnownClusterBlast matches for region '{f_path.stem}' - "
+                            f"SKIP"
+                        )
+                        continue
 
-        self.prepare_queries()
-        self.estimate_calc_time()
-        UtilityMethodManager().check_ms2query_req(
-            self.params.PeaktableParameters.polarity
-        )
-        self.create_ms2query_dirs()
-        self.remove_ms2query_temp_files()
-        save_as_mgf(
-            spectrums=self.queries,
-            filename=DefaultPaths().dirpath_ms2query_base.joinpath(
-                "queries/f_queries.mgf"
-            ),
-        )
+                    entries = data.split(">>")[1:]
+                    for entry in entries:
+                        bgc_id = _extract_bgcs(entry)[0]
+                        hits = entry.split(
+                            "Table of Blast hits (query gene, subject gene, %identity,"
+                            " blast score, %coverage, e-value):"
+                        )[1:][0].split("\n")
+                        nr_hits = len([item for item in hits if item != ""])
+                        cds_bgc = df_cds.loc[
+                            df_cds["mibig_id"] == bgc_id, "nr_cds"
+                        ].values[0]
+                        if (bgc_sim := round((nr_hits / cds_bgc), 2)) >= cutoff:
+                            if bgc_sim > 1.0:
+                                bgc_sim = 1.0
+                            try:
+                                if bgcs[bgc_id]["bgc_sim"] < bgc_sim:
+                                    bgcs[bgc_id] = {
+                                        "bgc_nr_cds": cds_bgc,
+                                        "matched_cds": nr_hits,
+                                        "bgc_sim": bgc_sim * 100,
+                                        "region": f_path.stem,
+                                    }
+                            except KeyError:
+                                bgcs[bgc_id] = {
+                                    "bgc_nr_cds": cds_bgc,
+                                    "matched_cds": nr_hits,
+                                    "bgc_sim": bgc_sim * 100,
+                                    "region": f_path.stem,
+                                }
 
-        if self.params.PeaktableParameters.polarity == "positive":
-            ms2library = create_library_object_from_one_dir(
-                DefaultPaths().dirpath_ms2query_pos
-            )
-            self.start_ms2query_algorithm(ms2library)
+        if len(bgcs) != 0:
+            return bgcs
         else:
-            ms2library = create_library_object_from_one_dir(
-                DefaultPaths().dirpath_ms2query_neg
+            raise RuntimeError(
+                "'UtilityMethodManager': could not find significant BGC matches in "
+                "antiSMASH KnownClusterBlast results."
             )
-            self.start_ms2query_algorithm(ms2library)
 
-        self.assign_feature_info(
-            DefaultPaths().dirpath_ms2query_base.joinpath("results/f_queries.csv")
+    @staticmethod
+    def create_mibig_spec_lib(mibig_ids: set) -> list[matchms.Spectrum]:
+        """Load MIBiG-derived in silico spectral library.
+
+        Attributes:
+            mibig_ids: A set of MIBiG IDs to create a targeted spectral library
+
+        Returns:
+            The spectral library
+
+        Raises:
+            RuntimeError: empty spectral library
+        """
+        spectra = list(
+            matchms.importing.load_from_mgf(DefaultPaths().library_mibig_pos)
         )
+        spectra = [matchms.filtering.add_precursor_mz(i) for i in spectra]
+        spectra = [matchms.filtering.normalize_intensities(i) for i in spectra]
+
+        filtered_spectra = []
+        for spectrum in spectra:
+            ids = set(spectrum.metadata.get("mibigaccession").split(","))
+            if not mibig_ids.isdisjoint(ids):
+                filtered_spectra.append(spectrum)
+
+        if len(filtered_spectra) != 0:
+            return filtered_spectra
+        else:
+            raise RuntimeError(
+                "'UtilityMethodManager': MIBiG spectral library construction: "
+                "spectral library empty - SKIP."
+            )
```

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py` & `fermo_core-0.2.0/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py` & `fermo_core-0.2.0/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/feature_filter/class_feature_filter.py` & `fermo_core-0.2.0/fermo_core/data_analysis/feature_filter/class_feature_filter.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/group_assigner/class_group_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/group_assigner/class_group_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py` & `fermo_core-0.2.0/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/score_assigner/class_score_assigner.py` & `fermo_core-0.2.0/fermo_core/data_analysis/score_assigner/class_score_assigner.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,19 +79,15 @@
                 feature.Annotations is not None
                 and feature.Annotations.matches is not None
                 and len(feature.Annotations.matches) != 0
             ):
                 annot_scores = [match.score for match in feature.Annotations.matches]
                 feature.Scores.novelty = 1 - max(annot_scores)
 
-            if feature.Scores.phenotype is None and feature.Scores.novelty is None:
-                feature.Scores = None
-                continue
-            else:
-                self.features.modify(f_id, feature)
+            self.features.modify(f_id, feature)
 
     def collect_sample_spec_networks(self: Self):
         """Collect sample:set of network ids for each used algorithm
 
         Raises:
             RuntimeError: no networks detected
         """
```

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py` & `fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py` & `fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py` & `fermo_core-0.2.0/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/class_repository.py` & `fermo_core-0.2.0/fermo_core/data_processing/class_repository.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/class_stats.py` & `fermo_core-0.2.0/fermo_core/data_processing/class_stats.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_feature_builder.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_feature_builder.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_general_feature_director.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_general_feature_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_specific_feature_director.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/class_specific_feature_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/dataclass_feature.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_feature/dataclass_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
     novelty: Optional[float] = None
 
     def to_json(self) -> dict:
         return {
             "phenotype": (
                 round(self.phenotype, 2) if self.phenotype is not None else 0.0
             ),
-            "novelty": round(self.novelty, 2) if self.novelty is not None else 0.0,
+            "novelty": round(self.novelty, 2) if self.novelty is not None else 1.0,
         }
 
 
 class Feature(BaseModel):
     """A Pydantic-based class to represent a molecular feature.
 
     Attributes:
```

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_sample_builder.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_sample_builder.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_samples_director.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_sample/class_samples_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/builder_sample/dataclass_sample.py` & `fermo_core-0.2.0/fermo_core/data_processing/builder_sample/dataclass_sample.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/class_general_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/class_general_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py` & `fermo_core-0.2.0/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/additional_module_parameter_managers.py` & `fermo_core-0.2.0/fermo_core/input_output/additional_module_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/class_argparse_manager.py` & `fermo_core-0.2.0/fermo_core/input_output/class_argparse_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/class_export_manager.py` & `fermo_core-0.2.0/fermo_core/input_output/class_export_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 """
 
 import json
 import logging
 import platform
 import shutil
 from datetime import datetime
-from pathlib import Path
-from typing import Any, Optional, Self
+from typing import Any, Self
 
 import networkx as nx
 import pandas as pd
-from pydantic import BaseModel, model_validator
+from pydantic import BaseModel
 
 from fermo_core.config.class_default_settings import DefaultPaths
 from fermo_core.data_processing.class_repository import Repository
 from fermo_core.data_processing.class_stats import Stats
 from fermo_core.input_output.class_parameter_manager import ParameterManager
 from fermo_core.input_output.class_summary_writer import SummaryWriter
 from fermo_core.input_output.class_validation_manager import ValidationManager
@@ -382,27 +381,20 @@
     """A Pydantic-based class managing data export.
 
     Attributes:
         params: a Parameter object with specified user parameters
         stats: a Stats object containing general information
         features: a Repository object containing feature and general information
         samples: a Repository object containing sample information
-        filename_base: the export filename derived from peaktable
     """
 
     params: ParameterManager
     stats: Stats
     features: Repository
     samples: Repository
-    filename_base: Optional[str] = None
-
-    @model_validator(mode="after")
-    def define_filename_base(self):
-        self.filename_base = f"out_{self.params.PeaktableParameters.filepath.stem}"
-        return self
 
     @staticmethod
     def log_start_module(file: str):
         """Log the start of the export of the corresponding file"""
         logger.debug(f"'ExportManager': started export of '{file}'.")
 
     @staticmethod
@@ -427,16 +419,16 @@
             version=version,
             starttime=starttime,
         )
         json_exporter.build_json_dict()
         session = json_exporter.return_session()
 
         session_path = self.params.OutputParameters.directory_path.joinpath(
-            self.filename_base
-        ).with_suffix(".fermo.session.json")
+            "out.fermo.session.json"
+        )
 
         with open(session_path, "w", encoding="utf-8") as outfile:
             outfile.write(json.dumps(session, indent=2, ensure_ascii=False))
 
         ValidationManager().validate_output_created(session_path)
 
         self.log_complete_module("fermo.session.json")
@@ -452,93 +444,64 @@
             samples=self.samples,
             df=pd.read_csv(self.params.PeaktableParameters.filepath),
         )
         csv_exporter.build_csv_output()
         df_full, df_abbr = csv_exporter.return_dfs()
 
         path_df_full = self.params.OutputParameters.directory_path.joinpath(
-            self.filename_base
-        ).with_suffix(".fermo.full.csv")
+            "out.fermo.full.csv"
+        )
         path_df_abbr = self.params.OutputParameters.directory_path.joinpath(
-            self.filename_base
-        ).with_suffix(".fermo.abbrev.csv")
+            "out.fermo.abbrev.csv"
+        )
 
         df_full.to_csv(path_df_full, encoding="utf-8", index=False, sep=",")
         df_abbr.to_csv(path_df_abbr, encoding="utf-8", index=False, sep=",")
 
         ValidationManager().validate_output_created(path_df_full)
         ValidationManager().validate_output_created(path_df_abbr)
 
         self.log_complete_module("fermo.full.csv/fermo.abbrev.csv")
 
-    def write_raw_ms2query_results(self: Self):
-        """If raw MS2Query results exist, write to output directory"""
-        src = DefaultPaths().dirpath_ms2query_base.joinpath("results/f_queries.csv")
-        dst = self.params.OutputParameters.directory_path.joinpath(
-            self.filename_base
-        ).with_suffix(".ms2query_results.csv")
-
-        if src.exists():
-            self.log_start_module(".ms2query_results.csv")
-            shutil.move(src=src, dst=dst)
-            ValidationManager().validate_output_created(dst)
-            self.log_complete_module(".ms2query_results.csv")
-
     def write_cytoscape_output(self: Self):
-        """Write cytoscape output if networking was performed"""
+        """Write Cytoscape-compatible graphml output if networking was performed"""
 
         self.log_start_module(".graphml")
 
         if self.stats.networks is None:
             logger.warning(
                 "'ExportManager': no spectral similarity networks generated - SKIP"
             )
             return
 
         for network in self.stats.networks:
             path_graphml = self.params.OutputParameters.directory_path.joinpath(
-                self.filename_base
-            ).with_suffix(f".fermo.{network}.graphml")
+                f"out.fermo.{network}.graphml"
+            )
             nx.write_graphml(self.stats.networks[network].network, path_graphml)
             ValidationManager().validate_output_created(path_graphml)
 
-        self.log_complete_module(".graphml.json")
+        self.log_complete_module(".graphml")
 
     def write_summary_output(self: Self):
         """Write a human-readable summary of steps performed."""
         dst = self.params.OutputParameters.directory_path.joinpath(
-            self.filename_base
-        ).with_suffix(".summary.txt")
-
+            "out.fermo.summary.txt"
+        )
         self.log_start_module("summary.txt")
         summary_writer = SummaryWriter(params=self.params, destination=dst)
         summary_writer.assemble_summary()
         summary_writer.write_summary()
         ValidationManager().validate_output_created(dst)
         self.log_complete_module("summary.txt")
 
-    def write_log_output(self: Self):
-        """Copy the log into the user-specified results directory"""
-        src = Path(__file__).parent.parent.joinpath("fermo_core.log")
-        dst = self.params.OutputParameters.directory_path.joinpath(
-            self.filename_base
-        ).with_suffix(".log")
-
-        if src.exists():
-            self.log_start_module(".log")
-            shutil.copy(src=src, dst=dst)
-            ValidationManager().validate_output_created(dst)
-            self.log_complete_module(".log")
-
     def run(self: Self, version: str, starttime: datetime):
         """Call export methods based on user-input
 
         Arguments:
             version: a str indicating the currently running version of fermo_core
             starttime: the date and time at start of fermo_core processing
         """
         self.write_fermo_json(version, starttime)
         self.write_csv_output()
-        self.write_raw_ms2query_results()
         self.write_cytoscape_output()
         self.write_summary_output()
-        self.write_log_output()
```

### Comparing `fermo_core-0.1.1/fermo_core/input_output/class_file_manager.py` & `fermo_core-0.2.0/fermo_core/input_output/class_file_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/class_parameter_manager.py` & `fermo_core-0.2.0/fermo_core/input_output/class_parameter_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,29 +264,25 @@
             ),
             (
                 user_params.get("ms2query_results"),
                 self.assign_ms2query_results,
                 "ms2query_results",
             ),
             (user_params.get("as_results"), self.assign_as_results, "as_results"),
-            (user_params.get("output"), self.assign_output, "output"),
         )
 
         for module in modules:
             if (data := module[0]) is not None:
                 module[1](data)
             else:
-                match module[2]:
-                    case "output":
-                        self.log_default_values(module[2])
-                        self.OutputParameters.validate_output_dir(
-                            peaktable_dir=self.PeaktableParameters.filepath.parent
-                        )
-                    case _:
-                        self.log_skipped_modules(module[2])
+                self.log_skipped_modules(module[2])
+
+        self.OutputParameters.validate_output_dir(
+            peaktable_dir=self.PeaktableParameters.filepath.parent
+        )
 
     def assign_core_modules_parameters(self: Self, user_params: dict):
         """Assigns user-input on core modules to ParameterManager.
 
         Arguments:
             user_params: a json-derived dict with user input; jsonschema-controlled.
         """
@@ -575,36 +571,14 @@
                 "for 'as_results'."
             )
         except Exception as e:
             logger.warning(str(e))
             self.log_malformed_parameters_skip("as_results")
             self.AsResultsParameters = None
 
-    def assign_output(self: Self, user_params: dict):
-        """Assign output parameters to self.OutputParameters.
-
-        Parameters:
-            user_params: user-provided params, read from json file
-        """
-        try:
-            self.OutputParameters = OutputParameters(**user_params)
-            self.OutputParameters.validate_output_dir(
-                self.PeaktableParameters.filepath.parent
-            )
-            logger.info(
-                "'ParameterManager': validated and assigned parameters for 'output'."
-            )
-        except Exception as e:
-            logger.warning(str(e))
-            self.log_malformed_parameters_skip("output")
-            self.OutputParameters = OutputParameters()
-            self.OutputParameters.validate_output_dir(
-                self.PeaktableParameters.filepath.parent
-            )
-
     def assign_adduct_annotation(self: Self, user_params: dict):
         """Assign adduct_annotation parameters to self.AdductAnnotationParameters.
 
         Parameters:
             user_params: user-provided params, read from json file
         """
         try:
```

### Comparing `fermo_core-0.1.1/fermo_core/input_output/class_summary_writer.py` & `fermo_core-0.2.0/fermo_core/input_output/class_summary_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,25 +345,24 @@
                 f"and the maximum precursor m/z difference of "
                 f"'{self.params.AsKcbDeepscoreMatchingParams.max_precursor_mass_diff}"
                 f"' was not exceeded."
             )
 
     def assemble_summary(self: Self):
         """Call methods to assemble the summary file"""
-        logger.info("'SummaryWriter': Started writing analysis summary")
-        logger.debug("'SummaryWriter': Started summary files")
+        logger.debug("'SummaryWriter': Started summary: files")
         self.summarize_peaktableparameters()
         self.summarize_msmsparameters()
         self.summarize_phenotypeparameters()
         self.summarize_groupmetadataparameters()
         self.summarize_speclibparameters()
         self.summarize_ms2queryresultsparameters()
         self.summarize_asresultsparameters()
-        logger.debug("'SummaryWriter': Completed summary files")
-        logger.debug("'SummaryWriter': Started summary analysis modules")
+        logger.debug("'SummaryWriter': Completed summary: files")
+        logger.debug("'SummaryWriter': Started summary: analysis modules")
         self.summarize_featurefilteringparameters()
         self.summarize_adductannotationparameters()
         self.summarize_neutrallossparameters()
         self.summarize_fragmentannparameters()
         self.summarize_specsimnetworkcosineparameters()
         self.summarize_specsimnetworkdeepscoreparameters()
         self.summarize_blankassignmentparameters()
@@ -372,9 +371,8 @@
         self.summarize_phenoquantpercentassgnparams()
         self.summarize_phenoquantconcassgnparams()
         self.summarize_spectrallibmatchingcosineparameters()
         self.summarize_spectrallibmatchingdeepscoreparameters()
         self.summarize_ms2queryannotationparameters()
         self.summarize_askcbcosinematchingparams()
         self.summarize_askcbdeepscorematchingparams()
-        logger.debug("'SummaryWriter': Completed summary analysis modules")
-        logger.info("'SummaryWriter': Completed writing analysis summary")
+        logger.debug("'SummaryWriter': Completed summary: analysis modules")
```

### Comparing `fermo_core-0.1.1/fermo_core/input_output/class_validation_manager.py` & `fermo_core-0.2.0/fermo_core/input_output/class_validation_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/core_module_parameter_managers.py` & `fermo_core-0.2.0/fermo_core/input_output/core_module_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/input_file_parameter_managers.py` & `fermo_core-0.2.0/fermo_core/input_output/input_file_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/input_output/output_file_parameter_managers.py` & `fermo_core-0.2.0/fermo_core/input_output/output_file_parameter_managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,17 @@
                 self.directory_path.mkdir(exist_ok=True)
                 logger.warning(
                     f"'ParameterManager/OutputParameters': create the default output "
                     f"directory '{self.directory_path}'."
                 )
 
         if self.directory_path is None:
-            logger.warning(
-                f"'ParameterManager/OutputParameters': output directory not "
-                f"specified. Results will be written to "
+            logger.info(
+                f"'ParameterManager/OutputParameters': "
+                f"all results will be written to "
                 f"'{peaktable_dir.joinpath('results')}'."
             )
             _create_output_dir()
         elif not self.directory_path.exists():
             logger.warning(
                 f"'ParameterManager/OutputParameters': output directory "
                 f"'{self.directory_path}' "
```

### Comparing `fermo_core-0.1.1/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv` & `fermo_core-0.2.0/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_bio_pos.csv` & `fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_bio_pos.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_neg.csv` & `fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_neg.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_pos.csv` & `fermo_core-0.2.0/fermo_core/libraries/loss_libs/generic_other_pos.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_glycosides.csv` & `fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_glycosides.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv` & `fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_ribosomal.csv` & `fermo_core-0.2.0/fermo_core/libraries/loss_libs/kersten_ribosomal.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/mibig/mibig_cds_count.csv` & `fermo_core-0.2.0/fermo_core/libraries/mibig/mibig_cds_count.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf` & `fermo_core-0.2.0/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/.gitignore` & `fermo_core-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/LICENSE` & `fermo_core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/README.md` & `fermo_core-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.1/pyproject.toml` & `fermo_core-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fermo_core"
-version = "0.1.1"
+version = "0.2.0"
 description = "Data processing/analysis functionality of metabolomics dashboard FERMO"
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 license-files = { paths = ["LICENSE"] }
 authors = [
     { name = "Mitja M. Zdouc", email = "zdoucmm@gmail.com" }
 ]
```

### Comparing `fermo_core-0.1.1/PKG-INFO` & `fermo_core-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fermo_core
-Version: 0.1.1
+Version: 0.2.0
 Summary: Data processing/analysis functionality of metabolomics dashboard FERMO
 Project-URL: Website, https://fermo.bioinformatics.nl/
 Project-URL: Repository, https://github.com/mmzdouc/fermo_core
 Project-URL: Documentation, https://mmzdouc.github.io/fermo_docs/
 Author-email: "Mitja M. Zdouc" <zdoucmm@gmail.com>
 License-File: LICENSE
 Keywords: cheminformatics,genomics,metabolomics
```

