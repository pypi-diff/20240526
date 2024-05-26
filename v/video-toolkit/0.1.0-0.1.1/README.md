# Comparing `tmp/video_toolkit-0.1.0.tar.gz` & `tmp/video_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_toolkit-0.1.0.tar", last modified: Mon Apr 29 06:38:11 2024, max compression
+gzip compressed data, was "video_toolkit-0.1.1.tar", last modified: Sun May 26 04:06:30 2024, max compression
```

## Comparing `video_toolkit-0.1.0.tar` & `video_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:38:11.763512 video_toolkit-0.1.0/
--rw-rw-rw-   0        0        0      235 2024-04-29 06:38:11.761519 video_toolkit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-29 06:38:11.763512 video_toolkit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      435 2024-04-29 06:33:21.000000 video_toolkit-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:38:11.749310 video_toolkit-0.1.0/video_toolkit/
--rw-rw-rw-   0        0        0     5353 2024-04-27 05:54:06.000000 video_toolkit-0.1.0/video_toolkit/SrtToCsv.py
--rw-rw-rw-   0        0        0      760 2024-04-27 05:50:15.000000 video_toolkit-0.1.0/video_toolkit/Video01.py
--rw-rw-rw-   0        0        0       94 2024-04-29 06:27:22.000000 video_toolkit-0.1.0/video_toolkit/__init__.py
--rw-rw-rw-   0        0        0    54733 2024-04-29 06:29:17.000000 video_toolkit-0.1.0/video_toolkit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:38:11.759523 video_toolkit-0.1.0/video_toolkit.egg-info/
--rw-rw-rw-   0        0        0      235 2024-04-29 06:38:11.000000 video_toolkit-0.1.0/video_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 06:38:11.000000 video_toolkit-0.1.0/video_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:38:11.000000 video_toolkit-0.1.0/video_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-04-29 06:38:11.000000 video_toolkit-0.1.0/video_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 06:38:11.000000 video_toolkit-0.1.0/video_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 04:06:30.626507 video_toolkit-0.1.1/
+-rw-rw-rw-   0        0        0      183 2024-05-26 04:06:30.624512 video_toolkit-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 04:06:30.627504 video_toolkit-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-26 04:05:06.000000 video_toolkit-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:06:30.606560 video_toolkit-0.1.1/video_toolkit/
+-rw-rw-rw-   0        0        0      100 2024-05-26 04:03:31.000000 video_toolkit-0.1.1/video_toolkit/__init__.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:07.000000 video_toolkit-0.1.1/video_toolkit/cant_use_vt.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:00.000000 video_toolkit-0.1.1/video_toolkit/fix_bug_vt.py
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:15:00.000000 video_toolkit-0.1.1/video_toolkit/sandbox1_vt.py
+-rw-rw-rw-   0        0        0    63469 2024-05-26 03:07:41.000000 video_toolkit-0.1.1/video_toolkit/utils_vt.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:06:30.622518 video_toolkit-0.1.1/video_toolkit.egg-info/
+-rw-rw-rw-   0        0        0      183 2024-05-26 04:06:30.000000 video_toolkit-0.1.1/video_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-05-26 04:06:30.000000 video_toolkit-0.1.1/video_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 04:06:30.000000 video_toolkit-0.1.1/video_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2024-05-26 04:06:30.000000 video_toolkit-0.1.1/video_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 04:06:30.000000 video_toolkit-0.1.1/video_toolkit.egg-info/top_level.txt
```

### Comparing `video_toolkit-0.1.0/video_toolkit/utils.py` & `video_toolkit-0.1.1/video_toolkit/utils_vt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,357 @@
 # imported from "C:\Users\Heng2020\OneDrive\Python NLP\NLP 06_ffmpeg\ffmpeg_01.py"
 from typing import Union,List,Tuple, Literal, Callable
 from pathlib import Path
 import sys
-
+import datetime
 import python_wizard as pw
 import os_toolkit as ost
 import dataframe_short as ds
+import pkg_resources
 
 import pandas as pd
 import seaborn as sns
 
+alarm_done_path = pkg_resources.resource_filename(__name__, 'assets/Sound Effect positive-logo-opener.wav')
+sound_error_path = pkg_resources.resource_filename(__name__, 'assets/Sound Effect Error.wav')
+
+CODEC_DICT = {'.mp3': "libmp3lame",
+                  'mp3' : "libmp3lame",
+                  '.wav': "pcm_s24le",
+                  'wav' : "pcm_s24le"
+                  }
+
 # v02 => add extract_audio2, extract_subtitle, _extract_media_setup,extract_sub_1_video
 # get_metadata2, get_all_metadata, get_metadata
 # get_subtitle_index,get_audio_index,get_video_index,_get_media_index,get_subtitle_extension,
 # get_audio_extension,get_video_extension, _get_media_extension
 
