# Comparing `tmp/netbox_otp_plugin-1.0.7-py3-none-any.whl.zip` & `tmp/netbox_otp_plugin-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7396 bytes, number of entries: 12
--rw-rw-r--  2.0 unx     1628 b- defN 23-Jun-13 12:09 netbox_otp_plugin/__init__.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-May-29 18:20 netbox_otp_plugin/forms.py
--rw-rw-r--  2.0 unx      453 b- defN 23-Jun-12 06:53 netbox_otp_plugin/middleware.py
--rw-rw-r--  2.0 unx      141 b- defN 23-May-29 18:20 netbox_otp_plugin/urls.py
+Zip file size: 7344 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx     1514 b- defN 24-May-26 12:01 netbox_otp_plugin/__init__.py
+-rw-rw-r--  2.0 unx     1016 b- defN 24-May-26 07:34 netbox_otp_plugin/forms.py
+-rw-rw-r--  2.0 unx      453 b- defN 24-May-26 06:16 netbox_otp_plugin/middleware.py
+-rw-rw-r--  2.0 unx      141 b- defN 24-May-26 06:16 netbox_otp_plugin/urls.py
 -rw-rw-r--  2.0 unx     4417 b- defN 23-May-29 18:20 netbox_otp_plugin/views.py
 -rw-rw-r--  2.0 unx      880 b- defN 23-May-29 18:20 netbox_otp_plugin/management/commands/addtotp.py
 -rw-rw-r--  2.0 unx      831 b- defN 23-May-29 18:20 netbox_otp_plugin/management/commands/resettotp.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-May-29 18:20 netbox_otp_plugin/templates/otp_login.html
--rw-rw-r--  2.0 unx      312 b- defN 23-Jun-13 12:09 netbox_otp_plugin-1.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 12:09 netbox_otp_plugin-1.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Jun-13 12:09 netbox_otp_plugin-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-13 12:09 netbox_otp_plugin-1.0.7.dist-info/RECORD
-12 files, 13347 bytes uncompressed, 5572 bytes compressed:  58.3%
+-rw-rw-r--  2.0 unx     3362 b- defN 24-May-26 07:29 netbox_otp_plugin/templates/otp_login.html
+-rw-rw-r--  2.0 unx      312 b- defN 24-May-26 12:21 netbox_otp_plugin-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-26 12:21 netbox_otp_plugin-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 24-May-26 12:21 netbox_otp_plugin-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 24-May-26 12:21 netbox_otp_plugin-1.1.0.dist-info/RECORD
+12 files, 14102 bytes uncompressed, 5520 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: netbox_otp_plugin/management/commands/resettotp.py
 Comment: 
 
 Filename: netbox_otp_plugin/templates/otp_login.html
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.7.dist-info/METADATA
+Filename: netbox_otp_plugin-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.7.dist-info/WHEEL
+Filename: netbox_otp_plugin-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.7.dist-info/top_level.txt
+Filename: netbox_otp_plugin-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: netbox_otp_plugin-1.0.7.dist-info/RECORD
+Filename: netbox_otp_plugin-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netbox_otp_plugin/__init__.py

```diff
@@ -1,30 +1,28 @@
 import importlib
 from django.core.exceptions import ImproperlyConfigured
 
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 import netbox.settings as netbox_settings
 
 if importlib.util.find_spec('django_otp') is None:
     raise ImproperlyConfigured(
         f"netbox_otp_plugin is enabled but django_otp is not present. It can be "
         f"installed by running 'pip install django_otp qrcode'." 
     )
 
 netbox_settings.INSTALLED_APPS.extend(['django_otp','django_otp.plugins.otp_totp'])
-if hasattr(netbox_settings, "AUTH_EXEMPT_PATHS"):
-    netbox_settings.AUTH_EXEMPT_PATHS = netbox_settings.AUTH_EXEMPT_PATHS + (f'/{netbox_settings.BASE_PATH}plugins/otp',)
-else:
-    netbox_settings.EXEMPT_PATHS = netbox_settings.EXEMPT_PATHS + (f'/{netbox_settings.BASE_PATH}plugins/otp',)
+# the plugin login URL must be exempt from authentication
+netbox_settings.AUTH_EXEMPT_PATHS = netbox_settings.AUTH_EXEMPT_PATHS + (f'/{netbox_settings.BASE_PATH}plugins/otp',)
 
 class OTPPluginConfig(PluginConfig):
     name = 'netbox_otp_plugin'
     verbose_name = 'OTP Login'
     description = 'OTP Login plugin'
-    version = '1.0.7'
+    version = '1.1.0'
     author = 'Andrey Shalashov'
     author_email = 'avshalashov@yandex.ru'
     base_url = 'otp'
     required_settings = []
     default_settings = {
         'otp_required': True,
         'issuer': 'Netbox'
```

