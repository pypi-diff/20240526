# Comparing `tmp/asyncwhois-1.1.2.tar.gz` & `tmp/asyncwhois-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncwhois-1.1.2.tar", last modified: Mon May 13 18:13:13 2024, max compression
+gzip compressed data, was "asyncwhois-1.1.3.tar", last modified: Sun May 26 02:02:59 2024, max compression
```

## Comparing `asyncwhois-1.1.2.tar` & `asyncwhois-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1088 2021-10-05 12:08:13.000000 asyncwhois-1.1.2/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)       68 2021-10-05 12:08:13.000000 asyncwhois-1.1.2/MANIFEST.in
--rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)     8386 2024-02-09 18:43:48.000000 asyncwhois-1.1.2/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.978112 asyncwhois-1.1.2/asyncwhois/
--rw-rw-r--   0 joe       (1000) joe       (1000)    24538 2024-05-13 18:13:00.000000 asyncwhois-1.1.2/asyncwhois/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     8253 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/asyncwhois/client.py
--rw-rw-r--   0 joe       (1000) joe       (1000)      166 2023-02-13 17:04:50.000000 asyncwhois-1.1.2/asyncwhois/errors.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    12916 2023-10-12 17:12:26.000000 asyncwhois-1.1.2/asyncwhois/parse.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    14331 2024-05-13 17:56:47.000000 asyncwhois-1.1.2/asyncwhois/parse_rir.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    69492 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/asyncwhois/parse_tld.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     8994 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/asyncwhois/query.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/asyncwhois/servers/
--rw-rw-r--   0 joe       (1000) joe       (1000)    46078 2024-05-12 23:25:10.000000 asyncwhois-1.1.2/asyncwhois/servers/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    15501 2024-05-12 23:25:10.000000 asyncwhois-1.1.2/asyncwhois/servers/ipv4.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/asyncwhois.egg-info/
--rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      574 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       62 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       11 2024-05-13 18:13:13.000000 asyncwhois-1.1.2/asyncwhois.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)      239 2021-10-05 12:08:13.000000 asyncwhois-1.1.2/pyproject.toml
--rw-rw-r--   0 joe       (1000) joe       (1000)     1047 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)     1806 2024-05-13 17:58:59.000000 asyncwhois-1.1.2/setup.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-13 18:13:13.982112 asyncwhois-1.1.2/tests/
--rw-rw-r--   0 joe       (1000) joe       (1000)      676 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_not_found.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     1476 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_package_methods.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     2741 2023-10-12 17:12:26.000000 asyncwhois-1.1.2/tests/test_parser_methods.py
--rw-rw-r--   0 joe       (1000) joe       (1000)    59474 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_parser_output.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     1250 2024-02-09 18:37:40.000000 asyncwhois-1.1.2/tests/test_query.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-26 02:02:59.315168 asyncwhois-1.1.3/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1088 2021-10-05 12:08:13.000000 asyncwhois-1.1.3/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)       68 2021-10-05 12:08:13.000000 asyncwhois-1.1.3/MANIFEST.in
+-rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-26 02:02:59.315168 asyncwhois-1.1.3/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8386 2024-02-09 18:43:48.000000 asyncwhois-1.1.3/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-26 02:02:59.311168 asyncwhois-1.1.3/asyncwhois/
+-rw-rw-r--   0 joe       (1000) joe       (1000)    24538 2024-05-26 02:02:44.000000 asyncwhois-1.1.3/asyncwhois/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8253 2024-02-09 18:37:40.000000 asyncwhois-1.1.3/asyncwhois/client.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      166 2023-02-13 17:04:50.000000 asyncwhois-1.1.3/asyncwhois/errors.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    12916 2023-10-12 17:12:26.000000 asyncwhois-1.1.3/asyncwhois/parse.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    14331 2024-05-13 17:56:47.000000 asyncwhois-1.1.3/asyncwhois/parse_rir.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1680 2024-05-25 23:20:29.000000 asyncwhois-1.1.3/asyncwhois/parse_tld.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     8994 2024-02-09 18:37:40.000000 asyncwhois-1.1.3/asyncwhois/query.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-26 02:02:59.311168 asyncwhois-1.1.3/asyncwhois/servers/
+-rw-rw-r--   0 joe       (1000) joe       (1000)    46078 2024-05-12 23:25:10.000000 asyncwhois-1.1.3/asyncwhois/servers/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    15501 2024-05-12 23:25:10.000000 asyncwhois-1.1.3/asyncwhois/servers/ipv4.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    58604 2024-05-26 01:49:42.000000 asyncwhois-1.1.3/asyncwhois/tldparsers.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-26 02:02:59.315168 asyncwhois-1.1.3/asyncwhois.egg-info/
+-rw-r--r--   0 joe       (1000) joe       (1000)     9570 2024-05-26 02:02:59.000000 asyncwhois-1.1.3/asyncwhois.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      617 2024-05-26 02:02:59.000000 asyncwhois-1.1.3/asyncwhois.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2024-05-26 02:02:59.000000 asyncwhois-1.1.3/asyncwhois.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       62 2024-05-26 02:02:59.000000 asyncwhois-1.1.3/asyncwhois.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       17 2024-05-26 02:02:59.000000 asyncwhois-1.1.3/asyncwhois.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      239 2021-10-05 12:08:13.000000 asyncwhois-1.1.3/pyproject.toml
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1047 2024-05-26 02:02:59.315168 asyncwhois-1.1.3/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1796 2024-05-26 02:02:44.000000 asyncwhois-1.1.3/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2024-05-26 02:02:59.315168 asyncwhois-1.1.3/tests/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2020-07-06 15:52:51.000000 asyncwhois-1.1.3/tests/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      676 2024-02-09 18:37:40.000000 asyncwhois-1.1.3/tests/test_not_found.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1476 2024-02-09 18:37:40.000000 asyncwhois-1.1.3/tests/test_package_methods.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     2741 2023-10-12 17:12:26.000000 asyncwhois-1.1.3/tests/test_parser_methods.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)    59474 2024-02-09 18:37:40.000000 asyncwhois-1.1.3/tests/test_parser_output.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1250 2024-02-09 18:37:40.000000 asyncwhois-1.1.3/tests/test_query.py
```

### Comparing `asyncwhois-1.1.2/LICENSE` & `asyncwhois-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/PKG-INFO` & `asyncwhois-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python utility for querying and parsing WHOIS information for Domains, IPv4s, IPv6s, and AS numbers.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.1.2/README.md` & `asyncwhois-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois/__init__.py` & `asyncwhois-1.1.3/asyncwhois/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "DomainClient",
     "NumberClient",
     "NotFoundError",
     "WhoIsError",
     "GeneralError",
     "QueryError",
 ]
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 
 def whois(
     search_term: Union[str, ipaddress.IPv4Address, ipaddress.IPv6Address],
     authoritative_only: bool = False,
     ignore_not_found: bool = False,
     proxy_url: str = None,
```

### Comparing `asyncwhois-1.1.2/asyncwhois/client.py` & `asyncwhois-1.1.3/asyncwhois/client.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois/parse.py` & `asyncwhois-1.1.3/asyncwhois/parse.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois/parse_rir.py` & `asyncwhois-1.1.3/asyncwhois/parse_rir.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois/parse_tld.py` & `asyncwhois-1.1.3/asyncwhois/tldparsers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,23 @@
+"""TLD-specific domain parser classes
+"""
+
+
 from datetime import datetime
 import re
-from typing import Dict, Any, Union
+from typing import Any, Union
 
 from .parse import BaseParser, TLDBaseKeys
-from .errors import NotFoundError
-
-
-class DomainParser:
-    _no_match_checks = [
-        "no match",
-        "not found",
-        "no entries found",
-        "invalid query",
-        "domain name not known",
-        "no object found",
-        "available for re-registration",
-        "object does not exist",
-        "domain you requested is not known",
-    ]
 
-    def __init__(self, ignore_not_found: bool = False):
-        self.ignore_not_found = ignore_not_found
 
-    def parse(self, blob: str, tld: str) -> dict[TLDBaseKeys, Any]:
-        if not self.ignore_not_found and any(
-            [n in blob.lower() for n in self._no_match_checks]
-        ):
-            raise NotFoundError("Domain not found!")
-        parser = self._init_parser(tld)
-        return parser.parse(blob)
-
-    @staticmethod
-    def _init_parser(tld: str) -> "TLDParser":
-        """
-        Retrieves the parser instance which can most accurately extract
-        key/value pairs from the whois server output for the given `tld`.
-
-        :param tld: the top level domain
-        :return: instance of TLDParser or a TLDParser subclass
-        """
-        if tld == "ae":
-            return RegexAE()
-        elif tld == "ar":
-            return RegexAR()
-        elif tld == "at":
-            return RegexAT()
-        elif tld == "au":
-            return RegexAU()
-        elif tld == "aw":
-            return RegexAW()
-        elif tld == "ax":
-            return RegexAX()
-        elif tld == "be":
-            return RegexBE()
-        elif tld == "br":
-            return RegexBR()
-        elif tld == "by":
-            return RegexBY()
-        elif tld == "cc":
-            return RegexCC()
-        elif tld == "ch":
-            return RegexCH()
-        elif tld == "cl":
-            return RegexCL()
-        elif tld == "cn":
-            return RegexCN()
-        elif tld == "cr":
-            return RegexCR()
-        elif tld == "cz":
-            return RegexCZ()
-        elif tld == "de":
-            return RegexDE()
-        elif tld == "dk":
-            return RegexDK()
-        elif tld == "edu":
-            return RegexEDU()
-        elif tld == "ee":
-            return RegexEE()
-        elif tld == "eu":
-            return RegexEU()
-        elif tld == "fi":
-            return RegexFI()
-        elif tld == "fr":
-            return RegexFR()
-        elif tld == "ga":
-            return RegexGA()
-        elif tld == "ge":
-            return RegexGE()
-        elif tld == "gg":
-            return RegexGG()
-        elif tld == "gq":
-            return RegexGQ()
-        elif tld == "hk":
-            return RegexHK()
-        elif tld == "hr":
-            return RegexHR()
-        elif tld == "id":
-            return RegexID()
-        elif tld == "ie":
-            return RegexIE()
-        elif tld == "il":
-            return RegexIL()
-        elif tld == "ir":
-            return RegexIR()
-        elif tld == "is":
-            return RegexIS()
-        elif tld == "it":
-            return RegexIT()
-        elif tld == "jp":
-            return RegexJP()
-        elif tld == "kg":
-            return RegexKG()
-        elif tld == "kr":
-            return RegexKR()
-        elif tld == "kz":
-            return RegexKZ()
-        elif tld == "li":
-            return RegexLI()
-        elif tld == "lu":
-            return RegexLU()
-        elif tld == "lv":
-            return RegexLV()
-        elif tld == "ma":
-            return RegexMA()
-        elif tld == "ml":
-            return RegexML()
-        elif tld == "mx":
-            return RegexMX()
-        elif tld == "nl":
-            return RegexNL()
-        elif tld == "no":
-            return RegexNO()
-        elif tld == "nu":
-            return RegexNU()
-        elif tld == "nz":
-            return RegexNZ()
-        elif tld == "om":
-            return RegexOM()
-        elif tld == "pe":
-            return RegexPE()
-        elif tld == "pl":
-            return RegexPL()
-        elif tld == "pt":
-            return RegexPT()
-        elif tld == "rf":
-            return RegexRF()
-        elif tld == "ro":
-            return RegexRO()
-        elif tld == "ru":
-            return RegexRU()
-        elif tld == "sa":
-            return RegexSA()
-        elif tld == "se":
-            return RegexSE()
-        elif tld == "si":
-            return RegexSI()
-        elif tld == "sk":
-            return RegexSK()
-        elif tld == "su":
-            return RegexSU()
-        elif tld == "tk":
-            return RegexTK()
-        elif tld == "tr":
-            return RegexTR()
-        elif tld == "tw":
-            return RegexTW()
-        elif tld == "ua":
-            return RegexUA()
-        elif tld == "uk":
-            return RegexUK()
-        elif tld == "uz":
-            return RegexUZ()
-        elif tld == "ve":
-            return RegexVE()
-
-        # The TLDParser can handle all "Generic" and some "Country-Code" TLDs.
-        # If the parsed output of lookup is not what you expect or even incorrect,
-        # check and modify the existing Regex subclass or create a new one.
-        return TLDParser()
+ExpressionDict = dict[str, str]
 
 
 class TLDParser(BaseParser):
-    base_expressions = {
+    base_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name: *(.+)",
         TLDBaseKeys.CREATED: r"Creation Date: *(.+)",
         TLDBaseKeys.UPDATED: r"Updated Date: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expir\w+\sDate: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar: *(.+)",
         TLDBaseKeys.REGISTRAR_IANA_ID: r"Registrar IANA ID: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"Registrar URL: *(.+)",
@@ -235,198 +67,161 @@
         TLDBaseKeys.TECH_ZIPCODE: r"Tech Postal Code: (.*)",
         TLDBaseKeys.TECH_COUNTRY: r"Tech Country: (.+)",
         TLDBaseKeys.TECH_PHONE: r"Tech Phone: (.+)",
         TLDBaseKeys.TECH_FAX: r"Tech Fax: (.+)",
         TLDBaseKeys.TECH_EMAIL: r"Tech Email: (.+)",
     }
 
+    tld_specific_expressions: ExpressionDict = {}
+
     multiple_match_keys = (TLDBaseKeys.NAME_SERVERS, TLDBaseKeys.STATUS)
     date_keys = (TLDBaseKeys.CREATED, TLDBaseKeys.UPDATED, TLDBaseKeys.EXPIRES)
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.reg_expressions = self.base_expressions.copy()
+        self.update_reg_expressions(self.tld_specific_expressions)
 
 
 # ==============================
 # Custom Query Output Parsers
 # ==============================
 
 
 class RegexRU(TLDParser):
-    _ru_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.CREATED: r"created: *(.+)",
         TLDBaseKeys.EXPIRES: r"paid-till: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org: *(.+)",
         TLDBaseKeys.STATUS: r"state: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.ADMIN_EMAIL: r"admin-contact: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ru_expressions)