+def clean_subtitle(string):
+    import re
+    pattern1 = "<.*?>"
+    
+    pattern2 = "<\/[a-zA-Z]>"
+    
+    string1 = re.sub(pattern1, "", string)
+    string2 = string1.replace("\n"," ")
+    new_string = re.sub(pattern2,"",string2)
+    return new_string
+
+def audio_duration(video_path):
+    from pydub import AudioSegment
+    from datetime import datetime, timedelta
+
+    if isinstance(video_path,str):
+        video_audio = AudioSegment.from_file(video_path)
+    else:
+        video_audio = video_path
+
+    # Get the duration of the audio segment in milliseconds
+    duration_ms = len(video_audio)
+
+    # Convert the duration from milliseconds to a timedelta object
+    duration = timedelta(milliseconds=duration_ms)
+
+    # Create a dummy datetime object with a zero timestamp
+    dummy_datetime = datetime(1, 1, 1, 0, 0, 0)
+
+    # Add the duration to the dummy datetime to get the final datetime
+    final_datetime = dummy_datetime + duration
+
+    return final_datetime.time()
+
+# Sub
+def split_1audio_by_subtitle(video_path: Union[str,Path],
+                            subtitle_path,
+                            output_folder,
+                            prefix_name = None,
+                            out_audio_ext = "wav",
+                            alarm_done:bool = False,
+                            verbose = 1,
+                            ) -> None:
+    import time
+    import os
+    from pydub import AudioSegment
+    from playsound import playsound
+    from pathlib import Path
+
+    import video_toolkit as vt
+    import python_wizard as pw
+    import py_string_tool as pst
+    
+    # alarm done path still have an error
+    # took about 1 hr(including testing)
+    # Add feature: input as video_folder_path and subtitle_folder_path, then 
+    # it would automatically know which subttile to use with which video(using SxxExx)
+    
+    # split_audio_by_subtitle
+    if prefix_name is None:
+        prefix_name_in = Path(video_path).stem
+    else:
+        prefix_name_in = str(prefix_name)
+        
+    # with dot and no dots supported
+    # but only tested with no dots out_audio_ext
+    
+    out_audio_ext_dot = out_audio_ext if out_audio_ext[0] == "." else ("." + out_audio_ext)
+    out_audio_ext_no_dot = out_audio_ext[1:] if out_audio_ext[0] == "." else ( out_audio_ext)
+    
+    subs = vt.srt_to_df(subtitle_path)
+
+    
+    # TODO: write a function input is video/video path & subs/sub path
+    t01 = time.time()
+    video_audio = AudioSegment.from_file(video_path)
+    t02 = time.time()
+    t01_02 = t02-t01
+
+    if verbose in [1]:
+        print("Load video time: ", end = " ")
+        pw.print_time(t01_02)
+    
+    if alarm_done:
+        playsound(alarm_done_path)
+    # ---------------------------- run til 1 -------------------------------
+    ########################## start run 2 ################################
+    t03 = time.time()
+    video_length = audio_duration(video_audio)
+    # Iterate over subtitle sentences
+    n = subs.shape[0]
+    t04 = time.time()
+    for i in range(n):
+        start_time = subs.loc[i,'start']
+        end_time = subs.loc[i,'end']
+        
+        if start_time > video_length:
+            break
+
+        start_time_ms = to_ms(start_time)
+        end_time_ms = to_ms(end_time)
+
+        # Extract audio segment based on timestamps
+        sentence_audio = video_audio[start_time_ms:end_time_ms]
+        
+        num_str = pst.num_format0(i+1,n+1)
+        # Save the audio segment to a file
+        audio_name = f'{prefix_name_in}_{num_str}{out_audio_ext_dot}'
+        audio_output = os.path.join(output_folder,audio_name)
+        sentence_audio.export(audio_output, format=out_audio_ext_no_dot)
+    t05 = time.time()
+
+    t04_05 = t05-t04
+    if alarm_done:
+        playsound(alarm_done_path)
+
+def extract_audio3(
+        video_folder:     Union[Path,str],
+        output_folder:    Union[Path,str],
+        video_extension:  Union[list,str] = [".mp4",".mkv"],
+        output_extension: Union[list,str] = ".mp3",
+        overwrite_file:   bool = True,
+        n_limit:          int = 150,
+        output_prefix:    str = "",
+        output_suffix:    str = "",
+        alarm_done:       bool = True,
+
+        one_output_per_lang: bool = True,
+        languages: Union[List[str],None] = None,
+):
+    """
+    the diff between 
+    extract_audio1 - use manually code to loop through folder
+    extract_audio2 - powered by _extract_media_setup while 
+    extract_audio3 - use extract_audio_1file as a base(which is more general than extract_audio1 & extract_audio2), but need more testing to see if it works
+    
+    # after testing I would then rename extract_audio3 to just extract_audio
+    
+    """
+
+
+    _extract_media_setup(
+        input_folder = video_folder,
+        output_folder = output_folder,
+        input_extension = video_extension,
+        output_extension = output_extension,
+        extract_1_file_func = extract_audio_1file,
+        overwrite_file = overwrite_file,
+        n_limit = n_limit,
+        output_prefix = output_prefix,
+        output_suffix = output_suffix,
+        alarm_done = alarm_done,
+        alarm_done_path = alarm_done_path,
+
+        one_output_per_lang = one_output_per_lang,
+        languages = languages
+
+    )
+
+
+def extract_audio_1file(
+        video_path:     Union[str,Path],
+        output_folder:  Union[str,Path],
+        output_name:    Union[str,Path, None] = None, 
+        output_extension: Union[str,list] = ".mp3",
+        alarm_done: bool = False,
+        overwrite_file: bool = True,
+        one_output_per_lang: bool = True,
+        languages: Union[List[str],None] = None,
+        
+        progress_bar:bool = True,
+                    ) -> None:
+    # time spend 5 hr
+    # this support multiple output_extension
+    # medium tested
+    
+    
+    #  tested Parameters:
+        # all default parameters
+        # when languages is str
+    
+    # untested Parameters
+        # output_extension as list
+        # overwrite_file = False
+        # one_output_per_lang = False
+        # languages as list
+        
+    # Not Done 
+    # Next right now I got a name BigBang_FR_S06E01.mp3_EN which is wrong
+    
+    from langcodes import Language
+    """
+    Extract audio from a video file. If video has multiple audio in different languages,
+    this function also support that
+    
+    it's more general than extract_audio. These functions need to be tested and merge in the future
+
+    Parameters
+    ----------
+    video_path : Union[str,Path]
+        DESCRIPTION.
+    output_folder : Union[str,Path]
+        DESCRIPTION.
+    output_name : Union[str,Path]
+        DESCRIPTION.
+    file_extension : Union[str,list], optional
+        DESCRIPTION. The default is ".mp3".
+    alarm_done : bool, optional
+        DESCRIPTION. The default is True.
+    overwrite_file : bool, optional
+        DESCRIPTION. The default is True.
+    
+    one_output_per_lang : bool, optional
+        If there are more than 1 audio files for each langauge, if True then it would one extract 1 file per
+        language, if not it would extract all of them seperately.
+        The default is True.
+        False is still not in production because I have to create index suffix at the end
+    Returns
+    -------
+    bool
+        DESCRIPTION.
+
+    """
+    from tqdm import tqdm
+    from langcodes import Language
+    from pathlib import Path
+    import subprocess
+    from playsound import playsound
+    import os
+
+    
+    codec = CODEC_DICT[output_extension]
+    
+    output_folder_in = Path(output_folder)
+    
+    file_extension_in = [output_extension] if isinstance(output_extension, str) else list(output_extension)
+    
+
+    if output_name is None:
+        output_name_in = Path(video_path).stem
+    else:
+        output_name_in = output_name
+    
+    filter_lang = [languages] if isinstance(languages,str) else languages
+    
+    if languages is None:
+        filter_lang_3chr = None
+    else:
+        filter_lang_3chr = []
+    
+        for language in filter_lang:
+            lang_obj =  closest_language_obj(language)
+            # variant = "B" would return fre for french
+            filter_lang_3chr.append(lang_obj.to_alpha3(variant = "B"))
+    
+    audio_index = get_audio_index(video_path)
+    metadata = get_metadata(video_path,"audio",language=filter_lang_3chr)
+    
+    if one_output_per_lang:
+        metadata_filter = metadata.drop_duplicates(subset=['language'], keep='first')
+    else:
+        metadata_filter = metadata.copy()
+    
+    audio_index = list(metadata_filter.index)
+    video_lang_list = metadata_filter['language'].tolist()
+
+
+    output_name_list = []
+    output_path_list = []
+
+    if progress_bar:
+        loop_obj = tqdm(enumerate(video_lang_list),total=len(video_lang_list))
+    else:
+        loop_obj = enumerate(video_lang_list)
+
+    for i, language_3_str in loop_obj:
+        
+        lang_obj =  Language.get(language_3_str)
+        language_2_str = str(lang_obj).upper()
+        lang_obj.to_alpha3()
+        for j, curr_file_ext in enumerate(file_extension_in):
+            
+            if curr_file_ext not in output_name_in:
+                if "." not in curr_file_ext:
+                    file_extension_in[j] = "." + curr_file_ext
+                else:
+                    file_extension_in[j] = curr_file_ext
+                curr_output_name = output_name_in + "_" + language_2_str + file_extension_in[j]
+                output_name_list.append(curr_output_name)
+                output_path = output_folder_in / curr_output_name
+                output_path_list.append(output_path)
+                
+                command = [
+                    "ffmpeg",
+                    "-i", str(video_path),
+                    "-map", f"0:{audio_index[i]}",
+                    "-c:a", codec,
+                    "-q:a", "0",
+                    str(output_path)
+                ]
+                # keep command_line for debugging
+                command_line = " ".join(command)
+ 
+                if os.path.exists(str(output_path)):
+                    if overwrite_file:
+                        os.remove(str(output_path))
+                    else:
+                        print("\nThe output path is already existed. Please delete the file or set the overwrite parameter to TRUE")
+                        return False
+                result = subprocess.run(command, text=True, stderr=subprocess.PIPE)
+                
+                if result.returncode != 0:
+                    print(f"\nError encountered: {curr_output_name}")
+                    print(result.stderr)
+                
+                elif result.returncode == 0:
+                    print(f"\nExtract audio successfully: {curr_output_name}!!!")
+                    
+                    if alarm_done:
+                        playsound(alarm_done_path)
+
+
+
 
 def make_1_season_Excel_unaligned(EN_folder_path: Union[str,Path],
                                   PT_folder_path: Union[str,Path], 
                                   out_excel_name: Union[str,Path],
                                   output_folder = None,
                                   drop_timestamp = True,
                                   ):