## netbox_otp_plugin/forms.py

```diff
@@ -1,25 +1,24 @@
 from django import forms
 from django.conf import settings
 from django.contrib.auth.forms import AuthenticationForm
 from django_otp.forms import OTPAuthenticationFormMixin
 from django_otp import user_has_device
-from utilities.forms import BootstrapMixin
 
 class OTPAuthenticationForm(OTPAuthenticationFormMixin, AuthenticationForm):
     otp_device = forms.CharField(required=False, widget=forms.Select)
     otp_token = forms.CharField(required=False, widget=forms.TextInput(attrs={'autocomplete': 'off', 'class': 'rounded'}), label="OTP Token")
     otp_challenge = forms.CharField(required=False)
 
     def clean(self):
         self.cleaned_data = super().clean()
         user = self.get_user()
-        # use get_plugin_config from extras.plugins better
+        # use get_plugin_config from netbox.plugins better
         plugin_config = settings.PLUGINS_CONFIG['netbox_otp_plugin'] 
         otp_required = plugin_config.get('otp_required')
         if user_has_device(user) or otp_required:
             self.clean_otp(self.get_user())
 
         return self.cleaned_data
 
-class OTPLoginForm(BootstrapMixin, OTPAuthenticationForm):
+class OTPLoginForm(OTPAuthenticationForm):
     pass
```

## netbox_otp_plugin/templates/otp_login.html

