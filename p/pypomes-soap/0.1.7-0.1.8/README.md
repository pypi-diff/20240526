# Comparing `tmp/pypomes_soap-0.1.7.tar.gz` & `tmp/pypomes_soap-0.1.8.tar.gz`

## Comparing `pypomes_soap-0.1.7.tar` & `pypomes_soap-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/src/pypomes_soap/__init__.py
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/src/pypomes_soap/soap_pomes.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/README.md
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/src/pypomes_soap/__init__.py
+-rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/src/pypomes_soap/soap_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/README.md
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pypomes_soap-0.1.8/PKG-INFO
```

### Comparing `pypomes_soap-0.1.7/src/pypomes_soap/soap_pomes.py` & `pypomes_soap-0.1.8/src/pypomes_soap/soap_pomes.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,160 +9,162 @@
 
 
 def soap_build_envelope(ws_url: str,
                         service: str,
                         payload: dict,
                         filepath: Path = None) -> bytes:
     """
-    Constrói e retorna o envelope SOAP para um dado serviço. Esse envelope não contem os *headers*.
+    Construct and return the SOAP envelope for a given service.
 
-    :param ws_url: a URL da solicitação
-    :param payload: os dados a serem enviados
-    :param service: o nome do serviço
-    :param filepath: Path to store the soap envelope.
-    :return: o envelope para a requisição SOAP, sem os headers
+    This envelope does not contain the *headers*.
+
+    :param ws_url: the request URL
+    :param payload: the data to be sent
+    :param service: the name of the service
+    :param filepath: path to store the soap envelope
+    :return: the envelope for the SOAP request, without the headers
     """
-    # obtem o cliente
+    # obtain the client
     zeep_client: Client = Client(wsdl=ws_url)
-    # obtem o envelope XML
+    # obtain the XML envelope
     root = zeep_client.create_message(zeep_client.service, service, **payload)
     result: bytes = etree.tostring(element_or_tree=root,
                                    pretty_print=True)
 
-    # salva o envelope em arquivo ?
+    # save the envelope to file ?
     if filepath:
-        # sim
+        # yes
         with filepath.open("wb") as f:
             f.write(result)
 
     return result
 
 
 def soap_post(ws_url: str,
               soap_envelope: bytes,
               extra_headers: dict = None,
               filepath: Path = None,
               timeout: int | None = HTTP_POST_TIMEOUT) -> bytes:
     """
-    Encaminha a solicitação SOAP, e retorna a resposta recebida.
+    Forward the SOAP request, and return the received response.
 
-    :param ws_url: a URL da solicitação
-    :param soap_envelope: o envelope SOAP
-    :param extra_headers: cabeçalho adicional
-    :param filepath: Path to store the response to the request.
+    :param ws_url: the request URL
+    :param soap_envelope: the SOAP envelope
+    :param extra_headers: additional headers
+    :param filepath: path to store the response to the request
     :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
-    :return: a resposta à solicitação
+    :return: the response to the SOAP request
     """
     # constrói o cabeçalho do envelope SOAP
     headers: dict = {"SOAPAction": '""',
                      "content-type": "application/soap+xml; charset=utf-8"}
 
-    # um cabeçalho adicional foi definido ?
+    # has additional headers been defined ?
     if extra_headers:
-        # sim, contabilize-o
+        # yes, acknowledge them
         headers.update(extra_headers)
 
-    # envia o request
+    # send the request
     response: requests.Response = requests.post(url=ws_url,
                                                 data=soap_envelope,
                                                 headers=headers,
                                                 timeout=timeout)
     result: bytes = response.content
 
-    # salva o response em arquivo ?
+    # save the response to file ?
     if filepath:
-        # sim
+        # yes
         with filepath.open("wb") as f:
             f.write(result)
 
     return result
 
 
 def soap_post_zeep(zeep_service: callable,
                    payload: dict,
                    filepath: Path = None) -> dict:
     """
-    Encaminha a solicitação SOAP utilizando o pacote *zeep*, e retorna a resposta recebida.
+    Forward the SOAP request using the *zeep* package, and return the received response.
 
-    :param zeep_service: o serviço de referência
-    :param payload: os dados a serem enviados
-    :param filepath: Path to store the JSON corresponding to the returned response.
-    :return: a resposta à solicitação
+    :param zeep_service: the reference service
+    :param payload: the data to be sent
+    :param filepath: path to store the JSON corresponding to the returned response
+    :return: the response to the SOAP request
     """