@@ -49,26 +382,22 @@
     out_df : TYPE
         DESCRIPTION.
 
     """
     import pandas as pd
     import sys
     from pathlib import Path
+
     
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\02 DataFrame')
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\06 General Python')
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\09 NLP_lib')
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\10 OS')
-    
-    import lib02_dataframe as ds
-    import video_tools as vt
-    import python_wizard01 as pw
-    import os_01 as ost
+    import dataframe_short as ds
+    import video_toolkit as vt
+    import python_wizard as pw
+    import os_toolkit as ost
     
-    en_df = vt.combine_files_1_season(str(EN_folder_path))
+    en_df = combine_files_1_season(str(EN_folder_path))
     en_df = en_df.add_suffix('_EN')
     # en_df.rename(columns = {'sentence':'sentence_EN',
     #                                 'start':'start_EN',
     #                                 'end':'end_EN',
     #                                 'NoSentence':'NoSentence_EN',
     #                                 },
     #              inplace = True,
@@ -79,15 +408,15 @@
     
     en_df['NoSentence_EN'] = en_df['NoSentence_EN'].astype('int')
     en_df['NoSentence_EN'] = en_df['NoSentence_EN'] + 1
     en_df = en_df.reset_index(drop = True)
 
 
 
-    pt_df = vt.combine_files_1_season(str(PT_folder_path))
+    pt_df = combine_files_1_season(str(PT_folder_path))
     pt_df = pt_df.add_suffix('_PT')
     pt_df["Episode"] = pt_df["Episode_PT"]
     pt_df = pt_df.drop(columns = ["Episode_PT"])
     # pt_df.rename(columns = {'sentence':'sentence_PT',
     #                                 'start':'start_PT',
     #                                 'end':'end_PT',
     #                                 'NoSentence':'NoSentence_PT',
@@ -106,24 +435,24 @@
 
     # Filter out rows where 'Column1' contains '♪'
     en_df_filter = en_df[~en_df['sentence_EN'].str.contains('♪', na=False)]
     pt_df_filter = pt_df[~pt_df['sentence_PT'].str.contains('♪', na=False)]
     en_df_music = en_df_filter[en_df_filter['sentence_EN'].str.contains('♪', na=False) ]
 
 
-    out_df = ds.indexAlignedAppend(en_df_filter,pt_df_filter,"Episode")
+    out_df = ds.index_aligned_append(en_df_filter,pt_df_filter,"Episode")
     out_df = out_df.reset_index(drop = True)
     out_df.index = out_df.index + 1
     # keep only the first occurrence of each column (Episode is duplicated)
     out_df = out_df.loc[:, ~out_df.columns.duplicated()]
     
     # automatically add .xlsx extension to the file 
     out_excel_name_in = out_excel_name if ".xlsx" in out_excel_name else (out_excel_name + ".xlsx")
     
-    ds.pd_move_col_front(out_df, "Episode")
+    ds.move_col_front(out_df, "Episode")
     
     if output_folder is None:
         out_excel_path = str(out_excel_name_in)
     else:
         out_excel_path = str(Path(output_folder) / Path(out_excel_name_in))
     
     if drop_timestamp:
@@ -269,16 +598,15 @@
                    sheet_name = 'Sheet1',
                    
                    n_episodes: Union[str,int] = "all",
                    portuguese_col = "F",
                    english_col = "D",
                    lang_from="PT",
                    lang_to="EN",
-                   alarm = True,
-                   alarm_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3",
+                   alarm_done:bool = True,
                    
                    ) -> pd.DataFrame:
     
     # imported from NLP 09_SenMem Pipeline
     """
     
     it would take about 1.2 min per 1 episode of BigBang(20 min)
