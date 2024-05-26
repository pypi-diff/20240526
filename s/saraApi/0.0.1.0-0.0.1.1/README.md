# Comparing `tmp/saraapi-0.0.1.0.tar.gz` & `tmp/saraapi-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saraapi-0.0.1.0.tar", last modified: Fri May 10 05:08:02 2024, max compression
+gzip compressed data, was "saraapi-0.0.1.1.tar", last modified: Sun May 26 03:38:45 2024, max compression
```

## Comparing `saraapi-0.0.1.0.tar` & `saraapi-0.0.1.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:08:02.580543 saraapi-0.0.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4817 2024-05-10 05:08:02.578300 saraapi-0.0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2024-05-06 04:15:07.000000 saraapi-0.0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 05:08:02.540226 saraapi-0.0.1.0/sara/
--rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.1.0/sara/__init__.py
--rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.1.0/sara/ext.py
--rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.1.0/sara/nsfw.py
--rw-rw-rw-   0        0        0      616 2024-05-10 05:07:28.000000 saraapi-0.0.1.0/sara/req.py
--rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.1.0/sara/sfw.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:08:02.575341 saraapi-0.0.1.0/saraApi.egg-info/
--rw-rw-rw-   0        0        0     4817 2024-05-10 05:08:02.000000 saraapi-0.0.1.0/saraApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-10 05:08:02.000000 saraapi-0.0.1.0/saraApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:08:02.000000 saraapi-0.0.1.0/saraApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 05:08:02.000000 saraapi-0.0.1.0/saraApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 05:08:02.000000 saraapi-0.0.1.0/saraApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 05:08:02.582127 saraapi-0.0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-10 05:07:48.000000 saraapi-0.0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:38:45.136386 saraapi-0.0.1.1/
+-rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5324 2024-05-26 03:38:45.134401 saraapi-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4591 2024-05-26 03:37:57.000000 saraapi-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 03:38:45.065210 saraapi-0.0.1.1/sara/
+-rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.1.1/sara/__init__.py
+-rw-rw-rw-   0        0        0      740 2024-05-26 03:23:22.000000 saraapi-0.0.1.1/sara/ext.py
+-rw-rw-rw-   0        0        0     2021 2024-05-26 03:22:27.000000 saraapi-0.0.1.1/sara/nsfw.py
+-rw-rw-rw-   0        0        0      616 2024-05-10 05:07:28.000000 saraapi-0.0.1.1/sara/req.py
+-rw-rw-rw-   0        0        0      575 2024-05-26 03:38:27.000000 saraapi-0.0.1.1/sara/rolplay.py
+-rw-rw-rw-   0        0        0      268 2024-05-26 03:23:00.000000 saraapi-0.0.1.1/sara/rolplayNsfw.py
+-rw-rw-rw-   0        0        0      988 2024-05-26 03:31:59.000000 saraapi-0.0.1.1/sara/sfw.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:38:45.133168 saraapi-0.0.1.1/saraApi.egg-info/
+-rw-rw-rw-   0        0        0     5324 2024-05-26 03:38:44.000000 saraapi-0.0.1.1/saraApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 03:38:45.000000 saraapi-0.0.1.1/saraApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 03:38:44.000000 saraapi-0.0.1.1/saraApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 03:38:44.000000 saraapi-0.0.1.1/saraApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 03:38:44.000000 saraapi-0.0.1.1/saraApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 03:38:45.136386 saraapi-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-26 03:38:27.000000 saraapi-0.0.1.1/setup.py
```

### Comparing `saraapi-0.0.1.0/PKG-INFO` & `saraapi-0.0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,18 @@
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
 
 ## Changelogs
 ### v0.1
 - new api
 
+### v1.1
+- new commands
+- new categories
+
 ## Example(s)
 **Python:**
 ```python
 import sara
 
 def function_name():
   # Get SFW Neko Images, uwu #
@@ -78,29 +82,45 @@
 sara.sfw.foxgirl()     # Awoo!~ Another example!
 sara.sfw.neko()        # Meow! An Example!
 ```
 Function | Description
 ---|---
 neko | SFW Neko Girls (Cat Girls)
 foxgirl | SFW Fox Girls (Thanks to @LamkasDev!)