-    # invoca o servico
-    # ('response' é uma subclasse de dict - definida como retorno do 'zeep_service' no wsdl)
+    # invoke the service
+    # ('response' is a dict subclass - defined in the wsdl as the return to 'zeep_service')
     response: any = zeep_service(**payload)
 
-    # converte o conteúdo retornado em dict e o prepara para descarga em JSON
+    # convert the returned content to 'dict' and prepare it for dumping in JSON
     result: dict = ast.literal_eval(str(response))
     json_normalize_dict(result)
 
-    # salva o retorno em arquivo ?
+    # save the response to file ?
     if filepath:
-        # sim
+        # yes
         with filepath.open("w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
 def soap_get_dict(soap_response: bytes,
                   xml_path: Path = None,
                   json_path: Path = None) -> dict:
     """
-    Recupera o objeto *dict* contendo os dados retornados pela solicitação SOAP.
+    Retrieve the *dict* object containing the data returned by the SOAP request.
 
-    Esse objeto é retornado em condições de ser descarregado em formato JSON.
+    This object is returned ready to be downloaded in JSON format.
 
-    :param soap_response: o conteúdo retornado pela solicitação SOAP
-    :param xml_path: Path to store the XML correspondinge to the returned response.
-    :param json_path: Path to store the JSON correspondinge to the returned response.
-    :return: o objeto com os dados de resposta à solicitação
+    :param soap_response: the content returned by the SOAP request
+    :param xml_path: path to store the XML correspondinge to the returned response
+    :param json_path: path to store the JSON correspondinge to the returned response
+    :return: the object with the response data to the SOAP request
     """
-    # restringe o conteúdo retornado ao conteúdo da tag soap:Body
+    # restrict the returned content to the content of 'soap:Body'
     pos_1: int = soap_response.find(b"<soap:Body>") + 11
     pos_2: int = soap_response.find(b"</soap:Body>", pos_1)
     content: bytes = soap_response[pos_1:pos_2]
 
-    # salva o conteúdo XML retornado em arquivo ?
+    # save the returned XML content to file ?
     if xml_path:
-        # sim
+        # yes
         with xml_path.open("wb") as f:
             f.write(content)
 
-    # converte o conteúdo XML em dict e o prepara para descarga em JSON
+    # convert the returned XML content to 'dict' and prepare it for dumping in JSON
     result: dict = xml_to_dict(content)
     json_normalize_dict(result)
 
-    # salva o retorno em arquivo ?
+    # save the response to file ?
     if json_path:
-        # sim
+        # yes
         with json_path.open("w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
 def soap_get_cids(soap_response: bytes) -> list[bytes]:
     """
-    Obtem os *cids* (*Content-IDs*), em *soap_response*, indicativos de anexos retornados no padrão *MTOM*.
-
-    O padrão *Message Transmission Optimization Mechanism* define *cids* em *tags* do tipo
+    Retrieve the *cids* in *soap_response*, indicative of attachments returned in the *MTOM* standard.
 
-    - <xop:Include xmlns:xop="http://www.w3.org/2004/08/xop/include" href="cid:<uuid4>-<NN>@<web-address>"/>
+    The standard *Message Transmission Optimization Mechanism* defines *cids* (*Content-IDs*)
+    in *tags* type
+        - <xop:Include xmlns:xop="http://www.w3.org/2004/08/xop/include" href="cid:<uuid4>-<NN>@<web-address>"/>
 
-    onde as variáveis tem o significado:
-   - *<uuid4*>: uma *UUID* versão 4
-   - *<NN*>: um inteiro de dois dígitos
-   - *<web-address*>: o endereço web associado
+    where the variables have the meanings:
+        - *<uuid4*>: uma *UUID* versão 4
+        - *<NN*>: um inteiro de dois dígitos
+        - *<web-address*>: o endereço web associado
 
-   Os *cids* retornados têm a forma *<uuid4>-<NN>@<web-address*.
+    The *cids* are returned as *<uuid4>-<NN>@<web-address*.
 
-    :param soap_response: o conteúdo retornado pela solicitação SOAP
-    :return: a lista de 'content ids' encontrados, podendo ser vazia
+    :param soap_response: the content returned by the SOAP request
+    :return: the list of 'content ids' found, which may be empty
     """
     # inicializa a variável de retorno
     result: list[bytes] = []
 
     prefix: bytes = b'href="cid:'
     pos_1: int = soap_response.find(prefix)
     while pos_1 > 0:
@@ -174,50 +176,51 @@
     return result
 
 
 def soap_get_attachment(soap_response: bytes,
                         cid: bytes,
                         filepath: Path = None) -> bytes:
     """
-    Obtem e retorna o anexo contido no *response* da solicitação *SOAP*, no padrão *MTOM*.
+    Retrieve and return the attachment contained in the *response* to the *SOAP* request, in the *MTOM* pattern.
 
-    Nesse padrão (*Message Transmission Optimization Mechanism*), o anexo é identificado pelo *cid* (Content-ID).
+    In this standard (*Message Transmission Optimization Mechanism*), the attachment is identified
+    by its *cid* (*Content-ID*).
 
-    :param soap_response: o conteúdo retornado pela solicitação SOAP
-    :param cid: a identificação do anexo
-    :param filepath: Path to store the JSON corresponding to the returned attachment.
-    :return: o anexo em referência, ou None se não for encontrado
+    :param soap_response: the content returned by the SOAP request
+    :param cid: the attachement identification
+    :param filepath: path to store the JSON corresponding to the returned attachment
+    :return: the reference attachment, or 'None' if it was not found
     """
-    # inicializa a variável de retorno
+    # initialize the return variable
     result: bytes | None = None
 
-    # localiza o início do anexo
+    # locate the start of the attachment
     mark: bytes = b"Content-ID: <" + cid + b">"
     pos_1 = soap_response.find(mark)
 
-    # o início do anexo foi localizado ?
+    # was the start of the attachment located ?
     if pos_1 > 0:
-        # sim, prossiga
+        # yes, proceed
         pos_1 += len(mark)
-        # salta caracteres de controle (CR, LF, e outros)
+        # skip control chars (CR, LF, and others)
         blank: int = b" "[0]
         while soap_response[pos_1] < blank:
             pos_1 += 1
 
-        # obtem o separador
+        # obtain the separator
         pos_2: int = soap_response.find(b"--uuid:")
 
         separator: bytes = soap_response[pos_2:pos_2+45]  # 45 = 2 + length of uuid4 + 7
 
-        # localiza o final do anexo
+        # locate the end of the attachment
         pos_2 = soap_response.find(separator, pos_1)
 
-        # obtem o anexo
+        # retrieve the attachment
         result: bytes = soap_response[pos_1:pos_2]
 
-        # salva o attachment em arquivo ?
+        # save the attachment to file ?
         if filepath:
-            # sim
+            # yes
             with filepath.open("wb") as f:
                 f.write(result)
 
     return result
```

### Comparing `pypomes_soap-0.1.7/LICENSE` & `pypomes_soap-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_soap-0.1.7/pyproject.toml` & `pypomes_soap-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_soap"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (SOAP module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "lxml>=4.9.3",
     "pip>=24.0",
-    "pypomes_core>=0.8.7",
-    "pypomes_http>=0.1.3",
+    "pypomes_core>=1.0.7",
+    "pypomes_http>=0.1.8",
+    "pypomes_security>=0.1.4",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0",
     "zeep>=4.2.1"
 ]
 
 [project.urls]
```

### Comparing `pypomes_soap-0.1.7/PKG-INFO` & `pypomes_soap-0.1.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: pypomes_soap
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (SOAP module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-SOAP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-SOAP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.7
-Requires-Dist: pypomes-http>=0.1.3
+Requires-Dist: pypomes-core>=1.0.7
+Requires-Dist: pypomes-http>=0.1.8
+Requires-Dist: pypomes-security>=0.1.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
 Requires-Dist: zeep>=4.2.1
```

