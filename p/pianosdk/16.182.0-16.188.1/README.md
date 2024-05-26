# Comparing `tmp/pianosdk-16.182.0.tar.gz` & `tmp/pianosdk-16.188.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pianosdk-16.182.0.tar", last modified: Sun May 19 20:12:19 2024, max compression
+gzip compressed data, was "pianosdk-16.188.1.tar", last modified: Sun May 26 20:12:57 2024, max compression
```

## Comparing `pianosdk-16.182.0.tar` & `pianosdk-16.188.1.tar`

### file list

```diff
@@ -1,579 +1,579 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.651210 pianosdk-16.182.0/
--rw-r--r--   0 root         (0) root         (0)     2220 2024-05-19 20:12:19.651210 pianosdk-16.182.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-19 20:12:04.000000 pianosdk-16.182.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.527210 pianosdk-16.182.0/pianosdk/
--rw-r--r--   0 root         (0) root         (0)     1216 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2514 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/access_token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.527210 pianosdk-16.182.0/pianosdk/anon/
--rw-r--r--   0 root         (0) root         (0)     3649 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.531210 pianosdk-16.182.0/pianosdk/anon/api/
--rw-r--r--   0 root         (0) root         (0)      981 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3932 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/access_api.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/access_token_api.py
--rw-r--r--   0 root         (0) root         (0)     4018 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/anon_assets_api.py
--rw-r--r--   0 root         (0) root         (0)     1637 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/anon_country_list_api.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/anon_error_api.py
--rw-r--r--   0 root         (0) root         (0)     1647 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/anon_mobile_sdk_id_deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/anon_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/anon_user_disable_api.py
--rw-r--r--   0 root         (0) root         (0)     9528 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/conversion_api.py
--rw-r--r--   0 root         (0) root         (0)     3304 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/conversion_external_api.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/conversion_registration_api.py
--rw-r--r--   0 root         (0) root         (0)     1877 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/email_confirmation_api.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/oauth_api.py
--rw-r--r--   0 root         (0) root         (0)     1953 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/subscription_api.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/api/swg_sync_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.539210 pianosdk-16.182.0/pianosdk/anon/models/
--rw-r--r--   0 root         (0) root         (0)     2666 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      566 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/access.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/access_dto.py
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/access_token_list.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/billing_plan_translation_request.py
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/check_subscription_response.py
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/client_configurations_dto.py
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/consent_model.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/country.py
--rw-r--r--   0 root         (0) root         (0)      238 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/currency.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/datatrans_apple_pay_config.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/external_css.py
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/key_source.py
--rw-r--r--   0 root         (0) root         (0)      834 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/light_offer_template_version.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/linked_term_checkout_track_params.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/linked_term_event_page_view_content.py
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/linked_term_event_session.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/linked_term_event_session_offer.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/linked_term_page_view_content_params.py
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/linked_term_session_params.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/locale_model.py
--rw-r--r--   0 root         (0) root         (0)      313 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/o_auth_token.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/passwordless_purchase_check_result.py
--rw-r--r--   0 root         (0) root         (0)      589 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/passwordless_purchase_complete_result.py
--rw-r--r--   0 root         (0) root         (0)      298 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/performance_metrics_dto.py
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/public_captcha_config.py
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/region.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/resource.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/resource_dto.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/source.py
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/swg_response.py
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/template_context.py
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/term.py
--rw-r--r--   0 root         (0) root         (0)      484 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/term_conversion.py
--rw-r--r--   0 root         (0) root         (0)      366 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/user.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/user_audit.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/user_dto.py
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/user_info.py
--rw-r--r--   0 root         (0) root         (0)      326 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/user_model.py
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/anon/models/user_subscription.py
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/api_response.py
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/base_api.py
--rw-r--r--   0 root         (0) root         (0)     3469 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/configuration.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/constants.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.539210 pianosdk-16.182.0/pianosdk/httpwrap/
--rw-r--r--   0 root         (0) root         (0)      802 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/httpwrap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3676 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/httpwrap/models.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/httpwrap/requests_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.539210 pianosdk-16.182.0/pianosdk/id/
--rw-r--r--   0 root         (0) root         (0)     2356 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.543210 pianosdk-16.182.0/pianosdk/id/api/
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1771 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/identity_oauth_api.py
--rw-r--r--   0 root         (0) root         (0)     1803 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/identity_token_api.py
--rw-r--r--   0 root         (0) root         (0)     4669 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_api.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_audit_api.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_form_api.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_identity_api.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_identity_set_api.py
--rw-r--r--   0 root         (0) root         (0)     2098 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_import_custom_fields_api.py
--rw-r--r--   0 root         (0) root         (0)     2202 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_login_api.py
--rw-r--r--   0 root         (0) root         (0)     4760 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_login_social_api.py
--rw-r--r--   0 root         (0) root         (0)     1933 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_reset_api.py
--rw-r--r--   0 root         (0) root         (0)     3128 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_token_api.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/api/publisher_users_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.547210 pianosdk-16.182.0/pianosdk/id/models/
--rw-r--r--   0 root         (0) root         (0)     1453 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/consent_model.py
--rw-r--r--   0 root         (0) root         (0)      698 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/custom_field_attribute_dto.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/custom_field_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/custom_field_value_dto.py
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/import_cf_result.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/input_stream.py
--rw-r--r--   0 root         (0) root         (0)      198 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/logout_response.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/o_auth_request.py
--rw-r--r--   0 root         (0) root         (0)      259 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/publisher_custom_field_response.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/publisher_login_request.py
--rw-r--r--   0 root         (0) root         (0)      366 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/publisher_password_request.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/publisher_register_request.py
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/publisher_set_password_request.py
--rw-r--r--   0 root         (0) root         (0)      646 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/publisher_user_profile_response.py
--rw-r--r--   0 root         (0) root         (0)      555 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/social_additional_input_request.py
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/social_link_response.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/social_linking_response.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/token_response.py
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/tooltip.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/id/models/validator.py
--rw-r--r--   0 root         (0) root         (0)    30919 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/piano_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.547210 pianosdk-16.182.0/pianosdk/publisher/
--rw-r--r--   0 root         (0) root         (0)    31488 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.571210 pianosdk-16.182.0/pianosdk/publisher/api/
--rw-r--r--   0 root         (0) root         (0)     8316 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_adblocker_api.py
--rw-r--r--   0 root         (0) root         (0)     3810 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_app_api.py
--rw-r--r--   0 root         (0) root         (0)     1719 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_app_api_token_api.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_app_features_api.py
--rw-r--r--   0 root         (0) root         (0)     3127 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_consent_api.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_consent_entry_api.py
--rw-r--r--   0 root         (0) root         (0)     8820 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_api.py
--rw-r--r--   0 root         (0) root         (0)     3346 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_custom_api.py
--rw-r--r--   0 root         (0) root         (0)     1839 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_data_api.py
--rw-r--r--   0 root         (0) root         (0)     3317 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_external_api.py
--rw-r--r--   0 root         (0) root         (0)     2442 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_registration_api.py
--rw-r--r--   0 root         (0) root         (0)     6725 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_api.py
--rw-r--r--   0 root         (0) root         (0)     3462 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_aam_api.py
--rw-r--r--   0 root         (0) root         (0)     2021 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_aam_monthly_api.py
--rw-r--r--   0 root         (0) root         (0)     2620 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_access_report_export_api.py
--rw-r--r--   0 root         (0) root         (0)    24939 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_api.py
--rw-r--r--   0 root         (0) root         (0)     4878 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_subscription_details_report_api.py
--rw-r--r--   0 root         (0) root         (0)     2328 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_transactions_report_api.py
--rw-r--r--   0 root         (0) root         (0)     4238 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_gdpr_api.py
--rw-r--r--   0 root         (0) root         (0)     9524 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_inquiry_api.py
--rw-r--r--   0 root         (0) root         (0)    11666 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_api.py
--rw-r--r--   0 root         (0) root         (0)     7860 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_domain_api.py
--rw-r--r--   0 root         (0) root         (0)     2404 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_domain_contract_user_api.py
--rw-r--r--   0 root         (0) root         (0)     6069 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_ip_range_api.py
--rw-r--r--   0 root         (0) root         (0)     1851 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_periods_api.py
--rw-r--r--   0 root         (0) root         (0)    12160 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_user_api.py
--rw-r--r--   0 root         (0) root         (0)     8563 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_licensee_api.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_notification_api.py
--rw-r--r--   0 root         (0) root         (0)     6739 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_notification_rule_api.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_schedule_api.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_schedule_contract_periods_api.py
--rw-r--r--   0 root         (0) root         (0)     4444 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_linked_term_api.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_linked_term_custom_field_api.py
--rw-r--r--   0 root         (0) root         (0)     7786 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_api.py
--rw-r--r--   0 root         (0) root         (0)    24925 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_api.py
--rw-r--r--   0 root         (0) root         (0)     2087 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_create_api.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_inherited_api.py
--rw-r--r--   0 root         (0) root         (0)     2238 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_update_api.py
--rw-r--r--   0 root         (0) root         (0)    10415 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_variant_api.py
--rw-r--r--   0 root         (0) root         (0)     5272 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_term_api.py
--rw-r--r--   0 root         (0) root         (0)     1976 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_term_offer_api.py
--rw-r--r--   0 root         (0) root         (0)     4462 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_api.py
--rw-r--r--   0 root         (0) root         (0)     7208 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_method_api.py
--rw-r--r--   0 root         (0) root         (0)     5797 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_method_billing_address_api.py
--rw-r--r--   0 root         (0) root         (0)     1900 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_method_gmo_api.py
--rw-r--r--   0 root         (0) root         (0)     1842 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_provider_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)    15124 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_api.py
--rw-r--r--   0 root         (0) root         (0)    10127 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_code_api.py
--rw-r--r--   0 root         (0) root         (0)     4581 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_fixed_discount_api.py
--rw-r--r--   0 root         (0) root         (0)     4630 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_term_api.py
--rw-r--r--   0 root         (0) root         (0)    14710 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_api.py
--rw-r--r--   0 root         (0) root         (0)     2075 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_bundle_api.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_cross_app_api.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_stats_api.py
--rw-r--r--   0 root         (0) root         (0)    10275 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_tag_api.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_user_api.py
--rw-r--r--   0 root         (0) root         (0)     8205 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_schedule_api.py
--rw-r--r--   0 root         (0) root         (0)     4703 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_schedule_period_api.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_address_api.py
--rw-r--r--   0 root         (0) root         (0)    16211 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_api.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_cancel_api.py
--rw-r--r--   0 root         (0) root         (0)    11228 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_share_api.py
--rw-r--r--   0 root         (0) root         (0)     3048 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_share_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1789 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_team_api.py
--rw-r--r--   0 root         (0) root         (0)     7788 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_api.py
--rw-r--r--   0 root         (0) root         (0)     6173 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_change_api.py
--rw-r--r--   0 root         (0) root         (0)     2424 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_change_option_api.py
--rw-r--r--   0 root         (0) root         (0)     3710 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_custom_api.py
--rw-r--r--   0 root         (0) root         (0)     4914 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_dynamic_api.py
--rw-r--r--   0 root         (0) root         (0)     5294 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_external_api.py
--rw-r--r--   0 root         (0) root         (0)     6081 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_gift_api.py
--rw-r--r--   0 root         (0) root         (0)     8456 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_payment_api.py
--rw-r--r--   0 root         (0) root         (0)     3761 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_registration_api.py
--rw-r--r--   0 root         (0) root         (0)     1786 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_stats_api.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_test_api.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_access_active_api.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_access_api.py
--rw-r--r--   0 root         (0) root         (0)     8919 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_address_api.py
--rw-r--r--   0 root         (0) root         (0)    19088 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1720 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_app_api.py
--rw-r--r--   0 root         (0) root         (0)     8674 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_billing_address_api.py
--rw-r--r--   0 root         (0) root         (0)     5786 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_bulk_import_api.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_email_api.py
--rw-r--r--   0 root         (0) root         (0)     2090 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_list_api.py
--rw-r--r--   0 root         (0) root         (0)     5937 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_note_api.py
--rw-r--r--   0 root         (0) root         (0)     4528 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_voucher_api.py
--rw-r--r--   0 root         (0) root         (0)     8220 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_webhook_api.py
--rw-r--r--   0 root         (0) root         (0)     3231 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_webhook_response_api.py
--rw-r--r--   0 root         (0) root         (0)     1853 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/api/publisher_webhook_settings_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.647210 pianosdk-16.182.0/pianosdk/publisher/models/
--rw-r--r--   0 root         (0) root         (0)    23206 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/publisher/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access.py
--rw-r--r--   0 root         (0) root         (0)      640 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access_dto.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access_granted_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access_modified_event.py
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access_period.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access_period_stats.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/access_revoked_event.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/action.py
--rw-r--r--   0 root         (0) root         (0)      670 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/action_dto.py
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/action_step_dto.py
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/address_config.py
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/address_updated_event.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/advanced_email_model.py
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/advanced_options.py
--rw-r--r--   0 root         (0) root         (0)      589 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/app.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/app_features.py
--rw-r--r--   0 root         (0) root         (0)      243 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/app_resource_count.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/apply_payment_method_dto.py
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/audit_changed_field_dto.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/avalara_configuration.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/avalara_origin_address.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/bill.py
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/billing_plan_table.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/billing_timing_option.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/brain_tree_create_credit_card_info_dto.py
--rw-r--r--   0 root         (0) root         (0)     1404 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/braintree_configuration.py
--rw-r--r--   0 root         (0) root         (0)      283 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/braintree_merchant_account_id_entry.py
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/browser_segment.py
--rw-r--r--   0 root         (0) root         (0)      328 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/bulk_user_import.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/bulk_user_import_processing_request_dto.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/c2_experience_config.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/categories_counter_model.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/change_subscription_term_step.py
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/check_users_email_result.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/checkout_flow.py
--rw-r--r--   0 root         (0) root         (0)      596 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/checkout_flow_light_model.py
--rw-r--r--   0 root         (0) root         (0)      487 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/churn_prevention_email.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/churn_prevention_logic.py
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/churn_prevention_template_version.py
--rw-r--r--   0 root         (0) root         (0)      229 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/comment_action.py
--rw-r--r--   0 root         (0) root         (0)      191 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/composer.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/configuration_property_metadata.py
--rw-r--r--   0 root         (0) root         (0)      527 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/consent.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/consent_box_entry.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_created_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_deleted_event.py
--rw-r--r--   0 root         (0) root         (0)      661 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_details.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_domain.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_ip_range.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_redeemed_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_renewed_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_updated_event.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_user.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_user_access_expired_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_user_access_revoked_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_user_created_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/contract_user_invited_event.py
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/conversion_value_dto.py
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/country.py
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/country_model.py
--rw-r--r--   0 root         (0) root         (0)      248 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/country_simple_model.py
--rw-r--r--   0 root         (0) root         (0)      697 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/create_access_period_params.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/create_billing_configuration_request.py
--rw-r--r--   0 root         (0) root         (0)      551 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/create_linked_term_request.py
--rw-r--r--   0 root         (0) root         (0)      963 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/credit_guard_stored_fields.py
--rw-r--r--   0 root         (0) root         (0)      238 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/currency.py
--rw-r--r--   0 root         (0) root         (0)      343 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/datatrans_properties.py
--rw-r--r--   0 root         (0) root         (0)      483 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/delivery_zone.py
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/deployment_app.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/deployment_app_details.py
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/deployment_content_fields.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/deployment_details.py
--rw-r--r--   0 root         (0) root         (0)      576 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/deployment_list_item.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/deployment_variant_param_dto.py
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/dns_forwarding_config.py
--rw-r--r--   0 root         (0) root         (0)      219 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/duration.py
--rw-r--r--   0 root         (0) root         (0)      657 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/dynamic_subscription_access_period_info.py
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/dynamic_subscription_details.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/dynamic_term_access_period.py
--rw-r--r--   0 root         (0) root         (0)      560 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/easypay_configuration.py
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/edgil_payway_hosted_page_setup.py
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/eigen_create_credit_card_info_dto.py
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/email.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_contract_user.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_conversion.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_subscription.py
--rw-r--r--   0 root         (0) root         (0)      249 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_transaction.py
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_user.py
--rw-r--r--   0 root         (0) root         (0)      516 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_user_payment.py
--rw-r--r--   0 root         (0) root         (0)      650 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_user_payment_info.py
--rw-r--r--   0 root         (0) root         (0)     1277 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_user_response.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/erase_user_subscription_account.py
--rw-r--r--   0 root         (0) root         (0)      223 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/error_code.py
--rw-r--r--   0 root         (0) root         (0)      330 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/error_codes.py
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/experian_configuration.py
--rw-r--r--   0 root         (0) root         (0)      861 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/experience.py
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/experience_stat.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/experience_version.py
--rw-r--r--   0 root         (0) root         (0)      612 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/export.py
--rw-r--r--   0 root         (0) root         (0)      623 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/ext_provider_dto.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/external_api_configuration.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/external_api_field.py
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/external_api_property_schema.py
--rw-r--r--   0 root         (0) root         (0)      257 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/external_api_provider_property.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/external_css.py
--rw-r--r--   0 root         (0) root         (0)     1493 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_deployment.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_deployment_item.py
--rw-r--r--   0 root         (0) root         (0)      461 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)      524 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_filter.py
--rw-r--r--   0 root         (0) root         (0)      501 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_filter_item.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_filter_sub_item.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_recent_deployments.py
--rw-r--r--   0 root         (0) root         (0)      825 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/global_template_version.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/grace_period_details.py
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/import_data.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/import_data_state.py
--rw-r--r--   0 root         (0) root         (0)      671 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/import_item.py
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/import_profile.py
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/import_section.py
--rw-r--r--   0 root         (0) root         (0)      265 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/import_user.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/input_stream.py
--rw-r--r--   0 root         (0) root         (0)      538 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/inquiry_comment.py
--rw-r--r--   0 root         (0) root         (0)      357 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/instrument_dto.py
--rw-r--r--   0 root         (0) root         (0)      313 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/key_source.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/keying_event.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/klarna_configuration.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/language_model.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/language_stats.py
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee_created_event.py
--rw-r--r--   0 root         (0) root         (0)      313 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee_manager.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee_notification.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee_notification_rule.py
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee_representative.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/licensee_updated_event.py
--rw-r--r--   0 root         (0) root         (0)      307 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/light_experience.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/light_global_template.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/lightweight_churn_prevention_logic.py
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/lightweight_experience.py
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/link.py
--rw-r--r--   0 root         (0) root         (0)      288 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/link_all_status_response.py
--rw-r--r--   0 root         (0) root         (0)      571 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/link_candidate.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_checkout_track_params.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_churn_params.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_configuration_request.py
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_conversion_params.py
--rw-r--r--   0 root         (0) root         (0)      212 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_custom_data.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_custom_field_configuration_request.py
--rw-r--r--   0 root         (0) root         (0)      288 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_custom_field_params.py
--rw-r--r--   0 root         (0) root         (0)      743 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_event_request.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_payment_params.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_purchase_params.py
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_shared_access_params.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_subscription_params.py
--rw-r--r--   0 root         (0) root         (0)      233 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/linked_term_upgrade_params.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/locale_model.py
--rw-r--r--   0 root         (0) root         (0)      225 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/mail.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/mail_log.py
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/mail_options_verification_result.py
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/mandate.py
--rw-r--r--   0 root         (0) root         (0)      283 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/money.py
--rw-r--r--   0 root         (0) root         (0)      193 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/my_account.py
--rw-r--r--   0 root         (0) root         (0)      368 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/newscycle_configuration.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/newscycle_configuration_test_result.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/notification.py
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/obi_configuration.py
--rw-r--r--   0 root         (0) root         (0)      649 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_model.py
--rw-r--r--   0 root         (0) root         (0)     1651 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_categories.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_content_field.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_histories.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_history.py
--rw-r--r--   0 root         (0) root         (0)      996 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_revision.py
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_sub_history.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_variant.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/offer_template_version.py
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/one_source_configuration.py
--rw-r--r--   0 root         (0) root         (0)      560 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/openpay_configuration.py
--rw-r--r--   0 root         (0) root         (0)      335 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/pay_source_dto.py
--rw-r--r--   0 root         (0) root         (0)      260 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/payee_settings_entry.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/payment_inquiry.py
--rw-r--r--   0 root         (0) root         (0)      530 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/payment_method.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/payment_method_dto.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/payment_provider_configuration.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/payment_refund_event.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/paypal_express_checkout_configuration.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/period.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/period_link.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/period_link_candidate.py
--rw-r--r--   0 root         (0) root         (0)      551 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/period_settings.py
--rw-r--r--   0 root         (0) root         (0)      330 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/permission_dto.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/pp_configuration.py
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/ppc_web_model.py
--rw-r--r--   0 root         (0) root         (0)      307 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/price_dto.py
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/promo_code.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/promotion.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/promotion_applicable_term_container.py
--rw-r--r--   0 root         (0) root         (0)      298 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/promotion_fixed_discountt.py
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/promotion_stats.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/promotion_term_stats.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/reallocation_batch.py
--rw-r--r--   0 root         (0) root         (0)      203 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/redemption_page.py
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/region.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/region_simple_model.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/rendered_email.py
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/report_response.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/resource.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/resource_compact_stats.py
--rw-r--r--   0 root         (0) root         (0)      838 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/resource_dto.py
--rw-r--r--   0 root         (0) root         (0)      341 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/resource_stats.py
--rw-r--r--   0 root         (0) root         (0)      266 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/resource_tag.py
--rw-r--r--   0 root         (0) root         (0)      561 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/result.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/sales_tax_rate_model.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/schedule.py
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/schedule_period.py
--rw-r--r--   0 root         (0) root         (0)      296 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/sections_counters.py
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/send_email_step.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/shared_account_param.py
--rw-r--r--   0 root         (0) root         (0)      585 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/shared_subscription.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/shared_subscription_child_access_granted_event.py
--rw-r--r--   0 root         (0) root         (0)      289 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/source.py
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/source_eligible_term.py
--rw-r--r--   0 root         (0) root         (0)      468 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/source_ineligible_term.py
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/source_term_change_variant.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/source_term_change_variants.py
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/split_test_object.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/spreedly_configuration.py
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/stripe_properties.py
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/stripe_setup_intent_model_definition.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_auto_renew_changed_by_end_user_event.py
--rw-r--r--   0 root         (0) root         (0)      609 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_log_item.py
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_migration_history_dto.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_reallocation_error.py
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_reallocation_validation_result.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_renewal_event.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_restrictions.py
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_term_change_options.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/subscription_upgrade_status.py
--rw-r--r--   0 root         (0) root         (0)      817 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/target_eligible_term.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/target_ineligible_term.py
--rw-r--r--   0 root         (0) root         (0)      676 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/target_term_change_variant.py
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/target_term_change_variants.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/target_upgrade_option.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/tax_country.py
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/tax_support_dto.py
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/team_member.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/template_config.py
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/template_counter_model.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/template_user_model.py
--rw-r--r--   0 root         (0) root         (0)      361 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/template_variable.py
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/template_version.py
--rw-r--r--   0 root         (0) root         (0)     3848 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term.py
--rw-r--r--   0 root         (0) root         (0)      259 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_brief.py
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_change_billing_options.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_change_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_change_finished_event.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_change_option.py
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_change_params.py
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_change_variants.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_changed_event.py
--rw-r--r--   0 root         (0) root         (0)     1338 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_conversion.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_conversion_data.py
--rw-r--r--   0 root         (0) root         (0)     1239 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_conversion_dto.py
--rw-r--r--   0 root         (0) root         (0)     1506 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_conversion_subscription.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_from.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_link.py
--rw-r--r--   0 root         (0) root         (0)      780 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_period_reallocation.py
--rw-r--r--   0 root         (0) root         (0)      545 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_reallocation.py
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_short.py
--rw-r--r--   0 root         (0) root         (0)      341 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_stats.py
--rw-r--r--   0 root         (0) root         (0)     1238 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_to_eligible.py
--rw-r--r--   0 root         (0) root         (0)      487 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_to_ineligible.py
--rw-r--r--   0 root         (0) root         (0)     1355 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_to_upgrade_option.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/term_type_dto.py
--rw-r--r--   0 root         (0) root         (0)     1494 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/tern_change_confirmation_dto.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/test_event.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/transaction_item.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/translation_map_revision.py
--rw-r--r--   0 root         (0) root         (0)      402 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/translation_stats.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/unknown_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/unsupported_event.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/update_access_period_params.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/update_billing_configuration_request.py
--rw-r--r--   0 root         (0) root         (0)      589 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/update_linked_term_request.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/upgrade_checkout_flow.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/upgrade_offer.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/upgrade_offer_variant.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/upgrade_sources.py
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/upgrade_subscription_step.py
--rw-r--r--   0 root         (0) root         (0)      645 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/upgrade_targets.py
--rw-r--r--   0 root         (0) root         (0)      666 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user.py
--rw-r--r--   0 root         (0) root         (0)      684 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_access_dto.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_address.py
--rw-r--r--   0 root         (0) root         (0)      528 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_address_dto.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_address_history.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_address_updated_event.py
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_alias_dto.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_audit.py
--rw-r--r--   0 root         (0) root         (0)      764 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_billing_address.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_conversion_dto.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_created_event.py
--rw-r--r--   0 root         (0) root         (0)      751 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_details.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_disabled_event.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_dto.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_email_confirmed_event.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_info.py
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_note.py
--rw-r--r--   0 root         (0) root         (0)     2393 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_payment.py
--rw-r--r--   0 root         (0) root         (0)     2367 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_payment_details_dto.py
--rw-r--r--   0 root         (0) root         (0)     1051 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_payment_dto.py
--rw-r--r--   0 root         (0) root         (0)      668 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_payment_info.py
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_payment_method_event.py
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_payment_refund_dto.py
--rw-r--r--   0 root         (0) root         (0)     3742 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_provider_configuration.py
--rw-r--r--   0 root         (0) root         (0)      332 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_ref.py
--rw-r--r--   0 root         (0) root         (0)     2380 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_subscription.py
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_subscription_account.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_subscription_dto.py
--rw-r--r--   0 root         (0) root         (0)     2029 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_subscription_list_item.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/user_updated_event.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/users_import_result.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/variant_item.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/version_item.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/voucher.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/voucher_delivered_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/voucher_purchased_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/voucher_redeemed_event.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/voucher_revoked_event.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/vouchering_policy.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/webhook_config.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/webhook_event.py
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/webhook_response.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/webhook_settings.py
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/webhook_status.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/worldpay_configuration.py
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/worldpay_payment_method.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/zuora_configuration.py
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-19 20:12:06.000000 pianosdk-16.182.0/pianosdk/publisher/models/zuora_connect_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.647210 pianosdk-16.182.0/pianosdk/user/
--rw-r--r--   0 root         (0) root         (0)      686 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.647210 pianosdk-16.182.0/pianosdk/user/api/
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4244 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/api/user_access_api.py
--rw-r--r--   0 root         (0) root         (0)     1583 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/api/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.651210 pianosdk-16.182.0/pianosdk/user/models/
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      566 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/access.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/access_dto.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/country.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/geo_location.py
--rw-r--r--   0 root         (0) root         (0)      498 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/payment_method.py
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/region.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/resource.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/resource_dto.py
--rw-r--r--   0 root         (0) root         (0)      356 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/user.py
--rw-r--r--   0 root         (0) root         (0)      701 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/user_address.py
--rw-r--r--   0 root         (0) root         (0)      362 2024-05-19 20:12:05.000000 pianosdk-16.182.0/pianosdk/user/models/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     4728 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/utils.py
--rw-r--r--   0 root         (0) root         (0)    11563 2024-05-19 20:12:08.000000 pianosdk-16.182.0/pianosdk/webhook_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 20:12:19.651210 pianosdk-16.182.0/pianosdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2220 2024-05-19 20:12:19.000000 pianosdk-16.182.0/pianosdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26838 2024-05-19 20:12:19.000000 pianosdk-16.182.0/pianosdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 20:12:19.000000 pianosdk-16.182.0/pianosdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-19 20:12:19.000000 pianosdk-16.182.0/pianosdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-19 20:12:19.000000 pianosdk-16.182.0/pianosdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-05-19 20:12:19.651210 pianosdk-16.182.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1054 2024-05-19 20:12:08.000000 pianosdk-16.182.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.336666 pianosdk-16.188.1/
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-05-26 20:12:57.336666 pianosdk-16.188.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-26 20:12:41.000000 pianosdk-16.188.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.212668 pianosdk-16.188.1/pianosdk/
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/access_token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.212668 pianosdk-16.188.1/pianosdk/anon/
+-rw-r--r--   0 root         (0) root         (0)     3649 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.216668 pianosdk-16.188.1/pianosdk/anon/api/
+-rw-r--r--   0 root         (0) root         (0)      981 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/access_api.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/access_token_api.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/anon_assets_api.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/anon_country_list_api.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/anon_error_api.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/anon_mobile_sdk_id_deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/anon_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/anon_user_disable_api.py
+-rw-r--r--   0 root         (0) root         (0)     9528 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/conversion_api.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/conversion_external_api.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/conversion_registration_api.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/email_confirmation_api.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/oauth_api.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/subscription_api.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/api/swg_sync_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.228668 pianosdk-16.188.1/pianosdk/anon/models/
+-rw-r--r--   0 root         (0) root         (0)     2666 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      566 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/access.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/access_dto.py
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/access_token_list.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/billing_plan_translation_request.py
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/check_subscription_response.py
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/client_configurations_dto.py
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/consent_model.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/country.py
+-rw-r--r--   0 root         (0) root         (0)      238 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/datatrans_apple_pay_config.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/external_css.py
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/key_source.py
+-rw-r--r--   0 root         (0) root         (0)      834 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/light_offer_template_version.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/linked_term_checkout_track_params.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/linked_term_event_page_view_content.py
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/linked_term_event_session.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/linked_term_event_session_offer.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/linked_term_page_view_content_params.py
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/linked_term_session_params.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/locale_model.py
+-rw-r--r--   0 root         (0) root         (0)      313 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/o_auth_token.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/passwordless_purchase_check_result.py
+-rw-r--r--   0 root         (0) root         (0)      589 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/passwordless_purchase_complete_result.py
+-rw-r--r--   0 root         (0) root         (0)      298 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/performance_metrics_dto.py
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/public_captcha_config.py
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/region.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/resource.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/resource_dto.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/source.py
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/swg_response.py
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/template_context.py
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/term.py
+-rw-r--r--   0 root         (0) root         (0)      484 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/term_conversion.py
+-rw-r--r--   0 root         (0) root         (0)      366 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/user.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/user_audit.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/user_info.py
+-rw-r--r--   0 root         (0) root         (0)      326 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/user_model.py
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/anon/models/user_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/api_response.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/base_api.py
+-rw-r--r--   0 root         (0) root         (0)     3469 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/constants.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.228668 pianosdk-16.188.1/pianosdk/httpwrap/
+-rw-r--r--   0 root         (0) root         (0)      802 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/httpwrap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3676 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/httpwrap/models.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/httpwrap/requests_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.228668 pianosdk-16.188.1/pianosdk/id/
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.232668 pianosdk-16.188.1/pianosdk/id/api/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/identity_oauth_api.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/identity_token_api.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_api.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_audit_api.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_form_api.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_identity_api.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_identity_set_api.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_import_custom_fields_api.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_login_api.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_login_social_api.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_reset_api.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_token_api.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/api/publisher_users_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.236668 pianosdk-16.188.1/pianosdk/id/models/
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/consent_model.py
+-rw-r--r--   0 root         (0) root         (0)      698 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/custom_field_attribute_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/custom_field_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/custom_field_value_dto.py
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/import_cf_result.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/input_stream.py
+-rw-r--r--   0 root         (0) root         (0)      198 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/logout_response.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/o_auth_request.py
+-rw-r--r--   0 root         (0) root         (0)      259 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/publisher_custom_field_response.py
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/publisher_login_request.py
+-rw-r--r--   0 root         (0) root         (0)      366 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/publisher_password_request.py
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/publisher_register_request.py
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/publisher_set_password_request.py
+-rw-r--r--   0 root         (0) root         (0)      646 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/publisher_user_profile_response.py
+-rw-r--r--   0 root         (0) root         (0)      555 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/social_additional_input_request.py
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/social_link_response.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/social_linking_response.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/token_response.py
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/tooltip.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/id/models/validator.py
+-rw-r--r--   0 root         (0) root         (0)    30919 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/piano_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.236668 pianosdk-16.188.1/pianosdk/publisher/
+-rw-r--r--   0 root         (0) root         (0)    31486 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.256667 pianosdk-16.188.1/pianosdk/publisher/api/
+-rw-r--r--   0 root         (0) root         (0)     8316 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_adblocker_api.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_app_api.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_app_api_token_api.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_app_features_api.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_consent_api.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_consent_entry_api.py
+-rw-r--r--   0 root         (0) root         (0)     8820 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_api.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_custom_api.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_data_api.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_external_api.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_registration_api.py
+-rw-r--r--   0 root         (0) root         (0)     6725 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_api.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_aam_api.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_aam_monthly_api.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_access_report_export_api.py
+-rw-r--r--   0 root         (0) root         (0)    24939 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_api.py
+-rw-r--r--   0 root         (0) root         (0)     4878 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_subscription_details_report_api.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_transactions_report_api.py
+-rw-r--r--   0 root         (0) root         (0)     4238 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_gdpr_api.py
+-rw-r--r--   0 root         (0) root         (0)     9524 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_inquiry_api.py
+-rw-r--r--   0 root         (0) root         (0)    11666 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_api.py
+-rw-r--r--   0 root         (0) root         (0)     7860 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_domain_api.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_domain_contract_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     6069 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_ip_range_api.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_periods_api.py
+-rw-r--r--   0 root         (0) root         (0)    12160 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     8563 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_licensee_api.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_notification_api.py
+-rw-r--r--   0 root         (0) root         (0)     6739 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_notification_rule_api.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_schedule_api.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_schedule_contract_periods_api.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_linked_term_api.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_linked_term_custom_field_api.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_api.py
+-rw-r--r--   0 root         (0) root         (0)    24925 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_api.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_create_api.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_inherited_api.py
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_update_api.py
+-rw-r--r--   0 root         (0) root         (0)    10415 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_variant_api.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_term_api.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_term_offer_api.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_api.py
+-rw-r--r--   0 root         (0) root         (0)     7208 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_method_api.py
+-rw-r--r--   0 root         (0) root         (0)     5797 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_method_billing_address_api.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_method_gmo_api.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_provider_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)    15124 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_api.py
+-rw-r--r--   0 root         (0) root         (0)    10127 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_code_api.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_fixed_discount_api.py
+-rw-r--r--   0 root         (0) root         (0)     4630 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_term_api.py
+-rw-r--r--   0 root         (0) root         (0)    14710 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_bundle_api.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_cross_app_api.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_stats_api.py
+-rw-r--r--   0 root         (0) root         (0)    10275 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_tag_api.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_schedule_api.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_schedule_period_api.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_address_api.py
+-rw-r--r--   0 root         (0) root         (0)    16211 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_api.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_cancel_api.py
+-rw-r--r--   0 root         (0) root         (0)    11228 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_share_api.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_share_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_team_api.py
+-rw-r--r--   0 root         (0) root         (0)     7788 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_api.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_change_api.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_change_option_api.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_custom_api.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_dynamic_api.py
+-rw-r--r--   0 root         (0) root         (0)     5294 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_external_api.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_gift_api.py
+-rw-r--r--   0 root         (0) root         (0)     8456 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_payment_api.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_registration_api.py
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_stats_api.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_access_active_api.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_access_api.py
+-rw-r--r--   0 root         (0) root         (0)     8919 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_address_api.py
+-rw-r--r--   0 root         (0) root         (0)    19088 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_app_api.py
+-rw-r--r--   0 root         (0) root         (0)     8674 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_billing_address_api.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_bulk_import_api.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_email_api.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_list_api.py
+-rw-r--r--   0 root         (0) root         (0)     5937 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_note_api.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_voucher_api.py
+-rw-r--r--   0 root         (0) root         (0)     8220 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_webhook_api.py
+-rw-r--r--   0 root         (0) root         (0)     3231 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_webhook_response_api.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/api/publisher_webhook_settings_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.332666 pianosdk-16.188.1/pianosdk/publisher/models/
+-rw-r--r--   0 root         (0) root         (0)    23204 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/publisher/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access.py
+-rw-r--r--   0 root         (0) root         (0)      640 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access_dto.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access_granted_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access_modified_event.py
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access_period.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access_period_stats.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/access_revoked_event.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/action.py
+-rw-r--r--   0 root         (0) root         (0)      670 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/action_dto.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/action_step_dto.py
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/address_config.py
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/address_updated_event.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/advanced_email_model.py
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/advanced_options.py
+-rw-r--r--   0 root         (0) root         (0)      589 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/app.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/app_features.py
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/app_resource_count.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/apply_payment_method_dto.py
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/audit_changed_field_dto.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/avalara_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/avalara_origin_address.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/bill.py
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/billing_plan_table.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/billing_timing_option.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/brain_tree_create_credit_card_info_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/braintree_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      283 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/braintree_merchant_account_id_entry.py
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/browser_segment.py
+-rw-r--r--   0 root         (0) root         (0)      328 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/bulk_user_import.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/bulk_user_import_processing_request_dto.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/c2_experience_config.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/categories_counter_model.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/change_subscription_term_step.py
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/check_users_email_result.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/checkout_flow.py
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/checkout_flow_light_model.py
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/churn_prevention_email.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/churn_prevention_logic.py
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/churn_prevention_template_version.py
+-rw-r--r--   0 root         (0) root         (0)      229 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/comment_action.py
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/composer.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/configuration_property_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      527 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/consent.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/consent_box_entry.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_created_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_deleted_event.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_details.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_domain.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_ip_range.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_redeemed_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_renewed_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_updated_event.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_user.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_user_access_expired_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_user_access_revoked_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_user_created_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/contract_user_invited_event.py
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/conversion_value_dto.py
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/country.py
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/country_model.py
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/country_simple_model.py
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/create_access_period_params.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/create_billing_configuration_request.py
+-rw-r--r--   0 root         (0) root         (0)      551 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/create_linked_term_request.py
+-rw-r--r--   0 root         (0) root         (0)      963 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/credit_guard_stored_fields.py
+-rw-r--r--   0 root         (0) root         (0)      238 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)      343 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/datatrans_properties.py
+-rw-r--r--   0 root         (0) root         (0)      483 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/delivery_zone.py
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/deployment_app.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/deployment_app_details.py
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/deployment_content_fields.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/deployment_details.py
+-rw-r--r--   0 root         (0) root         (0)      576 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/deployment_list_item.py
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/deployment_variant_param_dto.py
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/dns_forwarding_config.py
+-rw-r--r--   0 root         (0) root         (0)      219 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/duration.py
+-rw-r--r--   0 root         (0) root         (0)      657 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/dynamic_subscription_access_period_info.py
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/dynamic_subscription_details.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/dynamic_term_access_period.py
+-rw-r--r--   0 root         (0) root         (0)      560 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/easypay_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/edgil_payway_hosted_page_setup.py
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/eigen_create_credit_card_info_dto.py
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/email.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_contract_user.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_conversion.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_transaction.py
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_user.py
+-rw-r--r--   0 root         (0) root         (0)      516 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_user_payment.py
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_user_payment_info.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_user_response.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/erase_user_subscription_account.py
+-rw-r--r--   0 root         (0) root         (0)      223 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/error_code.py
+-rw-r--r--   0 root         (0) root         (0)      330 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/error_codes.py
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/experian_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      861 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/experience.py
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/experience_stat.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/experience_version.py
+-rw-r--r--   0 root         (0) root         (0)      612 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/export.py
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/ext_provider_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/external_api_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/external_api_field.py
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/external_api_property_schema.py
+-rw-r--r--   0 root         (0) root         (0)      257 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/external_api_provider_property.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/external_css.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_deployment.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_deployment_item.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_filter.py
+-rw-r--r--   0 root         (0) root         (0)      501 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_filter_item.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_filter_sub_item.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_recent_deployments.py
+-rw-r--r--   0 root         (0) root         (0)      825 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/global_template_version.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/grace_period_details.py
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/import_data.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/import_data_state.py
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/import_item.py
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/import_profile.py
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/import_section.py
+-rw-r--r--   0 root         (0) root         (0)      265 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/import_user.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/input_stream.py
+-rw-r--r--   0 root         (0) root         (0)      538 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/inquiry_comment.py
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/instrument_dto.py
+-rw-r--r--   0 root         (0) root         (0)      313 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/key_source.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/keying_event.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/klarna_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/language_model.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/language_stats.py
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee_created_event.py
+-rw-r--r--   0 root         (0) root         (0)      313 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee_manager.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee_notification.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee_notification_rule.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee_representative.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/licensee_updated_event.py
+-rw-r--r--   0 root         (0) root         (0)      307 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/light_experience.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/light_global_template.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/lightweight_churn_prevention_logic.py
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/lightweight_experience.py
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/link.py
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/link_all_status_response.py
+-rw-r--r--   0 root         (0) root         (0)      571 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/link_candidate.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_checkout_track_params.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_churn_params.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_configuration_request.py
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_conversion_params.py
+-rw-r--r--   0 root         (0) root         (0)      212 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_custom_data.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_custom_field_configuration_request.py
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_custom_field_params.py
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_event_request.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_payment_params.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_purchase_params.py
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_shared_access_params.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_subscription_params.py
+-rw-r--r--   0 root         (0) root         (0)      233 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/linked_term_upgrade_params.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/locale_model.py
+-rw-r--r--   0 root         (0) root         (0)      225 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/mail.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/mail_log.py
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/mail_options_verification_result.py
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/mandate.py
+-rw-r--r--   0 root         (0) root         (0)      283 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/money.py
+-rw-r--r--   0 root         (0) root         (0)      193 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/my_account.py
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/newscycle_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/newscycle_configuration_test_result.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/obi_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      649 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_model.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_categories.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_content_field.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_histories.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_history.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_revision.py
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_sub_history.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_variant.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/offer_template_version.py
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/one_source_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      560 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/openpay_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      335 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/pay_source_dto.py
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/payee_settings_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/payment_inquiry.py
+-rw-r--r--   0 root         (0) root         (0)      530 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/payment_method.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/payment_method_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/payment_provider_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/payment_refund_event.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/paypal_express_checkout_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/period.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/period_link.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/period_link_candidate.py
+-rw-r--r--   0 root         (0) root         (0)      551 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/period_settings.py
+-rw-r--r--   0 root         (0) root         (0)      330 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/permission_dto.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/pp_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/ppc_web_model.py
+-rw-r--r--   0 root         (0) root         (0)      307 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/price_dto.py
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/promo_code.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/promotion.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/promotion_applicable_term_container.py
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/promotion_fixed_discount.py
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/promotion_stats.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/promotion_term_stats.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/reallocation_batch.py
+-rw-r--r--   0 root         (0) root         (0)      203 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/redemption_page.py
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/region.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/region_simple_model.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/rendered_email.py
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/report_response.py
+-rw-r--r--   0 root         (0) root         (0)      832 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/resource.py
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/resource_compact_stats.py
+-rw-r--r--   0 root         (0) root         (0)      838 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/resource_dto.py
+-rw-r--r--   0 root         (0) root         (0)      341 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/resource_stats.py
+-rw-r--r--   0 root         (0) root         (0)      266 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/resource_tag.py
+-rw-r--r--   0 root         (0) root         (0)      561 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/result.py
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/sales_tax_rate_model.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/schedule.py
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/schedule_period.py
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/sections_counters.py
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/send_email_step.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/shared_account_param.py
+-rw-r--r--   0 root         (0) root         (0)      585 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/shared_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/shared_subscription_child_access_granted_event.py
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/source.py
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/source_eligible_term.py
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/source_ineligible_term.py
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/source_term_change_variant.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/source_term_change_variants.py
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/split_test_object.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/spreedly_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/stripe_properties.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/stripe_setup_intent_model_definition.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_auto_renew_changed_by_end_user_event.py
+-rw-r--r--   0 root         (0) root         (0)      609 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_log_item.py
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_migration_history_dto.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_reallocation_error.py
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_reallocation_validation_result.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_renewal_event.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_restrictions.py
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_term_change_options.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/subscription_upgrade_status.py
+-rw-r--r--   0 root         (0) root         (0)      817 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/target_eligible_term.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/target_ineligible_term.py
+-rw-r--r--   0 root         (0) root         (0)      676 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/target_term_change_variant.py
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/target_term_change_variants.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/target_upgrade_option.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/tax_country.py
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/tax_support_dto.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/team_member.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/template_config.py
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/template_counter_model.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/template_user_model.py
+-rw-r--r--   0 root         (0) root         (0)      361 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/template_variable.py
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/template_version.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term.py
+-rw-r--r--   0 root         (0) root         (0)      259 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_brief.py
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_change_billing_options.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_change_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_change_finished_event.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_change_option.py
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_change_params.py
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_change_variants.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_changed_event.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_conversion.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_conversion_data.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_conversion_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_conversion_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_from.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_link.py
+-rw-r--r--   0 root         (0) root         (0)      780 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_period_reallocation.py
+-rw-r--r--   0 root         (0) root         (0)      545 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_reallocation.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_short.py
+-rw-r--r--   0 root         (0) root         (0)      341 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_to_eligible.py
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_to_ineligible.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_to_upgrade_option.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/term_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/tern_change_confirmation_dto.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/test_event.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/transaction_item.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/translation_map_revision.py
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/translation_stats.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/unknown_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/unsupported_event.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/update_access_period_params.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/update_billing_configuration_request.py
+-rw-r--r--   0 root         (0) root         (0)      589 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/update_linked_term_request.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/upgrade_checkout_flow.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/upgrade_offer.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/upgrade_offer_variant.py
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/upgrade_sources.py
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/upgrade_subscription_step.py
+-rw-r--r--   0 root         (0) root         (0)      645 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/upgrade_targets.py
+-rw-r--r--   0 root         (0) root         (0)      666 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user.py
+-rw-r--r--   0 root         (0) root         (0)      684 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_access_dto.py
+-rw-r--r--   0 root         (0) root         (0)      755 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_address.py
+-rw-r--r--   0 root         (0) root         (0)      528 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_address_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_address_history.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_address_updated_event.py
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_alias_dto.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_audit.py
+-rw-r--r--   0 root         (0) root         (0)      764 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_billing_address.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_conversion_dto.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_created_event.py
+-rw-r--r--   0 root         (0) root         (0)      751 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_details.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_disabled_event.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_email_confirmed_event.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_info.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_note.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_payment.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_payment_details_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_payment_dto.py
+-rw-r--r--   0 root         (0) root         (0)      668 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_payment_info.py
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_payment_method_event.py
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_payment_refund_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_provider_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      332 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_subscription_account.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_subscription_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_subscription_list_item.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/user_updated_event.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/users_import_result.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/variant_item.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/version_item.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/voucher.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/voucher_delivered_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/voucher_purchased_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/voucher_redeemed_event.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/voucher_revoked_event.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/vouchering_policy.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/webhook_config.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/webhook_event.py
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/webhook_response.py
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/webhook_settings.py
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/webhook_status.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/worldpay_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/worldpay_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/zuora_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-26 20:12:44.000000 pianosdk-16.188.1/pianosdk/publisher/models/zuora_connect_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.332666 pianosdk-16.188.1/pianosdk/user/
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.332666 pianosdk-16.188.1/pianosdk/user/api/
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4244 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/api/user_access_api.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/api/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.336666 pianosdk-16.188.1/pianosdk/user/models/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      566 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/access.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/access_dto.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/country.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/geo_location.py
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/region.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/resource.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/resource_dto.py
+-rw-r--r--   0 root         (0) root         (0)      356 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/user.py
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/user_address.py
+-rw-r--r--   0 root         (0) root         (0)      362 2024-05-26 20:12:43.000000 pianosdk-16.188.1/pianosdk/user/models/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11563 2024-05-26 20:12:46.000000 pianosdk-16.188.1/pianosdk/webhook_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 20:12:57.336666 pianosdk-16.188.1/pianosdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-05-26 20:12:57.000000 pianosdk-16.188.1/pianosdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26837 2024-05-26 20:12:57.000000 pianosdk-16.188.1/pianosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 20:12:57.000000 pianosdk-16.188.1/pianosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-26 20:12:57.000000 pianosdk-16.188.1/pianosdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-26 20:12:57.000000 pianosdk-16.188.1/pianosdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-05-26 20:12:57.336666 pianosdk-16.188.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-26 20:12:46.000000 pianosdk-16.188.1/setup.py
```

### Comparing `pianosdk-16.182.0/PKG-INFO` & `pianosdk-16.188.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pianosdk
-Version: 16.182.0
+Version: 16.188.1
 Summary: Piano API SDK
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pianosdk-16.182.0/README.md` & `pianosdk-16.188.1/README.md`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/__init__.py` & `pianosdk-16.188.1/pianosdk/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/access_token.py` & `pianosdk-16.188.1/pianosdk/access_token.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/__init__.py` & `pianosdk-16.188.1/pianosdk/anon/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/__init__.py` & `pianosdk-16.188.1/pianosdk/anon/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/access_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/access_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/access_token_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/access_token_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/anon_assets_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/anon_assets_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/anon_country_list_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/anon_country_list_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/anon_error_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/anon_error_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/anon_mobile_sdk_id_deployment_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/anon_mobile_sdk_id_deployment_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/anon_user_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/anon_user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/anon_user_disable_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/anon_user_disable_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/conversion_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/conversion_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/conversion_external_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/conversion_external_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/conversion_registration_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/conversion_registration_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/email_confirmation_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/email_confirmation_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/oauth_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/oauth_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/subscription_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/subscription_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/api/swg_sync_api.py` & `pianosdk-16.188.1/pianosdk/anon/api/swg_sync_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/__init__.py` & `pianosdk-16.188.1/pianosdk/anon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/access.py` & `pianosdk-16.188.1/pianosdk/anon/models/access.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/access_dto.py` & `pianosdk-16.188.1/pianosdk/anon/models/access_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/light_offer_template_version.py` & `pianosdk-16.188.1/pianosdk/anon/models/light_offer_template_version.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/linked_term_event_session.py` & `pianosdk-16.188.1/pianosdk/anon/models/linked_term_event_session.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/linked_term_session_params.py` & `pianosdk-16.188.1/pianosdk/anon/models/linked_term_session_params.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/passwordless_purchase_complete_result.py` & `pianosdk-16.188.1/pianosdk/anon/models/passwordless_purchase_complete_result.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/anon/models/user_subscription.py` & `pianosdk-16.188.1/pianosdk/anon/models/user_subscription.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/base_api.py` & `pianosdk-16.188.1/pianosdk/base_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/configuration.py` & `pianosdk-16.188.1/pianosdk/configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/httpwrap/__init__.py` & `pianosdk-16.188.1/pianosdk/httpwrap/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/httpwrap/models.py` & `pianosdk-16.188.1/pianosdk/httpwrap/models.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/httpwrap/requests_client.py` & `pianosdk-16.188.1/pianosdk/httpwrap/requests_client.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/__init__.py` & `pianosdk-16.188.1/pianosdk/id/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/__init__.py` & `pianosdk-16.188.1/pianosdk/id/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/identity_oauth_api.py` & `pianosdk-16.188.1/pianosdk/id/api/identity_oauth_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/identity_token_api.py` & `pianosdk-16.188.1/pianosdk/id/api/identity_token_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_audit_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_audit_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_form_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_form_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_identity_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_identity_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_identity_set_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_identity_set_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_import_custom_fields_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_import_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_login_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_login_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_login_social_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_login_social_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_reset_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_reset_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_token_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_token_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/api/publisher_users_api.py` & `pianosdk-16.188.1/pianosdk/id/api/publisher_users_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/__init__.py` & `pianosdk-16.188.1/pianosdk/id/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/custom_field_attribute_dto.py` & `pianosdk-16.188.1/pianosdk/id/models/custom_field_attribute_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/custom_field_definition_dto.py` & `pianosdk-16.188.1/pianosdk/id/models/custom_field_definition_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/publisher_register_request.py` & `pianosdk-16.188.1/pianosdk/id/models/publisher_register_request.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/publisher_user_profile_response.py` & `pianosdk-16.188.1/pianosdk/id/models/publisher_user_profile_response.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/social_additional_input_request.py` & `pianosdk-16.188.1/pianosdk/id/models/social_additional_input_request.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/social_linking_response.py` & `pianosdk-16.188.1/pianosdk/id/models/social_linking_response.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/id/models/token_response.py` & `pianosdk-16.188.1/pianosdk/id/models/token_response.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/piano_client.py` & `pianosdk-16.188.1/pianosdk/piano_client.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/__init__.py` & `pianosdk-16.188.1/pianosdk/publisher/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 from pianosdk.publisher.models.permission_dto import PermissionDTO
 from pianosdk.publisher.models.pp_configuration import PpConfiguration
 from pianosdk.publisher.models.ppc_web_model import PpcWebModel
 from pianosdk.publisher.models.price_dto import PriceDTO
 from pianosdk.publisher.models.promo_code import PromoCode
 from pianosdk.publisher.models.promotion import Promotion
 from pianosdk.publisher.models.promotion_applicable_term_container import PromotionApplicableTermContainer
-from pianosdk.publisher.models.promotion_fixed_discountt import PromotionFixedDiscountt
+from pianosdk.publisher.models.promotion_fixed_discount import PromotionFixedDiscount
 from pianosdk.publisher.models.promotion_stats import PromotionStats
 from pianosdk.publisher.models.promotion_term_stats import PromotionTermStats
 from pianosdk.publisher.models.reallocation_batch import ReallocationBatch
 from pianosdk.publisher.models.redemption_page import RedemptionPage
 from pianosdk.publisher.models.region import Region
 from pianosdk.publisher.models.region_simple_model import RegionSimpleModel
 from pianosdk.publisher.models.rendered_email import RenderedEmail
```

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/__init__.py` & `pianosdk-16.188.1/pianosdk/publisher/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_adblocker_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_adblocker_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_app_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_app_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_app_api_token_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_app_api_token_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_app_features_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_app_features_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_consent_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_consent_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_consent_entry_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_consent_entry_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_custom_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_custom_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_data_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_data_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_external_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_external_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_conversion_registration_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_conversion_registration_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_aam_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_aam_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_aam_monthly_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_aam_monthly_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_access_report_export_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_access_report_export_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_subscription_details_report_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_subscription_details_report_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_export_create_transactions_report_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_export_create_transactions_report_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_gdpr_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_gdpr_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_inquiry_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_inquiry_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_domain_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_domain_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_domain_contract_user_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_domain_contract_user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_ip_range_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_ip_range_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_periods_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_periods_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_contract_user_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_contract_user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_licensee_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_licensee_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_notification_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_notification_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_notification_rule_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_notification_rule_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_schedule_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_schedule_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_licensing_schedule_contract_periods_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_licensing_schedule_contract_periods_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_linked_term_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_linked_term_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_linked_term_custom_field_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_linked_term_custom_field_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_create_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_create_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_inherited_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_inherited_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_update_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_update_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_template_variant_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_template_variant_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_term_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_term_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_offer_term_offer_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_offer_term_offer_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_method_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_method_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_method_billing_address_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_method_billing_address_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_method_gmo_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_method_gmo_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_payment_provider_configuration_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_payment_provider_configuration_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_code_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_code_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_fixed_discount_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_fixed_discount_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from typing import TextIO, Dict, List, Union
 
 from pianosdk.api_response import ApiResponse
 from pianosdk.base_api import BaseApi
 from pianosdk.configuration import Configuration
 from pianosdk.httpwrap import HttpCallBack
 from pianosdk.utils import _json_deserialize, _encode_parameter