-
 
 class RegexCL(TLDParser):
-    _cl_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.NAME_SERVERS: r"Name server: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant name: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Registrant organisation: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar name: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration date: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.CREATED: r"Creation date: (\d{4}-\d{2}-\d{2})",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._cl_expressions)
-
 
 class RegexPL(TLDParser):
-    _pl_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"DOMAIN NAME: *(.+)\n",
         TLDBaseKeys.REGISTRAR: r"REGISTRAR:\s*(.+)",
         TLDBaseKeys.CREATED: r"created: *(.+)",
         TLDBaseKeys.EXPIRES: r"option expiration date: *(.+)",
         TLDBaseKeys.UPDATED: r"last modified: *(.+)\n",
         TLDBaseKeys.DNSSEC: r"dnssec: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._pl_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         nameservers_match = self.find_match(
             r"nameservers:*(.+)\ncreated:\s", blob, flags=re.DOTALL | re.IGNORECASE
         )
         if nameservers_match:
             parsed_output[TLDBaseKeys.NAME_SERVERS] = [
                 self._process(m) for m in nameservers_match.split("\n")
             ]
         return parsed_output
 
 
 class RegexRO(TLDParser):
     # % The ROTLD WHOIS service on port 43 never discloses any information concerning the registrant.
 
