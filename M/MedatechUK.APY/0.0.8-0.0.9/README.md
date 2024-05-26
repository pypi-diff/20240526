# Comparing `tmp/MedatechUK.APY-0.0.8.tar.gz` & `tmp/MedatechUK.APY-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedatechUK.APY-0.0.8.tar", last modified: Sun May 29 11:47:33 2022, max compression
+gzip compressed data, was "MedatechUK.APY-0.0.9.tar", last modified: Wed Jun  1 16:25:58 2022, max compression
```

## Comparing `MedatechUK.APY-0.0.8.tar` & `MedatechUK.APY-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-05-29 11:47:33.393984 MedatechUK.APY-0.0.8/
--rw-rw-rw-   0        0        0     3147 2022-05-29 11:47:33.395959 MedatechUK.APY-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2490 2022-05-29 11:42:38.000000 MedatechUK.APY-0.0.8/README.md
--rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 MedatechUK.APY-0.0.8/licence
--rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 MedatechUK.APY-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      728 2022-05-29 11:47:33.405960 MedatechUK.APY-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-29 11:47:33.052941 MedatechUK.APY-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-05-29 11:47:33.283954 MedatechUK.APY-0.0.8/src/MedatechUK/
--rw-rw-rw-   0        0        0      415 2022-05-19 11:19:47.000000 MedatechUK.APY-0.0.8/src/MedatechUK/PriDate.py
--rw-rw-rw-   0        0        0    15224 2022-05-25 14:42:13.000000 MedatechUK.APY-0.0.8/src/MedatechUK/Serial.py
--rw-rw-rw-   0        0        0        0 2022-05-19 11:19:46.000000 MedatechUK.APY-0.0.8/src/MedatechUK/__init__.py
--rw-rw-rw-   0        0        0    18084 2022-05-23 07:05:49.000000 MedatechUK.APY-0.0.8/src/MedatechUK/apy.py
--rw-rw-rw-   0        0        0     2466 2022-05-20 09:05:43.000000 MedatechUK.APY-0.0.8/src/MedatechUK/mLog.py
--rw-rw-rw-   0        0        0     4969 2022-05-20 05:24:23.000000 MedatechUK.APY-0.0.8/src/MedatechUK/oDataConfig.py
--rw-rw-rw-   0        0        0    19155 2022-05-19 11:19:46.000000 MedatechUK.APY-0.0.8/src/MedatechUK/odata.py
-drwxrwxrwx   0        0        0        0 2022-05-29 11:47:33.372959 MedatechUK.APY-0.0.8/src/MedatechUK.APY.egg-info/
--rw-rw-rw-   0        0        0     3147 2022-05-29 11:47:30.000000 MedatechUK.APY-0.0.8/src/MedatechUK.APY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2022-05-29 11:47:33.000000 MedatechUK.APY-0.0.8/src/MedatechUK.APY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-29 11:47:31.000000 MedatechUK.APY-0.0.8/src/MedatechUK.APY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-05-29 11:47:32.000000 MedatechUK.APY-0.0.8/src/MedatechUK.APY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-06-01 16:25:58.037775 MedatechUK.APY-0.0.9/
+-rw-rw-rw-   0        0        0     3147 2022-06-01 16:25:58.037775 MedatechUK.APY-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2490 2022-05-29 11:42:38.000000 MedatechUK.APY-0.0.9/README.md
+-rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 MedatechUK.APY-0.0.9/licence
+-rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 MedatechUK.APY-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      728 2022-06-01 16:25:58.039776 MedatechUK.APY-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-06-01 16:25:57.948774 MedatechUK.APY-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-06-01 16:25:58.009775 MedatechUK.APY-0.0.9/src/MedatechUK/
+-rw-rw-rw-   0        0        0      415 2022-05-19 11:19:47.000000 MedatechUK.APY-0.0.9/src/MedatechUK/PriDate.py
+-rw-rw-rw-   0        0        0    16566 2022-06-01 14:28:29.000000 MedatechUK.APY-0.0.9/src/MedatechUK/Serial.py
+-rw-rw-rw-   0        0        0        0 2022-05-19 11:19:46.000000 MedatechUK.APY-0.0.9/src/MedatechUK/__init__.py
+-rw-rw-rw-   0        0        0    18084 2022-05-23 07:05:49.000000 MedatechUK.APY-0.0.9/src/MedatechUK/apy.py
+-rw-rw-rw-   0        0        0     7495 2022-06-01 13:47:10.000000 MedatechUK.APY-0.0.9/src/MedatechUK/epdm.py
+-rw-rw-rw-   0        0        0     2466 2022-05-20 09:05:43.000000 MedatechUK.APY-0.0.9/src/MedatechUK/mLog.py
+-rw-rw-rw-   0        0        0     5119 2022-05-30 10:26:07.000000 MedatechUK.APY-0.0.9/src/MedatechUK/oDataConfig.py
+-rw-rw-rw-   0        0        0    19155 2022-05-19 11:19:46.000000 MedatechUK.APY-0.0.9/src/MedatechUK/odata.py
+drwxrwxrwx   0        0        0        0 2022-06-01 16:25:58.033776 MedatechUK.APY-0.0.9/src/MedatechUK.APY.egg-info/
+-rw-rw-rw-   0        0        0     3147 2022-06-01 16:25:57.000000 MedatechUK.APY-0.0.9/src/MedatechUK.APY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2022-06-01 16:25:57.000000 MedatechUK.APY-0.0.9/src/MedatechUK.APY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-01 16:25:57.000000 MedatechUK.APY-0.0.9/src/MedatechUK.APY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2022-06-01 16:25:57.000000 MedatechUK.APY-0.0.9/src/MedatechUK.APY.egg-info/top_level.txt
```

### Comparing `MedatechUK.APY-0.0.8/PKG-INFO` & `MedatechUK.APY-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedatechUK.APY
-Version: 0.0.8
+Version: 0.0.9
 Summary: MedatechUK Python API for Priority oData
 Home-page: https://github.com/MedatechUK/Medatech.APY
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.APY/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `MedatechUK.APY-0.0.8/README.md` & `MedatechUK.APY-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MedatechUK.APY-0.0.8/licence` & `MedatechUK.APY-0.0.9/licence`

 * *Files identical despite different names*