+sad | sad :(
+angry | angry
+work | worked
+yandere | yandere
+wink | wink
+vomit | vomit 
+teehee | teehee
+pout | pout
+laugh | laugh
+dance | dance
+cry | cry
+bored | binding
+blush | blus
+run | running
 
 ## NSFW Function(s)
 Function | Description
 ---|---
 ass | I know you like anime ass~ uwu
 bdsm | If you don't know what it is, search it up
 blowjob | Basically an image of a girl sucking on a sharp blade!
+boobs | boobs ~<3
 cum | Basically sticky white stuff that is usually milked from sharpies.
 doujin | Sends a random doujin page imageURL!
 feet | So you like smelly feet huh?
 femdom | Female Domination?
 foxgirl | Girl's that are wannabe foxes, yes
 gifs | Basically an animated image, so yes :3
 glasses | Girls that wear glasses, uwu~
 hentai | Sends a random vanilla hentai imageURL~
+ahegao | Sends a random ahegao image ~
 netorare | Wow, I won't even question your fetishes.
 maid | Maids, Maid Uniforms, etc, you know what maids are :3
 masturbation | Solo Queue in CSGO!
 orgy | Group Lewd Acts
 panties | I mean... just why? You like underwear?
 pussy | The genitals of a female, or a cat, you give the meaning.
 school | School Uniforms!~ Yatta~!
@@ -111,14 +131,23 @@
 uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~
 yuri | Girls on Girls, and Girl's only!<3
 zettaiRyouiki | That one part of the flesh being squeeze in thigh-highs~<3
 
 
 Function | Description
 ---|---
+rolplayNsfw.fuck | sex 
+rolplayNsfw.anal | :0
+rolplayNsfw.happyend | happyend
+rolplayNsfw.kuni | kuni
+rolplayNsfw.spank | spank
+rolplayNsfw.suck | suck
+
+Function | Description
+---|---
 sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.0 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.1 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
@@ -13,45 +13,51 @@
   _____m_o_d_e_u_s___h_e_l_l_t_a_k_e_r___d_r_a_w_n___b_y___k_i_y_o_v_e_r_o_____6_5_b_d_0_b_9_9_d_0_8_0_b_c_e_b_3_9_f_f_f_3_f_4_d_e_7_c_c_5_8_6_._p_n_g_]
 
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use,
 however do understand that I'm the only one working on this, and I hand pick
 images to add, so you may get repeated images! Use it for your Discord Bot,
 your Self Made Console Waifu, or whatever it is :3 ## NOTE: This Readme.md is
 from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/) ##
