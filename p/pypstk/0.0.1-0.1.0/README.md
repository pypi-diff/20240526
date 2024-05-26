# Comparing `tmp/pypstk-0.0.1.tar.gz` & `tmp/pypstk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypstk-0.0.1.tar", last modified: Sun May 26 13:29:43 2024, max compression
+gzip compressed data, was "pypstk-0.1.0.tar", last modified: Sun May 26 14:43:18 2024, max compression
```

## Comparing `pypstk-0.0.1.tar` & `pypstk-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 13:29:43.380392 pypstk-0.0.1/
--rw-rw-rw-   0        0        0     1071 2024-05-26 13:28:43.000000 pypstk-0.0.1/LIcence
--rw-rw-rw-   0        0        0     2152 2024-05-26 13:29:43.374708 pypstk-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 13:29:43.341753 pypstk-0.0.1/PythonPaystackv2/
--rw-rw-rw-   0        0        0       96 2024-05-26 02:55:10.000000 pypstk-0.0.1/PythonPaystackv2/__init__.py
--rw-rw-rw-   0        0        0     1317 2024-05-26 02:51:03.000000 pypstk-0.0.1/PythonPaystackv2/payment.py
--rw-rw-rw-   0        0        0     1121 2024-05-26 02:54:38.000000 pypstk-0.0.1/PythonPaystackv2/status.py
--rw-rw-rw-   0        0        0     1716 2024-05-26 02:56:42.000000 pypstk-0.0.1/PythonPaystackv2/subscription.py
--rw-rw-rw-   0        0        0     1692 2024-05-26 13:28:53.000000 pypstk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 13:29:43.372713 pypstk-0.0.1/pypstk.egg-info/
--rw-rw-rw-   0        0        0     2152 2024-05-26 13:29:43.000000 pypstk-0.0.1/pypstk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-26 13:29:43.000000 pypstk-0.0.1/pypstk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 13:29:43.000000 pypstk-0.0.1/pypstk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 13:29:43.000000 pypstk-0.0.1/pypstk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 13:29:43.000000 pypstk-0.0.1/pypstk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 13:29:43.380392 pypstk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      692 2024-05-26 13:28:13.000000 pypstk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:43:18.753147 pypstk-0.1.0/
+-rw-rw-rw-   0        0        0     1071 2024-05-26 13:28:43.000000 pypstk-0.1.0/LIcence
+-rw-rw-rw-   0        0        0     2123 2024-05-26 14:43:18.745191 pypstk-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2024-05-26 14:42:29.000000 pypstk-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 14:43:18.675994 pypstk-0.1.0/pypstk/
+-rw-rw-rw-   0        0        0      102 2024-05-26 14:36:34.000000 pypstk-0.1.0/pypstk/__init__.py
+-rw-rw-rw-   0        0        0     1317 2024-05-26 02:51:03.000000 pypstk-0.1.0/pypstk/payment.py
+-rw-rw-rw-   0        0        0     1121 2024-05-26 02:54:38.000000 pypstk-0.1.0/pypstk/status.py
+-rw-rw-rw-   0        0        0     1716 2024-05-26 02:56:42.000000 pypstk-0.1.0/pypstk/subscription.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:43:18.741185 pypstk-0.1.0/pypstk.egg-info/
+-rw-rw-rw-   0        0        0     2123 2024-05-26 14:43:18.000000 pypstk-0.1.0/pypstk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-26 14:43:18.000000 pypstk-0.1.0/pypstk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:43:18.000000 pypstk-0.1.0/pypstk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 14:43:18.000000 pypstk-0.1.0/pypstk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 14:43:18.000000 pypstk-0.1.0/pypstk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:43:18.754145 pypstk-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      692 2024-05-26 14:41:29.000000 pypstk-0.1.0/setup.py
```

### Comparing `pypstk-0.0.1/LIcence` & `pypstk-0.1.0/LIcence`

 * *Files identical despite different names*

### Comparing `pypstk-0.0.1/PKG-INFO` & `pypstk-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypstk
-Version: 0.0.1
+Version: 0.1.0
 Home-page: https://github.com/emekadefirst/Paystack-Python-2-SDK
 Author: Victor Chibuogwu Chukwuemeka aka Emekadefirst
 Author-email: emekadefirst@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -24,34 +24,34 @@
 ```
 
 ## Usage
 
 ### 1. Payment
 
 ```python