### Comparing `MedatechUK.APY-0.0.8/setup.cfg` & `MedatechUK.APY-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6564 6174 6563 6855 4b2e 4150   = MedatechUK.AP
 00000020: 590d 0a76 6572 7369 6f6e 203d 2030 2e30  Y..version = 0.0
-00000030: 2e38 0d0a 6175 7468 6f72 203d 2053 696d  .8..author = Sim
+00000030: 2e39 0d0a 6175 7468 6f72 203d 2053 696d  .9..author = Sim
 00000040: 6f6e 2042 6172 6e65 7474 0d0a 6175 7468  on Barnett..auth
 00000050: 6f72 5f65 6d61 696c 203d 2073 6940 6d65  or_email = si@me
 00000060: 6461 7465 6368 756b 2e63 6f6d 0d0a 6465  datechuk.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4d65 6461  scription = Meda
 00000080: 7465 6368 554b 2050 7974 686f 6e20 4150  techUK Python AP
 00000090: 4920 666f 7220 5072 696f 7269 7479 206f  I for Priority o
 000000a0: 4461 7461 0d0a 6c6f 6e67 5f64 6573 6372  Data..long_descr
```

### Comparing `MedatechUK.APY-0.0.8/src/MedatechUK/Serial.py` & `MedatechUK.APY-0.0.9/src/MedatechUK/Serial.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,28 +138,34 @@
     #endregion
 
     #region "ctor"
     def __init__(self, form , **kwargs):
         self.form = form
         self.props = {}
         self.log = mLog() 
+
         for arg in kwargs.keys():  