-Changelogs ### v0.1 - new api ## Example(s) **Python:** ```python import sara
-def function_name(): # Get SFW Neko Images, uwu # print("SFW Neko: " +
-sara.sfw.neko()) # Get Lewd Neko (NSFW), owo # print("Lewd Neko:" +
-sara.lewdNeko()) # Lewd Bomb me onii-san~~ # print("Lewd Bomb: " +
-sara.lewdBomb(5)) # Get other NSFW Images# print("BDSM: " + sara.nsfw.bdsm())
-print("Maid: " + sara.nsfw.maid()) print("Hentai: " + sara.nsfw.hentai()) #
-Call Your Function! function_name() ``` ## Legacy Function(s) Example:
-```python sara.module.function() # Format sara.nsfw.lewdNeko() # Example
-sara.nsfw.lewdBomb(5) # Meow, I'm Example 2 ``` Function | Description ---|--
-- lewdNeko | NSFW Neko Girls (Cat Girls) lewdBomb(n) | Sends (n) amount of
-lewds! :3 ## SFW Function(s) Example: ```python sara.module.function() # Format
-sara.sfw.foxgirl() # Awoo!~ Another example! sara.sfw.neko() # Meow! An
-Example! ``` Function | Description ---|--- neko | SFW Neko Girls (Cat Girls)
-foxgirl | SFW Fox Girls (Thanks to @LamkasDev!) ## NSFW Function(s) Function |
-Description ---|--- ass | I know you like anime ass~ uwu bdsm | If you don't
-know what it is, search it up blowjob | Basically an image of a girl sucking on
-a sharp blade! cum | Basically sticky white stuff that is usually milked from
-sharpies. doujin | Sends a random doujin page imageURL! feet | So you like
-smelly feet huh? femdom | Female Domination? foxgirl | Girl's that are wannabe
-foxes, yes gifs | Basically an animated image, so yes :3 glasses | Girls that
-wear glasses, uwu~ hentai | Sends a random vanilla hentai imageURL~ netorare |
-Wow, I won't even question your fetishes. maid | Maids, Maid Uniforms, etc, you
-know what maids are :3 masturbation | Solo Queue in CSGO! orgy | Group Lewd
-Acts panties | I mean... just why? You like underwear? pussy | The genitals of
-a female, or a cat, you give the meaning. school | School Uniforms!~ Yatta~!
-succubus | Spooky Succubus, oh I'm so scared~ Totally don't suck me~ tentacles
-| I'm sorry but, why do they look like intestines? thighs | The top part of
-your legs, very hot, isn't it? uglyBastard | The one thing most of us can all
-agree to hate :) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~
-yuri | Girls on Girls, and Girl's only!<3 zettaiRyouiki | That one part of the
-flesh being squeeze in thigh-highs~<3 Function | Description ---|--
+Changelogs ### v0.1 - new api ### v1.1 - new commands - new categories ##
+Example(s) **Python:** ```python import sara def function_name(): # Get SFW
+Neko Images, uwu # print("SFW Neko: " + sara.sfw.neko()) # Get Lewd Neko
+(NSFW), owo # print("Lewd Neko:" + sara.lewdNeko()) # Lewd Bomb me onii-san~~ #
+print("Lewd Bomb: " + sara.lewdBomb(5)) # Get other NSFW Images# print("BDSM: "
++ sara.nsfw.bdsm()) print("Maid: " + sara.nsfw.maid()) print("Hentai: " +
+sara.nsfw.hentai()) # Call Your Function! function_name() ``` ## Legacy
+Function(s) Example: ```python sara.module.function() # Format
+sara.nsfw.lewdNeko() # Example sara.nsfw.lewdBomb(5) # Meow, I'm Example 2 ```
+Function | Description ---|--- lewdNeko | NSFW Neko Girls (Cat Girls) lewdBomb
+(n) | Sends (n) amount of lewds! :3 ## SFW Function(s) Example: ```python
+sara.module.function() # Format sara.sfw.foxgirl() # Awoo!~ Another example!
+sara.sfw.neko() # Meow! An Example! ``` Function | Description ---|--- neko |
+SFW Neko Girls (Cat Girls) foxgirl | SFW Fox Girls (Thanks to @LamkasDev!) sad
+| sad :( angry | angry work | worked yandere | yandere wink | wink vomit |
+vomit teehee | teehee pout | pout laugh | laugh dance | dance cry | cry bored |
+binding blush | blus run | running ## NSFW Function(s) Function | Description -
+--|--- ass | I know you like anime ass~ uwu bdsm | If you don't know what it
+is, search it up blowjob | Basically an image of a girl sucking on a sharp
+blade! boobs | boobs ~<3 cum | Basically sticky white stuff that is usually
+milked from sharpies. doujin | Sends a random doujin page imageURL! feet | So
+you like smelly feet huh? femdom | Female Domination? foxgirl | Girl's that are
+wannabe foxes, yes gifs | Basically an animated image, so yes :3 glasses |
+Girls that wear glasses, uwu~ hentai | Sends a random vanilla hentai imageURL~
+ahegao | Sends a random ahegao image ~ netorare | Wow, I won't even question
+your fetishes. maid | Maids, Maid Uniforms, etc, you know what maids are :
+3 masturbation | Solo Queue in CSGO! orgy | Group Lewd Acts panties | I mean...
+just why? You like underwear? pussy | The genitals of a female, or a cat, you
+give the meaning. school | School Uniforms!~ Yatta~! succubus | Spooky
+Succubus, oh I'm so scared~ Totally don't suck me~ tentacles | I'm sorry but,
+why do they look like intestines? thighs | The top part of your legs, very hot,
+isn't it? uglyBastard | The one thing most of us can all agree to hate :
+) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~ yuri | Girls on
+Girls, and Girl's only!<3 zettaiRyouiki | That one part of the flesh being
+squeeze in thigh-highs~<3 Function | Description ---|--- rolplayNsfw.fuck | sex
+rolplayNsfw.anal | :0 rolplayNsfw.happyend | happyend rolplayNsfw.kuni | kuni
+rolplayNsfw.spank | spank rolplayNsfw.suck | suck Function | Description ---|--
 - sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ## Discord
 Bot Example ```python import discord # Import the module import sara from
 discord.ext import commands # get commands from discord.ext client =
 commands.Bot(command_prefix='[PREFIX HERE]') @client.event # the function
```

