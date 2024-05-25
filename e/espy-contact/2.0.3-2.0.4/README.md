# Comparing `tmp/espy_contact-2.0.3.tar.gz` & `tmp/espy_contact-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-2.0.3.tar", last modified: Sat May 25 18:52:17 2024, max compression
+gzip compressed data, was "espy_contact-2.0.4.tar", last modified: Sat May 25 21:53:03 2024, max compression
```

## Comparing `espy_contact-2.0.3.tar` & `espy_contact-2.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.343713 espy_contact-2.0.3/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.3/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 18:52:17.343510 espy_contact-2.0.3/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.3/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.333806 espy_contact-2.0.3/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.3/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.336316 espy_contact-2.0.3/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.3/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.3/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.3/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.3/espy_contact/model/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1920 2024-05-24 06:56:06.000000 espy_contact-2.0.3/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.339942 espy_contact-2.0.3/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.3/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.3/espy_contact/schema/blog.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.3/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 17:11:06.000000 espy_contact-2.0.3/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.3/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1741 2024-05-09 02:58:06.000000 espy_contact-2.0.3/espy_contact/schema/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3370 2024-05-25 18:51:38.000000 espy_contact-2.0.3/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.3/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.340473 espy_contact-2.0.3/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.3/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.3/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.342421 espy_contact-2.0.3/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.3/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.3/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.3/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.3/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.3/espy_contact/util/esread.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.3/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.334805 espy_contact-2.0.3/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 18:52:17.000000 espy_contact-2.0.3/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-25 18:52:17.000000 espy_contact-2.0.3/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-25 18:52:17.000000 espy_contact-2.0.3/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-25 18:52:17.000000 espy_contact-2.0.3/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-25 18:52:17.000000 espy_contact-2.0.3/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-25 18:52:17.343791 espy_contact-2.0.3/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-25 18:51:55.000000 espy_contact-2.0.3/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 18:52:17.343257 espy_contact-2.0.3/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.3/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.3/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.3/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.553585 espy_contact-2.0.4/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.4/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 21:53:03.553365 espy_contact-2.0.4/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.4/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.543400 espy_contact-2.0.4/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.4/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.546398 espy_contact-2.0.4/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.4/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.4/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.4/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.4/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1920 2024-05-24 06:56:06.000000 espy_contact-2.0.4/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.549889 espy_contact-2.0.4/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.4/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.4/espy_contact/schema/blog.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.4/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 17:11:06.000000 espy_contact-2.0.4/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.4/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1741 2024-05-09 02:58:06.000000 espy_contact-2.0.4/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3741 2024-05-25 21:36:14.000000 espy_contact-2.0.4/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.4/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.550459 espy_contact-2.0.4/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.4/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.4/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.552327 espy_contact-2.0.4/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.4/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.4/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.4/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.4/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.4/espy_contact/util/esread.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.4/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.544498 espy_contact-2.0.4/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-25 21:53:03.553669 espy_contact-2.0.4/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-25 21:52:49.000000 espy_contact-2.0.4/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.553163 espy_contact-2.0.4/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.4/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.4/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.4/tests/test_service.py
```

### Comparing `espy_contact-2.0.3/LICENSE` & `espy_contact-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/model/messaging.py` & `espy_contact-2.0.4/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/model/models.py` & `espy_contact-2.0.4/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/model/reach.py` & `espy_contact-2.0.4/espy_contact/model/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/model/tranx.py` & `espy_contact-2.0.4/espy_contact/model/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/schema/blog.py` & `espy_contact-2.0.4/espy_contact/schema/blog.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/schema/campus.py` & `espy_contact-2.0.4/espy_contact/schema/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/schema/mgcampus.py` & `espy_contact-2.0.4/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/schema/reach.py` & `espy_contact-2.0.4/espy_contact/schema/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/schema/schema.py` & `espy_contact-2.0.4/espy_contact/schema/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 """
 from datetime import datetime, date
 from pydantic import BaseModel, EmailStr,Field
 from espy_contact.util.enums import AccessRoleEnum, StatusEnum,GenderEnum
 from typing import List, Optional, Union
 import uuid
+from pydantic import validator
 class ReachBase(BaseModel):
     id: str
     timestamp: datetime
 class SeoRequest(BaseModel):
     url: str = Field(min_length=4, description="Your website url")
 class WebbuilderRequest(BaseModel):
     id: str
@@ -31,14 +32,20 @@
     last_name: str
     email: EmailStr
     is_active: bool = False
     status: StatusEnum = StatusEnum.NEW
     roles: List[AccessRoleEnum]
     socialmedia: Optional[str] = None # comma separated string
     gender: GenderEnum
+
+    @validator('roles')
+    def validate_roles(cls, roles):
+        if AccessRoleEnum.STUDENT in roles and AccessRoleEnum.ADMIN in roles:
+            raise ValueError("User cannot have roles of Student and Admin at the same time")
+        return roles
 class AddressDto(BaseModel):
     id: Optional[str] = None
     street: str
     city: str
     state: str
     zip_code: int
     email: Optional[EmailStr] = None
@@ -79,14 +86,16 @@
 
 
 class SchoolDto(BaseModel):
     id: Optional[str] = str(uuid.uuid4())
     name: str
     address: AddressDto
     owner: str
+    email: Optional[EmailStr] = None
+    status: Optional[StatusEnum] = StatusEnum.NEW
 
 
 class SchoolResponse(BaseModel):
     id: str
     name: str
     create_at: datetime
     address_id: str
```

### Comparing `espy_contact-2.0.3/espy_contact/schema/tranx.py` & `espy_contact-2.0.4/espy_contact/schema/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/service/service.py` & `espy_contact-2.0.4/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/util/CONSTANTS.py` & `espy_contact-2.0.4/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/util/db.py` & `espy_contact-2.0.4/espy_contact/util/db.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/util/enums.py` & `espy_contact-2.0.4/espy_contact/util/enums.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact/util/pg.py` & `espy_contact-2.0.4/espy_contact/util/pg.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/espy_contact.egg-info/SOURCES.txt` & `espy_contact-2.0.4/espy_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.3/setup.py` & `espy_contact-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.4'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='2.0.3',
+    version='2.0.4',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
         'PyYAML ==6.0.1'
```

### Comparing `espy_contact-2.0.3/tests/test_copyright.py` & `espy_contact-2.0.4/tests/test_copyright.py`

 * *Files identical despite different names*

