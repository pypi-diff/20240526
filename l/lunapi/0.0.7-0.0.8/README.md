# Comparing `tmp/lunapi-0.0.7-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/lunapi-0.0.8-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,10 @@
-Zip file size: 10339519 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 00:15 lunapi.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 00:15 lunapi-0.0.7.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 00:15 lunapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 00:15 lunapi-0.0.7.dist-info/licenses/
--rw-rw-r--  2.0 unx     1350 b- defN 24-May-02 00:15 lunapi-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      640 b- defN 24-May-02 00:15 lunapi-0.0.7.dist-info/RECORD
--rw-rw-r--  2.0 unx      165 b- defN 24-May-02 00:15 lunapi-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx    35149 b- defN 24-May-02 00:15 lunapi-0.0.7.dist-info/licenses/LICENSE
--rw-r--r--  2.0 unx     9947 b- defN 24-May-02 00:15 lunapi/lunapi0.cpp
--rwxr-xr-x  2.0 unx 27300736 b- defN 24-May-02 00:15 lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    48099 b- defN 24-May-02 00:15 lunapi/lunapi1.py
--rw-r--r--  2.0 unx      352 b- defN 24-May-02 00:15 lunapi/__init__.py
-12 files, 27396438 bytes uncompressed, 10337985 bytes compressed:  62.3%
+Zip file size: 6916756 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      352 b- defN 24-May-26 02:31 lunapi/__init__.py
+-rw-r--r--  2.0 unx    84530 b- defN 24-May-26 02:31 lunapi/lunapi1.py
+-rwxr-xr-x  2.0 unx 15223136 b- defN 24-May-26 02:31 lunapi/lunapi0.pypy39-pp73-darwin.so
+-rw-r--r--  2.0 unx    12728 b- defN 24-May-26 02:31 lunapi/lunapi0.cpp
+-rw-rw-r--  2.0 unx      631 b- defN 24-May-26 02:31 lunapi-0.0.8.dist-info/RECORD
+-rw-rw-r--  2.0 unx      118 b- defN 24-May-26 02:31 lunapi-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1350 b- defN 24-May-26 02:31 lunapi-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-26 02:31 lunapi-0.0.8.dist-info/licenses/LICENSE
+8 files, 15357994 bytes uncompressed, 6915694 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,37 +1,25 @@
-Filename: lunapi.libs/
-Comment: 
-
-Filename: lunapi-0.0.7.dist-info/
-Comment: 
-
-Filename: lunapi/
-Comment: 
-
-Filename: lunapi-0.0.7.dist-info/licenses/
-Comment: 
-
-Filename: lunapi-0.0.7.dist-info/METADATA
+Filename: lunapi/__init__.py
 Comment: 
 
-Filename: lunapi-0.0.7.dist-info/RECORD
+Filename: lunapi/lunapi1.py
 Comment: 
 
-Filename: lunapi-0.0.7.dist-info/WHEEL
+Filename: lunapi/lunapi0.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: lunapi-0.0.7.dist-info/licenses/LICENSE
+Filename: lunapi/lunapi0.cpp
 Comment: 
 
-Filename: lunapi/lunapi0.cpp
+Filename: lunapi-0.0.8.dist-info/RECORD
 Comment: 
 
-Filename: lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
+Filename: lunapi-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: lunapi/lunapi1.py
+Filename: lunapi-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: lunapi/__init__.py
+Filename: lunapi-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## lunapi/lunapi0.cpp

```diff
@@ -260,24 +260,82 @@
 	 "List command/strata tuples resulting from a prior eval()" )
     .def("vars",&lunapi_inst_t::variables,
 	 "List variables (columns) from a table (defined by a command/strat pair) from a prior eval()")
     .def("table",py::overload_cast<const std::string &,const std::string &>(&lunapi_inst_t::results,py::const_) ,
 	 "Return a result table (defined by a command/strata pair) from a prior eval()" )
     .def("tables",py::overload_cast<>(&lunapi_inst_t::results,py::const_) ,
 	 "Return a result table (defined by a command/strata pair) from a prior eval()" )
-    
+
+    .def( "get_id", [](const lunapi_inst_t & a) { return a.get_id(); } )
+
     .def("__repr__",
 	 [](const lunapi_inst_t & a)
 	 {
 	   std::string s = "<lunapi-instance id:" + a.get_id();
 	   const std::string f1 = a.get_edf_file();
 	   const std::string f2 = a.get_annot_files();
 	   if ( f1 != "" ) s += " edf:" + f1;
 	   if ( f2 != "" ) s += " annot:" + f2;
 	   s += ">";
 	   return s;
 	 }
 	 );
- 
+
+
+
+  //
+  // segsrv_t : segment-server instance (linked to a single lunapi_inst_t)
+  //
   
+  py::class_<segsrv_t>(m, "segsrv")
+    .def(py::init<lunapi_inst_ptr>())
+    .def( "populate", &segsrv_t::populate,
+	  "Initiate segment-server channels, annots" ,
+	  "chs"_a , "anns"_a )
+    .def( "set_window", &segsrv_t::set_window,	  
+	  "Define current window" ,
+	  "start"_a , "stop"_a )
+    .def( "get_signal", &segsrv_t::get_signal )
+    .def( "get_timetrack", &segsrv_t::get_timetrack )
+    .def( "get_time_scale", &segsrv_t::get_time_scale )
+    .def( "set_scaling", &segsrv_t::set_scaling )
+    .def( "fix_physical_scale", &segsrv_t::fix_physical_scale )
+    .def( "free_physical_scale", &segsrv_t::free_physical_scale )
+    .def( "get_scaled_signal", &segsrv_t::get_scaled_signal )
+    .def( "get_gaps" , &segsrv_t::get_gaps )
+
+    .def( "set_epoch_size", &segsrv_t::set_epoch_size )
+    .def( "calc_bands", &segsrv_t::calc_bands ) // say which channels to do this for
+    .def( "calc_hjorths" , &segsrv_t::calc_hjorths )
+    .def( "nepochs" , &segsrv_t::nepochs )
+
+    .def( "get_epoch_size" , &segsrv_t::get_epoch_size )
+    //    .def( "get_epoch_timetrack" , &segsrv_t::get_epoch_timetrack )
+    .def( "get_bands", &segsrv_t::get_bands ) // actually return the final epoch x band matrix for channel ch
+    .def( "get_hjorths" , &segsrv_t::get_hjorths )
+
+    //    .def( "get_ungapped_total_sec" , &segsrv_t::get_ungapped_total_sec )
+    .def( "get_total_sec" , &segsrv_t::get_total_sec )
+    .def( "get_total_sec_original" , &segsrv_t::get_total_sec_original )
+    .def( "is_window_valid" , &segsrv_t::is_window_valid )
+    .def( "get_window_left"  , &segsrv_t::get_window_left )
+    .def( "get_window_right" , &segsrv_t::get_window_right )
+    .def( "get_window_left_hms" , &segsrv_t::get_window_left_hms )
+    .def( "get_window_right_hms" , &segsrv_t::get_window_right_hms )
+    .def( "get_clock_ticks" , &segsrv_t::get_clock_ticks )
+    .def( "get_window_phys_range" , &segsrv_t::get_window_phys_range )
+    .def( "get_ylabel" , &segsrv_t::get_ylabel )
+    .def( "throttle" , &segsrv_t::throttle )
+    .def( "input_throttle" , &segsrv_t::input_throttle )
+    .def( "summary_threshold_mins" , &segsrv_t::summary_threshold_mins )
+    .def( "serve_raw_signals", &segsrv_t::serve_raw_signals )
+    .def( "get_summary_stats", &segsrv_t::get_summary_stats )
+    .def( "get_summary_timetrack", &segsrv_t::get_summary_timetrack )
+
+    .def( "compile_evts" , &segsrv_t::compile_evts )
+    .def( "get_evnts_xaxes" , &segsrv_t::get_evnts_xaxes )
+    .def( "get_evnts_yaxes" , &segsrv_t::get_evnts_yaxes )
+    .def( "fetch_all_annots", &segsrv_t::fetch_all_evts )
+    .def( "fetch_annots" , &segsrv_t::fetch_evts ); 
+
 }
```