### Comparing `saraapi-0.0.1.0/README.md` & `saraapi-0.0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
 
 ## Changelogs
 ### v0.1
 - new api
 
+### v1.1
+- new commands
+- new categories
+
 ## Example(s)
 **Python:**
 ```python
 import sara
 
 def function_name():
   # Get SFW Neko Images, uwu #
@@ -57,29 +61,45 @@
 sara.sfw.foxgirl()     # Awoo!~ Another example!
 sara.sfw.neko()        # Meow! An Example!
 ```
 Function | Description
 ---|---
 neko | SFW Neko Girls (Cat Girls)
 foxgirl | SFW Fox Girls (Thanks to @LamkasDev!)
+sad | sad :(
+angry | angry
+work | worked
+yandere | yandere
+wink | wink
+vomit | vomit 
+teehee | teehee
+pout | pout
+laugh | laugh
+dance | dance
+cry | cry
+bored | binding
+blush | blus
+run | running
 
 ## NSFW Function(s)
 Function | Description
 ---|---
 ass | I know you like anime ass~ uwu
 bdsm | If you don't know what it is, search it up
 blowjob | Basically an image of a girl sucking on a sharp blade!
+boobs | boobs ~<3
 cum | Basically sticky white stuff that is usually milked from sharpies.
 doujin | Sends a random doujin page imageURL!
 feet | So you like smelly feet huh?
 femdom | Female Domination?
 foxgirl | Girl's that are wannabe foxes, yes
 gifs | Basically an animated image, so yes :3
 glasses | Girls that wear glasses, uwu~
 hentai | Sends a random vanilla hentai imageURL~
+ahegao | Sends a random ahegao image ~
 netorare | Wow, I won't even question your fetishes.
 maid | Maids, Maid Uniforms, etc, you know what maids are :3
 masturbation | Solo Queue in CSGO!
 orgy | Group Lewd Acts
 panties | I mean... just why? You like underwear?
 pussy | The genitals of a female, or a cat, you give the meaning.
 school | School Uniforms!~ Yatta~!
@@ -90,14 +110,23 @@
 uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~
 yuri | Girls on Girls, and Girl's only!<3
 zettaiRyouiki | That one part of the flesh being squeeze in thigh-highs~<3
 
 
 Function | Description
 ---|---
+rolplayNsfw.fuck | sex 
+rolplayNsfw.anal | :0
+rolplayNsfw.happyend | happyend
+rolplayNsfw.kuni | kuni
+rolplayNsfw.spank | spank
+rolplayNsfw.suck | suck
+
+Function | Description
+---|---
 sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop)
```

#### html2text {}

```diff
@@ -3,45 +3,51 @@
   _____m_o_d_e_u_s___h_e_l_l_t_a_k_e_r___d_r_a_w_n___b_y___k_i_y_o_v_e_r_o_____6_5_b_d_0_b_9_9_d_0_8_0_b_c_e_b_3_9_f_f_f_3_f_4_d_e_7_c_c_5_8_6_._p_n_g_]
 
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use,
 however do understand that I'm the only one working on this, and I hand pick
 images to add, so you may get repeated images! Use it for your Discord Bot,
 your Self Made Console Waifu, or whatever it is :3 ## NOTE: This Readme.md is
 from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/) ##
