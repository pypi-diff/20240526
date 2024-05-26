# Comparing `tmp/cv_smart_house_camera-0.1.6.tar.gz` & `tmp/cv_smart_house_camera-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cv_smart_house_camera-0.1.6.tar", max compression
+gzip compressed data, was "cv_smart_house_camera-0.1.7.tar", max compression
```

## Comparing `cv_smart_house_camera-0.1.6.tar` & `cv_smart_house_camera-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      244 2024-05-24 09:03:04.476722 cv_smart_house_camera-0.1.6/cv_smart_house_camera/__init__.py
--rw-r--r--   0        0        0      733 2024-05-20 13:14:13.260707 cv_smart_house_camera-0.1.6/cv_smart_house_camera/cam_capture.py
--rw-r--r--   0        0        0       91 2024-05-24 08:38:56.068779 cv_smart_house_camera-0.1.6/cv_smart_house_camera/constants.py
--rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.6/cv_smart_house_camera/data/frames.py
--rw-r--r--   0        0        0      976 2024-05-24 09:01:56.589663 cv_smart_house_camera-0.1.6/cv_smart_house_camera/generate_code.py
--rw-r--r--   0        0        0      347 2024-05-24 09:19:21.154139 cv_smart_house_camera-0.1.6/cv_smart_house_camera/helpers/poetry_install.py
--rw-r--r--   0        0        0      271 2024-05-24 09:08:20.156939 cv_smart_house_camera-0.1.6/cv_smart_house_camera/main.py
--rw-r--r--   0        0        0      778 2024-05-24 08:39:21.579651 cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_list.py
--rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_processing.py
--rw-r--r--   0        0        0     3543 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_pb2.py
--rw-r--r--   0        0        0     5512 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_twirp.py
--rw-r--r--   0        0        0     4697 2024-05-24 09:22:47.376868 cv_smart_house_camera-0.1.6/cv_smart_house_camera/server.py
--rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.6/cv_smart_house_camera/utils/get_local_ip.py
--rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.6/cv_smart_house_camera/utils/get_modules_from_toml.py
--rw-r--r--   0        0        0      660 2024-05-24 09:24:09.524311 cv_smart_house_camera-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.6/README.md
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      244 2024-05-24 09:03:04.476722 cv_smart_house_camera-0.1.7/cv_smart_house_camera/__init__.py
+-rw-r--r--   0        0        0     1221 2024-05-24 19:00:17.717430 cv_smart_house_camera-0.1.7/cv_smart_house_camera/cam_capture.py
+-rw-r--r--   0        0        0       91 2024-05-24 08:38:56.068779 cv_smart_house_camera-0.1.7/cv_smart_house_camera/constants.py
+-rw-r--r--   0        0        0       85 2024-05-18 16:24:24.102931 cv_smart_house_camera-0.1.7/cv_smart_house_camera/data/frames.py
+-rw-r--r--   0        0        0      976 2024-05-24 09:01:56.589663 cv_smart_house_camera-0.1.7/cv_smart_house_camera/generate_code.py
+-rw-r--r--   0        0        0      362 2024-05-26 08:13:23.539904 cv_smart_house_camera-0.1.7/cv_smart_house_camera/helpers/poetry_install.py
+-rw-r--r--   0        0        0      271 2024-05-24 09:08:20.156939 cv_smart_house_camera-0.1.7/cv_smart_house_camera/main.py
+-rw-r--r--   0        0        0      778 2024-05-24 08:39:21.579651 cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_list.py
+-rw-r--r--   0        0        0     1771 2024-05-20 17:54:20.117074 cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_processing.py
+-rw-r--r--   0        0        0     3543 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_pb2.py
+-rw-r--r--   0        0        0     5512 2024-05-24 08:47:27.279619 cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_twirp.py
+-rw-r--r--   0        0        0     4697 2024-05-24 09:22:47.376868 cv_smart_house_camera-0.1.7/cv_smart_house_camera/server.py
+-rw-r--r--   0        0        0      141 2024-05-19 14:26:26.476002 cv_smart_house_camera-0.1.7/cv_smart_house_camera/utils/get_local_ip.py
+-rw-r--r--   0        0        0      515 2024-05-20 12:20:23.424894 cv_smart_house_camera-0.1.7/cv_smart_house_camera/utils/get_modules_from_toml.py
+-rw-r--r--   0        0        0      620 2024-05-26 08:14:20.230102 cv_smart_house_camera-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 13:48:56.985064 cv_smart_house_camera-0.1.7/README.md
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 cv_smart_house_camera-0.1.7/PKG-INFO
```

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/generate_code.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/generate_code.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_list.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_list.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/modules/modules_processing.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/modules/modules_processing.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_pb2.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/proto_services/camera_service_twirp.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/proto_services/camera_service_twirp.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/server.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/server.py`

 * *Files identical despite different names*

### Comparing `cv_smart_house_camera-0.1.6/cv_smart_house_camera/utils/get_modules_from_toml.py` & `cv_smart_house_camera-0.1.7/cv_smart_house_camera/utils/get_modules_from_toml.py`

 * *Files identical despite different names*