-from pianosdk.publisher.models.promotion_fixed_discountt import PromotionFixedDiscountt
+from pianosdk.publisher.models.promotion_fixed_discount import PromotionFixedDiscount
 
 
 class PublisherPromotionFixedDiscountApi(BaseApi):
     def __init__(self, config: Configuration, http_callback: HttpCallBack = None) -> None:
         super().__init__(config, http_callback)
 
-    def create(self, promotion_id: str, aid: str, amount: float, currency: str) -> ApiResponse[PromotionFixedDiscountt]:
+    def create(self, promotion_id: str, aid: str, amount: float, currency: str) -> ApiResponse[PromotionFixedDiscount]:
         _url_path = '/api/v3/publisher/promotion/fixedDiscount/add'
         _query_url = self.config.get_base_url() + _url_path
         _query_parameters = {
             'promotion_id': _encode_parameter(promotion_id),
             'aid': _encode_parameter(aid),
             'amount': _encode_parameter(amount),
             'currency': _encode_parameter(currency)
@@ -40,15 +40,15 @@
                                                          _query_url,
                                                          headers=_headers,
                                                          query_parameters=_query_parameters,
                                                          parameters=_parameters,
                                                          json=_body,
                                                          files=_files)
         _response = self._execute_request(_request)
-        _result = _json_deserialize(_response, PromotionFixedDiscountt)
+        _result = _json_deserialize(_response, PromotionFixedDiscount)
         return _result
 
     def delete(self, fixed_discount_id: str, aid: str) -> ApiResponse[Dict]:
         _url_path = '/api/v3/publisher/promotion/fixedDiscount/delete'
         _query_url = self.config.get_base_url() + _url_path
         _query_parameters = {
 
@@ -74,15 +74,15 @@
                                                          parameters=_parameters,
                                                          json=_body,
                                                          files=_files)
         _response = self._execute_request(_request)
         _result = _json_deserialize(_response)
         return _result
 
