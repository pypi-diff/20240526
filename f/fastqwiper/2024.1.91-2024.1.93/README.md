# Comparing `tmp/fastqwiper-2024.1.91-py3-none-any.whl.zip` & `tmp/fastqwiper-2024.1.93-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12872 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-May-25 10:10 fastq_wiper/__init__.py
--rw-r--r--  2.0 unx     9984 b- defN 24-May-25 10:10 fastq_wiper/wiper.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-25 10:10 tests/__init__.py
--rw-r--r--  2.0 unx      816 b- defN 24-May-25 10:10 tests/test_wiper.py
--rw-r--r--  2.0 unx     7601 b- defN 24-May-25 10:10 fastqwiper-2024.1.91.dist-info/LICENSE
--rw-r--r--  2.0 unx    14374 b- defN 24-May-25 10:10 fastqwiper-2024.1.91.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-25 10:10 fastqwiper-2024.1.91.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 24-May-25 10:10 fastqwiper-2024.1.91.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 24-May-25 10:10 fastqwiper-2024.1.91.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      824 b- defN 24-May-25 10:10 fastqwiper-2024.1.91.dist-info/RECORD
-10 files, 33763 bytes uncompressed, 11450 bytes compressed:  66.1%
+Zip file size: 12935 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-May-26 07:22 fastq_wiper/__init__.py
+-rw-r--r--  2.0 unx    10069 b- defN 24-May-26 07:22 fastq_wiper/wiper.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-26 07:22 tests/__init__.py
+-rw-r--r--  2.0 unx      816 b- defN 24-May-26 07:22 tests/test_wiper.py
+-rw-r--r--  2.0 unx     7601 b- defN 24-May-26 07:23 fastqwiper-2024.1.93.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14528 b- defN 24-May-26 07:23 fastqwiper-2024.1.93.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 07:23 fastqwiper-2024.1.93.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-May-26 07:23 fastqwiper-2024.1.93.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-May-26 07:23 fastqwiper-2024.1.93.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      825 b- defN 24-May-26 07:23 fastqwiper-2024.1.93.dist-info/RECORD
+10 files, 34003 bytes uncompressed, 11513 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_wiper.py
 Comment: 
 
-Filename: fastqwiper-2024.1.91.dist-info/LICENSE
+Filename: fastqwiper-2024.1.93.dist-info/LICENSE
 Comment: 
 
-Filename: fastqwiper-2024.1.91.dist-info/METADATA
+Filename: fastqwiper-2024.1.93.dist-info/METADATA
 Comment: 
 
-Filename: fastqwiper-2024.1.91.dist-info/WHEEL
+Filename: fastqwiper-2024.1.93.dist-info/WHEEL
 Comment: 
 
-Filename: fastqwiper-2024.1.91.dist-info/entry_points.txt
+Filename: fastqwiper-2024.1.93.dist-info/entry_points.txt
 Comment: 
 
-Filename: fastqwiper-2024.1.91.dist-info/top_level.txt
+Filename: fastqwiper-2024.1.93.dist-info/top_level.txt
 Comment: 
 
-Filename: fastqwiper-2024.1.91.dist-info/RECORD
+Filename: fastqwiper-2024.1.93.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastq_wiper/wiper.py