```diff
@@ -1,81 +1,103 @@
 {# User login page. Extends base.html directly to override normal UI layout. #}
 {% extends 'base/base.html' %}
 {% load form_helpers %}
 {% load static %}
+{% load i18n %}
 
 {% block layout %}
-  <main class="login-container text-center">
 
-    {# Login banner #}
-    {% if config.BANNER_LOGIN %}
-      <div class="mw-90 mw-md-75 mw-lg-80 mw-xl-75 mw-xxl-50">
-        {{ config.BANNER_LOGIN|safe }}
-      </div>
-    {% endif %}
+  <div class="page page-center">
+    <div class="container container-tight py-4">
 
-    {# Login form errors #}
-    {% if form.non_field_errors %}
-      <div class="alert alert-danger" role="alert">
-        <h4 class="alert-heading">Errors</h4>
-        <p>
-          {{ form.non_field_errors }}
-        </p>
+      {# NetBox logo #}
+      <div class="text-center mb-4">
+        <img src="{% static 'netbox_logo.svg' %}" height="80" alt="{% trans "NetBox logo" %}" />
       </div>
-    {% endif %}
 
-    {# Login form #}
-    <div class="form-login">
-      <form method="post">
-        {% csrf_token %}
-
-        {# Logo #}
-        <div class="mb-4">
-          <img src="{% static 'netbox_logo.svg' %}" height="80" alt="NetBox logo" />
+      {# Login banner #}
+      {% if config.BANNER_LOGIN %}
+        <div class="mb-5 text-center">
+          {{ config.BANNER_LOGIN|safe }}
+        </div>
+      {% endif %}
+
+      {# Login form errors #}
+      {% if form.non_field_errors %}
+        <div class="alert alert-danger" role="alert">
+          <h4 class="alert-heading">{% trans "Errors" %}</h4>
+          <p>
+            {{ form.non_field_errors }}
+          </p>
+        </div>
+      {% endif %}
+
+      <div class="card card-md">
+        <div class="card-body">
+          <h2 class="text-center mb-4">{% trans "Log In" %}</h2>
+
+          {# Login form #}
+          <form method="post">
+            {% csrf_token %}
+
+            {# Set post-login URL #}
+            {% if 'next' in request.GET %}
+              <input type="hidden" name="next" value="{{ request.GET.next }}" />
+            {% elif 'next' in request.POST %}
+              <input type="hidden" name="next" value="{{ request.POST.next }}" />
+            {% endif %}
+
+            <div class="form-group mb-3">
+              <label for="id_username" class="form-label">{{ form.username.label }}</label>
+              {{ form.username }}
+              {% for error in form.username.errors %}
+                <div class="alert alert-danger">{{ error }}</div>
+              {% endfor %}
+            </div>
+
+            <div class="form-group">
+              <label for="id_password" class="form-label">{{ form.password.label }}</label>
+              {{ form.password }}
+              {% for error in form.password.errors %}
+                <div class="alert alert-danger">{{ error }}</div>
+              {% endfor %}
+            </div>
+
+            <div class="form-group mb-3">
+              <label for="id_otp_token" class="form-label">{{ form.otp_token.label }}</label>
+              {{ form.otp_token }}
+              {% for error in form.otp_token.errors %}
+                <div class="alert alert-danger">{{ error }}</div>
+              {% endfor %}
+            </div>
+
+            <div class="form-footer">
+              <button type="submit" class="btn btn-primary w-100">
+                {% trans "Sign In" %}
+              </button>
+            </div>
+          </form>
         </div>
 
-        {# Set post-login URL #}
-        {% if 'next' in request.GET %}
-        <input type="hidden" name="next" value="{{ request.GET.next }}" />
-        {% endif %} {% if 'next' in request.POST %}
-        <input type="hidden" name="next" value="{{ request.POST.next }}" />
+        {# SSO login #}
+        {% if auth_backends %}
+          <div class="hr-text">{% trans "Or" context "Denotes an alternative option" %}</div>
+          <div class="card-body">
+            <div class="row">
+              {% for backend in auth_backends %}
+                <div class="col">
+                  <a href="{{ backend.url }}" class="btn w-100">
+                    {% if backend.icon_name %}<i class="mdi mdi-{{ backend.icon_name }}"></i>{% endif %}
+                    {{ backend.display_name }}
+                  </a>
+                </div>
+              {% endfor %}
+            </div>
+          </div>
         {% endif %}
 
-        {{ form.username }}
-        {{ form.password }}
-        {{ form.otp_token }}
-
-        <button type="submit" class="btn btn-primary btn-lg w-100 mt-4">
-          Sign In
-        </button>
-      </form>
-    </div>
-    {% if auth_backends %}
-      <h6 class="mt-4 mb-3">Or use a single sign-on (SSO) provider:</h6>
-      {% for backend in auth_backends %}
-        <h5>
-          {% if backend.icon_name %}<i class="mdi mdi-{{ backend.icon_name }}"></i>{% endif %}
-          <a href="{{ backend.url }}" class="my-2">{{ backend.display_name }}</a>
-        </h5>
-      {% endfor %}
-    {% endif %}
-
-  </main>
-
-  {# Page footer #}
-  <footer class="footer container-fluid login-footer p-3">
-    <div class="row align-items-center w-100">
-      <div class="col-2 col-md-1 mb-0">
-        <button type="button" class="btn btn-sm color-mode-toggle" title="Toggle Color Mode">
-          <i class="color-mode-icon mdi mdi-lightbulb"></i>&nbsp;
-        </button>
-      </div>
-      <div class="col-1 col-md-auto mb-0"></div>
-      <div class="col text-end mb-0">
-        <small class="text-muted">
-          {{ settings.HOSTNAME }} (v{{ settings.VERSION }})
-        </small>
       </div>
+
     </div>
-  </footer>
+  </div>
 
 {% endblock layout %}
```

### html2text {}