-    def update(self, fixed_discount_id: str, aid: str, amount: float, currency: str) -> ApiResponse[PromotionFixedDiscountt]:
+    def update(self, fixed_discount_id: str, aid: str, amount: float, currency: str) -> ApiResponse[PromotionFixedDiscount]:
         _url_path = '/api/v3/publisher/promotion/fixedDiscount/update'
         _query_url = self.config.get_base_url() + _url_path
         _query_parameters = {
 
         }
 
         _headers = {
@@ -104,10 +104,10 @@
                                                          _query_url,
                                                          headers=_headers,
                                                          query_parameters=_query_parameters,
                                                          parameters=_parameters,
                                                          json=_body,
                                                          files=_files)
         _response = self._execute_request(_request)
-        _result = _json_deserialize(_response, PromotionFixedDiscountt)
+        _result = _json_deserialize(_response, PromotionFixedDiscount)
         return _result
```

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_promotion_term_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_promotion_term_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_bundle_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_bundle_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_cross_app_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_cross_app_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_stats_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_stats_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_tag_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_tag_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_resource_user_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_resource_user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_schedule_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_schedule_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_schedule_period_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_schedule_period_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_address_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_address_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_cancel_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_cancel_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_share_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_share_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_subscription_share_user_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_subscription_share_user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_team_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_team_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_change_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_change_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_change_option_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_change_option_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_custom_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_custom_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_dynamic_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_dynamic_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_external_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_external_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_gift_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_gift_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_payment_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_payment_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_registration_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_registration_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_term_stats_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_term_stats_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_test_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_test_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_access_active_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_access_active_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_access_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_access_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_address_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_address_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_app_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_app_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_billing_address_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_billing_address_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_bulk_import_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_bulk_import_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_email_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_email_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_list_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_list_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_user_note_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_user_note_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_voucher_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_voucher_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_webhook_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_webhook_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_webhook_response_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_webhook_response_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/api/publisher_webhook_settings_api.py` & `pianosdk-16.188.1/pianosdk/publisher/api/publisher_webhook_settings_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/__init__.py` & `pianosdk-16.188.1/pianosdk/publisher/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 from pianosdk.publisher.models.permission_dto import PermissionDTO
 from pianosdk.publisher.models.pp_configuration import PpConfiguration
 from pianosdk.publisher.models.ppc_web_model import PpcWebModel
 from pianosdk.publisher.models.price_dto import PriceDTO
 from pianosdk.publisher.models.promo_code import PromoCode
 from pianosdk.publisher.models.promotion import Promotion
 from pianosdk.publisher.models.promotion_applicable_term_container import PromotionApplicableTermContainer
-from pianosdk.publisher.models.promotion_fixed_discountt import PromotionFixedDiscountt
+from pianosdk.publisher.models.promotion_fixed_discount import PromotionFixedDiscount
 from pianosdk.publisher.models.promotion_stats import PromotionStats
 from pianosdk.publisher.models.promotion_term_stats import PromotionTermStats
 from pianosdk.publisher.models.reallocation_batch import ReallocationBatch
 from pianosdk.publisher.models.redemption_page import RedemptionPage
 from pianosdk.publisher.models.region import Region
 from pianosdk.publisher.models.region_simple_model import RegionSimpleModel
 from pianosdk.publisher.models.rendered_email import RenderedEmail
```

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/access.py` & `pianosdk-16.188.1/pianosdk/publisher/models/access.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/access_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/access_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/action.py` & `pianosdk-16.188.1/pianosdk/publisher/models/action.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/action_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/action_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/action_step_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/action_step_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/advanced_email_model.py` & `pianosdk-16.188.1/pianosdk/publisher/models/advanced_email_model.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/app.py` & `pianosdk-16.188.1/pianosdk/publisher/models/app.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/app_features.py` & `pianosdk-16.188.1/pianosdk/publisher/models/app_features.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/avalara_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/avalara_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/bill.py` & `pianosdk-16.188.1/pianosdk/publisher/models/bill.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/braintree_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/braintree_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/checkout_flow.py` & `pianosdk-16.188.1/pianosdk/publisher/models/checkout_flow.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/checkout_flow_light_model.py` & `pianosdk-16.188.1/pianosdk/publisher/models/checkout_flow_light_model.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/consent.py` & `pianosdk-16.188.1/pianosdk/publisher/models/consent.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/contract.py` & `pianosdk-16.188.1/pianosdk/publisher/models/contract.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/contract_details.py` & `pianosdk-16.188.1/pianosdk/publisher/models/contract_details.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/create_access_period_params.py` & `pianosdk-16.188.1/pianosdk/publisher/models/create_access_period_params.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/create_linked_term_request.py` & `pianosdk-16.188.1/pianosdk/publisher/models/create_linked_term_request.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/credit_guard_stored_fields.py` & `pianosdk-16.188.1/pianosdk/publisher/models/credit_guard_stored_fields.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/deployment_app_details.py` & `pianosdk-16.188.1/pianosdk/publisher/models/deployment_app_details.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/deployment_details.py` & `pianosdk-16.188.1/pianosdk/publisher/models/deployment_details.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/deployment_list_item.py` & `pianosdk-16.188.1/pianosdk/publisher/models/deployment_list_item.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/dynamic_subscription_access_period_info.py` & `pianosdk-16.188.1/pianosdk/publisher/models/dynamic_subscription_access_period_info.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/easypay_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/easypay_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/erase_user_payment.py` & `pianosdk-16.188.1/pianosdk/publisher/models/erase_user_payment.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/erase_user_payment_info.py` & `pianosdk-16.188.1/pianosdk/publisher/models/erase_user_payment_info.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/erase_user_response.py` & `pianosdk-16.188.1/pianosdk/publisher/models/erase_user_response.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/experience.py` & `pianosdk-16.188.1/pianosdk/publisher/models/experience.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/export.py` & `pianosdk-16.188.1/pianosdk/publisher/models/export.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/ext_provider_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/ext_provider_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/external_api_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/external_api_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/global_template.py` & `pianosdk-16.188.1/pianosdk/publisher/models/global_template.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/global_template_filter.py` & `pianosdk-16.188.1/pianosdk/publisher/models/global_template_filter.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/global_template_version.py` & `pianosdk-16.188.1/pianosdk/publisher/models/global_template_version.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/import_item.py` & `pianosdk-16.188.1/pianosdk/publisher/models/import_item.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/inquiry_comment.py` & `pianosdk-16.188.1/pianosdk/publisher/models/inquiry_comment.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/klarna_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/klarna_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/licensee.py` & `pianosdk-16.188.1/pianosdk/publisher/models/licensee.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/light_global_template.py` & `pianosdk-16.188.1/pianosdk/publisher/models/light_global_template.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/link_candidate.py` & `pianosdk-16.188.1/pianosdk/publisher/models/link_candidate.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/linked_term_configuration_request.py` & `pianosdk-16.188.1/pianosdk/publisher/models/linked_term_configuration_request.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/linked_term_event_request.py` & `pianosdk-16.188.1/pianosdk/publisher/models/linked_term_event_request.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/linked_term_subscription_params.py` & `pianosdk-16.188.1/pianosdk/publisher/models/linked_term_subscription_params.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/mail_log.py` & `pianosdk-16.188.1/pianosdk/publisher/models/mail_log.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/mail_options_verification_result.py` & `pianosdk-16.188.1/pianosdk/publisher/models/mail_options_verification_result.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/obi_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/obi_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/offer_model.py` & `pianosdk-16.188.1/pianosdk/publisher/models/offer_model.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/offer_template.py` & `pianosdk-16.188.1/pianosdk/publisher/models/offer_template.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/offer_template_history.py` & `pianosdk-16.188.1/pianosdk/publisher/models/offer_template_history.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/offer_template_revision.py` & `pianosdk-16.188.1/pianosdk/publisher/models/offer_template_revision.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/offer_template_variant.py` & `pianosdk-16.188.1/pianosdk/publisher/models/offer_template_variant.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/offer_template_version.py` & `pianosdk-16.188.1/pianosdk/publisher/models/offer_template_version.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/openpay_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/openpay_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/payment_inquiry.py` & `pianosdk-16.188.1/pianosdk/publisher/models/payment_inquiry.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/payment_method.py` & `pianosdk-16.188.1/pianosdk/publisher/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/payment_method_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/payment_method_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/payment_provider_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/payment_provider_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/paypal_express_checkout_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/paypal_express_checkout_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/period.py` & `pianosdk-16.188.1/pianosdk/publisher/models/period.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/period_settings.py` & `pianosdk-16.188.1/pianosdk/publisher/models/period_settings.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/pp_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/pp_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/ppc_web_model.py` & `pianosdk-16.188.1/pianosdk/publisher/models/ppc_web_model.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/promo_code.py` & `pianosdk-16.188.1/pianosdk/publisher/models/promo_code.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/promotion.py` & `pianosdk-16.188.1/pianosdk/publisher/models/promotion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import date, datetime
 from pydantic.main import BaseModel
 from typing import Optional