```diff
@@ -6,14 +6,15 @@
 import gzip
 import re
 import codecs
 import argparse
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
+reg = None
 
 # region Variables for final report
 blank: int = 0
 tot_lines: int = 0
 bad_seq: int = 0
 fixed_header: int = 0
 bad_header: int = 0
@@ -90,15 +91,15 @@
         header = line
         header = header[header.rfind("@"):]
         fixed_header += 1
 
     return header
 
 
-def check_seq_line(line: str) -> str:
+def check_seq_line(line: str, reg: str) -> str:
     global bad_seq
     raw_seq: str = ""
 
     if not line.isprintable() or not reg.match(line):
         bad_seq += 1
     else:
         raw_seq = line
@@ -229,28 +230,30 @@
 
     if blank == 0:
         logging.info(f"Blank lines: {blank}/{tot_lines}")
     else:
         logging.warning(f"Blank lines: {blank}/{tot_lines}")
 
 
-def wipe_fastq(fastq_in: str, fastq_out: str, log_out: str, log_frequency: int):
+def wipe_fastq(fastq_in: str, fastq_out: str, log_out: str, log_frequency: int, alphabet: str):
     # MIN_HEADER_LEN = 10
 
     fin = open_fastq_file(fastq_in)
     if not fin:
         logging.critical("The input FASTQ file does not exist or bad extension (.gz or .fastq.gz)")
     else:
         logging.info(f"Start wiping {fastq_in}")
 
         # Open file out stream
         fout = write_fastq_file(fastq_out)
 
         # global variables anchor
         global tot_lines, clean_reads, seq_len_neq_qual_len
+        # Allowed characters of the SEQ line
+        reg = re.compile(f"^[{alphabet}]+$")
 
         # Loop through 4-line reads
         for line in fin:
             if not line.strip():
                 # skip empty lines
                 continue
 
@@ -260,15 +263,15 @@
             # PROCESS THE HEADER LINE
             header: str = check_header_line(line.rstrip())
             if not header:
                 continue
 
             # PROCESS THE SEQ LINE
             line = read_next_line(fin, log_frequency)
-            raw_seq: str = check_seq_line(line.rstrip())
+            raw_seq: str = check_seq_line(line.rstrip(), reg)
             if not raw_seq:
                 continue
 
             # PROCESS the + line
             line = read_next_line(fin, log_frequency)
             plus: str = check_plus_line(line.rstrip())
             if not plus:
@@ -295,23 +298,24 @@
 
         if log_out:
             print_log_to_file(log_out)
         else:
             print_log_to_screen()
 
 
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(description='FastqWiper entrypoint')
     parser.add_argument("-i", '--fastq_in', help='The corrupted FASTQ file', required=True)
     parser.add_argument("-o", '--fastq_out', help='The wiped FASTQ file', required=True)
     parser.add_argument("-l", '--log_out', nargs='?',
                         help='The file name of the final quality report summary. Print on the screen if not specified')
     parser.add_argument("-f", '--log_frequency', type=int, nargs='?', default=500000, const=500000,
                         help='The number of reads you want to print a status message. Default: 500000')
     parser.add_argument("-a", '--alphabet', type=str, nargs='?', default="ACGTN", const="ACGTN",
                         help='Allowed character in the SEQ line. Default: ACGTN')
     args = parser.parse_args()
 
-    # Allowed character of the SEQ line
-    reg = re.compile(f"^[{args.alphabet}]+$")
+    wipe_fastq(args.fastq_in, args.fastq_out, args.log_out, args.log_frequency, args.alphabet)
+
 
-    wipe_fastq(args.fastq_in, args.fastq_out,args.log_out, args.log_frequency)
+if __name__ == "__main__":
+    main()
```

## Comparing `fastqwiper-2024.1.91.dist-info/LICENSE` & `fastqwiper-2024.1.93.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastqwiper-2024.1.91.dist-info/METADATA` & `fastqwiper-2024.1.93.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqwiper
-Version: 2024.1.91
+Version: 2024.1.93
 Summary: An ensemble method to recover corrupted FASTQ files, drop or fix pesky lines, remove unpaired reads, and fix reads interleaving
 Home-page: https://github.com/mazzalab/fastqwiper
 Author: Tommaso Mazza
 Author-email: bioinformatics@css-mendel.it
 License: MIT
 Project-URL: Source, https://github.com/mazzalab/fastqwiper
 Project-URL: Tracker, https://github.com/mazzalab/fastqwiper/issues
@@ -94,38 +94,39 @@
 #### One quick way (Docker)
 1. Pull the Docker image from DockerHub:
 
 `docker pull mazzalab/fastqwiper`
 
 2. Once downloaded the image, type:
 
-CMD: `docker run --rm -ti --name fastqwiper -v "YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data" mazzalab/fastqwiper paired 8 sample 50000000 33 ACGTN`
+CMD: `docker run --rm -ti --name fastqwiper -v "YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data" mazzalab/fastqwiper paired 8 sample 50000000 33 ACGTN 500000`
 
 #### Another quick way (Singularity)
 1. Pull the Singularity image from the Cloud Library:
 
 `singularity pull library://mazzalab/fastqwiper/fastqwiper.sif`
 
 2. Once downloaded the image (e.g., fastqwiper.sif_2024.1.89.sif), type:
 
