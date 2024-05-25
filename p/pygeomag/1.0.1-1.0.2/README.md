# Comparing `tmp/pygeomag-1.0.1.tar.gz` & `tmp/pygeomag-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeomag-1.0.1.tar", last modified: Thu Oct  5 23:00:46 2023, max compression
+gzip compressed data, was "pygeomag-1.0.2.tar", last modified: Sat May 25 22:23:43 2024, max compression
```

## Comparing `pygeomag-1.0.1.tar` & `pygeomag-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 justin    (1000) justin    (1000)        0 2023-10-05 23:00:46.185655 pygeomag-1.0.1/
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1069 2023-10-05 22:41:03.000000 pygeomag-1.0.1/LICENSE
--rwxrwxrwx   0 justin    (1000) justin    (1000)       52 2023-10-05 22:41:03.000000 pygeomag-1.0.1/MANIFEST.in
--rwxrwxrwx   0 justin    (1000) justin    (1000)     5985 2023-10-05 23:00:46.154403 pygeomag-1.0.1/PKG-INFO
--rwxrwxrwx   0 justin    (1000) justin    (1000)     5457 2023-10-05 22:41:03.000000 pygeomag-1.0.1/README.rst
-drwxrwxrwx   0 justin    (1000) justin    (1000)        0 2023-10-05 23:00:45.181122 pygeomag-1.0.1/pygeomag/
--rwxrwxrwx   0 justin    (1000) justin    (1000)      558 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/__init__.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     5189 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/format.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)    22914 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/geomag.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     2821 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/time.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)       22 2023-10-05 22:59:40.000000 pygeomag-1.0.1/pygeomag/util.py
-drwxrwxrwx   0 justin    (1000) justin    (1000)        0 2023-10-05 23:00:46.115614 pygeomag-1.0.1/pygeomag/wmm/
--rwxrwxrwx   0 justin    (1000) justin    (1000)     4557 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/WMM.COF
--rwxrwxrwx   0 justin    (1000) justin    (1000)     4557 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/WMM_2010.COF
--rwxrwxrwx   0 justin    (1000) justin    (1000)     4557 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/WMM_2015.COF
--rwxrwxrwx   0 justin    (1000) justin    (1000)     4557 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/WMM_2015v2.COF
--rwxrwxrwx   0 justin    (1000) justin    (1000)     3641 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/wmm_2010.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     3616 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/wmm_2015.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     3649 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/wmm_2015v2.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     3646 2023-10-05 22:41:03.000000 pygeomag-1.0.1/pygeomag/wmm/wmm_2020.py
-drwxrwxrwx   0 justin    (1000) justin    (1000)        0 2023-10-05 23:00:45.440580 pygeomag-1.0.1/pygeomag.egg-info/
--rwxrwxrwx   0 justin    (1000) justin    (1000)     5985 2023-10-05 23:00:44.000000 pygeomag-1.0.1/pygeomag.egg-info/PKG-INFO
--rwxrwxrwx   0 justin    (1000) justin    (1000)      469 2023-10-05 23:00:44.000000 pygeomag-1.0.1/pygeomag.egg-info/SOURCES.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)        1 2023-10-05 23:00:44.000000 pygeomag-1.0.1/pygeomag.egg-info/dependency_links.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)        9 2023-10-05 23:00:44.000000 pygeomag-1.0.1/pygeomag.egg-info/top_level.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)      834 2023-10-05 22:59:40.000000 pygeomag-1.0.1/pyproject.toml
--rwxrwxrwx   0 justin    (1000) justin    (1000)       38 2023-10-05 23:00:46.185655 pygeomag-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 22:23:43.545416 pygeomag-1.0.2/
+-rw-rw-rw-   0        0        0     1069 2024-05-25 21:15:40.000000 pygeomag-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-05-25 21:15:40.000000 pygeomag-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6179 2024-05-25 22:23:43.544394 pygeomag-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5516 2024-05-25 21:55:32.000000 pygeomag-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-25 22:23:43.530861 pygeomag-1.0.2/pygeomag/
+-rw-rw-rw-   0        0        0      558 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/__init__.py
+-rw-rw-rw-   0        0        0     5204 2024-05-25 21:24:31.000000 pygeomag-1.0.2/pygeomag/format.py
+-rw-rw-rw-   0        0        0    23681 2024-05-25 21:24:31.000000 pygeomag-1.0.2/pygeomag/geomag.py
+-rw-rw-rw-   0        0        0     2856 2024-05-25 21:24:31.000000 pygeomag-1.0.2/pygeomag/time.py
+-rw-rw-rw-   0        0        0       22 2024-05-25 22:23:16.000000 pygeomag-1.0.2/pygeomag/util.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:23:43.543394 pygeomag-1.0.2/pygeomag/wmm/
+-rw-rw-rw-   0        0        0     4557 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/WMM.COF
+-rw-rw-rw-   0        0        0     4557 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/WMM_2010.COF
+-rw-rw-rw-   0        0        0     4557 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/WMM_2015.COF
+-rw-rw-rw-   0        0        0     4557 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/WMM_2015v2.COF
+-rw-rw-rw-   0        0        0     3641 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/wmm_2010.py
+-rw-rw-rw-   0        0        0     3616 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/wmm_2015.py
+-rw-rw-rw-   0        0        0     3649 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/wmm_2015v2.py
+-rw-rw-rw-   0        0        0     3646 2024-05-25 21:15:40.000000 pygeomag-1.0.2/pygeomag/wmm/wmm_2020.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:23:43.544394 pygeomag-1.0.2/pygeomag.egg-info/
+-rw-rw-rw-   0        0        0     6179 2024-05-25 22:23:43.000000 pygeomag-1.0.2/pygeomag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2024-05-25 22:23:43.000000 pygeomag-1.0.2/pygeomag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 22:23:43.000000 pygeomag-1.0.2/pygeomag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 22:23:43.000000 pygeomag-1.0.2/pygeomag.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1011 2024-05-25 21:24:31.000000 pygeomag-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 22:23:43.545416 pygeomag-1.0.2/setup.cfg
```

### Comparing `pygeomag-1.0.1/LICENSE` & `pygeomag-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/PKG-INFO` & `pygeomag-1.0.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pygeomag
-Version: 1.0.1
-Summary: A python port of the World Magnetic Model (WMM)
-Author: Justin Myers
-Project-URL: Homepage, https://github.com/boxpet/pygeomag
-Project-URL: Bug Tracker, https://github.com/boxpet/pygeomag/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Welcome to pyGeoMag's documentation!
 ====================================
 
 .. image:: https://dl.circleci.com/status-badge/img/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main.svg?style=svg&circle-token=13df862914431a3f89a9bc1bcc8bb5b2a177d815
    :target: https://dl.circleci.com/status-badge/redirect/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main
    :alt: CircleCI
 .. image:: https://codecov.io/gh/boxpet/pygeomag/graph/badge.svg?token=ECHON65OG8
@@ -27,17 +12,18 @@
    :alt: PyPI
 .. image:: https://readthedocs.org/projects/pygeomag/badge/?version=latest
    :target: https://pygeomag.readthedocs.io/
    :alt: Documentation Status
 .. image:: https://img.shields.io/github/license/boxpet/pygeomag.svg
    :target: https://github.com/boxpet/pygeomag/blob/main/LICENSE
    :alt: License: MIT
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Code Style: Ruff
+
 
 **What is declination?**
 
 Declination is the angle that adjusts a compass reading from Magnetic North to True North. Many
 maps will show it in the legend, so you can adjust your compass (either physically or mentally).
 
 **Why do you need this?**
