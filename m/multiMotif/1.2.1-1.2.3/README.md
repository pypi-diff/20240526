# Comparing `tmp/multiMotif-1.2.1.tar.gz` & `tmp/multimotif-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiMotif-1.2.1.tar", last modified: Fri Apr  5 04:44:50 2024, max compression
+gzip compressed data, was "multimotif-1.2.3.tar", last modified: Sun May 26 14:59:56 2024, max compression
```

## Comparing `multiMotif-1.2.1.tar` & `multimotif-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:50.887712 multiMotif-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 04:44:41.000000 multiMotif-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-05 04:44:50.887712 multiMotif-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-05 04:44:41.000000 multiMotif-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:50.887712 multiMotif-1.2.1/multiMotif/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:41.000000 multiMotif-1.2.1/multiMotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71656 2024-04-05 04:44:41.000000 multiMotif-1.2.1/multiMotif/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:50.887712 multiMotif-1.2.1/multiMotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:44:50.887712 multiMotif-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 04:44:41.000000 multiMotif-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:59:56.719779 multimotif-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 14:59:47.000000 multimotif-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-26 14:59:56.719779 multimotif-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-26 14:59:47.000000 multimotif-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:59:56.715778 multimotif-1.2.3/multiMotif/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:59:47.000000 multimotif-1.2.3/multiMotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75630 2024-05-26 14:59:47.000000 multimotif-1.2.3/multiMotif/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:59:56.719779 multimotif-1.2.3/multiMotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-26 14:59:56.000000 multimotif-1.2.3/multiMotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-26 14:59:56.000000 multimotif-1.2.3/multiMotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:59:56.000000 multimotif-1.2.3/multiMotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 14:59:56.000000 multimotif-1.2.3/multiMotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 14:59:56.000000 multimotif-1.2.3/multiMotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 14:59:56.000000 multimotif-1.2.3/multiMotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:59:56.719779 multimotif-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-26 14:59:47.000000 multimotif-1.2.3/setup.py
```

### Comparing `multiMotif-1.2.1/LICENSE` & `multimotif-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multiMotif-1.2.1/multiMotif/main.py` & `multimotif-1.2.3/multiMotif/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 import numpy as np
 import pandas as pd
 from Bio.SeqRecord import SeqRecord
 from Bio import SeqIO
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
+import logging
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
 def get_singleMotif_args(parser):
     single = parser.add_argument_group("Option for single motif scanning")
     single.add_argument('-f', '--fasta', type=str, help='Input FASTA file containing sequences for motif scanning')
     single.add_argument('-motif', type=str, help='Input motif sequences')
     single.add_argument('-m', '--mismatches', default=0, type=int, help='Maximum allowed mismatches motif scanning. Default is 0')
     single.add_argument('-d', '--direction', type=str, default='+', choices=['+,-', '+', '-'], help='Search direction: both, forward (default), or reverse')
     single.add_argument('-o', '--output_dir', type=str, help='Output directory for result files')
@@ -79,15 +83,15 @@
     parser.add_argument("-up", "--upstream", dest="upstream", type=int, default=400, help="For the promoter option: specify the upstream length from gene start location (optional, default is 400)")
     parser.add_argument("-down", "--downstream", dest="downstream", type=int, default=0, help="For promoter option: specify the downstream length from gene start location  (optional, default is 0)")
     parser.add_argument("--promoter", dest="promoter", action="store_true", help="Extract promoter sequences")
     parser.add_argument("--orf", dest="orf", action="store_true", help="Extract ORF sequences")
     parser.add_argument('-o', '--output', type=str, help='Output sequence file')
 
 def get_args():
-    parser = argparse.ArgumentParser(description='VariaMotif for motif scanning')
+    parser = argparse.ArgumentParser(description='multiMotif for motif scanning')
     subparsers = parser.add_subparsers(help='sub-command help')
 
     singleMotif_parser = subparsers.add_parser('singleMotif', help='Scanning for single motif')
     get_singleMotif_args(singleMotif_parser)
     singleMotif_parser.set_defaults(func=singleMotif_function)
 
     multiMotif_parser = subparsers.add_parser('multiMotif', help='Scanning more than two ordered motifs')
@@ -106,45 +110,50 @@
 
     if hasattr(args, 'func'):
         args.func(args)
     else:
         parser.print_help()
 
 def singleMotif_function(args):
+    logging.info("Starting the singleMotif module.")
     fasta_file_path = args.fasta
     output_dir = args.output_dir
     all_results = []
     filtered_results = []
     motif = args.motif
     max_mismatches = args.mismatches
     direction = args.direction
     output_file_path1 = f"{output_dir}/single.out"
     pool = multiprocessing.Pool(multiprocessing.cpu_count())
     records = list(SeqIO.parse(fasta_file_path, "fasta"))
     if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 500000:
+        logging.info("Starting single motif scanning on DNA or RNA records(calculate_average_length>=500000).")
         if direction == '+' or direction == '+,-':  
             motif_results_pre = process_genome_file_forward(fasta_file_path, motif, max_mismatches)
             all_results.extend(motif_results_pre)
         if direction == '-' or direction == '+,-':  
             motif_results_pre = process_genome_file_reverse(fasta_file_path, motif, max_mismatches)
             all_results.extend(motif_results_pre)
         all_results = sorted(all_results, key=lambda x: (x['sequence_id'], x['start']))
 
         seen_positions = set()
         unique_positions = set()
         for result in all_results:
             key = (result['sequence_id'], result['start'])
             if key not in seen_positions and result['strand'] == '+':
                 seen_positions.add(key)
+                result['motif_type'] = "singleMotif"
                 filtered_results.append(result)
             elif key not in seen_positions:
                 unique_positions.add(key)
+                result['motif_type'] = "singleMotif"
                 filtered_results.append(result)
 
     if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
+        logging.info("Starting single motif scanning on DNA or RNA records(calculate_average_length<500000).")
         if direction == '+' or direction == '+,-':
             motif_results = pool.starmap(search_motif, [(record, motif, max_mismatches, len(motif)) for record in records])
             motif_results = [item for sublist in motif_results for item in sublist]
             all_results.extend(motif_results)
         if direction == '-' or direction == '+,-':
             motif_results = pool.starmap(reverse_search_fix, [(record, motif, max_mismatches, len(motif)) for record in records])
             motif_results = [item for sublist in motif_results for item in sublist]
@@ -153,38 +162,48 @@
 
         seen_positions = set()
         unique_positions = set()
         for result in all_results:
             key = (result['sequence_id'], result['start'])           
             if key not in seen_positions and result['strand'] == '+':
                 seen_positions.add(key)
+                result['motif_type'] = "singleMotif"
                 filtered_results.append(result)
+
             elif key not in seen_positions:
                 unique_positions.add(key)
+                result['motif_type'] = "singleMotif"
                 filtered_results.append(result)
 
+
     if args.protein:
+        logging.info("Starting single motif scanning on protein records.")
         motif_results = pool.starmap(search_motif_protein, [(record, motif, max_mismatches, len(motif)) for record in records])
         motif_results = [item for sublist in motif_results for item in sublist]
+        for result in motif_results:
+            result['motif_type'] = "singleMotif"
         filtered_results.extend(motif_results)
         filtered_results = sorted(filtered_results, key=lambda x: (x['sequence_id'], x['start']))
     if not filtered_results:
-        print("#No Result")
+        logging.info("Single motif scanning found no results.")
     else:
         with open(output_file_path1,'w') as output_file:
-            output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\n")
+            output_file.write("Sequence_ID\tSequence_Length\tmotif\tmotif_type\tstart\tend\tstrand\tmismatches\tmatched_sequence\n")
             for result in filtered_results:
                 result['motif']=f"single_{result['motif']}"
-                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\n")
+                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['motif_type']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\n")
+        logging.info("Single motif scanning is completed.")
     if args.image:
+        logging.info("Starting to visualize single motif scanning results.")
         plot_motifs_to_single_chart(output_file_path1, output_file_path1, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
     fimo_results=[]
     fimo_results_filter=[]
     if args.fimo_path:
+        logging.info("Receiving the result file from FIMO execution.")
         output_file_path2 = f"{output_dir}/fimo.out"
         records = list(SeqIO.parse(fasta_file_path, "fasta"))
         file_path=args.fimo_path
         data=[]
         with open(file_path,'r',newline='',encoding='utf-8') as file:
             reader=csv.DictReader(file, delimiter='\t')
             for row in reader:
@@ -218,28 +237,29 @@
 
         seen_positions = set()
         unique_positions = set()
         for result in fimo_results:
             key = (result['sequence_id'], result['start'])           
             if key not in seen_positions and result['strand'] == '+':
                 seen_positions.add(key)
+                result['motif_type'] = "FIMO"
                 fimo_results_filter.append(result)
             elif key not in seen_positions:
                 unique_positions.add(key)
+                result['motif_type'] = "FIMO"
                 fimo_results_filter.append(result)
 
-        if not fimo_results_filter:
-            print("#No Result")
-        else:
-            with open(output_file_path2,'w') as output_file:
-                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tp-value\tq-value\tmatched_sequence\n")
-                for result in fimo_results_filter:
-                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['p-value']}\t{result['q-value']}\t{result['fragment']}\n")
+        with open(output_file_path2,'w') as output_file:
+            output_file.write("Sequence_ID\tSequence_Length\tmotif\tmotif_type\tstart\tend\tstrand\tp-value\tq-value\tmatched_sequence\n")
+            for result in fimo_results_filter:
+                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['motif_type']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['p-value']}\t{result['q-value']}\t{result['fragment']}\n")
+        logging.info("Starting to visualize FIMO results.")
         plot_motifs_to_single_chart(output_file_path2, output_file_path2, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
+        logging.info("Starting comparison of singleMotif results and FIMO results.")
         output_file_path3 = f"{output_dir}/merge.out"
         merged_results = []
         seen_keys = set()
         for result in filtered_results:
             key = f"{result['sequence_id']}_{result['sequence_length']}_{result['start']}_{result['end']}_{result['strand']}"
             if key not in seen_keys:
                 seen_keys.add(key)
@@ -248,39 +268,45 @@
             key = f"{result['sequence_id']}_{result['sequence_length']}_{result['start']}_{result['end']}_{result['strand']}"
             if key not in seen_keys:
                 seen_keys.add(key)
                 merged_results.append(result)
             elif key in seen_keys:
                 for merged_result in merged_results:
                     if all(str(merged_result[k]) == str(result[k]) for k in ('sequence_id', 'sequence_length', 'start', 'end', 'strand')):
-                        merged_result['motif'] = merged_result['motif'].replace('single', 'both')
+                        merged_result['motif'] = merged_result['motif'].replace('singleMotif', 'Both')
+                        merged_result['motif_type'] = merged_result['motif_type'].replace('singleMotif', 'Both')
+
 
         with open(output_file_path3,'w') as output_file:
-            output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\n")
+            output_file.write("Sequence_ID\tSequence_Length\tmotif\tmotif_type\tstart\tend\tstrand\n")
             for result in merged_results:
-                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\n")
+                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['motif_type']}\t{result['start']}\t{result['end']}\t{result['strand']}\n")
+        logging.info("Starting to visualize the comparison results between singleMotif and FIMO.")
         plot_motifs_to_single_chart(output_file_path3, output_file_path3, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
+    logging.info("Done")
 
 def multiMotif_function(args):
+    logging.info("Starting the multiMotif module.")
     if not args.regulator:
         fasta_file_path = args.fasta
         motiflist = args.motiflist
         direction = args.direction
         output_dir = args.output_dir
         n=args.mis_motif_nums
         pool = multiprocessing.Pool(multiprocessing.cpu_count())
         records = list(SeqIO.parse(fasta_file_path, "fasta"))
         all_results = []
         motif_results_pre = []
         output_file_path1 = f"{output_dir}/multiMotifs_list.out"
-        output_file_path2 = f"{output_dir}/multiMotifs_statistics.out"    
+        output_file_path2 = f"{output_dir}/multiMotifs_statistics.out"
 
         with open(motiflist, 'r') as file:
             line_count = sum(1 for line in file)
         if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 500000:
+            logging.info("Starting multiple motifs scanning on DNA or RNA records(calculate_average_length>=500000).")
             with open(motiflist, 'r') as file:
                 for line_number, line in enumerate(file, start=1):
                     motif = line.strip().split('\t')[0]
                     max_mismatches = int(line.strip().split('\t')[1])
                     if direction == '+' or direction == '+,-':  
                         motif_results_pre = process_genome_file_forward(fasta_file_path, motif, max_mismatches)
                         for result in motif_results_pre:
@@ -290,14 +316,15 @@
                         motif_results_pre = process_genome_file_reverse(fasta_file_path, motif, max_mismatches)
                         for result in motif_results_pre:
                             result['motif_type'] = line_number
                         all_results.extend(motif_results_pre)
             all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
 
         if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
+            logging.info("Starting multiple motifs scanning on DNA or RNA records(calculate_average_length<500000).")
             with open(motiflist, 'r') as file:
                 for line_number, line in enumerate(file, start=1):
                     motif = line.strip().split('\t')[0]
                     max_mismatches = int(line.strip().split('\t')[1])
                     if direction == '+' or direction == '+,-':
                         motif_results = pool.starmap(search_motif, [(record, motif, max_mismatches, len(motif)) for record in records])
                         motif_results = [item for sublist in motif_results for item in sublist]
@@ -308,31 +335,33 @@
                         motif_results = pool.starmap(reverse_search_fix, [(record, motif, max_mismatches, len(motif)) for record in records])
                         motif_results = [item for sublist in motif_results for item in sublist]
                         for result in motif_results:
                             result['motif_type'] = line_number
                         all_results.extend(motif_results)
             all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
         if args.protein:
+            logging.info("Starting multiple motifs scanning on protein records.")
             with open(motiflist, 'r') as file:
                 for line_number, line in enumerate(file, start=1):
                     motif = line.strip().split('\t')[0]
                     max_mismatches = int(line.strip().split('\t')[1])
                     motif_results = pool.starmap(search_motif_protein, [(record, motif, max_mismatches, len(motif)) for record in records])
                     motif_results = [item for sublist in motif_results for item in sublist]
                     for result in motif_results:
                         result['motif_type'] = line_number
                     all_results.extend(motif_results)
             all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
         if not all_results:
-            print("#No Result")
+            logging.info("Multiple motifs scanning found no results.")
         else:
             with open(output_file_path1,'w') as output_file:
-                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\tmotif_type\n")
+                output_file.write("Sequence_ID\tSequence_Length\tmotif\tmotif_type\tstart\tend\tstrand\tmismatches\tmatched_sequence\n")
                 for result in all_results:
-                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\t{result['motif_type']}\n")
+                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['motif_type']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\n")
+            logging.info("Multiple motifs scanning is completed.")
 
         filtered_results = []
         seen_positions = set()
         unique_positions = set()
 
         for result in all_results:
             key = (result['sequence_id'], result['start'], result['motif_type'])
@@ -340,38 +369,42 @@
             if key not in seen_positions and result['strand'] == '+':
                 seen_positions.add(key)
                 filtered_results.append(result)
             elif key not in seen_positions:
                 unique_positions.add(key)
                 filtered_results.append(result)
 
+        logging.info("Checking the positional order of multiple types motif scanning results and conducting additional checks as requested by the user.")
         motif_nums = line_count - n
         manyMotifs_results = []
 
         filtered_results_sorted = sorted(filtered_results, key=lambda x: (x['sequence_id'],x['start']))
         grouped_results = groupby(filtered_results_sorted, key=lambda x: x['sequence_id'])
         grouped_results_list = [(key,list(group)) for key, group in grouped_results]
         manyMotifs_results_pre1 = pool.starmap(filter_rows, [(group, motif_nums,line_count,args.necessary) for key, group in grouped_results_list])
         manyMotifs_results_pre2 = [item for sublist in manyMotifs_results_pre1 if sublist is not None for item in sublist]    
         manyMotifs_results.extend(manyMotifs_results_pre2)
         manyMotifs_results= [item for sublist in manyMotifs_results if sublist is not None for item in sublist]
         manyMotifs_results = sorted(manyMotifs_results, key=lambda x: x['sequence_id'])
         
         if not manyMotifs_results:
-            print("#No Result")
+            logging.info("After the positional order check, no results met the criteria.")
         else:
             with open(output_file_path2,'w') as output_file:
-                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\tmotif_type\n")
+                output_file.write("Sequence_ID\tSequence_Length\tmotif\tmotif_type\tstart\tend\tstrand\tmismatches\tmatched_sequence\n")
                 for result in manyMotifs_results:
-                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\t{result['motif_type']}\n")
+                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['motif_type']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\n")
+            logging.info("Positional order check is completed.")
 
         if args.image:
+            logging.info("Starting to visualize multiple motifs scanning results.")
             plot_motifs_to_single_chart(output_file_path2, output_file_path2, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
     if args.regulator:
+        logging.info("Starting variable gap motifs scanning.")
         motiflist = args.motiflist
         with open(motiflist, 'r') as file:
             lines = file.readlines()
         motif1,max_mismatch1_str = lines[0].strip().split('\t')
         motif2,max_mismatch2_str = lines[1].strip().split('\t')
         max_mismatch1 = int(max_mismatch1_str) if max_mismatch1_str else 0 
         max_mismatch2 = int(max_mismatch2_str) if max_mismatch2_str else 0 
@@ -389,71 +422,89 @@
         if args.mismatches is None:
             args.mismatches = max_mismatch1 + max_mismatch2
             max_mismatches = args.mismatches
         else:
             max_mismatches = args.mismatches
 
         if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 500000:
+            logging.info("Starting variable gap motifs scanning on DNA or RNA records(calculate_average_length>=500000).")
             if direction == '+' or direction == '+,-':  
                 motif1_results_pre = process_genome_file_forward(fasta_file_path, motif1, max_mismatch1)
                 motif1_results = sorted(motif1_results_pre, key=lambda x: (x['sequence_id'], x['start']))
                 motif2_results_pre = process_genome_file_forward(fasta_file_path, motif2, max_mismatch2)
                 motif2_results = sorted(motif2_results_pre, key=lambda x: (x['sequence_id'], x['start']))
                 num_chunks = multiprocessing.cpu_count()
                 chunk_size = max(len(motif1_results) // num_chunks,1)
                 chunks = [motif1_results[i:i + chunk_size] for i in range(0, len(motif1_results), chunk_size)]
                     
                 for record in records:
                     combined_results = pool.starmap(combine_results_forward, [(record, motif1_results_chunk, motif2_results, max_mismatches, min_gap, max_gap) for motif1_results_chunk in chunks])
                     combined_results = [item for sublist in combined_results for item in sublist]
+                    for result in combined_results:
+                        result['motif_type'] = "variable_gap_motifs"
                     all_results.extend(combined_results)		                   
             if direction == '-' or direction == '+,-':  
                 motif1_results_pre = process_genome_file_reverse(fasta_file_path, motif1, max_mismatch1)
                 motif1_results = sorted(motif1_results_pre, key=lambda x: (x['sequence_id'], x['start']))
                 motif2_results_pre = process_genome_file_reverse(fasta_file_path, motif2, max_mismatch2)
                 motif2_results = sorted(motif2_results_pre, key=lambda x: (x['sequence_id'], x['start']))
                 num_chunks = multiprocessing.cpu_count()
                 chunk_size = max(len(motif1_results) // num_chunks,1)
                 chunks = [motif1_results[i:i + chunk_size] for i in range(0, len(motif1_results), chunk_size)]             
                 for record in records:
                     combined_results = pool.starmap(combine_results_reverse, [(record, motif1_results_chunk, motif2_results, max_mismatches, min_gap, max_gap) for motif1_results_chunk in chunks])
                     combined_results = [item for sublist in combined_results for item in sublist]
+                    for result in combined_results:
+                        result['motif_type'] = "variable_gap_motifs"
                     all_results.extend(combined_results)
         if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
+            logging.info("Starting variable gap motifs scanning on DNA or RNA records(calculate_average_length<500000).")
             if direction == '+' or direction == '+,-':
                 combined_results = pool.starmap(process_record_DNA_forward, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
                 combined_results = [item for sublist in combined_results for item in sublist]
+                for result in combined_results:
+                    result['motif_type'] = "variable_gap_motifs"
                 all_results.extend(combined_results)
             if direction == '-' or direction == '+,-':
                 combined_results = pool.starmap(process_record_DNA_reverse, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
                 combined_results = [item for sublist in combined_results for item in sublist]
+                for result in combined_results:
+                    result['motif_type'] = "variable_gap_motifs"
                 all_results.extend(combined_results)
         if args.protein:
             combined_results = pool.starmap(process_record_protein, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
             combined_results = [item for sublist in combined_results for item in sublist]
+            for result in combined_results:
+                result['motif_type'] = "variable_gap_motifs"
             all_results.extend(combined_results)
         if not all_results:
-            print("# No Result")
+            logging.info("Variable gap motifs scannin found no results.")
         else:
             with open(output_file_path, 'w') as output_file:
-                output_file.write("Sequence_ID\tSequence_Length\tMotif\tstart\tend\tstrand\tmotif1_mismatch\tfragment1\tmotif2_mismatch\tfragment2\tmismatches\tgap_length\tmatched_sequence\n")
+                output_file.write("Sequence_ID\tSequence_Length\tMotif\tmotif_type\tstart\tend\tstrand\tmotif1_mismatch\tfragment1\tmotif2_mismatch\tfragment2\tmismatches\tgap_length\tmatched_sequence\n")
                 for result in all_results:
-                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['motif1_mismatch']}\t{result['fragment1']}\t{result['motif2_mismatch']}\t{result['fragment2']}\t{result['mismatch']}\t{result['gap_length']}\t{result['sequence']}\n")
+                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['motif_type']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['motif1_mismatch']}\t{result['fragment1']}\t{result['motif2_mismatch']}\t{result['fragment2']}\t{result['mismatch']}\t{result['gap_length']}\t{result['sequence']}\n")
         if args.image:
+            logging.info("Starting to visualize variable gap motifs scanning results.")
             plot_motifs_to_single_chart(output_file_path, output_file_path, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
+    logging.info("Done")
 
 def visualMotif_function(args):
+    logging.info("Starting the visualMotif module.")
     output_dir = args.output_dir    
     output_file_path = f"{output_dir}/visualization"
     gff_file = args.gff
     motif_up = args.motif_up
     motif_down = args.motif_down
+    logging.info("Starting visualization.")
     plot_motifs_to_single_chart(args.table_file, output_file_path, args.display_both_directions, gff_file, motif_up, motif_down)
+    logging.info("Done")
 
 def extract_sequences_function(args):
+    logging.info("Starting the extract_sequences module.")
     if args.output is None:
         raise ValueError("Output file path is required.")
     sequences = SeqIO.to_dict(SeqIO.parse(args.fna, "fasta"))
 
     output_handle = open(args.output, "w")
 
     with open(args.gff, "r") as gff_handle:
@@ -496,16 +547,16 @@
                             seq_fragment = sequence[seq_start - 1:seq_end].reverse_complement()
                         else:
                             seq_fragment = sequence[seq_start - 1:seq_end]
                     else:
                         continue
                     seq_record = SeqRecord(seq_fragment, id=f"{seq_name}|{cds_id}|{parent}|{gene}|{seq_start}|{seq_end}|{strand}|{product}",description="")
                     SeqIO.write(seq_record, output_handle, "fasta")
-    # Close output file
     output_handle.close()
+    logging.info("Done")
 
 def generate_motif_variants(motif):
     variant_bases = []
     ambiguous_bases = {
         'W': 'AT',
         'S': 'GC',
         'M': 'AC',
@@ -863,15 +914,15 @@
         if nums[i] == sorted_nums[count]:
             ordered_nums.append((nums[i], i))
             processed_nums.add(nums[i])
             count += 1
             i+=1
 
         elif nums[i] != sorted_nums[count]:
-            if sorted_nums[count] not in nums[i:]: 
+            if sorted_nums[count] not in nums[i:]:
                 count += 1
             else:
                 for x in range(i, len(nums)):
                     if nums[x] == sorted_nums[count]:
                         if x-i >=m and len(ordered_nums)+len(sorted_nums)-1-count >=m:
                             count+=1
                         else:
@@ -891,14 +942,15 @@
         return None
 
     temp = []
     lists = []
     i = 0
 
     filtered_rows = []
+
     num_list = []
     num_list_add=[]
     nums=[]
     sorted_nums =[]
 
     count_positive_strand = 0
     count_negative_strand = 0
@@ -906,15 +958,15 @@
         if item['strand'] == '+':
             count_positive_strand += 1  
         else:
             count_negative_strand += 1
     if count_positive_strand > count_negative_strand:
         while i < len(result_list) -1:
             temp.append((result_list[i], i))
-            if result_list[i]['motif_type'] >= result_list[i + 1]['motif_type']:
+            if result_list[i]['motif_type'] >= result_list[i + 1]['motif_type'] or result_list[i+1]['start'] - result_list[i]['end'] > (result_list[i + 1]['motif_type'] - result_list[i]['motif_type'])*1000:  #一旦motif类型不是增长，就结束这个小列表
                 lists.append(temp)
                 temp = []
             i += 1
 
         if i == len(result_list) - 1:
             temp.append((result_list[i], i))
             lists.append(temp)
@@ -931,43 +983,42 @@
                     f_start=1
                 else:
                     for sub_list in lists:
                         if sub_list[0][0]["start"] <= up_value <= sub_list[-1][0]['end']:
                             f_start=sub_list[0][1]
                             break
                         elif up_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and up_value > lists[lists.index(sub_list)-1][-1][0]['end']:
-                            f_start=lists[lists.index(sub_list)-1][0][1]
+                            f_start=sub_list[0][1]
                             break
             else:
                 f_start = sublist[0][1]
             if sublist[-1][0]['motif_type'] < line_count:
                 down = ((int(line_count - sublist[-1][0]['motif_type'])) // 3 + 1) * 1000
                 down_value = sublist[-1][0]['end'] + down
                 if down_value > result_list[-1]['end']:
                     g_end = len(result_list)-1
                 else:
                     for sub_list in lists:
                         if sub_list[0][0]["start"] <= down_value <= sub_list[-1][0]['end']:
                             g_end =sub_list[-1][1]
                             break
                         elif down_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and down_value > lists[lists.index(sub_list)-1][-1][0]['end']:
-                            g_end =sub_list[-1][1]
+                            g_end =lists[lists.index(sub_list)-1][-1][1]
                             break
             else:
                 g_end = sublist[-1][1]
 
-            if g_end - f_start < motif_nums:
+            if g_end - f_start + 1 < motif_nums:
                 break
 
             num_list = result_list[f_start:g_end + 1]
             num_list_add.append(num_list)
             nums = [row['motif_type'] for row in num_list]
             sorted_nums = sorted(set(nums))
             result_index = check_sequential_numbers(nums, sorted_nums, motif_nums)
-
             if result_index is None:
                 if filtered_rows:
                     return filtered_rows
                 else:
                     return None
             else:
                 result_index = [item for expand in result_index if expand is not None for item in expand]
@@ -988,15 +1039,15 @@
                 else:
                     filtered_rows.append(filtered_temp)
 
 
     else:
         while i < len(result_list) -1:
             temp.append((result_list[i], i))
-            if result_list[i]['motif_type'] <= result_list[i + 1]['motif_type']:
+            if result_list[i]['motif_type'] <= result_list[i + 1]['motif_type'] or result_list[i+1]['start'] - result_list[i]['end'] > (result_list[i]['motif_type'] - result_list[i+1]['motif_type'])*1000:
                 lists.append(temp)
                 temp = []
             i += 1
             
         if i == len(result_list) - 1:
             temp.append((result_list[i], i))
             lists.append(temp)
@@ -1007,43 +1058,42 @@
                 continue
 
             if sublist[0][0]['motif_type'] < line_count:
                 up = ((line_count-sublist[0][0]['motif_type'] ) // 3 + 1) * 1000
                 up_value = sublist[0][0]['start'] - up
                 if up_value < result_list[0]['start']:
                     f_start=1
-
                 else:
                     for sub_list in lists:
                         if sub_list[0][0]["start"] <= up_value <= sub_list[-1][0]['end']:
                             f_start=sub_list[0][1]
                             break
                         elif up_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and up_value > lists[lists.index(sub_list)-1][-1][0]['end']:
-                            f_start=lists[lists.index(sub_list)-1][0][1]
+                            f_start=sub_list[0][1]
                             break
+
             else:
                 f_start = sublist[0][1]
 
             if sublist[-1][0]['motif_type'] >1 :
                 down = ((sublist[-1][0]['motif_type']-1) // 3 + 1) * 1000
                 down_value = sublist[-1][0]['end'] + down
                 if down_value > result_list[-1]['end']:
                     g_end = len(result_list)-1
                 else:
                     for sub_list in lists:
                         if sub_list[0][0]["start"] <= down_value <= sub_list[-1][0]['end']:
                             g_end = sub_list[-1][1]
                             break
                         elif down_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and down_value > lists[lists.index(sub_list)-1][-1][0]['end']:
-                            g_end =sub_list[-1][1]
+                            g_end =lists[lists.index(sub_list)-1][-1][1]
                             break
             else:
                 g_end = sublist[-1][1]
-
-            if g_end - f_start < motif_nums:
+            if g_end - f_start + 1 < motif_nums:
                 break
 
             num_list = result_list[f_start:g_end + 1]
             nums = [row['motif_type'] for row in num_list]
             sorted_nums = sorted(set(nums),reverse=True)
 
             result_index = check_sequential_numbers(nums, sorted_nums, motif_nums)
@@ -1053,26 +1103,23 @@
                 else:
                     return None
             else:
                 result_index = [item for expand in result_index if expand is not None for item in expand]
                 for i in result_index:
                     filtered_temp.append(num_list[i])
 
-
                 if necessary_file:
                     with open('file1.txt', 'r') as file:
                         motif_must = file.readline().strip().split(',')
                     data_list = [row['motif_type'] for row in filtered_temp]
                     all_in = all(item in data_list for item in motif_must)
-
                     if all_in:
                         filtered_rows.append(filtered_temp)
                     else:
                         return filtered_rows
-
                 else:
                     filtered_rows.append(filtered_temp)
     return filtered_rows
 
 def draw_triangle(fig, point1, point2, point3, color='blue', row=None, col=None):
     fig.add_trace(
         go.Scatter(
@@ -1159,15 +1206,15 @@
         else:
             continue
     modified_gene_list = filtered_rows.values.tolist()
 
     return modified_gene_list
 
 def plot_motifs_to_single_chart(file_path, output_file, display_both_directions=False, gff_file=None, motif_up=2000, motif_down=2000):
-    df = pd.read_csv(file_path, sep='\t', header=None, dtype={0: str, 1: int, 2: str, 3: int, 4: int, 5: str}, usecols=[0, 1, 2, 3, 4, 5], skiprows=1, names=["Sequence ID", "Length", "Motif", "Start", "End", "Strand"])
+    df = pd.read_csv(file_path, sep='\t', header=None, dtype={0: str, 1: int, 2: str, 3: str, 4: int, 5: int, 6: str}, usecols=[0, 1, 2, 3, 4, 5, 6], skiprows=1, names=["Sequence ID", "Length", "Motif", "motif_type", "Start", "End", "Strand"])
     grouped_df = df.groupby("Sequence ID")
     if df["Length"].min()>50000:
         min_length = min(50000,df["Length"].min())
     else:
         min_length = 50000
 
     correction_gff=[]
@@ -1225,42 +1272,36 @@
     height_interval = 0.7
     max_length = df["Length"].max()
     min_height = 300
     if num_sequences <= 2:
         height = min_height
     else:
         height = 100 * num_sequences
-
     screen_width = 1920
     max_length_proportion = 0.7
     line_length = screen_width * max_length_proportion
     multiplier = line_length / max_length
-
     color_list = ['#008000','#FF0000', '#0000FF', '#FF00FF', '#00FFFF', '#FFFF00', '#800000', '#00FF00', '#000080', '#808000', '#800080', '#008080', '#808080', '#C0C0C0', '#FFA500', '#E64B35','#4DBBD5','#3C5488','#F39B7F','#91D1C2','#925E9F','#84BD00','#8C564B','#5C88DA','#D6616B','#6B58EE','#FDD0A2','#E7BA52','#3F4041','#9632B8']
     color_map = {}
 
     if gff_file:
 
         fig = make_subplots(rows=num_sequences, cols=1, shared_xaxes=True)
 
         for idx, (seq_id, seq_group) in enumerate(grouped_again_df):
             y_position = idx * 2
             seq_length = seq_group.iloc[0]["Length"]
             line = seq_length * multiplier
-
             fig.add_trace(go.Scatter(x=[0, line], y=[y_position, y_position], mode='lines', line=dict(color='black'), showlegend=False),row=idx+1,col=1)
             fig.add_annotation(x=-0.5, y=y_position, text=seq_id, showarrow=False, font=dict(size=15), xanchor='right', yanchor='middle',row=idx+1,col=1)
             tick_positions = np.linspace(0, line, num=11)
-            if (seq_group.iloc[0]["type"]=="A"):
+            if (seq_group.iloc[0]["type"]=="A"):   
                 tick_labels = np.linspace(seq_group.iloc[0]["n"], seq_group.iloc[0]["n"]+min_length, num=11, dtype=int)
-            
             elif(seq_group.iloc[0]["type"]=="B"):
-
-                tick_labels = np.linspace(seq_group.iloc[0]["start_from"],seq_group.iloc[0]["end_to"], num=11, dtype=int)           
-            
+                tick_labels = np.linspace(seq_group.iloc[0]["start_from"],seq_group.iloc[0]["end_to"], num=11, dtype=int)                       
             else:
                 tick_labels = np.linspace(0, seq_length, num=11, dtype=int)
 
             for tick_pos, tick_label in zip(tick_positions, tick_labels):
                 fig.add_trace(go.Scatter(x=[tick_pos, tick_pos], y=[y_position, y_position-0.5], mode='lines', line=dict(color='black'),showlegend=False),row=idx+1,col=1)
                 fig.add_annotation(x=tick_pos, y=y_position-1.5, text=str(tick_label), showarrow=False, font=dict(size=15), xanchor='center', row=idx+1,col=1)
          
@@ -1295,25 +1336,25 @@
                     fig.add_shape(type='rect', x0=start_position, y0=y_position - height_interval, x1=end_position, y1=y_position, line=dict(color='gray'), fillcolor='gray',row=idx+1,col=1)
                     fig.add_annotation(x=(start_position+end_position)/2, y=y_position-1, text=str(gene), showarrow=False, font=dict(size=15), xanchor='center',row=idx+1,col=1)
 
             for _, row in seq_group.iterrows():
                 start = row["Start"]
                 end = row["End"]
                 direction = row["Strand"]
-                motif = row["Motif"]
+                motif_type = row["motif_type"]
                 arrow_length = (end-start) * multiplier * 0.3
 
                 if not display_both_directions and direction == '-':
                     continue
 
-                if motif not in color_map:
-                    color_map[motif] = color_list[len(color_map) % 15]
-                    fig.add_trace(go.Scatter(x=[None],y=[None],mode='markers',marker=dict(color=color_map[motif], size=30),name=motif))
+                if motif_type not in color_map:
+                    color_map[motif_type] = color_list[len(color_map) % 30]
+                    fig.add_trace(go.Scatter(x=[None],y=[None],mode='markers',marker=dict(color=color_map[motif_type], size=30),name=motif_type))
 
-                color = color_map[motif]
+                color = color_map[motif_type]
 
                 if direction == '+':
                     fig.add_shape(type='rect', x0=start * multiplier, y0=y_position, x1=end * multiplier - arrow_length, y1=y_position + height_interval, line=dict(color=color), fillcolor=color, row=idx+1,col=1)
                     draw_triangle(fig, [end * multiplier - arrow_length,y_position], [end * multiplier - arrow_length, y_position + height_interval], [end * multiplier, y_position + height_interval / 2], color=color,row=idx+1,col=1)
                 else:
                     fig.add_shape(type='rect', x0=start * multiplier + arrow_length, y0=y_position, x1=end * multiplier, y1=y_position + height_interval, line=dict(color=color), fillcolor=color, row=idx+1,col=1)
                     draw_triangle(fig, [start * multiplier, y_position + height_interval / 2], [start * multiplier + arrow_length, y_position], [start * multiplier + arrow_length, y_position + height_interval], color=color,row=idx+1,col=1)
@@ -1341,24 +1382,24 @@
             fig.add_trace(go.Scatter(x=[0, line], y=[y_position, y_position], mode='lines', line=dict(color='black'), showlegend=False))
             fig.add_annotation(x=-0.5, y=y_position, text=seq_id, showarrow=False, font=dict(size=15), xanchor='right', yanchor='middle')
 
             for _, row in seq_group.iterrows():
                 start = row["Start"]
                 end = row["End"]
                 direction = row["Strand"]
-                motif = row["Motif"]
+                motif_type = row["motif_type"]
                 arrow_length = (end-start) * multiplier * 0.3
 
                 if not display_both_directions and direction == '-':
                     continue
 
-                if motif not in color_map:
-                    color_map[motif] = color_list[len(color_map) % 15]
-                    fig.add_trace(go.Scatter(x=[None],y=[None],mode='markers',marker=dict(color=color_map[motif],size=30),name=motif))
-                color = color_map[motif]
+                if motif_type not in color_map:
+                    color_map[motif_type] = color_list[len(color_map) % 30]
+                    fig.add_trace(go.Scatter(x=[None],y=[None],mode='markers',marker=dict(color=color_map[motif_type],size=30),name=motif_type))
+                color = color_map[motif_type]
 
                 if direction == '+':
                     fig.add_shape(type='rect', x0=start * multiplier, y0=y_position, x1=end * multiplier - arrow_length, y1=y_position + height_interval, line=dict(color=color), fillcolor=color)
                     draw_triangle(fig, [end * multiplier - arrow_length,y_position], [end * multiplier - arrow_length, y_position + height_interval], [end * multiplier, y_position + height_interval / 2], color=color,row=None, col=None)
                 else:
                     fig.add_shape(type='rect', x0=start * multiplier + arrow_length, y0=y_position, x1=end * multiplier, y1=y_position + height_interval, line=dict(color=color), fillcolor=color)
                     draw_triangle(fig, [start * multiplier, y_position + height_interval / 2], [start * multiplier + arrow_length, y_position], [start * multiplier + arrow_length, y_position + height_interval], color=color,row=None, col=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `multiMotif-1.2.1/setup.py` & `multimotif-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='multiMotif',
-    version='1.2.1',
+    version='1.2.3',
     packages=find_packages(),
     install_requires=[
         'biopython>=1.78',
         'matplotlib>=3.3',
         'numpy>=1.19',
         'pandas>=1.1',
-        'plotly>=5.18.0'
+        'plotly>=5.18.0',
+        'kaleido>=0.2.1'
     ],
     author='Sainan Luo',
     description='A Computational Tool for Variable Motif scanning and Sequence-based Relative Position Visualization of Search Results in Sequences.',
     long_description=long_description,  # The new line
     long_description_content_type='text/markdown',  # The new line
     url='https://github.com/SainanLuo/multiMotif',
     entry_points={
```