-CMD `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data --writable-tmpfs fastqwiper.sif_2024.1.89.sif paired 8 sample 50000000 33 ACGTN`
+CMD `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data --writable-tmpfs fastqwiper.sif_2024.1.89.sif paired 8 sample 50000000 33 ACGTN 500000`
 
 If you want to bind the `.singularity` cache folder and the `logs` folder, you can omit `--writable-tmpfs`, create the folders `.singularity` and `logs` (`mkdir .singularity logs`) on the host system, and use this command instead:
 
 CMD: `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER/:/fastqwiper/data --bind YOUR_LOCAL_PATH_TO_.SNAKEMAKE_FOLDER/:/fastqwiper/.snakemake --bind YOUR_LOCAL_PATH_TO_LOGS_FOLDER/:/fastqwiper/logs fastqwiper.sif_2024.1.89.sif paired 8 sample 50000000 33 ACGTN`
 
 For both **Docker** and **Singularity**:
 
 - `YOUR_LOCAL_PATH_TO_DATA_FOLDER` is the path of the folder where the fastq.gz files to be wiped are located;
 - `paired` triggers the cleaning of R1 and R2. Alternatively, `single` will trigger the wipe of individual FASTQ files;
 - `8` is the number of your choice of computing cores to be spawned;
 - `sample` is part of the names of the FASTQ files to be wiped. <b>Be aware</b> that: for <b>paired-end</b> files (e.g., "sample_R1.fastq.gz" and "sample_R2.fastq.gz"), your files must finish with `_R1.fastq.gz` and `_R2.fastq.gz`. Therefore, the argument to pass is everything before these texts: `sample` in this case. For <b>single end</b>/individual files (e.g., "excerpt_R1_001.fastq.gz"), your file must end with the string `.fastq.gz`; the preceding text, i.e., "excerpt_R1_001" in this case, will be the text to be passed to the command as an argument. 
 - `50000000` (optional) is the number of rows-per-chunk (used when cores>1. It must be a number multiple of 4). Increasing this number too much would reduce the parallelism advantage. Decreasing this number too much would increase the number of chunks more than the number of available cpus, making parallelism unefficient. Choose this number wisely depending on the total number of reads in your starting file.
 - `33` (optional) is the ASCII offset (33=Sanger, 64=old Solexa)
 - `ACGTN` (optional) is the allowed alphabet in the SEQ line of the FASTQ file