-from payment import Pay
+from PythonPaystackv2.payment import Payment
 
-# Initialize payment
 email = "customer@email.com"
 amount = "20000"
-secret_key = "sk_test_6215942a0765956d18f05e4f52a12a6a8902cee2"
+secret_key = "your secret_key from api"
 
-new_payment = Pay(email, amount, secret_key)
+new_payment = Payment(email, amount, secret_key)
 transaction_data = new_payment.initialize_transaction()
 print(transaction_data)
 
 # Sample output:
-# {'status': True, 'message': 'Authorization URL created', 'data': {'authorization_url': 'https://checkout.paystack.com/1hxv7un'}}
+# {'references': '8pr6trcjj5', 'url': 'https://checkout.paystack.com/j62hay03a7dj6iu'}
+
 ```
 
 
 ### 3. Subscription
 
 ```python
-from subscription import Subscription
+from PythonPaystackv2.subscription import Subscription
 
 # Initialize subscription payment
 name = "Monthly Retainer"
 interval = "monthly"
 amount = 500000
 secret_key = "sk_test_daf386e7071c4613e54e4b71f43926409abd811e"
 
@@ -59,15 +59,15 @@
 pay_subscription.initialize_payment()
 pay_subscription.payment_status()
 ```
 
 ### 4. Webhook
 
 ```python
-from status import Verify
+from PythonPaystackv2.status import Verify
 
 # Check webhook status
 reference = "YOUR_REFERENCE"
 secret_key = "YOUR_SECRET_KEY"
 
 hook = Hook(reference, secret_key)
 status = hook.status()
```

### Comparing `pypstk-0.0.1/PythonPaystackv2/payment.py` & `pypstk-0.1.0/pypstk/payment.py`

 * *Files identical despite different names*

### Comparing `pypstk-0.0.1/PythonPaystackv2/status.py` & `pypstk-0.1.0/pypstk/status.py`

 * *Files identical despite different names*

### Comparing `pypstk-0.0.1/PythonPaystackv2/subscription.py` & `pypstk-0.1.0/pypstk/subscription.py`

 * *Files identical despite different names*

### Comparing `pypstk-0.0.1/README.md` & `pypstk-0.1.0/pypstk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pypstk
+Version: 0.1.0
+Home-page: https://github.com/emekadefirst/Paystack-Python-2-SDK
+Author: Victor Chibuogwu Chukwuemeka aka Emekadefirst
+Author-email: emekadefirst@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LIcence
+Requires-Dist: requests>=2.26.0
+
 # Pystack
 
 This Python package provides a set of classes to interact with the Paystack API for handling transactions, customers, subscriptions, and webhooks.
 
 ## Installation
 
 To use this package, you need to have Python installed. You can install the package using pip:
@@ -11,34 +24,34 @@
 ```
 
 ## Usage
 
 ### 1. Payment
 
 ```python
-from payment import Pay
+from PythonPaystackv2.payment import Payment
 
-# Initialize payment
 email = "customer@email.com"
 amount = "20000"
-secret_key = "sk_test_6215942a0765956d18f05e4f52a12a6a8902cee2"
+secret_key = "your secret_key from api"
 
-new_payment = Pay(email, amount, secret_key)
+new_payment = Payment(email, amount, secret_key)
 transaction_data = new_payment.initialize_transaction()
 print(transaction_data)
 
 # Sample output:
-# {'status': True, 'message': 'Authorization URL created', 'data': {'authorization_url': 'https://checkout.paystack.com/1hxv7un'}}
+# {'references': '8pr6trcjj5', 'url': 'https://checkout.paystack.com/j62hay03a7dj6iu'}
+
 ```
 
 
 ### 3. Subscription
 
 ```python
-from subscription import Subscription
+from PythonPaystackv2.subscription import Subscription
 
 # Initialize subscription payment
 name = "Monthly Retainer"
 interval = "monthly"
 amount = 500000
 secret_key = "sk_test_daf386e7071c4613e54e4b71f43926409abd811e"
 
@@ -46,15 +59,15 @@
 pay_subscription.initialize_payment()
 pay_subscription.payment_status()
 ```
 
 ### 4. Webhook
 
 ```python
-from status import Verify
+from PythonPaystackv2.status import Verify
 
 # Check webhook status
 reference = "YOUR_REFERENCE"
 secret_key = "YOUR_SECRET_KEY"
 
 hook = Hook(reference, secret_key)
 status = hook.status()
```

### Comparing `pypstk-0.0.1/pypstk.egg-info/PKG-INFO` & `pypstk-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pypstk
-Version: 0.0.1
-Home-page: https://github.com/emekadefirst/Paystack-Python-2-SDK
-Author: Victor Chibuogwu Chukwuemeka aka Emekadefirst
-Author-email: emekadefirst@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LIcence
-Requires-Dist: requests>=2.26.0
-
 # Pystack
 
 This Python package provides a set of classes to interact with the Paystack API for handling transactions, customers, subscriptions, and webhooks.
 
 ## Installation
 
 To use this package, you need to have Python installed. You can install the package using pip:
@@ -24,34 +11,34 @@
 ```
 
 ## Usage
 
 ### 1. Payment
 
 ```python
-from payment import Pay
+from PythonPaystackv2.payment import Payment
 
-# Initialize payment
 email = "customer@email.com"
 amount = "20000"
-secret_key = "sk_test_6215942a0765956d18f05e4f52a12a6a8902cee2"
+secret_key = "your secret_key from api"
 
-new_payment = Pay(email, amount, secret_key)
+new_payment = Payment(email, amount, secret_key)
 transaction_data = new_payment.initialize_transaction()
 print(transaction_data)
 
 # Sample output:
-# {'status': True, 'message': 'Authorization URL created', 'data': {'authorization_url': 'https://checkout.paystack.com/1hxv7un'}}
+# {'references': '8pr6trcjj5', 'url': 'https://checkout.paystack.com/j62hay03a7dj6iu'}
+
 ```
 
 
 ### 3. Subscription
 
 ```python
-from subscription import Subscription
+from PythonPaystackv2.subscription import Subscription
 
 # Initialize subscription payment
 name = "Monthly Retainer"
 interval = "monthly"
 amount = 500000
 secret_key = "sk_test_daf386e7071c4613e54e4b71f43926409abd811e"
 
@@ -59,15 +46,15 @@
 pay_subscription.initialize_payment()
 pay_subscription.payment_status()
 ```
 
 ### 4. Webhook
 
 ```python
-from status import Verify
+from PythonPaystackv2.status import Verify
 
 # Check webhook status
 reference = "YOUR_REFERENCE"
 secret_key = "YOUR_SECRET_KEY"
 
 hook = Hook(reference, secret_key)
 status = hook.status()
```

### Comparing `pypstk-0.0.1/setup.py` & `pypstk-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="pypstk",
-    version="0.0.1",
+    version="0.1.0",
     long_description= description,
     long_description_content_type= "text/markdown",
     author="Victor Chibuogwu Chukwuemeka aka Emekadefirst",
     author_email="emekadefirst@gmail.com",
     url="https://github.com/emekadefirst/Paystack-Python-2-SDK",
     packages=find_packages(),
     install_requires=[
```

