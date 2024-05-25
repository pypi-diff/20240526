# Comparing `tmp/espy_contact-2.0.4.tar.gz` & `tmp/espy_contact-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-2.0.4.tar", last modified: Sat May 25 21:53:03 2024, max compression
+gzip compressed data, was "espy_contact-2.0.5.tar", last modified: Sat May 25 22:56:09 2024, max compression
```

## Comparing `espy_contact-2.0.4.tar` & `espy_contact-2.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.553585 espy_contact-2.0.4/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.4/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 21:53:03.553365 espy_contact-2.0.4/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.4/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.543400 espy_contact-2.0.4/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.4/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.546398 espy_contact-2.0.4/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.4/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.4/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.4/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.4/espy_contact/model/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1920 2024-05-24 06:56:06.000000 espy_contact-2.0.4/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.549889 espy_contact-2.0.4/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.4/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.4/espy_contact/schema/blog.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.4/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 17:11:06.000000 espy_contact-2.0.4/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.4/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1741 2024-05-09 02:58:06.000000 espy_contact-2.0.4/espy_contact/schema/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3741 2024-05-25 21:36:14.000000 espy_contact-2.0.4/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.4/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.550459 espy_contact-2.0.4/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.4/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.4/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.552327 espy_contact-2.0.4/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.4/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.4/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.4/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.4/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.4/espy_contact/util/esread.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.4/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.544498 espy_contact-2.0.4/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-25 21:53:03.000000 espy_contact-2.0.4/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-25 21:53:03.553669 espy_contact-2.0.4/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-25 21:52:49.000000 espy_contact-2.0.4/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 21:53:03.553163 espy_contact-2.0.4/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.4/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.4/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.4/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.888278 espy_contact-2.0.5/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.5/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 22:56:09.888127 espy_contact-2.0.5/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.5/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.880061 espy_contact-2.0.5/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.5/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.881990 espy_contact-2.0.5/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.5/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.5/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.5/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.5/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1920 2024-05-24 06:56:06.000000 espy_contact-2.0.5/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.884970 espy_contact-2.0.5/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.5/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.5/espy_contact/schema/blog.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.5/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 17:11:06.000000 espy_contact-2.0.5/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.5/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1782 2024-05-25 22:24:50.000000 espy_contact-2.0.5/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3770 2024-05-25 22:55:07.000000 espy_contact-2.0.5/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.5/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.885473 espy_contact-2.0.5/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.5/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.5/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.887203 espy_contact-2.0.5/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.5/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.5/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.5/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.5/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.5/espy_contact/util/esread.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.5/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.880707 espy_contact-2.0.5/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 22:56:09.000000 espy_contact-2.0.5/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-25 22:56:09.000000 espy_contact-2.0.5/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-25 22:56:09.000000 espy_contact-2.0.5/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-25 22:56:09.000000 espy_contact-2.0.5/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-25 22:56:09.000000 espy_contact-2.0.5/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-25 22:56:09.888346 espy_contact-2.0.5/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-25 22:24:59.000000 espy_contact-2.0.5/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 22:56:09.887941 espy_contact-2.0.5/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.5/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.5/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.5/tests/test_service.py
```

### Comparing `espy_contact-2.0.4/LICENSE` & `espy_contact-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/model/messaging.py` & `espy_contact-2.0.5/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/model/models.py` & `espy_contact-2.0.5/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/model/reach.py` & `espy_contact-2.0.5/espy_contact/model/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/model/tranx.py` & `espy_contact-2.0.5/espy_contact/model/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/schema/blog.py` & `espy_contact-2.0.5/espy_contact/schema/blog.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/schema/campus.py` & `espy_contact-2.0.5/espy_contact/schema/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/schema/mgcampus.py` & `espy_contact-2.0.5/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/schema/reach.py` & `espy_contact-2.0.5/espy_contact/schema/reach.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 from typing import List,Optional
 from datetime import datetime,date,timedelta
 from decimal import Decimal
-from pydantic import BaseModel,Field, EmailStr
+from pydantic import BaseModel,Field, EmailStr, ConfigDict
 from espy_contact.schema.schema import AppuserDto,AddressDto
 from espy_contact.util.enums import StatusEnum
 class ProductBase(BaseModel):
     logo: str
     website: str
     ga_property_id: str
     socials: str
     cost: Decimal = Field(max_digits=10, decimal_places=2)
     expiry_date: Optional[datetime] = None
     note: str
 
 class ProductCreate(ProductBase):
     pass
 class Product(ProductBase):
+    model_config = ConfigDict(from_attributes=True)
     id: int
     customer_id: int
 
-    class Config:
-        orm_mode = True
 class CustomerBase(BaseModel):
     pass
 
 class CustomerCreate(CustomerBase):
