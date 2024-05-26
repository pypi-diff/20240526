# Comparing `tmp/CI_CloudConnector-0.8.zip` & `tmp/CI_CloudConnector-0.9.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 9411 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     5358 b- defN 16-Dec-13 08:05 CI_CloudConnector-0.8/CI_CloudConnector.py
--rw-rw-rw-  2.0 fat    24978 b- defN 16-Dec-13 08:07 CI_CloudConnector-0.8/CI_LC_BL.py
--rw-rw-rw-  2.0 fat      304 b- defN 16-Dec-13 08:07 CI_CloudConnector-0.8/PKG-INFO
--rw-rw-rw-  2.0 fat     2231 b- defN 16-Dec-07 15:42 CI_CloudConnector-0.8/README.txt
--rw-rw-rw-  2.0 fat      402 b- defN 16-Dec-13 08:07 CI_CloudConnector-0.8/setup.py
-5 files, 33273 bytes uncompressed, 8675 bytes compressed:  73.9%
+Zip file size: 9433 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     5482 b- defN 16-Dec-13 08:17 CI_CloudConnector-0.9/CI_CloudConnector.py
+-rw-rw-rw-  2.0 fat    24935 b- defN 16-Dec-13 08:17 CI_CloudConnector-0.9/CI_LC_BL.py
+-rw-rw-rw-  2.0 fat      304 b- defN 16-Dec-13 08:17 CI_CloudConnector-0.9/PKG-INFO
+-rw-rw-rw-  2.0 fat     2231 b- defN 16-Dec-07 15:42 CI_CloudConnector-0.9/README.txt
+-rw-rw-rw-  2.0 fat      402 b- defN 16-Dec-13 08:17 CI_CloudConnector-0.9/setup.py
+5 files, 33354 bytes uncompressed, 8697 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: CI_CloudConnector-0.8/CI_CloudConnector.py
+Filename: CI_CloudConnector-0.9/CI_CloudConnector.py
 Comment: 
 
-Filename: CI_CloudConnector-0.8/CI_LC_BL.py
+Filename: CI_CloudConnector-0.9/CI_LC_BL.py
 Comment: 
 
-Filename: CI_CloudConnector-0.8/PKG-INFO
+Filename: CI_CloudConnector-0.9/PKG-INFO
 Comment: 
 
-Filename: CI_CloudConnector-0.8/README.txt
+Filename: CI_CloudConnector-0.9/README.txt
 Comment: 
 
-Filename: CI_CloudConnector-0.8/setup.py
+Filename: CI_CloudConnector-0.9/setup.py
 Comment: 
 
 Zip file comment:
```

## Comparing `CI_CloudConnector-0.8/CI_CloudConnector.py` & `CI_CloudConnector-0.9/CI_CloudConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         #to prevent upgrading to much in case of a problem we count upgrade attempts and stop when its too big, but if the version changes we try again
         if serverVersion != updateToVer:
             serverVersion = updateToVer
             upgradeCounter = 0
 
         CI_LC_BL.ci_print ("local ver=" + localVer)
         CI_LC_BL.ci_print ("server ver= " + updateToVer)
+
+        now = datetime.datetime.now()
+        print now + ">>" + "local ver=" + localVer + "server ver= " + updateToVer
         if str(updateToVer)=='None':
             updateToVer=''
         if (bool(updateToVer!='') & bool(updateToVer!=localVer) & bool(upgradeCounter<10)):
             upgradeCounter = upgradeCounter + 1
             CI_LC_BL.ci_print('Local Version is different than server suggested version, start auto upgrade from:' + localVer + ' To:' + updateToVer + ' Upgrade count:'+str(upgradeCounter))
             upgradeLC()
             reloadLC()
```

## Comparing `CI_CloudConnector-0.8/CI_LC_BL.py` & `CI_CloudConnector-0.9/CI_LC_BL.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #config
 cfg_serverAddress = ''
 cfg_userName = ''
 cfg_passWord = ''
 cfg_plcMode = ''
         
 #VER = pkg_resources.require("CI_LocalConnector")[0].version
-VER = '0.8'
+VER = '0.9'
 sugestedUpdateVersion = ''
 configFile = 'config.ini'
 ScanRateLastRead = {}
 currentToken=''
 g_connectorTypeName = ''
 
 # ============================
@@ -199,15 +199,14 @@
         #    ci_print("Skipping getCloudVersion - no Token")
         #    return ""            
         #else:
         #    ci_print('Got Token Using Bearer auth')
         #    response = requests.get(url,
         #                            data = None,
         #                            headers={'Authorization': 'bearer %s' % token})
-        print "====" + str(response.text)
         ci_print ('gettags response=' + response.text)
         ans = json.loads(response.text)
         updateToVersion = ans[0]
         serverTime = ans[1]
         #ci_print (serverTime)
         
         sugestedUpdateVersion = updateToVersion
```

## Comparing `CI_CloudConnector-0.8/README.txt` & `CI_CloudConnector-0.9/README.txt`

 * *Files identical despite different names*

