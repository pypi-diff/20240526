# Comparing `tmp/powerpathfinder_models-0.0.2.tar.gz` & `tmp/powerpathfinder_models-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpathfinder_models-0.0.2.tar", last modified: Tue May 14 22:16:58 2024, max compression
+gzip compressed data, was "powerpathfinder_models-2.0.0.tar", last modified: Sat May 25 22:12:48 2024, max compression
```

## Comparing `powerpathfinder_models-0.0.2.tar` & `powerpathfinder_models-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.791967 powerpathfinder_models-0.0.2/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.791967 powerpathfinder_models-0.0.2/common/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.791967 powerpathfinder_models-0.0.2/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/charger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/common/models/valuation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 22:16:58.000000 powerpathfinder_models-0.0.2/powerpathfinder_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 22:16:54.000000 powerpathfinder_models-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 22:16:58.795967 powerpathfinder_models-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/charger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/fcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/valuation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/setup.cfg
```

### Comparing `powerpathfinder_models-0.0.2/common/models/charger.py` & `powerpathfinder_models-2.0.0/common/models/charger.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-0.0.2/common/models/payment.py` & `powerpathfinder_models-2.0.0/common/models/payment.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-0.0.2/common/models/route.py` & `powerpathfinder_models-2.0.0/common/models/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     originAlias = models.CharField(max_length=100)
 
     destinationLat = models.FloatField()
     destinationLon = models.FloatField()
     destinationAlias = models.CharField(max_length=100)
 
     polyline = models.TextField()
+    waypoints = models.JSONField(default=list)
     distance = models.PositiveIntegerField()
     duration = models.PositiveIntegerField()
 
     departureTime = models.DateTimeField()
     freeSeats = models.PositiveSmallIntegerField()
     price = models.FloatField(default=0.0)