```

### Comparing `pygeomag-1.0.1/README.rst` & `pygeomag-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,135 @@
-Welcome to pyGeoMag's documentation!
-====================================
-
-.. image:: https://dl.circleci.com/status-badge/img/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main.svg?style=svg&circle-token=13df862914431a3f89a9bc1bcc8bb5b2a177d815
-   :target: https://dl.circleci.com/status-badge/redirect/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main
-   :alt: CircleCI
-.. image:: https://codecov.io/gh/boxpet/pygeomag/graph/badge.svg?token=ECHON65OG8
-   :target: https://codecov.io/gh/boxpet/pygeomag
-   :alt: codecov
-.. image:: https://img.shields.io/pypi/v/pygeomag
-   :target: https://pypi.org/project/pygeomag/
-   :alt: PyPI
-.. image:: https://readthedocs.org/projects/pygeomag/badge/?version=latest
-   :target: https://pygeomag.readthedocs.io/
-   :alt: Documentation Status
-.. image:: https://img.shields.io/github/license/boxpet/pygeomag.svg
-   :target: https://github.com/boxpet/pygeomag/blob/main/LICENSE
-   :alt: License: MIT
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
-**What is declination?**
-
-Declination is the angle that adjusts a compass reading from Magnetic North to True North. Many
-maps will show it in the legend, so you can adjust your compass (either physically or mentally).
-
-**Why do you need this?**
-
-In Washington State, the declination angle is between 14° and 16° West depending on your location. Meaning if I just
-pull out my compass and head North, I'm really heading at about 15°. And now if I walk 500 feet on that course, I'll be
-about 130 feet to the East of where I wanted to be.
-
-Now say I'm building a device that includes a magnetometer. I get it all calibrated to point to Magnetic North, show
-this value on the device and now the user is pointing in the wrong direction. And of course, the values change yearly.
-In the last 10 years, it's dropped just over a full degree in the Greater Seattle area. Here is where pyGeoMag comes in.
-
-To help see how much the magnetic field changes as you travel across the globe, here is projection for 2020 from
-NOAA:
-
-.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Main%20Field-%20Annual%20Change%20Declination%20%28D%29.jpg
-   :alt: US/UK World Magnetic Model - Epoch 2020.0: Main Field Declination
-
-To see how much the value changes per year (The contour interval is 2 arcminutes/year):
-
-.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Secular%20Variation-%20Annual%20Change%20Declination%20%28D%29.jpg
-   :alt: US/UK World Magnetic Model - Epoch 2020.0: Annual Change Declination
-
-If you want to look up these values, you can use NOAA's
-`Magnetic Field Caculators <https://www.ngdc.noaa.gov/geomag/calculators/magcalc.shtml>`_ in a browser or install their
-**CrowdMag** app on your `Android <https://play.google.com/store/apps/details?id=gov.noaa.ngdc.wmm2>`_ or
-`iOS <https://itunes.apple.com/app/id910578825>`_ device.
-
-**pyGeoMag** is an implementation written in Python of the
-`World Magnetic Model (WMM) <https://www.ncei.noaa.gov/products/world-magnetic-model>`_, specifically to be used in
-lightweight versions (like MicroPython and CircuitPython).
-
-**From NOAA**
-
-   The World Magnetic Model (WMM) is the standard model for navigation, attitude, and heading referencing systems using
-   the geomagnetic field. Additional WMM uses include civilian applications, including navigation and heading systems.
-
-   The model is a joint product of the United States' National Geospatial-Intelligence Agency (NGA) and the United
-   Kingdom's Defence Geographic Centre (DGC). NCEI and the British Geological Survey (BGS) jointly developed the WMM.
-   The U.S. Department of Defense, the U.K. Ministry of Defence, the North Atlantic Treaty Organization (NATO), and the
-   International Hydrographic Organization (IHO) use the WMM.
-
-Installation
-------------
-
-Install using `pip <http://www.pip-installer.org/en/latest>`_ with:
-
-.. code-block:: shell
-
-   pip install pygeomag
-
-Example
--------
-
-Calculate the geomagnetic declination at the Space Needle in Seattle, WA:
-
-.. code-block:: pycon
-
-   >>> from pygeomag import GeoMag
-   >>> geo_mag = GeoMag()
-   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2023.75)
-   >>> print(result.d)
-   15.25942260585284
-
-And calculate it for the same spot 10 years ago:
-
-.. code-block:: pycon
-
-   >>> from pygeomag import GeoMag
-   >>> geo_mag = GeoMag(coefficients_file='wmm/WMM_2010.COF')
-   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2013.75)
-   >>> print(result.d)
-   16.32554283003356
-
-Validation
-----------
-
-All test values from the official NOAA WMM documentation are tested here for WMM-2020, WMM-2015v2, WMM-2015 and
-WMM-2010.
-
-Notes
------
-
-This is a direct port from the Legacy C code provided by NOAA. It defaults to using the WMM-2020 Coefficient file
-(WMM.COF) valid for 2020.0 - 2025.0. The code is specifically not 100% pythonic in order to make adding updates simple
-(for example uppercase variable names).
-
-At this point Annual change also known as Secular Variation is not in this package the Legacy C version does a direct
-``year+1.value - year2.value`` and both the test values and other existing code bases do something different.
-
-Documentation
--------------
-
-More documentation and examples can be found at `Read the Docs <http://pygeomag.readthedocs.io/>`_.
+Metadata-Version: 2.1
+Name: pygeomag
+Version: 1.0.2
+Summary: A python port of the World Magnetic Model (WMM)
+Author: Justin Myers
+Project-URL: Homepage, https://github.com/boxpet/pygeomag
+Project-URL: Bug Tracker, https://github.com/boxpet/pygeomag/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Welcome to pyGeoMag's documentation!
+====================================
+
+.. image:: https://dl.circleci.com/status-badge/img/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main.svg?style=svg&circle-token=13df862914431a3f89a9bc1bcc8bb5b2a177d815
+   :target: https://dl.circleci.com/status-badge/redirect/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main
+   :alt: CircleCI
+.. image:: https://codecov.io/gh/boxpet/pygeomag/graph/badge.svg?token=ECHON65OG8
+   :target: https://codecov.io/gh/boxpet/pygeomag
+   :alt: codecov
+.. image:: https://img.shields.io/pypi/v/pygeomag
+   :target: https://pypi.org/project/pygeomag/
+   :alt: PyPI
+.. image:: https://readthedocs.org/projects/pygeomag/badge/?version=latest
+   :target: https://pygeomag.readthedocs.io/
+   :alt: Documentation Status
+.. image:: https://img.shields.io/github/license/boxpet/pygeomag.svg
+   :target: https://github.com/boxpet/pygeomag/blob/main/LICENSE
+   :alt: License: MIT
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Code Style: Ruff
+
+
+**What is declination?**
+
+Declination is the angle that adjusts a compass reading from Magnetic North to True North. Many
+maps will show it in the legend, so you can adjust your compass (either physically or mentally).
+
+**Why do you need this?**
+
+In Washington State, the declination angle is between 14° and 16° West depending on your location. Meaning if I just
+pull out my compass and head North, I'm really heading at about 15°. And now if I walk 500 feet on that course, I'll be
+about 130 feet to the East of where I wanted to be.
+
+Now say I'm building a device that includes a magnetometer. I get it all calibrated to point to Magnetic North, show
+this value on the device and now the user is pointing in the wrong direction. And of course, the values change yearly.
+In the last 10 years, it's dropped just over a full degree in the Greater Seattle area. Here is where pyGeoMag comes in.
+
+To help see how much the magnetic field changes as you travel across the globe, here is projection for 2020 from
+NOAA:
+
+.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Main%20Field-%20Annual%20Change%20Declination%20%28D%29.jpg
+   :alt: US/UK World Magnetic Model - Epoch 2020.0: Main Field Declination
+
+To see how much the value changes per year (The contour interval is 2 arcminutes/year):
+
+.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Secular%20Variation-%20Annual%20Change%20Declination%20%28D%29.jpg
+   :alt: US/UK World Magnetic Model - Epoch 2020.0: Annual Change Declination
+
+If you want to look up these values, you can use NOAA's
+`Magnetic Field Caculators <https://www.ngdc.noaa.gov/geomag/calculators/magcalc.shtml>`_ in a browser or install their
+**CrowdMag** app on your `Android <https://play.google.com/store/apps/details?id=gov.noaa.ngdc.wmm2>`_ or
+`iOS <https://itunes.apple.com/app/id910578825>`_ device.
+
+**pyGeoMag** is an implementation written in Python of the
+`World Magnetic Model (WMM) <https://www.ncei.noaa.gov/products/world-magnetic-model>`_, specifically to be used in
+lightweight versions (like MicroPython and CircuitPython).
+
+**From NOAA**
+
+   The World Magnetic Model (WMM) is the standard model for navigation, attitude, and heading referencing systems using
+   the geomagnetic field. Additional WMM uses include civilian applications, including navigation and heading systems.
+
+   The model is a joint product of the United States' National Geospatial-Intelligence Agency (NGA) and the United
+   Kingdom's Defence Geographic Centre (DGC). NCEI and the British Geological Survey (BGS) jointly developed the WMM.
+   The U.S. Department of Defense, the U.K. Ministry of Defence, the North Atlantic Treaty Organization (NATO), and the
+   International Hydrographic Organization (IHO) use the WMM.
+
+Installation
+------------
+
+Install using `pip <http://www.pip-installer.org/en/latest>`_ with:
+
+.. code-block:: shell
+
+   pip install pygeomag
+
+Example
+-------
+
+Calculate the geomagnetic declination at the Space Needle in Seattle, WA:
+
+.. code-block:: pycon
+
+   >>> from pygeomag import GeoMag
+   >>> geo_mag = GeoMag()
+   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2023.75)
+   >>> print(result.d)
+   15.25942260585284
+
+And calculate it for the same spot 10 years ago:
+
+.. code-block:: pycon
+
+   >>> from pygeomag import GeoMag
+   >>> geo_mag = GeoMag(coefficients_file='wmm/WMM_2010.COF')
+   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2013.75)
+   >>> print(result.d)
+   16.32554283003356
+
+Validation
+----------
+
+All test values from the official NOAA WMM documentation are tested here for WMM-2020, WMM-2015v2, WMM-2015 and
+WMM-2010.
+
+Notes
+-----
+
+This is a direct port from the Legacy C code provided by NOAA. It defaults to using the WMM-2020 Coefficient file
+(WMM.COF) valid for 2020.0 - 2025.0. The code is specifically not 100% pythonic in order to make adding updates simple
+(for example uppercase variable names).
+
+At this point Annual change also known as Secular Variation is not in this package the Legacy C version does a direct
+``year+1.value - year2.value`` and both the test values and other existing code bases do something different.
+
+Documentation
+-------------
+
+More documentation and examples can be found at `Read the Docs <http://pygeomag.readthedocs.io/>`_.
```

### Comparing `pygeomag-1.0.1/pygeomag/__init__.py` & `pygeomag-1.0.2/pygeomag/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/format.py` & `pygeomag-1.0.2/pygeomag/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
 
 
 def round_to_digits(number, number_of_digits=0):
