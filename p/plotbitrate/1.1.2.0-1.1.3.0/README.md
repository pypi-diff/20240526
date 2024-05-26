# Comparing `tmp/plotbitrate-1.1.2.0-py3-none-any.whl.zip` & `tmp/plotbitrate-1.1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12427 bytes, number of entries: 10
--rw-r--r--  2.0 unx    23361 b- defN 24-Jan-14 01:06 plotbitrate.py
+Zip file size: 12603 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    23445 b- defN 24-May-26 17:52 plotbitrate.py
 -rw-r--r--  2.0 unx      323 b- defN 21-Apr-04 22:56 frame/__init__.py
 -rw-r--r--  2.0 unx      231 b- defN 21-Apr-04 22:56 frame/_frame_class.py
 -rw-r--r--  2.0 unx      252 b- defN 21-Apr-04 22:56 frame/_frame_dataclass.py
--rw-r--r--  2.0 unx     1364 b- defN 24-Jan-14 01:22 plotbitrate-1.1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4435 b- defN 24-Jan-14 01:22 plotbitrate-1.1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-14 01:22 plotbitrate-1.1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Jan-14 01:22 plotbitrate-1.1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 24-Jan-14 01:22 plotbitrate-1.1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 24-Jan-14 01:22 plotbitrate-1.1.2.0.dist-info/RECORD
-10 files, 30945 bytes uncompressed, 11021 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1364 b- defN 24-May-26 18:03 plotbitrate-1.1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4699 b- defN 24-May-26 18:03 plotbitrate-1.1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 18:03 plotbitrate-1.1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-26 18:03 plotbitrate-1.1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-May-26 18:03 plotbitrate-1.1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 24-May-26 18:03 plotbitrate-1.1.3.0.dist-info/RECORD
+10 files, 31293 bytes uncompressed, 11197 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: frame/_frame_class.py
 Comment: 
 
 Filename: frame/_frame_dataclass.py
 Comment: 
 
-Filename: plotbitrate-1.1.2.0.dist-info/LICENSE
+Filename: plotbitrate-1.1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: plotbitrate-1.1.2.0.dist-info/METADATA
+Filename: plotbitrate-1.1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: plotbitrate-1.1.2.0.dist-info/WHEEL
+Filename: plotbitrate-1.1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: plotbitrate-1.1.2.0.dist-info/entry_points.txt
+Filename: plotbitrate-1.1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: plotbitrate-1.1.2.0.dist-info/top_level.txt
+Filename: plotbitrate-1.1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: plotbitrate-1.1.2.0.dist-info/RECORD
+Filename: plotbitrate-1.1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plotbitrate.py

```diff
@@ -25,15 +25,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = "1.1.2.0"
+__version__ = "1.1.3.0"
 
 import argparse
 import csv
 import datetime
 import math
 import multiprocessing
 import os
@@ -91,16 +91,20 @@
     import matplotlib.pyplot as matplot  # type: ignore
 except ImportError as err:
     # satisfy undefined variable warnings
     matplotlib = None
     matplot = None
     exit_with_error("Missing package 'python3-matplotlib'")
 
+
+# bring your own ffprobe, if you want
+ffprobe = os.environ.get('FFPROBE_PATH', 'ffprobe')
+
 # check for ffprobe in path
-if not shutil.which("ffprobe"):
+if not shutil.which(ffprobe):
     exit_with_error("Missing ffprobe from package 'ffmpeg'")
 
 
 def parse_arguments() -> argparse.Namespace:
     """ Parses all arguments and returns them as an object. """
     if sys.version_info >= (3, 6):
         supported_filetypes = matplotlib.figure.Figure().canvas \
@@ -189,15 +193,15 @@
 
 def open_ffprobe_get_format(file_path: str) -> subprocess.Popen:
     """
     Opens an ffprobe process that reads the format data
     for file_path and returns the process.
     """
     return subprocess.Popen(
-        ["ffprobe",
+        [ffprobe,
          "-hide_banner",
          "-loglevel", "error",
          "-show_entries", "format",
          "-print_format", "xml",
          file_path
          ],
         stdout=subprocess.PIPE)
@@ -208,15 +212,15 @@
         stream_selector: str
 ) -> subprocess.Popen:
     """
     Opens an ffprobe process that reads all frame data for
     file_path and returns the process.
     """
     return subprocess.Popen(
-        ["ffprobe",
+        [ffprobe,
          "-hide_banner",
          "-loglevel", "error",
          "-select_streams", stream_selector,
          "-threads", str(multiprocessing.cpu_count()),
          "-print_format", "xml",
          "-show_entries",
          "frame=pict_type,pkt_pts_time,best_effort_timestamp_time,pkt_size",
@@ -243,15 +247,15 @@
 
     with open(target_path, "wb") as f:
         # open and clear file
         f.seek(0)
         f.truncate()
 
         with subprocess.Popen(
-                ["ffprobe",
+                [ffprobe,
                  "-hide_banner",
                  "-loglevel", "error",
                  "-select_streams", stream_selector,
                  "-threads", str(multiprocessing.cpu_count()),
                  "-print_format", "xml",
                  "-show_entries",
                  "format:frame=pict_type,pkt_pts_time,"
```

