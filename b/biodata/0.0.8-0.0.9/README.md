# Comparing `tmp/biodata-0.0.8.tar.gz` & `tmp/biodata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biodata-0.0.8.tar", last modified: Thu May 23 02:22:12 2024, max compression
+gzip compressed data, was "biodata-0.0.9.tar", last modified: Sun May 26 11:52:41 2024, max compression
```

## Comparing `biodata-0.0.8.tar` & `biodata-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-23 02:22:12.663633 biodata-0.0.8/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-23 02:22:12.639632 biodata-0.0.8/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5037 2023-01-23 06:58:01.000000 biodata-0.0.8/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-23 02:22:12.638632 biodata-0.0.8/biodata/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2021-11-03 03:50:28.000000 biodata-0.0.8/biodata/__init__.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9933 2024-05-07 11:00:55.000000 biodata-0.0.8/biodata/baseio.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    11737 2024-05-23 02:18:21.000000 biodata-0.0.8/biodata/bed.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     8834 2023-01-03 16:21:18.000000 biodata-0.0.8/biodata/delimited.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5522 2023-01-14 08:29:58.000000 biodata-0.0.8/biodata/fasta.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5659 2023-01-23 06:58:54.000000 biodata-0.0.8/biodata/gff.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     6360 2023-01-21 06:14:11.000000 biodata-0.0.8/biodata/meme.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-23 02:22:12.638632 biodata-0.0.8/biodata.egg-info/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      294 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       20 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/requires.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        8 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-23 02:22:12.663633 biodata-0.0.8/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      842 2024-05-23 02:18:39.000000 biodata-0.0.8/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-26 11:52:41.146657 biodata-0.0.9/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-26 11:52:41.146657 biodata-0.0.9/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5037 2023-01-23 06:58:01.000000 biodata-0.0.9/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-26 11:52:41.130657 biodata-0.0.9/biodata/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2021-11-03 03:50:28.000000 biodata-0.0.9/biodata/__init__.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9933 2024-05-07 11:00:55.000000 biodata-0.0.9/biodata/baseio.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    14795 2024-05-23 02:29:43.000000 biodata-0.0.9/biodata/bed.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     4654 2024-05-26 11:49:17.000000 biodata-0.0.9/biodata/bigwig.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     8834 2023-01-03 16:21:18.000000 biodata-0.0.9/biodata/delimited.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5522 2023-01-14 08:29:58.000000 biodata-0.0.9/biodata/fasta.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5659 2023-01-23 06:58:54.000000 biodata-0.0.9/biodata/gff.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     6360 2023-01-21 06:14:11.000000 biodata-0.0.9/biodata/meme.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-26 11:52:41.145657 biodata-0.0.9/biodata.egg-info/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-26 11:52:36.000000 biodata-0.0.9/biodata.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      312 2024-05-26 11:52:36.000000 biodata-0.0.9/biodata.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-26 11:52:36.000000 biodata-0.0.9/biodata.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       20 2024-05-26 11:52:36.000000 biodata-0.0.9/biodata.egg-info/requires.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        8 2024-05-26 11:52:36.000000 biodata-0.0.9/biodata.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-26 11:52:41.146657 biodata-0.0.9/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      842 2024-05-26 11:51:21.000000 biodata-0.0.9/setup.py
```

### Comparing `biodata-0.0.8/PKG-INFO` & `biodata-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodata
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package for common biological data I/O
 Home-page: https://github.com/aldenleung/biodata/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodata-0.0.8/README.md` & `biodata-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `biodata-0.0.8/biodata/baseio.py` & `biodata-0.0.9/biodata/baseio.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.8/biodata/bed.py` & `biodata-0.0.9/biodata/bed.py`

 * *Files 20% similar despite different names*