-    """
-    Round to number of digits, removing all if `0` and not Pythons round to even number strategy.
+    """Round to number of digits, removing all if `0` and not Pythons round to even number strategy.
 
     >>> from pygeomag import round_to_digits
     >>> round_to_digits(45.7625, 0)
     46
     >>> round_to_digits(45.7625, 1)
     45.8
     >>> round_to_digits(45.7625, 2)
@@ -16,16 +15,15 @@
     multiplier = 10**number_of_digits
     abs_rounded_value = math.floor(abs(number) * multiplier + 0.5) / multiplier
     rounded_value = math.copysign(abs_rounded_value, number)
     return int(rounded_value) if number_of_digits == 0 else rounded_value
 
 
 def decimal_degrees_to_degrees_minutes(decimal_degrees):
-    """
-    Convert decimal degrees to degrees and minutes.
+    """Convert decimal degrees to degrees and minutes.
 
     >>> from pygeomag import decimal_degrees_to_degrees_minutes
     >>> decimal_degrees_to_degrees_minutes(45.7625)
     (45, 45.75)
     """
     if not isinstance(decimal_degrees, (int, float)):
         raise TypeError("value is not a number")
@@ -33,31 +31,29 @@
     degrees = int(decimal_degrees)
     minutes = round_to_digits((float(decimal_degrees) - degrees) * 60, 12)
 
     return degrees, abs(minutes)
 
 
 def decimal_degrees_to_degrees_minutes_seconds(decimal_degrees):
-    """
-    Convert decimal degrees to degrees, minutes and seconds.
+    """Convert decimal degrees to degrees, minutes and seconds.
 
     >>> from pygeomag import decimal_degrees_to_degrees_minutes_seconds
     >>> decimal_degrees_to_degrees_minutes_seconds(45.7625)
     (45, 45, 45.0)
     """
     degrees, decimal_minutes = decimal_degrees_to_degrees_minutes(decimal_degrees)
     minutes = int(decimal_minutes)
     seconds = round_to_digits((float(decimal_minutes) - minutes) * 60, 12)
 
     return degrees, minutes, seconds
 
 
 def degrees_minutes_seconds_to_decimal_degrees(degrees, minutes, seconds):
-    """
-    Convert degrees, minutes and seconds  to decimal degrees.
+    """Convert degrees, minutes and seconds  to decimal degrees.
 
     >>> from pygeomag import degrees_minutes_seconds_to_decimal_degrees
     >>> degrees_minutes_seconds_to_decimal_degrees(45, 45, 45)
     45.7625
     """
     if not isinstance(degrees, (int, float)):
         raise TypeError("degrees is not a number")
@@ -66,32 +62,36 @@
     if not isinstance(seconds, (int, float)):
         raise TypeError("seconds is not a number")
 
     return degrees + minutes / 60 + seconds / 3600
 
 
 def degrees_minutes_to_decimal_degrees(degrees, minutes):
-    """
-    Convert degrees and minutes  to decimal degrees (45.7625).
+    """Convert degrees and minutes  to decimal degrees (45.7625).
 
     >>> from pygeomag import degrees_minutes_to_decimal_degrees
     >>> degrees_minutes_to_decimal_degrees(45, 45.75)
     45.7625
     """
     if not isinstance(degrees, (int, float)):
         raise TypeError("degrees is not a number")
     if not isinstance(minutes, (int, float)):
         raise TypeError("minutes is not a number")
 
     return degrees + minutes / 60
 
 
