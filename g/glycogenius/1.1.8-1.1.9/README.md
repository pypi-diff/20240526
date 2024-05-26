# Comparing `tmp/glycogenius-1.1.8.tar.gz` & `tmp/glycogenius-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glycogenius-1.1.8.tar", last modified: Tue Apr  2 12:31:30 2024, max compression
+gzip compressed data, was "glycogenius-1.1.9.tar", last modified: Thu Apr  4 14:17:15 2024, max compression
```

## Comparing `glycogenius-1.1.8.tar` & `glycogenius-1.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.469316 glycogenius-1.1.8/
--rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     5066 2024-04-02 12:31:30.469316 glycogenius-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4405 2024-01-24 20:27:19.000000 glycogenius-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.444391 glycogenius-1.1.8/glycogenius/
--rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.8/glycogenius/LICENSE.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.468303 glycogenius-1.1.8/glycogenius/Modules/
--rw-rw-rw-   0        0        0    43400 2024-04-01 13:11:42.000000 glycogenius-1.1.8/glycogenius/Modules/CLI.py
--rw-rw-rw-   0        0        0    19461 2024-04-01 13:33:48.000000 glycogenius-1.1.8/glycogenius/Modules/Config_Handler.py
--rw-rw-rw-   0        0        0   159861 2024-04-01 18:12:43.000000 glycogenius-1.1.8/glycogenius/Modules/Execution_Functions.py
--rw-rw-rw-   0        0        0    42498 2024-04-01 01:34:38.000000 glycogenius-1.1.8/glycogenius/Modules/File_Accessing.py
--rw-rw-rw-   0        0        0    27665 2024-03-25 13:41:16.000000 glycogenius-1.1.8/glycogenius/Modules/General_Functions.py
--rw-rw-rw-   0        0        0    30178 2024-03-31 01:55:59.000000 glycogenius-1.1.8/glycogenius/Modules/Library_Tools.py
--rw-rw-rw-   0        0        0        0 2023-12-15 19:43:14.000000 glycogenius-1.1.8/glycogenius/Modules/__init__.py
--rw-rw-rw-   0        0        0     3667 2024-03-25 20:18:12.000000 glycogenius-1.1.8/glycogenius/Modules/core.py
--rw-rw-rw-   0        0        0    10155 2024-04-01 13:10:33.000000 glycogenius-1.1.8/glycogenius/Parameters_Template.py
--rw-rw-rw-   0        0        0       64 2024-03-23 12:11:11.000000 glycogenius-1.1.8/glycogenius/__init__.py
--rw-rw-rw-   0        0        0       69 2024-03-22 21:56:00.000000 glycogenius-1.1.8/glycogenius/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:30.468303 glycogenius-1.1.8/glycogenius.egg-info/
--rw-rw-rw-   0        0        0     5066 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 12:31:30.000000 glycogenius-1.1.8/glycogenius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:31:30.470314 glycogenius-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2038 2024-04-02 12:31:29.000000 glycogenius-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:17:15.574321 glycogenius-1.1.9/
+-rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     5066 2024-04-04 14:17:15.573311 glycogenius-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4405 2024-01-24 20:27:19.000000 glycogenius-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 14:17:15.406973 glycogenius-1.1.9/glycogenius/
+-rw-rw-rw-   0        0        0    33094 2023-12-28 12:56:50.000000 glycogenius-1.1.9/glycogenius/LICENSE.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:17:15.568115 glycogenius-1.1.9/glycogenius/Modules/
+-rw-rw-rw-   0        0        0    43400 2024-04-01 13:11:42.000000 glycogenius-1.1.9/glycogenius/Modules/CLI.py
+-rw-rw-rw-   0        0        0    19461 2024-04-01 13:33:48.000000 glycogenius-1.1.9/glycogenius/Modules/Config_Handler.py
+-rw-rw-rw-   0        0        0   159839 2024-04-04 12:11:56.000000 glycogenius-1.1.9/glycogenius/Modules/Execution_Functions.py
+-rw-rw-rw-   0        0        0    42512 2024-04-04 14:16:33.000000 glycogenius-1.1.9/glycogenius/Modules/File_Accessing.py
+-rw-rw-rw-   0        0        0    27665 2024-03-25 13:41:16.000000 glycogenius-1.1.9/glycogenius/Modules/General_Functions.py
+-rw-rw-rw-   0        0        0    30178 2024-03-31 01:55:59.000000 glycogenius-1.1.9/glycogenius/Modules/Library_Tools.py
+-rw-rw-rw-   0        0        0        0 2023-12-15 19:43:14.000000 glycogenius-1.1.9/glycogenius/Modules/__init__.py
+-rw-rw-rw-   0        0        0     3667 2024-03-25 20:18:12.000000 glycogenius-1.1.9/glycogenius/Modules/core.py
+-rw-rw-rw-   0        0        0    10155 2024-04-01 13:10:33.000000 glycogenius-1.1.9/glycogenius/Parameters_Template.py
+-rw-rw-rw-   0        0        0       64 2024-03-23 12:11:11.000000 glycogenius-1.1.9/glycogenius/__init__.py
+-rw-rw-rw-   0        0        0       69 2024-03-22 21:56:00.000000 glycogenius-1.1.9/glycogenius/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:17:15.570118 glycogenius-1.1.9/glycogenius.egg-info/
+-rw-rw-rw-   0        0        0     5066 2024-04-04 14:17:15.000000 glycogenius-1.1.9/glycogenius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-04-04 14:17:15.000000 glycogenius-1.1.9/glycogenius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:17:15.000000 glycogenius-1.1.9/glycogenius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-04 14:17:15.000000 glycogenius-1.1.9/glycogenius.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-04-04 14:17:15.000000 glycogenius-1.1.9/glycogenius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 14:17:15.000000 glycogenius-1.1.9/glycogenius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:17:15.575787 glycogenius-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2038 2024-04-04 14:17:14.000000 glycogenius-1.1.9/setup.py
```

### Comparing `glycogenius-1.1.8/LICENSE` & `glycogenius-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/PKG-INFO` & `glycogenius-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glycogenius
-Version: 1.1.8
+Version: 1.1.9
 Summary: GlycoGenius is an all-in-one solution for data analysis of glycomics data.
 Author: Hector Franco Loponte
 Author-email: hectorfloponte@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `glycogenius-1.1.8/README.md` & `glycogenius-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/LICENSE.py` & `glycogenius-1.1.9/glycogenius/LICENSE.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/Modules/CLI.py` & `glycogenius-1.1.9/glycogenius/Modules/CLI.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/Modules/Config_Handler.py` & `glycogenius-1.1.9/glycogenius/Modules/Config_Handler.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/Modules/Execution_Functions.py` & `glycogenius-1.1.9/glycogenius/Modules/Execution_Functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2125,15 +2125,15 @@
     for i_i, i in enumerate(samples_names):
         isotopic_fits_dataframes.append({})
         raw_eic_dataframes.append({})
         eic_dataframes.append({})
         smoothed_eic_dataframes.append({})
         temp_eic_rt = []
         for j in analyzed_data[1][i_i]:
-            temp_eic_rt.append(float("%.4f" % round(j, 4)))
+            temp_eic_rt.append(j)
         raw_eic_dataframes[i_i]['RTs_'+str(i_i)] = temp_eic_rt
         eic_dataframes[i_i]['RTs_'+str(i_i)] = temp_eic_rt
         smoothed_eic_dataframes[i_i]['RTs_'+str(i_i)] = temp_eic_rt
         curve_fitting_dataframes.append({})
         df2["Sample_Number"].append(i_i)
         df2["File_Name"].append(i)
         df2["Average_Noise_Level"].append(float("%.1f" % round(analyzed_data[2][i_i],1)))
@@ -2172,15 +2172,15 @@
                 temp_aucs = []
                 temp_ppm = []
                 temp_s_n = []
                 temp_iso_score = []
                 temp_curve_score = []
                 temp_curve_data_total = []
                 for l_l, l in enumerate(analyzed_data[0][i]['Adducts_mz_data'][j][k][1]):
-                    temp_rts.append(float("%.2f" % round(l['rt'], 2)))
+                    temp_rts.append(float("%.4f" % round(l['rt'], 4)))
                     temp_aucs.append(float("%.2f" % round(l['AUC'], 2)))
                     temp_ppm.append(float("%.2f" % round(l['Average_PPM'][0], 2)))
                     temp_s_n.append(float("%.1f" % round(l['Signal-to-Noise'], 1)))
                     if isnan(l['Iso_Fit_Score']):
                         temp_iso_score.append(0.0)
                     else:
                         temp_iso_score.append(float("%.4f" % round(l['Iso_Fit_Score'], 4)))
@@ -2219,24 +2219,24 @@
                         if len(temp_fragments) != 0:
                             for m in temp_fragments:
                                 fragments_dataframes[k_k]["Glycan"].append(m[0])
                                 fragments_dataframes[k_k]["Adduct"].append(m[1])
                                 fragments_dataframes[k_k]["Fragment"].append(m[2])
                                 fragments_dataframes[k_k]["Fragment_mz"].append(float("%.4f" % round(m[3], 4)))
                                 fragments_dataframes[k_k]["Fragment_Intensity"].append(float("%.2f" % round(m[4], 2)))
-                                fragments_dataframes[k_k]["RT"].append(float("%.2f" % round(m[5],2)))
+                                fragments_dataframes[k_k]["RT"].append(float("%.4f" % round(m[5],4)))
                                 fragments_dataframes[k_k]["Precursor_mz"].append(float("%.4f" % round(m[6], 4)))
                                 fragments_dataframes[k_k]["% TIC explained"].append(float(m[7]))
                             df1[k_k]["Detected_Fragments"].append('Yes')
                         else:
                             df1[k_k]["Detected_Fragments"].append('No')
                     for m_m, m in enumerate(temp_rts):
                         temp_array = []
                         for n in temp_curve_data_total[m_m][0]:
-                            temp_array.append(float("%.4f" % round(n, 4)))
+                            temp_array.append(float("%.4f" % round(n,4)))
                         curve_fitting_dataframes[k_k][str(i)+"+"+str(j)+"_"+str(m)+"_RTs"] = temp_array
                         temp_array = []
                         for n in temp_curve_data_total[m_m][1]:
                             temp_array.append(int(n))
                         curve_fitting_dataframes[k_k][str(i)+"+"+str(j)+"_"+str(m)+"_Found_ints"] = temp_array
                         temp_array = []
                         for n in temp_curve_data_total[m_m][2]:
@@ -2548,15 +2548,15 @@
                                      rt_array_report,
                                      ms1_id,
                                      i,
                                      i_i)
             results.append(result)
             if from_GUI:
                 temp_results.append(result)
-                if len(temp_results) == cpu_count:
+                if len(temp_results) == cpu_count+1:
                     for k_k, k in enumerate(temp_results):
                         k.result()
                         del temp_results[k_k]
                         if len(temp_results) < cpu_count:
                             break
                 print('Analyzing glycan '+str(i)+': '+str(i_i+1)+'/'+str(lib_size))
     for i in results:
@@ -2962,15 +2962,15 @@
                                      unrestricted_fragments,
                                      rt_tolerance,
                                      i_i,
                                      i)
             results.append(result)
             if from_GUI:
                 temp_results.append(result)
-                if len(temp_results) == cpu_count:
+                if len(temp_results) == cpu_count+1:
                     for k_k, k in enumerate(temp_results):
                         k.result()
                         del temp_results[k_k]
                         if len(temp_results) < cpu_count:
                             break
                 print('Analyzing glycan '+str(i)+': '+str(i_i+1)+'/'+str(len(analyzed_data[0])))
             
@@ -3066,15 +3066,15 @@
                     if abs((k[l]['precursorMz'][0]['precursorMz']) - analyzed_data[0][i]['Adducts_mz'][j]) <= (1.0074/General_Functions.form_to_charge(j))+General_Functions.tolerance_calc(tolerance[0], tolerance[1], analyzed_data[0][i]['Adducts_mz'][j]): #checks if precursor matches adduct mz
                         found_count = 0
                         total = sum(k[l]['intensity array'])
                         former_peak_mz = 0
                         max_int = max(k[l]['intensity array'])
                         for m_m, m in enumerate(k[l]['m/z array']):
                         
-                            if k[l]['intensity array'][m_m] < max_int*0.1: #this avoids picking on super small intensity peaks... since MS2 data noise is sometimes almost boolean, it's easier to just filter by intensity related to base peak
+                            if k[l]['intensity array'][m_m] < max_int*0.05: #this avoids picking on super small intensity peaks... since MS2 data noise is sometimes almost boolean, it's easier to just filter by intensity related to base peak
                                 continue
                                 
                             if abs(m+former_peak_mz+General_Functions.h_mass) < General_Functions.tolerance_calc(tolerance[0], tolerance[1], m) or abs(m-former_peak_mz+(General_Functions.h_mass/2)) < General_Functions.tolerance_calc(tolerance[0], tolerance[1], m): #this stack makes it so that fragments are not picked as peaks of the envelope of former peaks. checks for singly or doubly charged fragments only
                                 former_peak_mz = m
                                 continue
                             former_peak_mz = m
```

