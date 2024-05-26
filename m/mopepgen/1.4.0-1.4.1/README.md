# Comparing `tmp/mopepgen-1.4.0.tar.gz` & `tmp/mopepgen-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopepgen-1.4.0.tar", last modified: Mon Apr  8 18:52:57 2024, max compression
+gzip compressed data, was "mopepgen-1.4.1.tar", last modified: Sun May 26 18:29:12 2024, max compression
```

## Comparing `mopepgen-1.4.0.tar` & `mopepgen-1.4.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.690782 mopepgen-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-08 18:52:53.000000 mopepgen-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 18:52:53.000000 mopepgen-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-08 18:52:57.690782 mopepgen-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-08 18:52:53.000000 mopepgen-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.670782 mopepgen-1.4.0/moPepGen/
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/SeqFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.670782 mopepgen-1.4.0/moPepGen/aa/
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/AminoAcidSeqDict.py
--rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/AminoAcidSeqRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/PeptidePoolSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/PeptidePoolSummarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/VariantPeptideIdentifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/VariantPeptideLabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/VariantPeptidePool.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/aa/expasy_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.670782 mopepgen-1.4.0/moPepGen/circ/
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/circ/CircRNA.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/circ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/circ/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.674782 mopepgen-1.4.0/moPepGen/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/call_alt_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/call_novel_orf.py
--rw-r--r--   0 runner    (1001) docker     (127)    33522 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/call_variant_peptide.py
--rw-r--r--   0 runner    (1001) docker     (127)    13965 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/decoy_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/encode_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/filter_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/generate_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/index_gvf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/merge_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_arriba.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_circexplorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_fusion_catcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_reditools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_rmats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_star_fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/parse_vep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/split_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/summarize_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/cli/update_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.674782 mopepgen-1.4.0/moPepGen/data/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/data/gencode_hs_exclusion_list.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.674782 mopepgen-1.4.0/moPepGen/dna/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/dna/DNASeqDict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/dna/DNASeqRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/err.py
--rw-r--r--   0 runner    (1001) docker     (127)    35730 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.678782 mopepgen-1.4.0/moPepGen/gtf/
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GTFPointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GTFRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GTFSeqFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GTFSourceInferrer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GeneAnnotationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GenomicAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GenomicAnnotationOnDisk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/GtfIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/TranscriptAnnotationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/gtf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.678782 mopepgen-1.4.0/moPepGen/parser/
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/ArribaParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/CIRCexplorerParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/FusionCatcherParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/REDItoolsParser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.682782 mopepgen-1.4.0/moPepGen/parser/RMATSParser/
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/A3SSRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/A5SSRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/MXERecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/RIRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/RMATSRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/SERecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/RMATSParser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/STARFusionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/VEPParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.682782 mopepgen-1.4.0/moPepGen/seqvar/
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/GVFIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/GVFMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/GVFMetadataInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/SplicingJunction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/VariantRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/VariantRecordPool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/VariantRecordPoolOnDisk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/VariantRecordWithCoordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/seqvar/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.686782 mopepgen-1.4.0/moPepGen/svgraph/
--rw-r--r--   0 runner    (1001) docker     (127)    49558 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/PVGNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/PVGNodeCollapser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/PVGOrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    63207 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/PeptideVariantGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/SubgraphTree.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/TVGCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/TVGEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)    35241 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/TVGNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/TVGNodeCollapser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/ThreeFrameCVG.py
--rw-r--r--   0 runner    (1001) docker     (127)    85064 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/ThreeFrameTVG.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/VariantCombinations.py
--rw-r--r--   0 runner    (1001) docker     (127)    37766 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/VariantPeptideDict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/VariantPeptideTable.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/svgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.686782 mopepgen-1.4.0/moPepGen/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/ResourcesMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/add_fuzz_test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    57504 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/brute_force.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/brute_force_novel_orf.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/downsample_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/extract_gvf.py
--rw-r--r--   0 runner    (1001) docker     (127)    32497 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/fuzz_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/validate_novel_orf_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/util/validate_variant_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-08 18:52:53.000000 mopepgen-1.4.0/moPepGen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:52:57.690782 mopepgen-1.4.0/mopepgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-08 18:52:57.000000 mopepgen-1.4.0/mopepgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-08 18:52:57.000000 mopepgen-1.4.0/mopepgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:52:57.000000 mopepgen-1.4.0/mopepgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 18:52:57.000000 mopepgen-1.4.0/mopepgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 18:52:57.000000 mopepgen-1.4.0/mopepgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 18:52:57.000000 mopepgen-1.4.0/mopepgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 18:52:53.000000 mopepgen-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-08 18:52:57.690782 mopepgen-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:52:53.000000 mopepgen-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.405355 mopepgen-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-26 18:29:09.000000 mopepgen-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-26 18:29:09.000000 mopepgen-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-26 18:29:12.405355 mopepgen-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-26 18:29:09.000000 mopepgen-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.385355 mopepgen-1.4.1/moPepGen/
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/SeqFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.385355 mopepgen-1.4.1/moPepGen/aa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/AminoAcidSeqDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/AminoAcidSeqRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/PeptidePoolSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/PeptidePoolSummarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/VariantPeptideIdentifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/VariantPeptideLabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/VariantPeptidePool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/aa/expasy_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.389355 mopepgen-1.4.1/moPepGen/circ/
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/circ/CircRNA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/circ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/circ/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.393355 mopepgen-1.4.1/moPepGen/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/call_alt_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/call_novel_orf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33522 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/call_variant_peptide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13965 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/decoy_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/encode_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/filter_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/generate_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/index_gvf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/merge_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_arriba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_circexplorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_fusion_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_reditools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_rmats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_star_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/parse_vep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/split_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/summarize_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/cli/update_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.393355 mopepgen-1.4.1/moPepGen/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/data/gencode_hs_exclusion_list.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.393355 mopepgen-1.4.1/moPepGen/dna/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/dna/DNASeqDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/dna/DNASeqRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35730 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.393355 mopepgen-1.4.1/moPepGen/gtf/
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GTFPointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GTFRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GTFSeqFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GTFSourceInferrer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GeneAnnotationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GenomicAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GenomicAnnotationOnDisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/GtfIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17134 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/TranscriptAnnotationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/gtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.397355 mopepgen-1.4.1/moPepGen/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/ArribaParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/CIRCexplorerParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/FusionCatcherParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/REDItoolsParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.397355 mopepgen-1.4.1/moPepGen/parser/RMATSParser/
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/A3SSRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/A5SSRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/MXERecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/RIRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/RMATSRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/SERecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/RMATSParser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/STARFusionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/VEPParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.397355 mopepgen-1.4.1/moPepGen/seqvar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/GVFIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/GVFMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/GVFMetadataInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/SplicingJunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/VariantRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/VariantRecordPool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/VariantRecordPoolOnDisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/VariantRecordWithCoordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/seqvar/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.401355 mopepgen-1.4.1/moPepGen/svgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)    49558 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/PVGNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/PVGNodeCollapser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/PVGOrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63207 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/PeptideVariantGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/SubgraphTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/TVGCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/TVGEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35241 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/TVGNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/TVGNodeCollapser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/ThreeFrameCVG.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85064 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/ThreeFrameTVG.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/VariantCombinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37766 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/VariantPeptideDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/VariantPeptideTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/svgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.405355 mopepgen-1.4.1/moPepGen/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/ResourcesMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/add_fuzz_test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57504 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/brute_force_novel_orf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/downsample_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/extract_gvf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32497 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/fuzz_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/validate_novel_orf_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/util/validate_variant_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-26 18:29:09.000000 mopepgen-1.4.1/moPepGen/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:29:12.405355 mopepgen-1.4.1/mopepgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-26 18:29:12.000000 mopepgen-1.4.1/mopepgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-26 18:29:12.000000 mopepgen-1.4.1/mopepgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:29:12.000000 mopepgen-1.4.1/mopepgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-26 18:29:12.000000 mopepgen-1.4.1/mopepgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 18:29:12.000000 mopepgen-1.4.1/mopepgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 18:29:12.000000 mopepgen-1.4.1/mopepgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 18:29:09.000000 mopepgen-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-26 18:29:12.405355 mopepgen-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 18:29:09.000000 mopepgen-1.4.1/setup.py
```

### Comparing `mopepgen-1.4.0/LICENSE.txt` & `mopepgen-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/PKG-INFO` & `mopepgen-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopepgen
-Version: 1.4.0
+Version: 1.4.1
 Summary: Multi-omic peptide generator
 Home-page: https://github.com/uclahs-cds/package-moPepGen
 Author: Chenghao Zhu, Yiyang Liu
 Author-email: ChenghaoZhu@mednet.ucla.edu, yiyangliu@mednet.ucla.edu
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/package-moPepGen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -19,29 +19,36 @@
 Requires-Dist: matplotlib
 Requires-Dist: regex
 
 # <u>M</u>ulti-<u>O</u>mics <u>Pep</u>tide <u>Gen</u>erator
 
 <!-- badges: start -->
 