@@ -353,15 +681,15 @@
             episode_aligned['sentence_' + lang_to  ] = episode_aligned[lang_to]
             
             episode_aligned = episode_aligned.drop(columns = [lang_from,lang_to])
             
             episode_aligned['Season'] =  season
             episode_aligned['Episode'] =  episode
             episode_aligned = episode_aligned.drop_duplicates(subset=['sentence_' + lang_from ,'sentence_' + lang_to])
-            ds.pd_move_col_front(episode_aligned, ['Season','Episode'])
+            ds.move_col_front(episode_aligned, ['Season','Episode'])
             # drop rows that are empty
             episode_aligned = episode_aligned.dropna(subset = ['sentence_' + lang_from] )
             
             season_aligned = pd.concat([season_aligned,episode_aligned])
             print(f"{episode_str} Done Aligning !!! ----------------------------------------")
         except:
             print(f"Error at {episode_str} was found !!! ########################")
@@ -390,39 +718,37 @@
     avg_per_ep = total_duration / i
     avg_per_ep /= 60
 
     print("\nTotal processing time")
     pw.print_time(total_duration)
     
     print(f"{avg_per_ep:.2f} min per episode\n")    
-    if alarm:
-        playsound(alarm_path)
+    if alarm_done:
+        playsound(alarm_done_path)
     
     return season_aligned
 
 
 def sen_alignment_df(df, lang_from = None, lang_to = None,
-                       alarm = True,
-                       alarm_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3",
+                       alarm_done:bool = True,
                      ):
     # medium tested
     if lang_from is None: lang_from = df.columns[0]
     if lang_to is None: lang_to = df.columns[1]
     
     text_list_from = df.iloc[:, 0].tolist()
     text_list_to = df.iloc[:, 1].tolist()
     # assume that text from is
-    result = sentence_alignment(text_list_from,text_list_to,lang_from,lang_to,alarm=alarm,alarm_path=alarm_path)
+    result = sentence_alignment(text_list_from,text_list_to,lang_from,lang_to,alarm_done=alarm_done)
     
     return result
     
 
 def sentence_alignment(text_from,text_to, lang_from = "pt", lang_to = "en",
-                       alarm = True,
-                       alarm_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3",
+                       alarm_done:bool = True,
                        
                        ):
     # v02 => add alarm parameter
     # text_from, text_to are expected to be text or list
     # medium tested, seem to work pretty well now
     
     import os
@@ -528,26 +854,23 @@
                                      lang_to:paragraph_to_result
                                      })
     
     ts02 = time()
     total_time = ts02-ts01
     pw.print_time(total_time)
     
-    if alarm:
-        playsound(alarm_path)
+    if alarm_done:
+        playsound(alarm_done_path)
     
     return paragraph_result
 
 
 def combine_files_1_season(folder_path):
     from functools import partial
-    import sys
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\02 DataFrame')
-    
-    import lib02_dataframe as ds
+    import dataframe_short as ds
     
     func = partial(ds.combine_files_to_df, 
                    extract_pattern = r'S\d+E\d+',
                    filename_col_name = "Episode",
                    )
     out_df = func(folder_path)
     out_df.columns.values[1] = 'NoSentence'
@@ -637,15 +960,15 @@
         'file_extension': file_extensions,
         'language': languages,
         'duration_in_min': durations
     })
     
     return info_df
 
-def get_metadata(media_path, media, language = None, file_extension = None):
+def get_metadata(media_path, media:Literal["video","audio","subtitle"], language = None, file_extension = None):
     #  not tested
     if language is None:
         language_in = None
     elif not isinstance(language, list):
         language_in = [language]
     else:
         language_in = list(language)