-Changelogs ### v0.1 - new api ## Example(s) **Python:** ```python import sara
-def function_name(): # Get SFW Neko Images, uwu # print("SFW Neko: " +
-sara.sfw.neko()) # Get Lewd Neko (NSFW), owo # print("Lewd Neko:" +
-sara.lewdNeko()) # Lewd Bomb me onii-san~~ # print("Lewd Bomb: " +
-sara.lewdBomb(5)) # Get other NSFW Images# print("BDSM: " + sara.nsfw.bdsm())
-print("Maid: " + sara.nsfw.maid()) print("Hentai: " + sara.nsfw.hentai()) #
-Call Your Function! function_name() ``` ## Legacy Function(s) Example:
-```python sara.module.function() # Format sara.nsfw.lewdNeko() # Example
-sara.nsfw.lewdBomb(5) # Meow, I'm Example 2 ``` Function | Description ---|--
-- lewdNeko | NSFW Neko Girls (Cat Girls) lewdBomb(n) | Sends (n) amount of
-lewds! :3 ## SFW Function(s) Example: ```python sara.module.function() # Format
-sara.sfw.foxgirl() # Awoo!~ Another example! sara.sfw.neko() # Meow! An
-Example! ``` Function | Description ---|--- neko | SFW Neko Girls (Cat Girls)
-foxgirl | SFW Fox Girls (Thanks to @LamkasDev!) ## NSFW Function(s) Function |
-Description ---|--- ass | I know you like anime ass~ uwu bdsm | If you don't
-know what it is, search it up blowjob | Basically an image of a girl sucking on
-a sharp blade! cum | Basically sticky white stuff that is usually milked from
-sharpies. doujin | Sends a random doujin page imageURL! feet | So you like
-smelly feet huh? femdom | Female Domination? foxgirl | Girl's that are wannabe
-foxes, yes gifs | Basically an animated image, so yes :3 glasses | Girls that
-wear glasses, uwu~ hentai | Sends a random vanilla hentai imageURL~ netorare |
-Wow, I won't even question your fetishes. maid | Maids, Maid Uniforms, etc, you
-know what maids are :3 masturbation | Solo Queue in CSGO! orgy | Group Lewd
-Acts panties | I mean... just why? You like underwear? pussy | The genitals of
-a female, or a cat, you give the meaning. school | School Uniforms!~ Yatta~!
-succubus | Spooky Succubus, oh I'm so scared~ Totally don't suck me~ tentacles
-| I'm sorry but, why do they look like intestines? thighs | The top part of
-your legs, very hot, isn't it? uglyBastard | The one thing most of us can all
-agree to hate :) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~
-yuri | Girls on Girls, and Girl's only!<3 zettaiRyouiki | That one part of the
-flesh being squeeze in thigh-highs~<3 Function | Description ---|--
+Changelogs ### v0.1 - new api ### v1.1 - new commands - new categories ##
+Example(s) **Python:** ```python import sara def function_name(): # Get SFW
+Neko Images, uwu # print("SFW Neko: " + sara.sfw.neko()) # Get Lewd Neko
+(NSFW), owo # print("Lewd Neko:" + sara.lewdNeko()) # Lewd Bomb me onii-san~~ #
+print("Lewd Bomb: " + sara.lewdBomb(5)) # Get other NSFW Images# print("BDSM: "
++ sara.nsfw.bdsm()) print("Maid: " + sara.nsfw.maid()) print("Hentai: " +
+sara.nsfw.hentai()) # Call Your Function! function_name() ``` ## Legacy
+Function(s) Example: ```python sara.module.function() # Format
+sara.nsfw.lewdNeko() # Example sara.nsfw.lewdBomb(5) # Meow, I'm Example 2 ```
+Function | Description ---|--- lewdNeko | NSFW Neko Girls (Cat Girls) lewdBomb
+(n) | Sends (n) amount of lewds! :3 ## SFW Function(s) Example: ```python
+sara.module.function() # Format sara.sfw.foxgirl() # Awoo!~ Another example!
+sara.sfw.neko() # Meow! An Example! ``` Function | Description ---|--- neko |
+SFW Neko Girls (Cat Girls) foxgirl | SFW Fox Girls (Thanks to @LamkasDev!) sad
+| sad :( angry | angry work | worked yandere | yandere wink | wink vomit |
+vomit teehee | teehee pout | pout laugh | laugh dance | dance cry | cry bored |
+binding blush | blus run | running ## NSFW Function(s) Function | Description -
+--|--- ass | I know you like anime ass~ uwu bdsm | If you don't know what it
+is, search it up blowjob | Basically an image of a girl sucking on a sharp
+blade! boobs | boobs ~<3 cum | Basically sticky white stuff that is usually
+milked from sharpies. doujin | Sends a random doujin page imageURL! feet | So
+you like smelly feet huh? femdom | Female Domination? foxgirl | Girl's that are
+wannabe foxes, yes gifs | Basically an animated image, so yes :3 glasses |
+Girls that wear glasses, uwu~ hentai | Sends a random vanilla hentai imageURL~
+ahegao | Sends a random ahegao image ~ netorare | Wow, I won't even question
+your fetishes. maid | Maids, Maid Uniforms, etc, you know what maids are :
+3 masturbation | Solo Queue in CSGO! orgy | Group Lewd Acts panties | I mean...
+just why? You like underwear? pussy | The genitals of a female, or a cat, you
+give the meaning. school | School Uniforms!~ Yatta~! succubus | Spooky
+Succubus, oh I'm so scared~ Totally don't suck me~ tentacles | I'm sorry but,
+why do they look like intestines? thighs | The top part of your legs, very hot,
+isn't it? uglyBastard | The one thing most of us can all agree to hate :
+) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~ yuri | Girls on
+Girls, and Girl's only!<3 zettaiRyouiki | That one part of the flesh being
+squeeze in thigh-highs~<3 Function | Description ---|--- rolplayNsfw.fuck | sex
+rolplayNsfw.anal | :0 rolplayNsfw.happyend | happyend rolplayNsfw.kuni | kuni
+rolplayNsfw.spank | spank rolplayNsfw.suck | suck Function | Description ---|--
 - sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ## Discord
 Bot Example ```python import discord # Import the module import sara from
 discord.ext import commands # get commands from discord.ext client =
 commands.Bot(command_prefix='[PREFIX HERE]') @client.event # the function
```

