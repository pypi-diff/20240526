# Comparing `tmp/panda3d-complexpbr-0.5.3.tar.gz` & `tmp/panda3d_complexpbr-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda3d-complexpbr-0.5.3.tar", last modified: Thu Oct 19 21:37:43 2023, max compression
+gzip compressed data, was "panda3d_complexpbr-0.5.4.tar", last modified: Sun May 26 01:08:31 2024, max compression
```

## Comparing `panda3d-complexpbr-0.5.3.tar` & `panda3d_complexpbr-0.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-10-19 21:37:43.141113 panda3d-complexpbr-0.5.3/
--rw-rw-rw-   0        0        0     1548 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/LICENSE
--rw-rw-rw-   0        0        0    11194 2023-10-19 21:37:43.140113 panda3d-complexpbr-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    10611 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-10-19 21:37:43.120571 panda3d-complexpbr-0.5.3/complexpbr/
--rw-rw-rw-   0        0        0     7207 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/__init__.py
--rw-rw-rw-   0        0        0     8542 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/brdf_lut_calculator.py
--rw-rw-rw-   0        0        0     8000 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/ibl_f.frag
--rw-rw-rw-   0        0        0     4256 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/ibl_v.vert
--rw-rw-rw-   0        0        0     8634 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/min_f.frag
--rw-rw-rw-   0        0        0      966 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/min_v.vert
--rw-rw-rw-   0        0        0    15263 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/output_brdf_lut.png
--rw-rw-rw-   0        0        0   282909 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/sample_output_brdf_lut.png
--rw-rw-rw-   0        0        0     1544 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/complexpbr/simplepbr_license.txt
-drwxrwxrwx   0        0        0        0 2023-10-19 21:37:43.138111 panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/
--rw-rw-rw-   0        0        0    11194 2023-10-19 21:37:43.000000 panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-10-19 21:37:43.000000 panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-19 21:37:43.000000 panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-10-19 21:37:43.000000 panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-19 21:37:43.000000 panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      773 2023-10-19 21:37:26.000000 panda3d-complexpbr-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-19 21:37:43.141113 panda3d-complexpbr-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-10-19 21:29:57.000000 panda3d-complexpbr-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:08:31.819052 panda3d_complexpbr-0.5.4/
+-rw-rw-rw-   0        0        0     1548 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0    11786 2024-05-26 01:08:31.818054 panda3d_complexpbr-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11203 2024-05-26 00:59:12.000000 panda3d_complexpbr-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 01:08:31.795581 panda3d_complexpbr-0.5.4/complexpbr/
+-rw-rw-rw-   0        0        0     7163 2024-05-26 00:07:49.000000 panda3d_complexpbr-0.5.4/complexpbr/__init__.py
+-rw-rw-rw-   0        0        0     8542 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/complexpbr/brdf_lut_calculator.py
+-rw-rw-rw-   0        0        0     8000 2024-04-22 02:33:51.000000 panda3d_complexpbr-0.5.4/complexpbr/ibl_f.frag
+-rw-rw-rw-   0        0        0     4256 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/complexpbr/ibl_v.vert
+-rw-rw-rw-   0        0        0     8634 2024-04-22 00:01:03.000000 panda3d_complexpbr-0.5.4/complexpbr/min_f.frag
+-rw-rw-rw-   0        0        0      966 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/complexpbr/min_v.vert
+-rw-rw-rw-   0        0        0    15263 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/complexpbr/output_brdf_lut.png
+-rw-rw-rw-   0        0        0   282909 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/complexpbr/sample_output_brdf_lut.png
+-rw-rw-rw-   0        0        0     1544 2024-04-22 00:00:09.000000 panda3d_complexpbr-0.5.4/complexpbr/simplepbr_license.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 01:08:31.816059 panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/
+-rw-rw-rw-   0        0        0    11786 2024-05-26 01:08:31.000000 panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2024-05-26 01:08:31.000000 panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 01:08:31.000000 panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-26 01:08:31.000000 panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 01:08:31.000000 panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      773 2024-05-26 00:43:05.000000 panda3d_complexpbr-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:08:31.820050 panda3d_complexpbr-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      210 2024-05-26 00:43:14.000000 panda3d_complexpbr-0.5.4/setup.py
```

### Comparing `panda3d-complexpbr-0.5.3/LICENSE` & `panda3d_complexpbr-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/PKG-INFO` & `panda3d_complexpbr-0.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-complexpbr
-Version: 0.5.3
+Version: 0.5.4
 Summary: Functional node level shader application for Panda3D
 Author: Logan Bier
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rayanalysis/panda3d-complexpbr
 Keywords: panda3d,gamedev,pbr
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -14,48 +14,44 @@
 License-File: LICENSE
 Requires-Dist: panda3d>=1.10.8
 Requires-Dist: typing_extensions~=4.7
 
 # panda3d-complexpbr
 Functional node level scene shader application for Panda3D. complexpbr supports realtime environment reflections for BSDF materials. These reflections are implemented with IBL (Image-based lighting) and PBR (Physically Based Rendering) forward shading constructs. Your machine must support GLSL version 430 or higher. Sample screenshots below.
 