-def pretty_print_degrees(decimal_degrees, is_latitude, show_seconds=False, full_words=False, number_of_digits=0):
-    """
-    Format decimal degrees into a human-readable string.
+def pretty_print_degrees(
+    decimal_degrees,
+    is_latitude,
+    show_seconds=False,
+    full_words=False,
+    number_of_digits=0,
+):
+    """Format decimal degrees into a human-readable string.
 
     :param float, int decimal_degrees: Decimal degrees you want converted
     :param bool is_latitude: True for latitude, False for longitude
     :param bool show_seconds: True to show seconds, False for just degrees and minutes
     :param bool full_words: True to use full words like "North", False for single characters like "N"
     :param int number_of_digits: The amount of digits to round the last value to
     :return: Human-readable string
@@ -101,29 +101,31 @@
     "45° 46' N"
     >>> pretty_print_degrees(decimal_degrees=45.7625, is_latitude=True, number_of_digits=2)
     "45° 45.75' N"
     >>> pretty_print_degrees(decimal_degrees=45.7625, is_latitude=True, full_words=True, number_of_digits=2)
     '45 Degrees 45.75 Minutes North'
     """
     if show_seconds:
-        degrees, minutes, seconds = decimal_degrees_to_degrees_minutes_seconds(decimal_degrees)
+        degrees, minutes, seconds = decimal_degrees_to_degrees_minutes_seconds(
+            decimal_degrees
+        )
         seconds = round_to_digits(seconds, number_of_digits)
         string_format = "{degrees}{degrees_word} {minutes}{minutes_word} {seconds}{seconds_word} {ordinal_word}"
     else:
         degrees, minutes = decimal_degrees_to_degrees_minutes(decimal_degrees)
         minutes = round_to_digits(minutes, number_of_digits)
         seconds = 0
         string_format = "{degrees}{degrees_word} {minutes}{minutes_word} {ordinal_word}"
 
     if full_words:
         degrees_word = " Degrees"
         minutes_word = " Minutes"
         seconds_word = " Seconds"
     else:
-        degrees_word = "\xB0"
+        degrees_word = "\xb0"
         minutes_word = "'"
         seconds_word = '"'
 
     if is_latitude and decimal_degrees >= 0:
         ordinal_word = "North"
     elif is_latitude and decimal_degrees < 0:
         ordinal_word = "South"
```

### Comparing `pygeomag-1.0.1/pygeomag/geomag.py` & `pygeomag-1.0.2/pygeomag/geomag.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import math
 
+WWM_MODEL_2015_LOWER = 2015.0
+WWM_MODEL_2015_UPPER = 2020.0
+WWM_MODEL_2020_LOWER = 2020.0
+WWM_MODEL_2020_UPPER = 2025.0
+
+BLACKOUT_ZONE = 2000
+CAUTION_ZONE = 6000
+
 
 class BlackoutZoneException(Exception):
-    """
-    Horizontal intensity is in a Blackout Zone.
+    """Horizontal intensity is in a Blackout Zone.
 
     The Blackout Zones are defined as regions around the north and south magnetic poles where the horizontal intensity
     of Earth's magnetic field (H) is less than 2000 nT. In these zones WMM declination values are inaccurate and
     compasses are unreliable.
     """
 
 
 class CautionZoneException(Exception):
-    """
-    Horizontal intensity is in a Caution Zone.
+    """Horizontal intensity is in a Caution Zone.
 
     A Caution Zone is an areas around a Blackout Zone where caution must be exercised while using a compass. It is
     defined where Earth's magnetic field (H) is between 2000 and 6000 nT. Compass accuracy may be degraded in this
     region.
     """
 
 
 class GeoMagResult:
-    """
-    The Magnetic Components values from ``GeoMag.calculate()``.
+    """The Magnetic Components values from ``GeoMag.calculate()``.
 
     - **glat** *(float)* – Geodetic Latitude, -90.00 to +90.00 degrees (North positive, South negative)
     - **glon** *(float)* – Geodetic Longitude, -180.00 to +180.00 degrees (East positive, West negative)
     - **alt** *(float)* – Altitude, -1 to 850km referenced to the WGS 84 ellipsoid OR the Mean Sea Level (MSL)
     - **time** *(float)* – Time (in decimal year), 2020.0 to 2025.0
     - **f**, **.ti**, **.total_intensity** *(float)* – Total Intensity
     - **h** *(float)* – Horizontal Intensity
@@ -79,39 +84,42 @@
     def total_intensity(self):
         """Additional name for variable f."""
         return self.f
 
     def calculate(self, raise_in_warning_zone):
         """Calculate extra result values."""
         # COMPUTE X, Y, Z, AND H COMPONENTS OF THE MAGNETIC FIELD
-        self.x = self.f * (math.cos(math.radians(self.d)) * math.cos(math.radians(self.i)))
-        self.y = self.f * (math.cos(math.radians(self.i)) * math.sin(math.radians(self.d)))
+        self.x = self.f * (
+            math.cos(math.radians(self.d)) * math.cos(math.radians(self.i))
+        )
+        self.y = self.f * (
+            math.cos(math.radians(self.i)) * math.sin(math.radians(self.d))
+        )
         self.z = self.f * (math.sin(math.radians(self.i)))
         self.h = self.f * (math.cos(math.radians(self.i)))
 
         # Check if in Caution or Blackout Zones
-        if self.h < 2000:
+        if self.h < BLACKOUT_ZONE:
             if raise_in_warning_zone:
                 raise BlackoutZoneException(
                     f"The horizontal field strength at this location is {self.h:.1f}. Compass readings have VERY LARGE "
                     "uncertainties in areas where H smaller than 2000 nT"
                 )
             self.in_blackout_zone = True
 
-        elif self.h < 6000:
+        elif self.h < CAUTION_ZONE:
             if raise_in_warning_zone:
                 raise CautionZoneException(
                     f"The horizontal field strength at this location is {self.h:.1f}. Compass readings have large "
                     "uncertainties in areas where H smaller than 6000 nT"
                 )
             self.in_caution_zone = True
 
     def calculate_uncertainty(self):
-        """
-        Calculate the uncertainty values for this ``GeoMagResult``.
+        """Calculate the uncertainty values for this ``GeoMagResult``.
 
         Uncertainty estimates provided by the **WMM2015** and **WMM2020** error model for the various field components.
         H is expressed in nT in the formula providing the error in D.
 
         These values can currently only be computed for ``GeoMagResult`` between 2015.0 and 2025.0 and using a value
         outside this will raise an Exception
 
@@ -122,16 +130,15 @@
         >>> print(uncertainty.d)
         0.3935273117953904
         """
         return GeoMagUncertaintyResult(self)
 
 
 class GeoMagUncertaintyResult:
-    """
-    The uncertainty values of a ``GeoMagResult``.
+    """The uncertainty values of a ``GeoMagResult``.
 
     - **f** *(float)* – Uncertainty of the Total Intensity in nT
     - **h** *(float)* – Uncertainty of the Horizontal Intensity in nT
     - **x** *(float)* – Uncertainty of the North Component in nT
     - **y** *(float)* – Uncertainty of the East Component in nT
     - **z** *(float)* – Uncertainty of the Vertical Component in nT
     - **i** *(float)* – Uncertainty of the Geomagnetic Inclination in degrees
@@ -143,17 +150,17 @@
         self.y = None
         self.z = None
         self.h = None
         self.f = None
         self.i = None
         self.d = None
 
-        if 2020.0 <= result.time <= 2025.0:
+        if WWM_MODEL_2020_LOWER <= result.time <= WWM_MODEL_2020_UPPER:
             self._error_model_wmm_2020(result)
-        elif 2015.0 <= result.time < 2020.0:
+        elif WWM_MODEL_2015_LOWER <= result.time < WWM_MODEL_2015_UPPER:
             self._error_model_wmm_2015(result)
         else:
             raise ValueError("GeoMagResult outside of known uncertainty estimates.")
 
     def _error_model_wmm_2015(self, result):
         """Calculate uncertainty estimates for 2015.0 to 2020.0."""
         self.x = 138.0
@@ -172,16 +179,15 @@
         self.h = 128.0
         self.f = 148.0
         self.i = 0.21
         self.d = math.sqrt(0.26**2 + (5625 / result.h) ** 2)
 
 
 class GeoMag:
-    """
-    Python port of the Legacy C code provided by NOAA for the World Magnetic Model (WMM).
+    """Python port of the Legacy C code provided by NOAA for the World Magnetic Model (WMM).
 
     It defaults to using the WMM-2020 Coefficient file (WMM.COF) valid for 2020.0 - 2025.0.
 
     Included are the following coefficient files, if you have the need to calculate past values:
 
     .. table::
        :widths: auto
@@ -193,24 +199,25 @@
        WMM_2015v2.COF  WMM-2015v2  2015.0 - 2020.0  09/18/2018
        WMM_2015.COF    WMM-2015    2015.0 - 2020.0  12/15/2014
        WMM_2010.COF    WMM-2010    2010.0 - 2015.0  11/20/2009
        ==============  ==========  ===============  ==========
     """
 
     def __init__(self, coefficients_file=None, coefficients_data=None):
-        """
-        Create a GeoMag instance.
+        """Create a GeoMag instance.
 
         Leaving both values as ``None`` will load the packages default coefficients file, supplying both will raise.
 
         :param str coefficients_file: Full or relative path to a coefficients file supplied by this package or WMM
         :param str coefficients_data: coefficients data from a python module
         """
         if coefficients_file is not None and coefficients_data is not None:
-            raise ValueError("Both coefficients_file and coefficients_data supplied, supply none or only one.")
+            raise ValueError(
+                "Both coefficients_file and coefficients_data supplied, supply none or only one."
+            )
 
         self._coefficients_data = coefficients_data
         self._coefficients_file = coefficients_file
         self._maxord = 12
         self._epoch = None
         self._model = None
         self._release_date = None
@@ -282,30 +289,32 @@
         try:
             with open(wmm_filepath_2):
                 self._coefficients_file = wmm_filepath_2
                 return wmm_filepath_2
         except OSError:
             return wmm_filepath
 
-    def _load_coefficients(self):
+    def _load_coefficients(self):  # noqa: PLR0915 - Too many statements
         """Load the coefficients model to calculate the Magnetic Components from."""
         if self._epoch is not None:
             return
 
         c = self._create_matrix(13, 13)
         cd = self._create_matrix(13, 13)
         snorm = self._create_list(169)
         fn = self._create_list(13)
         fm = self._create_list(13)
         k = self._create_matrix(13, 13)
 
         if self._coefficients_data:
             (epoch, model, release_date), coefficients = self._coefficients_data
         else:
-            (epoch, model, release_date), coefficients = self._read_coefficients_data_from_file()
+            (epoch, model, release_date), coefficients = (
+                self._read_coefficients_data_from_file()
+            )
 
         # READ WORLD MAGNETIC MODEL SPHERICAL HARMONIC COEFFICIENTS
         c[0][0] = 0.0
         cd[0][0] = 0.0
 
         for n, m, gnm, hnm, dgnm, dhnm in coefficients:
             if m > self._maxord:
@@ -322,18 +331,20 @@
         # CONVERT SCHMIDT NORMALIZED GAUSS COEFFICIENTS TO UNNORMALIZED
         snorm[0] = 1.0
         fm[0] = 0.0
         for n in range(1, self._maxord + 1):
             snorm[n] = snorm[n - 1] * float(2 * n - 1) / float(n)
             j = 2
             m = 0
-            D1 = 1  # noqa pyCharm: Variable in function should be lowercase
-            D2 = (n - m + D1) / D1  # noqa pyCharm: Variable in function should be lowercase
+            D1 = 1
+            D2 = (n - m + D1) / D1
             while D2 > 0:
-                k[m][n] = float(((n - 1) * (n - 1)) - (m * m)) / float((2 * n - 1) * (2 * n - 3))
+                k[m][n] = float(((n - 1) * (n - 1)) - (m * m)) / float(
+                    (2 * n - 1) * (2 * n - 3)
+                )
                 if m > 0:
                     flnmj = float((n - m + 1) * j) / float(n + m)
                     snorm[n + m * 13] = snorm[n + (m - 1) * 13] * math.sqrt(flnmj)
                     j = 1
                     c[n][m - 1] = snorm[n + m * 13] * c[n][m - 1]
                     cd[n][m - 1] = snorm[n + m * 13] * cd[n][m - 1]
                 c[m][n] = snorm[n + m * 13] * c[m][n]
@@ -360,46 +371,50 @@
 
         model_filename = self._get_model_filename()
 
         with open(model_filename) as coefficients_file:
             # READ WORLD MAGNETIC MODEL SPHERICAL HARMONIC COEFFICIENTS
             line_data = coefficients_file.readline()
             line_values = line_data.split()
-            if len(line_values) != 3:
+            if len(line_values) != 3:  # noqa: PLR2004 Magic value used in comparison:
                 raise ValueError("Invalid header in model file")
-            epoch, model, release_date = (t(s) for t, s in zip((float, str, str), line_values))
+            epoch, model, release_date = (
+                t(s) for t, s in zip((float, str, str), line_values)
+            )
 
             while True:
                 line_data = coefficients_file.readline()
 
                 # CHECK FOR LAST LINE IN FILE
                 if line_data[:4] == "9999":
                     break
 
                 # END OF FILE NOT ENCOUNTERED, GET VALUES
                 line_values = line_data.split()
-                if len(line_values) != 6:
+                if len(line_values) != 6:  # noqa: PLR2004 Magic value used in comparison
                     raise ValueError("Corrupt record in model file")
-                n, m, gnm, hnm, dgnm, dhnm = (t(s) for t, s in zip((int, int, float, float, float, float), line_values))
+                n, m, gnm, hnm, dgnm, dhnm = (
+                    t(s)
+                    for t, s in zip((int, int, float, float, float, float), line_values)
+                )
 
                 data.append((n, m, gnm, hnm, dgnm, dhnm))
 
         return (epoch, model, release_date), data
 