### Comparing `saraapi-0.0.1.0/sara/ext.py` & `saraapi-0.0.1.1/sara/ext.py`

 * *Files 25% similar despite different names*

```diff
@@ -37,9 +37,23 @@
     tentacles
     masturbation
     school
     yuri
     zettaiRyouiki
     zettairyouiki
     succubus
+ROLPLAYNSFW:
+    anal
+    fuck
+    happyend
+    spank
+    suck
+    kuni
+ROLPLAYSFW:
+    baka
+    kiss
+    kill
+    spank
+    puch
+    poke
     """
     return message
```

### Comparing `saraapi-0.0.1.0/sara/nsfw.py` & `saraapi-0.0.1.1/sara/nsfw.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,20 @@
         r = get('random')
         urls.append(r)
     return urls
 
 def ass():
     return get('ass')
 
+def boobs():
+    return get('boobs')
+
+def ahegao():
+    return get('ahegao')
+
 def bdsm():
     return get('bdsm')
 
 def bondage():
     return get('bdsm')
 
 def cum():
```

### Comparing `saraapi-0.0.1.0/sara/req.py` & `saraapi-0.0.1.1/sara/req.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.1.0/saraApi.egg-info/PKG-INFO` & `saraapi-0.0.1.1/saraApi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,18 @@
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
 
 ## Changelogs
 ### v0.1
 - new api
 
+### v1.1
+- new commands
+- new categories
+
 ## Example(s)
 **Python:**
 ```python
 import sara
 
 def function_name():
   # Get SFW Neko Images, uwu #
@@ -78,29 +82,45 @@
 sara.sfw.foxgirl()     # Awoo!~ Another example!
 sara.sfw.neko()        # Meow! An Example!
 ```
 Function | Description
 ---|---
 neko | SFW Neko Girls (Cat Girls)
 foxgirl | SFW Fox Girls (Thanks to @LamkasDev!)