-Featuring support for vertex displacement mapping, SSAO (Screen Space Ambient Occlusion), SSR (Screen Space Reflections), HSV color correction, Bloom, and Sobel based antialiasing in a screenspace kernel shader, which approximates temporal antialiasing. complexpbr.screenspace_init() automatically enables the AA, SSAO, SSR, and HSV color correction. To use the vertex displacement mapping, provide your displacement map as a shader input to your respective model node -- example below in the Usage section.
+Featuring support for vertex displacement mapping, SSAO (Screen Space Ambient Occlusion), HSV color correction, Bloom, and Sobel based antialiasing in a screenspace kernel shader, which approximates temporal antialiasing. complexpbr.screenspace_init() automatically enables the AA, SSAO, and HSV color correction. To use the vertex displacement mapping, provide your displacement map as a shader input to your respective model node -- example below in the Usage section.
 
 By default, the environment reflections dynamically track the camera view. You may set a custom position with the 'env_cam_pos' apply_shader() input variable to IE fix the view to a skybox somewhere on the scene graph. This env_cam_pos variable can be updated live afterwards by setting base.env_cam_pos = Vec3(some_pos). The option to disable or re-enable dynamic reflections is available. 
 
 As of version 0.5.2, complexpbr will default to a dummy BRDF LUT which it creates on the fly. complexpbr will remind you that you may create a custom BRDF LUT with the provided 'brdf_lut_calculator.py' script or copy the sample one provided. This feature is automatic, so if you provide the output_brdf_lut.png file in your program directory, it will default to that .png image ignoring the lut_fill input. The sample 'output_brdf_lut.png' and the creation script can be found in the panda3d-complexpbr git repo. For advanced users there is an option to set the LUT image RGB fill values via apply_shader(lut_fill=[r,g,b]) . See Usage section for an example of lut_fill.
 
 As of version 0.5.3, hardware skinning support is provided via complexpbr.skin(your_actor) for models with skeletal animations. See Usage section for an example of hardware skinning.
 
+As of version 0.5.4, panda3d-complexpbr may be considered mature and ready for production use. complexpbr will endeavor to continue supporting CommonFilters, which is still receiving some contemporary updates. complexpbr is still open to pull requests, feature requests, and so forth to continue expanding the filtering capabilities of screenspace_init() within reason.
+
 The goal of this project is to provide extremely easy to use scene shaders to expose the full functionality of Panda3D rendering, including interoperation with CommonFilters and setting shaders on a per-node basis.
 
 ![complexpbr_screen_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/a8a7d360-6b52-4fa8-91f8-31f052421043)
  
 ![complexpbr_reflections_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/d6d3867a-6dfb-4512-8a79-de80bf35bc26)
 
