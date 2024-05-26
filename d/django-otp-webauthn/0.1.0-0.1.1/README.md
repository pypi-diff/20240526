# Comparing `tmp/django_otp_webauthn-0.1.0.tar.gz` & `tmp/django_otp_webauthn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_otp_webauthn-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django_otp_webauthn-0.1.0.tar` & `django_otp_webauthn-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,66 @@
--rw-r--r--   0        0        0     1472 2024-04-30 12:15:19.818474 django_otp_webauthn-0.1.0/LICENSE
--rw-r--r--   0        0        0    12428 2024-05-12 20:37:46.602779 django_otp_webauthn-0.1.0/README.md
--rw-r--r--   0        0        0     1860 2024-05-12 12:39:12.154670 django_otp_webauthn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 12:06:20.291600 django_otp_webauthn-0.1.0/src/django_otp_webauthn/__init__.py
--rw-r--r--   0        0        0     3072 2024-05-12 19:36:31.822035 django_otp_webauthn-0.1.0/src/django_otp_webauthn/admin.py
--rw-r--r--   0        0        0      792 2024-05-12 12:31:54.490601 django_otp_webauthn-0.1.0/src/django_otp_webauthn/apps.py
--rw-r--r--   0        0        0     4602 2024-05-12 12:42:05.324011 django_otp_webauthn-0.1.0/src/django_otp_webauthn/checks.py
--rw-r--r--   0        0        0     1798 2024-05-11 15:36:36.840304 django_otp_webauthn-0.1.0/src/django_otp_webauthn/exceptions.py
--rw-r--r--   0        0        0    22876 2024-05-12 12:43:15.946264 django_otp_webauthn-0.1.0/src/django_otp_webauthn/helpers.py
--rw-r--r--   0        0        0     6148 2024-05-12 12:37:18.044415 django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/.DS_Store
--rw-r--r--   0        0        0     2789 2024-05-12 20:41:31.558027 django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4408 2024-05-12 20:41:29.614172 django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3027 2024-05-12 20:41:31.557975 django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3213 2024-05-12 20:41:29.287453 django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/nl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     6557 2024-05-12 13:23:25.996963 django_otp_webauthn-0.1.0/src/django_otp_webauthn/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-30 12:06:20.297993 django_otp_webauthn-0.1.0/src/django_otp_webauthn/migrations/__init__.py
--rw-r--r--   0        0        0    15741 2024-05-12 13:23:16.316029 django_otp_webauthn-0.1.0/src/django_otp_webauthn/models.py
--rw-r--r--   0        0        0     4439 2024-05-12 12:43:29.084674 django_otp_webauthn-0.1.0/src/django_otp_webauthn/settings.py
--rw-r--r--   0        0        0     6148 2024-05-12 12:35:58.822173 django_otp_webauthn-0.1.0/src/django_otp_webauthn/static/.DS_Store
--rw-r--r--   0        0        0    13498 2024-05-12 20:41:39.022110 django_otp_webauthn-0.1.0/src/django_otp_webauthn/static/django_otp_webauthn/otp_webauthn_auth.js
--rw-r--r--   0        0        0    46536 2024-05-12 20:41:39.022298 django_otp_webauthn-0.1.0/src/django_otp_webauthn/static/django_otp_webauthn/otp_webauthn_auth.js.map
--rw-r--r--   0        0        0    11620 2024-05-12 20:41:39.022084 django_otp_webauthn-0.1.0/src/django_otp_webauthn/static/django_otp_webauthn/otp_webauthn_register.js
--rw-r--r--   0        0        0    39252 2024-05-12 12:30:28.096985 django_otp_webauthn-0.1.0/src/django_otp_webauthn/static/django_otp_webauthn/otp_webauthn_register.js.map
--rw-r--r--   0        0        0      275 2024-05-11 15:28:28.996376 django_otp_webauthn-0.1.0/src/django_otp_webauthn/templates/django_otp_webauthn/auth_scripts.html
--rw-r--r--   0        0        0      279 2024-05-11 15:28:35.217841 django_otp_webauthn-0.1.0/src/django_otp_webauthn/templates/django_otp_webauthn/register_scripts.html
--rw-r--r--   0        0        0        0 2024-04-30 12:06:20.304053 django_otp_webauthn-0.1.0/src/django_otp_webauthn/templatetags/__init__.py
--rw-r--r--   0        0        0     1841 2024-05-02 13:44:01.465652 django_otp_webauthn-0.1.0/src/django_otp_webauthn/templatetags/otp_webauthn.py
--rw-r--r--   0        0        0     1070 2024-05-02 11:47:08.618818 django_otp_webauthn-0.1.0/src/django_otp_webauthn/urls.py
--rw-r--r--   0        0        0     6116 2024-05-10 11:12:47.818000 django_otp_webauthn-0.1.0/src/django_otp_webauthn/utils.py
--rw-r--r--   0        0        0     9332 2024-05-12 19:18:43.744524 django_otp_webauthn-0.1.0/src/django_otp_webauthn/views.py
--rw-r--r--   0        0        0    13536 1970-01-01 00:00:00.000000 django_otp_webauthn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/Caddyfile
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/DEVELOPMENT.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/ROADMAP.md
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/SECURITY.md
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/compile_translations.sh
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/manage.py
+-rw-r--r--   0        0        0    29065 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/poetry.lock
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox-requirements.txt
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/update_translations.sh
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/.editorconfig
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/.gitignore
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/package.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/tsconfig.json
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/webpack.base.config.ts
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/webpack.dev.config.ts
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/webpack.prod.config.ts
+-rw-r--r--   0        0        0   110076 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/yarn.lock
+-rw-r--r--   0        0        0    15810 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/src/auth.ts
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/src/globals.d.ts
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/src/register.ts
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/src/types.ts
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/client/src/utils.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/__init__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/admin.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/asgi.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/middleware.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/settings.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/urls.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/views.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/wsgi.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/static/sandbox/django_admin_login.css
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/static/sandbox/event_listeners.js
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/static/sandbox/style.css
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/templates/base.html
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/templates/django_admin_login.html
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/templates/registration/login.html
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/templates/sandbox/index.html
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/sandbox/templates/sandbox/second_factor_verification.html
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/__init__.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/admin.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/apps.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/checks.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/exceptions.py
+-rw-r--r--   0        0        0    22656 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/helpers.py
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/models.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/settings.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/urls.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/utils.py
+-rw-r--r--   0        0        0     9286 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/views.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/locale/nl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/migrations/0001_initial.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/migrations/0002_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/migrations/__init__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/templates/django_otp_webauthn/auth_scripts.html
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/templates/django_otp_webauthn/register_scripts.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/templatetags/__init__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/src/django_otp_webauthn/templatetags/otp_webauthn.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/LICENSE
+-rw-r--r--   0        0        0    12425 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/README.md
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 django_otp_webauthn-0.1.1/PKG-INFO
```

### Comparing `django_otp_webauthn-0.1.0/LICENSE` & `django_otp_webauthn-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2024 Stormbase
+Copyright (c) 2024 Stormbase
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
```

### Comparing `django_otp_webauthn-0.1.0/README.md` & `django_otp_webauthn-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   - [Compatibility](#compatibility)
     - [Browser compatibility](#browser-compatibility)
   - [Features](#features)
   - [Quick start guide - how to use Passkeys in your Django project](#quick-start-guide---how-to-use-passkeys-in-your-django-project)
   - [What exactly is a Passkey?](#what-exactly-is-a-passkey)
     - [How Passkeys work (in a nutshell)](#how-passkeys-work-in-a-nutshell)
     - [Why use Passkeys?](#why-use-passkeys)
-      - [A note about security](#a-note-about-security)
+    - [A note about security](#a-note-about-security)
   - [Who uses Passkeys?](#who-uses-passkeys)
   - [Further reading](#further-reading)
   - [Development](#development)
   - [License](#license)
 
 ## Compatibility
 
@@ -192,15 +192,15 @@
 3. The server looks up the public key associated with the given credential ID and uses it to check the signature. Was this signature generated by the private key that belongs to the public key we have on file? If yes, the user must be in possession of the private key and is authenticated.
 
 ### Why use Passkeys?
 
 - **Security.** Compared to passwords, Passkeys are resistant to phishing attacks, credential stuffing, and other common attacks.
 - **Convenience.** Passkeys are more convenient than passwords. Users don't have to choose and remember a password, they can use their phone, laptop, or security key to authenticate. Compared to other traditional forms of Multi Factor Authentication, there is no need to wait for an SMS code to arrive or copy a code from an authenticator app. Just click yes on the browser prompt.
 
-#### A note about security
+### A note about security
 
 Passkeys are sometimes claimed to be silver bullet for security. While they are more secure than passwords, they are not perfect.
 
 You put trust in the user's device and its manufacturer. Most devices support some form is syncing Passkeys between devices, like through an iCloud or Google account. This means that if someone gains access to the users' iCloud or Google account, they could potentially access their Passkeys. Users that have poorly secured their account and devices are at risk. However, this is not unique to Passkeys. The same risks exists for password managers and other forms of Multi Factor Authentication that support syncing between devices. Passkeys improve over other methods by their resistance to phishing attacks, credential stuffing and their convenience.
 
 It is the author's opinion that the benefits of Passkeys outweigh the risks. This section is here for your own consideration.
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/admin.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.utils.translation import gettext_lazy as _
 
 from django_otp_webauthn.models import WebAuthnCredential
 from django_otp_webauthn.settings import app_settings
 
 credential_model = app_settings.OTP_WEBAUTHN_CREDENTIAL_MODEL
 
+
 class WebAuthnCredentialAdmin(admin.ModelAdmin):
     list_display = [
         "user",
         "name",
         "credential_id_hex_display",
         "aaguid",
         "last_used_at",
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/apps.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,11 +10,9 @@
     name = "django_otp_webauthn"
     verbose_name = _("OTP WebAuthn")
 
     def ready(self):
         register(checks.check_settings_supported_cose_algorithms, Tags.security)
         register(checks.check_settings_dangerous_session_backend_used, Tags.security)
         register(checks.check_settings_allowed_origins_missing, Tags.compatibility)
-        register(
-            checks.check_settings_allowed_origins_misconfigured, Tags.compatibility
-        )
+        register(checks.check_settings_allowed_origins_misconfigured, Tags.compatibility)
         register(checks.check_settings_relying_party, Tags.models)
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/checks.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,25 @@
 ERR_ALLOWED_ORIGINS_MALFORMED = "otp_webauthn.E031"
 ERR_DANGEROUS_SESSION_BACKEND = "otp_webauthn.E040"
 
 
 def check_settings_relying_party(app_configs, **kwargs):
     errors = []
 
-    if (
-        not app_settings.OTP_WEBAUTHN_RP_ID_CALLABLE
-        and not app_settings.OTP_WEBAUTHN_RP_ID
-    ):
+    if not app_settings.OTP_WEBAUTHN_RP_ID_CALLABLE and not app_settings.OTP_WEBAUTHN_RP_ID:
         errors.append(
             Error(
                 "Relying party ID not configured.",
                 hint="Set the OTP_WEBAUTHN_RP_ID setting to the main domain of the web application, e.g. 'example.com'.",
                 obj=None,
                 id=ERR_NO_RP_ID,
             )
         )
 
-    if (
-        not app_settings.OTP_WEBAUTHN_RP_NAME_CALLABLE
-        and not app_settings.OTP_WEBAUTHN_RP_NAME
-    ):
+    if not app_settings.OTP_WEBAUTHN_RP_NAME_CALLABLE and not app_settings.OTP_WEBAUTHN_RP_NAME:
         errors.append(
             Error(
                 "Relying party name not configured.",
                 hint="Set the OTP_WEBAUTHN_RP_NAME setting to a human-readable name for the relying party, e.g. 'Acme Corp.'.",
                 obj=None,
                 id=ERR_NO_RP_NAME,
             )
@@ -100,17 +94,15 @@
                 obj=None,
                 id=ERR_ALLOWED_ORIGINS_MALFORMED,
             )
         )
         return errors
 
     for origin in allowed_origins:
-        if not origin.startswith("https://") and not origin.startswith(
-            "http://localhost"
-        ):
+        if not origin.startswith("https://") and not origin.startswith("http://localhost"):
             errors.append(
                 Error(
                     f"Allowed origin {origin!r} is not a secure origin.",
                     hint="Expected origins should start with 'https://'. Check the OTP_WEBAUTHN_ALLOWED_ORIGINS setting.",
                     obj=None,
                     id=ERR_ALLOWED_ORIGINS_MALFORMED,
                 )
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/exceptions.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 class OTPWebAuthnApiError(APIException):
     pass
 
 
 class InvalidState(OTPWebAuthnApiError):
     status_code = 400
-    default_detail = _(
-        "State is missing or invalid. Please begin the operation first before trying to complete it."
-    )
+    default_detail = _("State is missing or invalid. Please begin the operation first before trying to complete it.")
     default_code = "invalid_state"
 
 
 class UnprocessableEntity(OTPWebAuthnApiError):
     status_code = 422
     default_detail = _("Unprocessable Entity")
     default_code = "unprocessable_request"
@@ -54,11 +52,9 @@
     status_code = 403
     default_detail = _("This Passkey has been marked as disabled.")
     default_code = "credential_disabled"
 
 
 class CredentialNotFound(OTPWebAuthnApiError):
     status_code = 404
-    default_detail = _(
-        "The Passkey you tried to use was not found. Perhaps it was removed?"
-    )
+    default_detail = _("The Passkey you tried to use was not found. Perhaps it was removed?")
     default_code = "credential_not_found"
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/helpers.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,32 +246,26 @@
         """
 
         raw_algorithms = app_settings.OTP_WEBAUTHN_SUPPORTED_COSE_ALGORITHMS
         if raw_algorithms == "all":
             # Indicates all py_webauthn supported algorithms
             return None
 
-        algorithms = [
-            COSEAlgorithmIdentifier(a)
-            for a in raw_algorithms
-            if a in COSEAlgorithmIdentifier
-        ]
+        algorithms = [COSEAlgorithmIdentifier(a) for a in raw_algorithms if a in COSEAlgorithmIdentifier]
         return algorithms
 
     def get_generate_registration_options_kwargs(self, *, user: AbstractUser) -> dict:
         """Get the keyword arguments to pass to `webauthn.generate_registration_options`."""
         challenge = self.generate_challenge()
         rp = self.get_relying_party()
         user_entity = self.get_user_entity(user)
         attestation_preference = self.get_attestation_conveyance_preference()
         discoverable_credentials = self.get_discoverable_credentials_preference()
         user_verification = UserVerificationRequirement.PREFERRED
-        exclude_credentials = WebAuthnCredential.get_credential_descriptors_for_user(
-            user
-        )
+        exclude_credentials = WebAuthnCredential.get_credential_descriptors_for_user(user)
         supported_algorithms = self.get_supported_key_algorithms()
         authenticator_selection = AuthenticatorSelectionCriteria(
             user_verification=user_verification, resident_key=discoverable_credentials
         )
 
         options = {
             "attestation": attestation_preference,
@@ -304,17 +298,15 @@
 
     def get_registration_state(self, creation_options: dict) -> dict:
         """Get the state to store during registration. This state will be used
         to verify the registration later on."""
 
         return {
             "challenge": creation_options["challenge"],
-            "require_user_verification": creation_options["authenticatorSelection"][
-                "userVerification"
-            ]
+            "require_user_verification": creation_options["authenticatorSelection"]["userVerification"]
             == UserVerificationRequirement.REQUIRED.value,
         }
 
     def register_begin(self, user: AbstractUser) -> tuple[dict, dict]:
         """Begin the registration process."""
 
         kwargs = self.get_generate_registration_options_kwargs(user=user)
@@ -356,22 +348,20 @@
 
         response = verify_registration_response(
             credential=credential,
             expected_challenge=expected_challenge,
             expected_rp_id=expected_rp_id,
             expected_origin=allowed_origins,
             require_user_verification=require_user_verification,
-            **kwargs
+            **kwargs,
         )
 
         device = self.create_credential(user, response, credential, data)
         device.save()
-        self.create_attestation(
-            device, response.attestation_object, credential.response.client_data_json
-        )
+        self.create_attestation(device, response.attestation_object, credential.response.client_data_json)
         return device
 
     def _check_discoverable(self, original_data: dict) -> Optional[bool]:
         """Check the clientExtensionResults to determine if the credential was
         created as discoverable.
 
         SECURITY NOTE: clientExtensionResults is not signed by the
@@ -394,26 +384,22 @@
         response: VerifiedRegistration,
         parsed_credential: RegistrationCredential,
         original_data: dict,
     ):
         """Save the credential to the database."""
         discoverable = self._check_discoverable(original_data)
         transports = (
-            [x.value for x in parsed_credential.response.transports]
-            if parsed_credential.response.transports
-            else []
+            [x.value for x in parsed_credential.response.transports] if parsed_credential.response.transports else []
         )
 
         # We can't use the backup_eligible flag directly because it's not
         # exposed in the py_webauthn API. We can however infer it from the
         # credential device type. If it's a multi-device credential, it's backup
         # eligible.
-        backup_eligible = (
-            response.credential_device_type == CredentialDeviceType.MULTI_DEVICE
-        )
+        backup_eligible = response.credential_device_type == CredentialDeviceType.MULTI_DEVICE
         backup_state = response.credential_backed_up
 
         device = WebAuthnCredential(
             user=user,
             aaguid=response.aaguid,
             credential_id=response.credential_id,
             public_key=response.credential_public_key,
@@ -463,27 +449,24 @@
                 UserVerificationRequirement.REQUIRED
                 if require_user_verification
                 else UserVerificationRequirement.DISCOURAGED
             ),
         }
 
         if user:
-            kwargs["allow_credentials"] = (
-                WebAuthnCredential.get_credential_descriptors_for_user(user)
-            )
+            kwargs["allow_credentials"] = WebAuthnCredential.get_credential_descriptors_for_user(user)
 
         return kwargs
 
     def get_authentication_state(self, options: dict) -> dict:
         """Get the state to store during authentication. This state will be used
         to verify the authentication later on."""
         return {
             "challenge": options["challenge"],
-            "require_user_verification": options["userVerification"]
-            == UserVerificationRequirement.REQUIRED.value,
+            "require_user_verification": options["userVerification"] == UserVerificationRequirement.REQUIRED.value,
         }
 
     def authenticate_begin(
         self,
         user: Optional[AbstractUser] = None,
         require_user_verification: bool = True,
     ):
@@ -503,17 +486,15 @@
         # doesn't support this yet.
         extensions = self.get_authentication_extensions()
         data["extensions"] = extensions
 
         state = self.get_authentication_state(data)
         return data, state
 
-    def authenticate_complete(
-        self, user: Optional[AbstractUser], state: dict, data: dict
-    ):
+    def authenticate_complete(self, user: Optional[AbstractUser], state: dict, data: dict):
         """Complete the authentication process."""
 
         credential = parse_authentication_credential_json(data)
 
         try:
             device = WebAuthnCredential.get_by_credential_id(credential.raw_id)
         except WebAuthnCredential.DoesNotExist:
@@ -533,16 +514,16 @@
             credential=credential,
             credential_current_sign_count=device.sign_count,
             credential_public_key=device.public_key,
             expected_challenge=expected_challenge,
             expected_rp_id=expected_rp_id,
             expected_origin=expected_origins,
             require_user_verification=require_user_verification,
-            **kwargs
+            **kwargs,
         )
 
         device.sign_count = response.new_sign_count
         device.backup_state = response.credential_backed_up
-        device.update_last_used_at(commit=False)
+        device.set_last_used_timestamp(commit=False)
         device.save(update_fields=["sign_count", "last_used_at", "backup_state"])
 
         return device
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/nl/LC_MESSAGES/django.po` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/locale/nl/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,166 +4,158 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-12 13:16+0000\n"
+"POT-Creation-Date: 2024-05-26 18:48+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: src/django_otp_webauthn/admin.py:49
+#: src/django_otp_webauthn/admin.py:50
 msgid "credential ID"
 msgstr "credential ID"
 
-#: src/django_otp_webauthn/admin.py:50
+#: src/django_otp_webauthn/admin.py:51
 msgid "COSE public key"
 msgstr "Publieke COSE-sleutel"
 
-#: src/django_otp_webauthn/admin.py:70
+#: src/django_otp_webauthn/admin.py:71
 msgid "Identity"
 msgstr "Identiteit"
 
-#: src/django_otp_webauthn/admin.py:76
+#: src/django_otp_webauthn/admin.py:77
 msgid "Meta"
 msgstr "Meta-gegevens"
 
-#: src/django_otp_webauthn/admin.py:82
+#: src/django_otp_webauthn/admin.py:83
 msgid "WebAuthn credential data"
 msgstr "WebAuthn-gegevens"
 
 #: src/django_otp_webauthn/apps.py:11
 msgid "OTP WebAuthn"
 msgstr "OTP WebAuthn"
 
-#: src/django_otp_webauthn/exceptions.py:12
+#: src/django_otp_webauthn/exceptions.py:11
 msgid ""
 "State is missing or invalid. Please begin the operation first before trying "
 "to complete it."
 msgstr ""
 "Staat ontbreekt of is ongeldig. Begin de operatie eerst voordat u probeert "
 "deze te voltooien."
 
-#: src/django_otp_webauthn/exceptions.py:19
+#: src/django_otp_webauthn/exceptions.py:17
 msgid "Unprocessable Entity"
 msgstr "Onverwerkbare entiteit"
 
-#: src/django_otp_webauthn/exceptions.py:25
+#: src/django_otp_webauthn/exceptions.py:23
 msgid "Passwordless login is disabled."
 msgstr "Wachtwoordloze login is uitgeschakeld."
 
-#: src/django_otp_webauthn/exceptions.py:31
+#: src/django_otp_webauthn/exceptions.py:29
 msgid "Registration is disabled."
 msgstr "Registratie is uitgeschakeld."
 
-#: src/django_otp_webauthn/exceptions.py:37
+#: src/django_otp_webauthn/exceptions.py:35
 msgid "Authentication is disabled."
 msgstr "Authenticatie is uitgeschakeld."
 
-#: src/django_otp_webauthn/exceptions.py:43
+#: src/django_otp_webauthn/exceptions.py:41
 msgid "User is not logged in."
 msgstr "Gebruiker is niet ingelogd."
 
-#: src/django_otp_webauthn/exceptions.py:49
+#: src/django_otp_webauthn/exceptions.py:47
 msgid "This user account is marked as disabled."
 msgstr "Dit gebruikersaccount is gemarkeerd als uitgeschakeld."
 
-#: src/django_otp_webauthn/exceptions.py:55
+#: src/django_otp_webauthn/exceptions.py:53
 msgid "This Passkey has been marked as disabled."
 msgstr "Deze Passkey is gemarkeerd als uitgeschakeld."
 
-#: src/django_otp_webauthn/exceptions.py:62
+#: src/django_otp_webauthn/exceptions.py:59
 msgid "The Passkey you tried to use was not found. Perhaps it was removed?"
 msgstr ""
 "De Passkey die u probeert te gebruiken is niet gevonden. Misschien is deze "
 "verwijderd?"
 
-#: src/django_otp_webauthn/models.py:43
+#: src/django_otp_webauthn/models.py:42
 msgid "credential"
 msgstr "credential"
 
-#: src/django_otp_webauthn/models.py:48
+#: src/django_otp_webauthn/models.py:46
 msgid "format"
 msgstr "formaat"
 
-#: src/django_otp_webauthn/models.py:52
+#: src/django_otp_webauthn/models.py:49
 msgid "data"
 msgstr "data"
 
-#: src/django_otp_webauthn/models.py:56
+#: src/django_otp_webauthn/models.py:52
 msgid "client data JSON"
 msgstr "client data JSON"
 
-#: src/django_otp_webauthn/models.py:70
+#: src/django_otp_webauthn/models.py:65
 msgid "WebAuthn attestation"
 msgstr "WebAuthn attestatie"
 
-#: src/django_otp_webauthn/models.py:71
+#: src/django_otp_webauthn/models.py:66
 msgid "WebAuthn attestations"
 msgstr "WebAuthn attestaties"
 
-#: src/django_otp_webauthn/models.py:88
+#: src/django_otp_webauthn/models.py:83
 msgid "WebAuthn credential"
 msgstr "WebAuthn credential"
 
-#: src/django_otp_webauthn/models.py:89
+#: src/django_otp_webauthn/models.py:84
 msgid "WebAuthn credentials"
 msgstr "WebAuthn credentials"
 
-#: src/django_otp_webauthn/models.py:100
+#: src/django_otp_webauthn/models.py:95
 msgid "Public Key"
 msgstr "Publieke Sleutel"
 
-#: src/django_otp_webauthn/models.py:105
+#: src/django_otp_webauthn/models.py:100
 msgid "credential type"
 msgstr "type credential"
 
-#: src/django_otp_webauthn/models.py:118
+#: src/django_otp_webauthn/models.py:113
 msgid "credential id data"
 msgstr "credential id data"
 
-#: src/django_otp_webauthn/models.py:135
+#: src/django_otp_webauthn/models.py:129
 msgid "COSE public key data"
 msgstr "COSE publieke sleutel data"
 
-#: src/django_otp_webauthn/models.py:143
+#: src/django_otp_webauthn/models.py:136
 msgid "transports"
 msgstr "transports"
 
-#: src/django_otp_webauthn/models.py:163
+#: src/django_otp_webauthn/models.py:156
 msgid "sign count"
 msgstr "aantal ondertekeningen"
 
-#: src/django_otp_webauthn/models.py:178
+#: src/django_otp_webauthn/models.py:171
 msgid "backup eligible"
 msgstr "kan worden geback-upt"
 
-#: src/django_otp_webauthn/models.py:186
+#: src/django_otp_webauthn/models.py:179
 msgid "backup state"
 msgstr "back-up status"
 
-#: src/django_otp_webauthn/models.py:204
-msgid "created at"
-msgstr "aanmaakdatum"
-
-#: src/django_otp_webauthn/models.py:206
-msgid "last used at"
-msgstr "laatst gebruikt op"
-
-#: src/django_otp_webauthn/models.py:211
+#: src/django_otp_webauthn/models.py:197
 msgid "AAGUID"
 msgstr "AAGUID"
 
-#: src/django_otp_webauthn/models.py:226
+#: src/django_otp_webauthn/models.py:212
 msgid "hashed credential id"
 msgstr "gehashte credential id"
 
-#: src/django_otp_webauthn/models.py:235
+#: src/django_otp_webauthn/models.py:221
 msgid "discoverable"
 msgstr "zichtbaar"
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/locale/nl/LC_MESSAGES/djangojs.po` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/migrations/0001_initial.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/migrations/0001_initial.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
@@ -31,83 +30,65 @@
                     models.CharField(
                         help_text="The human-readable name of this device.",
                         max_length=64,
                     ),
                 ),
                 (
                     "confirmed",
-                    models.BooleanField(
-                        default=True, help_text="Is this device ready for use?"
-                    ),
+                    models.BooleanField(default=True, help_text="Is this device ready for use?"),
                 ),
                 (
                     "credential_type",
                     models.CharField(
                         choices=[("public-key", "Public Key")],
                         default="public-key",
                         editable=False,
                         max_length=32,
                         verbose_name="credential type",
                     ),
                 ),
                 (
                     "credential_id",
-                    models.BinaryField(
-                        max_length=1023, verbose_name="credential id data"
-                    ),
+                    models.BinaryField(max_length=1023, verbose_name="credential id data"),
                 ),
                 (
                     "public_key",
-                    models.BinaryField(
-                        max_length=1023, verbose_name="COSE public key data"
-                    ),
+                    models.BinaryField(max_length=1023, verbose_name="COSE public key data"),
                 ),
                 (
                     "transports",
-                    models.JSONField(
-                        default=list, editable=False, verbose_name="transports"
-                    ),
+                    models.JSONField(default=list, editable=False, verbose_name="transports"),
                 ),
                 (
                     "sign_count",
-                    models.PositiveIntegerField(
-                        default=0, editable=False, verbose_name="sign count"
-                    ),
+                    models.PositiveIntegerField(default=0, editable=False, verbose_name="sign count"),
                 ),
                 (
                     "backup_eligible",
-                    models.BooleanField(
-                        default=False, editable=False, verbose_name="backup eligible"
-                    ),
+                    models.BooleanField(default=False, editable=False, verbose_name="backup eligible"),
                 ),
                 (
                     "backup_state",
-                    models.BooleanField(
-                        default=False, editable=False, verbose_name="backup state"
-                    ),
+                    models.BooleanField(default=False, editable=False, verbose_name="backup state"),
                 ),
                 (
                     "created_at",
                     models.DateTimeField(auto_now_add=True, verbose_name="created at"),
                 ),
                 (
                     "last_used_at",
                     models.DateTimeField(null=True, verbose_name="last used at"),
                 ),
                 (
                     "aaguid",
-                    models.CharField(
-                        editable=False, max_length=36, verbose_name="AAGUID"
-                    ),
+                    models.CharField(editable=False, max_length=36, verbose_name="AAGUID"),
                 ),
                 (
                     "credential_id_sha256",
-                    models.BinaryField(
-                        max_length=32, unique=True, verbose_name="hashed credential id"
-                    ),
+                    models.BinaryField(max_length=32, unique=True, verbose_name="hashed credential id"),
                 ),
                 (
                     "discoverable",
                     models.BooleanField(
                         default=None,
                         editable=False,
                         null=True,
@@ -177,12 +158,10 @@
                 "verbose_name": "WebAuthn attestation",
                 "verbose_name_plural": "WebAuthn attestations",
                 "abstract": False,
             },
         ),
         migrations.AddIndex(
             model_name="webauthncredential",
-            index=models.Index(
-                fields=["credential_id_sha256"], name="webauthncredential_sha256_idx"
-            ),
+            index=models.Index(fields=["credential_id_sha256"], name="webauthncredential_sha256_idx"),
         ),
     ]
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/models.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import hashlib
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AbstractUser
 from django.db import models
 from django.http import HttpRequest
-from django.utils import timezone
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
-from django_otp.models import Device
+from django_otp.models import Device, TimestampMixin
 from webauthn.helpers import parse_attestation_object
 from webauthn.helpers.structs import (
     AttestationObject,
     AuthenticatorTransport,
     PublicKeyCredentialDescriptor,
 )
 
@@ -40,25 +39,21 @@
         to=get_credential_model_string(),
         on_delete=models.CASCADE,
         related_name="attestation",
         verbose_name=_("credential"),
         editable=False,
     )
 
-    fmt = models.CharField(
-        max_length=255, verbose_name=_("format"), editable=False, choices=Format.choices
-    )
+    fmt = models.CharField(max_length=255, verbose_name=_("format"), editable=False, choices=Format.choices)
     """The attestation format used by the authenticator. Extracted from the attestation object for convenience."""
 
     data = models.BinaryField(verbose_name=_("data"), editable=False)
     """The raw attestation data"""
 
-    client_data_json = models.BinaryField(
-        verbose_name=_("client data JSON"), editable=False
-    )
+    client_data_json = models.BinaryField(verbose_name=_("client data JSON"), editable=False)
     """The raw client data JSON, as originally sent by the client."""
 
     @cached_property
     def attestation_object(self) -> AttestationObject:
         """Return the parsed attestation object."""
         return parse_attestation_object(self.data)
 
@@ -67,15 +62,15 @@
 
     class Meta:
         abstract = True
         verbose_name = _("WebAuthn attestation")
         verbose_name_plural = _("WebAuthn attestations")
 
 
-class AbstractWebAuthnCredential(Device):
+class AbstractWebAuthnCredential(TimestampMixin, Device):
     """
     Abstract OTP device that validates against a user's WebAuthn credential.
 
     See https://www.w3.org/TR/webauthn-3/ for more information about the FIDO 2 Web Authentication standard.
     """
 
     class Meta:
@@ -127,17 +122,15 @@
     Previous revisions of the WebAuthn spec did not mention a maximum size for this field.
     The current L3 revision mentions a maximum size of 1023 bytes.
 
     See https://github.com/w3c/webauthn/pull/1664 for related discussion.
     """
 
     # https://www.w3.org/TR/webauthn-3/#abstract-opdef-credential-record-publickey
-    public_key = models.BinaryField(
-        max_length=1023, verbose_name=_("COSE public key data"), editable=False
-    )
+    public_key = models.BinaryField(max_length=1023, verbose_name=_("COSE public key data"), editable=False)
     """The public key of the credential, encoded in COSE_Key format (binary).
 
     Specification: https://www.rfc-editor.org/rfc/rfc9052#section-7
     """
 
     # https://www.w3.org/TR/webauthn-3/#abstract-opdef-credential-record-transports
     transports = models.JSONField(_("transports"), editable=False, default=list)
@@ -195,21 +188,14 @@
     # The idea behind uvInitialized is to keep track of whether this
     # authenticator supports user verification. Apparently, it is meant to be
     # used to influence policy decisions though it is unclear to me how this
     # would work exactly and what benefit it would bring. Our implementation
     # does not use this field. And because it appears it could be added later
     # without too much difficulty, we do not implement it yet.
 
-    # The following fields are not required or recommended by the WebAuthn L3
-    # specification, but are meaningful in our implementation.
-    created_at = models.DateTimeField(auto_now_add=True, verbose_name=_("created at"))
-    """When was this credential created."""
-    last_used_at = models.DateTimeField(null=True, verbose_name=_("last used at"))
-    """When was this credential last used successfully."""
-
     aaguid = models.CharField(
         max_length=36,
         verbose_name=_("AAGUID"),
         editable=False,
     )
     """The AAGUID of the authenticator. It can be used to identify the make and
     model of the authenticator but is often zeroed out to protect user
@@ -261,37 +247,33 @@
 
     For more information see:
     https://www.w3.org/TR/webauthn-3/#client-side-discoverable-public-key-credential-source
     """
 
     def save(self, *args, **kwargs):
         if not self.credential_id_sha256:
-            self.credential_id_sha256 = self.get_credential_id_sha256(
-                self.credential_id
-            )
+            self.credential_id_sha256 = self.get_credential_id_sha256(self.credential_id)
         super().save(*args, **kwargs)
 
     @classmethod
-    def get_by_credential_id(cls, credential_id) -> "WebAuthnCredential":
+    def get_by_credential_id(cls, credential_id: bytes) -> "WebAuthnCredential":
         """Return a WebAuthnCredential instance by its credential id.
 
         Will attempt to find a matching device by looking up the hash of the credential id.
         """
         hashed_credential_id = cls.get_credential_id_sha256(credential_id)
         return cls.objects.get(credential_id_sha256=hashed_credential_id)
 
     @classmethod
     def get_credential_id_sha256(cls, credential_id: bytes) -> bytes:
         """Return the SHA256 hash of the given credential id."""
         return hashlib.sha256(credential_id).digest()
 
     @classmethod
-    def get_credential_descriptors_for_user(
-        cls, user: AbstractUser
-    ) -> list[PublicKeyCredentialDescriptor]:
+    def get_credential_descriptors_for_user(cls, user: AbstractUser) -> list[PublicKeyCredentialDescriptor]:
         """Return a list of PublicKeyCredentialDescriptor objects for the given user.
 
         Each PublicKeyCredentialDescriptor object represents a credential that the
         user has registered.
 
         These descriptors are intended to inform the client about credential the
         user has registered with the server.
@@ -304,17 +286,16 @@
             # to the user. We don't explicitly keep track of preferred devices,
             # but we can make the assumption that the most recently used device
             # is most likely to be a preferred device.
             # Source: https://www.w3.org/TR/webauthn-3/#dom-publickeycredentialrequestoptions-allowcredentials
             # > The list is ordered in descending order of preference: the first
             # > item in the list is the most preferred credential, and the last
             # > is the least preferred.
-            .order_by(models.F("last_used_at").desc(nulls_last=True)).values_list(
-                "credential_id", "transports"
-            )
+            .order_by(models.F("last_used_at").desc(nulls_last=True))
+            .values_list("credential_id", "transports")
         )
 
         descriptors = []
         for id, raw_transports in queryset:
             transports = []
             for t in raw_transports:
                 # Though the spec recommends we SHOULD NOT modify the transports
@@ -327,33 +308,25 @@
                 # > When registering a new credential, the Relying Party SHOULD
                 # > store the value returned from getTransports(). When creating
                 # > a PublicKeyCredentialDescriptor for that credential, the
                 # > Relying Party SHOULD retrieve that stored value and set it
                 # > as the value of the transports member.
                 if t in AuthenticatorTransport:
                     transports.append(AuthenticatorTransport(t))
-            descriptors.append(
-                PublicKeyCredentialDescriptor(id=id, transports=transports)
-            )
+            descriptors.append(PublicKeyCredentialDescriptor(id=id, transports=transports))
         return descriptors
 
     @classmethod
     def get_provider(cls, request: HttpRequest):
         """Return the PyWebAuthnProvider instance for this device."""
         # Avoid circular imports
         from django_otp_webauthn.helpers import PyWebAuthnProvider
 
         return PyWebAuthnProvider(request=request)
 
-    def update_last_used_at(self, commit=True):
-        """Update the last used timestamp for this device."""
-        self.last_used_at = timezone.now()
-        if commit:
-            self.save(update_fields=["last_used_at"])
-
 
 class WebAuthnCredential(AbstractWebAuthnCredential):
     """A OTP device that validates against a user's credential.
 
     See https://www.w3.org/TR/webauthn-3/ for more information about the FIDO 2
     Web Authentication standard.
     """
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/settings.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/settings.py`

 * *Files identical despite different names*

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/templatetags/otp_webauthn.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/templatetags/otp_webauthn.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,30 +5,23 @@
 from django_otp_webauthn.settings import app_settings
 from django_otp_webauthn.utils import get_credential_model
 
 register = template.Library()
 
 WebAuthnCredential = get_credential_model()
 
+
 def get_configuration(extra_options: dict = {}) -> dict:
     configuration = {
         "autocompleteLoginFieldSelector": None,
         "csrfCookieName": settings.CSRF_COOKIE_NAME,
-        "beginAuthenticationUrl": reverse(
-            "otp_webauthn:credential-authentication-begin"
-        ),
-        "completeAuthenticationUrl": reverse(
-            "otp_webauthn:credential-authentication-complete"
-        ),
-        "beginRegistrationUrl": reverse(
-            "otp_webauthn:credential-registration-begin"
-        ),
-        "completeRegistrationUrl": reverse(
-            "otp_webauthn:credential-registration-complete"
-        ),
+        "beginAuthenticationUrl": reverse("otp_webauthn:credential-authentication-begin"),
+        "completeAuthenticationUrl": reverse("otp_webauthn:credential-authentication-complete"),
+        "beginRegistrationUrl": reverse("otp_webauthn:credential-registration-begin"),
+        "completeRegistrationUrl": reverse("otp_webauthn:credential-registration-complete"),
     }
     configuration.update(extra_options)
 
     return configuration
 
 
 @register.inclusion_tag("django_otp_webauthn/auth_scripts.html", takes_context=True)
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/urls.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         CompleteCredentialAuthenticationView.as_view(),
         name="credential-authentication-complete",
     ),
     path(
         "jsi18n/",
         JavaScriptCatalog.as_view(packages=["django_otp_webauthn"]),
         name="js-i18n-catalog",
-    )
+    ),
 ]
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/utils.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,15 @@
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.log_exception(exc_val)
         if exc_type is pywebauthn_exceptions.InvalidCBORData:
-            raise exceptions.UnprocessableEntity(
-                code="invalid_cbor", detail="Invalid CBOR data provided."
-            ) from exc_val
+            raise exceptions.UnprocessableEntity(code="invalid_cbor", detail="Invalid CBOR data provided.") from exc_val
         elif exc_type is pywebauthn_exceptions.InvalidRegistrationResponse:
             raise exceptions.UnprocessableEntity(
                 code="invalid_registration_response",
                 detail="Invalid registration response provided.",
             ) from exc_val
         elif exc_type is pywebauthn_exceptions.InvalidAuthenticationResponse:
             raise exceptions.UnprocessableEntity(
@@ -55,15 +53,18 @@
                 detail="There is a problem with the provided JSON data.",
             ) from exc_val
         elif exc_type is pywebauthn_exceptions.UnsupportedAlgorithm:
             raise exceptions.UnprocessableEntity(
                 code="unsupported_algorithm",
                 detail="The specified COSE algorithm is not supported by this server.",
             ) from exc_val
-        elif exc_type is pywebauthn_exceptions.UnsupportedPublicKey or exc_type is pywebauthn_exceptions.InvalidPublicKeyStructure:
+        elif (
+            exc_type is pywebauthn_exceptions.UnsupportedPublicKey
+            or exc_type is pywebauthn_exceptions.InvalidPublicKeyStructure
+        ):
             raise exceptions.UnprocessableEntity(
                 code="unsupported_public_key",
                 detail="The public key is malformed or not supported.",
             ) from exc_val
         elif exc_type is pywebauthn_exceptions.InvalidAuthenticatorDataStructure:
             raise exceptions.UnprocessableEntity(
                 code="invalid_authenticator_data_structure",
@@ -98,39 +99,31 @@
     ]
 
 
 def get_credential_model() -> "AbstractWebAuthnCredential":
     """Returns the WebAuthnCredential model that is active in this project."""
     # Inspired by Django's django.contrib.auth.get_user_model
     try:
-        return apps.get_model(
-            app_settings.OTP_WEBAUTHN_CREDENTIAL_MODEL, require_ready=False
-        )
+        return apps.get_model(app_settings.OTP_WEBAUTHN_CREDENTIAL_MODEL, require_ready=False)
     except ValueError:
-        raise ImproperlyConfigured(
-            "OTP_WEBAUTHN_CREDENTIAL_MODEL must be of the form 'app_label.model_name'"
-        )
+        raise ImproperlyConfigured("OTP_WEBAUTHN_CREDENTIAL_MODEL must be of the form 'app_label.model_name'")
     except LookupError:
         raise ImproperlyConfigured(
             f"OTP_WEBAUTHN_CREDENTIAL_MODEL refers to model '{app_settings.OTP_WEBAUTHN_CREDENTIAL_MODEL}' that has not been installed"
         )
 
 
 def get_attestation_model() -> "AbstractWebAuthnAttestation":
     """Returns the WebAuthnAttestation model that is active in this project."""
 
     # Inspired by Django's django.contrib.auth.get_user_model
     try:
-        return apps.get_model(
-            app_settings.OTP_WEBAUTHN_ATTESTATION_MODEL, require_ready=False
-        )
+        return apps.get_model(app_settings.OTP_WEBAUTHN_ATTESTATION_MODEL, require_ready=False)
     except ValueError:
-        raise ImproperlyConfigured(
-            "OTP_WEBAUTHN_ATTESTATION_MODEL must be of the form 'app_label.model_name'"
-        )
+        raise ImproperlyConfigured("OTP_WEBAUTHN_ATTESTATION_MODEL must be of the form 'app_label.model_name'")
     except LookupError:
         raise ImproperlyConfigured(
             f"OTP_WEBAUTHN_ATTESTATION_MODEL refers to model '{app_settings.OTP_WEBAUTHN_ATTESTATION_MODEL}' that has not been installed"
         )
 
 
 def get_credential_model_string() -> str:
```

### Comparing `django_otp_webauthn-0.1.0/src/django_otp_webauthn/views.py` & `django_otp_webauthn-0.1.1/src/django_otp_webauthn/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,15 @@
 
     def post(self, *args, **kwargs):
         user = self.user
 
         provider = WebAuthnCredential.get_provider(request=self.request)
         require_user_verification = not bool(user)
 
-        data, state = provider.authenticate_begin(
-            user=user, require_user_verification=require_user_verification
-        )
+        data, state = provider.authenticate_begin(user=user, require_user_verification=require_user_verification)
         self.request.session["otp_webauthn_authentication_state"] = state
 
         return Response(data=data, content_type="application/json")
 
 
 @method_decorator(never_cache, name="dispatch")
 class CompleteCredentialAuthenticationView(AuthenticationCeremonyMixin, APIView):
@@ -174,17 +172,15 @@
         You can override this method to implement your own custom logic. If you
         do, you should raise an exception if the user is not allowed to log in.
 
         Args:
             device (AbstractWebAuthnCredential): The device the user is trying to log
             in with.
         """
-        disallow_passwordless_login = (
-            not app_settings.OTP_WEBAUTHN_ALLOW_PASSWORDLESS_LOGIN
-        )
+        disallow_passwordless_login = not app_settings.OTP_WEBAUTHN_ALLOW_PASSWORDLESS_LOGIN
         if not device.confirmed:
             raise exceptions.CredentialDisabled()
 
         if self.get_user() is None and disallow_passwordless_login:
             raise exceptions.PasswordlessLoginDisabled()
 
         if not device.user.is_active:
```

### Comparing `django_otp_webauthn-0.1.0/PKG-INFO` & `django_otp_webauthn-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: django-otp-webauthn
-Version: 0.1.0
+Version: 0.1.1
 Summary: FIDO2 WebAuthn support for django-otp: lets your users authenticate with Passkeys
-License: BSD-3-Clause
-Author: Storm B. Heg
-Author-email: storm@stormbase.digital
-Requires-Python: >=3.10
+Project-URL: Changelog, https://github.com/Stormbase/django-otp-webauthn/blob/main/CHANGELOG.md
+Project-URL: Issues, https://github.com/Stormbase/django-otp-webauthn/issues
+Project-URL: Source, https://github.com/Stormbase/django-otp-webauthn
+Author-email: "Storm B. Heg" <storm@stormbase.digital>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
+Keywords: authentication,django,django-otp,fido2,mfa,security,u2f,webauthn
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: FIDO
 Classifier: Topic :: Security
-Requires-Dist: django (>=4.2,<6)
-Requires-Dist: django-otp (>=1.2)
-Requires-Dist: djangorestframework (>=3.14)
-Requires-Dist: webauthn (>=2.1.0,<3)
+Requires-Python: >=3.9
+Requires-Dist: django-otp<2.0,>=1.4
+Requires-Dist: django>=4.2
+Requires-Dist: djangorestframework>=3.14
+Requires-Dist: webauthn<3,>=2.1.0
 Description-Content-Type: text/markdown
 
 # Django OTP WebAuthn
 
 This package provides an implementation of [WebAuthn Passkeys](https://passkeys.dev/) for Django. It is written as a plugin for the [Django OTP framework](https://github.com/django-otp/django-otp) for multi-factor authentication. Under the hood, this package uses [py_webauth](https://github.com/duo-labs/py_webauthn/) to handle all cryptographic operations.
 
 > [!IMPORTANT]  
@@ -38,15 +43,15 @@
   - [Compatibility](#compatibility)
     - [Browser compatibility](#browser-compatibility)
   - [Features](#features)
   - [Quick start guide - how to use Passkeys in your Django project](#quick-start-guide---how-to-use-passkeys-in-your-django-project)
   - [What exactly is a Passkey?](#what-exactly-is-a-passkey)
     - [How Passkeys work (in a nutshell)](#how-passkeys-work-in-a-nutshell)
     - [Why use Passkeys?](#why-use-passkeys)
-      - [A note about security](#a-note-about-security)
+    - [A note about security](#a-note-about-security)
   - [Who uses Passkeys?](#who-uses-passkeys)
   - [Further reading](#further-reading)
   - [Development](#development)
   - [License](#license)
 
 ## Compatibility
 
@@ -221,15 +226,15 @@
 3. The server looks up the public key associated with the given credential ID and uses it to check the signature. Was this signature generated by the private key that belongs to the public key we have on file? If yes, the user must be in possession of the private key and is authenticated.
 
 ### Why use Passkeys?
 
 - **Security.** Compared to passwords, Passkeys are resistant to phishing attacks, credential stuffing, and other common attacks.
 - **Convenience.** Passkeys are more convenient than passwords. Users don't have to choose and remember a password, they can use their phone, laptop, or security key to authenticate. Compared to other traditional forms of Multi Factor Authentication, there is no need to wait for an SMS code to arrive or copy a code from an authenticator app. Just click yes on the browser prompt.
 
-#### A note about security
+### A note about security
 
 Passkeys are sometimes claimed to be silver bullet for security. While they are more secure than passwords, they are not perfect.
 
 You put trust in the user's device and its manufacturer. Most devices support some form is syncing Passkeys between devices, like through an iCloud or Google account. This means that if someone gains access to the users' iCloud or Google account, they could potentially access their Passkeys. Users that have poorly secured their account and devices are at risk. However, this is not unique to Passkeys. The same risks exists for password managers and other forms of Multi Factor Authentication that support syncing between devices. Passkeys improve over other methods by their resistance to phishing attacks, credential stuffing and their convenience.
 
 It is the author's opinion that the benefits of Passkeys outweigh the risks. This section is here for your own consideration.
 
@@ -255,8 +260,7 @@
 ## Development
 
 See [DEVELOPMENT.md](DEVELOPMENT.md) for information on how to develop and contribute to this project.
 
 ## License
 
 This project is licensed under the BSD 3-Clause License. See the [LICENSE](LICENSE) file for details.
-
```

