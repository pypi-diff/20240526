# Comparing `tmp/sole_bili_get-0.0.4.tar.gz` & `tmp/sole_bili_get-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sole_bili_get-0.0.4.tar", last modified: Fri May 24 13:49:26 2024, max compression
+gzip compressed data, was "sole_bili_get-0.0.5.tar", last modified: Sun May 26 04:23:39 2024, max compression
```

## Comparing `sole_bili_get-0.0.4.tar` & `sole_bili_get-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 13:49:26.384427 sole_bili_get-0.0.4/
--rw-rw-rw-   0        0        0     1072 2024-05-18 14:01:48.000000 sole_bili_get-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     6801 2024-05-24 13:49:26.383427 sole_bili_get-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6287 2024-05-19 14:54:23.000000 sole_bili_get-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 13:49:26.384427 sole_bili_get-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1366 2024-05-18 14:42:06.000000 sole_bili_get-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:49:26.377428 sole_bili_get-0.0.4/sole_bili_get/
--rw-rw-rw-   0        0        0       76 2024-05-21 12:04:46.000000 sole_bili_get-0.0.4/sole_bili_get/__init__.py
--rw-rw-rw-   0        0        0    41224 2024-05-21 12:21:41.000000 sole_bili_get-0.0.4/sole_bili_get/bili_get.py
--rw-rw-rw-   0        0        0    10620 2024-05-24 13:47:27.000000 sole_bili_get-0.0.4/sole_bili_get/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:49:26.383427 sole_bili_get-0.0.4/sole_bili_get.egg-info/
--rw-rw-rw-   0        0        0     6801 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 13:49:26.000000 sole_bili_get-0.0.4/sole_bili_get.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 04:23:39.265572 sole_bili_get-0.0.5/
+-rw-rw-rw-   0        0        0     1072 2024-05-18 14:01:48.000000 sole_bili_get-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     7425 2024-05-26 04:23:39.264569 sole_bili_get-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6856 2024-05-26 03:57:56.000000 sole_bili_get-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 04:23:39.265572 sole_bili_get-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1703 2024-05-26 04:16:09.000000 sole_bili_get-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:23:39.259568 sole_bili_get-0.0.5/sole_bili_get/
+-rw-rw-rw-   0        0        0       76 2024-05-24 14:34:10.000000 sole_bili_get-0.0.5/sole_bili_get/__init__.py
+-rw-rw-rw-   0        0        0    44706 2024-05-26 04:18:32.000000 sole_bili_get-0.0.5/sole_bili_get/bili_get.py
+-rw-rw-rw-   0        0        0    10227 2024-05-26 03:34:38.000000 sole_bili_get-0.0.5/sole_bili_get/chrome_cookie.py
+-rw-rw-rw-   0        0        0    10894 2024-05-26 04:07:53.000000 sole_bili_get-0.0.5/sole_bili_get/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:23:39.264569 sole_bili_get-0.0.5/sole_bili_get.egg-info/
+-rw-rw-rw-   0        0        0     7425 2024-05-26 04:23:39.000000 sole_bili_get-0.0.5/sole_bili_get.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-26 04:23:39.000000 sole_bili_get-0.0.5/sole_bili_get.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 04:23:39.000000 sole_bili_get-0.0.5/sole_bili_get.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-26 04:23:39.000000 sole_bili_get-0.0.5/sole_bili_get.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-26 04:23:39.000000 sole_bili_get-0.0.5/sole_bili_get.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 04:23:39.000000 sole_bili_get-0.0.5/sole_bili_get.egg-info/top_level.txt
```

### Comparing `sole_bili_get-0.0.4/LICENSE.txt` & `sole_bili_get-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sole_bili_get-0.0.4/PKG-INFO` & `sole_bili_get-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: sole_bili_get
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple tool to download videos from bilibili{*≧∀≦}
 Home-page: https://github.com/muggledy/bili-get
 Author: muggledy
 Author-email: zgjsycfndy2015@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
+Requires-Dist: pycryptodome
+Requires-Dist: pypiwin32
 
 # Bilibili视频下载器
 