## Comparing `plotbitrate-1.1.2.0.dist-info/LICENSE` & `plotbitrate-1.1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plotbitrate-1.1.2.0.dist-info/METADATA` & `plotbitrate-1.1.3.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotbitrate
-Version: 1.1.2.0
+Version: 1.1.3.0
 Summary: A simple bitrate plotter for media files
 Home-page: https://github.com/zeroepoch/plotbitrate
 Author: Eric Work
 Author-email: work.eric@gmail.com
 License: BSD
 Keywords: ffprobe bitrate plot
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -144,7 +144,18 @@
 ```
 
 Show the bitrate, but fill the area below the curve with a solid color.
 
 ```
 plotbitrate --solid input.mkv
 ```
+
+It's possible to specify a custom `FFPROBE_PATH` in case you don't have it on your `PATH` or want a custom `ffprobe`:
+
+```
+# Unix
+FFPROBE_PATH=/tmp/ffprobe plotbitrate input.mkv
+
+# Windows
+set FFPROBE_PATH=C:\temp\ffmpeg\bin\ffprobe.exe
+plotbitrate input.mkv
+```
```

## Comparing `plotbitrate-1.1.2.0.dist-info/RECORD` & `plotbitrate-1.1.3.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-plotbitrate.py,sha256=8kQkxnZqcPLdKmFrfzX6nJv9mgCB6G9VibNtueOCOXs,23361
+plotbitrate.py,sha256=ghmFcAZwJVq_V0iojB-SnzxcfWfF7PiPpKOkN7fo4cM,23445
 frame/__init__.py,sha256=lreLJjeFT9pLvyyf2stOlYFdyFzQRyhwKan6l3GIk8s,323
 frame/_frame_class.py,sha256=13_0I0ppVdU8CwzuawmEWlHdYbLONKAQULdaeYzrPOY,231
 frame/_frame_dataclass.py,sha256=-e_aeJVO6tMx64o0tYFodaT3iHtlrh715RIHv-PLfSE,252
-plotbitrate-1.1.2.0.dist-info/LICENSE,sha256=7gMLzipQQbYZ8EeaP-5b7kUeGlQLL9jtLkCcRo5NiGg,1364
-plotbitrate-1.1.2.0.dist-info/METADATA,sha256=N5cwUUSB_ZvLQ6gVUKi2MD_Ghd_w2JiviHdWkUMrqS4,4435
-plotbitrate-1.1.2.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-plotbitrate-1.1.2.0.dist-info/entry_points.txt,sha256=DCDetfld1tV6cn8F2n8ZJJrGvq-RUtlR-a4Bqi1B2tA,49
-plotbitrate-1.1.2.0.dist-info/top_level.txt,sha256=JeWBr1OWk8x_JVHfQRr10u6A3R8vLaV9XT6iEs1RzKU,18
-plotbitrate-1.1.2.0.dist-info/RECORD,,
+plotbitrate-1.1.3.0.dist-info/LICENSE,sha256=7gMLzipQQbYZ8EeaP-5b7kUeGlQLL9jtLkCcRo5NiGg,1364
+plotbitrate-1.1.3.0.dist-info/METADATA,sha256=q1G6v3dYuhLrPFFuzJf101hxiO2TQaznu-p32tmK9Pw,4699
+plotbitrate-1.1.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+plotbitrate-1.1.3.0.dist-info/entry_points.txt,sha256=DCDetfld1tV6cn8F2n8ZJJrGvq-RUtlR-a4Bqi1B2tA,49
+plotbitrate-1.1.3.0.dist-info/top_level.txt,sha256=JeWBr1OWk8x_JVHfQRr10u6A3R8vLaV9XT6iEs1RzKU,18
+plotbitrate-1.1.3.0.dist-info/RECORD,,
```