-    _ro_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Registered On: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expires On: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Nameserver: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"Referral URL: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ro_expressions)
-
 
 class RegexPE(TLDParser):
-    _pe_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant name: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar: *(.+)",
         TLDBaseKeys.ADMIN_EMAIL: r"Admin Email: *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name server: *(.+)",
         TLDBaseKeys.STATUS: r"Domain Status: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._pe_expressions)
-
 
 class RegexEE(TLDParser):
-    _ee_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *[\n\r]+\s*name: *([^\n\r]+)",
         TLDBaseKeys.STATUS: r"status: *([^\n\r]+)",
         TLDBaseKeys.CREATED: r"registered: *([^\n\r]+)",
         TLDBaseKeys.UPDATED: r"changed: *([^\n\r]+)",
         TLDBaseKeys.EXPIRES: r"expire: *([^\n\r]+)",
         TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?name: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?url: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"(?<=Registrar)[\s\S]*?phone: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"country: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ee_expressions)
-
 
 class RegexFR(TLDParser):
-    _fr_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.CREATED: r"created: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.UPDATED: r"last-update: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.EXPIRES: r"Expiry Date: (\d{4}-\d{2}-\d{2})",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._fr_expressions)
-
 
 class RegexBR(TLDParser):
-    _br_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"created: ",
         TLDBaseKeys.UPDATED: r"changed: ",
         TLDBaseKeys.STATUS: r"status: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"responsible: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"country: *(.+)",
         TLDBaseKeys.EXPIRES: r"expires: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._br_expressions)
-
 
 class RegexKR(TLDParser):
-    _kr_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Registered Date *: (\d{4}\.\s\d{2}\.\s\d{2}\.)",
         TLDBaseKeys.UPDATED: r"Last Updated Date *: (\d{4}\.\s\d{2}\.\s\d{2}\.)",
         TLDBaseKeys.EXPIRES: r"Expiration Date *: (\d{4}\.\s\d{2}\.\s\d{2}\.)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant *: (.+)",
         TLDBaseKeys.ADMIN_EMAIL: r"Administrative Contact(AC) *: *(.+)",
         TLDBaseKeys.ADMIN_NAME: r"AC E-Mail *: *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC *: ([a-zA-Z]+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"Registrant Zip Code: *: (.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant Address *: (.+)",
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name *: (.+)",
         TLDBaseKeys.NAME_SERVERS: r"Host Name *: (.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._kr_expressions)
-
 
 class RegexEU(TLDParser):
     # .EU whois server disclaimer:
     # % The EURid WHOIS service on port 43 (textual whois) never
     # % discloses any information concerning the registrant.
 
-    _eu_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\n.*Name: (.+)",
         TLDBaseKeys.REGISTRAR_URL: r"Registrar:\n.*Name:.+\n.*Website: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._eu_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # find name servers
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Name servers:", blob
         )
         return parsed_output
 
@@ -436,42 +231,34 @@
     #
     # % The DENIC whois service on port 43 doesn't disclose any information concerning
     # % the domain holder, general request and abuse contact.
     # % This information can be obtained through use of our web-based whois service
     # % available at the DENIC website:
     # % http://www.denic.de/en/domains/whois-service/web-whois.html
 
-    _de_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.UPDATED: r"Changed: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Nserver: *(.+)",
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._de_expressions)
-
 
 class RegexUK(TLDParser):
-    _uk_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain name:\r\n*(.+)",
         TLDBaseKeys.CREATED: r"Registered on:\s*(\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.UPDATED: r"Last updated:\s*(\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.EXPIRES: r"Expiry date:\s*(\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.REGISTRAR: r"Registrar:\s*(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?URL: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\n *(.+)",
         TLDBaseKeys.STATUS: r"Registration status:\n *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._uk_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # handle registrant address
         address_match = re.search(
             r"Registrant's address: *(.+)Data valid", blob, re.DOTALL
         )
         if address_match:
             address_pieces = [
@@ -482,30 +269,26 @@
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Name servers:", blob
         )
         return parsed_output
 
 
 class RegexJP(TLDParser):
-    _jp_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"\[Domain Name\] *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"\[Registrant\] *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"\[Organization\] *(.+)",
         TLDBaseKeys.CREATED: r"\[登録年月日\] *(.+)",
         TLDBaseKeys.EXPIRES: r"\[(?:有効限|有効期限)\]*(.+)",
         TLDBaseKeys.STATUS: r"\[状態\] *(.+)",
         TLDBaseKeys.UPDATED: r"\[最終更新\] *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"\[Name Server\] *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._jp_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # check for domain in japanese
         if not parsed_output.get(TLDBaseKeys.DOMAIN_NAME):
             parsed_output[TLDBaseKeys.DOMAIN_NAME] = self.find_match(
                 r"\[ドメイン名\] *(.+)", blob
             )
         # check for name servers in japanese
@@ -522,27 +305,23 @@
                 m.strip() for m in address_match.group(1).split("\n") if m.strip()
             ]
             parsed_output[TLDBaseKeys.REGISTRANT_ADDRESS] = ", ".join(address_pieces)
         return parsed_output
 
 
 class RegexAU(TLDParser):
-    _au_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.UPDATED: r"Last Modified: (\d{2}-\w{3}-\d{4})",
         TLDBaseKeys.REGISTRAR: r"Registrar Name:\s *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._au_expressions)
-
 
 class RegexAT(TLDParser):
-    _at_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.UPDATED: r"changed: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"registrant: *(.+)",
         TLDBaseKeys.TECH_NAME: r"tech-c: *(.+)",
     }