+10/30/23 Project Naer ([Project Naer complexpbr](https://github.com/rayanalysis/project-naer-complexpbr))
+
+![beige_screen_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/89428c83-5e6c-42d3-b30d-372e6ed8bd05)
+
+![silver_screen_1](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/478329ca-ba7c-4adf-b3a1-ae730bf54cc1)
+
 7/6/23 Lumberyard Bistro ([Amazon Lumberyard Bistro | NVIDIA Developer](https://developer.nvidia.com/orca/amazon-lumberyard-bistro))
 
 ![bistro_exterior_11](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/0cd476bb-d313-41f4-b5ea-d793589711e4)
 
 ![bistro_interior_5](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/ad75afa7-e1ef-41ea-aae9-4bb1cea54135)
 
 ![bistro_exterior_10](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/79df6bd6-14d8-4d19-ae5f-45c3418a7607)
 
-6/1/23 Sponza ([Intel GPU Research Samples](https://www.intel.com/content/www/us/en/developer/topic-technology/graphics-research/samples.html))
-
-![sponza_screen_1-Thu-Jun-01-08-16-18-2023-26](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/5d6a603f-9da1-49a1-affb-042658f343ed)
-
-![sponza_screen_1-Thu-Jun-01-08-17-47-2023-15](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7fffc0f4-75b3-476b-a328-127d231b9171)
-
-![sponza_screen_1-Thu-Jun-01-06-02-59-2023-22](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/913a5263-7750-47c1-b4c4-9f7dace84d6e)
-
-![sponza_screen_2-Thu-Jun-01-05-56-06-2023-591](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/b5055164-3235-48fa-86a7-0f6e3222b903)
-
-![sponza_screen_1-Fri-Jun-02-08-54-07-2023-428](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7a5c3f1f-1bb9-4dec-9e92-92dc52f77f29)
-
 ## Usage:
 ```python
 from direct.showbase.ShowBase import ShowBase
 import complexpbr
 
 class main(ShowBase):
     def __init__(self):
@@ -144,35 +140,45 @@
         # if complexpbr.screenspace_init() has not been called, you may use CommonFilters
         # scene_filters = CommonFilters(base.win, base.cam)
         # scene_filters.set_bloom(size='medium')
         # scene_filters.set_exposure_adjust(1.1)
         # scene_filters.set_gamma_adjust(1.1)
         # scene_filters.set_blur_sharpen(0.9)
 ```
-## Building:
+## Installing with PyPI:
+```bash
+pip install panda3d-complexpbr
+```
 
-The module may be built using setuptools. 
+## Building:
+The module may be built using build. 
 ```bash
-python3 setup.py bdist_wheel
+python -m build
 ```
 ```bash
-pip3 install 'path/to/panda3d-complexpbr.whl'
+pip install 'path/to/panda3d-complexpbr.whl'
 ```
-## Installing with PyPI:
-
-To-do.
-
-## Future Project Goals:
-- Function triggers for building new BRDF LUT samplers in realtime
-- Installation over pip
 
 ## Requirements:
 
 - panda3d
 
+
+6/1/23 Sponza ([Intel GPU Research Samples](https://www.intel.com/content/www/us/en/developer/topic-technology/graphics-research/samples.html))
+
+![sponza_screen_1-Thu-Jun-01-08-16-18-2023-26](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/5d6a603f-9da1-49a1-affb-042658f343ed)
+
+![sponza_screen_1-Thu-Jun-01-08-17-47-2023-15](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7fffc0f4-75b3-476b-a328-127d231b9171)
+
+![sponza_screen_1-Thu-Jun-01-06-02-59-2023-22](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/913a5263-7750-47c1-b4c4-9f7dace84d6e)
+
+![sponza_screen_2-Thu-Jun-01-05-56-06-2023-591](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/b5055164-3235-48fa-86a7-0f6e3222b903)
+
+![sponza_screen_1-Fri-Jun-02-08-54-07-2023-428](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7a5c3f1f-1bb9-4dec-9e92-92dc52f77f29)
+
 ![sponza_screen_1-Thu-Jun-01-05-39-29-2023-111](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/f366077b-b6d6-4c4a-896d-f456a06a53d1)
 
 ![sponza_screen_3-Thu-Jun-01-05-56-32-2023-657](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/23014163-4c7d-4a4d-9f6a-4b874ea364f2)
 
 ![sponza_screen_1-Thu-Jun-01-05-55-48-2023-540](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/ef2a71c3-169b-428c-a1a9-378c8906c644)
 
 ![sponza_screen_1-Thu-Jun-01-08-28-36-2023-104](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/4e40e642-f363-4328-bf99-4056f449e28a)
```

### Comparing `panda3d-complexpbr-0.5.3/README.md` & `panda3d_complexpbr-0.5.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # panda3d-complexpbr
 Functional node level scene shader application for Panda3D. complexpbr supports realtime environment reflections for BSDF materials. These reflections are implemented with IBL (Image-based lighting) and PBR (Physically Based Rendering) forward shading constructs. Your machine must support GLSL version 430 or higher. Sample screenshots below.
 
-Featuring support for vertex displacement mapping, SSAO (Screen Space Ambient Occlusion), SSR (Screen Space Reflections), HSV color correction, Bloom, and Sobel based antialiasing in a screenspace kernel shader, which approximates temporal antialiasing. complexpbr.screenspace_init() automatically enables the AA, SSAO, SSR, and HSV color correction. To use the vertex displacement mapping, provide your displacement map as a shader input to your respective model node -- example below in the Usage section.
+Featuring support for vertex displacement mapping, SSAO (Screen Space Ambient Occlusion), HSV color correction, Bloom, and Sobel based antialiasing in a screenspace kernel shader, which approximates temporal antialiasing. complexpbr.screenspace_init() automatically enables the AA, SSAO, and HSV color correction. To use the vertex displacement mapping, provide your displacement map as a shader input to your respective model node -- example below in the Usage section.
 
 By default, the environment reflections dynamically track the camera view. You may set a custom position with the 'env_cam_pos' apply_shader() input variable to IE fix the view to a skybox somewhere on the scene graph. This env_cam_pos variable can be updated live afterwards by setting base.env_cam_pos = Vec3(some_pos). The option to disable or re-enable dynamic reflections is available. 
 
 As of version 0.5.2, complexpbr will default to a dummy BRDF LUT which it creates on the fly. complexpbr will remind you that you may create a custom BRDF LUT with the provided 'brdf_lut_calculator.py' script or copy the sample one provided. This feature is automatic, so if you provide the output_brdf_lut.png file in your program directory, it will default to that .png image ignoring the lut_fill input. The sample 'output_brdf_lut.png' and the creation script can be found in the panda3d-complexpbr git repo. For advanced users there is an option to set the LUT image RGB fill values via apply_shader(lut_fill=[r,g,b]) . See Usage section for an example of lut_fill.
 
 As of version 0.5.3, hardware skinning support is provided via complexpbr.skin(your_actor) for models with skeletal animations. See Usage section for an example of hardware skinning.
 
+As of version 0.5.4, panda3d-complexpbr may be considered mature and ready for production use. complexpbr will endeavor to continue supporting CommonFilters, which is still receiving some contemporary updates. complexpbr is still open to pull requests, feature requests, and so forth to continue expanding the filtering capabilities of screenspace_init() within reason.
+
 The goal of this project is to provide extremely easy to use scene shaders to expose the full functionality of Panda3D rendering, including interoperation with CommonFilters and setting shaders on a per-node basis.
 
 ![complexpbr_screen_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/a8a7d360-6b52-4fa8-91f8-31f052421043)
  
 ![complexpbr_reflections_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/d6d3867a-6dfb-4512-8a79-de80bf35bc26)
 
+10/30/23 Project Naer ([Project Naer complexpbr](https://github.com/rayanalysis/project-naer-complexpbr))
+
+![beige_screen_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/89428c83-5e6c-42d3-b30d-372e6ed8bd05)
+
+![silver_screen_1](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/478329ca-ba7c-4adf-b3a1-ae730bf54cc1)
+
 7/6/23 Lumberyard Bistro ([Amazon Lumberyard Bistro | NVIDIA Developer](https://developer.nvidia.com/orca/amazon-lumberyard-bistro))
 
 ![bistro_exterior_11](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/0cd476bb-d313-41f4-b5ea-d793589711e4)
 
 ![bistro_interior_5](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/ad75afa7-e1ef-41ea-aae9-4bb1cea54135)
 
 ![bistro_exterior_10](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/79df6bd6-14d8-4d19-ae5f-45c3418a7607)
 
-6/1/23 Sponza ([Intel GPU Research Samples](https://www.intel.com/content/www/us/en/developer/topic-technology/graphics-research/samples.html))
-
-![sponza_screen_1-Thu-Jun-01-08-16-18-2023-26](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/5d6a603f-9da1-49a1-affb-042658f343ed)
-
-![sponza_screen_1-Thu-Jun-01-08-17-47-2023-15](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7fffc0f4-75b3-476b-a328-127d231b9171)
-
-![sponza_screen_1-Thu-Jun-01-06-02-59-2023-22](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/913a5263-7750-47c1-b4c4-9f7dace84d6e)
-
-![sponza_screen_2-Thu-Jun-01-05-56-06-2023-591](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/b5055164-3235-48fa-86a7-0f6e3222b903)
-
-![sponza_screen_1-Fri-Jun-02-08-54-07-2023-428](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7a5c3f1f-1bb9-4dec-9e92-92dc52f77f29)
-
 ## Usage:
 ```python
 from direct.showbase.ShowBase import ShowBase
 import complexpbr
 
 class main(ShowBase):
     def __init__(self):
@@ -127,35 +123,45 @@
         # if complexpbr.screenspace_init() has not been called, you may use CommonFilters
         # scene_filters = CommonFilters(base.win, base.cam)
         # scene_filters.set_bloom(size='medium')
         # scene_filters.set_exposure_adjust(1.1)
         # scene_filters.set_gamma_adjust(1.1)
         # scene_filters.set_blur_sharpen(0.9)
 ```
-## Building:
+## Installing with PyPI:
+```bash
+pip install panda3d-complexpbr
+```
 
-The module may be built using setuptools. 
+## Building:
+The module may be built using build. 
 ```bash
-python3 setup.py bdist_wheel
+python -m build
 ```
 ```bash
-pip3 install 'path/to/panda3d-complexpbr.whl'
+pip install 'path/to/panda3d-complexpbr.whl'
 ```
-## Installing with PyPI:
-
-To-do.
-
-## Future Project Goals:
-- Function triggers for building new BRDF LUT samplers in realtime
-- Installation over pip
 
 ## Requirements:
 
 - panda3d
 
+
+6/1/23 Sponza ([Intel GPU Research Samples](https://www.intel.com/content/www/us/en/developer/topic-technology/graphics-research/samples.html))
+
+![sponza_screen_1-Thu-Jun-01-08-16-18-2023-26](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/5d6a603f-9da1-49a1-affb-042658f343ed)
+
+![sponza_screen_1-Thu-Jun-01-08-17-47-2023-15](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7fffc0f4-75b3-476b-a328-127d231b9171)
+
+![sponza_screen_1-Thu-Jun-01-06-02-59-2023-22](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/913a5263-7750-47c1-b4c4-9f7dace84d6e)
+
+![sponza_screen_2-Thu-Jun-01-05-56-06-2023-591](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/b5055164-3235-48fa-86a7-0f6e3222b903)
+
+![sponza_screen_1-Fri-Jun-02-08-54-07-2023-428](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7a5c3f1f-1bb9-4dec-9e92-92dc52f77f29)
+
 ![sponza_screen_1-Thu-Jun-01-05-39-29-2023-111](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/f366077b-b6d6-4c4a-896d-f456a06a53d1)
 
 ![sponza_screen_3-Thu-Jun-01-05-56-32-2023-657](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/23014163-4c7d-4a4d-9f6a-4b874ea364f2)
 
 ![sponza_screen_1-Thu-Jun-01-05-55-48-2023-540](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/ef2a71c3-169b-428c-a1a9-378c8906c644)
 
 ![sponza_screen_1-Thu-Jun-01-08-28-36-2023-104](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/4e40e642-f363-4328-bf99-4056f449e28a)
```

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/brdf_lut_calculator.py` & `panda3d_complexpbr-0.5.4/complexpbr/brdf_lut_calculator.py`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/ibl_f.frag` & `panda3d_complexpbr-0.5.4/complexpbr/ibl_f.frag`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/ibl_v.vert` & `panda3d_complexpbr-0.5.4/complexpbr/ibl_v.vert`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/min_f.frag` & `panda3d_complexpbr-0.5.4/complexpbr/min_f.frag`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -272,18 +272,18 @@
     vec3 worldNormal = getViewNormal(tbn_tangent, tbn_bitangent, tbn_normal);
     vec3 viewNormal = transformNormalToViewSpace(worldNormal);
 
     SSRout ssrOut = screenSpaceReflection(texcoord, depth_fl, viewNormal);
     // blend the object color with the reflection color based on the intensity
     color = mix(color, ssrOut.color, max(ssrOut.intensity - reflection_threshold, 0.0));
 
-    vec3 hsvColor = rgb2hsv(color);
-    hsvColor *= vec3(hsv_r, hsv_g, hsv_b);
-    color = hsv2rgb(hsvColor);
-
     // apply SSAO to the final color
     float occlusion = ssao(texcoord, viewPos, viewNormal);
     color *= occlusion;
 
     o_color = vec4(bloomAA(color, texcoord), 1.0);
     // o_color = vec4(occlusion, 0, 0, 1.0);
+
+    vec3 hsvColor = rgb2hsv(color);
+    hsvColor *= vec3(hsv_r, hsv_g, hsv_b);
+    color = hsv2rgb(hsvColor);
 }
```

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/min_v.vert` & `panda3d_complexpbr-0.5.4/complexpbr/min_v.vert`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/output_brdf_lut.png` & `panda3d_complexpbr-0.5.4/complexpbr/output_brdf_lut.png`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/sample_output_brdf_lut.png` & `panda3d_complexpbr-0.5.4/complexpbr/sample_output_brdf_lut.png`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/complexpbr/simplepbr_license.txt` & `panda3d_complexpbr-0.5.4/complexpbr/simplepbr_license.txt`

 * *Files identical despite different names*

### Comparing `panda3d-complexpbr-0.5.3/panda3d_complexpbr.egg-info/PKG-INFO` & `panda3d_complexpbr-0.5.4/panda3d_complexpbr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda3d-complexpbr
-Version: 0.5.3
+Version: 0.5.4
 Summary: Functional node level shader application for Panda3D
 Author: Logan Bier
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/rayanalysis/panda3d-complexpbr
 Keywords: panda3d,gamedev,pbr
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -14,48 +14,44 @@
 License-File: LICENSE
 Requires-Dist: panda3d>=1.10.8
 Requires-Dist: typing_extensions~=4.7
 
 # panda3d-complexpbr
 Functional node level scene shader application for Panda3D. complexpbr supports realtime environment reflections for BSDF materials. These reflections are implemented with IBL (Image-based lighting) and PBR (Physically Based Rendering) forward shading constructs. Your machine must support GLSL version 430 or higher. Sample screenshots below.
 
-Featuring support for vertex displacement mapping, SSAO (Screen Space Ambient Occlusion), SSR (Screen Space Reflections), HSV color correction, Bloom, and Sobel based antialiasing in a screenspace kernel shader, which approximates temporal antialiasing. complexpbr.screenspace_init() automatically enables the AA, SSAO, SSR, and HSV color correction. To use the vertex displacement mapping, provide your displacement map as a shader input to your respective model node -- example below in the Usage section.
+Featuring support for vertex displacement mapping, SSAO (Screen Space Ambient Occlusion), HSV color correction, Bloom, and Sobel based antialiasing in a screenspace kernel shader, which approximates temporal antialiasing. complexpbr.screenspace_init() automatically enables the AA, SSAO, and HSV color correction. To use the vertex displacement mapping, provide your displacement map as a shader input to your respective model node -- example below in the Usage section.
 
 By default, the environment reflections dynamically track the camera view. You may set a custom position with the 'env_cam_pos' apply_shader() input variable to IE fix the view to a skybox somewhere on the scene graph. This env_cam_pos variable can be updated live afterwards by setting base.env_cam_pos = Vec3(some_pos). The option to disable or re-enable dynamic reflections is available. 
 
 As of version 0.5.2, complexpbr will default to a dummy BRDF LUT which it creates on the fly. complexpbr will remind you that you may create a custom BRDF LUT with the provided 'brdf_lut_calculator.py' script or copy the sample one provided. This feature is automatic, so if you provide the output_brdf_lut.png file in your program directory, it will default to that .png image ignoring the lut_fill input. The sample 'output_brdf_lut.png' and the creation script can be found in the panda3d-complexpbr git repo. For advanced users there is an option to set the LUT image RGB fill values via apply_shader(lut_fill=[r,g,b]) . See Usage section for an example of lut_fill.
 
 As of version 0.5.3, hardware skinning support is provided via complexpbr.skin(your_actor) for models with skeletal animations. See Usage section for an example of hardware skinning.
 
+As of version 0.5.4, panda3d-complexpbr may be considered mature and ready for production use. complexpbr will endeavor to continue supporting CommonFilters, which is still receiving some contemporary updates. complexpbr is still open to pull requests, feature requests, and so forth to continue expanding the filtering capabilities of screenspace_init() within reason.
+
 The goal of this project is to provide extremely easy to use scene shaders to expose the full functionality of Panda3D rendering, including interoperation with CommonFilters and setting shaders on a per-node basis.
 
 ![complexpbr_screen_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/a8a7d360-6b52-4fa8-91f8-31f052421043)
  
 ![complexpbr_reflections_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/d6d3867a-6dfb-4512-8a79-de80bf35bc26)
 
+10/30/23 Project Naer ([Project Naer complexpbr](https://github.com/rayanalysis/project-naer-complexpbr))
+
+![beige_screen_2](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/89428c83-5e6c-42d3-b30d-372e6ed8bd05)
+
+![silver_screen_1](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/478329ca-ba7c-4adf-b3a1-ae730bf54cc1)
+
 7/6/23 Lumberyard Bistro ([Amazon Lumberyard Bistro | NVIDIA Developer](https://developer.nvidia.com/orca/amazon-lumberyard-bistro))
 
 ![bistro_exterior_11](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/0cd476bb-d313-41f4-b5ea-d793589711e4)
 
 ![bistro_interior_5](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/ad75afa7-e1ef-41ea-aae9-4bb1cea54135)
 
 ![bistro_exterior_10](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/79df6bd6-14d8-4d19-ae5f-45c3418a7607)
 
-6/1/23 Sponza ([Intel GPU Research Samples](https://www.intel.com/content/www/us/en/developer/topic-technology/graphics-research/samples.html))
-
-![sponza_screen_1-Thu-Jun-01-08-16-18-2023-26](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/5d6a603f-9da1-49a1-affb-042658f343ed)
-
-![sponza_screen_1-Thu-Jun-01-08-17-47-2023-15](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7fffc0f4-75b3-476b-a328-127d231b9171)
-
-![sponza_screen_1-Thu-Jun-01-06-02-59-2023-22](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/913a5263-7750-47c1-b4c4-9f7dace84d6e)
-
-![sponza_screen_2-Thu-Jun-01-05-56-06-2023-591](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/b5055164-3235-48fa-86a7-0f6e3222b903)
-
-![sponza_screen_1-Fri-Jun-02-08-54-07-2023-428](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7a5c3f1f-1bb9-4dec-9e92-92dc52f77f29)
-
 ## Usage:
 ```python
 from direct.showbase.ShowBase import ShowBase
 import complexpbr
 
 class main(ShowBase):
     def __init__(self):
@@ -144,35 +140,45 @@
         # if complexpbr.screenspace_init() has not been called, you may use CommonFilters
         # scene_filters = CommonFilters(base.win, base.cam)
         # scene_filters.set_bloom(size='medium')
         # scene_filters.set_exposure_adjust(1.1)
         # scene_filters.set_gamma_adjust(1.1)
         # scene_filters.set_blur_sharpen(0.9)
 ```
-## Building:
+## Installing with PyPI:
+```bash
+pip install panda3d-complexpbr
+```
 
-The module may be built using setuptools. 
+## Building:
+The module may be built using build. 
 ```bash
-python3 setup.py bdist_wheel
+python -m build
 ```
 ```bash
-pip3 install 'path/to/panda3d-complexpbr.whl'
+pip install 'path/to/panda3d-complexpbr.whl'
 ```
-## Installing with PyPI:
-
-To-do.
-
-## Future Project Goals:
-- Function triggers for building new BRDF LUT samplers in realtime
-- Installation over pip
 
 ## Requirements:
 
 - panda3d
 
+
+6/1/23 Sponza ([Intel GPU Research Samples](https://www.intel.com/content/www/us/en/developer/topic-technology/graphics-research/samples.html))
+
+![sponza_screen_1-Thu-Jun-01-08-16-18-2023-26](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/5d6a603f-9da1-49a1-affb-042658f343ed)
+
+![sponza_screen_1-Thu-Jun-01-08-17-47-2023-15](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7fffc0f4-75b3-476b-a328-127d231b9171)
+
+![sponza_screen_1-Thu-Jun-01-06-02-59-2023-22](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/913a5263-7750-47c1-b4c4-9f7dace84d6e)
+
+![sponza_screen_2-Thu-Jun-01-05-56-06-2023-591](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/b5055164-3235-48fa-86a7-0f6e3222b903)
+
+![sponza_screen_1-Fri-Jun-02-08-54-07-2023-428](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/7a5c3f1f-1bb9-4dec-9e92-92dc52f77f29)
+
 ![sponza_screen_1-Thu-Jun-01-05-39-29-2023-111](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/f366077b-b6d6-4c4a-896d-f456a06a53d1)
 
 ![sponza_screen_3-Thu-Jun-01-05-56-32-2023-657](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/23014163-4c7d-4a4d-9f6a-4b874ea364f2)
 
 ![sponza_screen_1-Thu-Jun-01-05-55-48-2023-540](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/ef2a71c3-169b-428c-a1a9-378c8906c644)
 
 ![sponza_screen_1-Thu-Jun-01-08-28-36-2023-104](https://github.com/rayanalysis/panda3d-complexpbr/assets/3117958/4e40e642-f363-4328-bf99-4056f449e28a)
```

### Comparing `panda3d-complexpbr-0.5.3/pyproject.toml` & `panda3d_complexpbr-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools >= 61",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.5.3"
+version = "0.5.4"
 name = "panda3d-complexpbr"
 authors = [
     {name = "Logan Bier"}
 ]
 description = "Functional node level shader application for Panda3D"
 readme = "README.md"
 keywords = ["panda3d", "gamedev", "pbr"]
```