### Comparing `glycogenius-1.1.8/glycogenius/Modules/File_Accessing.py` & `glycogenius-1.1.9/glycogenius/Modules/File_Accessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
     def __iter__(self):
         return self.it
     def __getitem__(self,index):
         if type(index) == int:
             pre_data = self.it[index]
             if pre_data['ms level'] == 2:
                 if float(self.it[-1]['scanList']['scan'][0]['scan start time']) > 210: #210 scan time should allow for the correct evaluation of scan time being in seconds or minutes for every run that lasts between 3.5 minutes and 3.5 hours
-                    return {'num': pre_data['id'].split('=')[-1], 'retentionTime': float(pre_data['scanList']['scan'][0]['scan start time'])/60, 'msLevel': pre_data['ms level'], 'm/z array': pre_data['m/z array'], 'intensity array': pre_data['intensity array'], 'precursorMz': [{'precursorMz': pre_data['precursorList']['precursor'][0]['isolationWindow']['isolation window target m/z']}]}
+                    return {'num': pre_data['id'].split('=')[-1], 'retentionTime': float(pre_data['scanList']['scan'][0]['scan start time'])/60, 'msLevel': pre_data['ms level'], 'm/z array': pre_data['m/z array'], 'intensity array': pre_data['intensity array'], 'precursorMz': [{'precursorMz': pre_data['precursorList']['precursor'][0]['selectedIonList']['selectedIon'][0]['selected ion m/z']}]}
                 else:
-                    return {'num': pre_data['id'].split('=')[-1], 'retentionTime': float(pre_data['scanList']['scan'][0]['scan start time']), 'msLevel': pre_data['ms level'], 'm/z array': pre_data['m/z array'], 'intensity array': pre_data['intensity array'], 'precursorMz': [{'precursorMz': pre_data['precursorList']['precursor'][0]['isolationWindow']['isolation window target m/z']}]}
+                    return {'num': pre_data['id'].split('=')[-1], 'retentionTime': float(pre_data['scanList']['scan'][0]['scan start time']), 'msLevel': pre_data['ms level'], 'm/z array': pre_data['m/z array'], 'intensity array': pre_data['intensity array'], 'precursorMz': [{'precursorMz': pre_data['precursorList']['precursor'][0]['selectedIonList']['selectedIon'][0]['selected ion m/z']}]}
             else:
                 if float(self.it[-1]['scanList']['scan'][0]['scan start time']) > 210:
                     return {'num': pre_data['id'].split('=')[-1], 'retentionTime': float(pre_data['scanList']['scan'][0]['scan start time'])/60, 'msLevel': pre_data['ms level'], 'm/z array': pre_data['m/z array'], 'intensity array': pre_data['intensity array']}
                 else:
                     return {'num': pre_data['id'].split('=')[-1], 'retentionTime': float(pre_data['scanList']['scan'][0]['scan start time']), 'msLevel': pre_data['ms level'], 'm/z array': pre_data['m/z array'], 'intensity array': pre_data['intensity array']}
         else:
             first_index = str(index).split('(')[1].split(', ')[0]