-            if arg.upper() == 'XML':     
-                t = xmltodict.parse(kwargs[arg].read())           
-                self = self.__init__(**json.loads(json.dumps(t[list(t)[0]])))
+            if arg.upper() == '_XML':     
+                t = xmltodict.parse(kwargs[arg].read(),dict_constructor=dict)           
+                self = self.__init__(**json.loads(json.dumps(t[list(t)[0]]))) #
 
-            elif arg.upper() == 'JSON':
+            elif arg.upper() == '_JSON':
                 self = self.__init__(**json.loads(kwargs[arg].read()))
 
             elif ( hasattr( self , arg ) ) :
                 try:
                     setattr( self , arg , kwargs[arg] )
                 except:
                     pass
-    
+            elif ( hasattr( self , arg.lstrip('@') ) ) :
+                try:
+                    setattr( self , arg.lstrip('@') , kwargs[arg] )
+                except e:
+                    print(e)
+
     #endregion
 
     #region "Output Methods"
 
     def toFile(self, fn , method, **kwargs):
         self.log.logger.debug("Writing file [{}] {}".format( fn , method(**kwargs)))
         with open(fn, 'w') as the_file:            
@@ -176,35 +182,45 @@
         if isinstance(this, list):            
             for i in this:
                 ret += "<"+ type(i).__name__ +">"
                 ret +=self.toXML(i)    
                 ret += "</"+ type(i).__name__ +">"                                    
             
         else:
-            for key in this.__dict__ :                  
-                if (key != "_props" and key !="form" and key !="log"):                    
-                    if isinstance(this.__dict__[key], list):                              
-                        ret += self.toXML(this.__dict__[key])
-                    
-                    else:
-                        if(hasattr(this,"props")):                            
-                            ret += "<"+ key.lstrip('_') +">"+ str(this.__dict__[key]) +"</"+ key.lstrip('_') +">"
+            for p in range(3):
+                for key in this.__dict__ :                      
+                    if (key != "_props" and key !="form" and key !="log"):
+                        # print("{} {}".format(p,key))
+
+                        if isinstance(this.__dict__[key], list) and p==2:      
+                            ret += self.toXML(this.__dict__[key])
+
+                        elif hasattr(getattr(this , key), "props") and p==1:
+                            if(hasattr(this,"props")):                            
+                                ret += "<"+ key.lstrip('_') +">"+ self.toXML(this.__dict__[key]) +"</"+ key.lstrip('_') +">"
+                            
+                        elif p==0:
+                            if(hasattr(this,"props")) and this.props.__contains__(key.lstrip('_')):
+                                ret += "<"+ key.lstrip('_') +">"+ str(this.__dict__[key]) +"</"+ key.lstrip('_') +">"
                 
         if(l!=0):
             ret +=("</"+ root +">") 
             return parseString(ret).toprettyxml()            
         
         else:
             return ret
 
     def toJSON(self):        
         return json.dumps(self, default=lambda o: {
             key.lstrip('_'): 
-            value for key, value in o.__dict__.items() if key !="_props" and key !="form" and key !="log"}, 
-            sort_keys=False, indent=4)   
+            value for key, value in o.__dict__.items() if key !="_props" and key !="form" and key !="log"
+            }, 
+                sort_keys=False, 
+                indent=4
+        )   
 
     def toOdata(self , this = 0):         
         ret = ""  
         l = 0     
         if (this==0):            
             l = 1
             this = self
@@ -254,60 +270,72 @@
     def toFlatOdata(self , this = 0):         
         ret = ""  
         l = 0     
         if (this==0):            
             l = 1
             this = self
             ret +=("{ ") 