+- `500000` (optional) is the log frequency (# reads)
 
 ### <code style="color : red">The slow way (Linux & Mac OS)</code>
 To enable the use of preconfigured [pipelines](https://github.com/mazzalab/fastqwiper/tree/main/pipeline), you need to install **Snakemake**. The recommended way to install Snakemake is via Conda, because it enables **Snakemake** to [handle software dependencies of your workflow](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html#integrated-package-management).
 However, the default conda solver is slow and often hangs. Therefore, we recommend installing [Mamba](https://github.com/mamba-org/mamba) as a drop-in replacement via
 
 `$ conda install -c conda-forge mamba`
 
@@ -172,42 +173,42 @@
 
 <code style="color : orange">**N.b.**: In all commands above, you will pass the name of the sample to be analyzed to the workflow through the config argument: `sample_name`. Remember that your fastq files' names must finish with `_R1.fastq.gz` and `_R2.fastq.gz`, for paired fastq files, and with `.fastq.gz`, for individual fastq files, and, therefore, the text to be assigned to the variable `sample_name` must be everything before them. E.g., if your files are `my_sample_R1.fastq.gz` and `my_sample_R2.fastq.gz`, then `--config sample_name=my_sample`.</code>
 
 
 #### Paired-end files
 
 - **Get a dry run** of a pipeline (e.g., `fix_wipe_pairs_reads_sequential.smk`):<br />
-`snakemake --config sample_name=my_sample qin=33 alphabet=ACGTN -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 4`
+`snakemake --config sample_name=my_sample qin=33 alphabet=ACGTN log_freq=1000 -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 4 -np`
 
 - **Generate the planned DAG**:<br />
-`snakemake --config sample_name=my_sample qin=33 alphabet=ACGTN -s pipeline/fix_wipe_pairs_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /> <br />
+`snakemake --config sample_name=my_sample qin=33 alphabet=ACGTN log_freq=1000 -s pipeline/fix_wipe_pairs_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /> <br />
 <img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_pairs_reads.png?raw=true" width="400">
 
 - **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote packages and may take longer). The number of computing cores can be tuned accordingly:<br />
-`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
+`snakemake --config sample_name=my_sample alphabet=ACGTN log_freq=1000 -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 2`
 
 Fixed files will be copied in the `data` folder and will be suffixed with the string `_fixed_wiped_paired_interleaving`.
 We remind that the `fix_wipe_pairs_reads_sequential.smk` and `fix_wipe_pairs_reads_parallel.smk` pipelines perform the following actions:
 - execute `gzrt` on corrupted fastq.gz files (i.e., that cannot be unzipped because of errors) and recover readable reads;
 - execute `FastqWiper` on recovered reads to make them compliant with the FASTQ format (source: [Wipipedia](https://en.wikipedia.org/wiki/FASTQ_format))
 - execute `Trimmomatic` on wiped reads to remove residual unpaired reads
 - execute `BBmap (repair.sh)` on paired reads to fix the correct interleaving and sort fastq files.  
 
 #### Single-end files
 `fix_wipe_single_reads_parallel.smk` and `fix_wipe_single_reads_sequential.smk` will not execute `trimmomatic` and BBmap's `repair.sh`.
 
 - **Get a dry run** of a pipeline (e.g., `fix_wipe_single_reads_sequential.smk`):<br />
-`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2 -np`
+`snakemake --config sample_name=my_sample alphabet=ACGTN log_freq=1000 -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2 -np`
 
 - **Generate the planned DAG**:<br />
-`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /><br />
+`snakemake --config sample_name=my_sample alphabet=ACGTN log_freq=1000 -s pipeline/fix_wipe_single_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /><br />
 <img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_single_reads.png?raw=true" width="200">
 
 - **Run the pipeline** (n.b., The number of computing cores can be tuned accordingly):<br />
-`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
+`snakemake --config sample_name=my_sample alphabet=ACGTN log_freq=1000 -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
 
 # Author
 **Tommaso Mazza**  
 [![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white)](https://twitter.com/irongraft) [![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/tommasomazza/)
 
 Laboratory of Bioinformatics</br>
 Fondazione IRCCS Casa Sollievo della Sofferenza</br>
```

## Comparing `fastqwiper-2024.1.91.dist-info/RECORD` & `fastqwiper-2024.1.93.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 fastq_wiper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fastq_wiper/wiper.py,sha256=VW2w-TjE_EZnxF7djWepATjl6-3ll1Iy2dmZSuJ0QiE,9984
+fastq_wiper/wiper.py,sha256=Rmh222gryc_Tom333VVnwhKZhOqEirn6zDitU26dZH4,10069
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_wiper.py,sha256=SC8gElm6F6E1SXnPHGSznduT7T03E5u5G82btLjMzMc,816
-fastqwiper-2024.1.91.dist-info/LICENSE,sha256=DWt8ibsIVfsr_QsQ8XUkSM5hf5T0TJRHUc350xWkcdM,7601
-fastqwiper-2024.1.91.dist-info/METADATA,sha256=8Kt0MALIOTjIoFLv32KE-PxUplaQTiMC6huUDFEWsac,14374
-fastqwiper-2024.1.91.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-fastqwiper-2024.1.91.dist-info/entry_points.txt,sha256=dzVJAkMJq0vNxUYsSLd9CrRjvcpAyE8lXX0ONmohQEY,54
-fastqwiper-2024.1.91.dist-info/top_level.txt,sha256=PoRVateDzVx-xrn4iraE8TOWCGvtsEwbaM97BHkr6bU,18
-fastqwiper-2024.1.91.dist-info/RECORD,,
+fastqwiper-2024.1.93.dist-info/LICENSE,sha256=DWt8ibsIVfsr_QsQ8XUkSM5hf5T0TJRHUc350xWkcdM,7601
+fastqwiper-2024.1.93.dist-info/METADATA,sha256=CDcrx13f_CjkeRRqM5aJY5LdmCiuSWBqj9fucHtFsno,14528
+fastqwiper-2024.1.93.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+fastqwiper-2024.1.93.dist-info/entry_points.txt,sha256=dzVJAkMJq0vNxUYsSLd9CrRjvcpAyE8lXX0ONmohQEY,54
+fastqwiper-2024.1.93.dist-info/top_level.txt,sha256=PoRVateDzVx-xrn4iraE8TOWCGvtsEwbaM97BHkr6bU,18
+fastqwiper-2024.1.93.dist-info/RECORD,,
```

