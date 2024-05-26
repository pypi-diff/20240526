# Comparing `tmp/cutseq-0.0.8.tar.gz` & `tmp/cutseq-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.8.tar", max compression
+gzip compressed data, was "cutseq-0.0.9.tar", max compression
```

## Comparing `cutseq-0.0.8.tar` & `cutseq-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      362 2024-04-22 03:42:10.759173 cutseq-0.0.8/README.md
--rw-r--r--   0        0        0    22238 2024-04-22 03:42:10.759173 cutseq-0.0.8/cutseq/run.py
--rw-r--r--   0        0        0    14395 2024-04-22 03:42:10.759173 cutseq-0.0.8/cutseq/run_cmd.py
--rw-r--r--   0        0        0      510 2024-04-22 03:42:10.759173 cutseq-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      362 2024-04-22 03:53:42.743787 cutseq-0.0.9/README.md
+-rw-r--r--   0        0        0    22420 2024-04-22 03:53:42.743787 cutseq-0.0.9/cutseq/run.py
+-rw-r--r--   0        0        0    14395 2024-04-22 03:53:42.743787 cutseq-0.0.9/cutseq/run_cmd.py
+-rw-r--r--   0        0        0      510 2024-04-22 03:53:42.743787 cutseq-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.9/PKG-INFO
```

### Comparing `cutseq-0.0.8/cutseq/run.py` & `cutseq-0.0.9/cutseq/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Renamer,
     SingleEndModifier,
     SuffixRemover,
     UnconditionalCutter,
 )
 from cutadapt.pipeline import PairedEndPipeline, SingleEndPipeline
 from cutadapt.predicates import Predicate, TooShort
-from cutadapt.report import Statistics
+from cutadapt.report import Statistics, minimal_report
 from cutadapt.runners import make_runner
 from cutadapt.steps import (
     PairedEndFilter,
     PairedEndSink,
     SingleEndFilter,
     SingleEndSink,
 )
@@ -296,14 +296,15 @@
             )
         steps.append(
             # -o
             SingleEndSink(outfiles.open_record_writer(output1, interleaved=False)),
         )
         pipeline = SingleEndPipeline(modifiers, steps)
         _stats = runner.run(pipeline, Progress(), outfiles)
+        print(minimal_report(_stats, time=None, gc_content=None), file=sys.stderr)
         # _ = stats.as_json()
     outfiles.close()
 
 
 def pipeline_paired(
     input1,
     input2,
@@ -491,20 +492,21 @@
             )
         steps.append(
             # -o ... -p ...
             PairedEndSink(outfiles.open_record_writer(output1, output2))
         )
         pipeline = PairedEndPipeline(modifiers, steps)
         _stats = runner.run(pipeline, Progress(), outfiles)
+        print(minimal_report(_stats, time=None, gc_content=None), file=sys.stderr)
         # _ = stats.as_json()
     outfiles.close()
 
 
 def run_cutseq(args):
-    barcode_config = BarcodeConfig(args.replace(" ", "").adapter_scheme.upper())
+    barcode_config = BarcodeConfig(args.adapter_scheme.replace(" ", "").upper())
     settings = CutadaptConfig()
     settings.rname_suffix = args.with_rname_suffix
     settings.ensure_inline_barcode = args.ensure_inline_barcode
     settings.trim_polyA = args.trim_polyA
     settings.threads = args.threads
     settings.min_length = args.min_length
     settings.dry_run = args.dry_run
```

### Comparing `cutseq-0.0.8/cutseq/run_cmd.py` & `cutseq-0.0.9/cutseq/run_cmd.py`

 * *Files identical despite different names*

### Comparing `cutseq-0.0.8/PKG-INFO` & `cutseq-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutseq
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automatically cut adapter / barcode / UMI from NGS data
 Home-page: https://github.com/y9c/cutseq
 License: MIT
 Keywords: bioinformatics,NGS,adapter,barcode,UMI
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
```

