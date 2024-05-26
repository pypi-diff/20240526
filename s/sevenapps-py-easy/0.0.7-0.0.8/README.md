# Comparing `tmp/sevenapps_py_easy-0.0.7.tar.gz` & `tmp/sevenapps_py_easy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenapps_py_easy-0.0.7.tar", last modified: Sat May 25 07:06:48 2024, max compression
+gzip compressed data, was "sevenapps_py_easy-0.0.8.tar", last modified: Sun May 26 10:27:52 2024, max compression
```

## Comparing `sevenapps_py_easy-0.0.7.tar` & `sevenapps_py_easy-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-25 07:06:48.473237 sevenapps_py_easy-0.0.7/
--rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.7/LICENSE
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-25 07:06:48.473163 sevenapps_py_easy-0.0.7/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      205 2024-05-24 22:50:51.000000 sevenapps_py_easy-0.0.7/README.md
--rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-25 07:06:48.473420 sevenapps_py_easy-0.0.7/setup.cfg
--rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-25 07:06:19.000000 sevenapps_py_easy-0.0.7/setup.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-25 07:06:48.470927 sevenapps_py_easy-0.0.7/sevenapps/
--rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.7/sevenapps/__init__.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-25 07:06:48.471606 sevenapps_py_easy-0.0.7/sevenapps/services/
--rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:01.000000 sevenapps_py_easy-0.0.7/sevenapps/services/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     6547 2024-05-25 07:05:57.000000 sevenapps_py_easy-0.0.7/sevenapps/services/google_firestore_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.7/sevenapps/services/google_services_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.7/sevenapps/services/selenium_connector.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-25 07:06:48.471890 sevenapps_py_easy-0.0.7/sevenapps/utils/
--rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:09.000000 sevenapps_py_easy-0.0.7/sevenapps/utils/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.7/sevenapps/utils/file_manager.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-25 07:06:48.472852 sevenapps_py_easy-0.0.7/sevenapps_py_easy.egg-info/
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-25 07:06:48.000000 sevenapps_py_easy-0.0.7/sevenapps_py_easy.egg-info/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      491 2024-05-25 07:06:48.000000 sevenapps_py_easy-0.0.7/sevenapps_py_easy.egg-info/SOURCES.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-25 07:06:48.000000 sevenapps_py_easy-0.0.7/sevenapps_py_easy.egg-info/dependency_links.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-25 07:06:48.000000 sevenapps_py_easy-0.0.7/sevenapps_py_easy.egg-info/requires.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-25 07:06:48.000000 sevenapps_py_easy-0.0.7/sevenapps_py_easy.egg-info/top_level.txt
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.399908 sevenapps_py_easy-0.0.8/
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.8/LICENSE
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-26 10:27:52.399846 sevenapps_py_easy-0.0.8/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      205 2024-05-24 22:50:51.000000 sevenapps_py_easy-0.0.8/README.md
+-rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-26 10:27:52.400098 sevenapps_py_easy-0.0.8/setup.cfg
+-rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-26 10:27:44.000000 sevenapps_py_easy-0.0.8/setup.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.398117 sevenapps_py_easy-0.0.8/sevenapps/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.8/sevenapps/__init__.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.398577 sevenapps_py_easy-0.0.8/sevenapps/services/
+-rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:01.000000 sevenapps_py_easy-0.0.8/sevenapps/services/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     8576 2024-05-26 10:26:51.000000 sevenapps_py_easy-0.0.8/sevenapps/services/google_firestore_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.8/sevenapps/services/google_services_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.8/sevenapps/services/selenium_connector.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.398797 sevenapps_py_easy-0.0.8/sevenapps/utils/
+-rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:09.000000 sevenapps_py_easy-0.0.8/sevenapps/utils/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.8/sevenapps/utils/file_manager.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.399562 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      491 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/requires.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/top_level.txt
```

### Comparing `sevenapps_py_easy-0.0.7/LICENSE` & `sevenapps_py_easy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.7/sevenapps/services/google_firestore_connector.py` & `sevenapps_py_easy-0.0.8/sevenapps/services/google_firestore_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         firestore_creds = firebase_admin.initialize_app(
             credentials.Certificate(self.credentials_file_path),
             name=self.creds_id
         )
         return firestore.client(app=firestore_creds)
 
-
+    # Enviando un path estilo así 'collection1/document1/collection2/document2' y enviando la key del interior del doc puedes recuperar datos
     def get_data_by_path(self, path: str, data_target: str):
         """
         Obtiene datos de un documento específico dentro de una base de datos siguiendo una ruta dada.
 
         La ruta debe especificar alternadamente colecciones y documentos, comenzando con una colección.
         Por ejemplo: 'collection1/document1/collection2/document2'.
 
@@ -97,14 +97,62 @@
 
         # Imprimimos mensaje para avisar de que se está descargando
         print(f'[get_data_by_path()]: Descargando la información de "{path}/{data_target}"...\n', file=sys.stdout)
 
         # Devolver los datos.
         return data
 
+    # Enviando un path estilo así 'collection1/document1/collection2' y enviando la key del interior del doc puedes recuperar la coleccion al completo
+    def get_all_data_from_collection(self, path: str, data_target: str):
+        """
+        Obtiene datos de todos los documentos dentro de una colección específica.
+
+        Parámetros:
+        -----------
+        path: str
+            Ruta hasta la colección de la cual queremos obtener datos, e.g., 'anime/anime-by-letter/downloads'.
+        data_target: str
+            Clave dentro de los documentos desde la cual se obtendrán los datos. Debe ser un campo válido en los documentos.
+
+        Retorna:
+        --------
+        list
+            Lista de arrays asociados con la clave 'data_target' en los documentos de la colección especificada.
+
+        Excepciones:
+        ------------
+        ValueError
+            - Si la colección no existe.
+            - Si los documentos no contienen el campo 'data_target'.
+        """
+
+        # Obtener la referencia a la colección
+        collection_ref = self.db.collection(path)
+
+        # Obtener todos los documentos de la colección
+        docs = collection_ref.stream()
+        data_list = []
+
+        for doc in docs:
+            doc_dict = doc.to_dict()
+
+            # Verificar que el documento contiene el target
+            if data_target in doc_dict:
+                data_list.append(doc_dict[data_target])
+            else:
+                print(
+                    f"[Error][get_data_from_collection()]: El documento {doc.id} no contiene el objetivo '{data_target}'.")
+
+        # Imprimimos mensaje para avisar de que se está descargando
+        print(f'[get_all_data_from_collection()]: Descargando la información de "{path}/{data_target}"...\n',
+              file=sys.stdout)
+
+        return data_list
+
+    # Aquí puedes setear datos en la base de datos
     def set_data_by_path(self, path: str, data_target: str, data: any):
         """
         Sobrescribe datos en un documento específico dentro de una base de datos siguiendo una ruta dada.
 
         La ruta debe especificar alternadamente colecciones y documentos, comenzando con una colección.
         Por ejemplo: 'collection1/document1/collection2/document2'.
```

### Comparing `sevenapps_py_easy-0.0.7/sevenapps/services/google_services_connector.py` & `sevenapps_py_easy-0.0.8/sevenapps/services/google_services_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.7/sevenapps/services/selenium_connector.py` & `sevenapps_py_easy-0.0.8/sevenapps/services/selenium_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.7/sevenapps/utils/file_manager.py` & `sevenapps_py_easy-0.0.8/sevenapps/utils/file_manager.py`

 * *Files identical despite different names*