-<a alt="null">![](https://img.shields.io/badge/python-3.6+-green)&nbsp;<a href="https://pypi.org/project/sole-bili-get/" alt="null"><img src="https://img.shields.io/github/v/release/muggledy/bili-get"/></a></a>
+<a alt="null">![](https://img.shields.io/badge/python-3.6+-green)&nbsp;![](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-pink)&nbsp;<a href="https://pypi.org/project/sole-bili-get/" alt="null"><img src="https://img.shields.io/github/v/release/muggledy/bili-get"/></a></a>
 
 ## 下载
 
 ### 方式一
 
 ```console
 pip install sole-bili-get -i https://www.pypi.org/simple/
@@ -54,15 +56,15 @@
 100.00%|████████████████████| 下载完成【application/octet-stream】 84.96MB/84.96MB
 start to download p1(audio)...
 100.00%|████████████████████| 下载完成【application/octet-stream】 28.28MB/28.28MB
 ffmpeg merge success, save into C:\Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_总耗时近一年！七爷带你一步到位看完昭和《奥特曼》系列全部345集怪兽及宇宙人们！_1初代奥特曼.mp4
 Note: this is a multi-episode video, you can download them all at once with --playlist
 ```
 
-- 默认是下载到当前工作路径，可以通过`-o`或`--output`指定输出目录，不存在则自动创建，譬如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`。这会在`--output`目录下产生两个文件夹：`bili_tmp/`和`bili_output/`，前者存放一些临时文件，用于记录多剧集视频的下载进度，如果下载过程中发生中断，重新执行命令可以继续下载过程（且对于尚未合成的剧集会尝试进行合成，除非指定`--nomerge`参数），后者则是视频、音频、弹幕文件的输出文件夹
+- 默认是下载到当前工作路径，可以通过`-o`或`--output`指定输出目录，不存在则自动创建，譬如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`。这会在`--output`目录下产生两个文件夹：`bili_tmp/`和`bili_output/`，前者存放一些临时文件，用于记录多剧集视频的下载进度，如果下载过程中发生中断，重新执行命令可以继续下载过程（且对于尚未合成的剧集会尝试进行合成，除非指定`--nomerge`参数），后者则是视频、音频、封面、弹幕文件的输出文件夹
 
 - 对于多剧集视频，可以指定`--playlist`自动下载全部剧集，只要不删除对应的`bili_tmp/`临时文件，可以任意重复执行下载命令，如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP --playlist`，也不会重复下载，如果UP主新发布了剧集，则会继续下载
 
 - `-c`或`--cookie`用于指定您的B站Cookie信息，这样就可以下载1080P视频了
 
   ```console
   C:\Users\muggledy\Downloads>bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -c "your cookie"
@@ -81,22 +83,26 @@
   100.00%|████████████████████| 下载完成【video/mp4】 28.28MB/28.28MB
   ffmpeg merge success, save into C:\Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_总耗时近一年！七爷带你一步到位看完昭和《奥特曼》系列全部345集怪兽及宇宙人们！_1初代奥特曼.mp4
   Note: this is a multi-episode video, you can download them all at once with --playlist
   ```
 
   Cookie获取方式如下：
 
-  ![](https://raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+  ![B站cookie获取方式](https://raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+
+  注：如果是Windows平台使用Chrome浏览器，可以指定`-c`参数为`chrome`，程序将自动从`./AppData/Local/Google/Chrome/User Data/default/Network/Cookies`读取B站的Cookie信息，譬如我们可以通过`bili-get https://www.bilibili.com/video/BV18G411D7FM -c chrome`命令下载1080p视频
 
 - `-q`或`--quality`用于指定要下载的视频质量（清晰度），可选值有`MAX`（最高质量，缺省值）、`MIN`（最低质量）、`MANUAL`（手动选择视频质量）
 
-- `--nomerge`表示是否自动合成下载下来的音视频文件，默认合成，但需要提前下载[ffmpeg](https://ffmpeg.org/download.html)工具（[windows版本](https://www.gyan.dev/ffmpeg/builds/)）并将其路径添加到`PATH`环境变量
+- `--nomerge`表示是否自动合成下载下来的音视频文件，默认合成，但需要提前下载[ffmpeg](https://ffmpeg.org/download.html)工具（如[windows版本](https://www.gyan.dev/ffmpeg/builds/)）并将其路径添加到`PATH`环境变量
+
+- `--force`表示强制重新下载视频，如果没有指定`--playlist`参数，则只是重新下载当前剧集，否则会直接删除`bili_tmp/`临时文件，重新下载全部剧集，但不会立即删除全部已下载音视频文件，而是覆盖更新
 
-- `--force`表示强制重新下载视频，携带该参数会直接删除`bili_tmp/`临时文件，但不会立即删除全部已下载音视频文件，而是覆盖更新
+- `--debug`用于在控制台输出全部debug日志信息，不指定该参数，也会将日志输出到`bili_tmp/download.log`中以备查阅
 
-- `--debug`用于在控制台输出全部debug日志信息，不指定该参数，也会将日志输出到`bili_tmp/log`中以备查阅
+- 默认随视频会下载封面图片
 
 - 默认随视频会下载弹幕XML文件，可以使用[danmu2ass](https://github.com/ikde/danmu2ass)做弹幕格式转换，双击Danmu2Ass.sln，用Visual Studio打开并编译，在项目Danmu2Ass目录下会生成bin文件夹，进入其中的Debug文件夹，可以看到一个Kaedei.Danmu2Ass.exe可执行文件，将视频和弹幕文件一块拖动到该可执行文件图标上去即可生成ASS字幕文件，再通过[potplayer](https://potplayer.daum.net/)打开视频即可自动加载字幕
 
 ## 致谢
 
 如果觉得本工具有用，请点个Star呗~，有bug或有改进意见请提issue，thx！
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.4 Summary: A simple tool
+Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.5 Summary: A simple tool
 to download videos from bilibili{*â§ââ¦} Home-page: https://github.com/
 muggledy/bili-get Author: muggledy Author-email: zgjsycfndy2015@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: requests # Bilibiliè§é¢ä¸è½½å¨ ![](https://
-img.shields.io/badge/python-3.6+-green) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/
-_r_e_l_e_a_s_e_/_m_u_g_g_l_e_d_y_/_b_i_l_i_-_g_e_t_] ## ä¸è½½ ### æ¹å¼ä¸ ```console pip install sole-
-bili-get -i https://www.pypi.org/simple/ ``` PSï¼æ´æ°çæ¬ï¼ï¼`pip
-install sole-bili-get -U` ### æ¹å¼äº ```console git clone https://
-github.com/muggledy/bili-get.git python setup.py sdist bdist_wheel pip install
-dist\sole_bili_get-0.0.1-py3-none-any.whl //demo bili-get --help ``` ## ä½¿ç¨
-```console C:\Users\muggledy\Downloads>bili-get https://www.bilibili.com/video/
-BV1CY4y1F7hP output: C:\Users\muggledy\Downloads (origin url):https://
-www.bilibili.com/video/BV1CY4y1F7hP (title):
+LICENSE.txt Requires-Dist: requests Requires-Dist: pycryptodome Requires-Dist:
+pypiwin32 # Bilibiliè§é¢ä¸è½½å¨ ![](https://img.shields.io/badge/python-
+3.6+-green) ![](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-
+pink) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_m_u_g_g_l_e_d_y_/_b_i_l_i_-_g_e_t_] ## ä¸è½½ ###
+æ¹å¼ä¸ ```console pip install sole-bili-get -i https://www.pypi.org/simple/
+``` PSï¼æ´æ°çæ¬ï¼ï¼`pip install sole-bili-get -U` ### æ¹å¼äº
+```console git clone https://github.com/muggledy/bili-get.git python setup.py
+sdist bdist_wheel pip install dist\sole_bili_get-0.0.1-py3-none-any.whl //demo
+bili-get --help ``` ## ä½¿ç¨ ```console C:\Users\muggledy\Downloads>bili-get
+https://www.bilibili.com/video/BV1CY4y1F7hP output: C:\Users\muggledy\Downloads
+(origin url):https://www.bilibili.com/video/BV1CY4y1F7hP (title):
 p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼
 (desc):æ­¤è§é¢éç»å¸æä¸æ°çå®æ­åå¨å¥¥çæåä»¬ï¼ (episodes
 num):7 (quality):æ¸æ° 480P(id:32), æµç 360P(id:16) selected download
 quality(MAX):32 get danmu urls success for 7 episodes p1 danmu xml file is
 downloaded into C:
 \Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼.xml
 start to download p1(video:æ¸æ° 480P,852x480,avc1.64001F_581618_29.412) from
@@ -32,15 +33,15 @@
 Note: this is a multi-episode video, you can download them all at once with --
 playlist ``` - é»è®¤æ¯ä¸è½½å°å½åå·¥ä½è·¯å¾ï¼å¯ä»¥éè¿`-o`æ`--
 output`æå®è¾åºç®å½ï¼ä¸å­å¨åèªå¨åå»ºï¼è­¬å¦`bili-get https://
 www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`ãè¿ä¼å¨`--
 output`ç®å½ä¸äº§çä¸¤ä¸ªæä»¶å¤¹ï¼`bili_tmp/`å`bili_output/
 `ï¼åèå­æ¾ä¸äºä¸´æ¶æä»¶ï¼ç¨äºè®°å½å¤å§éè§é¢çä¸è½½è¿åº¦ï¼å¦æä¸è½½è¿ç¨ä¸­åçä¸­æ­ï¼éæ°æ§è¡å½ä»¤å¯ä»¥ç»§ç»­ä¸è½½è¿ç¨ï¼ä¸å¯¹äºå°æªåæçå§éä¼å°è¯è¿è¡åæï¼é¤éæå®`-
 -
-nomerge`åæ°ï¼ï¼åèåæ¯è§é¢ãé³é¢ãå¼¹å¹æä»¶çè¾åºæä»¶å¤¹
+nomerge`åæ°ï¼ï¼åèåæ¯è§é¢ãé³é¢ãå°é¢ãå¼¹å¹æä»¶çè¾åºæä»¶å¤¹
 - å¯¹äºå¤å§éè§é¢ï¼å¯ä»¥æå®`--
 playlist`èªå¨ä¸è½½å¨é¨å§éï¼åªè¦ä¸å é¤å¯¹åºç`bili_tmp/
 `ä¸´æ¶æä»¶ï¼å¯ä»¥ä»»æéå¤æ§è¡ä¸è½½å½ä»¤ï¼å¦`bili-get https://
 www.bilibili.com/video/BV1CY4y1F7hP --
 playlist`ï¼ä¹ä¸ä¼éå¤ä¸è½½ï¼å¦æUPä¸»æ°åå¸äºå§éï¼åä¼ç»§ç»­ä¸è½½
 - `-c`æ`--
 cookie`ç¨äºæå®æ¨çBç«Cookieä¿¡æ¯ï¼è¿æ ·å°±å¯ä»¥ä¸è½½1080Pè§é¢äº
@@ -57,25 +58,33 @@
 from https://www.bilibili.com/video/BV1CY4y1F7hP/?p=1...
 100.00%|ââââââââââââââââââââ|
 ä¸è½½å®æãvideo/mp4ã 342.48MB/342.48MB start to download p1(audio)...
 100.00%|ââââââââââââââââââââ|
 ä¸è½½å®æãvideo/mp4ã 28.28MB/28.28MB ffmpeg merge success, save into C:
 \Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼.mp4
 Note: this is a multi-episode video, you can download them all at once with --
-playlist ``` Cookieè·åæ¹å¼å¦ä¸ï¼ ![](https://raw.githubusercontent.com/
-muggledy/bili-get/master/bilibili_cookie.jpg) - `-q`æ`--
+playlist ``` Cookieè·åæ¹å¼å¦ä¸ï¼ ![Bç«cookieè·åæ¹å¼](https://
+raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+æ³¨ï¼å¦ææ¯Windowså¹³å°ä½¿ç¨Chromeæµè§å¨ï¼å¯ä»¥æå®`-
+c`åæ°ä¸º`chrome`ï¼ç¨åºå°èªå¨ä»`./AppData/Local/Google/Chrome/User
+Data/default/Network/
+Cookies`è¯»åBç«çCookieä¿¡æ¯ï¼è­¬å¦æä»¬å¯ä»¥éè¿`bili-get https://
+www.bilibili.com/video/BV18G411D7FM -c chrome`å½ä»¤ä¸è½½1080pè§é¢ - `-
+q`æ`--
 quality`ç¨äºæå®è¦ä¸è½½çè§é¢è´¨éï¼æ¸æ°åº¦ï¼ï¼å¯éå¼æ`MAX`ï¼æé«è´¨éï¼ç¼ºçå¼ï¼ã`MIN`ï¼æä½è´¨éï¼ã`MANUAL`ï¼æå¨éæ©è§é¢è´¨éï¼
 - `--
 nomerge`è¡¨ç¤ºæ¯å¦èªå¨åæä¸è½½ä¸æ¥çé³è§é¢æä»¶ï¼é»è®¤åæï¼ä½éè¦æåä¸è½½
-[ffmpeg](https://ffmpeg.org/download.html)å·¥å·ï¼[windowsçæ¬](https://
+[ffmpeg](https://ffmpeg.org/download.html)å·¥å·ï¼å¦[windowsçæ¬](https://
 www.gyan.dev/ffmpeg/builds/)ï¼å¹¶å°å¶è·¯å¾æ·»å å°`PATH`ç¯å¢åé - `--
-force`è¡¨ç¤ºå¼ºå¶éæ°ä¸è½½è§é¢ï¼æºå¸¦è¯¥åæ°ä¼ç´æ¥å é¤`bili_tmp/
-`ä¸´æ¶æä»¶ï¼ä½ä¸ä¼ç«å³å é¤å¨é¨å·²ä¸è½½é³è§é¢æä»¶ï¼èæ¯è¦çæ´æ°
+force`è¡¨ç¤ºå¼ºå¶éæ°ä¸è½½è§é¢ï¼å¦ææ²¡ææå®`--
+playlist`åæ°ï¼ååªæ¯éæ°ä¸è½½å½åå§éï¼å¦åä¼ç´æ¥å é¤`bili_tmp/
+`ä¸´æ¶æä»¶ï¼éæ°ä¸è½½å¨é¨å§éï¼ä½ä¸ä¼ç«å³å é¤å¨é¨å·²ä¸è½½é³è§é¢æä»¶ï¼èæ¯è¦çæ´æ°
 - `--
 debug`ç¨äºå¨æ§å¶å°è¾åºå¨é¨debugæ¥å¿ä¿¡æ¯ï¼ä¸æå®è¯¥åæ°ï¼ä¹ä¼å°æ¥å¿è¾åºå°`bili_tmp/
-log`ä¸­ä»¥å¤æ¥é - é»è®¤éè§é¢ä¼ä¸è½½å¼¹å¹XMLæä»¶ï¼å¯ä»¥ä½¿ç¨
-[danmu2ass](https://github.com/ikde/
+download.log`ä¸­ä»¥å¤æ¥é - é»è®¤éè§é¢ä¼ä¸è½½å°é¢å¾ç -
+é»è®¤éè§é¢ä¼ä¸è½½å¼¹å¹XMLæä»¶ï¼å¯ä»¥ä½¿ç¨[danmu2ass](https://
+github.com/ikde/
 danmu2ass)åå¼¹å¹æ ¼å¼è½¬æ¢ï¼åå»Danmu2Ass.slnï¼ç¨Visual
 Studioæå¼å¹¶ç¼è¯ï¼å¨é¡¹ç®Danmu2Assç®å½ä¸ä¼çæbinæä»¶å¤¹ï¼è¿å¥å¶ä¸­çDebugæä»¶å¤¹ï¼å¯ä»¥çå°ä¸ä¸ªKaedei.Danmu2Ass.exeå¯æ§è¡æä»¶ï¼å°è§é¢åå¼¹å¹æä»¶ä¸åæå¨å°è¯¥å¯æ§è¡æä»¶å¾æ ä¸å»å³å¯çæASSå­å¹æä»¶ï¼åéè¿
 [potplayer](https://potplayer.daum.net/)æå¼è§é¢å³å¯èªå¨å è½½å­å¹ ##
 è´è°¢
 å¦æè§å¾æ¬å·¥å·æç¨ï¼è¯·ç¹ä¸ªStarå~ï¼æbugæææ¹è¿æè§è¯·æissueï¼thxï¼
```

### Comparing `sole_bili_get-0.0.4/README.md` & `sole_bili_get-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Bilibili视频下载器
 
-<a alt="null">![](https://img.shields.io/badge/python-3.6+-green)&nbsp;<a href="https://pypi.org/project/sole-bili-get/" alt="null"><img src="https://img.shields.io/github/v/release/muggledy/bili-get"/></a></a>
+<a alt="null">![](https://img.shields.io/badge/python-3.6+-green)&nbsp;![](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-pink)&nbsp;<a href="https://pypi.org/project/sole-bili-get/" alt="null"><img src="https://img.shields.io/github/v/release/muggledy/bili-get"/></a></a>
 
 ## 下载
 
 ### 方式一
 
 ```console
 pip install sole-bili-get -i https://www.pypi.org/simple/
@@ -38,15 +38,15 @@
 100.00%|████████████████████| 下载完成【application/octet-stream】 84.96MB/84.96MB
 start to download p1(audio)...
 100.00%|████████████████████| 下载完成【application/octet-stream】 28.28MB/28.28MB
 ffmpeg merge success, save into C:\Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_总耗时近一年！七爷带你一步到位看完昭和《奥特曼》系列全部345集怪兽及宇宙人们！_1初代奥特曼.mp4
 Note: this is a multi-episode video, you can download them all at once with --playlist
 ```
 
-- 默认是下载到当前工作路径，可以通过`-o`或`--output`指定输出目录，不存在则自动创建，譬如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`。这会在`--output`目录下产生两个文件夹：`bili_tmp/`和`bili_output/`，前者存放一些临时文件，用于记录多剧集视频的下载进度，如果下载过程中发生中断，重新执行命令可以继续下载过程（且对于尚未合成的剧集会尝试进行合成，除非指定`--nomerge`参数），后者则是视频、音频、弹幕文件的输出文件夹
+- 默认是下载到当前工作路径，可以通过`-o`或`--output`指定输出目录，不存在则自动创建，譬如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`。这会在`--output`目录下产生两个文件夹：`bili_tmp/`和`bili_output/`，前者存放一些临时文件，用于记录多剧集视频的下载进度，如果下载过程中发生中断，重新执行命令可以继续下载过程（且对于尚未合成的剧集会尝试进行合成，除非指定`--nomerge`参数），后者则是视频、音频、封面、弹幕文件的输出文件夹
 
 - 对于多剧集视频，可以指定`--playlist`自动下载全部剧集，只要不删除对应的`bili_tmp/`临时文件，可以任意重复执行下载命令，如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP --playlist`，也不会重复下载，如果UP主新发布了剧集，则会继续下载
 
 - `-c`或`--cookie`用于指定您的B站Cookie信息，这样就可以下载1080P视频了
 
   ```console
   C:\Users\muggledy\Downloads>bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -c "your cookie"
@@ -65,22 +65,26 @@
   100.00%|████████████████████| 下载完成【video/mp4】 28.28MB/28.28MB
   ffmpeg merge success, save into C:\Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_总耗时近一年！七爷带你一步到位看完昭和《奥特曼》系列全部345集怪兽及宇宙人们！_1初代奥特曼.mp4
   Note: this is a multi-episode video, you can download them all at once with --playlist
   ```
 
   Cookie获取方式如下：
 
-  ![](https://raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+  ![B站cookie获取方式](https://raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+
+  注：如果是Windows平台使用Chrome浏览器，可以指定`-c`参数为`chrome`，程序将自动从`./AppData/Local/Google/Chrome/User Data/default/Network/Cookies`读取B站的Cookie信息，譬如我们可以通过`bili-get https://www.bilibili.com/video/BV18G411D7FM -c chrome`命令下载1080p视频
 
 - `-q`或`--quality`用于指定要下载的视频质量（清晰度），可选值有`MAX`（最高质量，缺省值）、`MIN`（最低质量）、`MANUAL`（手动选择视频质量）
 
-- `--nomerge`表示是否自动合成下载下来的音视频文件，默认合成，但需要提前下载[ffmpeg](https://ffmpeg.org/download.html)工具（[windows版本](https://www.gyan.dev/ffmpeg/builds/)）并将其路径添加到`PATH`环境变量
+- `--nomerge`表示是否自动合成下载下来的音视频文件，默认合成，但需要提前下载[ffmpeg](https://ffmpeg.org/download.html)工具（如[windows版本](https://www.gyan.dev/ffmpeg/builds/)）并将其路径添加到`PATH`环境变量
+
+- `--force`表示强制重新下载视频，如果没有指定`--playlist`参数，则只是重新下载当前剧集，否则会直接删除`bili_tmp/`临时文件，重新下载全部剧集，但不会立即删除全部已下载音视频文件，而是覆盖更新
 
-- `--force`表示强制重新下载视频，携带该参数会直接删除`bili_tmp/`临时文件，但不会立即删除全部已下载音视频文件，而是覆盖更新
+- `--debug`用于在控制台输出全部debug日志信息，不指定该参数，也会将日志输出到`bili_tmp/download.log`中以备查阅
 
-- `--debug`用于在控制台输出全部debug日志信息，不指定该参数，也会将日志输出到`bili_tmp/log`中以备查阅
+- 默认随视频会下载封面图片
 
 - 默认随视频会下载弹幕XML文件，可以使用[danmu2ass](https://github.com/ikde/danmu2ass)做弹幕格式转换，双击Danmu2Ass.sln，用Visual Studio打开并编译，在项目Danmu2Ass目录下会生成bin文件夹，进入其中的Debug文件夹，可以看到一个Kaedei.Danmu2Ass.exe可执行文件，将视频和弹幕文件一块拖动到该可执行文件图标上去即可生成ASS字幕文件，再通过[potplayer](https://potplayer.daum.net/)打开视频即可自动加载字幕
 
 ## 致谢
 
 如果觉得本工具有用，请点个Star呗~，有bug或有改进意见请提issue，thx！
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-# Bilibiliè§é¢ä¸è½½å¨ ![](https://img.shields.io/badge/python-3.6+-green) 
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_m_u_g_g_l_e_d_y_/_b_i_l_i_-_g_e_t_] ## ä¸è½½ ###
-æ¹å¼ä¸ ```console pip install sole-bili-get -i https://www.pypi.org/simple/
-``` PSï¼æ´æ°çæ¬ï¼ï¼`pip install sole-bili-get -U` ### æ¹å¼äº
-```console git clone https://github.com/muggledy/bili-get.git python setup.py
-sdist bdist_wheel pip install dist\sole_bili_get-0.0.1-py3-none-any.whl //demo
-bili-get --help ``` ## ä½¿ç¨ ```console C:\Users\muggledy\Downloads>bili-get
-https://www.bilibili.com/video/BV1CY4y1F7hP output: C:\Users\muggledy\Downloads
+# Bilibiliè§é¢ä¸è½½å¨ ![](https://img.shields.io/badge/python-3.6+-green) !
+[](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-pink) _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_m_u_g_g_l_e_d_y_/_b_i_l_i_-_g_e_t_] ## ä¸è½½ ### æ¹å¼ä¸
+```console pip install sole-bili-get -i https://www.pypi.org/simple/ ```
+PSï¼æ´æ°çæ¬ï¼ï¼`pip install sole-bili-get -U` ### æ¹å¼äº ```console
+git clone https://github.com/muggledy/bili-get.git python setup.py sdist
+bdist_wheel pip install dist\sole_bili_get-0.0.1-py3-none-any.whl //demo bili-
+get --help ``` ## ä½¿ç¨ ```console C:\Users\muggledy\Downloads>bili-get https:
+//www.bilibili.com/video/BV1CY4y1F7hP output: C:\Users\muggledy\Downloads
 (origin url):https://www.bilibili.com/video/BV1CY4y1F7hP (title):
 p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼
 (desc):æ­¤è§é¢éç»å¸æä¸æ°çå®æ­åå¨å¥¥çæåä»¬ï¼ (episodes
 num):7 (quality):æ¸æ° 480P(id:32), æµç 360P(id:16) selected download
 quality(MAX):32 get danmu urls success for 7 episodes p1 danmu xml file is
 downloaded into C:
 \Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼.xml
@@ -25,15 +26,15 @@
 Note: this is a multi-episode video, you can download them all at once with --
 playlist ``` - é»è®¤æ¯ä¸è½½å°å½åå·¥ä½è·¯å¾ï¼å¯ä»¥éè¿`-o`æ`--
 output`æå®è¾åºç®å½ï¼ä¸å­å¨åèªå¨åå»ºï¼è­¬å¦`bili-get https://
 www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`ãè¿ä¼å¨`--
 output`ç®å½ä¸äº§çä¸¤ä¸ªæä»¶å¤¹ï¼`bili_tmp/`å`bili_output/
 `ï¼åèå­æ¾ä¸äºä¸´æ¶æä»¶ï¼ç¨äºè®°å½å¤å§éè§é¢çä¸è½½è¿åº¦ï¼å¦æä¸è½½è¿ç¨ä¸­åçä¸­æ­ï¼éæ°æ§è¡å½ä»¤å¯ä»¥ç»§ç»­ä¸è½½è¿ç¨ï¼ä¸å¯¹äºå°æªåæçå§éä¼å°è¯è¿è¡åæï¼é¤éæå®`-
 -
-nomerge`åæ°ï¼ï¼åèåæ¯è§é¢ãé³é¢ãå¼¹å¹æä»¶çè¾åºæä»¶å¤¹
+nomerge`åæ°ï¼ï¼åèåæ¯è§é¢ãé³é¢ãå°é¢ãå¼¹å¹æä»¶çè¾åºæä»¶å¤¹
 - å¯¹äºå¤å§éè§é¢ï¼å¯ä»¥æå®`--
 playlist`èªå¨ä¸è½½å¨é¨å§éï¼åªè¦ä¸å é¤å¯¹åºç`bili_tmp/
 `ä¸´æ¶æä»¶ï¼å¯ä»¥ä»»æéå¤æ§è¡ä¸è½½å½ä»¤ï¼å¦`bili-get https://
 www.bilibili.com/video/BV1CY4y1F7hP --
 playlist`ï¼ä¹ä¸ä¼éå¤ä¸è½½ï¼å¦æUPä¸»æ°åå¸äºå§éï¼åä¼ç»§ç»­ä¸è½½
 - `-c`æ`--
 cookie`ç¨äºæå®æ¨çBç«Cookieä¿¡æ¯ï¼è¿æ ·å°±å¯ä»¥ä¸è½½1080Pè§é¢äº
@@ -50,25 +51,33 @@
 from https://www.bilibili.com/video/BV1CY4y1F7hP/?p=1...
 100.00%|ââââââââââââââââââââ|
 ä¸è½½å®æãvideo/mp4ã 342.48MB/342.48MB start to download p1(audio)...
 100.00%|ââââââââââââââââââââ|
 ä¸è½½å®æãvideo/mp4ã 28.28MB/28.28MB ffmpeg merge success, save into C:
 \Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼.mp4
 Note: this is a multi-episode video, you can download them all at once with --
-playlist ``` Cookieè·åæ¹å¼å¦ä¸ï¼ ![](https://raw.githubusercontent.com/
-muggledy/bili-get/master/bilibili_cookie.jpg) - `-q`æ`--
+playlist ``` Cookieè·åæ¹å¼å¦ä¸ï¼ ![Bç«cookieè·åæ¹å¼](https://
+raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+æ³¨ï¼å¦ææ¯Windowså¹³å°ä½¿ç¨Chromeæµè§å¨ï¼å¯ä»¥æå®`-
+c`åæ°ä¸º`chrome`ï¼ç¨åºå°èªå¨ä»`./AppData/Local/Google/Chrome/User
+Data/default/Network/
+Cookies`è¯»åBç«çCookieä¿¡æ¯ï¼è­¬å¦æä»¬å¯ä»¥éè¿`bili-get https://
+www.bilibili.com/video/BV18G411D7FM -c chrome`å½ä»¤ä¸è½½1080pè§é¢ - `-
+q`æ`--
 quality`ç¨äºæå®è¦ä¸è½½çè§é¢è´¨éï¼æ¸æ°åº¦ï¼ï¼å¯éå¼æ`MAX`ï¼æé«è´¨éï¼ç¼ºçå¼ï¼ã`MIN`ï¼æä½è´¨éï¼ã`MANUAL`ï¼æå¨éæ©è§é¢è´¨éï¼
 - `--
 nomerge`è¡¨ç¤ºæ¯å¦èªå¨åæä¸è½½ä¸æ¥çé³è§é¢æä»¶ï¼é»è®¤åæï¼ä½éè¦æåä¸è½½
-[ffmpeg](https://ffmpeg.org/download.html)å·¥å·ï¼[windowsçæ¬](https://
+[ffmpeg](https://ffmpeg.org/download.html)å·¥å·ï¼å¦[windowsçæ¬](https://
 www.gyan.dev/ffmpeg/builds/)ï¼å¹¶å°å¶è·¯å¾æ·»å å°`PATH`ç¯å¢åé - `--
-force`è¡¨ç¤ºå¼ºå¶éæ°ä¸è½½è§é¢ï¼æºå¸¦è¯¥åæ°ä¼ç´æ¥å é¤`bili_tmp/
-`ä¸´æ¶æä»¶ï¼ä½ä¸ä¼ç«å³å é¤å¨é¨å·²ä¸è½½é³è§é¢æä»¶ï¼èæ¯è¦çæ´æ°
+force`è¡¨ç¤ºå¼ºå¶éæ°ä¸è½½è§é¢ï¼å¦ææ²¡ææå®`--
+playlist`åæ°ï¼ååªæ¯éæ°ä¸è½½å½åå§éï¼å¦åä¼ç´æ¥å é¤`bili_tmp/
+`ä¸´æ¶æä»¶ï¼éæ°ä¸è½½å¨é¨å§éï¼ä½ä¸ä¼ç«å³å é¤å¨é¨å·²ä¸è½½é³è§é¢æä»¶ï¼èæ¯è¦çæ´æ°
 - `--
 debug`ç¨äºå¨æ§å¶å°è¾åºå¨é¨debugæ¥å¿ä¿¡æ¯ï¼ä¸æå®è¯¥åæ°ï¼ä¹ä¼å°æ¥å¿è¾åºå°`bili_tmp/
-log`ä¸­ä»¥å¤æ¥é - é»è®¤éè§é¢ä¼ä¸è½½å¼¹å¹XMLæä»¶ï¼å¯ä»¥ä½¿ç¨
-[danmu2ass](https://github.com/ikde/
+download.log`ä¸­ä»¥å¤æ¥é - é»è®¤éè§é¢ä¼ä¸è½½å°é¢å¾ç -
+é»è®¤éè§é¢ä¼ä¸è½½å¼¹å¹XMLæä»¶ï¼å¯ä»¥ä½¿ç¨[danmu2ass](https://
+github.com/ikde/
 danmu2ass)åå¼¹å¹æ ¼å¼è½¬æ¢ï¼åå»Danmu2Ass.slnï¼ç¨Visual
 Studioæå¼å¹¶ç¼è¯ï¼å¨é¡¹ç®Danmu2Assç®å½ä¸ä¼çæbinæä»¶å¤¹ï¼è¿å¥å¶ä¸­çDebugæä»¶å¤¹ï¼å¯ä»¥çå°ä¸ä¸ªKaedei.Danmu2Ass.exeå¯æ§è¡æä»¶ï¼å°è§é¢åå¼¹å¹æä»¶ä¸åæå¨å°è¯¥å¯æ§è¡æä»¶å¾æ ä¸å»å³å¯çæASSå­å¹æä»¶ï¼åéè¿
 [potplayer](https://potplayer.daum.net/)æå¼è§é¢å³å¯èªå¨å è½½å­å¹ ##
 è´è°¢
 å¦æè§å¾æ¬å·¥å·æç¨ï¼è¯·ç¹ä¸ªStarå~ï¼æbugæææ¹è¿æè§è¯·æissueï¼thxï¼
```

### Comparing `sole_bili_get-0.0.4/sole_bili_get/bili_get.py` & `sole_bili_get-0.0.5/sole_bili_get/bili_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
     subprocess, platform, sys, \
     time, argparse
 from logging.handlers import RotatingFileHandler
 #from lxml import etree
 from pathlib import Path
 from copy import deepcopy
 from . import utils
+if platform.system() == 'Windows':
+    from .chrome_cookie import get_bilibili_cookie
 
 __all__ = ['Bilibili', 'main']
 
 class Bilibili:
     def __init__(self, origin_url, **kwargs):
         if kwargs.get('base_dir') and os.path.isdir(kwargs['base_dir']):
             utils._base_dir = kwargs['base_dir']
@@ -39,24 +41,31 @@
         if self.auto_merge:
             if not self.check_tool('ffmpeg'):
                 self.__ffmpeg_exist = False
                 ffmpeg_not_exist_prompt = \
                     'ffmpeg not exists, can\'t merge video and audio, you can prepare this tool and re-exec the download cmd'
             else:
                 self.__ffmpeg_exist = True
-        if self.force_re_download:
+        if self.force_re_download and self.fetch_playlists: #只有在指定fetch_playlists的情况下，指定force_re_download才会整个删除临时文件，全部强制重新下载，否则只是强制重新下载对应一集
+            self.__force_re_download_p = float('inf')
             if os.path.exists(self.__local_playlists_info_path):
                 self.logger.warning(f'delete old file {self.__local_playlists_info_path} for force_re_download')
                 os.remove(self.__local_playlists_info_path)
             __local_playlists_info = {}
             self.__local_already_download_p_list = []
         else:
             #首先从本地获取视频信息并填充到self.playlists_info，如果视频（含子剧集）未全部下载完成，则
             #针对未下载剧集需要重新从B站服务器获取相应的剧集信息并更新本地数据
             __local_playlists_info = self.get_playlists_info_from_local()
+            if self.force_re_download:
+                __local_playlists_info = self.clear_download_info_for_origin_url(playlists_info=__local_playlists_info)
+                if __local_playlists_info:
+                    self.save_playlists_info_into_local(__local_playlists_info)
+            else:
+                self.__force_re_download_p = 0
             self.__local_already_download_p_list = \
                 [v['p_num'] for k,v in __local_playlists_info.items() if v['download_flag'] == 3]
             if self.__local_already_download_p_list and self.__ffmpeg_exist:
                 not_merged_p_list = [i for i in self.__local_already_download_p_list if not __local_playlists_info[i]['merge_flag']]
                 if not_merged_p_list:
                     self.logger.info('first, merge previously downloaded videos/audios...')
                     if self.disable_console_log:
@@ -72,18 +81,23 @@
             self.__all_downloed_flag = True #先预设能够全部下载成功，如果有一个失败了，则再置为False
             self.download_by_playlists_info()
         total, downloaded, not_download, download_failed, merged, not_merge, merge_failed = self.get_current_downloaded_info()
         self.logger.info(f"total:{total}, downloaded:{downloaded}, not_download:{not_download}, download_failed:{download_failed}, "
                          f"merged:{merged}, not_merge:{not_merge}, merge_failed:{merge_failed}")
         if self.__all_downloed_flag:
             if total == downloaded:
-                self.logger.info(f'(all) videos has already been downloaded in {self.__output_dir}!')
+                all_download_ok_prompt = f'{"(all)videos have" if total>1 else "This video has"} already been downloaded in {self.__output_dir}!'
+                self.logger.info(all_download_ok_prompt)
+                if self.disable_console_log:
+                    print(all_download_ok_prompt)
         else:
             self.save_playlists_info_into_local()
             self.logger.info('some videos/audios download failed, you can re-exec command to download them')
+            if self.disable_console_log:
+                print('some videos/audios download failed, you can re-exec command to download them')
         if self.auto_merge:
             if not self.__ffmpeg_exist and downloaded != 0:
                 self.logger.warning(ffmpeg_not_exist_prompt)
                 if self.disable_console_log:
                     print(f'Note: {ffmpeg_not_exist_prompt}')
             else:
                 self.check_playlists_is_merged()
@@ -94,14 +108,16 @@
                 continue
             playlists_info[i]['download_flag'] = self.playlists_info[i]['download_flag']
             playlists_info[i]['merge_flag'] = self.playlists_info[i]['merge_flag']
             if self.playlists_info[i].get('video_save_path'):
                 playlists_info[i]['video_save_path'] = self.playlists_info[i]['video_save_path']
             if self.playlists_info[i].get('audio_save_path'):
                 playlists_info[i]['audio_save_path'] = self.playlists_info[i]['audio_save_path']
+            if self.playlists_info[i].get('danmu_url'):
+                playlists_info[i]['danmu_url'] = self.playlists_info[i]['danmu_url']
         self.playlists_info.update(playlists_info)
 
     def get_current_downloaded_info(self): #返回：(剧集总数,已下载,未下载,下载失败,已合入,未合入,合入失败)
         if not self.playlists_info:
             return (0,0,0,0,0,0,0)
         current_info = sorted([(p_num, info['download_flag'], info['merge_flag']) for p_num, info in self.playlists_info.items()], key=lambda x:x[0])
         total = self.playlists_info[current_info[0][0]]['videos']
@@ -122,15 +138,15 @@
 
     @origin_url.setter
     def origin_url(self, origin_url):
         if hasattr(self, f'_{self.__class__.__name__}__origin_url') \
                 and (origin_url == self.__origin_url):
             return
         self.__origin_url = origin_url
-        bvid = re.findall(r'video/([^/?]+)', self.__origin_url)
+        bvid = re.findall(r'video/([^/\?]+)', self.__origin_url)
         if bvid: #key id
             self.__bvid, self.__local_playlists_info_path = \
                 bvid[0], get_absolute_path(f'./bili_tmp/local_playlists_info_{bvid[0]}.pickle')
             self.__output_dir = get_absolute_path(f'./bili_output/{self.__bvid}/')
         else:
             self.__bvid, self.__local_playlists_info_path = None, None
             self.__output_dir = None
@@ -163,14 +179,15 @@
                     new_add_info_num += 1
                 if self.debug_all:
                     self.logger.info(f'html analyse succeed: {str(origin_video_info)}')
                 quality_dict = {_1:_2['quality'] for _1, _2 in origin_video_info['video_info'].items()}
                 _desc = re.sub('\n',' ',origin_video_info['desc'])
                 video_main_info = f"{'(title):':>15}"\
                     f"{origin_video_info['title']}\n{'(desc):':>15}{_desc}\n"\
+                    f"{'(author):':>15}{origin_video_info['author']['name']}\n"\
                     f"{'(episodes num):':>15}{origin_video_info['videos']}"\
                     f"\n{'(quality):':>15}{', '.join([_[1]+'(id:'+str(_[0])+')' for _ in quality_dict.items()])}"
                 self.logger.info(f"origin html({origin_video_info['url']}) analyse succeed\n{video_main_info}")
                 if self.disable_console_log:
                     print(f"{'(origin url):':>15}{self.origin_url}\n{video_main_info}")
                 if not ((origin_video_info['videos'] == len(self.__local_already_download_p_list)) and 
                         list(sorted(self.__local_already_download_p_list)) == list(range(1, origin_video_info['videos']+1))):
@@ -185,15 +202,15 @@
                     else: #default is MAX quality
                         self.__quality_id = max(quality_dict.keys())
                     select_down_quality_info = f'selected download quality({self.quality}):{self.__quality_id}'
                     self.logger.info(select_down_quality_info)
                     if self.disable_console_log:
                         print(select_down_quality_info)
                         if self.__local_already_download_p_list:
-                            print(f"Note: {', '.join(['p'+str(_) for _ in self.__local_already_download_p_list])} has already been downloaded in {self.__output_dir}")
+                            print(f"Note: {', '.join(['p'+str(_) for _ in sorted(self.__local_already_download_p_list)])} has already been downloaded in {self.__output_dir}")
                     if not ((not self.fetch_playlists) and (origin_video_info['p_num'] in self.__local_already_download_p_list)):
                         self.get_danmu_urls()
                 else:
                     self.logger.info(f'(all) videos has already been downloaded in {self.__output_dir}! '
                                      f'if you want to re-download, please delete {self.__local_playlists_info_path} or pass force_re_download param')
                     self.__all_downloed_flag = True
                     return self.playlists_info
@@ -315,36 +332,42 @@
                 continue
             info = self.playlists_info[p]
             available_qualities = list(info['video_info'].keys())
             best_quality_idx = sorted([(i,abs(q-self.__quality_id)) 
                                        for i,q in enumerate(available_qualities)], key=lambda x:x[1])[0][0]
             best_quality = available_qualities[best_quality_idx]
             get_video_url_already_succeed = 0
-            if self.danmu_urls.get(p):
+            if self.danmu_urls.get(p): #弹幕文件只是附带下载，不保证下载成功
                 if self.download_danmu_xml(self.danmu_urls[p], save_path=os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}.xml"))):
                     danmu_ok_prompt = f"p{p} danmu xml file is downloaded into "+os.path.normpath(os.path.join(os.path.join(self.__output_dir, f"{info['title']}.xml")))
                     self.logger.info(danmu_ok_prompt+f" from {self.danmu_urls[p]}")
                     if self.disable_console_log: print(danmu_ok_prompt)
                     self.playlists_info[p]['danmu_url'] = self.danmu_urls[p]
+            self.__crawler.url = self.playlists_info[p]['cover']
+            self.__crawler.save_path = os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}"))
+            if self.__crawler.get(): #视频封面只是附带下载，不保证下载成功
+                self.logger.info(f'p{p} cover is downloaded into {self.__crawler.save_path}')
+                if self.disable_console_log:
+                    print(f'p{p} cover is downloaded into {self.__crawler.save_path}')
             if self.playlists_info[p]['download_flag'] != 1:
                 for url,codec_info in sorted(info['video_info'][best_quality]['urls'], 
                                              key=lambda x:get_idx_of_specific_codedc(x[1])):
                     #if not [_c for _c in download_specific_codec_video if codec_info.lower().startswith(_c.lower())]:
                     #    continue
                     downloading_video_info = f"start to download p{p}(video:{info['video_info'][best_quality]['quality']},"\
                         f"{'x'.join([str(_) for _ in info['video_info'][best_quality]['size']])},{codec_info})"\
                         f"{' from '+info['url'] if self.disable_console_log else ''}..."
                     self.logger.info(downloading_video_info)
                     if self.disable_console_log:
                         print(downloading_video_info)
                     self.__crawler.url = url
                     self.__crawler.save_path = os.path.normpath(os.path.join(self.__output_dir, 
                         f"{info['title']}{'' if (0 == get_video_url_already_succeed) else '_'+str(get_video_url_already_succeed)}.mp4"))
-                    if self.force_re_download and os.path.exists(self.__crawler.save_path):
-                        self.logger.warning(f'delete old p{p} video file {self.__crawler.save_path} for force_re_download')
+                    if ((self.__force_re_download_p == float('inf')) or (self.__force_re_download_p == p)) and os.path.exists(self.__crawler.save_path):
+                        self.logger.warning(f'delete old p{p} video file {self.__crawler.save_path} and re-download it')
                         os.remove(self.__crawler.save_path)
                     start_time = time.time()
                     ok = self.__crawler.get()
                     if ok:
                         get_video_url_already_succeed += 1
                         if get_video_url_already_succeed == 1:
                             self.playlists_info[p]['video_save_path'] = self.__crawler.save_path
@@ -363,16 +386,16 @@
                 continue
             self.logger.info(f"start to download p{p}(audio)...")
             if self.disable_console_log:
                 print(f"start to download p{p}(audio)...")
             self.__crawler.url = info['audio_url']
             self.__crawler.save_path = os.path.normpath(os.path.join(self.__output_dir, f"{info['title']}_audio.mp3")) #audio may also be *.mp4 file 
                                                         #which is the same with video filename in this case, we rename it to *.mp3
-            if self.force_re_download and os.path.exists(self.__crawler.save_path):
-                self.logger.warning(f'delete old p{p} audio file {self.__crawler.save_path} for force_re_download')
+            if ((self.__force_re_download_p == float('inf')) or (self.__force_re_download_p == p)) and os.path.exists(self.__crawler.save_path):
+                self.logger.warning(f'delete old p{p} audio file {self.__crawler.save_path} and re-download it')
                 os.remove(self.__crawler.save_path)
             start_time = time.time()
             ok = self.__crawler.get()
             if ok:
                 self.logger.info(f"download audio from {self.__crawler.url} into {self.__crawler.save_path} succeed, runtime: {time.time()-start_time:.2f}s")
                 if os.path.exists(self.__crawler.save_path):
                     if self.playlists_info[p].get('video_save_path') and \
@@ -478,17 +501,17 @@
     @staticmethod
     def generate_bilibili_video_url(bvid, p=None):
         if p is None:
             return f'https://www.bilibili.com/video/{bvid}'
         else:
             return f'https://www.bilibili.com/video/{bvid}/?p={p}'
 
-    def save_playlists_info_into_local(self):
+    def save_playlists_info_into_local(self, playlists_info=None):
         with open(self.__local_playlists_info_path, 'wb') as f:
-            pickle.dump(self.playlists_info, f, pickle.HIGHEST_PROTOCOL)
+            pickle.dump(self.playlists_info if playlists_info is None else playlists_info, f, pickle.HIGHEST_PROTOCOL)
         self.logger.info(f'write playlists info into {self.__local_playlists_info_path}')
 
     def get_playlists_info_from_local(self):
         if not os.path.exists(self.__local_playlists_info_path):
             self.logger.info(f'{self.__local_playlists_info_path} not exists')
             return {}
         with open(self.__local_playlists_info_path, 'rb') as f:
@@ -535,14 +558,34 @@
 
     @staticmethod
     def normalize_filename(filename): #Windows文件名不能含有\/:*?"<>|
         illegal_chars = r'\/:*?"<>|'
         filename = ''.join(char for char in filename if char not in illegal_chars)
         return filename
 
+    def clear_download_info_for_origin_url(self, playlists_info=None):
+        p = re.findall(r'video/[^/\?]+/\?p=(\d+)', self.origin_url)
+        p = int(p[0]) if p else 1
+        self.__force_re_download_p = p
+        if (not self.playlists_info) and (playlists_info is None):
+            return None
+        flag = True if playlists_info is None else False
+        playlists_info = self.playlists_info if playlists_info is None else playlists_info
+        if p in playlists_info.keys():
+            playlists_info[p]['download_flag'] = 0
+            playlists_info[p]['merge_flag'] = False
+            playlists_info[p]['video_save_path'] = ''
+            playlists_info[p]['audio_save_path'] = ''
+            playlists_info[p]['danmu_url'] = ''
+            self.logger.info(f'delete p{p} download info of original url {self.origin_url} for force_re_download')
+        if flag:
+            self.playlists_info = playlists_info
+            return self.playlists_info
+        return playlists_info
+
     @property
     def disable_console_log(self):
         return self.__disable_console_log
 
     @disable_console_log.setter
     def disable_console_log(self, disable_console_log):
         set_flag = hasattr(self, f'_{self.__class__.__name__}__disable_console_log')
@@ -568,15 +611,15 @@
         self.logger.setLevel(logging.DEBUG) #logger.setLevel()对低于该等级的日志丢弃，否则再转发给FileHandler和StreamHandler处理，因此该等级必须最低
         Bilibili.logger_console_handler = logging.StreamHandler()
         self.logger_console_handler.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s(%(funcName)s:%(lineno)s): %(message)s'))
         if not (hasattr(self, f'_{self.__class__.__name__}__disable_console_log') and self.disable_console_log):
             if not self.logger_concole_handler_add_once:
                 Bilibili.logger_concole_handler_add_once = True
                 self.logger.addHandler(self.logger_console_handler)
-        file_log_handler = RotatingFileHandler(filename=get_absolute_path(f'./bili_tmp/log'), 
+        file_log_handler = RotatingFileHandler(filename=get_absolute_path(f'./bili_tmp/download.log'), 
                                                maxBytes=1024*1024, backupCount=3, encoding='utf-8') #logging.FileHandler(filename='log', encoding='utf-8')
         file_log_handler.setFormatter(logging.Formatter('%(asctime)s[%(name)s] - %(pathname)s[line:%(lineno)d(%(funcName)s)] - %(levelname)s: %(message)s'))
         file_log_handler.setLevel(logging.INFO)
         self.logger.addHandler(file_log_handler)
 
     @staticmethod
     def check_tool(tool_name):
@@ -605,15 +648,24 @@
     output = args.output
     if (output=='') or os.path.isfile(output):
         output = Path.cwd()
     else:
         output = os.path.normpath(output)
         if not os.path.isdir(output):
             os.makedirs(output)
+    utils._base_dir = output #for chrome_cookie.py
+    if args.debug:
+        utils._utils_debug = True #for chrome_cookie.py
     if args.cookie:
+        if (platform.system() == 'Windows') and (args.cookie.lower().strip() == 'chrome'):
+            bili_ck = get_bilibili_cookie()
+            if bili_ck is not None:
+                args.cookie = bili_ck
+            else:
+                print('(ignore)get bilibili cookie from local for chrome failed')
         cookies = parse_cookies(args.cookie)
     else:
         cookies = None
     if args.debug:
         print(f"input params: url({url}), quality({args.quality}), cookie({str(cookies)}), "
               f"output({output}), download_playlist({args.playlist}), force_download({args.force}), not_merge({args.nomerge})")
     else:
```

### Comparing `sole_bili_get-0.0.4/sole_bili_get/utils.py` & `sole_bili_get-0.0.5/sole_bili_get/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,16 @@
                 suffix = minetype2suffix.get(response.headers['Content-Type'], '.unknown')
                 if self.save_path is None:
                     self.save_path = self.gen_default_save_path(suffix)
                     if _utils_debug: print(f'generate default save_path: {self.save_path}')
                 elif (suffix != '.unknown') and (not self.save_path.endswith(suffix)):
                     old_path = self.save_path
                     split_save_path = os.path.splitext(self.save_path)
+                    if (split_save_path[-1] != '') and re.findall(r'[\u4e00-\u9fa5]+', split_save_path[-1]): #避免“哈哈.图片”这种中文名称中含“.”的被错误切割为('哈哈', '.图片')
+                        split_save_path = (self.save_path, '')
                     if split_save_path[-1] != '':
                         self.save_path = split_save_path[0] + '.' + suffix
                     else:
                         self.save_path += f'.{suffix}'
                     self.save_path = os.path.normpath(self.save_path)
                     if _utils_debug: print(f'change save_path from {old_path} to {self.save_path}')
                 total_size = float(response.headers['content-length']) + start_byte
```

### Comparing `sole_bili_get-0.0.4/sole_bili_get.egg-info/PKG-INFO` & `sole_bili_get-0.0.5/sole_bili_get.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: sole_bili_get
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple tool to download videos from bilibili{*≧∀≦}
 Home-page: https://github.com/muggledy/bili-get
 Author: muggledy
 Author-email: zgjsycfndy2015@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
+Requires-Dist: pycryptodome
+Requires-Dist: pypiwin32
 
 # Bilibili视频下载器
 
-<a alt="null">![](https://img.shields.io/badge/python-3.6+-green)&nbsp;<a href="https://pypi.org/project/sole-bili-get/" alt="null"><img src="https://img.shields.io/github/v/release/muggledy/bili-get"/></a></a>
+<a alt="null">![](https://img.shields.io/badge/python-3.6+-green)&nbsp;![](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-pink)&nbsp;<a href="https://pypi.org/project/sole-bili-get/" alt="null"><img src="https://img.shields.io/github/v/release/muggledy/bili-get"/></a></a>
 
 ## 下载
 
 ### 方式一
 
 ```console
 pip install sole-bili-get -i https://www.pypi.org/simple/
@@ -54,15 +56,15 @@
 100.00%|████████████████████| 下载完成【application/octet-stream】 84.96MB/84.96MB
 start to download p1(audio)...
 100.00%|████████████████████| 下载完成【application/octet-stream】 28.28MB/28.28MB
 ffmpeg merge success, save into C:\Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_总耗时近一年！七爷带你一步到位看完昭和《奥特曼》系列全部345集怪兽及宇宙人们！_1初代奥特曼.mp4
 Note: this is a multi-episode video, you can download them all at once with --playlist
 ```
 
-- 默认是下载到当前工作路径，可以通过`-o`或`--output`指定输出目录，不存在则自动创建，譬如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`。这会在`--output`目录下产生两个文件夹：`bili_tmp/`和`bili_output/`，前者存放一些临时文件，用于记录多剧集视频的下载进度，如果下载过程中发生中断，重新执行命令可以继续下载过程（且对于尚未合成的剧集会尝试进行合成，除非指定`--nomerge`参数），后者则是视频、音频、弹幕文件的输出文件夹
+- 默认是下载到当前工作路径，可以通过`-o`或`--output`指定输出目录，不存在则自动创建，譬如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`。这会在`--output`目录下产生两个文件夹：`bili_tmp/`和`bili_output/`，前者存放一些临时文件，用于记录多剧集视频的下载进度，如果下载过程中发生中断，重新执行命令可以继续下载过程（且对于尚未合成的剧集会尝试进行合成，除非指定`--nomerge`参数），后者则是视频、音频、封面、弹幕文件的输出文件夹
 
 - 对于多剧集视频，可以指定`--playlist`自动下载全部剧集，只要不删除对应的`bili_tmp/`临时文件，可以任意重复执行下载命令，如`bili-get https://www.bilibili.com/video/BV1CY4y1F7hP --playlist`，也不会重复下载，如果UP主新发布了剧集，则会继续下载
 
 - `-c`或`--cookie`用于指定您的B站Cookie信息，这样就可以下载1080P视频了
 
   ```console
   C:\Users\muggledy\Downloads>bili-get https://www.bilibili.com/video/BV1CY4y1F7hP -c "your cookie"
@@ -81,22 +83,26 @@
   100.00%|████████████████████| 下载完成【video/mp4】 28.28MB/28.28MB
   ffmpeg merge success, save into C:\Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_总耗时近一年！七爷带你一步到位看完昭和《奥特曼》系列全部345集怪兽及宇宙人们！_1初代奥特曼.mp4
   Note: this is a multi-episode video, you can download them all at once with --playlist
   ```
 
   Cookie获取方式如下：
 
-  ![](https://raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+  ![B站cookie获取方式](https://raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+
+  注：如果是Windows平台使用Chrome浏览器，可以指定`-c`参数为`chrome`，程序将自动从`./AppData/Local/Google/Chrome/User Data/default/Network/Cookies`读取B站的Cookie信息，譬如我们可以通过`bili-get https://www.bilibili.com/video/BV18G411D7FM -c chrome`命令下载1080p视频
 
 - `-q`或`--quality`用于指定要下载的视频质量（清晰度），可选值有`MAX`（最高质量，缺省值）、`MIN`（最低质量）、`MANUAL`（手动选择视频质量）
 
-- `--nomerge`表示是否自动合成下载下来的音视频文件，默认合成，但需要提前下载[ffmpeg](https://ffmpeg.org/download.html)工具（[windows版本](https://www.gyan.dev/ffmpeg/builds/)）并将其路径添加到`PATH`环境变量
+- `--nomerge`表示是否自动合成下载下来的音视频文件，默认合成，但需要提前下载[ffmpeg](https://ffmpeg.org/download.html)工具（如[windows版本](https://www.gyan.dev/ffmpeg/builds/)）并将其路径添加到`PATH`环境变量
+
+- `--force`表示强制重新下载视频，如果没有指定`--playlist`参数，则只是重新下载当前剧集，否则会直接删除`bili_tmp/`临时文件，重新下载全部剧集，但不会立即删除全部已下载音视频文件，而是覆盖更新
 
-- `--force`表示强制重新下载视频，携带该参数会直接删除`bili_tmp/`临时文件，但不会立即删除全部已下载音视频文件，而是覆盖更新
+- `--debug`用于在控制台输出全部debug日志信息，不指定该参数，也会将日志输出到`bili_tmp/download.log`中以备查阅
 
-- `--debug`用于在控制台输出全部debug日志信息，不指定该参数，也会将日志输出到`bili_tmp/log`中以备查阅
+- 默认随视频会下载封面图片
 
 - 默认随视频会下载弹幕XML文件，可以使用[danmu2ass](https://github.com/ikde/danmu2ass)做弹幕格式转换，双击Danmu2Ass.sln，用Visual Studio打开并编译，在项目Danmu2Ass目录下会生成bin文件夹，进入其中的Debug文件夹，可以看到一个Kaedei.Danmu2Ass.exe可执行文件，将视频和弹幕文件一块拖动到该可执行文件图标上去即可生成ASS字幕文件，再通过[potplayer](https://potplayer.daum.net/)打开视频即可自动加载字幕
 
 ## 致谢
 
 如果觉得本工具有用，请点个Star呗~，有bug或有改进意见请提issue，thx！
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.4 Summary: A simple tool
+Metadata-Version: 2.1 Name: sole_bili_get Version: 0.0.5 Summary: A simple tool
 to download videos from bilibili{*â§ââ¦} Home-page: https://github.com/
 muggledy/bili-get Author: muggledy Author-email: zgjsycfndy2015@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE.txt Requires-Dist: requests # Bilibiliè§é¢ä¸è½½å¨ ![](https://
-img.shields.io/badge/python-3.6+-green) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/
-_r_e_l_e_a_s_e_/_m_u_g_g_l_e_d_y_/_b_i_l_i_-_g_e_t_] ## ä¸è½½ ### æ¹å¼ä¸ ```console pip install sole-
-bili-get -i https://www.pypi.org/simple/ ``` PSï¼æ´æ°çæ¬ï¼ï¼`pip
-install sole-bili-get -U` ### æ¹å¼äº ```console git clone https://
-github.com/muggledy/bili-get.git python setup.py sdist bdist_wheel pip install
-dist\sole_bili_get-0.0.1-py3-none-any.whl //demo bili-get --help ``` ## ä½¿ç¨
-```console C:\Users\muggledy\Downloads>bili-get https://www.bilibili.com/video/
-BV1CY4y1F7hP output: C:\Users\muggledy\Downloads (origin url):https://
-www.bilibili.com/video/BV1CY4y1F7hP (title):
+LICENSE.txt Requires-Dist: requests Requires-Dist: pycryptodome Requires-Dist:
+pypiwin32 # Bilibiliè§é¢ä¸è½½å¨ ![](https://img.shields.io/badge/python-
+3.6+-green) ![](https://img.shields.io/badge/platform-Windows%20%7C%20Linux-
+pink) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_m_u_g_g_l_e_d_y_/_b_i_l_i_-_g_e_t_] ## ä¸è½½ ###
+æ¹å¼ä¸ ```console pip install sole-bili-get -i https://www.pypi.org/simple/
+``` PSï¼æ´æ°çæ¬ï¼ï¼`pip install sole-bili-get -U` ### æ¹å¼äº
+```console git clone https://github.com/muggledy/bili-get.git python setup.py
+sdist bdist_wheel pip install dist\sole_bili_get-0.0.1-py3-none-any.whl //demo
+bili-get --help ``` ## ä½¿ç¨ ```console C:\Users\muggledy\Downloads>bili-get
+https://www.bilibili.com/video/BV1CY4y1F7hP output: C:\Users\muggledy\Downloads
+(origin url):https://www.bilibili.com/video/BV1CY4y1F7hP (title):
 p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼
 (desc):æ­¤è§é¢éç»å¸æä¸æ°çå®æ­åå¨å¥¥çæåä»¬ï¼ (episodes
 num):7 (quality):æ¸æ° 480P(id:32), æµç 360P(id:16) selected download
 quality(MAX):32 get danmu urls success for 7 episodes p1 danmu xml file is
 downloaded into C:
 \Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼.xml
 start to download p1(video:æ¸æ° 480P,852x480,avc1.64001F_581618_29.412) from
@@ -32,15 +33,15 @@
 Note: this is a multi-episode video, you can download them all at once with --
 playlist ``` - é»è®¤æ¯ä¸è½½å°å½åå·¥ä½è·¯å¾ï¼å¯ä»¥éè¿`-o`æ`--
 output`æå®è¾åºç®å½ï¼ä¸å­å¨åèªå¨åå»ºï¼è­¬å¦`bili-get https://
 www.bilibili.com/video/BV1CY4y1F7hP -o D:\workspace\bilibili`ãè¿ä¼å¨`--
 output`ç®å½ä¸äº§çä¸¤ä¸ªæä»¶å¤¹ï¼`bili_tmp/`å`bili_output/
 `ï¼åèå­æ¾ä¸äºä¸´æ¶æä»¶ï¼ç¨äºè®°å½å¤å§éè§é¢çä¸è½½è¿åº¦ï¼å¦æä¸è½½è¿ç¨ä¸­åçä¸­æ­ï¼éæ°æ§è¡å½ä»¤å¯ä»¥ç»§ç»­ä¸è½½è¿ç¨ï¼ä¸å¯¹äºå°æªåæçå§éä¼å°è¯è¿è¡åæï¼é¤éæå®`-
 -
-nomerge`åæ°ï¼ï¼åèåæ¯è§é¢ãé³é¢ãå¼¹å¹æä»¶çè¾åºæä»¶å¤¹
+nomerge`åæ°ï¼ï¼åèåæ¯è§é¢ãé³é¢ãå°é¢ãå¼¹å¹æä»¶çè¾åºæä»¶å¤¹
 - å¯¹äºå¤å§éè§é¢ï¼å¯ä»¥æå®`--
 playlist`èªå¨ä¸è½½å¨é¨å§éï¼åªè¦ä¸å é¤å¯¹åºç`bili_tmp/
 `ä¸´æ¶æä»¶ï¼å¯ä»¥ä»»æéå¤æ§è¡ä¸è½½å½ä»¤ï¼å¦`bili-get https://
 www.bilibili.com/video/BV1CY4y1F7hP --
 playlist`ï¼ä¹ä¸ä¼éå¤ä¸è½½ï¼å¦æUPä¸»æ°åå¸äºå§éï¼åä¼ç»§ç»­ä¸è½½
 - `-c`æ`--
 cookie`ç¨äºæå®æ¨çBç«Cookieä¿¡æ¯ï¼è¿æ ·å°±å¯ä»¥ä¸è½½1080Pè§é¢äº
@@ -57,25 +58,33 @@
 from https://www.bilibili.com/video/BV1CY4y1F7hP/?p=1...
 100.00%|ââââââââââââââââââââ|
 ä¸è½½å®æãvideo/mp4ã 342.48MB/342.48MB start to download p1(audio)...
 100.00%|ââââââââââââââââââââ|
 ä¸è½½å®æãvideo/mp4ã 28.28MB/28.28MB ffmpeg merge success, save into C:
 \Users\muggledy\Downloads\bili_output\BV1CY4y1F7hP\p1_æ»èæ¶è¿ä¸å¹´ï¼ä¸ç·å¸¦ä½ ä¸æ­¥å°ä½çå®æ­åãå¥¥ç¹æ¼ãç³»åå¨é¨345éæªå½åå®å®äººä»¬ï¼_1åä»£å¥¥ç¹æ¼.mp4
 Note: this is a multi-episode video, you can download them all at once with --
-playlist ``` Cookieè·åæ¹å¼å¦ä¸ï¼ ![](https://raw.githubusercontent.com/
-muggledy/bili-get/master/bilibili_cookie.jpg) - `-q`æ`--
+playlist ``` Cookieè·åæ¹å¼å¦ä¸ï¼ ![Bç«cookieè·åæ¹å¼](https://
+raw.githubusercontent.com/muggledy/bili-get/master/bilibili_cookie.jpg)
+æ³¨ï¼å¦ææ¯Windowså¹³å°ä½¿ç¨Chromeæµè§å¨ï¼å¯ä»¥æå®`-
+c`åæ°ä¸º`chrome`ï¼ç¨åºå°èªå¨ä»`./AppData/Local/Google/Chrome/User
+Data/default/Network/
+Cookies`è¯»åBç«çCookieä¿¡æ¯ï¼è­¬å¦æä»¬å¯ä»¥éè¿`bili-get https://
+www.bilibili.com/video/BV18G411D7FM -c chrome`å½ä»¤ä¸è½½1080pè§é¢ - `-
+q`æ`--
 quality`ç¨äºæå®è¦ä¸è½½çè§é¢è´¨éï¼æ¸æ°åº¦ï¼ï¼å¯éå¼æ`MAX`ï¼æé«è´¨éï¼ç¼ºçå¼ï¼ã`MIN`ï¼æä½è´¨éï¼ã`MANUAL`ï¼æå¨éæ©è§é¢è´¨éï¼
 - `--
 nomerge`è¡¨ç¤ºæ¯å¦èªå¨åæä¸è½½ä¸æ¥çé³è§é¢æä»¶ï¼é»è®¤åæï¼ä½éè¦æåä¸è½½
-[ffmpeg](https://ffmpeg.org/download.html)å·¥å·ï¼[windowsçæ¬](https://
+[ffmpeg](https://ffmpeg.org/download.html)å·¥å·ï¼å¦[windowsçæ¬](https://
 www.gyan.dev/ffmpeg/builds/)ï¼å¹¶å°å¶è·¯å¾æ·»å å°`PATH`ç¯å¢åé - `--
-force`è¡¨ç¤ºå¼ºå¶éæ°ä¸è½½è§é¢ï¼æºå¸¦è¯¥åæ°ä¼ç´æ¥å é¤`bili_tmp/
-`ä¸´æ¶æä»¶ï¼ä½ä¸ä¼ç«å³å é¤å¨é¨å·²ä¸è½½é³è§é¢æä»¶ï¼èæ¯è¦çæ´æ°
+force`è¡¨ç¤ºå¼ºå¶éæ°ä¸è½½è§é¢ï¼å¦ææ²¡ææå®`--
+playlist`åæ°ï¼ååªæ¯éæ°ä¸è½½å½åå§éï¼å¦åä¼ç´æ¥å é¤`bili_tmp/
+`ä¸´æ¶æä»¶ï¼éæ°ä¸è½½å¨é¨å§éï¼ä½ä¸ä¼ç«å³å é¤å¨é¨å·²ä¸è½½é³è§é¢æä»¶ï¼èæ¯è¦çæ´æ°
 - `--
 debug`ç¨äºå¨æ§å¶å°è¾åºå¨é¨debugæ¥å¿ä¿¡æ¯ï¼ä¸æå®è¯¥åæ°ï¼ä¹ä¼å°æ¥å¿è¾åºå°`bili_tmp/
-log`ä¸­ä»¥å¤æ¥é - é»è®¤éè§é¢ä¼ä¸è½½å¼¹å¹XMLæä»¶ï¼å¯ä»¥ä½¿ç¨
-[danmu2ass](https://github.com/ikde/
+download.log`ä¸­ä»¥å¤æ¥é - é»è®¤éè§é¢ä¼ä¸è½½å°é¢å¾ç -
+é»è®¤éè§é¢ä¼ä¸è½½å¼¹å¹XMLæä»¶ï¼å¯ä»¥ä½¿ç¨[danmu2ass](https://
+github.com/ikde/
 danmu2ass)åå¼¹å¹æ ¼å¼è½¬æ¢ï¼åå»Danmu2Ass.slnï¼ç¨Visual
 Studioæå¼å¹¶ç¼è¯ï¼å¨é¡¹ç®Danmu2Assç®å½ä¸ä¼çæbinæä»¶å¤¹ï¼è¿å¥å¶ä¸­çDebugæä»¶å¤¹ï¼å¯ä»¥çå°ä¸ä¸ªKaedei.Danmu2Ass.exeå¯æ§è¡æä»¶ï¼å°è§é¢åå¼¹å¹æä»¶ä¸åæå¨å°è¯¥å¯æ§è¡æä»¶å¾æ ä¸å»å³å¯çæASSå­å¹æä»¶ï¼åéè¿
 [potplayer](https://potplayer.daum.net/)æå¼è§é¢å³å¯èªå¨å è½½å­å¹ ##
 è´è°¢
 å¦æè§å¾æ¬å·¥å·æç¨ï¼è¯·ç¹ä¸ªStarå~ï¼æbugæææ¹è¿æè§è¯·æissueï¼thxï¼
```