-[![Lifecycle:Maturing](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)
+[![Lifecycle:Stable](https://img.shields.io/badge/Lifecycle-Stable-97ca00)](https://img.shields.io/badge/Lifecycle-Stable-97ca00)
 [![Tests](https://github.com/uclahs-cds/package-moPepGen/actions/workflows/tests.yaml/badge.svg)](https://github.com/uclahs-cds/package-moPepGen/actions/workflows/tests.yaml)
+![PyPI - Version](https://img.shields.io/pypi/v/mopepgen?logo=Python)
 [![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=plastic&logo=docker&logoColor=white)](https://github.com/uclahs-cds/package-moPepGen/pkgs/container/mopepgen)
 [![Documentation](https://img.shields.io/static/v1?style=plastic&message=ReadTheDocs&color=2C4AA8&logo=ReadTheDocs&logoColor=FFFFFF&label=Documentation)](https://uclahs-cds.github.io/package-moPepGen/)
 [![License](https://img.shields.io/badge/License-GPL_v2-blue)](./LICENSE.txt)
 [![DOI:10.1101/2024.03.28.587261](https://zenodo.org/badge/DOI/10.1101/2024.03.28.587261.svg)](https://doi.org/10.1101/2024.03.28.587261)
 
 <!-- badges: end -->
 
 moPepGen (multi-omics peptide generator) uses data from one or more omics experiments and calls variant peptides as custom databases for proteogenomic library search.
 
 moPepGen takes genomic and transcriptomic variants such as single nucleotide variants (SNPs or SNVs), small insertions/deletions (indels), gene fusion, alternative splicing, RNA circularization and RNA editing events, and generates noncanonical peptides affected by the variants.
 
 ## Installation
 
+Install from PyPI
+
+```shell
+pip install mopepgen
+```
+
 Install directly from GitHub
 
 ```shell
 pip install git+ssh://git@github.com/uclahs-cds/package-moPepGen.git
 ```
 
 ## Documentation
```

### Comparing `mopepgen-1.4.0/README.md` & `mopepgen-1.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # <u>M</u>ulti-<u>O</u>mics <u>Pep</u>tide <u>Gen</u>erator
 
 <!-- badges: start -->
 
-[![Lifecycle:Maturing](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)
+[![Lifecycle:Stable](https://img.shields.io/badge/Lifecycle-Stable-97ca00)](https://img.shields.io/badge/Lifecycle-Stable-97ca00)
 [![Tests](https://github.com/uclahs-cds/package-moPepGen/actions/workflows/tests.yaml/badge.svg)](https://github.com/uclahs-cds/package-moPepGen/actions/workflows/tests.yaml)
+![PyPI - Version](https://img.shields.io/pypi/v/mopepgen?logo=Python)
 [![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=plastic&logo=docker&logoColor=white)](https://github.com/uclahs-cds/package-moPepGen/pkgs/container/mopepgen)
 [![Documentation](https://img.shields.io/static/v1?style=plastic&message=ReadTheDocs&color=2C4AA8&logo=ReadTheDocs&logoColor=FFFFFF&label=Documentation)](https://uclahs-cds.github.io/package-moPepGen/)
 [![License](https://img.shields.io/badge/License-GPL_v2-blue)](./LICENSE.txt)
 [![DOI:10.1101/2024.03.28.587261](https://zenodo.org/badge/DOI/10.1101/2024.03.28.587261.svg)](https://doi.org/10.1101/2024.03.28.587261)
 
 <!-- badges: end -->
 
 moPepGen (multi-omics peptide generator) uses data from one or more omics experiments and calls variant peptides as custom databases for proteogenomic library search.
 
 moPepGen takes genomic and transcriptomic variants such as single nucleotide variants (SNPs or SNVs), small insertions/deletions (indels), gene fusion, alternative splicing, RNA circularization and RNA editing events, and generates noncanonical peptides affected by the variants.
 
 ## Installation
 
+Install from PyPI
+
+```shell
+pip install mopepgen
+```
+
 Install directly from GitHub
 
 ```shell
 pip install git+ssh://git@github.com/uclahs-cds/package-moPepGen.git
 ```
 
 ## Documentation
```

### Comparing `mopepgen-1.4.0/moPepGen/SeqFeature.py` & `mopepgen-1.4.1/moPepGen/SeqFeature.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/__init__.py` & `mopepgen-1.4.1/moPepGen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import hashlib
 import itertools
 from typing import Iterable, IO
 import logging
 from . import constant
 
 
-__version__ = '1.4.0'
+__version__ = '1.4.1'
 
 ## Error messages
 ERROR_INDEX_IN_INTRON = 'The genomic index seems to be in an intron'
 ERROR_NO_TX_AVAILABLE = 'No transcripts available'
 ERROR_VARIANT_NOT_IN_GENE_COORDINATE = 'Variant is not in gene coordinates.'
 ERROR_REF_LENGTH_NOT_MATCH_WITH_LOCATION = \
     'Length of ref does not match with the location.'
```

### Comparing `mopepgen-1.4.0/moPepGen/aa/AminoAcidSeqDict.py` & `mopepgen-1.4.1/moPepGen/aa/AminoAcidSeqDict.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/aa/AminoAcidSeqRecord.py` & `mopepgen-1.4.1/moPepGen/aa/AminoAcidSeqRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/aa/PeptidePoolSplitter.py` & `mopepgen-1.4.1/moPepGen/aa/PeptidePoolSplitter.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/aa/PeptidePoolSummarizer.py` & `mopepgen-1.4.1/moPepGen/aa/PeptidePoolSummarizer.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/aa/VariantPeptideIdentifier.py` & `mopepgen-1.4.1/moPepGen/aa/VariantPeptideIdentifier.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/aa/VariantPeptideLabel.py` & `mopepgen-1.4.1/moPepGen/aa/VariantPeptideLabel.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/aa/VariantPeptidePool.py` & `mopepgen-1.4.1/moPepGen/aa/VariantPeptidePool.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             cleavage_params (CleavageParams): cleavage parameters.
             skip_checking (bool): whether to skip checking cleavage parameters.
         """
         if not skip_checking:
             min_mw = cleavage_params.min_mw
             min_length = cleavage_params.min_length
             max_length = cleavage_params.max_length
-            if SeqUtils.molecular_weight(peptide, 'protein') < min_mw:
+            if SeqUtils.molecular_weight(peptide.seq, 'protein') < min_mw:
                 return False
-            if len(peptide.seq) < min_length or len(peptide) > max_length:
+            if len(peptide.seq) < min_length or len(peptide.seq) > max_length:
                 return False
             if str(peptide.seq) in canonical_peptides:
                 return False
         same_peptide = get_equivalent(self.peptides, peptide)
         if same_peptide:
             same_peptide:Seq
             new_label = peptide.description
```

### Comparing `mopepgen-1.4.0/moPepGen/aa/expasy_rules.py` & `mopepgen-1.4.1/moPepGen/aa/expasy_rules.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/circ/CircRNA.py` & `mopepgen-1.4.1/moPepGen/circ/CircRNA.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/circ/io.py` & `mopepgen-1.4.1/moPepGen/circ/io.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/__init__.py` & `mopepgen-1.4.1/moPepGen/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/__main__.py` & `mopepgen-1.4.1/moPepGen/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/call_alt_translation.py` & `mopepgen-1.4.1/moPepGen/cli/call_alt_translation.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/call_novel_orf.py` & `mopepgen-1.4.1/moPepGen/cli/call_novel_orf.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/call_variant_peptide.py` & `mopepgen-1.4.1/moPepGen/cli/call_variant_peptide.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/common.py` & `mopepgen-1.4.1/moPepGen/cli/common.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/decoy_fasta.py` & `mopepgen-1.4.1/moPepGen/cli/decoy_fasta.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/encode_fasta.py` & `mopepgen-1.4.1/moPepGen/cli/encode_fasta.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/filter_fasta.py` & `mopepgen-1.4.1/moPepGen/cli/filter_fasta.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/generate_index.py` & `mopepgen-1.4.1/moPepGen/cli/generate_index.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/index_gvf.py` & `mopepgen-1.4.1/moPepGen/cli/index_gvf.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/merge_fasta.py` & `mopepgen-1.4.1/moPepGen/cli/merge_fasta.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_arriba.py` & `mopepgen-1.4.1/moPepGen/cli/parse_arriba.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_circexplorer.py` & `mopepgen-1.4.1/moPepGen/cli/parse_circexplorer.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_fusion_catcher.py` & `mopepgen-1.4.1/moPepGen/cli/parse_fusion_catcher.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_reditools.py` & `mopepgen-1.4.1/moPepGen/cli/parse_reditools.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_rmats.py` & `mopepgen-1.4.1/moPepGen/cli/parse_rmats.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_star_fusion.py` & `mopepgen-1.4.1/moPepGen/cli/parse_star_fusion.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/parse_vep.py` & `mopepgen-1.4.1/moPepGen/cli/parse_vep.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/split_fasta.py` & `mopepgen-1.4.1/moPepGen/cli/split_fasta.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/summarize_fasta.py` & `mopepgen-1.4.1/moPepGen/cli/summarize_fasta.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/cli/update_index.py` & `mopepgen-1.4.1/moPepGen/cli/update_index.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/constant.py` & `mopepgen-1.4.1/moPepGen/constant.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/dna/DNASeqDict.py` & `mopepgen-1.4.1/moPepGen/dna/DNASeqDict.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/dna/DNASeqRecord.py` & `mopepgen-1.4.1/moPepGen/dna/DNASeqRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/err.py` & `mopepgen-1.4.1/moPepGen/err.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/fake.py` & `mopepgen-1.4.1/moPepGen/fake.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GTFPointer.py` & `mopepgen-1.4.1/moPepGen/gtf/GTFPointer.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GTFRecord.py` & `mopepgen-1.4.1/moPepGen/gtf/GTFRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GTFSeqFeature.py` & `mopepgen-1.4.1/moPepGen/gtf/GTFSeqFeature.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GTFSourceInferrer.py` & `mopepgen-1.4.1/moPepGen/gtf/GTFSourceInferrer.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GeneAnnotationModel.py` & `mopepgen-1.4.1/moPepGen/gtf/GeneAnnotationModel.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GenomicAnnotation.py` & `mopepgen-1.4.1/moPepGen/gtf/GenomicAnnotation.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GenomicAnnotationOnDisk.py` & `mopepgen-1.4.1/moPepGen/gtf/GenomicAnnotationOnDisk.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/GtfIO.py` & `mopepgen-1.4.1/moPepGen/gtf/GtfIO.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/gtf/TranscriptAnnotationModel.py` & `mopepgen-1.4.1/moPepGen/gtf/TranscriptAnnotationModel.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/index.py` & `mopepgen-1.4.1/moPepGen/index.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/params.py` & `mopepgen-1.4.1/moPepGen/params.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/ArribaParser.py` & `mopepgen-1.4.1/moPepGen/parser/ArribaParser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/CIRCexplorerParser.py` & `mopepgen-1.4.1/moPepGen/parser/CIRCexplorerParser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/FusionCatcherParser.py` & `mopepgen-1.4.1/moPepGen/parser/FusionCatcherParser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/REDItoolsParser.py` & `mopepgen-1.4.1/moPepGen/parser/REDItoolsParser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/A3SSRecord.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/A3SSRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/A5SSRecord.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/A5SSRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/MXERecord.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/MXERecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/RIRecord.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/RIRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/RMATSRecord.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/RMATSRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/SERecord.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/SERecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/RMATSParser/__init__.py` & `mopepgen-1.4.1/moPepGen/parser/RMATSParser/__init__.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/STARFusionParser.py` & `mopepgen-1.4.1/moPepGen/parser/STARFusionParser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/parser/VEPParser.py` & `mopepgen-1.4.1/moPepGen/parser/VEPParser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/GVFIndex.py` & `mopepgen-1.4.1/moPepGen/seqvar/GVFIndex.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/GVFMetadata.py` & `mopepgen-1.4.1/moPepGen/seqvar/GVFMetadata.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/GVFMetadataInfo.py` & `mopepgen-1.4.1/moPepGen/seqvar/GVFMetadataInfo.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/SplicingJunction.py` & `mopepgen-1.4.1/moPepGen/seqvar/SplicingJunction.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/VariantRecord.py` & `mopepgen-1.4.1/moPepGen/seqvar/VariantRecord.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/VariantRecordPool.py` & `mopepgen-1.4.1/moPepGen/seqvar/VariantRecordPool.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/VariantRecordPoolOnDisk.py` & `mopepgen-1.4.1/moPepGen/seqvar/VariantRecordPoolOnDisk.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/VariantRecordWithCoordinate.py` & `mopepgen-1.4.1/moPepGen/seqvar/VariantRecordWithCoordinate.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/__init__.py` & `mopepgen-1.4.1/moPepGen/seqvar/__init__.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/seqvar/io.py` & `mopepgen-1.4.1/moPepGen/seqvar/io.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/PVGNode.py` & `mopepgen-1.4.1/moPepGen/svgraph/PVGNode.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/PVGNodeCollapser.py` & `mopepgen-1.4.1/moPepGen/svgraph/PVGNodeCollapser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/PVGOrf.py` & `mopepgen-1.4.1/moPepGen/svgraph/PVGOrf.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/PeptideVariantGraph.py` & `mopepgen-1.4.1/moPepGen/svgraph/PeptideVariantGraph.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/SubgraphTree.py` & `mopepgen-1.4.1/moPepGen/svgraph/SubgraphTree.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/TVGEdge.py` & `mopepgen-1.4.1/moPepGen/svgraph/TVGEdge.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/TVGNode.py` & `mopepgen-1.4.1/moPepGen/svgraph/TVGNode.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/TVGNodeCollapser.py` & `mopepgen-1.4.1/moPepGen/svgraph/TVGNodeCollapser.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/ThreeFrameCVG.py` & `mopepgen-1.4.1/moPepGen/svgraph/ThreeFrameCVG.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/ThreeFrameTVG.py` & `mopepgen-1.4.1/moPepGen/svgraph/ThreeFrameTVG.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/VariantCombinations.py` & `mopepgen-1.4.1/moPepGen/svgraph/VariantCombinations.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/VariantPeptideDict.py` & `mopepgen-1.4.1/moPepGen/svgraph/VariantPeptideDict.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/svgraph/VariantPeptideTable.py` & `mopepgen-1.4.1/moPepGen/svgraph/VariantPeptideTable.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/ResourcesMonitor.py` & `mopepgen-1.4.1/moPepGen/util/ResourcesMonitor.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/__main__.py` & `mopepgen-1.4.1/moPepGen/util/__main__.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/add_fuzz_test_log.py` & `mopepgen-1.4.1/moPepGen/util/add_fuzz_test_log.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/brute_force.py` & `mopepgen-1.4.1/moPepGen/util/brute_force.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/brute_force_novel_orf.py` & `mopepgen-1.4.1/moPepGen/util/brute_force_novel_orf.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/common.py` & `mopepgen-1.4.1/moPepGen/util/common.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/downsample_reference.py` & `mopepgen-1.4.1/moPepGen/util/downsample_reference.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/extract_gvf.py` & `mopepgen-1.4.1/moPepGen/util/extract_gvf.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/fuzz_test.py` & `mopepgen-1.4.1/moPepGen/util/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/validate_novel_orf_calling.py` & `mopepgen-1.4.1/moPepGen/util/validate_novel_orf_calling.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/util/validate_variant_calling.py` & `mopepgen-1.4.1/moPepGen/util/validate_variant_calling.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/moPepGen/version.py` & `mopepgen-1.4.1/moPepGen/version.py`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/mopepgen.egg-info/PKG-INFO` & `mopepgen-1.4.1/mopepgen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mopepgen
-Version: 1.4.0
+Version: 1.4.1
 Summary: Multi-omic peptide generator
 Home-page: https://github.com/uclahs-cds/package-moPepGen
 Author: Chenghao Zhu, Yiyang Liu
 Author-email: ChenghaoZhu@mednet.ucla.edu, yiyangliu@mednet.ucla.edu
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/package-moPepGen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -19,29 +19,36 @@
 Requires-Dist: matplotlib
 Requires-Dist: regex
 
 # <u>M</u>ulti-<u>O</u>mics <u>Pep</u>tide <u>Gen</u>erator
 
 <!-- badges: start -->
 
-[![Lifecycle:Maturing](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)](https://img.shields.io/badge/Lifecycle-Maturing-007EC6)
+[![Lifecycle:Stable](https://img.shields.io/badge/Lifecycle-Stable-97ca00)](https://img.shields.io/badge/Lifecycle-Stable-97ca00)
 [![Tests](https://github.com/uclahs-cds/package-moPepGen/actions/workflows/tests.yaml/badge.svg)](https://github.com/uclahs-cds/package-moPepGen/actions/workflows/tests.yaml)
+![PyPI - Version](https://img.shields.io/pypi/v/mopepgen?logo=Python)
 [![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=plastic&logo=docker&logoColor=white)](https://github.com/uclahs-cds/package-moPepGen/pkgs/container/mopepgen)
 [![Documentation](https://img.shields.io/static/v1?style=plastic&message=ReadTheDocs&color=2C4AA8&logo=ReadTheDocs&logoColor=FFFFFF&label=Documentation)](https://uclahs-cds.github.io/package-moPepGen/)
 [![License](https://img.shields.io/badge/License-GPL_v2-blue)](./LICENSE.txt)
 [![DOI:10.1101/2024.03.28.587261](https://zenodo.org/badge/DOI/10.1101/2024.03.28.587261.svg)](https://doi.org/10.1101/2024.03.28.587261)
 
 <!-- badges: end -->
 
 moPepGen (multi-omics peptide generator) uses data from one or more omics experiments and calls variant peptides as custom databases for proteogenomic library search.
 
 moPepGen takes genomic and transcriptomic variants such as single nucleotide variants (SNPs or SNVs), small insertions/deletions (indels), gene fusion, alternative splicing, RNA circularization and RNA editing events, and generates noncanonical peptides affected by the variants.
 
 ## Installation
 
+Install from PyPI
+
+```shell
+pip install mopepgen
+```
+
 Install directly from GitHub
 
 ```shell
 pip install git+ssh://git@github.com/uclahs-cds/package-moPepGen.git
 ```
 
 ## Documentation
```

### Comparing `mopepgen-1.4.0/mopepgen.egg-info/SOURCES.txt` & `mopepgen-1.4.1/mopepgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopepgen-1.4.0/setup.cfg` & `mopepgen-1.4.1/setup.cfg`

 * *Files identical despite different names*