@@ -552,15 +552,15 @@
             iso_quali = 0.0
             
         if len(mono_ppm) > 0:
             ppm_error = mean(mono_ppm)
         else:
             ppm_error = inf
         
-        buffer.append(([glycan_id, file_id, ms1_id, float("%.2f" % round(ret_time, 2))], [ppm_error, iso_quali, intensity, [mz_isos, iso_target, iso_actual, iso_quali]]))
+        buffer.append(([glycan_id, file_id, ms1_id, float("%.4f" % round(ret_time, 4))], [ppm_error, iso_quali, intensity, [mz_isos, iso_target, iso_actual, iso_quali]]))
         
     #dinamical clean-up of buffer
     min_in_a_row = 3
     buffer_size = 10
     if len(buffer) >= buffer_size or ms1_id == last_ms1_id: 
         highest_in_a_row = 0
         in_a_row = 0
```

### Comparing `glycogenius-1.1.8/glycogenius/Modules/General_Functions.py` & `glycogenius-1.1.9/glycogenius/Modules/General_Functions.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/Modules/Library_Tools.py` & `glycogenius-1.1.9/glycogenius/Modules/Library_Tools.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/Modules/core.py` & `glycogenius-1.1.9/glycogenius/Modules/core.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius/Parameters_Template.py` & `glycogenius-1.1.9/glycogenius/Parameters_Template.py`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/glycogenius.egg-info/PKG-INFO` & `glycogenius-1.1.9/glycogenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glycogenius
-Version: 1.1.8
+Version: 1.1.9
 Summary: GlycoGenius is an all-in-one solution for data analysis of glycomics data.
 Author: Hector Franco Loponte
 Author-email: hectorfloponte@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `glycogenius-1.1.8/glycogenius.egg-info/SOURCES.txt` & `glycogenius-1.1.9/glycogenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glycogenius-1.1.8/setup.py` & `glycogenius-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     for lines in f:
         if lines[0] != "!":
             long_description_from_file+= lines
     f.close()
 
 setup(
     name='glycogenius',
-    version='1.1.8',
+    version='1.1.9',
     author='Hector Franco Loponte',
     author_email='hectorfloponte@gmail.com',
     description='GlycoGenius is an all-in-one solution for data analysis of glycomics data.',
     long_description=long_description_from_file,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

