# Comparing `tmp/pretix-sumup-payment-1.1.2.tar.gz` & `tmp/pretix_sumup_payment-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sumup-payment-1.1.2.tar", last modified: Sun Jan 28 05:45:08 2024, max compression
+gzip compressed data, was "pretix_sumup_payment-1.1.4.tar", last modified: Sun May 26 18:30:43 2024, max compression
```

## Comparing `pretix-sumup-payment-1.1.2.tar` & `pretix_sumup_payment-1.1.4.tar`

### file list

```diff
@@ -1,43 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.550247 pretix-sumup-payment-1.1.2/
--rw-rw-rw-   0        0        0      575 2024-01-21 06:19:06.000000 pretix-sumup-payment-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      167 2024-01-21 06:19:06.000000 pretix-sumup-payment-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1844 2024-01-28 05:45:08.550247 pretix-sumup-payment-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2024-01-23 15:51:20.000000 pretix-sumup-payment-1.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.533857 pretix-sumup-payment-1.1.2/pretix_sumup/
--rw-rw-rw-   0        0        0       23 2024-01-28 04:32:11.000000 pretix-sumup-payment-1.1.2/pretix_sumup/__init__.py
--rw-rw-rw-   0        0        0      721 2024-01-22 16:25:57.000000 pretix-sumup-payment-1.1.2/pretix_sumup/apps.py
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.533857 pretix-sumup-payment-1.1.2/pretix_sumup/locale/
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.506050 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de/
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.535864 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2502 2024-01-28 04:31:45.000000 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3622 2024-01-28 04:34:16.000000 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.536864 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2024-01-21 06:19:06.000000 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.539383 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2487 2024-01-28 04:31:45.000000 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3607 2024-01-28 04:34:07.000000 pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     2855 2024-01-28 04:31:37.000000 pretix-sumup-payment-1.1.2/pretix_sumup/locale/django.pot
--rw-rw-rw-   0        0        0    13978 2024-01-28 04:33:56.000000 pretix-sumup-payment-1.1.2/pretix_sumup/payment.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:41:03.000000 pretix-sumup-payment-1.1.2/pretix_sumup/signals.py
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.508371 pretix-sumup-payment-1.1.2/pretix_sumup/static/
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.540384 pretix-sumup-payment-1.1.2/pretix_sumup/static/pretix_sumup/
--rw-rw-rw-   0        0        0        0 2024-01-21 06:19:06.000000 pretix-sumup-payment-1.1.2/pretix_sumup/static/pretix_sumup/.gitkeep
--rw-rw-rw-   0        0        0     3405 2024-01-24 13:37:40.000000 pretix-sumup-payment-1.1.2/pretix_sumup/sumup_client.py
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.509668 pretix-sumup-payment-1.1.2/pretix_sumup/templates/
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.543048 pretix-sumup-payment-1.1.2/pretix_sumup/templates/pretix_sumup/
--rw-rw-rw-   0        0        0      295 2024-01-28 04:33:56.000000 pretix-sumup-payment-1.1.2/pretix_sumup/templates/pretix_sumup/control.html
--rw-rw-rw-   0        0        0     2954 2024-01-24 14:06:19.000000 pretix-sumup-payment-1.1.2/pretix_sumup/templates/pretix_sumup/payment_widget.html
--rw-rw-rw-   0        0        0       80 2024-01-24 13:37:40.000000 pretix-sumup-payment-1.1.2/pretix_sumup/templates/pretix_sumup/pending.html
--rw-rw-rw-   0        0        0      439 2024-01-23 18:47:03.000000 pretix-sumup-payment-1.1.2/pretix_sumup/urls.py
--rw-rw-rw-   0        0        0     3390 2024-01-24 14:16:19.000000 pretix-sumup-payment-1.1.2/pretix_sumup/views.py
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.549247 pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/
--rw-rw-rw-   0        0        0     1844 2024-01-28 05:45:08.000000 pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-01-28 05:45:08.000000 pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-28 05:45:08.000000 pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-01-28 05:45:08.000000 pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-01-28 05:45:08.000000 pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      992 2024-01-23 15:52:00.000000 pretix-sumup-payment-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      887 2024-01-28 05:45:08.551674 pretix-sumup-payment-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-01-21 06:19:06.000000 pretix-sumup-payment-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-28 05:45:08.548240 pretix-sumup-payment-1.1.2/tests/
--rw-rw-rw-   0        0        0       75 2024-01-21 06:19:06.000000 pretix-sumup-payment-1.1.2/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.860017 pretix_sumup_payment-1.1.4/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.816406 pretix_sumup_payment-1.1.4/.github/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.833966 pretix_sumup_payment-1.1.4/.github/workflows/
+-rw-rw-rw-   0        0        0     3132 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/.github/workflows/style.yml
+-rw-rw-rw-   0        0        0      963 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/.github/workflows/tests.yml
+-rw-rw-rw-   0        0        0      868 2024-01-22 09:46:12.000000 pretix_sumup_payment-1.1.4/.gitignore
+-rw-rw-rw-   0        0        0      546 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/.install-hooks.sh
+-rw-rw-rw-   0        0        0      610 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/.update-locales.sh
+-rw-rw-rw-   0        0        0      575 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      167 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      281 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/Makefile
+-rw-rw-rw-   0        0        0     1844 2024-05-26 18:30:43.859022 pretix_sumup_payment-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2024-01-23 15:51:20.000000 pretix_sumup_payment-1.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.841018 pretix_sumup_payment-1.1.4/pretix_sumup/
+-rw-rw-rw-   0        0        0       23 2024-05-26 18:27:30.000000 pretix_sumup_payment-1.1.4/pretix_sumup/__init__.py
+-rw-rw-rw-   0        0        0      721 2024-01-28 06:16:55.000000 pretix_sumup_payment-1.1.4/pretix_sumup/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.841925 pretix_sumup_payment-1.1.4/pretix_sumup/locale/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.817405 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.843916 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2502 2024-01-28 04:31:45.000000 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3622 2024-01-28 04:34:16.000000 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.845028 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.846012 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2487 2024-01-28 04:31:45.000000 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3607 2024-01-28 04:34:07.000000 pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     2855 2024-01-28 04:31:37.000000 pretix_sumup_payment-1.1.4/pretix_sumup/locale/django.pot
+-rw-rw-rw-   0        0        0    14019 2024-05-26 18:24:47.000000 pretix_sumup_payment-1.1.4/pretix_sumup/payment.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:41:03.000000 pretix_sumup_payment-1.1.4/pretix_sumup/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.819406 pretix_sumup_payment-1.1.4/pretix_sumup/static/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.846962 pretix_sumup_payment-1.1.4/pretix_sumup/static/pretix_sumup/
+-rw-rw-rw-   0        0        0        0 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/pretix_sumup/static/pretix_sumup/.gitkeep
+-rw-rw-rw-   0        0        0     3405 2024-01-24 13:37:40.000000 pretix_sumup_payment-1.1.4/pretix_sumup/sumup_client.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.820407 pretix_sumup_payment-1.1.4/pretix_sumup/templates/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.850022 pretix_sumup_payment-1.1.4/pretix_sumup/templates/pretix_sumup/
+-rw-rw-rw-   0        0        0      295 2024-01-28 04:33:56.000000 pretix_sumup_payment-1.1.4/pretix_sumup/templates/pretix_sumup/control.html
+-rw-rw-rw-   0        0        0     2954 2024-01-24 14:06:19.000000 pretix_sumup_payment-1.1.4/pretix_sumup/templates/pretix_sumup/payment_widget.html
+-rw-rw-rw-   0        0        0       80 2024-01-24 13:37:40.000000 pretix_sumup_payment-1.1.4/pretix_sumup/templates/pretix_sumup/pending.html
+-rw-rw-rw-   0        0        0      439 2024-01-23 18:47:03.000000 pretix_sumup_payment-1.1.4/pretix_sumup/urls.py
+-rw-rw-rw-   0        0        0     3390 2024-01-24 14:16:19.000000 pretix_sumup_payment-1.1.4/pretix_sumup/views.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.859022 pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/
+-rw-rw-rw-   0        0        0     1844 2024-05-26 18:30:43.000000 pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2024-05-26 18:30:43.000000 pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:30:43.000000 pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-05-26 18:30:43.000000 pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-05-26 18:30:43.000000 pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/pretixplugin.toml
+-rw-rw-rw-   0        0        0      992 2024-05-26 18:23:02.000000 pretix_sumup_payment-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      887 2024-05-26 18:30:43.939673 pretix_sumup_payment-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-05-26 18:23:02.000000 pretix_sumup_payment-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:30:43.856957 pretix_sumup_payment-1.1.4/tests/
+-rw-rw-rw-   0        0        0       33 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/tests/conftest.py
+-rw-rw-rw-   0        0        0       75 2024-01-21 06:19:06.000000 pretix_sumup_payment-1.1.4/tests/test_main.py
```

### Comparing `pretix-sumup-payment-1.1.2/LICENSE` & `pretix_sumup_payment-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/PKG-INFO` & `pretix_sumup_payment-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup-payment
-Version: 1.1.2
+Version: 1.1.4
 Summary: Enables creditcard payments via Sumup
 Author-email: Christoph Walcher <chris@wiomoc.de>
 Maintainer-email: Christoph Walcher <chris@wiomoc.de>
 License: Apache
 Project-URL: homepage, https://github.com/wiomoc/pretix-sumup-payment
 Project-URL: repository, https://github.com/wiomoc/pretix-sumup-payment
 Keywords: pretix