```

### Comparing `powerpathfinder_models-0.0.2/common/models/user.py` & `powerpathfinder_models-2.0.0/common/models/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,65 +3,77 @@
 
 This will be shared through all the dockers and can be accesses by importing it.
 
 __example: from common.models import User, Driver
 """
 
 from django.contrib.auth.models import User as baseUser
+from django.core.validators import MinValueValidator
 from django.db import models
+from storages.backends.s3boto3 import S3Boto3Storage
 
 
 class User(baseUser):
     """
     User class for our project
 
     Args:
         baseUser (User): default django implementation for user
             (see the documentation for more info)
     """
 
+    Google = "google"
+    Facebook = "facebook"
+    Base = "base"
+
+    typeLoginChoices = [(Google, "google"), (Facebook, "facebook"), (Base, "base")]
+
     # change to keep the pk defined in the UML consistent
-    baseUser.email = models.EmailField(
-        "email address", unique=True)  # type: ignore
+    baseUser.email = models.EmailField("email address", unique=True)  # type: ignore
     birthDate = models.DateField(auto_now=False, auto_now_add=False)
     points = models.IntegerField(default=0)
     updatedAt = models.DateTimeField(
         "Last modification of the User", auto_now=True, auto_now_add=False
     )
-    createdAt = models.DateTimeField(
-        "Creation date of the User", auto_now=False, auto_now_add=True)
+    createdAt = models.DateTimeField("Creation date of the User", auto_now=False, auto_now_add=True)
 
     profileImage = models.ImageField(
-        upload_to="profile_image", null=True, blank=True, default="default.png")
+        upload_to="profile_image/",
+        null=True,
+        blank=True,
+        default="default.png",
+        storage=S3Boto3Storage(location="media/profile_image"),
+    )
+
+    typeOfLogin = models.CharField(max_length=50, choices=typeLoginChoices, default=Base)
 
     class Meta:
         app_label = "common"
 
 
 class ChargerType(models.Model):
     """
     Model to represent the types of chargers.
     """
 
-    MENNEKES = "Mennekes"
-    TESLA = "Tesla"
-    SCHUKO = "Schuko"
-    CHADEMO = "ChadeMO"
-    CSS_COMBO2 = "CSS Combo2"
+    MENNEKES = "MENNEKES"
+    TESLA = "TESLA"
+    SCHUKO = "SCHUKO"
+    CHADEMO = "CHADEMO"
+    CCS_COMBO2 = "CCS COMBO2"
 
     CHARGER_CHOICES = [
-        (MENNEKES, "Mennekes"),
-        (TESLA, "Tesla"),
-        (SCHUKO, "Schuko"),
-        (CHADEMO, "ChadeMO"),
-        (CSS_COMBO2, "CSS Combo2"),
+        (MENNEKES, "MENNEKES"),
+        (TESLA, "TESLA"),
+        (SCHUKO, "SCHUKO"),
+        (CHADEMO, "CHADEMO"),
+        (CCS_COMBO2, "CCS COMBO2"),
     ]
 
-    chargerType = models.CharField(
-        max_length=20, choices=CHARGER_CHOICES, unique=True)
+    chargerType = models.CharField(max_length=20, choices=CHARGER_CHOICES, unique=True)
 
     def __str__(self):
         return self.chargerType
 
     class Meta:
         app_label = "common"
 
@@ -107,23 +119,21 @@
     parent_pointer = models.OneToOneField(
         "User", verbose_name="Parent Class", on_delete=models.CASCADE, parent_link=True
     )
 
     # Rest of the fields needed
     dni = models.CharField(max_length=50, unique=True)
     driverPoints = models.IntegerField(default=0)
-    autonomy = models.IntegerField(default=0)
+    autonomy = models.IntegerField(default=1, validators=[MinValueValidator(1)])
 
     # Charger type attributes
-    chargerTypes = models.ManyToManyField(
-        "ChargerType", related_name="drivers")
+    chargerTypes = models.ManyToManyField("ChargerType", related_name="drivers")
 
     # Preferences attributes
-    preference = models.OneToOneField(
-        "Preference", on_delete=models.CASCADE, null=True)
+    preference = models.OneToOneField("Preference", on_delete=models.CASCADE, null=True)
 
     iban = models.CharField(max_length=36, unique=True, blank=True)
 
     def save(self, *args, **kwargs) -> None:
         """
         Override of the save method to add the preference if it does not exist
         """
@@ -137,18 +147,16 @@
 
 
 class Report(models.Model):
     """
     Model for storing Reports given by users to users or drivers.
     """
 
-    reporter = models.ForeignKey(
-        User, related_name="report_giver", on_delete=models.CASCADE)
-    reported = models.ForeignKey(
-        User, related_name="report_receiver", on_delete=models.CASCADE)
+    reporter = models.ForeignKey(User, related_name="report_giver", on_delete=models.CASCADE)
+    reported = models.ForeignKey(User, related_name="report_receiver", on_delete=models.CASCADE)
 
     updatedAt = models.DateTimeField(
         "Last modification of the Report", auto_now=True, auto_now_add=False
     )
     createdAt = models.DateTimeField(
         "Creation date of the Report", auto_now=False, auto_now_add=True
     )
```

### Comparing `powerpathfinder_models-0.0.2/common/models/valuation.py` & `powerpathfinder_models-2.0.0/common/models/valuation.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from .user import User
 from .route import Route
 
+
 class Valuation(models.Model):
     """
     Model for storing valuations given by users to users or drivers.
     """
 
     RATING_CHOICES = [
         (1, "1"),
@@ -31,15 +32,16 @@
         on_delete=models.CASCADE,
     )
     route = models.ForeignKey(Route, related_name="route_valuations", on_delete=models.CASCADE)
     rating = models.IntegerField(
         choices=RATING_CHOICES, validators=[MinValueValidator(1), MaxValueValidator(5)]
     )
     comment = models.TextField(blank=True)
+    createdAt = models.DateTimeField(auto_now_add=True)
 
     class Meta:
         """
         Meta used to add the label so that the imports work correctly
         """
 
         app_label = "common"
-        unique_together = ("giver", "receiver", "route")
+        unique_together = ("giver", "receiver", "route")
```