+sad | sad :(
+angry | angry
+work | worked
+yandere | yandere
+wink | wink
+vomit | vomit 
+teehee | teehee
+pout | pout
+laugh | laugh
+dance | dance
+cry | cry
+bored | binding
+blush | blus
+run | running
 
 ## NSFW Function(s)
 Function | Description
 ---|---
 ass | I know you like anime ass~ uwu
 bdsm | If you don't know what it is, search it up
 blowjob | Basically an image of a girl sucking on a sharp blade!
+boobs | boobs ~<3
 cum | Basically sticky white stuff that is usually milked from sharpies.
 doujin | Sends a random doujin page imageURL!
 feet | So you like smelly feet huh?
 femdom | Female Domination?
 foxgirl | Girl's that are wannabe foxes, yes
 gifs | Basically an animated image, so yes :3
 glasses | Girls that wear glasses, uwu~
 hentai | Sends a random vanilla hentai imageURL~
+ahegao | Sends a random ahegao image ~
 netorare | Wow, I won't even question your fetishes.
 maid | Maids, Maid Uniforms, etc, you know what maids are :3
 masturbation | Solo Queue in CSGO!
 orgy | Group Lewd Acts
 panties | I mean... just why? You like underwear?
 pussy | The genitals of a female, or a cat, you give the meaning.
 school | School Uniforms!~ Yatta~!
@@ -111,14 +131,23 @@
 uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~
 yuri | Girls on Girls, and Girl's only!<3
 zettaiRyouiki | That one part of the flesh being squeeze in thigh-highs~<3
 
 
 Function | Description
 ---|---
+rolplayNsfw.fuck | sex 
+rolplayNsfw.anal | :0
+rolplayNsfw.happyend | happyend
+rolplayNsfw.kuni | kuni
+rolplayNsfw.spank | spank
+rolplayNsfw.suck | suck
+
+Function | Description
+---|---
 sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.0 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.1.1 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
@@ -13,45 +13,51 @@
   _____m_o_d_e_u_s___h_e_l_l_t_a_k_e_r___d_r_a_w_n___b_y___k_i_y_o_v_e_r_o_____6_5_b_d_0_b_9_9_d_0_8_0_b_c_e_b_3_9_f_f_f_3_f_4_d_e_7_c_c_5_8_6_._p_n_g_]
 
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use,
 however do understand that I'm the only one working on this, and I hand pick
 images to add, so you may get repeated images! Use it for your Discord Bot,
 your Self Made Console Waifu, or whatever it is :3 ## NOTE: This Readme.md is
 from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/) ##