-from pianosdk.publisher.models.promotion_fixed_discountt import PromotionFixedDiscountt
+from pianosdk.publisher.models.promotion_fixed_discount import PromotionFixedDiscount
 from typing import List
 
 
 class Promotion(BaseModel):
     promotion_id: Optional[str] = None
     aid: Optional[str] = None
     name: Optional[str] = None
@@ -26,14 +26,14 @@
     start_date: Optional[datetime] = None
     end_date: Optional[datetime] = None
     create_date: Optional[datetime] = None
     create_by: Optional[str] = None
     update_date: Optional[datetime] = None
     update_by: Optional[str] = None
     deleted: Optional[bool] = None
-    fixed_discount_list: Optional['List[PromotionFixedDiscountt]'] = None
+    fixed_discount_list: Optional['List[PromotionFixedDiscount]'] = None
     apply_to_all_billing_periods: Optional[bool] = None
     can_be_applied_on_renewal: Optional[bool] = None
     billing_period_limit: Optional[int] = None
 
 
 Promotion.model_rebuild()
```

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/resource.py` & `pianosdk-16.188.1/pianosdk/publisher/models/resource.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/resource_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/resource_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/result.py` & `pianosdk-16.188.1/pianosdk/publisher/models/result.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/shared_subscription.py` & `pianosdk-16.188.1/pianosdk/publisher/models/shared_subscription.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/source_term_change_variant.py` & `pianosdk-16.188.1/pianosdk/publisher/models/source_term_change_variant.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/spreedly_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/spreedly_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/subscription_log_item.py` & `pianosdk-16.188.1/pianosdk/publisher/models/subscription_log_item.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/subscription_term_change_options.py` & `pianosdk-16.188.1/pianosdk/publisher/models/subscription_term_change_options.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/subscription_upgrade_status.py` & `pianosdk-16.188.1/pianosdk/publisher/models/subscription_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/target_eligible_term.py` & `pianosdk-16.188.1/pianosdk/publisher/models/target_eligible_term.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/target_term_change_variant.py` & `pianosdk-16.188.1/pianosdk/publisher/models/target_term_change_variant.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/target_upgrade_option.py` & `pianosdk-16.188.1/pianosdk/publisher/models/target_upgrade_option.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/team_member.py` & `pianosdk-16.188.1/pianosdk/publisher/models/team_member.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/template_config.py` & `pianosdk-16.188.1/pianosdk/publisher/models/template_config.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/template_version.py` & `pianosdk-16.188.1/pianosdk/publisher/models/template_version.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_change_option.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_change_option.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_change_variants.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_change_variants.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_conversion.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_conversion.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_conversion_data.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_conversion_data.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_conversion_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_conversion_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_conversion_subscription.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_conversion_subscription.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_period_reallocation.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_period_reallocation.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_reallocation.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_reallocation.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_to_eligible.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_to_eligible.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/term_to_upgrade_option.py` & `pianosdk-16.188.1/pianosdk/publisher/models/term_to_upgrade_option.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/tern_change_confirmation_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/tern_change_confirmation_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/transaction_item.py` & `pianosdk-16.188.1/pianosdk/publisher/models/transaction_item.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/update_access_period_params.py` & `pianosdk-16.188.1/pianosdk/publisher/models/update_access_period_params.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/update_linked_term_request.py` & `pianosdk-16.188.1/pianosdk/publisher/models/update_linked_term_request.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/upgrade_checkout_flow.py` & `pianosdk-16.188.1/pianosdk/publisher/models/upgrade_checkout_flow.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/upgrade_subscription_step.py` & `pianosdk-16.188.1/pianosdk/publisher/models/upgrade_subscription_step.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/upgrade_targets.py` & `pianosdk-16.188.1/pianosdk/publisher/models/upgrade_targets.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_access_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_access_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_address.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_address.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_address_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_address_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_address_history.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_address_history.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_audit.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_audit.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_billing_address.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_billing_address.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_details.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_details.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_info.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_info.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_note.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_note.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_payment.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_payment.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_payment_details_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_payment_details_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_payment_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_payment_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_payment_info.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_payment_info.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_provider_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_provider_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_subscription.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_subscription.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_subscription_dto.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_subscription_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,11 @@
     psc_subscriber_number: Optional[str] = None
     conversion_result: Optional[str] = None
     external_api_name: Optional[str] = None
     charge_count: Optional[int] = None
     status_display: Optional[str] = None
     auto_renew: Optional[bool] = None
     user_payment_info_id: Optional[str] = None
+    access_id: Optional[str] = None
 
 
 UserSubscriptionDto.model_rebuild()
```

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/user_subscription_list_item.py` & `pianosdk-16.188.1/pianosdk/publisher/models/user_subscription_list_item.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/voucher.py` & `pianosdk-16.188.1/pianosdk/publisher/models/voucher.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/webhook_event.py` & `pianosdk-16.188.1/pianosdk/publisher/models/webhook_event.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/publisher/models/worldpay_configuration.py` & `pianosdk-16.188.1/pianosdk/publisher/models/worldpay_configuration.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/__init__.py` & `pianosdk-16.188.1/pianosdk/user/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/api/user_access_api.py` & `pianosdk-16.188.1/pianosdk/user/api/user_access_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/api/user_api.py` & `pianosdk-16.188.1/pianosdk/user/api/user_api.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/models/__init__.py` & `pianosdk-16.188.1/pianosdk/user/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/models/access.py` & `pianosdk-16.188.1/pianosdk/user/models/access.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/models/access_dto.py` & `pianosdk-16.188.1/pianosdk/user/models/access_dto.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/user/models/user_address.py` & `pianosdk-16.188.1/pianosdk/user/models/user_address.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/utils.py` & `pianosdk-16.188.1/pianosdk/utils.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk/webhook_events.py` & `pianosdk-16.188.1/pianosdk/webhook_events.py`

 * *Files identical despite different names*

### Comparing `pianosdk-16.182.0/pianosdk.egg-info/PKG-INFO` & `pianosdk-16.188.1/pianosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pianosdk
-Version: 16.182.0
+Version: 16.188.1
 Summary: Piano API SDK
 License: Apache License, Version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pianosdk-16.182.0/pianosdk.egg-info/SOURCES.txt` & `pianosdk-16.188.1/pianosdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
 pianosdk/publisher/models/permission_dto.py
 pianosdk/publisher/models/pp_configuration.py
 pianosdk/publisher/models/ppc_web_model.py
 pianosdk/publisher/models/price_dto.py
 pianosdk/publisher/models/promo_code.py
 pianosdk/publisher/models/promotion.py
 pianosdk/publisher/models/promotion_applicable_term_container.py
-pianosdk/publisher/models/promotion_fixed_discountt.py
+pianosdk/publisher/models/promotion_fixed_discount.py
 pianosdk/publisher/models/promotion_stats.py
 pianosdk/publisher/models/promotion_term_stats.py
 pianosdk/publisher/models/reallocation_batch.py
 pianosdk/publisher/models/redemption_page.py
 pianosdk/publisher/models/region.py
 pianosdk/publisher/models/region_simple_model.py
 pianosdk/publisher/models/rendered_email.py
```

### Comparing `pianosdk-16.182.0/setup.py` & `pianosdk-16.188.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='pianosdk',
-    version='16.182.0',
+    version='16.188.1',
     packages=find_packages(),
     # url='url will be here',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
```