```diff
@@ -348,7 +348,90 @@
 				"" if bedpe.name is None else bedpe.name, 
 				"" if bedpe.score is None else bedpe.score, 
 				"" if bedpe.strand1 is None else bedpe.strand1,
 				"" if bedpe.strand2 is None else bedpe.strand2
 				]))) + "\n")
 
 
+# import tabix
+# 
+# class BEDGraphIReader():
+# 	def __init__(self, file, index_file, dataValueType=float):
+# 		self.dataValueType = dataValueType
+# 	def value(self, r, method="sum"):
+# 		arr = tabix.query(r.genomic_pos.name, r.genomic_pos.zstart, r.genomic_pos.ostop)
+# 		
+# 		chrom = words_array[0]
+# 		chromStart = int(words_array[1]) 
+# 		chromEnd = int(words_array[2])
+# 		dataValue = self.dataValueType(words_array[3])
+# 		return BEDGraph(chrom, chromStart, chromEnd, dataValue)
+
+
+class PINTSBidirectional(BED3):
+	__slots__ = "confidence", "major_tss_pls", "major_tss_mns"
+	def __init__(self, chrom, chromStart, chromEnd, confidence, major_tss_pls, major_tss_mns):
+		super(PINTSBidirectional, self).__init__(chrom, chromStart, chromEnd)
+		self.confidence = confidence
+		self.major_tss_pls = major_tss_pls
+		self.major_tss_mns = major_tss_mns
+class PINTSBidirectionalReader(BaseReader):
+	def __init__(self, arg):
+		super(PINTSBidirectionalReader, self).__init__(arg)
+	
+	def _read(self):
+		line = self._line
+		if line is None:
+			return None
+		self._proceed_next_line() 
+		words_array = line.split('\t')
+		chrom = words_array[0]
+		chromStart = int(words_array[1]) 
+		chromEnd = int(words_array[2])
+		confidence = set(words_array[3].split(","))
+		major_tss_pls = list(map(int, words_array[4].split(",")))
+		major_tss_mns = list(map(int, words_array[5].split(",")))
+		return PINTSBidirectional(chrom, chromStart, chromEnd, confidence, major_tss_pls, major_tss_mns)
+
+class BigBedIReader(BaseIReader):
+	__slots__ = "bigbed", "fieldnames", "fieldfuncs", "BEDX"
+	def __init__(self, arg, fieldnames=[], fieldfuncs=None, x=3, classname="BEDX"):
+		'''
+		fieldnames: List of names of the additional fields. 
+		fieldfuncs: It can either be a list or a dict. 
+		x: bedx+ 
+		'''
+		import pyBigWig
+		super(BigBedIReader, self).__init__(arg)
+		BigBedIReaderSelf = self
+		def _init(self, chrom, chromStart, chromEnd, *args):
+			super(BigBedIReaderSelf.BEDX, self).__init__(chrom, chromStart, chromEnd)
+			if len(args) != len(self.__slots__):
+				raise Exception("Inconsistent field names and entries")
+			for slot, arg in zip(self.__slots__, args):
+				setattr(self, slot, arg)
+		if x < 3 or x > 12:
+			raise Exception("Incorrect X")
+		self.fieldnames = _bed_additional_fields[:x - 3] + fieldnames
+
+		addition_field_funcs = {_bed_additional_fields[i]:_bed_additional_field_funcs[i] for i in range(x - 3)}
+		if fieldfuncs is None:
+			self.fieldfuncs = addition_field_funcs
+		elif type(fieldfuncs) is dict:
+			self.fieldfuncs = fieldfuncs
+		else:
+			self.fieldfuncs = _bed_additional_field_funcs[:x - 3] + fieldfuncs
+		self.BEDX = type(classname, (BED3,), {"__slots__":self.fieldnames, "__init__":_init})
+		self.bigbed = pyBigWig.open(arg)
+		
+	def __getitem__(self, key):
+		r = GenomicPos(key)
+		if r.name not in self.bigbed.chroms():
+			return []
+		entries = self.bigbed.entries(r.name, r.zstart, r.ostop)
+		if entries is None:
+			return []
+		return [self.BEDX(r.name, zstart, ostop, *s.split()) for zstart, ostop, s in entries]
+	
+	def close(self):
+		self.bigbed.close()
+
```

### Comparing `biodata-0.0.8/biodata/delimited.py` & `biodata-0.0.9/biodata/delimited.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.8/biodata/fasta.py` & `biodata-0.0.9/biodata/fasta.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.8/biodata/gff.py` & `biodata-0.0.9/biodata/gff.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.8/biodata/meme.py` & `biodata-0.0.9/biodata/meme.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.8/biodata.egg-info/PKG-INFO` & `biodata-0.0.9/biodata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodata
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package for common biological data I/O
 Home-page: https://github.com/aldenleung/biodata/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodata-0.0.8/setup.py` & `biodata-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
-requirements = ["genomictools>=0.0.5"]
+requirements = ["genomictools>=0.0.7"]
 
 setup(
 	name="biodata",
-	version="0.0.8",
+	version="0.0.9",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A python package for common biological data I/O",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/biodata/",
 	packages=find_packages(),
```