@@ -554,19 +333,15 @@
         "country": r"country: *(.+)",
         "zipcode": r"postal code: *(.+)",
         "email": "e-mail: *(.+)",
         "phone": "phone: *(.+)",
         "fax": "fax-no: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._at_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parser_output = super().parse(blob)
         contact_field_fills = [
             ["registrant", r"registrant: *(.+)"],
             ["admin", r"admin-c"],
             ["tech", r"tech-c: *(.+)"],
         ]
         # find and save nic-hdls
@@ -588,243 +363,188 @@
                         field_regex, contact_blob.group()
                     )
 
         return parser_output
 
 
 class RegexBE(TLDParser):
-    _be_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"Registered: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\n.+Name: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"Registrar:\n.+Name:.+\n.+Website:*(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\n *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._be_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Name servers:", blob
         )
         return parsed_output
 
 
-class RegexRF(TLDParser):  # same as RU
-    def __init__(self):
-        super().__init__()
-
-        self.update_reg_expressions(RegexRU._ru_expressions)
+class RegexRF(RegexRU):  # same as RU
+    pass
 
 
-class RegexSU(TLDParser):  # same as RU
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(RegexRU._ru_expressions)
+class RegexSU(RegexRU):  # same as RU
+    pass
 
 
 class RegexKG(TLDParser):
-    _kg_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain *(.+) ",
         TLDBaseKeys.REGISTRAR: r"Domain support: \s*(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Name: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Address: *(.+)",
         TLDBaseKeys.CREATED: r"Record created: *(.+)",
         TLDBaseKeys.EXPIRES: r"Record expires on \s*(.+)",
         TLDBaseKeys.UPDATED: r"Record last updated on\s*(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._kg_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Name servers in the listed order:", blob
         )
         return parsed_output
 
 
 class RegexCH(TLDParser):
-    _ch_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRANT_NAME: r"Holder of domain name:\s*(?:.*\n){1}\s*(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Holder of domain name:\s*(?:.*\n){2}\s*(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\n*(.+)",
         TLDBaseKeys.CREATED: r"First registration date:\n*(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC:*([\S]+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ch_expressions)
-
 
-class RegexLI(TLDParser):  # same as CH
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(RegexCH._ch_expressions)
+class RegexLI(RegexCH):  # same as CH
+    pass
 
 
 class RegexID(TLDParser):
-    _id_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Created On:(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Date:(.+)",
         TLDBaseKeys.UPDATED: r"Last Updated On:(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC:(.+)",
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar Organization:(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"Sponsoring Registrar Phone: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Sponsoring Registrar Email: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"Sponsoring Registrar URL: *(.+)",
         TLDBaseKeys.STATUS: r"Status:(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Name:(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant Street1:(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._id_expressions)
-
 
 class RegexSE(TLDParser):
-    _se_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"holder\.*: *(.+)",
         TLDBaseKeys.CREATED: r"created\.*: *(.+)",
         TLDBaseKeys.UPDATED: r"modified\.*: *(.+)",
         TLDBaseKeys.EXPIRES: r"expires\.*: *(.+)",
         TLDBaseKeys.DNSSEC: r"dnssec\.*: *(.+)",
         TLDBaseKeys.STATUS: r"status\.*: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._se_expressions)
-
 
 class RegexIT(TLDParser):
-    _it_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"(?<! )Created: *(.+)",
         TLDBaseKeys.UPDATED: r"(?<! )Last Update: *(.+)",
         TLDBaseKeys.EXPIRES: r"(?<! )Expire Date: *(.+)",
         TLDBaseKeys.STATUS: r"Status: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant)[\s\S]*?Organization:(.*)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant)[\s\S]*?Address:(.*)",
         TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?Name: *(.*)",
         TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?Web: *(.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._it_expressions)
-
 
 class RegexSA(TLDParser):
-    _sa_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Created on: *(.+)",
         TLDBaseKeys.UPDATED: r"Last Updated on: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\s*(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant)[\s\S]*?Address:((?:.+\n)*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._sa_expressions)
-
 
 class RegexSK(TLDParser):
-    _sk_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"(?<=Domain:)[\s\w\W]*?Created: *(.+)",
         TLDBaseKeys.UPDATED: r"(?<=Domain:)[\s\w\W]*?Updated: *(.+)",
         TLDBaseKeys.EXPIRES: r"Valid Until: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Name:\s*(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Street:\s*(.+)",
         TLDBaseKeys.REGISTRAR: r"(?<=Registrar)[\s\S]*?Organization:(.*)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"(?<=Registrar)[\s\S]*?Email: *(.*)",
         TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"(?<=Registrar)[\s\S]*?Phone: *(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=^Contact)[\s\S]*?City:(.*)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"(?<=^Contact)[\s\S]*?Postal Code:(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=^Contact)[\s\S]*?Country Code:(.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._sk_expressions)
-
 
 class RegexMX(TLDParser):
-    _mx_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Created On: *(.+)",
         TLDBaseKeys.UPDATED: r"Last Updated On: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Date: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\s*(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"URL: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant)[\s\S]*?Name:(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=Registrant)[\s\S]*?City:(.*)",
         TLDBaseKeys.REGISTRANT_STATE: r"(?<=Registrant)[\s\S]*?State:(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=Registrant)[\s\S]*?Country:(.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._mx_expressions)
-
 
 class RegexTW(TLDParser):
-    _tw_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Record created on (.+) ",
         TLDBaseKeys.EXPIRES: r"Record expires on (.+) ",
         TLDBaseKeys.REGISTRAR: r"Registration Service Provider: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"Registration Service URL: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant:)\s+(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=Registrant:)\s*(?:.*\n){5}\s+(.*),",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant:)\s*(?:.*\n){4}\s+(.*)",
         TLDBaseKeys.REGISTRANT_STATE: r"(?<=Registrant:)\s*(?:.*\n){5}.*, (.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=Registrant:)\s*(?:.*\n){6}\s+(.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._tw_expressions)
-
 
 class RegexTR(TLDParser):