@@ -738,46 +1061,52 @@
         output_folder:    Union[Path,str],
         video_extension:  Union[list,str] = [".mp4",".mkv"],
         output_extension: Union[list,str] = ".mp3",
         overwrite_file:   bool = True,
         n_limit:          int = 150,
         output_prefix:    str = "",
         output_suffix:    str = "",
-        play_alarm:       bool = True,
-        alarm_done_path:str = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
+        alarm_done:       bool = True,
 ):
+    """
+    the diff between 
+    extract_audio1 - use manually code to loop through folder
+    extract_audio2 - powered by _extract_media_setup while 
+    extract_audio3 - use extract_audio_1file as a base(which is more general than extract_audio1 & extract_audio2), but need more testing to see if it works
+    
+    # after testing I would then rename extract_audio3 to just extract_audio
+    
+    """
     input_param = {
         'video_path': 6
     }
 
     _extract_media_setup(
         input_folder = video_folder,
         output_folder = output_folder,
         input_extension = video_extension,
         output_extension = output_extension,
         extract_1_file_func = extract_1_audio,
         overwrite_file = overwrite_file,
         n_limit = n_limit,
         output_prefix = output_prefix,
         output_suffix = output_suffix,
-        play_alarm = play_alarm,
-        alarm_done_path = alarm_done_path,
+        alarm_done = alarm_done,
     )
 
 def extract_subtitle(
         video_folder:     Union[Path,str],
         output_folder:    Union[Path,str],
         video_extension:  Union[list,str] = [".mp4",".mkv"],
         output_extension: Union[list,str] = None,
         overwrite_file:   bool = True,
         n_limit:          int = 150,
         output_prefix:    str = "",
         output_suffix:    str = "",
-        play_alarm:       bool = True,
-        alarm_done_path:str = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
+        alarm_done:       bool = True,
 ):
     input_param = {
         'video_path': 6
     }
     
     _extract_media_setup(
         input_folder = video_folder,
@@ -785,45 +1114,57 @@
         input_extension = video_extension,
         output_extension = output_extension,
         extract_1_file_func = extract_sub_1_video,
         overwrite_file = overwrite_file,
         n_limit = n_limit,
         output_prefix = output_prefix,
         output_suffix = output_suffix,
-        play_alarm = play_alarm,
-        alarm_done_path = alarm_done_path,
+        alarm_done = alarm_done,
     )
 
+# Sub
 def _extract_media_setup(
         input_folder: Union[str,Path],
         output_folder: Union[str,Path],
         extract_1_file_func: Callable,
         input_extension: Union[list[str],str],
         output_extension: Union[list[str],str],
         # input_param_name: list[str],
         overwrite_file:   bool = True,
         n_limit: int = 150,
         output_prefix:    str = "",
         output_suffix:    str = "",
-        play_alarm: bool = True,
-        alarm_done_path:str = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
-):
+        alarm_done: bool = True,
+
+        one_output_per_lang: bool = True,
+        languages: Union[List[str],None] = None,
+) -> None :
+    # 
+    
     """
     helper function to reduce code redundancy
     it would setup which/ how many files should be extracted in inputs
     how many files should be created in output 
 
+    extract_1_file_func that are compatible with this function will contain these parameters(no more no less)
+    
+    (video_path ,output_extension ,output_folder ,output_name,alarm_done,overwrite_file)
+
+    if extract_1_file_func doesn't have this requirement you need to modify the code in this function to support that manually
 
     """
+    import inspect_py as inp
+    import python_wizard as pw
+
     import sys
     from pathlib import Path
     from playsound import playsound
     from time import time, perf_counter
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\08 Other')
-    import lib08_Other as pw
+    from tqdm import tqdm
+
 
     ts01 = time()
     output_extension = [output_extension]
     output_extension_in = []
     
     # add . to extension in case it doesn't have .
     if output_extension[0] is not None:
@@ -841,56 +1182,90 @@
     # warrus operator, makes it usuable only for python >= 3.8
     (n_file := min(len(filename_list_ext),n_limit))
     filename_list_ext = filename_list_ext[:n_file]
     path_list = path_list[:n_file]
 
     filename_list = [filename.split('.')[0] for filename in filename_list_ext]
 
-    for i, filename in enumerate(filename_list):
+    for i, filename in tqdm(enumerate(filename_list),total = len(filename_list)):
         
             
         output_name = output_prefix + filename_list[i] + output_suffix
         # original_stdout = sys.stdout
         # sys.stdout = open('nul', 'w')
          
         # the problem here is that the input parameter name in extract_1_file_func
         # could be different and 
 
+        # extract_1_file_func should support only 1 output
+        # if multiple output is supported in extract_1_file_func, it could create multiple files(not tested)
+
         for j, extension in enumerate(output_extension_in):
             # input_dict = {
             #     input_param_name[0]:path_list[i],
             #     input_param_name[1]:extension,
             # }
-            extract_1_file_func(
-                video_path = path_list[i],
-                output_extension = extension,
-                output_folder = output_folder,
-                output_name = output_name,
-                play_alarm=False,
-                overwrite_file=overwrite_file)
+            extract_1_file_params = inp.input_params(extract_1_file_func)
+
+            if "languages" in extract_1_file_params:
+                
+                if pw.contain_all_items(extract_1_file_params,["one_output_per_lang","progress_bar"]):
+                    extract_1_file_func(
+                        video_path = path_list[i],
+                        output_extension = extension,
+                        output_folder = output_folder,
+                        output_name = output_name,
+                        alarm_done=False,
+                        overwrite_file=overwrite_file,
+                        one_output_per_lang = one_output_per_lang,
+                        languages = languages,
+
+                        progress_bar = False
+
+                        )
+                else:
+                    extract_1_file_func(
+                        video_path = path_list[i],
+                        output_extension = extension,
+                        output_folder = output_folder,
+                        output_name = output_name,
+                        alarm_done=False,
+                        overwrite_file=overwrite_file,
+                        languages = languages,
+
+                        )
+            else:
+
+                extract_1_file_func(
+                    video_path = path_list[i],
+                    output_extension = extension,
+                    output_folder = output_folder,
+                    output_name = output_name,
+                    alarm_done=False,
+                    overwrite_file=overwrite_file)
             print(f"extracted {output_name} successfully!!!")
         
         # sys.stdout = original_stdout