## lunapi/lunapi1.py

```diff
@@ -1,27 +1,34 @@
 """lunapi1 module provides a high-level convenience wrapper around lunapi0 module functions."""
 
 # Luna Python wrapper
-# v0.0.7, 1-May-2024
+# v0.0.8, 23-May-2024
 
 import lunapi.lunapi0 as _luna
+
 import pandas as pd
 import numpy as np
+from scipy.stats.mstats import winsorize
+
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from IPython.core import display as ICD
-from scipy.stats.mstats import winsorize
+import plotly.graph_objects as go
+import plotly.express as px
+from ipywidgets import widgets, AppLayout
+from itertools import cycle
+
 
 # resource set for Docker container version
 class resources:
    POPS_PATH = '/build/nsrr/common/resources/pops/'
    POPS_LIB = 's2'
    MODEL_PATH = '/build/luna-models/'
 
-lp_version = "v0.0.7"
+lp_version = "v0.0.8"
    
 # C++ singleton class (engine & sample list)
 # lunapi_t      --> luna
 
 # one observation
 # lunapi_inst_T --> inst
 
@@ -477,14 +484,18 @@
       else:
          self.edf = _luna.inst()
 
    def __repr__(self):
       return f'{self.edf}'
 
    #------------------------------------------------------------------------
+   def id(self):
+      return self.edf.get_id()
+      
+   #------------------------------------------------------------------------
    def attach_edf( self, f ):
       """Attach an EDF from a file"""
       return self.edf.attach_edf( f )
 
    #------------------------------------------------------------------------
    def attach_annot( self, annot ):
       """Attach annotations from a file"""
@@ -590,14 +601,38 @@
    def annots( self ):
       """Returns of dataframe of current annotations"""
       t = pd.DataFrame( self.edf.annots() )
       if len( t ) == 0: return t
       t.columns = ["Annotations"]
       return t
 
+   #------------------------------------------------------------------------   
+   def fetch_annots( self , anns ):
+      """Returns of dataframe of annotation events"""
+      if type( anns ) is not list: anns = [ anns ]
+      t = pd.DataFrame( self.edf.fetch_annots( anns ) )
+      if len( t ) == 0: return t
+      t.columns = ['Class', 'Start', 'Stop' ]
+      t = t.sort_values(by=['Start', 'Stop', 'Class'])
+      t['Start'] = t['Start'].round(decimals=3)
+      t['Stop'] = t['Stop'].round(decimals=3)
+      return t
+
+   #------------------------------------------------------------------------   
+   def fetch_fulls_annots( self , anns ):
+      """Returns of dataframe of annotation events"""
+      if type( anns ) is not list: anns = [ anns ]
+      t = pd.DataFrame( self.edf.fetch_full_annots( anns ) )
+      if len( t ) == 0: return t
+      t.columns = ['Class', 'Instance','Channel','Meta','Start', 'Stop' ]
+      t = t.sort_values(by=['Start', 'Stop', 'Class','Instance'])
+      t['Start'] = t['Start'].round(decimals=3)
+      t['Stop'] = t['Stop'].round(decimals=3)
+      return t
+
    #------------------------------------------------------------------------
    def eval( self, cmdstr ):
       """Evaluate one or more Luna commands, storing results internally"""
       self.edf.eval( cmdstr )
       return self.strata()
       
    #------------------------------------------------------------------------
@@ -770,28 +805,181 @@
       psd( df = df , ch = ch , var = var ,
            minf = minf , maxf = maxf , minp = minp , maxp = maxp ,
            xlines = xlines , ylines = ylines )
       
     
    # --------------------------------------------------------------------------------
    def spec( self, ch, var = 'PSD' , mine = None, maxe = None, minf = None, maxf = None , w = 0.025 ):
-      """Generates a PSD spectrogram (from PSD or MTM)"""
+      """Generates an epoch-level PSD spectrogram (from PSD or MTM)"""
       if ch is None: return
       if type(ch) is not list: ch = [ ch ]
 
       if var == 'PSD':
          self.eval( 'PSD epoch-spectrum dB sig=' + ','.join(ch) )
          df = self.table( 'PSD' , 'CH_E_F' )
       else:
          self.eval( 'MTM epoch-spectra epoch epoch-output dB tw=15 sig=' + ','.join(ch) )
          df = self.table( 'MTM' , 'CH_E_F' )
          
       spec( df = df , ch = None , var = var ,
             mine = mine , maxe = maxe , minf = minf , maxf = maxf , w = w )
-   
+
+
+   # --------------------------------------------------------------------------------
+   #  tfview : spectral regional viewer
+
+   # for high-def plots:
+   # import matplotlib as mpl 
+   # mpl.rcParams['figure.dpi'] = 300 
+
+   def tfview( self , ch,
+               e = None , t = None , a = None,
+               tw = 2, sec = 2 , inc = 0.1 ,             
+               f = ( 0.5 , 30 ) , winsor = 0.025 ,
+               anns = None , norm = None ,
+               traces = True, 
+               xlines = None , ylines = None , silent = True , pal = 'turbo' ):
+
+      """Generates an MTM spectrogram
+
+      Main channel
+      ------------
+      ch   : a single channel --> MTM 
+
+      Selection of intervals
+      ----------------------
+      e    : one or [ start , stop ] epochs (1-based)
+    
+      Optional views
+      --------------
+      traces  : T/F show raw signal
+      anns : show optional annotations
+
+      Misc
+      ----
+      norm : normalization mode    
+      todo: option to specify hms times
+      todo: collapse over time-locked values (e.g. TLOCK)
+      
+      """
+
+      # for now, accept only a single channel
+      assert type(ch) is str
+
+      # units
+      hdr = self.headers()
+      units = dict( zip( hdr.CH , hdr.PDIM ) )
+
+      # define window                                                                                                                                                                                                                                          
+      w = None
+      if type(e) is list and len(e) == 2 :
+         w = self.e2i( e )
+         w = [ i for tuple in w for i in tuple ]
+         w = [ min(w) , max(w) ] 
+      elif type(e) is int:
+         w = self.e2i( e )
+         w = [ i for tuple in w for i in tuple ]
+      elif type( t ) is list and len( t ) == 2:
+         w = t
+
+      if w is None: return
+
+      # window in seconds
+      ws = [ x * 1e-9 for x in w ]
+      ls = ws[1] - ws[0]
+
+      # build command
+      cstr = 'MTM dB  segment-sec=' + str(sec) + ' segment-inc=' + str(inc) + ' tw=' + str(tw)
+      cstr += ' segment-spectra segment-output sig=' + ','.join( [ ch ] )
+      cstr += ' start=' + str(ws[0]) + ' stop=' + str(ws[1]) 
+      if f is not None: cstr += ' min=' + str(f[0]) + ' max=' + str(f[1]) 
+                
+      # run MTM
+      if silent is True: self.silent_proc( cstr )
+      else: self.proc( cstr )
+    
+      if self.empty_result_set(): return
+    
+      # extract
+      tf = self.table( 'MTM' , 'CH_F_SEG' )
+      tf = tf.astype({'SEG': int })
+      tf.drop( 'ID' , axis=1, inplace=True)
+
+      tt = self.table('MTM','CH_SEG')
+      tt = tt.astype({'SEG': int })
+      tt['T'] = tt[['START', 'STOP']].mean(axis=1)
+      tt.drop( ['ID','DISC','START','STOP'] , axis=1, inplace=True)
+
+      m = pd.merge( tt ,tf , on= ['CH','SEG'] )    
+
+      x = m['T'].to_numpy(dtype=float)
+      y = m['F'].to_numpy(dtype=float)
+      z = m['MTM'].to_numpy(dtype=float)    
+      u = m['T'].unique()
+
+      # normalize?
+      if norm == 't':
+         groups = m.groupby(['CH','F'])[['MTM']]
+         mean, std = groups.transform("mean"), groups.transform("std")
+         mz = (m[mean.columns] - mean) / std
+         z = mz['MTM'].to_numpy(dtype=float)
+
+
+      # clip y-axes to observed
+      if max(y) < f[1]: f = (f[0] , max(y))
+      if min(y) > f[0]: f = (min(y) , f[1])
+    
+      # get time domain signal/annotations
+      d = self.slices( [ (w[0] , w[1] )] , chs = ch , annots = anns , time = True )
+      dt = d[1][0]
+      tx = dt[:,0]
+      dvs = d[0][1:]
+    
+      # make spectrogram
+      xn = np.unique(x).size
+      yn = np.unique(y).size
+    
+      # winsorize power
+      z = winsorize( z , limits=[winsor, winsor] )
+    
+      zi, yi, xi = np.histogram2d(y, x, bins=(yn,xn), weights=z, density=False )
+      counts, _, _ = np.histogram2d(y, x, bins=(yn,xn))
+      with np.errstate(divide='ignore', invalid='ignore'): zi = zi / counts
+      zi = np.ma.masked_invalid(zi)    
+    
+      # do plot
+  
+      if traces is True:
+         fig, axs = plt.subplots( nrows = 2 , ncols = 1 , sharex=True,  height_ratios=[1, 2] )
+         axs[0].set_title( self.id() )
+         fig.set_figheight(5)
+         fig.set_figwidth(15)
+         axs[0].set_ylabel( ch + ' (' + units[ch] + ')' ) 
+         axs[0].set(xlim=ws)
+         axs[1].set(xlim=ws, ylim=f)
+         axs[1].set_xlabel('Time (secs)')
+         axs[1].set_ylabel('Frequency (Hz)')
+         p1 = axs[1].pcolormesh(xi, yi, zi, cmap = pal )
+         fig.colorbar(p1, orientation="horizontal", drawedges = False, shrink = 0.2 , pad = 0.3)
+         [ axs[0].plot( tx , dt[:,di+1] , label = dvs[di] , linewidth=0.5 ) for di in range(0,len(dvs)) if dvs[di] in [ ch ] ]
+
+      if traces is False:
+         fig, ax = plt.subplots( nrows = 1 , ncols = 1 , sharex=True  )
+         ax.set_title( self.id() )
+         fig.set_figheight(5)
+         fig.set_figwidth(15)
+         ax.set(xlim=ws, ylim=f)
+         ax.set_xlabel('Time (secs)')
+         ax.set_ylabel('Frequency (Hz)')
+         p1 = ax.pcolormesh(xi, yi, zi, cmap = pal )
+         fig.colorbar(p1, orientation="horizontal", drawedges = False, shrink = 0.2 , pad = 0.3)
+
+      return
+
+
    # --------------------------------------------------------------------------------
    def pops( self, s = None, s1 = None , s2 = None,
              path = None , lib = None ,
              do_edger = True ,
              no_filter = False ,
              do_reref = False ,
              m = None , m1 = None , m2 = None ,
@@ -1190,15 +1378,14 @@
    ax.stackplot(x, y.T , colors = stgcol([ 'N1','N2','N3','R','W']) )
    ax.set(xlim=(1, ne), xticks=[ 1 , ne ] , 
           ylim=(0, 1), yticks=np.arange(0, 1))                                                                                             
    plt.show()
 
 
 
-
 # --------------------------------------------------------------------------------
 def psd(df , ch, var = 'PSD' , minf = None, maxf = None, minp = None, maxp = None , 
         xlines = None , ylines = None, dB = False ):
     """Returns a PSD plot from PSD or MTM epoch table (CH_F)"""
     if ch is None: return
     if type( ch ) is not list: ch = [ ch ]
     if type( xlines ) is not list and xlines != None: xlines = [ xlines ]
@@ -1334,7 +1521,751 @@
 #th_vals[ch_names == "O2"] = 0
 #lmts=[-4, 4]#"default"
 #ltopo_heat(ch_names, ch_vals, th_vals = th_vals, th=0.05,
 #           lmts=lmts, sz=70,
 #           colormap = "bwr", title = "DENSITY", 
 #           rimcolor="black", lab = "n/min")
    
+
+# --------------------------------------------------------------------------------
+# segsrv
+
+class segsrv:
+   """Segment server instance"""
+
+   def __init__(self,p):
+      assert isinstance(p,inst)
+      self.p = p
+      self.segsrv = _luna.segsrv(p.edf)
+      
+   def populate(self,chs=None,anns=None,max_sr=None):
+      if chs is None: chs = self.p.edf.channels()
+      if anns is None: anns = self.p.edf.annots()
+      if type(chs) is not list: chs = [ chs ]
+      if type(anns) is not list: anns = [ anns ]
+      if type(max_sr) is int: self.segsrv.input_throttle( max_sr )
+      self.segsrv.populate( chs , anns )
+
+   def window(self,a,b):
+      assert isinstance(a, (int, float) )
+      assert isinstance(b, (int, float) )
+      self.segsrv.set_window( a, b )
+      
+   def get_signal(self,ch):
+      assert isinstance(ch, str )
+      return self.segsrv.get_signal( ch )
+
+   def get_timetrack(self,ch):
+      assert isinstance(ch, str )
+      return self.segsrv.get_timetrack( ch )
+
+   def get_time_scale(self):
+      return self.segsrv.get_time_scale()
+
+   def get_gaps(self):
+      return self.segsrv.get_gaps()
+
+   def set_scaling(self, nchs, nanns = 0 , yscale = 1 , ygroup = 1 , yheader = 0.05 , yfooter = 0.05 , scaling_fixed_annot = 0.1 ):
+      self.segsrv.set_scaling( nchs, nanns, yscale, ygroup, yheader, yfooter, scaling_fixed_annot )
+
+   def get_scaled_signal(self, ch, n1):
+      return self.segsrv.get_scaled_signal( ch , n1 )
+
+   def fix_physical_scale(self,ch,lwr,upr):
+      self.segsrv.fix_physical_scale( ch, lwr, upr )
+
+   def free_physical_scale( self, ch ):
+      self.segsrv.free_physical_scal( ch )
+
+   def set_epoch_size( self, s ):
+      self.segsrv.set_epoch_size( s )
+
+   def get_epoch_size( self):
+      return self.segsrv.get_epoch_size()
+
+#   def get_epoch_timetrack(self):
+#      return self.segsrv.get_epoch_timetrack()
+      
+   def num_epochs( self) :
+      return self.segsrv.nepochs()
+
+#   def num_seconds( self ):
+#      return self.segsrv.get_ungapped_total_sec()
+   
+   def num_seconds_clocktime( self ):
+      return self.segsrv.get_total_sec()
+   
+   def num_seconds_clocktime_original( self ):
+      return self.segsrv.get_total_sec_original()
+
+   def calc_bands( self, chs ):
+      if type( chs ) is not list: chs = [ chs ]
+      self.segsrv.calc_bands( chs );
+
+   def calc_hjorths( self, chs ):
+      if type( chs ) is not list: chs = [ chs ]
+      self.segsrv.calc_hjorths( chs );
+
+   def get_bands( self, ch ):
+      return self.segsrv.get_bands( ch )
+
+   def get_hjorths( self, ch ):
+      return self.segsrv.get_hjorths( ch )
+   
+   def valid_window( self ):
+      return self.segsrv.is_window_valid()
+
+   def is_clocktime( self ):
+      return self.segsrv.is_clocktime()
+
+   def get_window_left( self ):
+      return self.segsrv.get_window_left()
+
+   def get_window_right( self ):
+      return self.segsrv.get_window_right()
+   
+   def get_window_left_hms( self ):
+      return self.segsrv.get_window_left_hms()
+
+   def get_window_right_hms( self ):
+      return self.segsrv.get_window_right_hms()
+
+   def get_clock_ticks( self , n = 6 ):
+      assert type( n ) is int
+      return self.segsrv.get_clock_ticks( n )
+   
+   def get_window_phys_range( self , ch ):
+      assert type(ch) is str
+      return self.segsrv.get_window_phys_range( ch )
+   
+   def get_ylabel( self , n ):
+      assert type(n) is int
+      return self.segsrv.get_ylabel( n )
+
+   def throttle(self,n):
+      assert type(n) is int
+      self.segsrv.throttle(n)
+
+   def input_throttle(self,n):
+      assert type(n) is int
+      self.segsrv.input_throttle(n)
+
+   def summary_threshold_mins(self,m):
+      assert type(m) is int or type(m) is float
+      self.segsrv.summary_threshold_mins(m)
+
+   def get_annots(self):
+      return self.segsrv.fetch_annots()
+
+   def get_all_annots(self,anns):
+      return self.segsrv.fetch_all_annots(anns)
+
+   def compile_windowed_annots(self,anns):
+      self.segsrv.compile_evts( anns )
+
+   def get_annots_xaxes(self,ann):
+      return self.segsrv.get_evnts_xaxes( ann )
+
+   def get_annots_yaxes(self,ann):
+      return self.segsrv.get_evnts_yaxes( ann )
+
+
+
+
+# --------------------------------------------------------------------------------
+#
+# Scope viewer
+#
+# --------------------------------------------------------------------------------
+
+def scope( p,
+           chs = None,
+           bsigs = None , 
+           hsigs = None,
+           anns = None ,
+           stgs = [ 'N1' , 'N2' , 'N3' , 'R' , 'W' , '?' , 'L' ] ,
+           stgcols = { 'N1':'blue' , 'N2':'blue', 'N3':'navy','R':'red','W':'green','?':'gray','L':'yellow' } ,
+           stgns = { 'N1':-1 , 'N2':-2, 'N3':-3,'R':0,'W':1,'?':2,'L':2 } ,
+           sigcols = None,
+           anncols = None, 
+           throttle1_sr = 100 ,
+           throttle2_np = 5 * 30 * 100 , 
+           summary_mins = 30 ,
+           height = 600 ,
+           annot_height = 0.15 ,
+           header_height = 0.04 ,
+           footer_height = 0.01 
+          ):
+
+    # defaults
+    scope_epoch_sec = 30
+    
+    # internally, we use 'sigs' but 'chs' is a more lunapi-consistent label
+    sigs = chs
+    
+    # all signals/annotations present    
+    all_sigs = p.edf.channels()
+    all_annots = p.edf.annots()
+
+    # units
+    hdr = p.headers()
+    units = dict( zip( hdr.CH , hdr.PDIM ) )
+    
+    # defaults
+    if sigs is None: sigs = all_sigs
+    if bsigs is None: bsigs = p.var( 'eeg' ).split(",")
+    if hsigs is None: hsigs = p.var( 'eeg' ).split(",")
+    if anns is None: anns = all_annots
+    
+    # ensure we do not have weird channels
+    sigs = [x for x in all_sigs if x in sigs]
+    bsigs = [x for x in sigs if x in bsigs ]
+    hsigs = [x for x in sigs if x in hsigs ]
+    anns = [x for x in all_annots if x in anns ]
+    sig2n = dict( zip( sigs , list(range(0,len(sigs)))) )
+
+    # empty?
+    if len( sigs ) == 0 and len( anns ) == 0:
+        print( 'No valid channels or annotations to display')
+        return None
+    
+    # initiate segment-serverns 
+    ss = segsrv( p )
+    ss.calc_bands( bsigs )
+    ss.calc_hjorths( hsigs )
+    if type( throttle1_sr ) is int: ss.input_throttle( throttle1_sr )
+    if type( throttle2_np ) is int: ss.throttle( throttle2_np )
+    if type( summary_mins ) is int or type( summary_mins ) is float: ss.summary_threshold_mins( summary_mins )
+    
+    ss.populate( chs = sigs , anns = anns )
+
+    # some key variables
+    nsecs_clk = ss.num_seconds_clocktime_original()
+    epoch_max = int( nsecs_clk / scope_epoch_sec )
+    
+    # color palette
+    pcyc = cycle(px.colors.qualitative.Bold)
+    palette = dict( zip( sigs , [ next(pcyc) for i in list(range(0,len(sigs))) ] ) )    
+    apalette = dict( zip( anns , [ next(pcyc) for i in list(range(0,len(anns))) ] ) )
+    # update w/ any user-specified cols, from anncols = { 'ann':'col' }  
+    if sigcols is not None:
+        for key, value in sigcols.items(): palette[ key ] = value
+    if stgcols is not None:
+        for key, value in stgcols.items(): apalette[ key ] = value
+    if anncols is not None:
+        for key, value in anncols.items(): apalette[ key ] = value
+    
+
+
+    # define widgets
+
+    wlay1 = widgets.Layout( width='95%' ) 
+    
+    # channel selection box
+    chlab = widgets.Label( value = 'Channels:' )
+    chbox  = widgets.SelectMultiple( options=sigs, value=sigs, rows=7, description='', disabled=False , layout = wlay1 )
+    if len(bsigs) != 0: pow_sel = widgets.Dropdown( options = bsigs, value=bsigs[0],description='',disabled=False,layout = wlay1 )
+    else: pow_sel = widgets.Dropdown( options = bsigs, value=None,description="Band power:",disabled=False,layout = wlay1 )
+    band_hjorth_sel = widgets.Checkbox( value = True , description = 'Hjorth' , disabled=False, indent=False )
+    
+    # annotations (display)
+    anlab = widgets.Label( value = 'Annotations:' )
+    anbox = widgets.SelectMultiple( options=anns , value=[], rows=3, description='', disabled=False , layout = wlay1 )
+
+    # annotations (instance list/navigation)
+    a1lab = widgets.Label( value = 'Instances:' )
+    ansel = widgets.SelectMultiple( options=anns , value=[], rows=3, description='', disabled=False , layout = wlay1 )
+    a1box = widgets.Select( options=[None] , value=None, rows=3, description='', disabled=False , layout = wlay1 )
+
+    # time display labels
+    tbox = widgets.Label( value = 'T: ' )
+    tbox2 = widgets.Label( value = '' )                                                                                                                                                                                                                      
+    tbox3 = widgets.Label( value = '' )                                                                                                                                                                                                                      
+
+    # misc buttons
+    reset_button = widgets.Button( description='Reset', disabled=False,button_style='',tooltip='',layout=widgets.Layout(width='98%') )
+    keep_xscale = widgets.Checkbox( value = False , description = 'Fixed int.' , disabled=False, indent=False )
+    show_ranges = widgets.Checkbox( value = True , description = 'Units' , disabled=False, indent=False )
+
+
+    # naviation: main slider (top)
+    smid = widgets.IntSlider(min=scope_epoch_sec/2, max=nsecs_clk - scope_epoch_sec/2, value=scope_epoch_sec/2, step=30, description='', readout=False,layout=widgets.Layout(width='100%') )
+        
+    # left panel buttons: interval width
+    swid_label = widgets.Label( value = 'Width' )
+    swid_dec_button = widgets.Button( description='<', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+    swid = widgets.Label( value = '30' )
+    swid_inc_button = widgets.Button( description='>', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+
+    # left panel buttons: left/right advances
+    epoch_label = widgets.Label( value = 'Epoch' )
+    epoch_dec_button = widgets.Button( description='<', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+    epoch = widgets.Label( value = '1' )
+    epoch_inc_button = widgets.Button( description='>', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+
+    # left panel buttons: Y-spacing
+    yspace_label = widgets.Label( value = 'Space' )
+    yspace_dec_button = widgets.Button( description='<', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+    yspace = widgets.Label( value = '1' )
+    yspace_inc_button = widgets.Button( description='>', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+
+    # left panel buttons: Y-scaling
+    yscale_label = widgets.Label( value = 'Scale' )
+    yscale_dec_button = widgets.Button( description='<', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+    yscale = widgets.Label( value = '0' )
+    yscale_inc_button = widgets.Button( description='>', disabled=False,button_style='',tooltip='', layout=widgets.Layout(width='30px'))
+
+
+    # --------------------- signal plotter (g)
+
+    # traces (xNS), gaps(x1), labels (xNS), annots(xNA), clock-ticks(x1)
+    fig = [go.Scatter(x = None, 
+                      y = None, 
+                      mode = 'lines',
+                      line=dict(color=palette[sig], width=1),
+                      hoverinfo='none',
+                      name = sig ) for sig in sigs
+    ] + [ go.Scatter( x = None , y = None ,
+                      mode = 'lines' ,
+                      fill='toself' ,
+                      fillcolor='#223344',
+                      line=dict(color='#888888', width=1),
+                      hoverinfo='none',
+                      name='Gap' ) 
+    ] + [ go.Scatter( x = None , y = None ,
+                      mode='text' ,
+                      textposition='middle right',
+                      textfont=dict(
+                          size=11,
+                          color='white'),
+                      hoverinfo='none' ,
+                      showlegend=False ) for sig in sigs 
+    ] + [ go.Scatter( x = None , 
+                      y = None , 
+                      mode = 'lines',
+                      fill='toself',
+                      line=dict(color=apalette[ann], width=1),
+                      hoverinfo='none',
+                      name = ann ) for ann in anns
+    ] + [ go.Scatter( x = None , y = None ,
+                      mode = 'text' ,
+                      textposition='bottom right',
+                      textfont=dict(
+                          size=11,
+                          color='white'),
+                      hoverinfo='none' ,
+                      showlegend=False ) ] 
+
+    
+    layout = go.Layout( margin=dict(l=8, r=8, t=0, b=0),
+                        yaxis=dict(range=[0,1]),
+                        modebar={'orientation': 'v','bgcolor': '#E9E9E9','color': 'white','activecolor': 'white' },
+                        yaxis_visible=False, 
+                        yaxis_showticklabels=False,
+                        xaxis_visible=False,
+                        xaxis_showticklabels=False,
+                        autosize=True, 
+                        height=height,
+                        plot_bgcolor='rgb(02,15,50)' ) 
+
+    g = go.FigureWidget(data=fig, layout= layout )
+    g._config = g._config | {'displayModeBar': False}
+    #g.update_xaxes(showgrid=True, gridwidth=0.1, gridcolor='#445555')
+    g.update_xaxes(showgrid=False)
+    g.update_yaxes(showgrid=False)
+    
+    
+    # -------------------- segment-plotter (sg)
+
+    num_epochs = ss.num_epochs()
+    tscale = ss.get_time_scale()
+    tstarts = [ tscale[idx] for idx in range(0,len(tscale),2)]
+    tstops = [ tscale[idx] for idx in range(1,len(tscale),2)]
+    times = np.concatenate((tstarts, tstops), axis=1)
+
+    # upper/lower boxes, then frame select, then actual segs
+    sfig = [ go.Scatter(x=[0,0],y=[0.05,0.05],
+                        mode='markers+lines',
+                        marker=dict(color="navy",size=8)) 
+            ] + [ go.Scatter(x=[0,0],y=[0.95,0.95],
+                        mode='markers+lines',
+                        marker=dict(color="navy",size=8))                             
+            ] + [ go.Scatter(x=[0,0,0,0,0,None],y=[0,0,1,1,0,None],
+                        mode='lines',
+                        fill='toself',
+                        fillcolor = 'rgba( 18, 65, 92, 0.75)' ,
+                        line=dict(color="red",width=0.5)) 
+            ] + [ go.Scatter(x=[x[1],x[1],x[3],x[3]],y=[0,1,1,0],   # was 0 1 3 2 
+                        fill="toself",
+                        mode = 'lines',
+                        hoverinfo = 'none',
+                        line=dict(color='rgb(19,114,38)', width=1), ) for x in times ]
+
+    slayout = go.Layout( margin=dict(l=8, r=8, t=2, b=4),
+                         showlegend=False,
+                         xaxis=dict(range=[0,1]),
+                         yaxis=dict(range=[0,1]),
+                         yaxis_visible=False, 
+                         yaxis_showticklabels=False,
+                         xaxis_visible=False, 
+                         xaxis_showticklabels=False,                         
+                         autosize=True, 
+                         height=15,
+                         plot_bgcolor='rgb(255,255,255)' ) 
+
+    sg = go.FigureWidget( data=sfig, layout=slayout )
+    sg._config = sg._config | {'displayModeBar': False}
+
+    # --------------------- hypnogram-level summary
+
+    stgs = [ 'N1' , 'N2' , 'N3' , 'R' , 'W' , '?' , 'L' ]
+    stgcols = { 'N1':'rgba(32, 178, 218, 1)' , 'N2':'blue', 'N3':'navy','R':'red','W':'green','?':'gray','L':'yellow' }
+    stgns = { 'N1':-1 , 'N2':-2, 'N3':-3,'R':0,'W':1,'?':2,'L':2 }
+
+    # clock-time stage info
+    stg_evts = p.fetch_annots( stgs ) 
+    if len( stg_evts ) != 0:
+         stg_evts2 = stg_evts.copy()
+         stg_evts2[ 'Start' ] = stg_evts2[ 'Stop' ]
+         stg_evts = pd.concat( [stg_evts2, stg_evts] )
+         stg_evts = stg_evts.sort_values(by=['Start', 'Class'])
+         times = stg_evts['Start'].to_numpy()    
+         ys = [ stgns[c] for c in stg_evts['Class'].tolist() ]
+         cols = [ stgcols[c] for c in stg_evts['Class'].tolist() ]
+    else:
+        times = None
+        ys = None
+        cols = None
+        
+    hypfig = [ go.Scatter( x = times, y=ys, mode='lines', line=dict(color='gray')) ]  
+    
+    hypfig.append( go.Scatter(x = times, 
+                              y = ys , 
+                              mode = 'markers' , 
+                              marker=dict( color = cols , size=2),
+                              hoverinfo='none' )  )
+    
+    hyplayout =  go.Layout( margin=dict(l=8, r=8, t=0, b=0),
+                            showlegend=False,
+                            xaxis=dict(range=[0,nsecs_clk]),
+                            yaxis=dict(range=[-4,3]),
+                            yaxis_visible=False, 
+                            yaxis_showticklabels=False,
+                            xaxis_visible=False, 
+                            xaxis_showticklabels=False,
+                            autosize=True, 
+                            height=35,
+                            plot_bgcolor='rgb(255,255,255)' ) 
+         
+    hypg = go.FigureWidget( data = hypfig , layout = hyplayout )
+    hypg._config = hypg._config | {'displayModeBar': False}
+
+
+    # --------------------- band power/spectrogram (bg)
+    
+    #bfig = go.Heatmap( z = None , type = 'heatmap',  colorscale = 'RdBu_r', showscale = False , hoverinfo = 'none' )
+    bfig = go.Heatmap( z = None , type = 'heatmap',  colorscale = 'turbo', showscale = False , hoverinfo = 'none' )
+    
+    blayout = go.Layout( margin=dict(l=8, r=8, t=0, b=0),
+                         modebar={'orientation': 'h','bgcolor': '#E9E9E9','color': 'white','activecolor': 'white' },
+                         showlegend=False,
+                         yaxis_visible=False, 
+                         yaxis_showticklabels=False,
+                         xaxis_visible=False, 
+                         xaxis_showticklabels=False,
+                         autosize=True,                          
+                         height=50,
+                         plot_bgcolor='rgb(255,255,255)' ) 
+    
+    bg = go.FigureWidget( bfig , blayout )
+    bg._config = bg._config | {'displayModeBar': False}
+
+
+    # --------------------- build overall box (containerP)
+
+    # ----- containers - left panel
+
+    ctr_lab_container = widgets.VBox(children=[ swid_label , epoch_label, yspace_label , yscale_label  ] ,
+                                     layout = widgets.Layout( width='30%', align_items='center' , display='flex', flex_flow='column' ) )
+                                 
+    ctr_dec_container = widgets.VBox(children=[ swid_dec_button , epoch_dec_button, yspace_dec_button , yscale_dec_button  ] ,
+                                     layout = widgets.Layout( width='20%', align_items='center' , display='flex', flex_flow='column' ))
+                                 
+    ctr_val_container = widgets.VBox(children=[ swid , epoch , yspace , yscale  ] ,
+                                     layout = widgets.Layout( width='30%', align_items='center' , display='flex', flex_flow='column' ))
+                                 
+    ctr_inc_container = widgets.VBox(children=[ swid_inc_button ,  epoch_inc_button, yspace_inc_button , yscale_inc_button ] ,
+                                     layout = widgets.Layout( width='20%', align_items='center' , display='flex', flex_flow='column' ))
+
+    # left panel: group top set of widgets
+    ctr_container = widgets.VBox( children=[ tbox, widgets.HBox(children=[ ctr_lab_container, ctr_dec_container, ctr_val_container, ctr_inc_container ] ) , reset_button ] ,
+                                  layout = widgets.Layout( width='100%' ) )
+
+    # left panel: lower buttons
+    lower_buttons = widgets.HBox( children=[ keep_xscale , show_ranges ] ,
+                                  layout = widgets.Layout( width='100%' ) )
+
+    # left panel: construct all
+    left_panel = widgets.VBox(children=[ ctr_container,
+                                         chlab, chbox,
+                                         widgets.HBox( children = [ band_hjorth_sel, pow_sel ] ),
+                                         anlab, anbox, a1lab, ansel, a1box,
+                                         lower_buttons ] ,
+                              layout = widgets.Layout( width='95%' , margin='0 0 0 5px' , overflow_x = 'hidden' ) )
+
+    # right panel: combine plots
+    containerS = widgets.VBox(children=[ smid , hypg, sg, bg, g ] , layout = widgets.Layout( width='95%' , margin='0 5px 0 5px' , overflow_x = 'hidden' ) )
+    
+    # make the final app (just join left+right panels)
+    container_app = AppLayout(header=None,
+                              left_sidebar=left_panel,
+                              center=containerS,
+                              right_sidebar=None,
+                              pane_widths=[1, 8, 0],
+                              align_items = 'stretch' ,
+                              footer=None , layout = widgets.Layout( border='3px none #708090' , margin='10px 5px 10px 5px' , overflow_x = 'hidden' ) )
+
+    
+    # --------------------- callback functions
+        
+    def redraw():
+
+        # update hms message
+        tbox.value = 'T: ' + ss.get_window_left_hms() + ' - ' + ss.get_window_right_hms()
+
+        # get annots
+        ss.compile_windowed_annots( anbox.value )
+ 
+        x1 = ss.get_window_left()
+        x2 = ss.get_window_right()
+
+        # update pointers on segment plot
+        s1 = x1 / nsecs_clk
+        s2 = x2 / nsecs_clk
+        sg.data[0].x = [ s1, s2 ]
+        sg.data[1].x = [ s1, s2 ]
+        sg.data[2].x = [ s1 , s2 , s2 , s1 , s1 , None ]
+
+        # update main plot
+        with g.batch_update():
+            ns = len(sigs)
+            na = len(anns)
+
+            # axes
+            g.update_xaxes(range = [x1,x2])
+            
+            # signals (0)
+            selected = [ x in chbox.value for x in sigs ]
+            idx=0
+            for i in list(range(0,ns)):
+                if selected[i] is True:
+                    g.data[i].x = ss.get_timetrack( sigs[i] )
+                    g.data[i].y = ss.get_scaled_signal( sigs[i] , idx )
+                    g.data[i].visible = True
+                    idx += 1
+                else:
+                    g.data[i].visible = False
+
+            # gaps (last trace)
+            gidx = ns
+            gaps = list( ss.get_gaps() )
+            if len(gaps) == 0:
+                g.data[ gidx ].visible = False
+            else:
+                # make into 6-value formats
+                xgaps = [(a, b, b, a, a, None ) for a, b in gaps ]
+                ygaps = [(0, 0, 1-header_height, 1-header_height, 0, None ) for a, b in gaps ]
+                g.data[ gidx ].x = [x for sub in xgaps for x in sub]
+                g.data[ gidx ].y = [y for sub in ygaps for y in sub]
+                g.data[ gidx ].visible = True
+
+            # ranges? (+ns)
+            if show_ranges.value is True:
+                idx=0
+                xl = x1 + (x2-x1 ) * 0.01 
+                for i in list(range(0,ns)):
+                    if selected[i] is True:
+                        ylim = ss.get_window_phys_range( sigs[i] )
+                        ylab = sigs[i] + ' ' + str(round(ylim[0],3)) + ':' + str(round(ylim[1],3)) + ' (' + units[sigs[i]] +')'
+                        g.data[i+ns+1].x = [ xl ]
+                        g.data[i+ns+1].y = [ ss.get_ylabel( idx ) * (1 - header_height ) ]
+                        g.data[i+ns+1].text = [ ylab ]
+                        g.data[i+ns+1].visible = True
+                        idx += 1
+                    else:
+                        g.data[i+ns+1].visible = False
+ 
+
+            # annots (+2ns + gap)
+            ns2 = 2 * ns + 1
+            selected = [ x in anbox.value for x in anns ]
+            for i in list(range(0,na)):
+                if selected[i] is True:
+                    g.data[i+ns2].x = ss.get_annots_xaxes( anns[i] )
+                    g.data[i+ns2].y = ss.get_annots_yaxes( anns[i] )
+                    g.data[i+ns2].visible = True
+                else:
+                    g.data[i+ns2].visible = False
+
+            # clock-ticks
+            gidx = 2 * ns + na + 1
+            tks = ss.get_clock_ticks(6)
+            tx = list( tks.keys() )
+            tv = list( tks.values() )
+            if len( tx ) == 0:
+                g.data[ gidx ].visible = False
+            else:
+                g.data[ gidx ].x = tx 
+                g.data[ gidx ].y = [ 1 - header_height + ( header_height ) * 0.5 for x in tx ]
+                g.data[ gidx ].text = tv
+                g.data[ gidx ].visible = True
+
+    def rescale(change):
+        ss.set_scaling( len(chbox.value) , len( anbox.value) , 2**float(yscale.value) , float(yspace.value) , header_height, footer_height , annot_height )
+        redraw()
+    
+    def update_bandpower(change):
+        if type( pow_sel.value ) is None: return 
+        if len( pow_sel.value ) == 0: return
+        if band_hjorth_sel.value is True:
+           S = np.transpose( ss.get_hjorths( pow_sel.value ) )
+           S = np.asarray(S,dtype=object)
+           S[np.isnan(S.astype(np.float_))] = None
+           bg.update_traces({'z': S } , selector = {'type':'heatmap'} )
+        else:
+           S = np.transpose( ss.get_bands( pow_sel.value ) )
+           S = np.asarray(S,dtype=object)
+           S[np.isnan(S.astype(np.float_))] = None
+           bg.update_traces({'z': S } , selector = {'type':'heatmap'} )
+
+    def pop_a1(change):
+        a1box.options = ss.get_all_annots( ansel.value )
+
+    def a1_win(change):
+        # format <annot> | t1-t2 (seconds)
+        # allow for pipe in <annot> name
+        nwin = a1box.value.split( '| ')[-1]
+        nwin = nwin.split('-')
+        nwin = [ float(x) for x in nwin ]
+
+        # center on mid of annot
+        mid = nwin[0] + ( nwin[1] - nwin[0] ) / 2
+
+        # width: either based on annot, or keep as is
+        if keep_xscale.value is False:
+            swid.unobserve(set_window_from_sliders, names="value")
+            swid.value = str( round( nwin[1] - nwin[0] , 2 ) )
+            swid.observe(set_window_from_sliders, names="value")
+            
+        # update smid, and trigger redraw via set_window_from_sliders()
+        smid.value = mid
+
+    def set_window_from_sliders(change):
+        w = float( swid.value )
+        p1 = smid.value - 0.5 * w
+        if p1 < 0: p1 = 0
+        p2 = p1 + w
+        if p2 >= ss.num_seconds_clocktime():
+            p2 = ss.num_seconds_clocktime() - 1 
+        ss.window( p1 , p2 )
+        epoch.value = str(1+int(smid.value/30))
+        redraw()
+
+    def fn_reset(b):
+        swid.value = str( 30 )
+        yspace.value = str( 1 )
+        yscale.value = str( 0 )
+                
+    def fn_dec_epoch(b):
+        if ( smid.value - scope_epoch_sec ) >= smid.min :
+            smid.value = smid.value - scope_epoch_sec
+
+    def fn_inc_epoch(b):
+        if ( smid.value + scope_epoch_sec ) <= smid.max :
+            smid.value = smid.value + scope_epoch_sec
+        
+    def fn_dec_swid(b):
+        swid_var = float( swid.value )
+        if swid_var > 3.5: swid_var = swid_var / 2
+        if swid_var > 100: swid.value = str( int( swid_var ))
+        else: swid.value = str( swid_var )
+
+    def fn_inc_swid(b):
+        swid_var = float( swid.value )
+        if swid_var < 40000: swid_var = swid_var * 2
+        if swid_var > 100: swid.value = str( int( swid_var ) )
+        else: swid.value = str( swid_var )
+
+    def fn_yspace_dec(b):
+        yspace_var = float( yspace.value )
+        if yspace_var > 0.05: yspace_var = yspace_var - 0.1
+        yspace.value = str( round( yspace_var , 1 ) )
+
+    def fn_yspace_inc(b):
+        yspace_var = float( yspace.value )
+        if yspace_var < 0.95: yspace_var = yspace_var + 0.1
+        yspace.value = str( round( yspace_var , 1 ) )
+        
+    def fn_yscale_dec(b):
+        yscale_var = float( yscale.value )
+        if yscale_var > -2: yscale_var = yscale_var - 0.2
+        yscale.value = str( round( yscale_var , 1 ) )
+
+    def fn_yscale_inc(b):
+        yscale_var = float( yscale.value )
+        if yscale_var < 2: yscale_var = yscale_var + 0.2
+        yscale.value = str( round( yscale_var , 1 ) )
+
+    def fn_hjorth_band(b):
+        if band_hjorth_sel.value is True:
+           pow_sel.options = hsigs
+        else:
+           pow_sel.options = bsigs
+        
+    # --------------------- hook up widgets
+
+    # observers
+    smid.observe(set_window_from_sliders, names="value")
+    swid.observe(set_window_from_sliders, names="value")
+
+    show_ranges.observe(set_window_from_sliders)
+
+    band_hjorth_sel.observe( fn_hjorth_band )
+    
+    swid_dec_button.on_click(fn_dec_swid)
+    swid_inc_button.on_click(fn_inc_swid)
+
+    epoch_dec_button.on_click(fn_dec_epoch)
+    epoch_inc_button.on_click(fn_inc_epoch)
+
+    reset_button.on_click(fn_reset)
+                          
+    # summaries
+    pow_sel.observe(update_bandpower,names="value")
+
+    # rescale plots
+    yscale_dec_button.on_click( fn_yscale_dec )
+    yscale_inc_button.on_click( fn_yscale_inc )
+    yspace_dec_button.on_click( fn_yspace_dec )
+    yspace_inc_button.on_click( fn_yspace_inc )
+
+    yscale.observe( rescale , names="value")
+    yspace.observe( rescale , names="value")
+    
+
+    # channel selection
+    chbox.observe( rescale ,names="value")
+
+    # annots
+    anbox.observe( rescale , names="value")
+    ansel.observe( pop_a1 , names="value")
+    a1box.observe( a1_win , names="value")
+
+    
+    # ---------------------  display
+    update_bandpower(None)
+    ss.set_scaling( len(chbox.value) , len( anbox.value) , 2**float(yscale.value) , float(yspace.value) , header_height, footer_height , annot_height )
+
+    return container_app
+
+
+
```