-            ret +=(this.props["bubbleid"].oData(this.form.bubbleid) )  + ", "            
-            ret +=(this.props["typename"].oData(this.form.typename) )  + ", " + chr(34) + "ZODA_LOAD_SUBFORM" + chr(34) + " : ["            
+            if self.form.fname == "ZODA_TRANS" :
+                ret +=(this.props["bubbleid"].oData(this.form.bubbleid) )  + ", "            
+                ret +=(this.props["typename"].oData(this.form.typename) )  + ", " + chr(34) + "ZODA_LOAD_SUBFORM" + chr(34) + " : ["            
 
         if isinstance(this, list):            
             for i in this:                               
-                ret +=self.toFlatOdata(i)    
-                ret += " } "            
-                if(this[-1]!=i):
-                    ret += (",")            
-            
+                ret += self.toFlatOdata(i)                              
+                if(this[-1]!=i) and ret[len(ret)-4:] != " } ,":
+                    ret += (" } ,")
+
         else:
             f = 0
             ret += " { "
             if(this.props.__contains__("rt")) :
                 if(f==0): 
                     f = 1
                 else :
                     ret +=(", ")
                 ret +=(this.props["rt"].oData(this.form.rt) ) 
             
-            for key in this.__dict__ :  
-                if (key != "_props" and key !="form" and key !="log"):
-                    if isinstance(this.__dict__[key], list):      
-                        ret+=" } ,"
-                        ret += self.toFlatOdata(this.__dict__[key])
-                    
-                    else:
-                        if(hasattr(this,"props")) and this.props.__contains__(key.lstrip('_')):
-                            if(f==0):
-                                f = 1
-                            else :
-                                ret +=(", ")
-                            ret +=(this.props[key.lstrip('_')].oData(this.__dict__[key]))                        
-            
             # Iterate through readonly properties
             for key in this.props:
                 if (key != "rt" and key !="bubbleid" and key !="typename"):
                     if not this.__dict__.__contains__("_" + key):
                         if(f==0):
                             f = 1
                         else :
                             ret +=(", ")
-                        ret +=(this.props[key.lstrip('_')].oData(getattr(this, key)))                  
+                        ret +=(this.props[key.lstrip('_')].oData(getattr(this, key))) 
+
+            for p in range(3):
+                for key in this.__dict__ :                      
+                    if (key != "_props" and key !="form" and key !="log"):
+                        # print("{} {}".format(p,key))
+
+                        if isinstance(this.__dict__[key], list) and p==2:      
+                            if ret[len(ret)-4:] != " } ,":
+                                ret+=" } ,"
+                            ret += self.toFlatOdata(this.__dict__[key])                            
+
+                        elif hasattr(getattr(this , key), "props") and p==1:
+                            if ret[len(ret)-4:] != " } ,":
+                                ret+=" } ,"
+                            ret += self.toFlatOdata(this.__dict__[key])
+                            
+                        elif p==0:
+                            if(hasattr(this,"props")) and this.props.__contains__(key.lstrip('_')):
+                                if(f==0):
+                                    f = 1
+                                else :
+                                    ret +=(", ")
+                                ret +=(this.props[key.lstrip('_')].oData(this.__dict__[key]))                                                 
                 
         if(l!=0):
-            ret += "] }"
+            if ret[len(ret)-4:] == " } ,":
+                ret=ret[0:len(ret)-4]  
+            
+            ret += " } ] }"
 
         return ret
     
     def toPri(self, config, method, **kwargs):            
         
         ## This function will PATCH a completion request ONLY
         ## if the fornname of the upper level is 'ZODA_TRANS'
@@ -340,15 +368,15 @@
         )
         res = r.getresponse()             
         if res.status == 201: # Created
             self.log.logger.debug("[{}] OK".format( res.status ))
 
             # If we're using the oData loading form, send a PATCH
             # to identify that all data has been sent.
-            if self.form.fname == 'ZODA_TRANS':
+            if self.form.fname != 'ZODA_TRANS':
                 self.log.logger.debug("[{}] {}".format( res.status , res.reason ))
                 ret.Status = res.status
                 ret.Message = res.reason
                 ret.data = json.load(res)
                 self.log.logger.debug("Result: {}".format( json.dumps(ret.data  , indent = 4 )))
 
             else:
@@ -380,24 +408,24 @@
 
                     elif res.getheader("Content-Type","").find("text/html") > -1:
                             ret.data = {"error": "Priority service not responding." }     
                             self.log.logger.critical("{}".format( "Priority service not responding." ))   
 
                     else:
                         # Create reponse from json 
-                        Response.data = json.load(res)  
-                        self.log.logger.critical( "{}".format( json.dumps(Response.data  , indent = 4 ) ) )
+                        ret.data = json.load(res)  
+                        self.log.logger.critical( "{}".format( json.dumps(ret.data , indent = 4 ) ) )
 
                 else:
                     ## Sucsess!
                     self.log.logger.debug("[{}] {}".format( res.status , res.reason ))
                     ret.Status = res.status
                     ret.Message = res.reason
                     ret.data = json.load(res)
-                    self.log.logger.debug("Result: {}".format( json.dumps(ret.data  , indent = 4 ) ))
+                    self.log.logger.debug("Result: {}".format( json.dumps(ret.data , indent = 4 ) ))
 
         else:   
             ret.Status = res.status
             ret.Message = "POST Failed: " + res.reason   
             self.log.logger.critical( "[{}] Fail: {}".format( res.status , res.reason ) )            
 
             # If the response is text, create a response with the text         
@@ -408,13 +436,13 @@
 
             elif res.getheader("Content-Type","").find("text/html") > -1:
                     ret.data = {"error": "Priority service not responding." }     
                     self.log.logger.critical("{}".format( "Priority service not responding." ))   
 
             else:
                 # Create reponse from json 
-                Response.data = json.load(res)  
-                self.log.logger.critical( "{}".format( json.dumps(Response.data  , indent = 4 ) ) )
+                ret.data = json.load(res)  
+                self.log.logger.critical( "{}".format( json.dumps(ret.data  , indent = 4 ) ) )
     
     #endregion
 
 #endregion
```

### Comparing `MedatechUK.APY-0.0.8/src/MedatechUK/apy.py` & `MedatechUK.APY-0.0.9/src/MedatechUK/apy.py`

 * *Files identical despite different names*

### Comparing `MedatechUK.APY-0.0.8/src/MedatechUK/mLog.py` & `MedatechUK.APY-0.0.9/src/MedatechUK/mLog.py`

 * *Files identical despite different names*

### Comparing `MedatechUK.APY-0.0.8/src/MedatechUK/oDataConfig.py` & `MedatechUK.APY-0.0.9/src/MedatechUK/oDataConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,8 +107,10 @@
                 if 'ODATAHOST' in line.split("=")[0].upper():
                     self.oDataHost = line.split("=")[1].split('"')[1]            
                 if 'TABULAINI' in line.split("=")[0].upper():
                     self.tabulaini = line.split("=")[1].split('"')[1]
                 if 'OUSER' in line.split("=")[0].upper():
                     self.ouser = line.split("=")[1].split('"')[1]
                 if 'OPASS' in line.split("=")[0].upper():
-                    self.opass = line.split("=")[1].split('"')[1]                                
+                    self.opass = line.split("=")[1].split('"')[1]                                
+                if 'CONNSTR' in line.split("=")[0].upper():
+                    self.connstr = line.split("=")[1].split('"')[1]
```

### Comparing `MedatechUK.APY-0.0.8/src/MedatechUK/odata.py` & `MedatechUK.APY-0.0.9/src/MedatechUK/odata.py`

 * *Files identical despite different names*

### Comparing `MedatechUK.APY-0.0.8/src/MedatechUK.APY.egg-info/PKG-INFO` & `MedatechUK.APY-0.0.9/src/MedatechUK.APY.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedatechUK.APY
-Version: 0.0.8
+Version: 0.0.9
 Summary: MedatechUK Python API for Priority oData
 Home-page: https://github.com/MedatechUK/Medatech.APY
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.APY/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