-    _tr_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Created on.*: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expires on.*: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=[**] Registrant:)[\s\S]((?:\s.+)*)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=[**] Administrative Contact)[\s\S]*?Address\s+: (.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._tr_expressions)
-
 
 class RegexIS(TLDParser):
-    _is_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.CREATED: r"created\.*: *(.+)",
         TLDBaseKeys.EXPIRES: r"expires\.*: *(.+)",
         TLDBaseKeys.DNSSEC: r"dnssec\.*: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver\.*: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._is_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # find first instance of person/role (registrant)
         registrant_block = False
         registrant_name = None
         addresses = []
         for line in blob.split("\n"):
             if line.startswith("role") or line.startswith("person"):
@@ -840,49 +560,41 @@
         parsed_output[TLDBaseKeys.REGISTRANT_NAME] = registrant_name
         # join the address lines together and save
         parsed_output[TLDBaseKeys.REGISTRANT_ADDRESS] = ", ".join(addresses)
         return parsed_output
 
 
 class RegexDK(TLDParser):
-    _dk_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"Registered: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expires: *(.+)",
         TLDBaseKeys.DNSSEC: r"Dnssec: *(.+)",
         TLDBaseKeys.STATUS: r"Status: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant\s*(?:.*\n){2}\s*Name: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant\s*(?:.*\n){3}\s*Address: *(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"Registrant\s*(?:.*\n){4}\s*Postalcode: *(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"Registrant\s*(?:.*\n){5}\s*City: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"Registrant\s*(?:.*\n){6}\s*Country: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._dk_expressions)
-
 
 class RegexIL(TLDParser):
-    _li_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.EXPIRES: r"validity: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"person: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"address *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC: *(.+)",
         TLDBaseKeys.STATUS: r"status: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar name: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._li_expressions)
-
 
 class RegexFI(TLDParser):