-Changelogs ### v0.1 - new api ## Example(s) **Python:** ```python import sara
-def function_name(): # Get SFW Neko Images, uwu # print("SFW Neko: " +
-sara.sfw.neko()) # Get Lewd Neko (NSFW), owo # print("Lewd Neko:" +
-sara.lewdNeko()) # Lewd Bomb me onii-san~~ # print("Lewd Bomb: " +
-sara.lewdBomb(5)) # Get other NSFW Images# print("BDSM: " + sara.nsfw.bdsm())
-print("Maid: " + sara.nsfw.maid()) print("Hentai: " + sara.nsfw.hentai()) #
-Call Your Function! function_name() ``` ## Legacy Function(s) Example:
-```python sara.module.function() # Format sara.nsfw.lewdNeko() # Example
-sara.nsfw.lewdBomb(5) # Meow, I'm Example 2 ``` Function | Description ---|--
-- lewdNeko | NSFW Neko Girls (Cat Girls) lewdBomb(n) | Sends (n) amount of
-lewds! :3 ## SFW Function(s) Example: ```python sara.module.function() # Format
-sara.sfw.foxgirl() # Awoo!~ Another example! sara.sfw.neko() # Meow! An
-Example! ``` Function | Description ---|--- neko | SFW Neko Girls (Cat Girls)
-foxgirl | SFW Fox Girls (Thanks to @LamkasDev!) ## NSFW Function(s) Function |
-Description ---|--- ass | I know you like anime ass~ uwu bdsm | If you don't
-know what it is, search it up blowjob | Basically an image of a girl sucking on
-a sharp blade! cum | Basically sticky white stuff that is usually milked from
-sharpies. doujin | Sends a random doujin page imageURL! feet | So you like
-smelly feet huh? femdom | Female Domination? foxgirl | Girl's that are wannabe
-foxes, yes gifs | Basically an animated image, so yes :3 glasses | Girls that
-wear glasses, uwu~ hentai | Sends a random vanilla hentai imageURL~ netorare |
-Wow, I won't even question your fetishes. maid | Maids, Maid Uniforms, etc, you
-know what maids are :3 masturbation | Solo Queue in CSGO! orgy | Group Lewd
-Acts panties | I mean... just why? You like underwear? pussy | The genitals of
-a female, or a cat, you give the meaning. school | School Uniforms!~ Yatta~!
-succubus | Spooky Succubus, oh I'm so scared~ Totally don't suck me~ tentacles
-| I'm sorry but, why do they look like intestines? thighs | The top part of
-your legs, very hot, isn't it? uglyBastard | The one thing most of us can all
-agree to hate :) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~
-yuri | Girls on Girls, and Girl's only!<3 zettaiRyouiki | That one part of the
-flesh being squeeze in thigh-highs~<3 Function | Description ---|--
+Changelogs ### v0.1 - new api ### v1.1 - new commands - new categories ##
+Example(s) **Python:** ```python import sara def function_name(): # Get SFW
+Neko Images, uwu # print("SFW Neko: " + sara.sfw.neko()) # Get Lewd Neko
+(NSFW), owo # print("Lewd Neko:" + sara.lewdNeko()) # Lewd Bomb me onii-san~~ #
+print("Lewd Bomb: " + sara.lewdBomb(5)) # Get other NSFW Images# print("BDSM: "
++ sara.nsfw.bdsm()) print("Maid: " + sara.nsfw.maid()) print("Hentai: " +
+sara.nsfw.hentai()) # Call Your Function! function_name() ``` ## Legacy
+Function(s) Example: ```python sara.module.function() # Format
+sara.nsfw.lewdNeko() # Example sara.nsfw.lewdBomb(5) # Meow, I'm Example 2 ```
+Function | Description ---|--- lewdNeko | NSFW Neko Girls (Cat Girls) lewdBomb
+(n) | Sends (n) amount of lewds! :3 ## SFW Function(s) Example: ```python
+sara.module.function() # Format sara.sfw.foxgirl() # Awoo!~ Another example!
+sara.sfw.neko() # Meow! An Example! ``` Function | Description ---|--- neko |
+SFW Neko Girls (Cat Girls) foxgirl | SFW Fox Girls (Thanks to @LamkasDev!) sad
+| sad :( angry | angry work | worked yandere | yandere wink | wink vomit |
+vomit teehee | teehee pout | pout laugh | laugh dance | dance cry | cry bored |
+binding blush | blus run | running ## NSFW Function(s) Function | Description -
+--|--- ass | I know you like anime ass~ uwu bdsm | If you don't know what it
+is, search it up blowjob | Basically an image of a girl sucking on a sharp
+blade! boobs | boobs ~<3 cum | Basically sticky white stuff that is usually
+milked from sharpies. doujin | Sends a random doujin page imageURL! feet | So
+you like smelly feet huh? femdom | Female Domination? foxgirl | Girl's that are
+wannabe foxes, yes gifs | Basically an animated image, so yes :3 glasses |
+Girls that wear glasses, uwu~ hentai | Sends a random vanilla hentai imageURL~
+ahegao | Sends a random ahegao image ~ netorare | Wow, I won't even question
+your fetishes. maid | Maids, Maid Uniforms, etc, you know what maids are :
+3 masturbation | Solo Queue in CSGO! orgy | Group Lewd Acts panties | I mean...
+just why? You like underwear? pussy | The genitals of a female, or a cat, you
+give the meaning. school | School Uniforms!~ Yatta~! succubus | Spooky
+Succubus, oh I'm so scared~ Totally don't suck me~ tentacles | I'm sorry but,
+why do they look like intestines? thighs | The top part of your legs, very hot,
+isn't it? uglyBastard | The one thing most of us can all agree to hate :
+) uniform |Military, Konbini, Work, Nurse Uniforms, etc!~ Sexy~ yuri | Girls on
+Girls, and Girl's only!<3 zettaiRyouiki | That one part of the flesh being
+squeeze in thigh-highs~<3 Function | Description ---|--- rolplayNsfw.fuck | sex
+rolplayNsfw.anal | :0 rolplayNsfw.happyend | happyend rolplayNsfw.kuni | kuni
+rolplayNsfw.spank | spank rolplayNsfw.suck | suck Function | Description ---|--
 - sara.sfw.mobileWallpapers() | Fetch a random SFW Wallpaper! (Mobile)
 sara.sfw.wallpapers() | Fetch a random SFW Wallpaper! (Desktop)
 sara.nsfw.mobileWallpapers() | Fetch a random NSFW Wallpaper! (Mobile)
 sara.nsfw.wallpapers() | Fetch a random NSFW Wallpaper! (Desktop) ## Discord
 Bot Example ```python import discord # Import the module import sara from
 discord.ext import commands # get commands from discord.ext client =
 commands.Bot(command_prefix='[PREFIX HERE]') @client.event # the function
```

### Comparing `saraapi-0.0.1.0/setup.py` & `saraapi-0.0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md','r', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 install_requires = [
 	'requests'
 ]
 
-version = '0.0.1.0'
+version = '0.0.1.1'
 
 setup(
     author='evergaster',
     version=version,
     description='sara api public based akanekopy',
     install_package_data=True,
     install_requires=install_requires,
```