-    def calculate(
+    def calculate(  # noqa: PLR0912,PLR0913,PLR0915 - Too many branches,Too many arguments,Too many statements
         self,
         glat,
         glon,
         alt,
         time,
         allow_date_outside_lifespan=False,
         raise_in_warning_zone=False,
     ):
-        """
-        Calculate the Magnetic Components from a latitude, longitude, altitude and date.
+        """Calculate the Magnetic Components from a latitude, longitude, altitude and date.
 
         :param float glat: Geodetic Latitude, -90.00 to +90.00 degrees (North positive, South negative)
         :param float glon: Geodetic Longitude, -180.00 to +180.00 degrees (East positive, West negative)
         :param float alt: Altitude, -1 to 850km referenced to the WGS 84 ellipsoid OR the Mean Sea Level (MSL)
         :param float time: Time (in decimal year), 2020.0 to 2025.0
         :param bool allow_date_outside_lifespan: True, if you want an estimation outside the 5-year life span
         :param bool raise_in_warning_zone: True if you want to raise a BlackoutZoneException or CautionZoneException
@@ -450,15 +465,15 @@
         #        which are in the legacy c app for speeding it up for getting the Secular Change
         #   2. Remove them
         # otime = oalt = olat = olon = -1000.0
 
         dt = time - self._epoch
         # TODO #1: Legacy C code static vars for speed
         # if otime < 0.0 and (dt < 0.0 or dt > 5.0) and not allow_date_past_lifespan:
-        if True and (dt < 0.0 or dt > 5.0) and not allow_date_outside_lifespan:
+        if True and (dt < 0.0 or dt > 5.0) and not allow_date_outside_lifespan:  # noqa: PLR2004 Magic value used in comparison:
             raise ValueError("Time extends beyond model 5-year life span")
 
         rlon = math.radians(glon)
         rlat = math.radians(glat)
         srlon = math.sin(rlon)
         srlat = math.sin(rlat)
         crlon = math.cos(rlon)
@@ -490,35 +505,44 @@
                 cp[m] = cp[1] * cp[m - 1] - sp[1] * sp[m - 1]
         aor = re / r
         ar = aor * aor
         br = bt = bp = bpp = 0.0
         for n in range(1, self._maxord + 1):
             ar = ar * aor
             m = 0
-            D3 = 1  # noqa pyCharm: Variable in function should be lowercase
-            D4 = (n + m + D3) / D3  # noqa pyCharm: Variable in function should be lowercase
+            D3 = 1
+            D4 = (n + m + D3) / D3
             while D4 > 0:
                 # COMPUTE UNNORMALIZED ASSOCIATED LEGENDRE POLYNOMIALS
                 # AND DERIVATIVES VIA RECURSION RELATIONS
                 # TODO #1: Legacy C code static vars for speed
                 # if alt != oalt or glat != olat:
                 if True:
                     if n == m:
                         self._p[n + m * 13] = st * self._p[n - 1 + (m - 1) * 13]
-                        dp[m][n] = st * dp[m - 1][n - 1] + ct * self._p[n - 1 + (m - 1) * 13]
+                        dp[m][n] = (
+                            st * dp[m - 1][n - 1] + ct * self._p[n - 1 + (m - 1) * 13]
+                        )
                     elif n == 1 and m == 0:
                         self._p[n + m * 13] = ct * self._p[n - 1 + m * 13]
                         dp[m][n] = ct * dp[m][n - 1] - st * self._p[n - 1 + m * 13]
                     elif n > 1 and n != m:
                         if m > n - 2:
                             self._p[n - 2 + m * 13] = 0.0
                         if m > n - 2:
                             dp[m][n - 2] = 0.0
-                        self._p[n + m * 13] = ct * self._p[n - 1 + m * 13] - self._k[m][n] * self._p[n - 2 + m * 13]
-                        dp[m][n] = ct * dp[m][n - 1] - st * self._p[n - 1 + m * 13] - self._k[m][n] * dp[m][n - 2]
+                        self._p[n + m * 13] = (
+                            ct * self._p[n - 1 + m * 13]
+                            - self._k[m][n] * self._p[n - 2 + m * 13]
+                        )
+                        dp[m][n] = (
+                            ct * dp[m][n - 1]
+                            - st * self._p[n - 1 + m * 13]
+                            - self._k[m][n] * dp[m][n - 2]
+                        )
 
                 # TIME ADJUST THE GAUSS COEFFICIENTS
                 # TODO #1: Legacy C code static vars for speed
                 # if time != otime:
                 if True:
                     tc[m][n] = self._c[m][n] + dt * self._cd[m][n]
                     if m != 0:
@@ -570,26 +594,26 @@
 
         # COMPUTE MAGNETIC GRID VARIATION IF THE CURRENT
         # GEODETIC POSITION IS IN THE ARCTIC OR ANTARCTIC
         # (I.E. GLAT > +55 DEGREES OR GLAT < -55 DEGREES)
         #
         # OTHERWISE, SET MAGNETIC GRID VARIATION TO -999.0
         result.gv = gv_default = -999.0
-        if math.fabs(glat) >= 55.0:
+        if math.fabs(glat) >= 55.0:  # noqa: PLR2004 Magic value used in comparison
             if glat > 0.0 and glon >= 0.0:
                 result.gv = result.d - glon
-            if glat > 0.0 and glon < 0.0:  # noqa pyCharm: simplify chained comparison
+            if glat > 0.0 and glon < 0.0:
                 result.gv = result.d + math.fabs(glon)
-            if glat < 0.0 and glon >= 0.0:  # noqa pyCharm: simplify chained comparison
+            if glat < 0.0 and glon >= 0.0:
                 result.gv = result.d + glon
             if glat < 0.0 and glon < 0.0:
                 result.gv = result.d - math.fabs(glon)
-            if result.gv > +180.0:
+            if result.gv > +180.0:  # noqa: PLR2004 Magic value used in comparison
                 result.gv -= 360.0
-            if result.gv < -180.0:
+            if result.gv < -180.0:  # noqa: PLR2004 Magic value used in comparison
                 result.gv += 360.0
         if result.gv == gv_default:
             result.gv = None
 
         result.calculate(raise_in_warning_zone)
 
         # TODO #1: Legacy C code static vars for speed
```

### Comparing `pygeomag-1.0.1/pygeomag/time.py` & `pygeomag-1.0.2/pygeomag/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 SECONDS_PER_DAY = 86400
 
 
 def decimal_year_from_struct_time(date):
-    """
-    Calculate the decimal year (2022.5) from a 'time.struct_time'.
+    """Calculate the decimal year (2022.5) from a 'time.struct_time'.
 
     >>> import time
     >>> from pygeomag import decimal_year_from_struct_time
     >>> value = time.struct_time((2020, 7, 2, 0, 0, 0, 0, 0, 0))
     >>> decimal_year_from_struct_time(value)
     2020.5
     """
@@ -23,16 +22,15 @@
     following_year = time.mktime(time.struct_time((year + 1, 1, 1, 0, 0, 0, 0, 0, 0)))
     days_in_year = (following_year - current_year) / SECONDS_PER_DAY
     days_passed = int((time.mktime(date) - current_year) / SECONDS_PER_DAY)
     return year + float(days_passed) / days_in_year
 
 
 def decimal_year_from_date(date):
-    """
-    Calculate the decimal year (2022.5) from a 'datetime.date' or 'datetime.datetime'.
+    """Calculate the decimal year (2022.5) from a 'datetime.date' or 'datetime.datetime'.
 
     >>> import datetime
     >>> from pygeomag import decimal_year_from_date
     >>> value = datetime.datetime(2020, 7, 2)
     >>> decimal_year_from_date(value)
     2020.5
     """
@@ -46,30 +44,29 @@
     following_year = datetime.date(year, 1, 1)
     days_in_year = (current_year - following_year).days
     days_passed = (date - datetime.date(year, 1, 1)).days
     return year + float(days_passed) / days_in_year
 
 
 def calculate_decimal_year(date):
-    """
-    Calculate the decimal year (2022.5) from a value (i.e. 'datetime.datetime' or 'time.struct_time').
+    """Calculate the decimal year (2022.5) from a value (i.e. 'datetime.datetime' or 'time.struct_time').
 
     If you know using either date format will work in your version of Python, you can use this wrapper method.
 
     >>> import datetime
     >>> from pygeomag import calculate_decimal_year
     >>> calculate_decimal_year(datetime.datetime(2020, 7, 2))
     2020.5
     """
     # Inline imports to not fail on lightweight versions of Python
     import datetime
     import time
 
     if isinstance(date, (float, int)):
-        if date < 3000:
+        if date < 3000:  # noqa: PLR2004 - Magic value used in comparison
             return float(date)
         else:
             return decimal_year_from_struct_time(time.localtime(date))
     elif isinstance(date, datetime.date):
         return decimal_year_from_date(date)
     elif isinstance(date, time.struct_time):
         return decimal_year_from_struct_time(date)
```

### Comparing `pygeomag-1.0.1/pygeomag/wmm/WMM.COF` & `pygeomag-1.0.2/pygeomag/wmm/WMM.COF`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/WMM_2010.COF` & `pygeomag-1.0.2/pygeomag/wmm/WMM_2010.COF`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/WMM_2015.COF` & `pygeomag-1.0.2/pygeomag/wmm/WMM_2015.COF`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/WMM_2015v2.COF` & `pygeomag-1.0.2/pygeomag/wmm/WMM_2015v2.COF`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/wmm_2010.py` & `pygeomag-1.0.2/pygeomag/wmm/wmm_2010.py`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/wmm_2015.py` & `pygeomag-1.0.2/pygeomag/wmm/wmm_2015.py`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/wmm_2015v2.py` & `pygeomag-1.0.2/pygeomag/wmm/wmm_2015v2.py`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag/wmm/wmm_2020.py` & `pygeomag-1.0.2/pygeomag/wmm/wmm_2020.py`

 * *Files identical despite different names*

### Comparing `pygeomag-1.0.1/pygeomag.egg-info/PKG-INFO` & `pygeomag-1.0.2/pygeomag.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,135 @@
-Metadata-Version: 2.1
-Name: pygeomag
-Version: 1.0.1
-Summary: A python port of the World Magnetic Model (WMM)
-Author: Justin Myers
-Project-URL: Homepage, https://github.com/boxpet/pygeomag
-Project-URL: Bug Tracker, https://github.com/boxpet/pygeomag/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Welcome to pyGeoMag's documentation!
-====================================
-
-.. image:: https://dl.circleci.com/status-badge/img/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main.svg?style=svg&circle-token=13df862914431a3f89a9bc1bcc8bb5b2a177d815
-   :target: https://dl.circleci.com/status-badge/redirect/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main
-   :alt: CircleCI
-.. image:: https://codecov.io/gh/boxpet/pygeomag/graph/badge.svg?token=ECHON65OG8
-   :target: https://codecov.io/gh/boxpet/pygeomag
-   :alt: codecov
-.. image:: https://img.shields.io/pypi/v/pygeomag
-   :target: https://pypi.org/project/pygeomag/
-   :alt: PyPI
-.. image:: https://readthedocs.org/projects/pygeomag/badge/?version=latest
-   :target: https://pygeomag.readthedocs.io/
-   :alt: Documentation Status
-.. image:: https://img.shields.io/github/license/boxpet/pygeomag.svg
-   :target: https://github.com/boxpet/pygeomag/blob/main/LICENSE
-   :alt: License: MIT
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
-**What is declination?**
-
-Declination is the angle that adjusts a compass reading from Magnetic North to True North. Many
-maps will show it in the legend, so you can adjust your compass (either physically or mentally).
-
-**Why do you need this?**
-
-In Washington State, the declination angle is between 14° and 16° West depending on your location. Meaning if I just
-pull out my compass and head North, I'm really heading at about 15°. And now if I walk 500 feet on that course, I'll be
-about 130 feet to the East of where I wanted to be.
-
-Now say I'm building a device that includes a magnetometer. I get it all calibrated to point to Magnetic North, show
-this value on the device and now the user is pointing in the wrong direction. And of course, the values change yearly.
-In the last 10 years, it's dropped just over a full degree in the Greater Seattle area. Here is where pyGeoMag comes in.
-
-To help see how much the magnetic field changes as you travel across the globe, here is projection for 2020 from
-NOAA:
-
-.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Main%20Field-%20Annual%20Change%20Declination%20%28D%29.jpg
-   :alt: US/UK World Magnetic Model - Epoch 2020.0: Main Field Declination
-
-To see how much the value changes per year (The contour interval is 2 arcminutes/year):
-
-.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Secular%20Variation-%20Annual%20Change%20Declination%20%28D%29.jpg
-   :alt: US/UK World Magnetic Model - Epoch 2020.0: Annual Change Declination
-
-If you want to look up these values, you can use NOAA's
-`Magnetic Field Caculators <https://www.ngdc.noaa.gov/geomag/calculators/magcalc.shtml>`_ in a browser or install their
-**CrowdMag** app on your `Android <https://play.google.com/store/apps/details?id=gov.noaa.ngdc.wmm2>`_ or
-`iOS <https://itunes.apple.com/app/id910578825>`_ device.
-
-**pyGeoMag** is an implementation written in Python of the
-`World Magnetic Model (WMM) <https://www.ncei.noaa.gov/products/world-magnetic-model>`_, specifically to be used in
-lightweight versions (like MicroPython and CircuitPython).
-
-**From NOAA**
-
-   The World Magnetic Model (WMM) is the standard model for navigation, attitude, and heading referencing systems using
-   the geomagnetic field. Additional WMM uses include civilian applications, including navigation and heading systems.
-
-   The model is a joint product of the United States' National Geospatial-Intelligence Agency (NGA) and the United
-   Kingdom's Defence Geographic Centre (DGC). NCEI and the British Geological Survey (BGS) jointly developed the WMM.
-   The U.S. Department of Defense, the U.K. Ministry of Defence, the North Atlantic Treaty Organization (NATO), and the
-   International Hydrographic Organization (IHO) use the WMM.
-
-Installation
-------------
-
-Install using `pip <http://www.pip-installer.org/en/latest>`_ with:
-
-.. code-block:: shell
-
-   pip install pygeomag
-
-Example
--------
-
-Calculate the geomagnetic declination at the Space Needle in Seattle, WA:
-
-.. code-block:: pycon
-
-   >>> from pygeomag import GeoMag
-   >>> geo_mag = GeoMag()
-   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2023.75)
-   >>> print(result.d)
-   15.25942260585284
-
-And calculate it for the same spot 10 years ago:
-
-.. code-block:: pycon
-
-   >>> from pygeomag import GeoMag
-   >>> geo_mag = GeoMag(coefficients_file='wmm/WMM_2010.COF')
-   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2013.75)
-   >>> print(result.d)
-   16.32554283003356
-
-Validation
-----------
-
-All test values from the official NOAA WMM documentation are tested here for WMM-2020, WMM-2015v2, WMM-2015 and
-WMM-2010.
-
-Notes
------
-
-This is a direct port from the Legacy C code provided by NOAA. It defaults to using the WMM-2020 Coefficient file
-(WMM.COF) valid for 2020.0 - 2025.0. The code is specifically not 100% pythonic in order to make adding updates simple
-(for example uppercase variable names).
-
-At this point Annual change also known as Secular Variation is not in this package the Legacy C version does a direct
-``year+1.value - year2.value`` and both the test values and other existing code bases do something different.
-
-Documentation
--------------
-
-More documentation and examples can be found at `Read the Docs <http://pygeomag.readthedocs.io/>`_.
+Metadata-Version: 2.1
+Name: pygeomag
+Version: 1.0.2
+Summary: A python port of the World Magnetic Model (WMM)
+Author: Justin Myers
+Project-URL: Homepage, https://github.com/boxpet/pygeomag
+Project-URL: Bug Tracker, https://github.com/boxpet/pygeomag/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Welcome to pyGeoMag's documentation!
+====================================
+
+.. image:: https://dl.circleci.com/status-badge/img/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main.svg?style=svg&circle-token=13df862914431a3f89a9bc1bcc8bb5b2a177d815
+   :target: https://dl.circleci.com/status-badge/redirect/circleci/5uMninjUXjCnNMzvVzq9EJ/A7hoBacfgFtGdDUiyiXcBy/tree/main
+   :alt: CircleCI
+.. image:: https://codecov.io/gh/boxpet/pygeomag/graph/badge.svg?token=ECHON65OG8
+   :target: https://codecov.io/gh/boxpet/pygeomag
+   :alt: codecov
+.. image:: https://img.shields.io/pypi/v/pygeomag
+   :target: https://pypi.org/project/pygeomag/
+   :alt: PyPI
+.. image:: https://readthedocs.org/projects/pygeomag/badge/?version=latest
+   :target: https://pygeomag.readthedocs.io/
+   :alt: Documentation Status
+.. image:: https://img.shields.io/github/license/boxpet/pygeomag.svg
+   :target: https://github.com/boxpet/pygeomag/blob/main/LICENSE
+   :alt: License: MIT
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Code Style: Ruff
+
+
+**What is declination?**
+
+Declination is the angle that adjusts a compass reading from Magnetic North to True North. Many
+maps will show it in the legend, so you can adjust your compass (either physically or mentally).
+
+**Why do you need this?**
+
+In Washington State, the declination angle is between 14° and 16° West depending on your location. Meaning if I just
+pull out my compass and head North, I'm really heading at about 15°. And now if I walk 500 feet on that course, I'll be
+about 130 feet to the East of where I wanted to be.
+
+Now say I'm building a device that includes a magnetometer. I get it all calibrated to point to Magnetic North, show
+this value on the device and now the user is pointing in the wrong direction. And of course, the values change yearly.
+In the last 10 years, it's dropped just over a full degree in the Greater Seattle area. Here is where pyGeoMag comes in.
+
+To help see how much the magnetic field changes as you travel across the globe, here is projection for 2020 from
+NOAA:
+
+.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Main%20Field-%20Annual%20Change%20Declination%20%28D%29.jpg
+   :alt: US/UK World Magnetic Model - Epoch 2020.0: Main Field Declination
+
+To see how much the value changes per year (The contour interval is 2 arcminutes/year):
+
+.. image:: https://www.ncei.noaa.gov/sites/default/files/2022-02/Miller%20Projection%20Secular%20Variation-%20Annual%20Change%20Declination%20%28D%29.jpg
+   :alt: US/UK World Magnetic Model - Epoch 2020.0: Annual Change Declination
+
+If you want to look up these values, you can use NOAA's
+`Magnetic Field Caculators <https://www.ngdc.noaa.gov/geomag/calculators/magcalc.shtml>`_ in a browser or install their
+**CrowdMag** app on your `Android <https://play.google.com/store/apps/details?id=gov.noaa.ngdc.wmm2>`_ or
+`iOS <https://itunes.apple.com/app/id910578825>`_ device.
+
+**pyGeoMag** is an implementation written in Python of the
+`World Magnetic Model (WMM) <https://www.ncei.noaa.gov/products/world-magnetic-model>`_, specifically to be used in
+lightweight versions (like MicroPython and CircuitPython).
+
+**From NOAA**
+
+   The World Magnetic Model (WMM) is the standard model for navigation, attitude, and heading referencing systems using
+   the geomagnetic field. Additional WMM uses include civilian applications, including navigation and heading systems.
+
+   The model is a joint product of the United States' National Geospatial-Intelligence Agency (NGA) and the United
+   Kingdom's Defence Geographic Centre (DGC). NCEI and the British Geological Survey (BGS) jointly developed the WMM.
+   The U.S. Department of Defense, the U.K. Ministry of Defence, the North Atlantic Treaty Organization (NATO), and the
+   International Hydrographic Organization (IHO) use the WMM.
+
+Installation
+------------
+
+Install using `pip <http://www.pip-installer.org/en/latest>`_ with:
+
+.. code-block:: shell
+
+   pip install pygeomag
+
+Example
+-------
+
+Calculate the geomagnetic declination at the Space Needle in Seattle, WA:
+
+.. code-block:: pycon
+
+   >>> from pygeomag import GeoMag
+   >>> geo_mag = GeoMag()
+   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2023.75)
+   >>> print(result.d)
+   15.25942260585284
+
+And calculate it for the same spot 10 years ago:
+
+.. code-block:: pycon
+
+   >>> from pygeomag import GeoMag
+   >>> geo_mag = GeoMag(coefficients_file='wmm/WMM_2010.COF')
+   >>> result = geo_mag.calculate(glat=47.6205, glon=-122.3493, alt=0, time=2013.75)
+   >>> print(result.d)
+   16.32554283003356
+
+Validation
+----------
+
+All test values from the official NOAA WMM documentation are tested here for WMM-2020, WMM-2015v2, WMM-2015 and
+WMM-2010.
+
+Notes
+-----
+
+This is a direct port from the Legacy C code provided by NOAA. It defaults to using the WMM-2020 Coefficient file
+(WMM.COF) valid for 2020.0 - 2025.0. The code is specifically not 100% pythonic in order to make adding updates simple
+(for example uppercase variable names).
+
+At this point Annual change also known as Secular Variation is not in this package the Legacy C version does a direct
+``year+1.value - year2.value`` and both the test values and other existing code bases do something different.
+
+Documentation
+-------------
+
+More documentation and examples can be found at `Read the Docs <http://pygeomag.readthedocs.io/>`_.
```