-    _fi_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain\.*: *([\S]+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Holder\s*name\.*:\s(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"[Holder\w\W]address\.*: ([\S\ ]+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"[Holder\w\W]address\.*:.+\naddress\.*:\s(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"[Holder\w\W]address\.*:.+\naddress\.*:.+\naddress\.*:\s(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"country\.*:\s(.+)",
         TLDBaseKeys.STATUS: r"status\.*: *([\S]+)",
@@ -890,131 +602,103 @@
         TLDBaseKeys.UPDATED: r"modified\.*: *([\S]+)",
         TLDBaseKeys.EXPIRES: r"expires\.*: *([\S]+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver\.*: *([\S]+) \[\S+\]",
         TLDBaseKeys.DNSSEC: r"dnssec\.*: *([\S]+)",
         TLDBaseKeys.REGISTRAR: r"registrar\.*:\s(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._fi_expressions)
-
 
 class RegexNU(TLDParser):
-    _nu_expression = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain\.*: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"holder\.*: *(.+)",
         TLDBaseKeys.CREATED: r"created\.*: *(.+)",
         TLDBaseKeys.UPDATED: r"modified\.*: *(.+)",
         TLDBaseKeys.EXPIRES: r"expires\.*: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver\.*: *(.+)",
         TLDBaseKeys.DNSSEC: r"dnssec\.*: *(.+)",
         TLDBaseKeys.STATUS: r"status\.*: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._nu_expression)
-
 
 class RegexPT(TLDParser):
-    _pt_expression = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.CREATED: r"Creation Date: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Date: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Owner Name: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Owner Address: *(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"Owner Locality: *(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"Owner ZipCode: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name Server: *(.+) \|",
         TLDBaseKeys.STATUS: r"Domain Status: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._pt_expression)
-
 
 class RegexIE(TLDParser):
-    _ie_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRANT_NAME: r"Domain Holder: *(.+)",
         TLDBaseKeys.CREATED: r"Registration Date: *(.+)",
         TLDBaseKeys.EXPIRES: r"Renewal Date: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Nserver: *(.+)",
         TLDBaseKeys.STATUS: r"Renewal status: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Account Name: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ie_expressions)
-
 
 class RegexNZ(TLDParser):
     # These don't seem to be valid anymore:
-    # _nz_expressions = {
+    # tld_specific_expressions: ExpressionDict = {
     #     TLDBaseKeys.DOMAIN_NAME: r"",
     #     TLDBaseKeys.REGISTRAR: r"registrar_name:\s*([^\n\r]+)",
     #     TLDBaseKeys.UPDATED: r"domain_datelastmodified:\s*([^\n\r]+)",
     #     TLDBaseKeys.CREATED: r"domain_dateregistered:\s*([^\n\r]+)",
     #     TLDBaseKeys.EXPIRES: r"domain_datebilleduntil:\s*([^\n\r]+)",
     #     TLDBaseKeys.NAME_SERVERS: r"ns_name_\d*:\s*([^\n\r]+)",
     #     TLDBaseKeys.STATUS: r"status:\s*([^\n\r]+)",
     #     TLDBaseKeys.REGISTRANT_NAME: r"registrant_contact_name:\s*([^\n\r]+)",
     #     TLDBaseKeys.REGISTRANT_ADDRESS: r"registrant_contact_address\d*:\s*([^\n\r]+)",
     #     TLDBaseKeys.REGISTRANT_CITY: r"registrant_contact_city:\s*([^\n\r]+)",
     #     TLDBaseKeys.REGISTRANT_ZIPCODE: r"registrant_contact_postalcode:\s*([^\n\r]+)",
     #     TLDBaseKeys.REGISTRANT_COUNTRY: r"registrant_contact_country:\s*([^\n\r]+)",
     # }
-
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions({})
+    pass
 
 
 class RegexLU(TLDParser):
-    _lu_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domainname: *(.+)",
         TLDBaseKeys.CREATED: r"registered: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.STATUS: r"domaintype: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar-name: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"registrar-email: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"registrar-url: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org-name: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"org-address: *(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"org-zipcode:*(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"org-city: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"org-country: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-
-        self.update_reg_expressions(self._lu_expressions)
-
 
 class RegexCZ(TLDParser):
-    _cz_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"name: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.CREATED: r"registered: *(.+)",
         TLDBaseKeys.UPDATED: r"changed: *(.+)",
         TLDBaseKeys.EXPIRES: r"expire: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._cz_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         addresses = []
         seen_contact = False
         # extract address from registrant info block
         for line in blob.split("\n"):
             # check that this is first "contact" block
             if line.startswith("contact:"):
@@ -1030,31 +714,27 @@
         # just combine address lines; don't assume city/zipcode/country happen in any specific order
         address = ", ".join(addresses)
         parsed_output[TLDBaseKeys.REGISTRANT_ADDRESS] = address
         return parsed_output
 
 
 class RegexHR(TLDParser):
-    _hr_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name: *(.+)",
         TLDBaseKeys.UPDATED: r"Updated Date: *(.+)",
         TLDBaseKeys.CREATED: r"Creation Date: *(.+)",
         TLDBaseKeys.EXPIRES: r"Registrar Registration Expiration Date: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name Server: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Name:\s(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Registrant Street:\s*(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._hr_expressions)
-
 
 class RegexHK(TLDParser):
-    _hk_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.STATUS: r"Domain Status: *(.+)",
         TLDBaseKeys.DNSSEC: r"DNSSEC: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar Name: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Registrar Contact Information: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"Registrar Contact Information: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Contact Information:\s*Company English Name.*:(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Registrant Contact Information:)[\s\S]*?Address: (.*)",
@@ -1062,21 +742,17 @@
         # 'registrant_email': r'[Registrant Contact Information\w\W]+Email: ([\S\ ]+)',
         TLDBaseKeys.UPDATED: r"Updated Date: *(.+)",
         TLDBaseKeys.CREATED: r"[Registrant Contact Information\w\W]+Domain Name Commencement Date: (.+)",
         TLDBaseKeys.EXPIRES: r"[Registrant Contact Information\w\W]+Expiry Date: (.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name Servers Information:\s+((?:.+\n)*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._hk_expressions)
-
 
 class RegexUA(TLDParser):
-    _ua_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.STATUS: r"status: *(.+)",
         TLDBaseKeys.REGISTRAR: r"(?:Registrar: |(?<=Registrar:)[\s\W\w]*?organization-loc: )(.*)",
         TLDBaseKeys.REGISTRAR_URL: r"(?<=Registrar)[\s\S]*?url: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_PHONE: r"(?<=Registrar)[\s\S]*?abuse-phone: *(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"(?<=Registrar)[\s\S]*?abuse-email: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Registrant:)[\s\W\w]*?organization-loc:(.*)",
@@ -1091,18 +767,14 @@
         TLDBaseKeys.NAME_SERVERS: "nserver: *(.+)",
     }
 
     KNOWN_DATE_FORMATS = [
         "%Y-%m-%d %H:%M:%S%z",
     ]
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ua_expressions)
-
     @staticmethod
     def _fix_timezone(date_string: str) -> str:
         """
         Fix timezone format for datetime.strptime
 
         :param date_string: date string
         :return: fixed date string
@@ -1139,82 +811,62 @@
             except ValueError:
                 pass
 
         return date_string
 
 
 class RegexCN(TLDParser):
-    _cn_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar: *(.+)",
         TLDBaseKeys.CREATED: r"Registration Time: *(.+)",
         TLDBaseKeys.EXPIRES: r"Expiration Time: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant: *(.+)",
         TLDBaseKeys.REGISTRANT_EMAIL: r"Registrant Contact Email: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._cn_expressions)
-
 
 class RegexAR(TLDParser):
-    _ar_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.UPDATED: r"changed: *(.+)",
         TLDBaseKeys.CREATED: r"created: *(.+)",
         TLDBaseKeys.EXPIRES: r"expire: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+) \(.*\)",
         TLDBaseKeys.REGISTRANT_NAME: r"name: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ar_expressions)
-
 
 class RegexBY(TLDParser):
-    _by_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Person: *(.+)",
         TLDBaseKeys.REGISTRANT_EMAIL: r"Email: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Org: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"Country: *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Address: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._by_expressions)
-
 
-class RegexCR(TLDParser):
-    _cr_expressions = {
+class RegexCR(RegexCZ):
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"name: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.UPDATED: r"changed: *(.+)",
         TLDBaseKeys.CREATED: r"registered: *(.+)",
         TLDBaseKeys.EXPIRES: r"expire: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._cr_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
-        # CR server has the same format as CZ
-        return RegexCZ().parse(blob)
-
 
 class RegexVE(TLDParser):  # double check
-    _ve_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
         TLDBaseKeys.CREATED: "registered: *(.+)",
         TLDBaseKeys.EXPIRES: "expire: *(.+)",
         TLDBaseKeys.UPDATED: "changed: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"registrant: *(.+)",
@@ -1222,116 +874,92 @@
         TLDBaseKeys.REGISTRANT_CITY: r"address:.+\naddress: *(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"(?:address:.+\n){2}address: *(.+)",
         TLDBaseKeys.REGISTRANT_STATE: r"(?:address:.+\n){3}address: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?:address:.+\n){4}address: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ve_expressions)
-
 
 class RegexAE(TLDParser):
-    _ae_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.STATUS: r"Status: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Contact Name: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Registrant Contact Organisation: *(.+)",
         TLDBaseKeys.REGISTRANT_EMAIL: r"Registrant Contact Email: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar Name: *(.+)",
         TLDBaseKeys.TECH_NAME: r"Tech Contact Name: *(.+)",
         TLDBaseKeys.TECH_EMAIL: r"Tech Contact Email: *(.+)",
         TLDBaseKeys.TECH_ORGANIZATION: r"Tech Contact Organisation: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ae_expressions)
-
 
 class RegexSI(TLDParser):
-    _si_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRAR: r"registrar: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"registrar-url: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nameserver: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"registrant: *(.+)",
         TLDBaseKeys.CREATED: r"created: *(.+)",
         TLDBaseKeys.EXPIRES: r"expire: *(.+)",
         TLDBaseKeys.DOMAIN_NAME: "domain: *(.+)",
         TLDBaseKeys.STATUS: "status: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._si_expressions)
-
 
 class RegexNO(TLDParser):
     """
     % The whois service at port 43 is intended to contribute to resolving
     % technical problems where individual domains threaten the
     % functionality, security and stability of other domains or the
     % internet as an infrastructure. It does not give any information
     % about who the holder of a domain is. To find information about a
     % domain holder, please visit our website:
     % https://www.norid.no/en/domeneoppslag/
     """
 
-    _no_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: r"Created:\s*(.+)",
         TLDBaseKeys.UPDATED: r"Last updated:\s*(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name Server Handle\.*: *(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar Handle\.*: *(.+)",
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name\.*: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._no_expressions)
-
 
 class RegexKZ(TLDParser):
-    _kz_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain Name.*: (.+)",
         TLDBaseKeys.REGISTRAR: r"Current Registar:\s*(.+)",  # "Registar" typo exists on the whois server
         TLDBaseKeys.CREATED: r"Domain created:\s*(.+)\s\(",
         TLDBaseKeys.UPDATED: r"Last modified\s:\s*(.+)\s\(",
         TLDBaseKeys.NAME_SERVERS: r".+\sserver\.*:\s*(.+)",
         TLDBaseKeys.STATUS: r"Domain status\s:\s(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Organization Using Domain Name\nName\.*:\s(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"Street Address\.*:\s*(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"City\.*:\s*(.+)",
         TLDBaseKeys.REGISTRANT_ZIPCODE: r"Postal Code\.*:\s*(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"Country\.*:\s*(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Organization Name\.*:\s*(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._kz_expressions)
-
 
 class RegexIR(TLDParser):
-    _ir_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.UPDATED: r"last-updated: *(.+)",
         TLDBaseKeys.EXPIRES: r"expire-date: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"org: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"remarks:\s+\(Domain Holder\) *(.+)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"remarks:\s+\(Domain Holder Address\) *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver: *(.+)",
         TLDBaseKeys.DOMAIN_NAME: r"domain: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ir_expressions)
-
 
 class RegexTK(TLDParser):
-    _tk_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"(?<=Owner contact)[\s\S]*?Organization:(.*)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Owner contact)[\s\S]*?Name:(.*)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Owner contact)[\s\S]*?Address:(.*)",
         TLDBaseKeys.REGISTRANT_STATE: r"(?<=Owner contact)[\s\S]*?State:(.*)",
         TLDBaseKeys.REGISTRANT_CITY: r"(?<=Owner contact)[\s\S]*?City:(.*)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"(?<=Owner contact)[\s\S]*?Country:(.*)",
         TLDBaseKeys.REGISTRANT_EMAIL: r"(?<=Owner contact)[\s\S]*?E-mail:(.*)",
@@ -1362,19 +990,15 @@
         TLDBaseKeys.TECH_CITY: r"(?<=Tech contact)[\s\S]*?City:(.*)",
         TLDBaseKeys.TECH_COUNTRY: r"(?<=Tech contact)[\s\S]*?Country:(.*)",
         TLDBaseKeys.TECH_EMAIL: r"(?<=Tech contact)[\s\S]*?E-mail:(.*)",
         TLDBaseKeys.TECH_FAX: r"(?<=Tech contact)[\s\S]*?Fax:(.*)",
         TLDBaseKeys.TECH_PHONE: r"(?<=Tech contact)[\s\S]*?Phone:(.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._tk_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # handle multiline nameservers
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Domain nameservers:", blob
         )
         # a date parser exists for '%d/%m/%Y', but this interferes with the parser needed
         # for this one, which is '%m/%d/%Y', so this date format needs to be parsed separately here
@@ -1407,33 +1031,27 @@
                 parsed_output[TLDBaseKeys.DOMAIN_NAME] = self._process(
                     domain_name_match.group(1).replace("\n", "")
                 )
         return parsed_output
 
 
 class RegexCC(TLDParser):
-    _cc_expressions = {TLDBaseKeys.STATUS: r"Domain Status: *(.+)"}
-
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._cc_expressions)
+    tld_specific_expressions: ExpressionDict = {
+        TLDBaseKeys.STATUS: r"Domain Status: *(.+)"
+    }
 
 
 class RegexEDU(TLDParser):
-    _edu_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.CREATED: "Domain record activated: *(.+)",
         TLDBaseKeys.UPDATED: "Domain record last updated: *(.+)",
         TLDBaseKeys.EXPIRES: "Domain expires: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._edu_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         registrant_match = re.search(
             r"Registrant:*(.+)Administrative Contact", blob, re.DOTALL | re.IGNORECASE
         )
         if registrant_match:
             reg_info_raw = registrant_match.group(1).split("\n")
             # remove duplicates and empty strings
@@ -1462,91 +1080,63 @@
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Name Servers:", blob
         )
         return parsed_output
 
 
 class RegexLV(TLDParser):
-    _lv_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain: *(.+)",
         TLDBaseKeys.REGISTRAR: r"\[Registrar\]\n(?:.*)\nName:(.*)+",
         TLDBaseKeys.REGISTRANT_NAME: r"\[Holder\]\n(?:.*)\nName:(.*)+",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"\[Holder\]\n(?:.*)\Address:(.*)+",
         TLDBaseKeys.NAME_SERVERS: r"Nserver: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._lv_expressions)
-
-
-class RegexGQ(TLDParser):
-    _gq_expressions = {}
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._gq_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
-        # GQ server has the same format as TK
-        return RegexTK().parse(blob)
+class RegexGQ(RegexTK):
+    ...
 
 
 class RegexNL(TLDParser):
-    _nl_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRAR: r"Registrar:\n(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Abuse Contact:\n(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._nl_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # handle multiline nameservers
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Domain nameservers:", blob
         )
         return parsed_output
 
 
 class RegexMA(TLDParser):
-    _ma_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRAR: r"Sponsoring Registrar: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ma_expressions)
-
 
 class RegexGE(TLDParser):
-    _ge_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ge_expressions)
-
 
 class RegexGG(TLDParser):
-    _gg_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain:\n*(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\n*(.+)",
         TLDBaseKeys.REGISTRAR: r"Registrar:\n*(.+)",
         TLDBaseKeys.CREATED: r"Registered on *(.+) at",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._gg_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         # parse created date
         created_match = parsed_output.get(
             "created"
         )  # looks like 30th April 2003; need to remove day suffix
         if created_match and isinstance(created_match, str):
             date_string = re.sub(r"(\d)(st|nd|rd|th)", r"\1", created_match)
@@ -1560,70 +1150,58 @@
         parsed_output[TLDBaseKeys.STATUS] = self.find_multiline_match(
             "Domain status:", blob
         )
         return parsed_output
 
 
 class RegexAW(TLDParser):
-    _aw_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRAR: r"Registrar:\n*(.+)",
         TLDBaseKeys.REGISTRAR_ABUSE_EMAIL: r"Abuse Contact:\n*(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._aw_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Domain nameservers:", blob
         )
         return parsed_output
 
 
 class RegexAX(TLDParser):
-    _ax_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"domain\.+: *(.+)",
         TLDBaseKeys.REGISTRAR: r"registrar\.+: *(.+)",
         TLDBaseKeys.REGISTRAR_URL: r"www\.+: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"name\.+: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"country\.+: *(.+)",
         TLDBaseKeys.CREATED: r"created\.+: *(.+)",
         TLDBaseKeys.EXPIRES: r"expires\.+: *(.+)",
         TLDBaseKeys.UPDATED: r"modified\.+: *(.+)",
         TLDBaseKeys.STATUS: r"status\.+: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"nserver\.+: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ax_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         addresses = self.find_match(r"address\.+: *(.+)", blob, many=True)
         if addresses:
             parsed_output[TLDBaseKeys.REGISTRANT_ADDRESS] = ", ".join(addresses)
         return parsed_output
 
 
 class RegexML(TLDParser):
-    _ml_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.EXPIRES: r"Record will expire on: *(.+)",
         TLDBaseKeys.CREATED: r"Domain registered: *(.+)",
         TLDBaseKeys.DOMAIN_NAME: r"Domain name:\n*(.+)\sis\s",
         TLDBaseKeys.STATUS: r"Domain name:\n.+\sis\s*(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ml_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         parsed_output = super().parse(blob)
         parsed_output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Domain nameservers:", blob
         )
         for contact in ("Admin", "Billing", "Owner", "Tech"):
             # isolate the appropriate contact block
             contact_blob = re.search(f"{contact} contact:\n(.+)\n\n", blob, re.DOTALL)
@@ -1663,15 +1241,15 @@
             parsed_output[TLDBaseKeys.CREATED] = datetime.strptime(
                 parsed_output.get(TLDBaseKeys.CREATED), date_format
             )
         return parsed_output
 
 
 class RegexOM(TLDParser):
-    _om_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRAR: r"Registrar Name: *(.+)",
         TLDBaseKeys.UPDATED: r"Last Modified: *(.+)",
         TLDBaseKeys.REGISTRANT_CITY: r"Registrant Contact City: *(.+)",
         TLDBaseKeys.REGISTRANT_COUNTRY: r"Registrant Contact Country: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"Registrant Contact Organisation: *(.+)",
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant Contact Name: *(.+)",
         TLDBaseKeys.REGISTRANT_EMAIL: r"Registrant Contact Email: *(.+)",
@@ -1679,42 +1257,34 @@
         TLDBaseKeys.TECH_COUNTRY: r"Tech Contact Country: *(.+)",
         TLDBaseKeys.TECH_ORGANIZATION: r"Tech Contact Organisation: *(.+)",
         TLDBaseKeys.TECH_NAME: r"Tech Contact Name: *(.+)",
         TLDBaseKeys.TECH_EMAIL: r"Tech Contact Email: *(.+)",
         TLDBaseKeys.NAME_SERVERS: r"Name Server: *(.+)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._om_expressions)
-
 
 class RegexUZ(TLDParser):
-    _uz_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.REGISTRANT_NAME: r"Registrant:\s+([A-Za-z0-9\.\s]+\n)",
         TLDBaseKeys.REGISTRANT_EMAIL: r"Contact with Registrant: *(.+)",
         TLDBaseKeys.ADMIN_NAME: r"Administrative Contact:\s+([A-Za-z0-9\.\s]+\n)",
         TLDBaseKeys.BILLING_NAME: r"Billing Contact:\s+([A-Za-z0-9\.\s]+\n)",
         TLDBaseKeys.TECH_NAME: r"Technical Contact:\s+([A-Za-z0-9\.\s]+\n)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._uz_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         output = super().parse(blob)
         output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Domain servers in listed order:", blob
         )
         return output
 
 
 class RegexGA(TLDParser):
-    _ga_expressions = {
+    tld_specific_expressions: ExpressionDict = {
         TLDBaseKeys.DOMAIN_NAME: r"Domain name:\n*(.+) is",
         TLDBaseKeys.STATUS: r"Domain name:\n*.+ is (.+)",
         TLDBaseKeys.CREATED: r"Domain registered: *(.+)",
         TLDBaseKeys.EXPIRES: r"Record will expire on: *(.+)",
         TLDBaseKeys.REGISTRANT_ORGANIZATION: r"(?<=Owner contact)[\s\S]*?Organization:(.*)",
         TLDBaseKeys.REGISTRANT_NAME: r"(?<=Owner contact)[\s\S]*?Name:(.*)",
         TLDBaseKeys.REGISTRANT_ADDRESS: r"(?<=Owner contact)[\s\S]*?Address:(.*)",
@@ -1749,19 +1319,15 @@
         TLDBaseKeys.TECH_CITY: r"(?<=Tech contact)[\s\S]*?City:(.*)",
         TLDBaseKeys.TECH_COUNTRY: r"(?<=Tech contact)[\s\S]*?Country:(.*)",
         TLDBaseKeys.TECH_EMAIL: r"(?<=Tech contact)[\s\S]*?Phone:(.*)",
         TLDBaseKeys.TECH_FAX: r"(?<=Tech contact)[\s\S]*?Fax:(.*)",
         TLDBaseKeys.TECH_PHONE: r"(?<=Tech contact)[\s\S]*?Phone:(.*)",
     }
 
-    def __init__(self):
-        super().__init__()
-        self.update_reg_expressions(self._ga_expressions)
-
-    def parse(self, blob: str) -> Dict[str, Any]:
+    def parse(self, blob: str) -> dict[str, Any]:
         output = super().parse(blob)
         output[TLDBaseKeys.NAME_SERVERS] = self.find_multiline_match(
             "Domain Nameservers:", blob
         )
         # date format is m/d/Y
         created = output.get(TLDBaseKeys.CREATED)
         if created:
```

### Comparing `asyncwhois-1.1.2/asyncwhois/query.py` & `asyncwhois-1.1.3/asyncwhois/query.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois/servers/__init__.py` & `asyncwhois-1.1.3/asyncwhois/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois/servers/ipv4.py` & `asyncwhois-1.1.3/asyncwhois/servers/ipv4.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/asyncwhois.egg-info/PKG-INFO` & `asyncwhois-1.1.3/asyncwhois.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python utility for querying and parsing WHOIS information for Domains, IPv4s, IPv6s, and AS numbers.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.1.2/asyncwhois.egg-info/SOURCES.txt` & `asyncwhois-1.1.3/asyncwhois.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 asyncwhois/__init__.py
 asyncwhois/client.py
 asyncwhois/errors.py
 asyncwhois/parse.py
 asyncwhois/parse_rir.py
 asyncwhois/parse_tld.py
 asyncwhois/query.py
+asyncwhois/tldparsers.py
 asyncwhois.egg-info/PKG-INFO
 asyncwhois.egg-info/SOURCES.txt
 asyncwhois.egg-info/dependency_links.txt
 asyncwhois.egg-info/requires.txt
 asyncwhois.egg-info/top_level.txt
 asyncwhois/servers/__init__.py
 asyncwhois/servers/ipv4.py
+tests/__init__.py
 tests/test_not_found.py
 tests/test_package_methods.py
 tests/test_parser_methods.py
 tests/test_parser_output.py
 tests/test_query.py
```

### Comparing `asyncwhois-1.1.2/setup.cfg` & `asyncwhois-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/setup.py` & `asyncwhois-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development",
         "Topic :: Security",
         "Framework :: AsyncIO",
     ],
     url="https://github.com/pogzyb/asyncwhois",
-    packages=["asyncwhois", "asyncwhois.servers"],
+    packages=setuptools.find_packages(),
     package_dir={"asyncwhois": "asyncwhois"},
     python_requires=">=3.9",
 )
```

### Comparing `asyncwhois-1.1.2/tests/test_not_found.py` & `asyncwhois-1.1.3/tests/test_not_found.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/tests/test_package_methods.py` & `asyncwhois-1.1.3/tests/test_package_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/tests/test_parser_methods.py` & `asyncwhois-1.1.3/tests/test_parser_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/tests/test_parser_output.py` & `asyncwhois-1.1.3/tests/test_parser_output.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.1.2/tests/test_query.py` & `asyncwhois-1.1.3/tests/test_query.py`

 * *Files identical despite different names*

