# Comparing `tmp/henxel-0.3.1.tar.gz` & `tmp/henxel-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henxel-0.3.1.tar", last modified: Mon Apr 15 17:33:54 2024, max compression
+gzip compressed data, was "henxel-0.3.2.tar", last modified: Sun May 26 14:25:57 2024, max compression
```

## Comparing `henxel-0.3.1.tar` & `henxel-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.893362 henxel-0.3.1/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2024-03-26 11:13:09.000000 henxel-0.3.1/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2024-03-26 11:13:09.000000 henxel-0.3.1/MANIFEST.in
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5351 2024-04-15 17:33:54.893362 henxel-0.3.1/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4616 2024-04-15 17:30:33.000000 henxel-0.3.1/README.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2024-04-15 17:30:33.000000 henxel-0.3.1/pyproject.toml
--rw-r--r--   0 samuel    (1000) samuel    (1000)      833 2024-04-15 17:33:54.893362 henxel-0.3.1/setup.cfg
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.869362 henxel-0.3.1/src/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.893362 henxel-0.3.1/src/henxel/
--rw-r--r--   0 samuel    (1000) samuel    (1000)   165232 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    10837 2024-03-26 17:17:11.000000 henxel-0.3.1/src/henxel/changefont.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2024-03-26 11:13:09.000000 henxel-0.3.1/src/henxel/editor.png
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7571 2024-03-26 11:13:09.000000 henxel-0.3.1/src/henxel/fdialog.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     8153 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/help.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)     8141 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/help_mac.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2947 2024-04-15 17:30:33.000000 henxel-0.3.1/src/henxel/wordexpand.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-04-15 17:33:54.893362 henxel-0.3.1/src/henxel.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5351 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      351 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2024-04-15 17:33:54.000000 henxel-0.3.1/src/henxel.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-05-26 14:25:57.436615 henxel-0.3.2/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2024-03-26 11:13:09.000000 henxel-0.3.2/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2024-03-26 11:13:09.000000 henxel-0.3.2/MANIFEST.in
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5360 2024-05-26 14:25:57.436615 henxel-0.3.2/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     4625 2024-05-26 14:25:05.000000 henxel-0.3.2/README.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2024-04-15 17:38:25.000000 henxel-0.3.2/pyproject.toml
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      833 2024-05-26 14:25:57.440614 henxel-0.3.2/setup.cfg
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-05-26 14:25:57.412616 henxel-0.3.2/src/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-05-26 14:25:57.436615 henxel-0.3.2/src/henxel/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)   176653 2024-05-26 14:25:05.000000 henxel-0.3.2/src/henxel/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8827 2024-05-26 14:25:05.000000 henxel-0.3.2/src/henxel/changefont.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2024-03-26 11:13:09.000000 henxel-0.3.2/src/henxel/editor.png
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7571 2024-03-26 11:13:09.000000 henxel-0.3.2/src/henxel/fdialog.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8045 2024-05-26 14:25:05.000000 henxel-0.3.2/src/henxel/help.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8033 2024-05-26 14:25:05.000000 henxel-0.3.2/src/henxel/help_mac.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2947 2024-04-15 17:30:33.000000 henxel-0.3.2/src/henxel/wordexpand.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2024-05-26 14:25:57.436615 henxel-0.3.2/src/henxel.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     5360 2024-05-26 14:25:57.000000 henxel-0.3.2/src/henxel.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      351 2024-05-26 14:25:57.000000 henxel-0.3.2/src/henxel.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2024-05-26 14:25:57.000000 henxel-0.3.2/src/henxel.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2024-05-26 14:25:57.000000 henxel-0.3.2/src/henxel.egg-info/top_level.txt
```

### Comparing `henxel-0.3.1/LICENSE` & `henxel-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `henxel-0.3.1/PKG-INFO` & `henxel-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.3.1
+Version: 0.3.2
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Editors
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Henxel
 GUI-editor for Python development. Tested to work with Debian 12, Windows 10 and 11 and macOS 12.
 
 ![editor_mac](pics/editor_macOS.png)
+
 ![editor_linux](pics/editor_linux.png)
 
 # Featuring
 * Auto-indent
 * Font Chooser
 * Color Chooser
 * Line numbering
@@ -112,16 +113,16 @@
 
 Launch Henxel:
 myproject> env\launch_ed.bat
 ```
 
 
 # Prerequisites in macOS and venv-creation
-Python installation (you may need to install newer version of python from python.org)
-should already include tkinter. There currently is no mkvenv script for macOS,
+You will need to install newer version of python with Homebrew. Look info on the ARR-repository
+about how to do that. There currently is no mkvenv script for macOS,
 but making venv is quite same as in Linux. It seems to be enough to make venv
 and then install henxel to it without anything else.
 
 ```console
 ~$ mkdir myproject
 ~$ cd myproject
 ~/myproject$ python -m venv env
@@ -173,13 +174,15 @@
 (env) ~/myproject/henxel$ pip install --no-build-isolation -e .
 ```
 
 Files are in src/henxel/
 
 
 # More resources