+    model_config = ConfigDict(from_attributes=True)
     business_name: str
     business_email: EmailStr
     contact_name: str
     contact_phone: str
     contact_email: EmailStr
     address: AddressDto
-    class Config:
-        orm_mode = True
 
 class Customer(CustomerBase):
+    model_config = ConfigDict(from_attributes=True)
     id: int
     staff: List[AppuserDto] = []
     products: List[Product] = []
 
-    class Config:
-        orm_mode = True
-
 class Campaign(BaseModel):
     id: Optional[int] = None
     title: str
     goals: Optional[str] = None
     target_audience: Optional[str] = None
     target_city: Optional[str] = None
     target_age_group: Optional[str] = None
```

### Comparing `espy_contact-2.0.4/espy_contact/schema/schema.py` & `espy_contact-2.0.5/espy_contact/schema/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 For permission requests, write to the publisher at the email address below:
 office@myeverlasting.net
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 from datetime import datetime, date
-from pydantic import BaseModel, EmailStr,Field
+from pydantic import BaseModel, EmailStr,Field, ConfigDict, field_validator
 from espy_contact.util.enums import AccessRoleEnum, StatusEnum,GenderEnum
 from typing import List, Optional, Union
 import uuid
 from pydantic import validator
 class ReachBase(BaseModel):
     id: str
     timestamp: datetime
@@ -33,39 +33,38 @@
     email: EmailStr
     is_active: bool = False
     status: StatusEnum = StatusEnum.NEW
     roles: List[AccessRoleEnum]
     socialmedia: Optional[str] = None # comma separated string
     gender: GenderEnum
 
-    @validator('roles')
+    @field_validator('roles')
     def validate_roles(cls, roles):
         if AccessRoleEnum.STUDENT in roles and AccessRoleEnum.ADMIN in roles:
             raise ValueError("User cannot have roles of Student and Admin at the same time")
         return roles
 class AddressDto(BaseModel):
-    id: Optional[str] = None
+    id: Optional[int] = None
     street: str
     city: str
     state: str
     zip_code: int
     email: Optional[EmailStr] = None
     phone_number: Optional[str] = None
     country: str
 
 
 class AppuserDto(UserResponse):
+    model_config = ConfigDict(from_attributes=True)
     password: str
     address: Optional[AddressDto] = None
 
-    class Config:
-        from_attributes = True
-
 
 class EnrollmentDto(UserResponse):
+    model_config = ConfigDict(from_attributes=True)
     dob: date
     gender: str
     nationality: str
     address: AddressDto
     parent_email: str
     current_school: str
     current_class: str
@@ -77,20 +76,17 @@
     religion: str
     password: Optional[str] = None
     photo: Optional[Union[str, bytes]] = None
     birth_certificate: Optional[Union[str, bytes]] = None
     signature: str
     is_paid: Optional[bool] = False
 
-    class Config:
-        from_attributes = True
-
 
 class SchoolDto(BaseModel):
-    id: Optional[str] = str(uuid.uuid4())
+    id: Optional[int] = None
     name: str
     address: AddressDto
     owner: str
     email: Optional[EmailStr] = None
     status: Optional[StatusEnum] = StatusEnum.NEW
 
 
@@ -100,23 +96,22 @@
     create_at: datetime
     address_id: str
     owner_id: str
 
 
 class AcademicHistory(ReachBase):
     """Student or teacher can have multiple AcademicHistory."""
+    model_config = ConfigDict(from_attributes=True)
 
     school_name: str
     start_date: str
     end_date: str
     grade_level: str
     reason_for_leaving: str
     classroom: str  # ForeignKey to Classroom or String
     owner: AppuserDto  # ForeignKey to StudentProfile or None
 
     # teacher: Teacher  # Optional ForeignKey to Teacher (null allowed) or None
-    class Config:
-        from_attributes = True
 
 class GenDto(BaseModel):
     start_date: date
     end_date: date
```

### Comparing `espy_contact-2.0.4/espy_contact/schema/tranx.py` & `espy_contact-2.0.5/espy_contact/schema/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/service/service.py` & `espy_contact-2.0.5/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/util/CONSTANTS.py` & `espy_contact-2.0.5/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/util/db.py` & `espy_contact-2.0.5/espy_contact/util/db.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/util/enums.py` & `espy_contact-2.0.5/espy_contact/util/enums.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact/util/pg.py` & `espy_contact-2.0.5/espy_contact/util/pg.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/espy_contact.egg-info/SOURCES.txt` & `espy_contact-2.0.5/espy_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.4/setup.py` & `espy_contact-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.4'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='2.0.4',
+    version='2.0.5',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
         'PyYAML ==6.0.1'
```

### Comparing `espy_contact-2.0.4/tests/test_copyright.py` & `espy_contact-2.0.5/tests/test_copyright.py`

 * *Files identical despite different names*