```

### Comparing `pretix-sumup-payment-1.1.2/README.rst` & `pretix_sumup_payment-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/apps.py` & `pretix_sumup_payment-1.1.4/pretix_sumup/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/locale/de/LC_MESSAGES/django.mo` & `pretix_sumup_payment-1.1.4/pretix_sumup/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/locale/de/LC_MESSAGES/django.po` & `pretix_sumup_payment-1.1.4/pretix_sumup/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.mo` & `pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_sumup_payment-1.1.4/pretix_sumup/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/locale/django.pot` & `pretix_sumup_payment-1.1.4/pretix_sumup/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/payment.py` & `pretix_sumup_payment-1.1.4/pretix_sumup/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                         widget=forms.TextInput(
                             attrs={
                                 "maxlength": 10,
                                 "readonly": "readonly",
                                 "placeholder": _("Automatically filled in"),
                             }
                         ),
+                        required=False,
                         label=_("Merchant Code"),
                     ),
                 ),
             ]
             + list(super().settings_form_fields.items())
         )
```

#### html2text {}

```diff
@@ -11,53 +11,53 @@
 SumUp") public_name = _("Credit card") abort_pending_allowed = True @property
 def settings_form_fields(self): d = OrderedDict( [ ( "access_token",
 SecretKeySettingsField( label=_("API Key"), required=True, help_text=_( "API
 keys are authorization tokens that allow pretix to call SumUp on your behalf. "
 '_C_l_i_c_k_ _h_e_r_e_ _t_o_ _'_ _"_m_a_n_a_g_e_ _A_P_I_ _K_e_y_s_ _i_n_ _S_u_m_U_p" ), validators=(StripeKeyValidator
 ("sup_sk_"),), ), ), ( "merchant_code", forms.CharField( widget=forms.TextInput
 ( attrs={ "maxlength": 10, "readonly": "readonly", "placeholder": _
-("Automatically filled in"), } ), label=_("Merchant Code"), ), ), ] + list
-(super().settings_form_fields.items()) ) d.move_to_end("_enabled", last=False)
-return d def settings_form_clean(self, cleaned_data: dict): cleaned_data =
-super().settings_form_clean(cleaned_data) access_token = cleaned_data.get
-("payment_sumup_access_token") if access_token is None: # access token was
-already validated and turned out to be invalid return cleaned_data
-merchant_code = sumup_client.validate_access_token_and_get_merchant_code
-( access_token ) cleaned_data["payment_sumup_merchant_code"] = merchant_code
-return cleaned_data def is_allowed(self, request: HttpRequest, total: Decimal =
-None): if total is None: return True # minimum amount is 1 EUR or similar in
-other currencies return total >= 1 def execute_payment(self, request:
-HttpRequest, payment: OrderPayment): payment_id = payment.local_id order =
-payment.order event = order.event has_valid_checkout =
-self._synchronize_payment_status(payment) if has_valid_checkout: return try:
-checkout_id = sumup_client.create_checkout( checkout_reference=f"{event.slug}/
-{order.code}/{payment_id}", amount=payment.amount, currency=event.currency,
-description=f"{event.name} #{order.code}", merchant_code=self.settings.get
-("merchant_code"), return_url=build_absolute_uri( event, "plugins:pretix_sumup:
-checkout_event", kwargs={"payment": payment.pk}, ),
-access_token=self.settings.get("access_token"), ) info_data = payment.info_data
-info_data["sumup_checkout_id"] = checkout_id payment.info_data = info_data
-payment.save() except Exception as err: internal_exception_message = f"Error
-while creating SumUp checkout: {err}" payment.fail
-(info=internal_exception_message) logger.exception(internal_exception_message)
-raise PaymentException(_("Error while creating SumUp checkout")) def
-checkout_confirm_render(self, request: HttpRequest, **kwargs): return _( "After
-confirmation you will be redirected to SumUp to complete the payment." ) def
-payment_form_render(self, request: HttpRequest, **kwargs): return
-self.checkout_confirm_render(request, **kwargs) def payment_pending_render
-(self, request: HttpRequest, payment: OrderPayment): checkout_id =
-payment.info_data.get("sumup_checkout_id") if checkout_id is None: return "" #
-Synchronize the payment status as backup if the return webhook fails
-self._synchronize_payment_status(payment) return get_template("pretix_sumup/
-pending.html").render( { "iframe_url": eventreverse( payment.order.event,
-"plugins:pretix_sumup:payment_widget", kwargs={ "payment": payment.pk, "order":
-payment.order.code, "secret": payment.order.secret, }, ) } ) def
-payment_is_valid_session(self, request: HttpRequest): return True def
-cancel_payment(self, payment: OrderPayment): checkout_id =
-payment.info_data.get("sumup_checkout_id") if checkout_id: try:
+("Automatically filled in"), } ), required=False, label=_("Merchant Code"), ),
+), ] + list(super().settings_form_fields.items()) ) d.move_to_end("_enabled",
+last=False) return d def settings_form_clean(self, cleaned_data: dict):
+cleaned_data = super().settings_form_clean(cleaned_data) access_token =
+cleaned_data.get("payment_sumup_access_token") if access_token is None: #
+access token was already validated and turned out to be invalid return
+cleaned_data merchant_code =
+sumup_client.validate_access_token_and_get_merchant_code( access_token )
+cleaned_data["payment_sumup_merchant_code"] = merchant_code return cleaned_data
+def is_allowed(self, request: HttpRequest, total: Decimal = None): if total is
+None: return True # minimum amount is 1 EUR or similar in other currencies
+return total >= 1 def execute_payment(self, request: HttpRequest, payment:
+OrderPayment): payment_id = payment.local_id order = payment.order event =
+order.event has_valid_checkout = self._synchronize_payment_status(payment) if
+has_valid_checkout: return try: checkout_id = sumup_client.create_checkout
+( checkout_reference=f"{event.slug}/{order.code}/{payment_id}",
+amount=payment.amount, currency=event.currency, description=f"{event.name} #
+{order.code}", merchant_code=self.settings.get("merchant_code"),
+return_url=build_absolute_uri( event, "plugins:pretix_sumup:checkout_event",
+kwargs={"payment": payment.pk}, ), access_token=self.settings.get
+("access_token"), ) info_data = payment.info_data info_data
+["sumup_checkout_id"] = checkout_id payment.info_data = info_data payment.save
+() except Exception as err: internal_exception_message = f"Error while creating
+SumUp checkout: {err}" payment.fail(info=internal_exception_message)
+logger.exception(internal_exception_message) raise PaymentException(_("Error
+while creating SumUp checkout")) def checkout_confirm_render(self, request:
+HttpRequest, **kwargs): return _( "After confirmation you will be redirected to
+SumUp to complete the payment." ) def payment_form_render(self, request:
+HttpRequest, **kwargs): return self.checkout_confirm_render(request, **kwargs)
+def payment_pending_render(self, request: HttpRequest, payment: OrderPayment):
+checkout_id = payment.info_data.get("sumup_checkout_id") if checkout_id is
+None: return "" # Synchronize the payment status as backup if the return
+webhook fails self._synchronize_payment_status(payment) return get_template
+("pretix_sumup/pending.html").render( { "iframe_url": eventreverse
+( payment.order.event, "plugins:pretix_sumup:payment_widget", kwargs=
+{ "payment": payment.pk, "order": payment.order.code, "secret":
+payment.order.secret, }, ) } ) def payment_is_valid_session(self, request:
+HttpRequest): return True def cancel_payment(self, payment: OrderPayment):
+checkout_id = payment.info_data.get("sumup_checkout_id") if checkout_id: try:
 sumup_client.cancel_checkout( checkout_id, self.settings.get("access_token") )
 except Exception as err: logger.warn(f"Error while canceling SumUp checkout:
 {err}") pass # Ignore errors, this hasn't any impact on us super
 ().cancel_payment(payment) def payment_refund_supported(self, payment:
 OrderPayment): self._synchronize_payment_status(payment) return
 payment.info_data.get("sumup_transaction") is not None def
 payment_partial_refund_supported(self, payment: OrderPayment):
```

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/sumup_client.py` & `pretix_sumup_payment-1.1.4/pretix_sumup/sumup_client.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/templates/pretix_sumup/payment_widget.html` & `pretix_sumup_payment-1.1.4/pretix_sumup/templates/pretix_sumup/payment_widget.html`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup/views.py` & `pretix_sumup_payment-1.1.4/pretix_sumup/views.py`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/PKG-INFO` & `pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sumup-payment
-Version: 1.1.2
+Version: 1.1.4
 Summary: Enables creditcard payments via Sumup
 Author-email: Christoph Walcher <chris@wiomoc.de>
 Maintainer-email: Christoph Walcher <chris@wiomoc.de>
 License: Apache
 Project-URL: homepage, https://github.com/wiomoc/pretix-sumup-payment
 Project-URL: repository, https://github.com/wiomoc/pretix-sumup-payment
 Keywords: pretix
```

### Comparing `pretix-sumup-payment-1.1.2/pretix_sumup_payment.egg-info/SOURCES.txt` & `pretix_sumup_payment-1.1.4/pretix_sumup_payment.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+.gitignore
+.install-hooks.sh
+.update-locales.sh
 LICENSE
 MANIFEST.in
+Makefile
 README.rst
+pretixplugin.toml
 pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/style.yml
+.github/workflows/tests.yml
 pretix_sumup/__init__.py
 pretix_sumup/apps.py
 pretix_sumup/payment.py
 pretix_sumup/signals.py
 pretix_sumup/sumup_client.py
 pretix_sumup/urls.py
 pretix_sumup/views.py
@@ -22,8 +29,9 @@
 pretix_sumup/templates/pretix_sumup/payment_widget.html
 pretix_sumup/templates/pretix_sumup/pending.html
 pretix_sumup_payment.egg-info/PKG-INFO
 pretix_sumup_payment.egg-info/SOURCES.txt
 pretix_sumup_payment.egg-info/dependency_links.txt
 pretix_sumup_payment.egg-info/entry_points.txt
 pretix_sumup_payment.egg-info/top_level.txt
+tests/conftest.py
 tests/test_main.py
```

### Comparing `pretix-sumup-payment-1.1.2/pyproject.toml` & `pretix_sumup_payment-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-sumup-payment-1.1.2/setup.cfg` & `pretix_sumup_payment-1.1.4/setup.cfg`

 * *Files identical despite different names*

