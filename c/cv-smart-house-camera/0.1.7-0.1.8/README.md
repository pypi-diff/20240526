# Comparing `tmp/cv_smart_house_camera-0.1.7.tar.gz` & `tmp/cv_smart_house_camera-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv_smart_house_camera-0.1.7.tar", max compression
+gzip compressed data, was "cv_smart_house_camera-0.1.8.tar", max compression
```

## Comparing `cv_smart_house_camera-0.1.7.tar` & `cv_smart_house_camera-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      244 2024-05-24 09:03:04.476722 cv_smart_house_camera-0.1.7/cv_smart_house_camera/__init__.py
--rw-r--r--   0        0        0     1221 2024-05-24 19:00:17.717430 cv_smart_house_camera-0.1.7/cv_smart_house_camera/cam_capture.py
--rw-r--r--   0        0        0       91 2024-05-24 08:38:56.068779 cv_smart_house_camera-0.1.7/cv_smart_house_camera/constants.py
--rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.7/cv_smart_house_camera/data/frames.py
--rw-r--r--   0        0        0      976 2024-05-24 09:01:56.589663 cv_smart_house_camera-0.1.7/cv_smart_house_camera/generate_code.py
--rw-r--r--   0        0        0      362 2024-05-26 08:13:23.539904 cv_smart_house_camera-0.1.7/cv_smart_house_camera/helpers/poetry_install.py
--rw-r--r--   0        0        0      271 2024-05-24 09:08:20.156939 cv_smart_house_camera-0.1.7/cv_smart_house_camera/main.py
--rw-r--r--   0        0        0      778 2024-05-24 08:39:21.579651 cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_list.py
--rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_processing.py
--rw-r--r--   0        0        0     3543 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_pb2.py
--rw-r--r--   0        0        0     5512 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_twirp.py
--rw-r--r--   0        0        0     4697 2024-05-24 09:22:47.376868 cv_smart_house_camera-0.1.7/cv_smart_house_camera/server.py
--rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.7/cv_smart_house_camera/utils/get_local_ip.py
--rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.7/cv_smart_house_camera/utils/get_modules_from_toml.py
--rw-r--r--   0        0        0      620 2024-05-26 08:14:20.230102 cv_smart_house_camera-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.7/README.md
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      244 2024-05-24 09:03:04.476722 cv_smart_house_camera-0.1.8/cv_smart_house_camera/__init__.py
+-rw-r--r--   0        0        0     1221 2024-05-24 19:00:17.717430 cv_smart_house_camera-0.1.8/cv_smart_house_camera/cam_capture.py
+-rw-r--r--   0        0        0       91 2024-05-24 08:38:56.068779 cv_smart_house_camera-0.1.8/cv_smart_house_camera/constants.py
+-rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.8/cv_smart_house_camera/data/frames.py
+-rw-r--r--   0        0        0      976 2024-05-24 09:01:56.589663 cv_smart_house_camera-0.1.8/cv_smart_house_camera/generate_code.py
+-rw-r--r--   0        0        0      362 2024-05-26 08:13:23.539904 cv_smart_house_camera-0.1.8/cv_smart_house_camera/helpers/poetry_install.py
+-rw-r--r--   0        0        0      271 2024-05-24 09:08:20.156939 cv_smart_house_camera-0.1.8/cv_smart_house_camera/main.py
+-rw-r--r--   0        0        0      778 2024-05-24 08:39:21.579651 cv_smart_house_camera-0.1.8/cv_smart_house_camera/modules/modules_list.py
+-rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.8/cv_smart_house_camera/modules/modules_processing.py
+-rw-r--r--   0        0        0     3543 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.8/cv_smart_house_camera/proto_services/camera_service_pb2.py
+-rw-r--r--   0        0        0     5512 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.8/cv_smart_house_camera/proto_services/camera_service_twirp.py
+-rw-r--r--   0        0        0     4697 2024-05-24 09:22:47.376868 cv_smart_house_camera-0.1.8/cv_smart_house_camera/server.py
+-rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.8/cv_smart_house_camera/utils/get_local_ip.py
+-rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.8/cv_smart_house_camera/utils/get_modules_from_toml.py
+-rw-r--r--   0        0        0      620 2024-05-26 08:23:45.228964 cv_smart_house_camera-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.8/README.md
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.8/PKG-INFO
```

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/cam_capture.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/cam_capture.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/generate_code.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/generate_code.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_list.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/modules/modules_list.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_processing.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/modules/modules_processing.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_pb2.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/proto_services/camera_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_twirp.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/proto_services/camera_service_twirp.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/server.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/server.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/cv_smart_house_camera/utils/get_modules_from_toml.py` & `cv_smart_house_camera-0.1.8/cv_smart_house_camera/utils/get_modules_from_toml.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.7/pyproject.toml` & `cv_smart_house_camera-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cv-smart-house-camera"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = [ "Your Name <you@example.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 toml = "^0.10.2"
 opencv-python = "^4.9.0.80"
 twirp = "^0.0.7"
 uvicorn = "^0.29.0"
 starlette = "^0.37.2"
 aiohttp = "^3.9.5"
```

