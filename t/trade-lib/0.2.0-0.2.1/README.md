# Comparing `tmp/trade_lib-0.2.0.tar.gz` & `tmp/trade_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trade_lib-0.2.0.tar", max compression
+gzip compressed data, was "trade_lib-0.2.1.tar", max compression
```

## Comparing `trade_lib-0.2.0.tar` & `trade_lib-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      432 2023-02-08 04:07:13.086440 trade_lib-0.2.0/README.md
--rw-r--r--   0        0        0      364 2023-02-12 00:50:17.046140 trade_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      114 2023-02-08 04:07:13.087323 trade_lib-0.2.0/trade_lib/__init__.py
--rw-r--r--   0        0        0     4835 2022-12-03 14:50:00.368519 trade_lib-0.2.0/trade_lib/message.py
--rw-r--r--   0        0        0     2533 2022-12-03 14:45:34.387874 trade_lib-0.2.0/trade_lib/util.py
--rwxr-xr-x   0        0        0     6773 2022-12-03 14:44:55.951887 trade_lib-0.2.0/trade_lib/weixin.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 trade_lib-0.2.0/setup.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 trade_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      603 2024-04-01 12:29:31.912264 trade_lib-0.2.1/README.md
+-rw-r--r--   0        0        0      364 2024-05-26 05:20:52.123136 trade_lib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-04-01 12:29:31.912647 trade_lib-0.2.1/trade_lib/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-01 12:29:31.912949 trade_lib-0.2.1/trade_lib/message.py
+-rw-r--r--   0        0        0     3668 2024-04-01 12:29:31.913114 trade_lib-0.2.1/trade_lib/util.py
+-rw-r--r--   0        0        0      700 2024-04-01 12:29:31.913233 trade_lib-0.2.1/trade_lib/venus.py
+-rwxr-xr-x   0        0        0     6773 2024-04-01 12:29:31.913518 trade_lib-0.2.1/trade_lib/weixin.py
+-rw-r--r--   0        0        0     1288 1970-01-01 00:00:00.000000 trade_lib-0.2.1/setup.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 trade_lib-0.2.1/PKG-INFO
```

### Comparing `trade_lib-0.2.0/trade_lib/message.py` & `trade_lib-0.2.1/trade_lib/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,14 +118,14 @@
                 print('成功发送企业微信')
     except Exception as e:
         print(f"发送企业微信失败:{e}")
         print(traceback.format_exc())
 
 # async def main():
 #     message_instance = Message(MessageMethod.DINGDING, {
-#         'robot_id': 'e02d79d08f29878bf1351299091143cf781488dd58301ed8dde74e4ee9d9d91a',
-#         'secret': 'SEC4efd80819c5ecfefa93adcd214478292724b1a7558d2d2c1eca73afdd1eb8419'
+#         'robot_id': 'e02d79d08............1ed8dde74e4ee9d9d91a',
+#         'secret': 'SEC4efd8.............1eca73afdd1eb8419'
 #     })
 #     await message_instance.send('哈哈哈')
 #
 # if __name__ == '__main__':
 #     asyncio.run(main())
```

### Comparing `trade_lib-0.2.0/trade_lib/weixin.py` & `trade_lib-0.2.1/trade_lib/weixin.py`

 * *Files identical despite different names*

### Comparing `trade_lib-0.2.0/setup.py` & `trade_lib-0.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0', 'aiohttp>=3.8.3,<4.0.0', 'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'trade-lib',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '我的交易库',
-    'long_description': "# trade-lib\n自己的交易常用库\n\n```\npip install trade-lib\n```\n\n## 使用\n\n```python\n\nimport trade_lib\n\n# load exchange config from ~/.config/exchange.yaml\nconfig = trade_lib.get_exchange_config(exname)\n\n# set_dingding\ndingding_config = {'robot_id':'', 'secret':''}\ntrade_lib.set_dingding(dingding_config)\ntrade_lib.dinding_send('ding...')\n```\n\n## upload to pypi\n\n```\npython3 setup.py sdist bdist_wheel\n\ntwine upload dist/*\n```",
+    'long_description': "# trade-lib\n自己的交易常用库\n\n```\npip install trade-lib\n```\n\n## 使用\n\n```python\n\nimport trade_lib\n\n# load exchange config from ~/.config/exchange.yaml\nconfig = trade_lib.get_exchange_config(exname)\n\n# set_dingding\ndingding_config = {'robot_id':'', 'secret':''}\ntrade_lib.set_dingding(dingding_config)\ntrade_lib.dinding_send('ding...')\n```\n\n## upload to pypi\n\n```\npython3 setup.py sdist bdist_wheel\n\ntwine upload dist/*\n```\n\n\n## api\n\n1、 取 venus.io 上的借贷利率\n```python\nfrom trade_lib.venus import get_apy\n\nsupply_apy, borrow_apy = get_apy('BNB')\nprint(supply_apy, borrow_apy)\n\n```\n\n",
     'author': 'oscar',
     'author_email': 'oscnet@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `trade_lib-0.2.0/PKG-INFO` & `trade_lib-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: trade-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: 我的交易库
 Author: oscar
 Author-email: oscnet@163.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
@@ -39,7 +41,21 @@
 ## upload to pypi
 
 ```
 python3 setup.py sdist bdist_wheel
 
 twine upload dist/*
 ```
+
+
+## api
+
+1、 取 venus.io 上的借贷利率
+```python
+from trade_lib.venus import get_apy
+
+supply_apy, borrow_apy = get_apy('BNB')
+print(supply_apy, borrow_apy)
+
+```
+
+
```

