# Comparing `tmp/tsugu-2.0.7.tar.gz` & `tmp/tsugu-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-2.0.7.tar", last modified: Thu May 23 13:39:31 2024, max compression
+gzip compressed data, was "tsugu-2.0.8.tar", last modified: Sun May 26 15:25:48 2024, max compression
```

## Comparing `tsugu-2.0.7.tar` & `tsugu-2.0.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.563161 tsugu-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-23 13:39:23.000000 tsugu-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-23 13:39:31.563161 tsugu-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-23 13:39:23.000000 tsugu-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:39:31.563161 tsugu-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 13:39:23.000000 tsugu-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.555161 tsugu-2.0.7/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.555161 tsugu-2.0.7/tsugu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.559161 tsugu-2.0.7/tsugu/src/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.559161 tsugu-2.0.7/tsugu/src/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/help/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.559161 tsugu-2.0.7/tsugu/src/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.563161 tsugu-2.0.7/tsugu/src/universal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/src/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.563161 tsugu-2.0.7/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-23 13:39:23.000000 tsugu-2.0.7/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:39:31.555161 tsugu-2.0.7/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-23 13:39:31.000000 tsugu-2.0.7/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-23 13:39:31.000000 tsugu-2.0.7/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:39:31.000000 tsugu-2.0.7/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 13:39:31.000000 tsugu-2.0.7/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 13:39:31.000000 tsugu-2.0.7/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.915341 tsugu-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-26 15:25:40.000000 tsugu-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-26 15:25:48.915341 tsugu-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-26 15:25:40.000000 tsugu-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 15:25:48.915341 tsugu-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-26 15:25:40.000000 tsugu-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.911341 tsugu-2.0.8/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.911341 tsugu-2.0.8/tsugu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.911341 tsugu-2.0.8/tsugu/src/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.911341 tsugu-2.0.8/tsugu/src/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.911341 tsugu-2.0.8/tsugu/src/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.915341 tsugu-2.0.8/tsugu/src/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/src/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.915341 tsugu-2.0.8/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-26 15:25:40.000000 tsugu-2.0.8/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:25:48.911341 tsugu-2.0.8/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-26 15:25:48.000000 tsugu-2.0.8/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-26 15:25:48.000000 tsugu-2.0.8/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:25:48.000000 tsugu-2.0.8/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-26 15:25:48.000000 tsugu-2.0.8/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 15:25:48.000000 tsugu-2.0.8/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-2.0.7/LICENSE` & `tsugu-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/PKG-INFO` & `tsugu-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.7
+Version: 2.0.8
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.7 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.8 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.7/README.md` & `tsugu-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/setup.py` & `tsugu-2.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='2.0.7',
+    version='2.0.8',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
     packages=find_packages(exclude=('test','test*')),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
-            "loguru==0.7.2",
+            "loguru",
             "tsugu-api-python==1.2.0",
             "arclet-alconna==1.8.13",
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-2.0.7/tsugu/handler.py` & `tsugu-2.0.8/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/__init__.py` & `tsugu-2.0.8/tsugu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/bandoristation/rooms_forward.py` & `tsugu-2.0.8/tsugu/src/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/bandoristation/ycm.py` & `tsugu-2.0.8/tsugu/src/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/help/help.py` & `tsugu-2.0.8/tsugu/src/help/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/bind_player.py` & `tsugu-2.0.8/tsugu/src/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/bind_player_verification_off.py` & `tsugu-2.0.8/tsugu/src/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/bind_player_verification_on.py` & `tsugu-2.0.8/tsugu/src/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/change_default_server.py` & `tsugu-2.0.8/tsugu/src/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/change_server_mode.py` & `tsugu-2.0.8/tsugu/src/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/player_status.py` & `tsugu-2.0.8/tsugu/src/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/switch_car_forwarding_off.py` & `tsugu-2.0.8/tsugu/src/remote/switch_car_forwarding_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/switch_car_forwarding_on.py` & `tsugu-2.0.8/tsugu/src/remote/switch_car_forwarding_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/remote/unbind_player.py` & `tsugu-2.0.8/tsugu/src/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/event_stage.py` & `tsugu-2.0.8/tsugu/src/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/gacha_simulate.py` & `tsugu-2.0.8/tsugu/src/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/get_card_illustration.py` & `tsugu-2.0.8/tsugu/src/universal/get_card_illustration.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/lsycx.py` & `tsugu-2.0.8/tsugu/src/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/search_card.py` & `tsugu-2.0.8/tsugu/src/universal/search_card.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/search_character.py` & `tsugu-2.0.8/tsugu/src/universal/search_character.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/search_event.py` & `tsugu-2.0.8/tsugu/src/universal/search_event.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/search_gacha.py` & `tsugu-2.0.8/tsugu/src/universal/search_gacha.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/search_player.py` & `tsugu-2.0.8/tsugu/src/universal/search_player.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
         user = get_user(user_id, platform)
         if res.serverName:
-            server = res.serverName
+            server = server_name_2_server_id(res.serverName)
         else:
             server = user.server_mode
+        print(res.playerId, server)
         return tsugu_api.search_player(res.playerId, server)
 
     return res
 
 
 async def handler_async(message: str, user_id: str, platform: str, channel_id: str):
     res = alc.parse(message)
 
     if res.matched:
         user = get_user(user_id, platform)
         if res.serverName:
-            server = res.serverName
+            server = server_name_2_server_id(res.serverName)
         else:
             server = user.server_mode
         return await tsugu_api_async.search_player(res.playerId, server)
 
     return res
```

### Comparing `tsugu-2.0.7/tsugu/src/universal/search_song.py` & `tsugu-2.0.8/tsugu/src/universal/search_song.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/song_chart.py` & `tsugu-2.0.8/tsugu/src/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/song_meta.py` & `tsugu-2.0.8/tsugu/src/universal/song_meta.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/ycx.py` & `tsugu-2.0.8/tsugu/src/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/src/universal/ycx_all.py` & `tsugu-2.0.8/tsugu/src/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu/utils/__init__.py` & `tsugu-2.0.8/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-2.0.7/tsugu.egg-info/PKG-INFO` & `tsugu-2.0.8/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 2.0.7
+Version: 2.0.8
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 2.0.7 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 2.0.8 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ## ð¦ å®è£ ```shell pip install tsugu --upgrade ``` > API powered by
```

### Comparing `tsugu-2.0.7/tsugu.egg-info/SOURCES.txt` & `tsugu-2.0.8/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