-    if play_alarm:
+    if alarm_done:
         playsound(alarm_done_path)
     ts02 = time()
     duration = ts02-ts01
     pw.print_time(duration)
     print()
     return filename_list
 
 def extract_sub_1_video(
     video_path:         Union[str,Path],
     output_folder:      Union[str,Path],
     output_name:        Union[str,Path] = None, 
     output_extension:   Union[str,list] = None,
-    play_alarm:         bool = True,
+    alarm_done:         bool = True,
     overwrite_file:     bool = True,
     language:           Union[str,list, None] = None,
-    alarm_done_path:    str = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
+
                     ):
     # medium tested
     # ToAdd feature 01: extract mutiple subtitles for many languages
     # ToAdd feature 02: select only some languages to extract
     
     
     """
@@ -906,15 +1281,15 @@
         
     output_name : str
         The name of the output audio file (without extension).
         
     file_extension : str, optional
         The desired file extension for the output audio file (default is ".mp3").
         
-    play_alarm : bool, optional
+    alarm_done : bool, optional
         Whether to play an alarm sound upon successful extraction (default is True).
         
     overwrite_file : bool, optional
         Whether to overwrite the output file if it already exists (default is True).
     
     Returns:
     --------
@@ -922,15 +1297,15 @@
         True if audio extraction is successful, False otherwise.
     
     Notes:
     ------
     - Additional feature 1: Output both .wav & .mp3 formats.
     - This function relies on FFmpeg for audio extraction, so make sure FFmpeg is installed.
     - The codec for output format is determined based on the file_extension parameter.
-    - An alarm sound is played if play_alarm is set to True upon successful extraction.
+    - An alarm sound is played if alarm_done is set to True upon successful extraction.
     - If the output file already exists and overwrite_file is set to False, the function will return False.
     
     Example:
     --------
     extract_1_audio("input_video.mp4", "output_folder", "output_audio", file_extension=".wav")
     
     """
@@ -1003,35 +1378,33 @@
     if result.returncode != 0:
         print("Error encountered:")
         print(result.stderr)
     
     elif result.returncode == 0:
         # print("Extract audio successfully!!!")
         
-        if play_alarm:
+        if alarm_done:
             playsound(alarm_done_path)
 
 
 
 def crop_video(
         video_path: str, 
         t_start: str, 
         t_end: str, 
         time_slice: List[Tuple[str, str]],
         output_extension: Literal["mp3", ".mp3",".mp4","mp4","mkv",".mkv","wav",".wav"] = None,
-        play_alarm = True
+        alarm_done = True
         ):
     # tested only input(mkv) => output(mkv)
     import subprocess
     import os
     from playsound import playsound
     
     
-    alarm_done_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
-    
     # Construct the base output filename
     base_name = os.path.splitext(video_path)[0]
     
     if output_extension is None:
         extension_in = os.path.splitext(video_path)[1][1:]
     else:
         extension_in = (output_extension.split(".")[1]) if "." in output_extension else output_extension
@@ -1053,15 +1426,15 @@
     if result.returncode != 0:
         print("Error encountered:")
         print(result.stderr)
     
     elif result.returncode == 0:
         print("Extract audio successfully!!!")
         
-        if play_alarm:
+        if alarm_done:
             playsound(alarm_done_path)
     
     return output_path  # Return the output file path
 
 
 
 def is_ffmpeg_installed():
@@ -1075,14 +1448,18 @@
     except subprocess.CalledProcessError:
         # An error occurred while running FFmpeg, it might not be installed or in PATH
         print("FFmpeg is not installed.")
     except FileNotFoundError:
         # FFmpeg is not in PATH
         print("FFmpeg is installed but not in PATH.")
 
+def language_name_list():
+    import pycountry
+    language_names = [lang.name for lang in pycountry.languages if hasattr(lang, 'name')]
+    return language_names
 
 def closest_language(misspelled_language):
     
     from fuzzywuzzy import process
     import pycountry
     # Get a list of all language names
     language_names = [lang.name for lang in pycountry.languages if hasattr(lang, 'name')]
@@ -1126,15 +1503,15 @@
     correct_language = closest_language(misspelled_language)
     return Language.find(correct_language)
     
 def extract_1_audio(video_path:     Union[str,Path],
                     output_folder:  Union[str,Path],
                     output_name:    Union[str,Path], 
                     file_extension: Union[str,list] = ".mp3",
-                    play_alarm:     bool = True,
+                    alarm_done:     bool = True,
                     overwrite_file: bool = True
                     ):
     # Additional feature 1: output both .wav & .mp3
     
     
     """
     Extract audio from a video file and save it in the specified format.
@@ -1149,15 +1526,15 @@
         
     output_name : str
         The name of the output audio file (without extension).
         
     file_extension : str, optional
         The desired file extension for the output audio file (default is ".mp3").
         
-    play_alarm : bool, optional
+    alarm_done : bool, optional
         Whether to play an alarm sound upon successful extraction (default is True).
         
     overwrite_file : bool, optional
         Whether to overwrite the output file if it already exists (default is True).
     
     Returns:
     --------
@@ -1165,48 +1542,44 @@
         True if audio extraction is successful, False otherwise.
     
     Notes:
     ------
     - Additional feature 1: Output both .wav & .mp3 formats.
     - This function relies on FFmpeg for audio extraction, so make sure FFmpeg is installed.
     - The codec for output format is determined based on the file_extension parameter.
-    - An alarm sound is played if play_alarm is set to True upon successful extraction.
+    - An alarm sound is played if alarm_done is set to True upon successful extraction.
     - If the output file already exists and overwrite_file is set to False, the function will return False.
     
     Example:
     --------
     extract_1_audio("input_video.mp4", "output_folder", "output_audio", file_extension=".wav")
     
     """
     
     from pathlib import Path
     import subprocess
     from playsound import playsound
     import os
     