## Comparing `lunapi-0.0.7.dist-info/METADATA` & `lunapi-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python interface to the Luna toolset for sleep signal analysis
 Keywords: Sleep,EEG,PSG,Luna,Signal processing
 Author-Email: Shaun Purcell <smpurcell@bwh.harvard.edu>, Senthil Palanivelu <spalanivelu@mgh.harvard.edu>, Nataliia Kozhemiako <nkozhemiako@bwh.harvard.edu>
 Maintainer-Email: Senthil Palanivelu <spalanivelu@mgh.harvard.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Project-URL: Www, https://zzz.bwh.harvard.edu/luna
 Project-URL: Github, http://github.com/remnrem/luna-api
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: IPython
 Description-Content-Type: text/markdown
```

## Comparing `lunapi-0.0.7.dist-info/RECORD` & `lunapi-0.0.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lunapi-0.0.7.dist-info/METADATA,sha256=JEB8OaQtY1eJSw_cP8QK1506x0oCPDnvQKo5dbF8Ssc,1350
-lunapi-0.0.7.dist-info/RECORD,,
-lunapi-0.0.7.dist-info/WHEEL,sha256=cyka432ivP0ubIngQuqcegb6o2uOP74f8QTnJ39n61U,165
-lunapi-0.0.7.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-lunapi/lunapi0.cpp,sha256=Wjyd7Js_kjwGSEJGTlSjlvjzuhDTqLRcXQRIu-pFdhI,9947
-lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so,sha256=iwMi5Urjs-6UlCERj17PKErFRVOZO4okQKDqkm-Dq7k,27300736
-lunapi/lunapi1.py,sha256=1mQLyIQA9Kolt1R5yx4H3WBON7wr3c870273zJ5cp1o,48099
 lunapi/__init__.py,sha256=cDep9d2N4KKUt81AzHUyFsuRdGwxCD1rqqFmptsAqsk,352
+lunapi/lunapi1.py,sha256=NwOdZFTrVfP5sDIKGSu-m-C4hqhhgWGcq8iuRvspht0,84530
+lunapi/lunapi0.pypy39-pp73-darwin.so,sha256=zfwxCpW9ozuzU7fTP_ae8Mgi2RAXTuVtYCUHaasJ9xQ,15223136
+lunapi/lunapi0.cpp,sha256=BCVMWAyJNKM8mnUFU7yRioH2TGyph5iIt85wxBE8kKo,12728
+lunapi-0.0.8.dist-info/RECORD,,
+lunapi-0.0.8.dist-info/WHEEL,sha256=-Y2h0TzuVqnBMpOSwPGoQau9oUtTW_que8PUWHln_Ow,118
+lunapi-0.0.8.dist-info/METADATA,sha256=7vt4VzSaunOqZbnuM5ilDWoDAg8eFvqU5-qh2cXIroU,1350
+lunapi-0.0.8.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
```

## Comparing `lunapi-0.0.7.dist-info/licenses/LICENSE` & `lunapi-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