-[Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
-[Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
-[Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
+* [Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
+
+* [Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
+
+* [Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
 
 # Licence
 This project is licensed under the terms of the GNU General Public License v3.0.
```

### Comparing `henxel-0.3.1/README.md` & `henxel-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Henxel
 GUI-editor for Python development. Tested to work with Debian 12, Windows 10 and 11 and macOS 12.
 
 ![editor_mac](pics/editor_macOS.png)
+
 ![editor_linux](pics/editor_linux.png)
 
 # Featuring
 * Auto-indent
 * Font Chooser
 * Color Chooser
 * Line numbering
@@ -92,16 +93,16 @@
 
 Launch Henxel:
 myproject> env\launch_ed.bat
 ```
 
 
 # Prerequisites in macOS and venv-creation
-Python installation (you may need to install newer version of python from python.org)
-should already include tkinter. There currently is no mkvenv script for macOS,
+You will need to install newer version of python with Homebrew. Look info on the ARR-repository
+about how to do that. There currently is no mkvenv script for macOS,
 but making venv is quite same as in Linux. It seems to be enough to make venv
 and then install henxel to it without anything else.
 
 ```console
 ~$ mkdir myproject
 ~$ cd myproject
 ~/myproject$ python -m venv env
@@ -153,13 +154,15 @@
 (env) ~/myproject/henxel$ pip install --no-build-isolation -e .
 ```
 
 Files are in src/henxel/
 
 
 # More resources
-[Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
-[Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
-[Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
+* [Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
+
+* [Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
+
+* [Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
 
 # Licence
 This project is licensed under the terms of the GNU General Public License v3.0.
```

### Comparing `henxel-0.3.1/setup.cfg` & `henxel-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = henxel
-version = 0.3.1
+version = 0.3.2
 author = SamuelKos
 author_email = koskinens371@gmail.com
 description = GUI-editor for Python development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SamuelKos/henxel
 project_urls = 
@@ -20,15 +20,15 @@
 	Topic :: Text Editors
 
 [options]
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
-python_requires = >=3.12
+python_requires = >=3.11
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `henxel-0.3.1/src/henxel/__init__.py` & `henxel-0.3.2/src/henxel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,17 +277,20 @@
 	def __init__(self):
 		
 		self.root = self.__class__.root
 		super().__init__(self.root, class_='Henxel', bd=4)
 		self.protocol("WM_DELETE_WINDOW", self.quit_me)
 		
 		
-		# other widgets
+		# Other widgets
 		self.to_be_closed = list()
 		
+		# Used in check_caps
+		self.to_be_cancelled = list()
+		
 		self.ln_string = ''
 		self.want_ln = True
 		self.syntax = True
 		self.oldconf = None
 		self.tab_char = TAB_WIDTH_CHAR
 			
 		if sys.prefix != sys.base_prefix:
@@ -330,14 +333,18 @@
 		self.tracevar_filename = tkinter.StringVar()
 		self.tracefunc_name = None
 		self.lastdir = None
 
 		self.check_pars = False
 		self.par_err = False
 		
+		# Used in copy() and paste()
+		self.flag_fix_indent = False
+		self.checksum_fix_indent = False
+
 		self.waitvar = tkinter.IntVar()
 		self.fullscreen = False
 		self.state = 'normal'
 		
 		
 		self.helptxt = 'Could not load help-file. Press ESC to return.'
 		
@@ -352,26 +359,40 @@
 		
 		# Initiate widgets
 		####################################
 		self.btn_git = tkinter.Button(self, takefocus=0)
 		
 		if self.branch:
 			branch = self.branch[:5]
+			# Set branch name lenght to 5.
+			# Reason: avoid ln_widget geometry changes
+			# when showing capslock-state in btn_git.
+			if len(branch) < 5:
+				diff = 5-len(branch)
+				t=1
+				for i in range(diff):
+					if t > 0:
+						branch += ' '
+					else:
+						branch = ' ' + branch
+
+					t *= -1
+
 			self.btn_git.config(font=self.menufont, relief='flat', highlightthickness=0,
 						padx=0, text=branch, state='disabled')
 
 			if 'main' in self.branch or 'master' in self.branch:
 				self.btn_git.config(disabledforeground='brown1')
 
 		else:
 			self.btn_git.config(font=self.menufont, relief='flat', highlightthickness=0,
 						padx=0, bitmap='info', state='disabled')
 
 		
-		self.entry = tkinter.Entry(self, bd=4, highlightthickness=0)
+		self.entry = tkinter.Entry(self, bd=4, highlightthickness=0, takefocus=0)
 		if self.os_type != 'mac_os': self.entry.config(bg='#d9d9d9')
 		self.entry.bind("<Return>", self.load)
 		
 		self.btn_open=tkinter.Button(self, takefocus=0, text='Open', bd=4, highlightthickness=0, command=self.load)
 		self.btn_save=tkinter.Button(self, takefocus=0, text='Save', bd=4, highlightthickness=0, command=self.save)
 		
 		# Get conf:
@@ -404,15 +425,15 @@
 		# disable copying linenumbers:
 		shortcut = '<Mod1-Key-c>'
 		if self.os_type != 'mac_os': shortcut = '<Control-c>'
 		self.ln_widget.bind(shortcut, self.no_copy_ln)
 		
 		self.contents = tkinter.Text(self, undo=True, maxundo=-1, autoseparators=True, tabstyle='wordprocessor', highlightthickness=0, bd=4, pady=4, padx=10)
 		
-		self.scrollbar = tkinter.Scrollbar(self, orient=tkinter.VERTICAL, highlightthickness=0, bd=0, command = self.contents.yview)
+		self.scrollbar = tkinter.Scrollbar(self, orient=tkinter.VERTICAL, highlightthickness=0, bd=0, takefocus=0, command = self.contents.yview)
 
 		# tab-completion, used in tab_override()
 		self.expander = wordexpand.ExpandWord(self.contents)
 		
 		
 		# Needed in leave() taglink in: Run file Related
 		self.name_of_cursor_in_text_widget = self.contents['cursor']
@@ -459,16 +480,16 @@
 		if self.os_type == 'windows':
 			
 			# To fix: replace array ::tcl::WordBreakRE contents with newer version, and
 			# replace proc tk::TextNextWord with newer version which was looked in Debian 12
 			# Need for some reason generate event: <<NextWord>> before this,
 			# because array ::tcl::WordBreakRE does not exist yet,
 			# but after this event it does. This was done above.
-
-			self.tk.eval('set l3 [list previous {\W*(\w+)\W*$} after {\w\W|\W\w} next {\w*\W+\w} end {\W*\w+\W} before {^.*(\w\W|\W\w)}] ')
+			
+			self.tk.eval(r'set l3 [list previous {\W*(\w+)\W*$} after {\w\W|\W\w} next {\w*\W+\w} end {\W*\w+\W} before {^.*(\w\W|\W\w)}] ')
 			self.tk.eval('array set ::tcl::WordBreakRE $l3 ')
 			self.tk.eval('proc tk::TextNextWord {w start} {TextNextPos $w $start tcl_endOfWord} ')
 
 		
 		if data:
 			self.apply_config()
 			
@@ -515,14 +536,15 @@
 		d['selfs'] = ['', gray]
 		n['selfs'] = ['', gray]
 		
 		d['match'] = ['lightyellow', 'black']
 		n['match'] = ['lightyellow', 'black']
 		d['focus'] = ['lightgreen', 'black']
 		n['focus'] = ['lightgreen', 'black']
+		
 		d['replaced'] = ['yellow', 'black']
 		n['replaced'] = ['yellow', 'black']
 		
 		d['mismatch'] = ['brown1', 'white']
 		n['mismatch'] = ['brown1', 'white']
 		
 		d['sel'] = ['#c3c3c3', black]
@@ -623,23 +645,17 @@
 			self.right_mousebutton_num = 2
 			
 			# Default cmd-q does not trigger quit_me
 			# Override Cmd-Q:
 			# https://www.tcl.tk/man/tcl8.6/TkCmd/tk_mac.html
 			self.root.createcommand("tk::mac::Quit", self.quit_me)
 			#self.root.createcommand("tk::mac::OnHide", self.test_hide)
-				
+			
 		self.contents.bind( "<Button-%i>" % self.right_mousebutton_num, self.raise_popup)
 		
-		
-		if self.os_type == 'windows':
-			# fix copying to clipboard in Windows.
-			self.bind( "<Control-c>", self.copy_windows)
-		
-		
 		if self.os_type == 'linux':
 			self.contents.bind( "<ISO_Left_Tab>", self.unindent)
 		
 		
 		############################################################
 		# In macOS all Alt-shortcuts makes some special symbol.
 		# Have to bind to this symbol-name to get Alt-shorcuts work.
@@ -679,16 +695,20 @@
 			self.bind( "<Alt-w>", self.walk_tabs)
 			self.bind( "<Alt-q>", lambda event: self.walk_tabs(event, **{'back':True}) )
 			
 			self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
 			self.contents.bind( "<Alt-l>", self.toggle_ln)
 			self.contents.bind( "<Alt-x>", self.toggle_syntax)
 			self.contents.bind( "<Alt-f>", self.font_choose)
-		
+			
+			self.contents.bind( "<Control-c>", self.copy)
 			self.contents.bind( "<Control-v>", self.paste)
+			self.contents.bind( "<Control-x>",
+				lambda event: self.copy(event, **{'flag_cut':True}) )
+			
 			self.contents.bind( "<Control-y>", self.yank_line)
 			
 			self.contents.bind( "<Control-Left>", self.move_by_words)
 			self.contents.bind( "<Control-Right>", self.move_by_words)
 			self.contents.bind( "<Control-Shift-Left>", self.select_by_words)
 			self.contents.bind( "<Control-Shift-Right>", self.select_by_words)
 			
@@ -727,21 +747,28 @@
 			#self.contents.bind( "<Command-Key-k>", lambda event, arg=('AAA'): print(arg) )
 			#self.contents.bind( "<Mod1-Key-k>", lambda event, arg=('AAA'): print(arg) )
 			
 			
 			self.contents.bind( "<Mod1-Key-y>", self.yank_line)
 			self.contents.bind( "<Mod1-Key-n>", self.new_tab)
 			self.contents.bind( "<Mod1-Key-f>", self.search)
+			
+			self.contents.bind( "<Mod1-Key-c>", self.copy)
 			self.contents.bind( "<Mod1-Key-v>", self.paste)
+			self.contents.bind( "<Mod1-Key-x>",
+				lambda event: self.copy(event, **{'flag_cut':True}) )
+			
 			self.contents.bind( "<Mod1-Key-R>", self.replace_all)
 			self.contents.bind( "<Mod1-Key-g>", self.gotoline)
 			self.contents.bind( "<Mod1-Key-a>", self.goto_linestart)
 			self.contents.bind( "<Mod1-Key-e>", self.goto_lineend)
+			
 			self.entry.bind( "<Mod1-Key-a>", self.goto_linestart)
 			self.entry.bind( "<Mod1-Key-e>", self.goto_lineend)
+			
 			self.contents.bind( "<Mod1-Key-r>", self.replace)
 			self.contents.bind( "<Mod1-Key-z>", self.undo_override)
 			self.contents.bind( "<Mod1-Key-Z>", self.redo_override)
 			
 			# Could not get keysym for Alt-l and x, so use ctrl
 			self.contents.bind( "<Control-l>", self.toggle_ln)
 			self.contents.bind( "<Control-x>", self.toggle_syntax)
@@ -754,14 +781,20 @@
 			self.contents.bind( "<dagger>", self.toggle_color)		# Alt-t
 			self.contents.bind( "<ssharp>", self.color_choose)		# Alt-s
 			
 			
 		#######################################################
 		
 		
+		# Arrange detection of CapsLock-state.
+		self.capslock = 'init'
+		self.motion_bind = self.bind('<Motion>', self.check_caps)
+		self.bind('<KeyRelease-Caps_Lock>', self.check_caps)
+		self.bind('<KeyPress-Caps_Lock>', self.check_caps)
+		
 		self.bind( "<Control-R>", self.replace_all)
 		self.bind( "<Control-g>", self.gotoline)
 		self.bind( "<Control-r>", self.replace)
 
 		self.bind( "<Escape>", self.do_nothing )
 		self.bind( "<Return>", self.do_nothing)
 		self.bind( "<Control-minus>", self.decrease_scrollbar_width)
@@ -775,41 +808,47 @@
 		
 		self.contents.bind( "<Control-a>", self.goto_linestart)
 		self.contents.bind( "<Control-e>", self.goto_lineend)
 		self.contents.bind( "<Control-A>", self.goto_linestart)
 		self.contents.bind( "<Control-E>", self.goto_lineend)
 		
 		if self.os_type == 'windows':
-			self.entry.bind( "<Control-E>", lambda event, arg=('<<SelectLineEnd>>'): self.entry.event_generate)
-			self.entry.bind( "<Control-A>", lambda event, arg=('<<SelectLineStart>>'): self.entry.event_generate)
-		
-		self.contents.bind( "<Control-i>", self.move_right)
-		self.contents.bind( "<Control-b>", self.move_left)
-		self.contents.bind( "<Control-n>", self.move_down)
-		self.contents.bind( "<Control-p>", self.move_up)
-		
+			self.entry.bind( "<Control-E>",
+				lambda event, arg=('<<SelectLineEnd>>'): self.entry.event_generate)
+			self.entry.bind( "<Control-A>",
+				lambda event, arg=('<<SelectLineStart>>'): self.entry.event_generate)
+			
+			self.entry.bind( "<Control-c>", self.copy_windows)
+			self.entry.bind( "<Control-x>",
+				lambda event: self.copy_windows(event, **{'flag_cut':True}) )
+			
+			
 		self.contents.bind( "<Control-j>", self.center_view)
-		self.contents.bind( "<Control-u>", lambda event: self.center_view(event, **{'up':True}) )
-		
-		self.contents.bind( "<Return>", self.return_override)
+		self.contents.bind( "<Control-u>",
+			lambda event: self.center_view(event, **{'up':True}) )
 		
 		self.contents.bind( "<Control-d>", self.del_tab)
-		self.contents.bind( "<Control-Q>", lambda event: self.del_tab(event, **{'save':False}) )
+		self.contents.bind( "<Control-Q>",
+			lambda event: self.del_tab(event, **{'save':False}) )
 		
 		self.contents.bind( "<Shift-Return>", self.comment)
 		self.contents.bind( "<Shift-BackSpace>", self.uncomment)
 		self.contents.bind( "<Tab>", self.tab_override)
+		self.contents.bind( "<Control-Tab>", self.insert_tab)
 		
 		self.contents.bind( "<Control-t>", self.tabify_lines)
 		self.contents.bind( "<Control-z>", self.undo_override)
 		self.contents.bind( "<Control-Z>", self.redo_override)
 		self.contents.bind( "<Control-f>", self.search)
 		
+		self.contents.bind( "<Return>", self.return_override)
 		self.contents.bind( "<BackSpace>", self.backspace_override)
 		self.contents.bind( "<Control-BackSpace>", self.search_next)
+		self.contents.bind( "<Control-Shift-BackSpace>",
+				lambda event: self.search_next(event, **{'back':True}) )
 		
 		
 ##		# this move_line interferes with search_next,check_nextevent, so not in use
 ##		self.contents.bind("<Left>", lambda event: self.move_line(event, **{'direction':'left'} ))
 ##		self.contents.bind("<Right>", lambda event: self.move_line(event, **{'direction':'right'} ))
 ##
 ##		# updown_override not in use
@@ -883,14 +922,16 @@
 		
 		self.contents.tag_config('keywords', font=self.boldfont)
 		self.contents.tag_config('numbers', font=self.boldfont)
 		self.contents.tag_config('comments', font=self.boldfont)
 		self.contents.tag_config('breaks', font=self.boldfont)
 		self.contents.tag_config('calls', font=self.boldfont)
 
+		self.contents.tag_config('focus', underline=True)
+
 		# search tags have highest priority
 		self.contents.tag_raise('match')
 		self.contents.tag_raise('replaced')
 		self.contents.tag_raise('sel')
 		self.contents.tag_raise('focus')
 		
 		
@@ -984,35 +1025,47 @@
 				self.fullscreen = False
 				
 		
 		self.text_widget_height = self.scrollbar.winfo_height()
 		self.update_linenums()
 		
 	
-	def copy_windows(self, event=None):
-		
+	def copy_windows(self, event=None, selection=None, flag_cut=False):
 		
 		try:
 			#self.clipboard_clear()
-			tmp = self.selection_get()
+			# From copy():
+			if selection:
+				tmp = selection
+			else:
+				tmp = self.selection_get()
+			
+			
+			if flag_cut:
+				w = self.contents
+				
+				# Event should only come when in entry
+				if event:
+					w = event.widget
+					
+				w.delete(tkinter.SEL_FIRST, tkinter.SEL_LAST)
 			
 			
 			# https://stackoverflow.com/questions/51921386
 			# pyperclip approach works in windows fine
 			# import clipboard as cb
 			# cb.copy(tmp)
 			
 			# os.system approach also works but freezes editor for a little time
 			
 			
 			d = dict()
 			d['input'] = tmp.encode('ascii')
 			
 			t = threading.Thread( target=subprocess.run, args=('clip',), kwargs=d, daemon=True )
-			#t.setDeamon(True)
 			t.start()
 			
 				
 			#self.clipboard_append(tmp)
 		except tkinter.TclError:
 			# is empty
 			return 'break'
@@ -1044,17 +1097,87 @@
 		return 'break'
 		
 	
 	def do_nothing_without_bell(self, event=None):
 		return 'break'
 	
 	
+	def check_caps(self, event=None):
+		'''	Check if CapsLock is on.
+		'''
+		e = event.state
+		
+		if e in [0, 2]:
+			
+			# CapsLock is being turned off
+			if e == 0 and self.capslock in [True, 'init']:
+				self.capslock = False
+				
+				# If quickly pressed CapsLock off,
+				# cancel flashing started at the end of this callback.
+				for i in range(len(self.to_be_cancelled)-1, -1, -1):
+					item = self.to_be_cancelled[i]
+					self.after_cancel(item)
+					self.to_be_cancelled.pop(i)
+					
+					
+				# Put Git-branch name back if on one
+				if self.branch:
+					branch = self.branch[:5]
+					# Set branch name lenght to 5.
+					# Reason: avoid ln_widget geometry changes
+					# when showing capslock-state in btn_git.
+					if len(branch) < 5:
+						diff = 5-len(branch)
+						t=1
+						for i in range(diff):
+							if t > 0:
+								branch += ' '
+							else:
+								branch = ' ' + branch
+
+							t *= -1
+				
+					self.btn_git.config(text=branch, disabledforeground='')
+		
+					if 'main' in self.branch or 'master' in self.branch:
+						self.btn_git.config(disabledforeground='brown1')
+		
+				else:
+					self.btn_git.config(bitmap='info')
+				
+				
+			# CapsLock is being turned on
+			elif e == 2 and self.capslock in [False, 'init']:
+				self.capslock = True
+				
+				self.btn_git.config(text="CAPS ", disabledforeground='brown1')
+					
+				# Flash text and enable canceling flashing later.
+				#
+				# For two times, i=1,2:
+				#	wait 300
+				# 	change btn_git text to spaces
+				# 	again wait 300
+				# 	change btn_git text to CAPS
+				for i in range(1,3):
+					self.to_be_cancelled.append(
+						self.after((2*i-1)*300, lambda kwargs={'text': 5*' '}:
+							self.btn_git.config(**kwargs) )
+					)
+					
+					self.to_be_cancelled.append(
+						self.after(2*i*300, lambda kwargs={'text': 'CAPS '}:
+							self.btn_git.config(**kwargs) )
+					)
+					
+		
 	def test_bind(self, event=None):
 		print('jou')
-	
+		
 	
 	def skip_bindlevel(self, event=None):
 		return 'continue'
 		
 	
 	def ensure_idx_visibility(self, index, back=None):
 		b=2
@@ -1078,15 +1201,15 @@
 		
 		
 	def quit_me(self, event=None):
 	
 		self.save(forced=True)
 		self.save_config()
 		
-		# affects color, fontchoose, load:
+		# Affects color, fontchoose, load:
 		for widget in self.to_be_closed:
 			widget.destroy()
 		
 		self.quit()
 		self.destroy()
 		
 		
@@ -1095,15 +1218,14 @@
 		
 			# This osascript-language is funny
 			# https://ss64.com/osx/osascript.html
 			
 			mac_term = 'Terminal'
 			
 			
-			
 			try:
 				# Giving focus back to python terminal-window is not very simple task in macOS
 				# https://apple.stackexchange.com/questions/421137
 				tmp = None
 				if self.__class__.mac_term and self.__class__.win_id:
 					mac_term = self.__class__.mac_term
 					win_id  = self.__class__.win_id
@@ -1112,16 +1234,14 @@
 					if mac_term == 'iTerm2':
 						tmp = [ 'osascript', '-e', 'tell app "%s" to select windows whose id = %s' % (mac_term, win_id), '-e', 'tell app "%s" to activate' % mac_term ]
 						
 					else:
 						tmp = [ 'osascript', '-e', 'tell app "%s" to set frontmost of windows whose id = %s to true' % (mac_term, win_id), '-e', 'tell app "%s" to activate' % mac_term ]
 
 
-
-
 				elif self.__class__.mac_term:
 					mac_term = self.__class__.mac_term
 					tmp = ['osascript', '-e', 'tell app "%s" to activate' % mac_term ]
 
 				else:
 					tmp = ['osascript', '-e', 'tell app "%s" to activate' % mac_term ]
 
@@ -1139,15 +1259,15 @@
 		if self.tracefunc_name:
 			self.tracevar_filename.trace_remove('write', self.tracefunc_name)
 		
 		del self.font
 		del self.menufont
 		del self.boldfont
 		
-		# this is maybe not necessary
+		# This is maybe not necessary
 		del self.entry
 		del self.btn_open
 		del self.btn_save
 		del self.btn_git
 		del self.contents
 		del self.ln_widget
 		del self.scrollbar
@@ -1339,20 +1459,22 @@
 					self.goto_lineend(event=event)
 					
 				elif event.keysym == 'Left':
 					self.goto_linestart(event=event)
 					
 				elif event.keysym == 'Up':
 					for i in range(10):
-						self.contents.event_generate('<<SelectPrevLine>>')
-				
+						self.after(12, lambda args=['<<SelectPrevLine>>']:
+							self.contents.event_generate(*args) )
+						
 				elif event.keysym == 'Down':
 					for i in range(10):
-						self.contents.event_generate('<<SelectNextLine>>')
-					
+						self.after(12, lambda args=['<<SelectNextLine>>']:
+							self.contents.event_generate(*args) )
+						
 				else:
 					return
 			
 			return 'break'
 		
 		
 		# Pressed Cmd + arrow left or right.
@@ -1961,14 +2083,15 @@
 		
 			# check if inside multiline string
 			elif 'strings' in self.contents.tag_names(tkinter.INSERT) and \
 					not ( start_idx == '1.0' and end_idx == tkinter.END ):
 				
 				try:
 					s, e = self.contents.tag_prevrange('strings', tkinter.INSERT)
+					# Clarify this:################################################
 					l0, l1 = map( lambda x: int( x.split('.')[0] ), [s, e] )
 				
 					if l0 != l1:
 						start_idx, end_idx = (s, e)
 						linecontents = None
 		
 				except ValueError:
@@ -2414,54 +2537,50 @@
 			big = True
 			shortcut = "<function>"
 		
 		
 		fonttop.protocol("WM_DELETE_WINDOW", lambda: ( fonttop.destroy(),
 				self.contents.bind( shortcut, self.font_choose)) )
 		
-		changefont.FontChooser( fonttop, [self.font, self.menufont], big, tracefunc=self.update_fonts, os_type=self.os_type )
+		changefont.FontChooser( fonttop, [self.font, self.menufont], big,
+			tracefunc=self.update_fonts, os_type=self.os_type )
 		self.contents.bind( shortcut, self.do_nothing)
 		self.to_be_closed.append(fonttop)
 	
 		return 'break'
 		
 		
 	def enter2(self, args, event=None):
 		''' When mousecursor enters hyperlink tagname in colorchooser.
 		'''
 		wid = args[0]
 		tagname = args[1]
 		
 		t = wid.textwid
 		
-##		wid.after(200, lambda kwargs={'cursor':'hand2'}: t.config(**kwargs) )
-##
-		
-		
+		# Maybe left as lambda-example?
+		#wid.after(200, lambda kwargs={'cursor':'hand2'}: t.config(**kwargs) )
+
 		t.config(cursor="hand2")
 		wid.after(50, lambda args=[tagname],
 				kwargs={'underline':1, 'font':self.boldfont}: t.tag_config(*args, **kwargs) )
 		
-		#t.tag_config(tagname, underline=1, font=self.boldfont)
-		
 		
 	def leave2(self, args, event=None):
 		''' When mousecursor leaves hyperlink tagname in colorchooser.
 		'''
 		wid = args[0]
 		tagname = args[1]
 		
 		t = wid.textwid
 		
 		t.config(cursor=self.name_of_cursor_in_text_widget)
 		wid.after(50, lambda args=[tagname],
 				kwargs={'underline':0, 'font':self.menufont}: t.tag_config(*args, **kwargs) )
 		
-		#t.tag_config(tagname, underline=0, font=self.menufont)
-		
 		
 	def lclick2(self, args, event=None):
 		'''	When clicked hyperlink in colorchooser.
 		'''
 		wid = args[0]
 		tagname = args[1]
 		
@@ -2947,15 +3066,16 @@
 		self.contents.mark_set('insert', line)
 		self.ensure_idx_visibility(line)
 					
 		
 		self.contents.edit_reset()
 		self.contents.edit_modified(0)
 		
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num,
+			lambda event: self.raise_popup(event))
 		self.state = 'normal'
 		self.update_title()
 		
 
 	def run(self):
 		'''	Run file currently being edited. This can not catch errlines of
 			those exceptions that are catched. Like:
@@ -3133,15 +3253,16 @@
 						self.update_tokens(start=start, end=end, line=line)
 			
 					
 									
 	def stop_show_errors(self, event=None):
 		self.state = 'normal'
 		self.bind("<Escape>", self.do_nothing)
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num,
+			lambda event: self.raise_popup(event))
 		
 		self.entry.delete(0, tkinter.END)
 		
 		if self.tabs[self.tabindex].type == 'normal':
 			self.entry.insert(0, self.tabs[self.tabindex].filepath)
 			self.entry.xview_moveto(1.0)
 			
@@ -3163,70 +3284,15 @@
 		self.contents.edit_reset()
 		self.contents.edit_modified(0)
 		
 		
 ########## Run file Related End
 ########## Select and move Begin
 
-	def move_right(self, event=None):
-		''' move cursor right with
-			ctrl-i
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		self.contents.event_generate('<<NextChar>>')
-		
-		return "break"
-		
-		
-	def move_left(self, event=None):
-		''' move cursor left with
-			ctrl-b
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		self.contents.event_generate('<<PrevChar>>')
-		
-		return "break"
-		
-		
-	def move_up(self, event=None):
-		''' move cursor up with
-			ctrl-p
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-			
-		self.contents.event_generate('<<PrevLine>>')
-		
-		return "break"
-		
-		
-	def move_down(self, event=None):
-		''' move cursor down with
-			ctrl-n
-		'''
-		
-		if self.state not in  [ 'normal', 'error' ]:
-			self.bell()
-			return "break"
-	
-		self.contents.event_generate('<<NextLine>>')
-		
-		return "break"
-	
-	
+
 ##	def updown_override(self, event=None, direction=None):
 ##		''' up-down override, to expand possibly incorrect indentation
 ##		'''
 ##
 ##		if self.state != 'normal':
 ##			return "continue"
 ##
@@ -3301,26 +3367,36 @@
 		if event.keysym == 'Up':
 			e = '<<SelectPrevLine>>'
 			
 			if event.state not in [ 5, 262157, 262149 ]:
 				e = '<<PrevLine>>'
 			
 			for i in range(10):
-				self.contents.event_generate(e)
+				# Add some delay
+				if 'Select' in e:
+					self.after(12, lambda args=[e]:
+						self.contents.event_generate(*args) )
+				else:
+					self.contents.event_generate(e)
 				
 			return 'break'
 		
 		elif event.keysym == 'Down':
 			e = '<<SelectNextLine>>'
 			
 			if event.state not in [ 5, 262157, 262149 ]:
 				e = '<<NextLine>>'
 			
 			for i in range(10):
-				self.contents.event_generate(e)
+				# Add some delay
+				if 'Select' in e:
+					self.after(12, lambda args=[e]:
+						self.contents.event_generate(*args) )
+				else:
+					self.contents.event_generate(e)
 			
 			return 'break'
 		
 		else:
 			return
 			
 			
@@ -3371,42 +3447,59 @@
 ##		Adjust the index to refer to the last index on the line (the newline). If the display submodifier is given, this is the last index on the display line, otherwise on the logical line.
 
 		pos = self.contents.index( 'insert display lineend' )
 		return pos
 		
 			
 	def idx_linestart(self):
+		'''	Returns tuple:
+			
+			pos, line_is_wrapped
+		
+			Where pos is tkinter.Text -index of linestart:
+			
+			if line is wrapped:
+				pos = start of display-line
+			else:
+				pos = end of indentation if there is such.
+				
+			If line is empty, pos = None
+			
+			Wrapped line definition:
+			Line that has not started on (display-) line with cursor
+		'''
 		
 		# In case of wrapped lines
 		y_cursor = self.contents.bbox(tkinter.INSERT)[1]
 		p = self.contents.index( '@0,%s' % y_cursor )
 		p2 = self.contents.index( '%s linestart' % p )
+		line_is_wrapped = False
 		
-		# is wrapped?
+		# Is line wrapped?
 		c1 = int(p.split('.')[1])
 		l2 = int(p2.split('.')[0])
 		
-		pos = None
-		# yes, put cursor start of line not the whole line:
+		pos = False
+		# Yes, put cursor start of (display-) line, not the whole (=logical) line:
 		if c1 != 0:
 			pos = p
+			line_is_wrapped = True
 			
-		# no, so put cursor after indentation:
+		# No, put cursor after indentation:
 		else:
 			tmp = self.contents.get( '%s linestart' % p2, '%s lineend' % p2 )
 			if len(tmp) > 0:
 				if not tmp.isspace():
 					tmp2 = tmp.lstrip()
 					indent = tmp.index(tmp2)
 					pos = self.contents.index( '%i.%i' % (l2, indent) )
 		
-		return pos
+		return pos, line_is_wrapped
 		
 	
-
 	def select_by_words(self, event=None):
 		'''	Pressed ctrl or Alt + shift and arrow left or right.
 			Make <<SelectNextWord>> and <<SelectPrevWord>> to stop at lineends.
 		'''
 		if self.state not in [ 'normal', 'error', 'search', 'replace', 'replace_all' ]:
 			self.bell()
 			return "break"
@@ -3433,20 +3526,14 @@
 		
 		
 		have_selection = len(self.contents.tag_ranges('sel')) > 0
 		selection_started_from_top = False
 		
 		if event.keysym == 'Right':
 			s = self.contents.index( 'insert')
-			e = self.idx_lineend()
-			idx_linestart = self.idx_linestart()
-			# empty line?
-			if not idx_linestart: return
-			t = self.contents.get(idx_linestart, e).strip()
-
 			
 			# tkinter.SEL_FIRST is always before tkinter.SEL_LAST
 			# no matter if selection started from top or bottom:
 			if have_selection:
 				sel_start = self.contents.index(tkinter.SEL_FIRST)
 				sel_end = self.contents.index(tkinter.SEL_LAST)
 				if s == sel_end:
@@ -3459,89 +3546,47 @@
 				sel_start = s
 
 			
 			
 			##################### Right Real start:
 			
 			
-			self.contents.event_generate('<<NextWord>>')
-			i = self.contents.index( 'insert')
-
-			# Already at lineend, proceed to next line
-			if s == e:
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.mark_set(self.anchorname, sel_start)
-						self.contents.tag_add('sel', sel_start, i)
-					else:
-						self.contents.mark_set(self.anchorname, sel_end)
-						self.contents.tag_add('sel', i, sel_end)
-						
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.mark_set(self.anchorname, s)
-					self.contents.tag_add('sel', s, i)
-					
-				self.contents.mark_set('insert', i)
-
+			pos = self.move_by_words_right()
 			
-			# if i is over lineend:
-			# 	stop at lineend == e
-			elif self.contents.compare( e,'<',i ):
-				
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
+			
+			if have_selection:
+				self.contents.tag_remove('sel', '1.0', tkinter.END)
 
-					if selection_started_from_top:
-						self.contents.mark_set(self.anchorname, sel_start)
-						self.contents.tag_add('sel', sel_start, e)
-					else:
-						self.contents.mark_set(self.anchorname, sel_end)
-						self.contents.tag_add('sel', e, sel_end)
-						
-				# No selection,
-				# no need to check direction of selection:
+				if selection_started_from_top:
+					self.contents.mark_set(self.anchorname, sel_start)
+					self.contents.tag_add('sel', sel_start, pos)
+					
 				else:
-					self.contents.mark_set(self.anchorname, s)
-					self.contents.tag_add('sel', s, e)
+					# Check if selection is about to be closed
+					# (selecting towards selection-start)
+					# to avoid one char selection -leftovers.
+					if self.contents.compare( '%s +1 chars' % pos, '>=' , sel_end ):
+						
+						self.contents.mark_set('insert', sel_end)
+						self.contents.mark_set(self.anchorname, sel_end)
+						return 'break'
 					
-				self.contents.mark_set('insert', e)
+					self.contents.mark_set(self.anchorname, sel_end)
+					self.contents.tag_add('sel', pos, sel_end)
 
-
-			# i is on the current line:
-			# 	stop at i == nextword
+			# No selection,
+			# no need to check direction of selection:
 			else:
-				
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
+				self.contents.mark_set(self.anchorname, s)
+				self.contents.tag_add('sel', s, pos)
+
 
-					if selection_started_from_top:
-						self.contents.mark_set(self.anchorname, sel_start)
-						self.contents.tag_add('sel', sel_start, i)
-						
-					else:
-						self.contents.mark_set(self.anchorname, sel_end)
-						self.contents.tag_add('sel', i, sel_end)
-						
-						
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.mark_set(self.anchorname, s)
-					self.contents.tag_add('sel', s, i)
-					
-					
-				self.contents.mark_set('insert', i)
-				
-				
 
 		elif event.keysym == 'Left':
+				
 			s = self.contents.index( 'insert')
 			
 			# tkinter.SEL_FIRST is always before tkinter.SEL_LAST
 			# no matter if selection started from top or bottom:
 			if have_selection:
 				sel_start = self.contents.index(tkinter.SEL_FIRST)
 				sel_end = self.contents.index(tkinter.SEL_LAST)
@@ -3551,162 +3596,266 @@
 				#else: selection_started_from_top = False
 
 			else:
 				#selection_started_from_top = False
 				sel_end = s
 
 
-			i_orig = s
-			i_linestart = self.idx_linestart()
-			# empty line?
-			if not i_linestart: return
-			
-			
 			
 			##################### Left Real start:
 			
 			
-			self.contents.event_generate('<<PrevWord>>')
-			i_prevword = self.contents.index( 'insert')
+			pos = self.move_by_words_left()
 			
-
-			# Already at linestart, proceed over last word of prev line.
-			if i_orig == i_linestart:
-
-				if have_selection:
-					
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
-
-					if selection_started_from_top:
-						self.contents.mark_set(self.anchorname, sel_start)
-						self.contents.tag_add('sel', sel_start, i_prevword)
-					else:
-						self.contents.mark_set(self.anchorname, sel_end)
-						self.contents.tag_add('sel', i_prevword, sel_end)
-						
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.mark_set(self.anchorname, s)
-					self.contents.tag_add('sel', i_prevword, s)
-					
-				self.contents.mark_set('insert', i_prevword)
-
 			
-			# if i_prevword is over(before) linestart:
-			# 	stop at linestart == i_linestart
-			elif self.contents.compare( i_prevword, '<', i_linestart):
-
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
+			if have_selection:
+				
+				self.contents.tag_remove('sel', '1.0', tkinter.END)
 
-					if selection_started_from_top:
+				if selection_started_from_top:
+					# Check if selection is about to be closed
+					# (selecting towards selection-start)
+					# to avoid one char selection -leftovers.
+					if self.contents.compare( '%s -1 chars' % pos, '<=' , sel_start ):
+						
+						self.contents.mark_set('insert', sel_start)
 						self.contents.mark_set(self.anchorname, sel_start)
-						self.contents.tag_add('sel', sel_start, i_linestart)
-					else:
-						self.contents.mark_set(self.anchorname, sel_end)
-						self.contents.tag_add('sel', i_linestart, sel_end)
-								
-				# No selection,
-				# no need to check direction of selection:
+						return 'break'
+					
+					self.contents.mark_set(self.anchorname, sel_start)
+					self.contents.tag_add('sel', sel_start, pos)
+				
 				else:
-					self.contents.mark_set(self.anchorname, s)
-					self.contents.tag_add('sel', i_linestart, s)
-
-				self.contents.mark_set('insert', i_linestart)
-
-
-			# i_prevword is on the current line:
-			# 	stop at i_prevword
+					self.contents.mark_set(self.anchorname, sel_end)
+					self.contents.tag_add('sel', pos, sel_end)
+				
+								
+			# No selection,
+			# no need to check direction of selection:
 			else:
-				if have_selection:
-					self.contents.tag_remove('sel', '1.0', tkinter.END)
+				self.contents.mark_set(self.anchorname, s)
+				self.contents.tag_add('sel', pos, s)
+			
+			
+		return 'break'
+	
+	
+	def move_by_words_left(self):
+		''' Returns tkinter.Text -index: pos
+			and moves cursor to it.
+		'''
+		
+		idx_linestart, line_is_wrapped = self.idx_linestart()
+		i_orig = self.contents.index('insert')
+		
+		# Empty line
+		if not idx_linestart:
+			# Go over empty space first
+			self.contents.event_generate('<<PrevWord>>')
+			
+			# And put cursor to line end
+			i_new = self.idx_lineend()
+			self.contents.mark_set('insert', i_new)
+		
 
-					if selection_started_from_top:
-						self.contents.mark_set(self.anchorname, sel_start)
-						self.contents.tag_add('sel', sel_start, i_prevword)
-					else:
-						self.contents.mark_set(self.anchorname, sel_end)
-						self.contents.tag_add('sel', i_prevword, sel_end)
-								
-				# No selection,
-				# no need to check direction of selection:
-				else:
-					self.contents.mark_set(self.anchorname, s)
-					self.contents.tag_add('sel', i_prevword, s)
+		# Is cursor on such line that has not started on that (display-) line?
+		elif line_is_wrapped:
+			
+			# At indent0, put cursor to line end of previous line
+			if self.contents.compare('insert', '==', idx_linestart):
+				self.contents.event_generate('<<PrevWord>>')
+				self.contents.mark_set('insert', 'insert display lineend')
+				
+			# Not at indent0, just check cursor not go over indent0
+			else:
+				self.contents.event_generate('<<PrevWord>>')
+				if self.contents.compare('insert', '<', idx_linestart):
+					self.contents.mark_set('insert', idx_linestart)
+			
+			
+		# Below this line is non empty and not wrapped
+		############
+		# Most common scenario:
+		# Is cursor after idx_linestart?
+		# i_orig > idx_linestart
+		elif self.contents.compare( i_orig, '>', idx_linestart ):
+			self.contents.event_generate('<<PrevWord>>')
+			
+			# Check that cursor did not go over idx_linestart
+			i_new = self.contents.index(tkinter.INSERT)
+			if self.contents.compare( i_new, '<', idx_linestart):
+				self.contents.mark_set('insert', idx_linestart)
+		
+		
+		## Below this i_orig <= idx_linestart
+		############
+		# At idx_linestart
+		elif i_orig == idx_linestart:
+			
+			# No indentation?
+			if int(idx_linestart.split('.')[1]) == 0:
+				# At filestart?
+				if self.contents.compare( i_orig, '==', '1.0'):
+					pos = i_orig
+					return pos
+					
+				# Go over empty space first
+				self.contents.event_generate('<<PrevWord>>')
+				
+				# And put cursor to line end
+				i_new = self.idx_lineend()
+				self.contents.mark_set('insert', i_new)
+			
+			# Cursor is at idx_linestart (end of indentation)
+			# of line that has indentation.
+			else:
+				# Put cursor at indent0 (start of indentation)
+				self.contents.mark_set('insert', 'insert linestart')
+		
+		
+		# Below this only lines that has indentation
+		############
+		# 1: Cursor is not after idx_linestart
+		#
+		# 2: Nor at idx_linestart == end of indentation, if line has indentation
+		# 							start of line, (indent0), if line has no indentation
+		#
+		# --> Cursor is in indentation
+		
+		# At indent0 of line that has indentation
+		elif int(i_orig.split('.')[1]) == 0:
+			# At filestart?
+			if self.contents.compare( i_orig, '==', '1.0'):
+				pos = i_orig
+				return pos
+			
+			# Go over empty space first
+			self.contents.event_generate('<<PrevWord>>')
+			
+			# And put cursor to line end
+			i_new = self.idx_lineend()
+			self.contents.mark_set('insert', i_new)
+		
+		else:
+			# Put cursor at indent0
+			self.contents.mark_set('insert', 'insert linestart')
+			
+		
+		pos = self.contents.index('insert')
+		return pos
+	
+	
+	def move_by_words_right(self):
+		''' Returns tkinter.Text -index: pos
+			and moves cursor to it.
+		'''
+		
+		# Get some basic indexes first
+		idx_linestart, line_is_wrapped = self.idx_linestart()
+		i_orig = self.contents.index('insert')
+		
+		# Get idx_lineend (of non empty line)
+		if idx_linestart:
+			e = self.idx_lineend()
+		
+		# Empty line
+		if not idx_linestart:
+			# Go over empty space first
+			self.contents.event_generate('<<NextWord>>')
+			
+			# And put cursor to idx_linestart
+			i_new, line_is_wrapped = self.idx_linestart()
+			
+			# Check not at fileend, if not then proceed
+			if i_new:
+				self.contents.mark_set('insert', i_new)
+				
+		
+		# Below this line is non empty
+		##################
+		# Cursor is at lineend, goto idx_linestart of next non empty line
+		elif i_orig == e:
+		
+			# Check if at fileend
+			if self.contents.compare('%s +1 chars' % i_orig, '==', tkinter.END):
+				pos = i_orig
+				return pos
+			
+			self.contents.event_generate('<<NextWord>>')
+			idx_linestart, line_is_wrapped = self.idx_linestart()
+			
+			if idx_linestart:
+				self.contents.mark_set('insert', idx_linestart)
 
-				self.contents.mark_set('insert', i_prevword)
+		
+		# Below this line cursor is before line end
+		############
+		# Most common scenario
+		# Cursor is at or after idx_linestart
+		# idx_lineend > i_orig >= idx_linestart
+		elif self.contents.compare(i_orig, '>=', idx_linestart):
 
+			self.contents.event_generate('<<NextWord>>')
+			
+			# Check not over lineend
+			if self.contents.compare('insert', '>', e):
+				self.contents.mark_set('insert', e)
+		
+		
+		############
+		# Below this line has indentation and is not wrapped
+		# Cursor is at
+		# indent0 <= i_orig < idx_linestart
+		
+		# --> put cursor to idx_linestart
+		############
+		else:
+			self.contents.mark_set('insert', idx_linestart)
+			
+		
+		pos = self.contents.index('insert')
+		return pos
 
-		return 'break'
-	
-	
+		
 	def move_by_words(self, event=None):
 		'''	Pressed ctrl or Alt and arrow left or right.
-			Make <<NextWord>> and <<PrevWord>> to stop at lineends.
+			Make <<NextWord>> and <<PrevWord>> to handle lineends.
 		'''
 		if self.state not in [ 'normal', 'error', 'search', 'replace', 'replace_all' ]:
 			self.bell()
 			return "break"
 			
-		idx_linestart = self.idx_linestart()
-		# empty line?
-		if not idx_linestart: return
-		
-		
 		# Check if: not only ctrl down, then return
 		# MacOS event is already checked.
 		if self.os_type == 'linux':
 			if event.state != 4: return
 		
 		elif self.os_type == 'windows':
 			if event.state not in [ 262156, 262148 ]: return
 			
 		
-		# Check if near lineend, so stop there
 		if event.keysym == 'Right':
-			i_orig = self.contents.index( 'insert')
-			e = self.idx_lineend()
-			# Already at lineend, proceed over first word of next line
-			if i_orig == e: return
+			pos = self.move_by_words_right()
 			
-			self.contents.event_generate('<<NextWord>>')
-			i = self.contents.index( 'insert')
-			if self.contents.compare( e, '<', i ):
-				self.contents.mark_set('insert', e)
-				
-				
-		# Check if near linestart, so stop there
 		elif event.keysym == 'Left':
-			i_orig = self.contents.index( 'insert')
-			self.contents.event_generate('<<PrevWord>>')
-			i_prevword = self.contents.index( 'insert')
+			pos = self.move_by_words_left()
 			
-			self.contents.mark_set('insert', i_orig)
-			self.goto_linestart(event=event)
-			i_linestart = self.contents.index( 'insert')
-			
-			# Already at linestart, proceed over last word of prev line
-			if i_orig == i_linestart: return
-			
-			if self.contents.compare( i_prevword, '<', i_linestart ):
-				self.contents.mark_set('insert', i_linestart)
-			else:
-				self.contents.mark_set('insert', i_prevword)
+		else:
+			return
+				
 				
-
 		return 'break'
 	
 		
 	def check_sel(self, event=None):
 		'''	Pressed arrow left or right.
 			If have selection, put cursor on the wanted side of selection.
 		'''
 		
-		if self.state in  [ 'filedialog' ]:
+		if self.state in [ 'filedialog' ]:
 			self.bell()
 			return "break"
 	
 		
 		# self.contents or self.entry
 		wid = event.widget
 			
@@ -3806,18 +3955,19 @@
 			
 			self.contents.tag_remove('sel', '1.0', tkinter.END)
 			self.contents.tag_add('sel', s, e)
 		
 			if self.os_type != 'windows':
 				self.contents.clipboard_append(tmp)
 			else:
-				self.copy_windows(event=event)
+				self.copy_windows(selection=tmp)
+			
+			self.after(600, lambda args=['sel', '1.0', tkinter.END]:
+					self.contents.tag_remove(*args) )
 			
-			self.after(600, lambda args=['sel', '1.0', tkinter.END]: self.contents.tag_remove(*args) )
-		
 			
 		return 'break'
 		
 		
 	def goto_lineend(self, event=None):
 		if self.state in [ 'filedialog' ]:
 			self.bell()
@@ -3829,15 +3979,15 @@
 			wid.selection_clear()
 			idx = tkinter.END
 			wid.icursor(idx)
 			wid.xview_moveto(1.0)
 			return 'break'
 		
 		
-		idx_linestart = self.idx_linestart()
+		idx_linestart, line_is_wrapped = self.idx_linestart()
 		# Empty line?
 		if not idx_linestart: return "break"
 		
 		
 		have_selection = False
 		want_selection = False
 		
@@ -3927,15 +4077,15 @@
 				idx = tmp.index(':') + 2
 			
 			wid.icursor(idx)
 			wid.xview_moveto(0)
 			return 'break'
 			
 		
-		idx_linestart = self.idx_linestart()
+		idx_linestart, line_is_wrapped = self.idx_linestart()
 		# Empty line?
 		if not idx_linestart: return "break"
 		
 		
 		have_selection = False
 		want_selection = False
 		
@@ -3980,15 +4130,15 @@
 		# Dont want selection, ctrl/cmd-a/e:
 		else:
 			self.contents.tag_remove('sel', '1.0', tkinter.END)
 			
 		
 		self.ensure_idx_visibility('insert')
 		
-		pos = self.idx_linestart()
+		pos, line_is_wrapped = self.idx_linestart()
 		
 		self.contents.see(pos)
 		self.contents.mark_set('insert', pos)
 	
 		if want_selection:
 			
 			if have_selection:
@@ -4022,28 +4172,383 @@
 		self.popup.focus_set() # Needed to remove popup when clicked outside.
 		
 		
 	def popup_focusOut(self, event=None):
 		self.popup.unpost()
 	
 	
-	def copy(self):
-		''' When copy is selected from popup-menu
-		'''
+	def copy_fallback(self, selection=None, flag_cut=False):
+		
 		if self.os_type == 'windows':
-			self.copy_windows()
+			self.copy_windows(selection=selection, flag_cut=flag_cut)
 		
 		else:
 			try:
 				self.clipboard_clear()
 				self.clipboard_append(self.selection_get())
+				if flag_cut:
+					self.contents.delete(tkinter.SEL_FIRST, tkinter.SEL_LAST)
+				
 			except tkinter.TclError:
 				# is empty
+				pass
+		
+		return 'break'
+		
+	
+	def copy(self, event=None, flag_cut=False):
+		''' When selection started from start of block,
+				for example: cursor is before if-word,
+			and
+				selected at least one whole line below firsline
+				
+			Then
+				preserve indentation
+				of all lines in selection.
+				
+			This is done in paste()
+			if self.flag_fix_indent is True.
+			If not, paste_fallback() is used instead.
+		'''
+		self.indent_selstart = 0
+		self.indent_nextline = 0
+		self.indent_diff = 0
+		self.flag_fix_indent = False
+		self.checksum_fix_indent = False
+
+				
+		# Check if have_selection
+		have_selection = len(self.contents.tag_ranges('sel')) > 0
+		if not have_selection:
+			#print('copy fail 1, no selection')
+			return 'break'
+
+		
+		t_orig = self.contents.selection_get()
+		
+		
+		# Check if num selection lines > 1
+		startline, startcol = map(int, self.contents.index(tkinter.SEL_FIRST).split(sep='.'))
+		endline = int(self.contents.index(tkinter.SEL_LAST).split(sep='.')[0])
+		numlines = endline - startline
+		if not numlines > 1:
+			#print('copy fail 2, numlines not > 1')
+			return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+			
+
+		# Selection start indexes:
+		line, col = startline, startcol
+
+		self.indent_selstart = col
+
+		
+		# Check if selstart line not empty
+		tmp = self.contents.get('%s.0' % str(line),'%s.0 lineend' % str(line))
+		if len(tmp.strip()) == 0:
+			#print('copy fail 4, startline empty')
+			return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+		
+		# Check if cursor not at idx_linestart
+		for i in range(len(tmp)):
+			if not tmp[i].isspace():
+				break
+		
+		if i > self.indent_selstart:
+			# Cursor is inside indentation or indent0
+			#print('copy fail 3, Cursor in indentation')
+			return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+			
+		elif i < self.indent_selstart:
+			#print('copy fail 3, SEL_FIRST after idx_linestart')
+			return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+		
+		# Check if two nextlines below selstart not empty
+		t = t_orig.splitlines(keepends=True)
+		tmp = t[1]
+		
+		if len(tmp.strip()) == 0:
+			
+			if numlines > 2:
+				tmp = t[2]
+				
+				if len(tmp.strip()) == 0:
+					#print('copy fail 6, two nextlines empty')
+					return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+					
+			# numlines == 2:
+			else:
+				#print('copy fail 5, numlines == 2, nextline is empty')
+				return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+		
+		for i in range(len(tmp)):
+			if not tmp[i].isspace():
+				self.indent_nextline = i
+				break
+
+		# Indentation difference of first line and next nonempty line
+		self.indent_diff = self.indent_nextline - self.indent_selstart
+		
+		# Continue checks
+		if self.indent_diff < 0:
+			# For example:
+			#
+			#			self.indent_selstart
+			#		self.indent_nextline
+			#indent0
+			#print('copy fail 7, indentation decreasing on first non empty line')
+			return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+			
+			
+		# Check if indent of any line in selection < self.indent_selstart
+		min_ind = self.indent_selstart
+		for i in range(1, numlines):
+			tmp = t[i]
+			
+			if len(tmp.strip()) == 0:
+				# This will skip rest of for-loop contents below
+				# and start next iteration.
+				continue
+			
+			for j in range(len(tmp)):
+				if not tmp[j].isspace():
+					if j < min_ind:
+						min_ind = j
+					# This will break out from this for-loop only.
+					break
+						
+		if self.indent_selstart > min_ind:
+			#print('copy fail 8, indentation of line in selection < self.indent_selstart')
+			return self.copy_fallback(selection=t_orig, flag_cut=flag_cut)
+
+		
+		if self.os_type != 'windows':
+			self.contents.clipboard_clear()
+			self.contents.clipboard_append(t_orig)
+		else:
+			self.copy_windows(selection=t_orig, flag_cut=flag_cut)
+			
+		self.flag_fix_indent = True
+		self.checksum_fix_indent = t_orig
+		
+		if flag_cut:
+			self.contents.delete(tkinter.SEL_FIRST, tkinter.SEL_LAST)
+		
+		#print('copy ok')
+		return 'break'
+		###################
+		
+	
+	def paste(self, event=None):
+		''' When selection started from start of block,
+				for example: cursor is before if-word,
+			and
+				selected at least one whole line below firsline
+				
+			Then
+				preserve indentation
+				of all lines in selection.
+				
+			This is done if self.flag_fix_indent is True.
+			If not, paste_fallback() is used instead.
+			self.flag_fix_indent is set in copy()
+		'''
+		
+		try:
+			t = self.contents.clipboard_get()
+			if len(t) == 0:
 				return 'break'
+				
+		# Clipboard empty
+		except tkinter.TclError:
+			return 'break'
+			
+		if not self.flag_fix_indent or t != self.checksum_fix_indent:
+			self.paste_fallback(event=event)
+			self.contents.edit_separator()
+			#print('paste norm')
+			return 'break'
+			
+		#print('paste ride')
+		
+
+		
+		have_selection = False
 		
+		if len( self.contents.tag_ranges('sel') ) > 0:
+			selstart = self.contents.index( '%s' % tkinter.SEL_FIRST)
+			selend = self.contents.index( '%s' % tkinter.SEL_LAST)
+			
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			have_selection = True
+		
+		
+		# Cursor index:
+		idx_insert_orig = self.contents.index(tkinter.INSERT)
+		idx_ins, col = map(int, idx_insert_orig.split('.'))
+		indent_cursor = col
+		indent_diff_cursor = indent_cursor - self.indent_selstart
+
+
+		# Split selection from clipboard to list
+		# and build string to be pasted.
+		tmp_orig = t.splitlines(keepends=True)
+		s = ''
+		s += tmp_orig[0]
+		lno = idx_ins + 1
+
+		for line in tmp_orig[1:]:
+
+			if indent_diff_cursor > 0:
+				# For example:
+				#
+				#	self.indent_selstart
+				#			indent_cursor
+				#indent0
+				
+				line = indent_diff_cursor*'\t' + line
+				
+			elif indent_diff_cursor < 0:
+				# For example:
+				#
+				#			self.indent_selstart
+				#		indent_cursor
+				#indent0
+				
+				# This is one reason to cancel in copy()
+				# if indentation of any line in selection < self.indent_selstart
+				line = line[-1*indent_diff_cursor:]
+				
+			#else:
+			#line == line
+			# same indentation level,
+			# so do nothing.
+			
+			s += line
+			lno += 1
+		
+		# Do paste string
+		self.contents.insert(idx_insert_orig, s)
+		lastline = lno - 1
+		len_lastline = len(tmp_orig[-1])
+		idx_insert_after = self.contents.index(
+			'%d.0 +%d chars' % (lastline, len_lastline) )
+		
+		
+		
+		tmp = t.splitlines(True)
+		
+		# Taken from paste_fallback
+		##########################
+		s = self.contents.index( '%s linestart' % idx_insert_orig)
+		e = self.contents.index( '%d.0 lineend' % lastline )
+		t = self.contents.get( s, e )
+		
+		if self.tabs[self.tabindex].filepath:
+			if self.can_do_syntax():
+				self.update_tokens( start=s, end=e, line=t )
+				
+		
+		if have_selection:
+			self.contents.tag_add('sel', selstart, selend)
+			
+		else:
+			self.contents.tag_add('sel', idx_insert_orig, idx_insert_after)
+			
+		self.contents.mark_set('insert', idx_insert_orig)
+		
+		
+		self.wait_for(100)
+		self.ensure_idx_visibility(idx_insert_orig)
+		#####
+		
+		self.contents.edit_separator()
+		return 'break'
+	
+	
+	def paste_fallback(self, event=None):
+		''' Fallback from paste
+		'''
+		
+		try:
+			tmp = self.clipboard_get()
+			tmp = tmp.splitlines(keepends=True)
+			
+			
+		except tkinter.TclError:
+			# is empty
+			return 'break'
+			
+		have_selection = False
+		
+		if len( self.contents.tag_ranges('sel') ) > 0:
+			selstart = self.contents.index( '%s' % tkinter.SEL_FIRST)
+			selend = self.contents.index( '%s' % tkinter.SEL_LAST)
+			
+			self.contents.tag_remove('sel', '1.0', tkinter.END)
+			have_selection = True
+			
+			
+		idx_ins = self.contents.index(tkinter.INSERT)
+		self.contents.event_generate('<<Paste>>')
+		
+		
+		# Selected many lines or
+		# one line and cursor is not at the start of next line:
+		if len(tmp) > 1:
+		
+			s = self.contents.index( '%s linestart' % idx_ins)
+			e = self.contents.index( 'insert lineend')
+			t = self.contents.get( s, e )
+			
+			if self.tabs[self.tabindex].filepath:
+				if self.can_do_syntax():
+					self.update_tokens( start=s, end=e, line=t )
+					
+			
+			if have_selection:
+				self.contents.tag_add('sel', selstart, selend)
+				
+			else:
+				self.contents.tag_add('sel', idx_ins, tkinter.INSERT)
+				
+			self.contents.mark_set('insert', idx_ins)
+			
+			
+			self.wait_for(100)
+			self.ensure_idx_visibility(idx_ins)
+			
+			
+		# Selected one line and cursor is at the start of next line:
+		elif len(tmp) == 1 and tmp[-1][-1] == '\n':
+			s = self.contents.index( '%s linestart' % idx_ins)
+			e = self.contents.index( '%s lineend' % idx_ins)
+			t = self.contents.get( s, e )
+			
+			if self.tabs[self.tabindex].filepath:
+				if self.can_do_syntax():
+					self.update_tokens( start=s, end=e, line=t )
+					
+			
+			if have_selection:
+				self.contents.tag_add('sel', selstart, selend)
+				
+			else:
+				self.contents.tag_add('sel', idx_ins, tkinter.INSERT)
+				
+			self.contents.mark_set('insert', idx_ins)
+			
+					
+		else:
+			if have_selection:
+				self.contents.tag_add('sel', selstart, selend)
+				self.contents.mark_set('insert', idx_ins)
+			
+			
+		return 'break'
+	
 
 	def move_line(self, event=None, direction=None):
 		''' Adjust cursor line indentation, with arrow left and right,
 			when pasting more than one line etc.
 		'''
 		
 		# currently this interferes with backspace_override
@@ -4110,93 +4615,22 @@
 					
 
 			return 'break'
 
 		return 'continue'
 	
 
-	def paste(self, event=None):
-		'''	First line usually is in wrong place after paste
-			because of selection has not started at the beginning of the line.
-			So we put cursor at the beginning of insertion after pasting it
-			so we can start indenting it.
-		'''
-		
-		try:
-			tmp = self.clipboard_get()
-			tmp = tmp.splitlines(keepends=True)
-			
-			
-		except tkinter.TclError:
-			# is empty
-			return 'break'
-			
-		have_selection = False
-		
-		if len( self.contents.tag_ranges('sel') ) > 0:
-			selstart = self.contents.index( '%s' % tkinter.SEL_FIRST)
-			selend = self.contents.index( '%s' % tkinter.SEL_LAST)
-			
-			self.contents.tag_remove('sel', '1.0', tkinter.END)
-			have_selection = True
-			
-			
-		line = self.contents.index(tkinter.INSERT)
-		self.contents.event_generate('<<Paste>>')
-		
-		
-		# Selected many lines or
-		# one line and cursor is not at the start of next line:
-		if len(tmp) > 1:
-		
-			s = self.contents.index( '%s linestart' % line)
-			e = self.contents.index( 'insert lineend')
-			t = self.contents.get( s, e )
-			
-			if self.tabs[self.tabindex].filepath:
-				if self.can_do_syntax():
-					self.update_tokens( start=s, end=e, line=t )
-					
-			
-			if have_selection:
-				self.contents.tag_add('sel', selstart, selend)
-				
-			else:
-				self.contents.tag_add('sel', line, tkinter.INSERT)
-				
-			self.contents.mark_set('insert', line)
-			
-			
-			self.wait_for(100)
-			self.ensure_idx_visibility(line)
-			
-			
-		# Selected one line and cursor is at the start of next line:
-		elif len(tmp) == 1 and tmp[-1][-1] == '\n':
-			s = self.contents.index( '%s linestart' % line)
-			e = self.contents.index( '%s lineend' % line)
-			t = self.contents.get( s, e )
-			
-			if self.tabs[self.tabindex].filepath:
-				if self.can_do_syntax():
-					self.update_tokens( start=s, end=e, line=t )
-					
-					
-		return 'break'
-	
-
 	def undo_override(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 		 
 		try:
 			self.contents.edit_undo()
 			
-			
 			self.do_syntax()
 			
 			
 		except tkinter.TclError:
 			self.bell()
 			
 		return 'break'
@@ -4236,14 +4670,26 @@
 		# self.search_idx marks range of focus-tag:
 		self.save_pos = self.search_idx[1]
 		self.stop_search()
 		
 		return 'break'
 	
 	
+	def insert_tab(self, event):
+		'''	Used to insert tab
+		'''
+		
+		if self.state in [ 'search', 'replace', 'replace_all' ]:
+			return 'break'
+			
+		self.contents.insert(tkinter.INSERT, '\t')
+		
+		return 'break'
+	
+	
 	def tab_override(self, event):
 		'''	Used to bind Tab-key with indent() and expander.expand_word()
 		'''
 		
 		if self.state in [ 'search', 'replace', 'replace_all' ]:
 			return 'break'
 		
@@ -5239,15 +5685,16 @@
 		
 			
 		self.contents.edit_reset()
 		self.contents.edit_modified(0)
 		self.avoid_viewsync_mess()
 		
 		self.bind("<Escape>", self.do_nothing)
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num,
+			lambda event: self.raise_popup(event))
 		
 		
 	def help(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 			
@@ -5493,156 +5940,154 @@
 			startpos = self.contents.index( '%s linestart' % s )
 			
 			endline = int( e.split('.')[0] )
 			endpos = self.contents.index( '%s lineend' % e )
 			
 			
 			for linenum in range(startline, endline+1):
-				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-				self.contents.insert(tkinter.INSERT, '##')
+				self.contents.insert('%d.0' % linenum, '##')
 				
 						
 			self.update_tokens(start=startpos, end=endpos)
+
 			
-				
-			self.contents.edit_separator()
-			return "break"
-		
+		# No selection, comment curline
 		except tkinter.TclError as e:
-			print(e)
-			return "break"
+			self.contents.insert('%s linestart' % tkinter.INSERT, '##')
+		
+		
+		self.contents.edit_separator()
+		return "break"
 	
 
 	def uncomment(self, event=None):
 		''' Should work even if there are uncommented lines between commented lines. '''
 		if self.state != 'normal':
 			self.bell()
 			return "break"
-			
+		
+		idx_ins = self.contents.index(tkinter.INSERT)
+		
 		try:
 			s = self.contents.index(tkinter.SEL_FIRST)
 			e = self.contents.index(tkinter.SEL_LAST)
 		
 			startline = int(s.split('.')[0])
 			endline = int(e.split('.')[0])
 			startpos = self.contents.index('%s linestart' % s)
 			endpos = self.contents.index('%s lineend' % e)
-				
 			changed = False
 			
 			for linenum in range(startline, endline+1):
-				self.contents.mark_set(tkinter.INSERT, '%s.0' % linenum)
-				tmp = self.contents.get('%s.0' % linenum,'%s.0 lineend' % linenum)
+				tmp = self.contents.get('%d.0' % linenum,'%d.0 lineend' % linenum)
 				
 				if tmp.lstrip()[:2] == '##':
-					tmp = tmp.replace('##', '', 1)
-					self.contents.delete('%s.0' % linenum,'%s.0 lineend' % linenum)
-					self.contents.insert(tkinter.INSERT, tmp)
+					self.contents.delete('%d.0' % linenum,
+						'%d.0 +2c' % linenum)
+					
 					changed = True
 					
 					
 			if changed:
-			
 				self.update_tokens(start=startpos, end=endpos)
-				
 				self.contents.edit_separator()
-			
+
+		
+		# No selection, uncomment curline
 		except tkinter.TclError as e:
-			print(e)
+			tmp = self.contents.get('%s linestart' % idx_ins,
+				'%s lineend' % idx_ins)
+			
+			if tmp.lstrip()[:2] == '##':
+				self.contents.delete('%s linestart' % idx_ins,
+					'%s linestart +2c' % idx_ins)
+				
+				self.contents.edit_separator()
+				
 		return "break"
 		
 ########## Indent and Comment End
 ################ Search Begin
 	
 	def check_next_event(self, event=None):
 		
 		if event.keysym == 'Left':
 			line = self.lastcursorpos
 			self.contents.tag_remove('sel', '1.0', tkinter.END)
 			self.contents.mark_set('insert', line)
 			self.ensure_idx_visibility(line)
 			
-			
 			self.contents.unbind("<Any-Key>", funcid=self.anykeyid)
 			self.contents.unbind("<Any-Button>", funcid=self.anybutid)
 			
 			f = self.check_sel
 			if self.os_type == 'mac_os': f = self.mac_cmd_overrides
 			
 			self.bid_left = self.contents.bind("<Left>", f )
-		
 			return 'break'
 			
 		else:
 			self.contents.unbind("<Any-Key>", funcid=self.anykeyid)
 			self.contents.unbind("<Any-Button>", funcid=self.anybutid)
 			
 			f = self.check_sel
 			if self.os_type == 'mac_os': f = self.mac_cmd_overrides
 			self.bid_left = self.contents.bind("<Left>", f )
-			
 			return
 			
 		
-		
-	def search_next(self, event=None):
-		'''	Do last search from cursor position, show and select next match.
+	def search_next(self, event=None, back=False):
+		'''	Do last search from cursor position, show and select next/previous match.
 			
-			This is for cases when you can not do replace ALL.
-			You need to choose when to insert AND insertion is not always
-			the same. But replace is too limited (can not insert, like in search).
-			So you do normal search and quit quickly. Then copy your insertion
-			'pattern' in clipboard, what you add to certain matches and then
-			maybe change something else, or you need sometimes delete match and
-			insert your clipboard 'pattern' etc...
-			
-			In short:
-			1: Do normal search
-			2: copy what you need to have in clipboard
-			3: ctrl-backspace until in right place
-			4: now easy to delete or add clipboard contents etc..
-			5: repeat 3-4
-			
-			shortcut: ctrl-backspace
+			Shortcut: Ctrl-(Shift)-Backspace
 		'''
 		
 		if self.state != 'normal' or self.old_word == '':
 			self.bell()
 			return "break"
 			
 			
 		wordlen = len(self.old_word)
 		self.lastcursorpos = self.contents.index(tkinter.INSERT)
-		pos = self.contents.search(self.old_word, 'insert +1c', tkinter.END)
+	
+		if back:
+			pos = self.contents.search(self.old_word, 'insert', backwards=True)
+		else:
+			pos = self.contents.search(self.old_word, 'insert +1c')
 		
-		# Try again from the beginning this time:
+
+		# Try again from the beginning/end this time:
 		if not pos:
-			pos = self.contents.search(self.old_word, '1.0', tkinter.END)
+		
+			if back:
+				pos = self.contents.search(self.old_word, tkinter.END, backwards=True)
+			else:
+				pos = self.contents.search(self.old_word, '1.0')
 			
-			# no oldword in file:
+			# No oldword in file:
 			if not pos:
 				self.bell()
-				#print('no')
 				return "break"
 		
+				
 		# Go back to last place with arrow left
 		self.anykeyid = self.contents.bind( "<Any-Key>", self.check_next_event)
 		self.anybutid = self.contents.bind( "<Any-Button>", self.check_next_event)
-		
+
 		# Without this one can not search by holding ctrl down and
 		# pressing and releasing repeatedly backspace only:
-		if self.bid_left: self.contents.unbind("<Left>", self.bid_left)
+		if self.bid_left: self.contents.unbind("<Left>", funcid=self.bid_left)
 		self.bid_left = None
+
 		
-		
-		lastpos = "%s + %dc" % (pos, wordlen)
+		word_end = "%s + %dc" % (pos, wordlen)
 		self.contents.tag_remove('sel', '1.0', tkinter.END)
 		self.contents.mark_set(self.anchorname, pos)
-		self.contents.tag_add('sel', pos, lastpos)
-		self.contents.mark_set('insert', lastpos)
+		self.contents.tag_add('sel', pos, word_end)
+		self.contents.mark_set('insert', word_end)
 		line = pos
 		self.ensure_idx_visibility(line)
 					
 		return "break"
 
 
 	def show_next(self, event=None):
@@ -5944,19 +6389,23 @@
 			return "break"
 			
 		self.contents.tag_remove('replaced', '1.0', tkinter.END)
 		self.bind("<Escape>", self.do_nothing)
 		
 	
 	def stop_search(self, event=None):
+		if self.state == 'waiting':
+			return 'break'
+			
 		self.contents.config(state='normal')
 		self.entry.config(state='normal')
 		self.btn_open.config(state='normal')
 		self.btn_save.config(state='normal')
-		self.contents.bind("<Button-%i>" % self.right_mousebutton_num, lambda event: self.raise_popup(event))
+		self.contents.bind("<Button-%i>" % self.right_mousebutton_num,
+			lambda event: self.raise_popup(event))
 		
 		#self.wait_for(200)
 		self.contents.tag_remove('focus', '1.0', tkinter.END)
 		self.contents.tag_remove('match', '1.0', tkinter.END)
 		self.contents.tag_remove('sel', '1.0', tkinter.END)
 		
 		# Leave marks on replaced areas, Esc clears.
@@ -5990,16 +6439,14 @@
 				
 				
 		self.state = 'normal'
 		self.contents.unbind( "<Control-n>", funcid=self.bid1 )
 		self.contents.unbind( "<Control-p>", funcid=self.bid2 )
 		self.contents.unbind( "<Double-Button-1>", funcid=self.bid3 )
 		self.contents.unbind( "<space>", funcid=self.bid4 )
-		self.contents.bind( "<Control-n>", self.move_down)
-		self.contents.bind( "<Control-p>", self.move_up)
 		self.contents.bind("<Return>", self.return_override)
 		self.entry.bind("<Control-n>", self.do_nothing_without_bell)
 		self.entry.bind("<Control-p>", self.do_nothing_without_bell)
 		self.bind( "<Return>", self.do_nothing_without_bell)
 		
 		
 		#self.wait_for(200)
@@ -6061,15 +6508,16 @@
 		
 		self.entry.delete(0, tkinter.END)
 		
 		
 		# Autofill from clipboard
 		try:
 			tmp = self.clipboard_get()
-			if 80 > len(tmp) > 0:
+			# Allow one linebreak
+			if 80 > len(tmp) > 0 and len(tmp.splitlines()) < 3:
 				self.entry.insert(tkinter.END, tmp)
 				self.entry.xview_moveto(1.0)
 				self.entry.select_to(tkinter.END)
 				self.entry.icursor(tkinter.END)
 				
 		# Empty clipboard
 		except tkinter.TclError:
```

### Comparing `henxel-0.3.1/src/henxel/changefont.py` & `henxel-0.3.2/src/henxel/changefont.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,39 +18,29 @@
 		self.fonts = fontlist
 		
 		if tracefunc:
 			self.tracefunc = tracefunc
 		else:
 			self.tracefunc = None
 		
-		self.badfonts = [
-					'Standard Symbols PS',
-					'OpenSymbol',
-					'Noto Color Emoji',
-					'FontAwesome',
-					'Dingbats',
-					'Droid Sans Fallback',
-					'D050000L'
-					]
-		
-		
 		self.max = 42
 		self.min = 8
 		
 		self.topframe = tkinter.Frame(self.top)
 		self.bottomframe = tkinter.Frame(self.top)
 		self.topframe.pack()
 		self.bottomframe.pack()
 		
 
 		self.option_menu_list = list()
 
 		for font in self.fonts:
 			self.option_menu_list.append(font.name)
 		
+		self.waitvar = tkinter.IntVar()
 		self.var = tkinter.StringVar()
 		self.var.set(self.option_menu_list[0])
 		self.font = tkinter.font.nametofont(self.var.get())
 		
 		self.optionmenu = tkinter.OptionMenu(self.topframe, self.var, *self.option_menu_list, command=self.optionmenu_command)
 		
 		# Set font of dropdown button:
@@ -101,50 +91,32 @@
 ##
 ##		self.overstrike = tkinter.StringVar()
 ##		self.cb4 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Overstrike', variable=self.overstrike)
 ##		self.cb4.pack(pady=10, anchor='w')
 ##		self.cb4.config(command=lambda args=[self.overstrike, 'overstrike']: self.checkbutton_command(args))
 		
 		
-		
 		self.filter_mono = tkinter.IntVar()
 		self.cb5 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Mono', variable=self.filter_mono)
 		self.cb5.pack(pady=10, anchor='w')
 		self.cb5.config(command=self.filter_fonts)
 		
-		self.filter_const_height = tkinter.IntVar()
-		self.cb6 = tkinter.Checkbutton(self.topframe, font=('TkDefaultFont', 10), offvalue=0, onvalue=1, text='Const height', variable=self.filter_const_height)
-		self.cb6.pack(pady=10, anchor='w')
-		self.cb6.config(command=self.filter_fonts)
-		
-			
-		info_text = '''Being monospaced does not guarantee same lineheight between lines not containing bold text
-and lines that do contain bold text, like keywords.
-Courier for example is monospaced but does not have this kind of constant lineheight.
-If choosing other than constant lineheight font, linenumbers
-can have little offset. If this does not bother, then select any monospaced for programming.'''
-
-
-		self.l = tkinter.Label(self.bottomframe, text=info_text, font=('TkDefaultFont', 10), anchor="e", justify=tkinter.LEFT)
-		self.l.pack(padx=4, pady=4)
-		
 		
 		# Get current fontsize and show it in spinbox
 		self.sb.delete(0, 'end')
 		fontsize = self.font['size']
 		self.sb.insert(0, fontsize)
 
 
 		# Check rest font configurations:
 		self.cb1.deselect()
 ##		self.cb2.deselect()
 ##		self.cb3.deselect()
 ##		self.cb4.deselect()
 		self.cb5.deselect()
-		self.cb6.deselect()
 		
 		if self.font['weight'] == 'bold': self.cb1.select()
 ##		if self.font['slant'] == 'italic': self.cb2.select()
 ##		if self.font['underline'] == 1: self.cb3.select()
 ##		if self.font['overstrike'] == 1: self.cb4.select()
 
 		self.lb.bind('<ButtonRelease-1>', self.change_font)
@@ -171,17 +143,15 @@
 					self.menu,
 					self.lb,
 					self.sb,
 					self.cb1,
 ##					self.cb2,
 ##					self.cb3,
 ##					self.cb4,
-					self.cb5,
-					self.cb6,
-					self.l
+					self.cb5
 					]
 					
 		if self.button['text'] == 'BIG':
 			for widget in widgetlist:
 				widget.config(font=('TkDefaultFont', 20))
 			
 		if self.button['text'] == 'SMALL':
@@ -192,38 +162,28 @@
 			self.button['text'] = 'SMALL'
 		else:
 			self.button['text'] = 'BIG'
 			
 	
 	
 	def filter_fonts(self, event=None):
-		'''	Show all fonts, mono-spaced, constant line height, or
-			mono-spaced and constant line height depending on cb5 and cb6
-			settings.
+		'''	Show all fonts or mono-spaced,
+			depending on cb5 setting.
 		'''
 	
 		filter_mono = self.filter_mono.get()
-		filter_const_height = self.filter_const_height.get()
-
 		fonts = None
 		
-		if filter_mono and filter_const_height:
-			fonts = self.fontnames_const_line_mono
-					
-		elif filter_mono:
-			fonts = self.fontnames_mono
-			
-		elif filter_const_height:
-			fonts = self.fontnames_const_line
 		
+		if filter_mono:
+			fonts = self.fontnames_mono
 		else:
 			fonts = self.fontnames
 		
 		
-		
 		self.top.selection_clear()
 		self.lb.delete(0, 'end')
 		
 		
 		for name in fonts:
 			self.lb.insert('end', name)
 		
@@ -309,74 +269,53 @@
 				)
 
 
 		if self.tracefunc:
 			self.tracefunc()
 
 	
+	def wait_for(self, ms):
+		self.waitvar.set(False)
+		self.top.after(ms, self.waiter)
+		self.top.wait_variable(self.waitvar)
+		
+		
+	def waiter(self):
+		self.waitvar.set(True)
+	
+	
 	def get_fonts(self):
 		'''	Return list of fonts, that have: same lineheight between normal
 			lines and lines with bold font.
 		'''
 		
-		font1 = tkinter.font.Font(family='TkDefaultFont', size=12)
-		boldfont = font1.copy()
-		boldfont.config(weight='bold')
+		font = tkinter.font.Font(family='TkDefaultFont', size=12)
 		
-		# Second test: filter out vertical fonts.
+		# Test: filter out vertical fonts.
 		def test_font(f):
-			return f in self.badfonts or f[0] == '@'
+			return f[0] == '@'
 			
 		
 		fontnames = [f for f in tkinter.font.families() if not test_font(f)]
 		
 		# Remove duplicates then sort
 		s = set(fontnames)
 		fontnames = [f for f in s]
 		fontnames.sort()
 		
 		
 		for name in fontnames:
-			font1.config(family=name)
-			boldfont.config(family=name)
-			
-			l1=font1.metrics()['linespace']
-			l2=boldfont.metrics()['linespace']
-			
-			a1=font1.metrics()['ascent']
-			a2=boldfont.metrics()['ascent']
-			
-			d1=font1.metrics()['descent']
-			d2=boldfont.metrics()['descent']
-			
-			f1=font1.metrics()['fixed']
-			f2=boldfont.metrics()['fixed']
-			
-			
-			# Give info that something is happening.
+			font.config(family=name)
+			font_is_fixed = font.metrics()['fixed']
 			self.fontnames.append(name)
 			self.lb.insert('end', name)
 			self.lb.see('end')
-			self.top.update_idletasks()
-			
-			
-			# This guarantees same lineheight between
-			# normal and bold lines. Consolas for example.
-			if l1 == l2 and a1 == a2 and d1 == d2:
-				self.fontnames_const_line.append(name)
+			self.wait_for(12)
 			
-				if f1 == True and f1 == f2:
-					self.fontnames_const_line_mono.append(name)
-			
-			
-			# Being monospaced does not guarantee same lineheight between
-			# normal and bold lines. Courier for example.
-			if f1 == True and f1 == f2:
-				self.fontnames_mono.append(name)
-					
+			if font_is_fixed: self.fontnames_mono.append(name)
 			
 
 		# Show current fontname in listbox
 		try:
 			fontname = self.font.actual("family")
 			fontindex = self.fontnames.index(fontname)
 			self.top.after(100, lambda args=[fontindex]: self.lb.select_set(args))
```

### Comparing `henxel-0.3.1/src/henxel/fdialog.py` & `henxel-0.3.2/src/henxel/fdialog.py`

 * *Files identical despite different names*

### Comparing `henxel-0.3.1/src/henxel/help.txt` & `henxel-0.3.2/src/henxel/help.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-		Keyboard shortcuts for macOS:
+		Keyboard shortcuts:
 		
 		If key-sequence is like: Ctrl-c
 		It means: while holding Ctrl-key down, press c-key.
 		
 		If key-sequence is like: Ctrl-c-f
 		It means: while holding Ctrl-key down, press first
 		c-key then f-key. It can be quite fast, more like: Ctrl-cf
 		 
 		Ctrl-Return		Open file
 		Ctrl-BackSpace  Show and select next occurence of last search.
 						If got too far, press arrowleft to go to last
 						cursor position. Search again in short.
+						To search backwards press
+						Ctrl-Shift-BackSpace
+						
 		Ctrl-f  Search
 		Ctrl-r  Replace
 		Ctrl-R  Replace all
 		Ctrl-g  Gotoline:	-1 and empty goes to file-end.
 							-20 goes to 20 lines before file-end etc.
 		Shift-Tab  Unindent
 		Tab        Indent, complete word
+		Ctrl-Tab   Insert Tab
 		
 		Shift-Return	Comment
 		Shift-BackSpace	Uncomment
 		
 		Ctrl-c  Copy		Try this: Ctrl-c-f
 		Ctrl-v  Paste
 		Ctrl-x  Cut
@@ -69,23 +73,15 @@
 		
 		# Not often needed:
 		Ctrl-plus 	Increase scrollbar-width
 		Ctrl-minus	Decrease scrollbar-width
 		
 		Ctrl-t  	Change indentation of selected lines to current setting
 		
-		Ctrl-i  Move cursor right
-		Ctrl-b  Move cursor left
-		Ctrl-n  Move cursor down
-		Ctrl-p  Move cursor up
 		
-		Ctrl-k  Remove from cursor to lineend
-		Ctrl-o  Insert linebreak at cursor
-		
-
 		While searching:
 			Ctrl-n  Next match
 			Ctrl-p  Prev match
 			-	Copying text to clipboard is possible with yank-line etc.
 			-	Changing the replacement string is possible while replacing.
 			-	1: Press Space to exit search to focus.
 				2: Double-click to exit to cursor.
```

### Comparing `henxel-0.3.1/src/henxel/help_mac.txt` & `henxel-0.3.2/src/henxel/help_mac.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-		Keyboard shortcuts for macOS:
+		Keyboard shortcuts:
 		
 		If key-sequence is like: Cmd-c
 		It means: while holding Cmd-key down, press c-key.
 		
 		If key-sequence is like: Cmd-c-f
 		It means: while holding Cmd-key down, press first
 		c-key then f-key. It can be quite fast, more like: Cmd-cf
 		 
 		Cmd-Return		Open file
 		Ctrl-BackSpace  Show and select next occurence of last search.
 						If got too far, press arrowleft to go to last
 						cursor position. Search again in short.
+						To search backwards press
+						Ctrl-Shift-BackSpace
+						
 		Cmd-f  Search
 		Cmd-r  Replace
 		Cmd-R  Replace all
 		Cmd-g  Gotoline:	-1 and empty goes to file-end.
 							-20 goes to 20 lines before file-end etc.
 		Shift-Tab  Unindent
 		Tab        Indent, complete word
+		Ctrl-Tab   Insert Tab
 		
 		Shift-Return	Comment
 		Shift-BackSpace	Uncomment
 		
 		Cmd-c  Copy		Try this: Cmd-c-f
 		Cmd-v  Paste
 		Cmd-x  Cut
@@ -69,23 +73,15 @@
 		
 		# Not often needed:
 		Ctrl-plus 	Increase scrollbar-width
 		Ctrl-minus	Decrease scrollbar-width
 		
 		Ctrl-t  	Change indentation of selected lines to current setting
 		
-		Ctrl-i  Move cursor right
-		Ctrl-b  Move cursor left
-		Ctrl-n  Move cursor down
-		Ctrl-p  Move cursor up
 		
-		Ctrl-k  Remove from cursor to lineend
-		Ctrl-o  Insert linebreak at cursor
-		
-
 		While searching:
 			Ctrl-n  Next match
 			Ctrl-p  Prev match
 			-	Copying text to clipboard is possible with yank-line etc.
 			-	Changing the replacement string is possible while replacing.
 			-	1: Press Space to exit search to focus.
 				2: Double-click to exit to cursor.
```

### Comparing `henxel-0.3.1/src/henxel/wordexpand.py` & `henxel-0.3.2/src/henxel/wordexpand.py`

 * *Files identical despite different names*

### Comparing `henxel-0.3.1/src/henxel.egg-info/PKG-INFO` & `henxel-0.3.2/src/henxel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: henxel
-Version: 0.3.1
+Version: 0.3.2
 Summary: GUI-editor for Python development.
 Home-page: https://github.com/SamuelKos/henxel
 Author: SamuelKos
 Author-email: koskinens371@gmail.com
 Project-URL: Bug Tracker, https://github.com/SamuelKos/henxel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Editors
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Henxel
 GUI-editor for Python development. Tested to work with Debian 12, Windows 10 and 11 and macOS 12.
 
 ![editor_mac](pics/editor_macOS.png)
+
 ![editor_linux](pics/editor_linux.png)
 
 # Featuring
 * Auto-indent
 * Font Chooser
 * Color Chooser
 * Line numbering
@@ -112,16 +113,16 @@
 
 Launch Henxel:
 myproject> env\launch_ed.bat
 ```
 
 
 # Prerequisites in macOS and venv-creation
-Python installation (you may need to install newer version of python from python.org)
-should already include tkinter. There currently is no mkvenv script for macOS,
+You will need to install newer version of python with Homebrew. Look info on the ARR-repository
+about how to do that. There currently is no mkvenv script for macOS,
 but making venv is quite same as in Linux. It seems to be enough to make venv
 and then install henxel to it without anything else.
 
 ```console
 ~$ mkdir myproject
 ~$ cd myproject
 ~/myproject$ python -m venv env
@@ -173,13 +174,15 @@
 (env) ~/myproject/henxel$ pip install --no-build-isolation -e .
 ```
 
 Files are in src/henxel/
 
 
 # More resources
-[Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
-[Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
-[Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
+* [Tcl/Tk](https://tcl.tk/man/tcl9.0/TkCmd/index.html)
+
+* [Python/Tkinter](https://docs.python.org/3/library/tkinter.html)
+
+* [Changelog](https://github.com/SamuelKos/henxel/blob/main/CHANGELOG)
 
 # Licence
 This project is licensed under the terms of the GNU General Public License v3.0.
```