```diff
@@ -1,21 +1,35 @@
 {# User login page. Extends base.html directly to override normal UI layout. #}
 {% extends 'base/base.html' %} {% load form_helpers %} {% load static %} {%
-block layout %} {# Login banner #} {% if config.BANNER_LOGIN %}
+load i18n %} {% block layout %}
+{# NetBox logo #}
+}" />
+{# Login banner #} {% if config.BANNER_LOGIN %}
 {{ config.BANNER_LOGIN|safe }}
 {% endif %} {# Login form errors #} {% if form.non_field_errors %}
-****** EErrrroorrss ******
+****** {{%% ttrraannss ""EErrrroorrss"" %%}} ******
 {{ form.non_field_errors }}
-{% endif %} {# Login form #}
-{% csrf_token %} {# Logo #}
-[NetBox logo]
-{# Set post-login URL #} {% if 'next' in request.GET %} {% endif %} {% if
-'next' in request.POST %} {% endif %} {{ form.username }} {{ form.password }} {
-{ form.otp_token }} Sign In
-{% if auth_backends %}
-** OOrr uussee aa ssiinnggllee ssiiggnn--oonn ((SSSSOO)) pprroovviiddeerr:: **
+{% endif %}
+********** {{%% ttrraannss ""LLoogg IInn"" %%}} **********
+{# Login form #}
+{% csrf_token %} {# Set post-login URL #} {% if 'next' in request.GET %} {%
+elif 'next' in request.POST %} {% endif %}
+{{ form.username.label }} {{ form.username }} {% for error in
+form.username.errors %}
+{{ error }}
+{% endfor %}
+{{ form.password.label }} {{ form.password }} {% for error in
+form.password.errors %}
+{{ error }}
+{% endfor %}
+{{ form.otp_token.label }} {{ form.otp_token }} {% for error in
+form.otp_token.errors %}
+{{ error }}
+{% endfor %}
+{% trans "Sign In" %}
+{# SSO login #} {% if auth_backends %}
+{% trans "Or" context "Denotes an alternative option" %}
 {% for backend in auth_backends %}
-{{%% iiff bbaacckkeenndd..iiccoonn__nnaammee %%}}{{%% eennddiiff %%}} _{{_{{_ _bb_aa_cc_kk_ee_nn_dd_.._dd_ii_ss_pp_ll_aa_yy____nn_aa_mm_ee_ _}}_}}
-{% endfor %} {% endif %} {# Page footer #}
- 
-{{ settings.HOSTNAME }} (v{{ settings.VERSION }})
+_{_%_ _i_f_ _b_a_c_k_e_n_d_._i_c_o_n___n_a_m_e_ _%_}_{_%_ _e_n_d_i_f_ _%_}_ _{_{_ _b_a_c_k_e_n_d_._d_i_s_p_l_a_y___n_a_m_e_ _}_}
+{% endfor %}
+{% endif %}
 {% endblock layout %}
```

## Comparing `netbox_otp_plugin-1.0.7.dist-info/RECORD` & `netbox_otp_plugin-1.1.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-netbox_otp_plugin/__init__.py,sha256=q-j8Sg0dnuN-OGAzk3zPOKKltBZo-7cutkBidVryY1U,1628
-netbox_otp_plugin/forms.py,sha256=dbQkE1P8Q8zsHPWs46QxJxKlIyUZilR2_6swMxdqoxE,1075
+netbox_otp_plugin/__init__.py,sha256=fMEN57U1pmkGOweE7lGZu629wWc0dNqJ5kwQXHQrWGw,1514
+netbox_otp_plugin/forms.py,sha256=8zzcVN-TKxUt7g5zzFlqbvHdumaJGuYLDKHKo0lSfPc,1016
 netbox_otp_plugin/middleware.py,sha256=Pja6J7oTsIpY96MsF_VG2P742GRsC9NWkg7R2ySDDlw,453
 netbox_otp_plugin/urls.py,sha256=Y9px4QUdp6URAa6gzwckIAGVkvMleLy6Bihtxfbszyc,141
 netbox_otp_plugin/views.py,sha256=zrDaMQyv3YCoEiF6igzgtgQu3QvvNEx2VbTZ6Hz7i1A,4417
 netbox_otp_plugin/management/commands/addtotp.py,sha256=45ydKm7XtDhBnFOh1x2qRZzCAexYNQxHQKsdOZapIys,880
 netbox_otp_plugin/management/commands/resettotp.py,sha256=zuQVQwsTVDcumDFoolOkVcPinZ9kwwTy4zUXBnqp_Lg,831
-netbox_otp_plugin/templates/otp_login.html,sha256=Qjkx2tL_UjPvU00ynlD7WpJF0iQoUTn-Chl8iFaNHjM,2434
-netbox_otp_plugin-1.0.7.dist-info/METADATA,sha256=zRS6WNB3BXYqXkxiEZ9j24w4E6-JPWVj0iHeB4ginrk,312
-netbox_otp_plugin-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-netbox_otp_plugin-1.0.7.dist-info/top_level.txt,sha256=T322x6_TOk3lbaU-efVeIjMvWZQ5QiqFTFIeGhX8JlE,18
-netbox_otp_plugin-1.0.7.dist-info/RECORD,,
+netbox_otp_plugin/templates/otp_login.html,sha256=CVH1j1qnmk0IAd4tyPOaZGCAs2cNybDPWVgQPKAGbPA,3362
+netbox_otp_plugin-1.1.0.dist-info/METADATA,sha256=FRtWXh9kHkC0kq05L-0yWOfquHhgCn004S5gi6CyOrI,312
+netbox_otp_plugin-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+netbox_otp_plugin-1.1.0.dist-info/top_level.txt,sha256=T322x6_TOk3lbaU-efVeIjMvWZQ5QiqFTFIeGhX8JlE,18
+netbox_otp_plugin-1.1.0.dist-info/RECORD,,
```