-    codec_dict = {'.mp3': "libmp3lame",
-                  'mp3' : "libmp3lame",
-                  '.wav': "pcm_s24le",
-                  'wav' : "pcm_s24le"
-                  }
     
-    codec = codec_dict[file_extension]
+    
+    codec = CODEC_DICT[file_extension]
     
     output_folder_in = Path(output_folder)
     
     if isinstance(file_extension, str):
         if file_extension not in output_name:
             
             if "." not in file_extension:
                 file_extension = "." + file_extension
             output_name += file_extension
     
     output_path = output_folder / output_name
     
-    alarm_done_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
+
     
     
     command = [
         "ffmpeg",
         "-i", str(video_path),
         # "-map", "0:a:m:language:por",
         "-c:a", codec,
@@ -1225,24 +1598,24 @@
     if result.returncode != 0:
         print("Error encountered:")
         print(result.stderr)
     
     elif result.returncode == 0:
         print("Extract audio successfully!!!")
         
-        if play_alarm:
+        if alarm_done:
             playsound(alarm_done_path)
 
-def extract_audio(video_folder:     Union[Path,str],
+def extract_audio1(video_folder:     Union[Path,str],
                   output_folder:    Union[Path,str],
                   video_extension:  Union[list,str] = [".mp4",".mkv"],
                   output_extension: Union[list,str] = ".mp3",
                   output_prefix:    str = "",
                   output_suffix:    str = "",
-                  play_alarm:       bool = True,
+                  alarm_done:       bool = True,
                   overwrite_file:   bool = True,
                   n_limit:          int = 150
                   ):
     # TODO 
     # add feature: support multiple languages
     # support multiple output eg [.wav,.mp3,.eac3]
     
@@ -1265,15 +1638,15 @@
         
     output_prefix : str, optional
         A prefix to be added to the output audio file names. Defaults to an empty string.
         
     output_suffix : str, optional
         A suffix to be added to the output audio file names. Defaults to an empty string.
         
-    play_alarm : bool, optional
+    alarm_done : bool, optional
         Whether to play an alarm sound when the extraction is completed. Defaults to True.
         
     overwrite_file : bool, optional
         Whether to overwrite existing audio files with the same name in the `output_folder`. Defaults to True.
         
     n_limit : int, optional
         The maximum number of video files to process. Defaults to 150.
@@ -1285,19 +1658,17 @@
     import sys
     from pathlib import Path
     from playsound import playsound
     
     from time import time
     ts01 = time()
     
-    alarm_done_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
     
-    sys.path.append(r"C:\Users\Heng2020\OneDrive\Python MyLib")
-    import lib08_SrtToCsv as f8
-    import lib08_Other as f9
+    import os_toolkit as ost
+    import python_wizard as pw
     
     codec_dict = {'.mp3': "libmp3lame",
                   'mp3' : "libmp3lame",
                   '.wav': "pcm_s24le",
                   'wav' : "pcm_s24le"
                   }
     
@@ -1307,16 +1678,16 @@
     # add . to extension in case it doesn't have .
     for extension in output_extension:
         if not "." in extension:
             output_extension_in.append("."+extension)
         else:
             output_extension_in.append(extension)
     
-    video_name_list_ext = f8.get_filename(video_folder,video_extension)
-    video_path_list = f8.get_full_filename(video_folder,video_extension)
+    video_name_list_ext = ost.get_filename(video_folder,video_extension)
+    video_path_list = ost.get_full_filename(video_folder,video_extension)
     
     n_file = min(len(video_name_list_ext),n_limit)
     video_name_list_ext = video_name_list_ext[:n_file]
     video_path_list = video_path_list[:n_file]
     
     video_name_list = [filename.split('.')[0] for filename in video_name_list_ext]
     
@@ -1329,88 +1700,40 @@
         
         for i, extension in enumerate(output_extension_in):
             extract_1_audio(
                 video_path = video_path_list[i],
                 output_folder = output_folder,
                 output_name = output_name,
                 file_extension = extension,
-                play_alarm=False,
+                alarm_done=False,
                 overwrite_file=overwrite_file)
         
         # sys.stdout = original_stdout
         
-    if play_alarm:
+    if alarm_done:
         playsound(alarm_done_path)
     ts02 = time()
     duration = ts02-ts01
-    f9.print_time(duration)
+    pw.print_time(duration)
     
     return video_name_list
        
 
-def test_extract_1_audio():
-    
-    folder = Path(r"E:\Videos\The Big Bang Theory\The Big Bang Theory French Season 06")
-    video_name = "The Big Bang Theory French S06E01.mp4"
-    video_path = folder / video_name
-    output_folder = Path(r"C:\Users\Heng2020\OneDrive\Python NLP\NLP 06_ffmpeg")
-    output_name = "The Big Bang Theory French S06E01.mp3"
-    output_path = output_folder / output_name
-    
-    extract_1_audio(video_path,output_folder,output_name)
-    extract_1_audio(video_path,output_folder,output_name,overwrite_file = False)
-
-def test_extract_audio():
-    
-    from pathlib import Path
-    French_bigbang = Path(r"E:\Videos\The Big Bang Theory\The Big Bang Theory French Season 06")
-    output_folder = Path(r"E:\Videos\The Big Bang Theory\The Big Bang Theory French Season 06\Audio")
-    extract_audio(French_bigbang,output_folder,n_limit=10)
-    return True
-
-def test_crop_video():
-    from pathlib import Path
-    video_path = r"C:\Users\Heng2020\OneDrive\Python NLP\InputData\Westworld S04E01 Portuguese.mkv"
-    t1 = "0:02:25"
-    t2 = "0:06:00"
-    
-    crop_video(video_path,t1,t2)
-
-def test_create_subtitle():
-    import whisper
-    from whisper.utils import get_writer
-    from playsound import playsound
-    from time import time
-    
-    alarm_done_path = r"H:\D_Music\Sound Effect positive-logo-opener.mp3"
-    
-    ts01 = time()
-    
-    input_path = r"C:\Users\Heng2020\OneDrive\Python NLP\InputData\Westworld S04E01 Portuguese_01.mkv"
-    
-    model = whisper.load_model("base")
-    result = model.transcribe(input_path)
-    
-    output_directory = r"C:\Users\Heng2020\OneDrive\Python NLP\InputData\Westworld S04E01 Portuguese_01.srt"
-    
-    writer = get_writer("srt", str(output_directory))
-    writer(result, output_name)
-    ts02 = time()
-    
-    duration = ts02 - ts01 
-    print(duration)
 
 
 def srt_to_df(srt_path,
               remove_stopwords=True,
               stopwords = ["♪","\n","<i>","</i>","<b>","</b>"]):
 # remove_newline will remove '\n' from the extracted text
     import pysrt
     import pandas as pd
-    if ".srt" in srt_path:
+    import py_string_tool as pst
+    import os_toolkit as ost
+
+    if ".srt" in str(srt_path):
         # 1 file case
         subs = pysrt.open(srt_path)
         # Initialize empty lists for storing data
         sentences = []
         start_times = []
         end_times = []
     
@@ -1419,24 +1742,24 @@
             sentences.append(sub.text)
             start_times.append(sub.start.to_time())
             end_times.append(sub.end.to_time())
     
         # Create a DataFrame
         if remove_stopwords:
             #FIX it's still can't replace properly 
-            sentences = [St_replace(sentence,stopwords,"") for sentence in sentences]
+            sentences = [pst.replace(sentence,stopwords,"") for sentence in sentences]
         df = pd.DataFrame({
             'sentence': sentences,
             'start': start_times,
             'end': end_times
         })
         return df
     else:
         # many srt's file using folder
-        str_file_names = get_full_filename(srt_path,".srt")
+        str_file_names = ost.get_full_filename(srt_path,".srt")
         df_list = []
         for str_file_name in str_file_names:
             each_df = srt_to_df(str_file_name)
             df_list.append(each_df)
         return df_list
 
 
@@ -1462,92 +1785,31 @@
     # encoding='utf-8-sig' for Portuguese
         if pd_ver < (2,0,0):
             df_sub.to_excel(output_path, encoding=encoding,index=index)
         else:
             df_sub.to_excel(output_path, index=index)
             
     elif isinstance(df_sub,list):
-        short_names = get_filename(srt_path,".srt")
+        short_names = ost.get_filename(srt_path,".srt")
         out_full_name = [os.path.join(output_path,short_name).replace(".srt",".xlsx") for short_name in short_names]
         
         if pd_ver < (2,0,0):
             df_sub.to_excel(output_path, encoding=encoding,index=index)
             for i,df in enumerate(df_sub):
                 df.to_excel(out_full_name[i], encoding=encoding,index=index)
                 
         else:
             for i,df in enumerate(df_sub):
                 df.to_excel(out_full_name[i], index=index)
 
-def to_ms(time_obj):
+def to_ms(time_obj: datetime.time) -> float:
     time_obj_ms = (time_obj.hour * 3600 + time_obj.minute * 60 + time_obj.second) * 1000 + time_obj.microsecond // 1000
     return time_obj_ms
 
-def get_filename(folder_path,extension = "all"):
-    # also include "folder"  case
-# tested small
-# new feature1: include subfolders
-    import os
-    if extension == "all":
-        out_list = [ file for file in os.listdir(folder_path) ]
-
-    elif isinstance(extension,str):
-        extension_temp = [extension]
 
-        out_list = []
-
-        for file in os.listdir(folder_path):
-            if "." in file:
-                file_extension = file.split('.')[-1]
-                for each_extention in extension_temp:
-                    # support when it's ".csv" or only "csv"
-                    if file_extension in each_extention:
-                        out_list.append(file)
-            elif extension == "folder":
-                out_list.append(file)
-
-
-    elif isinstance(extension,list):
-        out_list = []
-        for file in os.listdir(folder_path):
-
-            if "." in file:
-                file_extension = file.split('.')[-1]
-                for each_extention in extension:
-                    # support when it's ".csv" or only "csv"
-                    if file_extension in each_extention:
-                        out_list.append(file)
-
-            elif "folder" in extension:
-                out_list.append(file)
-
-        return out_list
-
-    else:
-        print("Don't support this dataype for extension: please input only string or list")
-        return False
-
-    return out_list
-
-def get_full_filename(folder_path,extension = "all"):
-    # tested small
-    import os 
-    short_names = get_filename(folder_path,extension)
-    out_list = []
-    for short_name in short_names:
-        full_name = os.path.join(folder_path,short_name)
-        out_list.append(full_name)
-    return out_list
-
-def St_replace(text,to_replace,replace_by):
-    # unit_tested
-    for word in to_replace:
-        new_text = text.replace(word, replace_by)
-        
-    return new_text
 
 # TODO: srt_to_Excel => similar to srt_to_csv but output as excel
 # srt_to_Excel(srt_path,sub_output)
 
 # n_file = len(srt_to_df(srt_folder_path))
 # srt_to_Excel(srt_folder_path,output_folder)
```

