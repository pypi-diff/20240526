# Comparing `tmp/dsptoolbox-0.3.7.tar.gz` & `tmp/dsptoolbox-0.3.8.tar.gz`

## Comparing `dsptoolbox-0.3.7.tar` & `dsptoolbox-0.3.8.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/.gitattributes
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/.readthedocs.yaml
--rw-r--r--   0        0        0    18939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/CHANGELOG.rst
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/requirements.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/__rdme.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/classes.rst
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/conf.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/index.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/make.bat
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules.rst
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/readme.rst
--rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/logo/logo.png
--rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/logo/logo2.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.audio_io.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.beamforming.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.distances.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.effects.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.filterbanks.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.generators.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.plots.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.room_acoustics.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.standard_functions.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.transfer_functions.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/docs/modules/dsptoolbox.transforms.rst
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/__init__.py
--rw-r--r--   0        0        0    37498 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/_general_helpers.py
--rw-r--r--   0        0        0    36355 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/_standard.py
--rw-r--r--   0        0        0    47469 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/standard_functions.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/audio_io/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/audio_io/_audio_io.py
--rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/audio_io/audio_io.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/beamforming/__init__.py
--rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/beamforming/_beamforming.py
--rw-r--r--   0        0        0    62886 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/beamforming/beamforming.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/__init__.py
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/_filter.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/_lattice_ladder_filter.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/_phaseLinearizer.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/_plots.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/_svfilter.py
--rw-r--r--   0        0        0    32846 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/filter_class.py
--rw-r--r--   0        0        0    29479 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/filterbank.py
--rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/multibandsignal.py
--rw-r--r--   0        0        0    57835 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/classes/signal_class.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/distances/__init__.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/distances/_distances.py
--rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/distances/distances.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/effects/__init__.py
--rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/effects/_effects.py
--rw-r--r--   0        0        0    58609 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/effects/effects.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/filterbanks/__init__.py
--rw-r--r--   0        0        0    48939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/filterbanks/_filterbank.py
--rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/filterbanks/filterbanks.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/generators/__init__.py
--rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/generators/generators.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/plots/__init__.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/plots/plots.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/room_acoustics/__init__.py
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/room_acoustics/_room_acoustics.py
--rw-r--r--   0        0        0    22480 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/room_acoustics/room_acoustics.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/transfer_functions/__init__.py
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/transfer_functions/_transfer_functions.py
--rw-r--r--   0        0        0    63670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/transfer_functions/transfer_functions.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/transforms/__init__.py
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/transforms/_transforms.py
--rw-r--r--   0        0        0    30334 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/dsptoolbox/transforms/transforms.py
--rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/audio_io_module.ipynb
--rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/beamforming_module.ipynb
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/distances_module.ipynb
--rw-r--r--   0        0        0   409017 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/filterbanks_module.ipynb
--rw-r--r--   0        0        0  1013477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/general.ipynb
--rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/generators_module.ipynb
--rw-r--r--   0        0        0   180489 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/room_acoustics_module.ipynb
--rw-r--r--   0        0        0    94731 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/standard_module.ipynb
--rw-r--r--   0        0        0   208870 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/transfer_function_module.ipynb
--rw-r--r--   0        0        0  1248737 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/transforms_module.ipynb
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/array.xml
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/chirp.wav
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/chirp_mono.wav
--rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/chirp_stereo.wav
--rw-r--r--   0        0        0  1766444 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/fuer_elise.wav
--rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/rir.wav
--rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/examples/data/speech.flac
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_audio_io.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_beamforming.py
--rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_classes.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_distances.py
--rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_filterbanks.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_fx.py
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_generators.py
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_room_acoustics.py
--rw-r--r--   0        0        0    12211 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_standard.py
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_transfer_functions.py
--rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/tests/test_transforms.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/LICENSE
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/README.rst
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dsptoolbox-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/.gitattributes
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/.readthedocs.yaml
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/CHANGELOG.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/requirements.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/__rdme.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/classes.rst
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/conf.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/index.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/make.bat
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules.rst
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/readme.rst
+-rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/logo/logo.png
+-rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/logo/logo2.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.audio_io.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.beamforming.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.distances.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.effects.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.filterbanks.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.generators.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.plots.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.room_acoustics.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.standard_functions.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.transfer_functions.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/docs/modules/dsptoolbox.transforms.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/__init__.py
+-rw-r--r--   0        0        0    41152 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/_general_helpers.py
+-rw-r--r--   0        0        0    34244 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/_standard.py
+-rw-r--r--   0        0        0    47469 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/standard_functions.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/audio_io/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/audio_io/_audio_io.py
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/audio_io/audio_io.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/beamforming/__init__.py
+-rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/beamforming/_beamforming.py
+-rw-r--r--   0        0        0    62886 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/beamforming/beamforming.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/__init__.py
+-rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/_filter.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/_lattice_ladder_filter.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/_phaseLinearizer.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/_plots.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/_svfilter.py
+-rw-r--r--   0        0        0    32874 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/filter_class.py
+-rw-r--r--   0        0        0    29479 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/filterbank.py
+-rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/multibandsignal.py
+-rw-r--r--   0        0        0    57850 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/classes/signal_class.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/distances/__init__.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/distances/_distances.py
+-rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/distances/distances.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/effects/__init__.py
+-rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/effects/_effects.py
+-rw-r--r--   0        0        0    58609 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/effects/effects.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/filterbanks/__init__.py
+-rw-r--r--   0        0        0    48939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/filterbanks/_filterbank.py
+-rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/filterbanks/filterbanks.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/generators/__init__.py
+-rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/generators/generators.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/plots/__init__.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/plots/plots.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/room_acoustics/__init__.py
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/room_acoustics/_room_acoustics.py
+-rw-r--r--   0        0        0    22480 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/room_acoustics/room_acoustics.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/transfer_functions/__init__.py
+-rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/transfer_functions/_transfer_functions.py
+-rw-r--r--   0        0        0    63906 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/transfer_functions/transfer_functions.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/transforms/__init__.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/transforms/_transforms.py
+-rw-r--r--   0        0        0    30334 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/dsptoolbox/transforms/transforms.py
+-rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/audio_io_module.ipynb
+-rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/beamforming_module.ipynb
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/distances_module.ipynb
+-rw-r--r--   0        0        0   409017 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/filterbanks_module.ipynb
+-rw-r--r--   0        0        0  1013477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/general.ipynb
+-rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/generators_module.ipynb
+-rw-r--r--   0        0        0   180489 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/room_acoustics_module.ipynb
+-rw-r--r--   0        0        0    94731 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/standard_module.ipynb
+-rw-r--r--   0        0        0   208870 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/transfer_function_module.ipynb
+-rw-r--r--   0        0        0  1248737 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/transforms_module.ipynb
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/array.xml
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/chirp.wav
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/chirp_mono.wav
+-rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/chirp_stereo.wav
+-rw-r--r--   0        0        0  1766444 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/fuer_elise.wav
+-rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/rir.wav
+-rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/examples/data/speech.flac
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_audio_io.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_beamforming.py
+-rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_classes.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_distances.py
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_filterbanks.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_fx.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_generators.py
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_room_acoustics.py
+-rw-r--r--   0        0        0    12211 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_standard.py
+-rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_transfer_functions.py
+-rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/tests/test_transforms.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/README.rst
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dsptoolbox-0.3.8/PKG-INFO
```

### Comparing `dsptoolbox-0.3.7/.readthedocs.yaml` & `dsptoolbox-0.3.8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/CHANGELOG.rst` & `dsptoolbox-0.3.8/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,30 @@
 
 `To Do's for future releases`_
 ------------------------------
 
 - Validation for results from tests in every module (so far many tests are
   only regarding functionality)
 
+`0.3.8 <https://pypi.org/project/dsptoolbox/0.3.8>`_ - 
+---------------------
+
+Misc
+~~~~~~~
+- renamed paramater `remove_impulse_delay` to `remove_ir_latency`
+- changed default values in `PhaseLinearizer`
+- general documentation improvements
+
+Bugfix
+~~~~~~
+- `find_ir_latency` now searches for the latency in comparison to the minimum
+  phase ir
+- `harmonic_distortion_analysis` was fixed so that it can succesfully trim
+  the fundamental ir
+
 `0.3.7 <https://pypi.org/project/dsptoolbox/0.3.7>`_ - 
 ---------------------
 
 Misc
 ~~~~~~~
 - `trim_rir` has an improved approach where users do not need to set any
   parameters. It was also migrated to the ``transfer_functions`` module
```

### Comparing `dsptoolbox-0.3.7/docs/Makefile` & `dsptoolbox-0.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/classes.rst` & `dsptoolbox-0.3.8/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/conf.py` & `dsptoolbox-0.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/index.rst` & `dsptoolbox-0.3.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/make.bat` & `dsptoolbox-0.3.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/modules.rst` & `dsptoolbox-0.3.8/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/readme.rst` & `dsptoolbox-0.3.8/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/logo/logo.png` & `dsptoolbox-0.3.8/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/docs/logo/logo2.png` & `dsptoolbox-0.3.8/docs/logo/logo2.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
     "filterbanks",
     "transforms",
     "audio_io",
     "beamforming",
     "effects",
 ]
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/_general_helpers.py` & `dsptoolbox-0.3.8/dsptoolbox/_general_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """
 General functionality from helper methods
 """
 
 import numpy as np
-from scipy.signal import windows, convolve as scipy_convolve, hilbert
+from scipy.signal import (
+    windows,
+    convolve as scipy_convolve,
+    hilbert,
+    correlate,
+)
 from scipy.interpolate import interp1d
 from scipy.linalg import toeplitz as toeplitz_scipy
 from os import sep
 from warnings import warn
 
 
 def _find_nearest(points, vector) -> np.ndarray:
@@ -1231,15 +1236,15 @@
             latency_samples[ch] = delay_samples[ch] + int(move_back_one_sample)
             continue
 
         latency_samples[ch] = delay_samples[ch] + fractional_delay_samples
     return latency_samples + start_offset
 
 
-def _remove_impulse_delay_from_phase(
+def _remove_ir_latency_from_phase(
     freqs: np.ndarray,
     phase: np.ndarray,
     time_data: np.ndarray,
     sampling_rate_hz: int,
 ):
     """
     Remove the impulse delay from a phase response.
@@ -1257,9 +1262,116 @@
 
     Returns
     -------
     new_phase : `np.ndarray`
         New phase response without impulse delay.
 
     """
-    delays_s = _get_fractional_impulse_peak_index(time_data) / sampling_rate_hz
+    min_ir = _min_phase_ir_from_real_cepstrum(time_data)
+    delays_s = _fractional_latency(time_data, min_ir) / sampling_rate_hz
     return _wrap_phase(phase + 2 * np.pi * freqs[:, None] * delays_s[None, :])
+
+
+def _min_phase_ir_from_real_cepstrum(time_data: np.ndarray):
+    """Returns minimum-phase version of a time series using the real cepstrum
+    method.
+
+    Parameters
+    ----------
+    time_data : `np.ndarray`
+        Time series to compute the minimum phase version from. It is assumed
+        to have shape (time samples, channels).
+
+    Returns
+    -------
+    min_phase_time_data : `np.ndarray`
+        New time series.
+
+    """
+    return np.real(
+        np.fft.ifft(
+            _get_minimum_phase_spectrum_from_real_cepstrum(time_data), axis=0
+        )
+    )
+
+
+def _get_minimum_phase_spectrum_from_real_cepstrum(time_data: np.ndarray):
+    """Returns minimum-phase version of a time series using the real cepstrum
+    method.
+
+    Parameters
+    ----------
+    time_data : `np.ndarray`
+        Time series to compute the minimum phase version from. It is assumed
+        to have shape (time samples, channels).
+
+    Returns
+    -------
+    `np.ndarray`
+        New spectrum with minimum phase.
+
+    """
+    # Real cepstrum
+    y = np.real(
+        np.fft.ifft(np.log(np.abs(np.fft.fft(time_data, axis=0))), axis=0)
+    )
+
+    # Window in the cepstral domain, like obtaining hilbert transform
+    w = np.zeros(y.shape[0])
+    w[0] = 1
+    w[: len(w) // 2 - 1] = 2
+    # If length is even, nyquist is exactly in the middle
+    if len(w) % 2 == 0:
+        w[len(w) // 2] = 1
+
+    # Windowing in cepstral domain and back to spectral domain
+    return np.exp(np.fft.fft(y * w[..., None], axis=0))
+
+
+def _fractional_latency(
+    td1: np.ndarray, td2: np.ndarray | None = None, polynomial_points: int = 1
+):
+    """This function computes the sub-sample latency between two signals using
+    Zero-Crossing of the analytic (hilbert transformed) correlation function.
+    The number of polynomial points taken around the correlation maximum can be
+    set, although some polynomial orders might fail to compute the root. In
+    that case, integer latency will be returned for the respective channel.
+
+    Parameters
+    ----------
+    td1 : `np.ndaray`
+        Delayed version of the signal.
+    td2 : `np.ndarray`, optional
+        Original version of the signal. If `None` is passed, the latencies
+        are computed between the first channel of td1 and every other.
+        Default: `None`.
+    polynomial_points : int, optional
+        This corresponds to the number of points taken around the root in order
+        to fit a polynomial. Accuracy might improve with higher orders but
+        it could also lead to ill-conditioned polynomials. In case root finding
+        is not successful, integer latency values are returned. Default: 1.
+
+    Returns
+    -------
+    lags : `np.ndarray`
+        Fractional delays. It has shape (channel). In case td2 was `None`, its
+        length is `channels - 1`.
+
+    References
+    ----------
+    - N. S. M. Tamim and F. Ghani, "Hilbert transform of FFT pruned cross
+      correlation function for optimization in time delay estimation," 2009
+      IEEE 9th Malaysia International Conference on Communications (MICC),
+      Kuala Lumpur, Malaysia, 2009, pp. 809-814,
+      doi: 10.1109/MICC.2009.5431382.
+
+    """
+    if td2 is None:
+        td2 = td1[:, 0][..., None]
+        td1 = np.atleast_2d(td1[:, 1:])
+        xcor = correlate(td2, td1)
+    else:
+        xcor = np.zeros((td1.shape[0] + td2.shape[0] - 1, td2.shape[1]))
+        for i in range(td2.shape[1]):
+            xcor[:, i] = correlate(td2[:, i], td1[:, i])
+    inds = _get_fractional_impulse_peak_index(xcor, polynomial_points)
+    return td1.shape[0] - inds - 1
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/_standard.py` & `dsptoolbox-0.3.8/dsptoolbox/_standard.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import numpy as np
 from scipy.signal import correlate, check_COLA, windows, hilbert, convolve
 from scipy.special import iv as bessel_first_mod
 from ._general_helpers import (
     _pad_trim,
     _compute_number_frames,
-    _get_fractional_impulse_peak_index,
     _wrap_phase,
 )
 from warnings import warn
 
 
 def _latency(
     in1: np.ndarray, in2: np.ndarray | None = None, polynomial_points: int = 0
@@ -31,64 +30,14 @@
         peak_inds = np.zeros(in1.shape[1], dtype=int)
         for i in range(in1.shape[1]):
             xcorr = correlate(in2[:, i].flatten(), in1[:, i].flatten())
             peak_inds[i] = int(np.argmax(np.abs(xcorr)))
     return in1.shape[0] - peak_inds - 1
 
 
-def _fractional_latency(
-    td1: np.ndarray, td2: np.ndarray | None = None, polynomial_points: int = 1
-):
-    """This function computes the sub-sample latency between two signals using
-    Zero-Crossing of the analytic (hilbert transformed) correlation function.
-    The number of polynomial points taken around the correlation maximum can be
-    set, although some polynomial orders might fail to compute the root. In
-    that case, integer latency will be returned for the respective channel.
-
-    Parameters
-    ----------
-    td1 : `np.ndaray`
-        Delayed version of the signal.
-    td2 : `np.ndarray`, optional
-        Original version of the signal. If `None` is passed, the latencies
-        are computed between the first channel of td1 and every other.
-        Default: `None`.
-    polynomial_points : int, optional
-        This corresponds to the number of points taken around the root in order
-        to fit a polynomial. Accuracy might improve with higher orders but
-        it could also lead to ill-conditioned polynomials. In case root finding
-        is not successful, integer latency values are returned. Default: 1.
-
-    Returns
-    -------
-    lags : `np.ndarray`
-        Fractional delays. It has shape (channel). In case td2 was `None`, its
-        length is `channels - 1`.
-
-    References
-    ----------
-    - N. S. M. Tamim and F. Ghani, "Hilbert transform of FFT pruned cross
-      correlation function for optimization in time delay estimation," 2009
-      IEEE 9th Malaysia International Conference on Communications (MICC),
-      Kuala Lumpur, Malaysia, 2009, pp. 809-814,
-      doi: 10.1109/MICC.2009.5431382.
-
-    """
-    if td2 is None:
-        td2 = td1[:, 0][..., None]
-        td1 = np.atleast_2d(td1[:, 1:])
-        xcor = correlate(td2, td1)
-    else:
-        xcor = np.zeros((td1.shape[0] + td2.shape[0] - 1, td2.shape[1]))
-        for i in range(td2.shape[1]):
-            xcor[:, i] = correlate(td2[:, i], td1[:, i])
-    inds = _get_fractional_impulse_peak_index(xcor, polynomial_points)
-    return td1.shape[0] - inds - 1
-
-
 def _welch(
     x: np.ndarray,
     y: np.ndarray | None,
     fs_hz: int,
     window_type: str = "hann",
     window_length_samples: int = 1024,
     overlap_percent=50,
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/standard_functions.py` & `dsptoolbox-0.3.8/dsptoolbox/standard_functions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     _latency,
     _center_frequencies_fractional_octaves_iec,
     _exact_center_frequencies_fractional_octaves,
     # _kaiser_window_beta,
     _indices_above_threshold_dbfs,
     _detrend,
     _rms,
-    _fractional_latency,
     _fractional_delay_filter,
 )
 from ._general_helpers import (
     _pad_trim,
     _normalize,
     _fade,
     _check_format_in_path,
     _get_smoothing_factor_ema,
+    _fractional_latency,
 )
 
 
 def latency(
     in1: Signal | MultiBandSignal,
     in2: Signal | MultiBandSignal | None = None,
     polynomial_points: int = 0,
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/audio_io/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/audio_io/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/audio_io/_audio_io.py` & `dsptoolbox-0.3.8/dsptoolbox/audio_io/_audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/audio_io/audio_io.py` & `dsptoolbox-0.3.8/dsptoolbox/audio_io/audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/beamforming/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/beamforming/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/beamforming/_beamforming.py` & `dsptoolbox-0.3.8/dsptoolbox/beamforming/_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/beamforming/beamforming.py` & `dsptoolbox-0.3.8/dsptoolbox/beamforming/beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/_filter.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/_lattice_ladder_filter.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/_lattice_ladder_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/_phaseLinearizer.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/_phaseLinearizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,30 +78,30 @@
             target_group_delay
         ), f"Target group delay shape {target_group_delay.shape} is invalid"
         self.target_group_delay = target_group_delay
 
     def set_parameters(
         self,
         delay_increase_percent: float = 100.0,
-        total_length_factor: float = 1.5,
+        total_length_factor: float = 1.0,
     ):
         """Set parameters for the FIR filter.
 
         Parameters
         ----------
         delay_increase_percent : float, optional
             This is the increase (in percentage) in delay to the current
             maximum group delay of the phase response. Increasing this improves
             the quality of the designed filter but also makes it longer.
             Passing a value of 100 means that the total group delay will be
             2 times larger than the longest group delay in the phase response.
             Default: 100.
         total_length_factor : float, optional
             The total length of the filter is based on the longest group delay.
-            This factor can augment it. Default: 1.5.
+            This factor can augment it. Default: 1.
 
         Notes
         -----
         - If there is a target group delay, no increase is applied by
           `delay_increase_percent`, but `total_length_factor` is still used
           for the output filter.
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/_plots.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/_plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/_svfilter.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/_svfilter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/filter_class.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/filter_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
             `'ba'` or `'zpk'`. Default: `'sos'`.
 
         Returns
         -------
         coefficients : array-like
             Array with filter coefficients with shape depending on mode:
             - `'ba'`: list(b, a) with b and a of type `np.ndarray`.
-            - `'sos'`: `np.ndarray`
+            - `'sos'`: `np.ndarray` with shape (n_sections, 6).
             - `'zpk'`: tuple(z, p, k) with z, p, k of type `np.ndarray`
             - Return `None` if user decides that ba->sos is too costly. The
               threshold is for filters with order > 500.
 
         """
         if mode == "sos":
             if hasattr(self, "sos"):
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/filterbank.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/multibandsignal.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/multibandsignal.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/classes/signal_class.py` & `dsptoolbox-0.3.8/dsptoolbox/classes/signal_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     _get_normalized_spectrum,
     _pad_trim,
     _find_nearest,
     _fractional_octave_smoothing,
     _check_format_in_path,
     _scale_spectrum,
     _wrap_phase,
-    _remove_impulse_delay_from_phase,
+    _remove_ir_latency_from_phase,
 )
 from .._standard import _welch, _group_delay_direct, _stft, _csm
 
 
 class Signal:
     """Class for general signals (time series). Most of the methods and
     supported computations are focused on audio signals, but some features
@@ -1014,22 +1014,22 @@
             info_box=txt,
             returns=True,
             labels=[f"Channel {n}" for n in range(self.number_of_channels)],
             range_y=range_db,
         )
         return fig, ax
 
-    def plot_time(self) -> tuple[Figure, Axes]:
+    def plot_time(self) -> tuple[Figure, list[Axes]]:
         """Plots time signals.
 
         Returns
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
-        ax : `matplotlib.axes.Axes`
+        ax : list of `matplotlib.axes.Axes`
             Axes.
 
         """
         if not hasattr(self, "time_vector_s"):
             self._generate_time_vector()
         fig, ax = general_subplots_line(
             self.time_vector_s,
@@ -1061,15 +1061,15 @@
         return fig, ax
 
     def plot_spl(
         self,
         normalize_at_peak: bool = False,
         range_db: float | None = 100.0,
         window_length_s: float = 0.0,
-    ) -> tuple[Figure, Axes]:
+    ) -> tuple[Figure, list[Axes]]:
         """Plots the momentary sound pressure level (dB or dBFS) of each
         channel. If the signal is calibrated and not normalized at peak, the
         values correspond to dB, otherwise they are dBFS.
 
         Parameters
         ----------
         normalize_at_peak : bool, optional
@@ -1083,15 +1083,15 @@
             When different than 0, a moving average along the time axis is done
             with the given length. Default: 0.
 
         Returns
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
-        ax : `matplotlib.axes.Axes`
+        ax : list of `matplotlib.axes.Axes`
             Axes.
 
         Notes
         -----
         - All values are clipped to be at least -800 dBFS.
         - If it is an analytic signal and normalization is applied, the peak
           value of the real part is used as the normalization factor.
@@ -1187,27 +1187,27 @@
                     [max_values[n] - np.abs(range_db), max_values[n]]
                 )
         return fig, ax
 
     def plot_group_delay(
         self,
         range_hz=[20, 20000],
-        remove_impulse_delay: bool = False,
+        remove_ir_latency: bool = False,
         smoothing: int = 0,
     ) -> tuple[Figure, Axes]:
         """Plots group delay of each channel.
         Only works if `signal_type in ('ir', 'h1', 'h2', 'h3', 'rir', 'chirp',
         'noise', 'dirac')`.
 
         Parameters
         ----------
         range_hz : array-like with length 2, optional
             Range of frequencies for which to show group delay.
             Default: [20, 20e3].
-        remove_impulse_delay : bool, optional
+        remove_ir_latency : bool, optional
             When `True`, the delay of the impulse is removed prior to the
             computation of the group delay. Default: `False`.
         smoothing : int, optional
             When different than 0, smoothing is applied to the group delay
             along the (1/smoothing) octave band. This only affects the values
             in the plot. Default: 0.
 
@@ -1237,16 +1237,16 @@
         # Handle spectrum parameters
         prior_spectrum_parameters = self._spectrum_parameters
         self.set_spectrum_parameters("standard", scaling=None, smoothe=0)
         f, sp = self.get_spectrum()
         self._spectrum_parameters = prior_spectrum_parameters
 
         sp = np.angle(sp)
-        if remove_impulse_delay:
-            sp = _remove_impulse_delay_from_phase(
+        if remove_ir_latency:
+            sp = _remove_ir_latency_from_phase(
                 f, sp, self.time_data, self.sampling_rate_hz
             )
 
         gd = np.zeros((len(f), self.number_of_channels))
         for n in range(self.number_of_channels):
             gd[:, n] = _group_delay_direct(sp[:, n], f[1] - f[0])
 
@@ -1333,22 +1333,22 @@
             xlog=False,
             ylog=logfreqs,
             colorbar=True,
             returns=True,
         )
         return fig, ax
 
-    def plot_coherence(self) -> tuple[Figure, Axes]:
+    def plot_coherence(self) -> tuple[Figure, list[Axes]]:
         """Plots coherence measurements if there are any.
 
         Returns
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
-        ax : `matplotlib.axes.Axes`
+        ax : list of `matplotlib.axes.Axes`
             Axes.
 
         """
         if not hasattr(self, "coherence"):
             raise AttributeError("There is no coherence data saved")
         f, coh = self.get_coherence()
         fig, ax = general_subplots_line(
@@ -1368,15 +1368,15 @@
         return fig, ax
 
     def plot_phase(
         self,
         range_hz=[20, 20e3],
         unwrap: bool = False,
         smoothing: int = 0,
-        remove_impulse_delay: bool = False,
+        remove_ir_latency: bool = False,
     ) -> tuple[Figure, Axes]:
         """Plots phase of the frequency response, only available if the method
         for the spectrum `"standard"`.
 
         Parameters
         ----------
         range_hz : array-like with length 2, optional
@@ -1384,15 +1384,15 @@
             Default: [20, 20e3].
         unwrap : bool, optional
             When `True`, the unwrapped phase is plotted. Default: `False`.
         smoothing : int, optional
             When different than 0, the phase response is smoothed across the
             1/smoothing-octave band. This only applies smoothing to the plot
             data. Default: 0.
-        remove_impulse_delay : bool, optional
+        remove_ir_latency : bool, optional
             If the signal is of type `"rir"` or `"ir"`, the delay of the
             impulse can be removed. Default: `False`.
 
         Returns
         -------
         fig : `matplotlib.figure.Figure`
             Figure.
@@ -1411,20 +1411,20 @@
 
         # Get spectrum
         f, sp = self.get_spectrum()
         ph = np.angle(sp)
 
         self._spectrum_parameters["smoothe"] = prior_smoothing
 
-        if remove_impulse_delay:
+        if remove_ir_latency:
             assert self.signal_type in (
                 "rir",
                 "ir",
             ), f"{self.signal_type} is not valid, use rir or ir"
-            ph = _remove_impulse_delay_from_phase(
+            ph = _remove_ir_latency_from_phase(
                 f, ph, self.time_data, self.sampling_rate_hz
             )
 
         if smoothing != 0:
             ph = _wrap_phase(
                 _fractional_octave_smoothing(np.unwrap(ph, axis=0), smoothing)
             )
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/distances/_distances.py` & `dsptoolbox-0.3.8/dsptoolbox/distances/_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/distances/distances.py` & `dsptoolbox-0.3.8/dsptoolbox/distances/distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/effects/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/effects/_effects.py` & `dsptoolbox-0.3.8/dsptoolbox/effects/_effects.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/effects/effects.py` & `dsptoolbox-0.3.8/dsptoolbox/effects/effects.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/filterbanks/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/filterbanks/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/filterbanks/_filterbank.py` & `dsptoolbox-0.3.8/dsptoolbox/filterbanks/_filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/filterbanks/filterbanks.py` & `dsptoolbox-0.3.8/dsptoolbox/filterbanks/filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/generators/generators.py` & `dsptoolbox-0.3.8/dsptoolbox/generators/generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/plots/plots.py` & `dsptoolbox-0.3.8/dsptoolbox/plots/plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/room_acoustics/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/room_acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/room_acoustics/_room_acoustics.py` & `dsptoolbox-0.3.8/dsptoolbox/room_acoustics/_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/room_acoustics/room_acoustics.py` & `dsptoolbox-0.3.8/dsptoolbox/room_acoustics/room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/transfer_functions/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/transfer_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/transfer_functions/_transfer_functions.py` & `dsptoolbox-0.3.8/dsptoolbox/transfer_functions/_transfer_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -156,70 +156,14 @@
     else:
         vec = np.pad(vec, ((0, padding_after_adaptation)))
         window = np.pad(window, ((0, padding_after_adaptation)))
 
     return vec * window, window, start_sample
 
 
-def _min_phase_ir_from_real_cepstrum(time_data: np.ndarray):
-    """Returns minimum-phase version of a time series using the real cepstrum
-    method.
-
-    Parameters
-    ----------
-    time_data : `np.ndarray`
-        Time series to compute the minimum phase version from. It is assumed
-        to have shape (time samples, channels).
-
-    Returns
-    -------
-    min_phase_time_data : `np.ndarray`
-        New time series.
-
-    """
-    return np.real(
-        np.fft.ifft(
-            _get_minimum_phase_spectrum_from_real_cepstrum(time_data), axis=0
-        )
-    )
-
-
-def _get_minimum_phase_spectrum_from_real_cepstrum(time_data: np.ndarray):
-    """Returns minimum-phase version of a time series using the real cepstrum
-    method.
-
-    Parameters
-    ----------
-    time_data : `np.ndarray`
-        Time series to compute the minimum phase version from. It is assumed
-        to have shape (time samples, channels).
-
-    Returns
-    -------
-    `np.ndarray`
-        New spectrum with minimum phase.
-
-    """
-    # Real cepstrum
-    y = np.real(
-        np.fft.ifft(np.log(np.abs(np.fft.fft(time_data, axis=0))), axis=0)
-    )
-
-    # Window in the cepstral domain, like obtaining hilbert transform
-    w = np.zeros(y.shape[0])
-    w[0] = 1
-    w[: len(w) // 2 - 1] = 2
-    # If length is even, nyquist is exactly in the middle
-    if len(w) % 2 == 0:
-        w[len(w) // 2] = 1
-
-    # Windowing in cepstral domain and back to spectral domain
-    return np.exp(np.fft.fft(y * w[..., None], axis=0))
-
-
 def _window_this_ir(
     vec, total_length: int, window_type: str = "hann", window_parameter=None
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """This function windows an impulse response by placing the peak exactly
     in the middle of the window. It trims or pads at the end if needed. The
     windowed IR, window and the start sample are passed.
 
@@ -325,28 +269,28 @@
         if n in ns:
             print(f"Warped: {(ns.pop(0) / td.shape[0] * 100):.0f}% of signal")
     return warped_td
 
 
 def _get_harmonic_times(
     chirp_range_hz: list,
-    chirp_length_seconds: float,
+    chirp_length_s: float,
     n_harmonics: int,
     time_offset_seconds: float = 0.0,
 ) -> np.ndarray:
     """Get the time at which each harmonic IR occur relative to the fundamental
     IR in a measurement with an exponential chirp. This is computed according
     to [1]. If the fundamental happens at time `t=0`, all harmonics will be at
     a negative time.
 
     Parameters
     ----------
     chirp_range_hz : list of length 2
         The frequency range of the chirp.
-    chirp_length_seconds : float
+    chirp_length_s : float
         Length of chirp in seconds (without zero-padding).
     n_harmonics : int
         Number of harmonics to analyze.
     time_offset_seconds : float, optional
         Time at which the fundamental occurs. Default: 0.
 
     Returns
@@ -356,15 +300,15 @@
         are given in seconds.
 
     References
     ----------
     - [1]: Weinzierl, S. Handbuch der Audiotechnik. Chapter 21.
 
     """
-    rate = _get_chirp_rate(chirp_range_hz, chirp_length_seconds)
+    rate = _get_chirp_rate(chirp_range_hz, chirp_length_s)
     return time_offset_seconds - np.log2(np.arange(n_harmonics) + 2) / rate
 
 
 def _trim_ir(
     time_data: np.ndarray,
     fs_hz: int,
     offset_start_s: float,
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/transfer_functions/transfer_functions.py` & `dsptoolbox-0.3.8/dsptoolbox/transfer_functions/transfer_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,41 @@
 from scipy.fft import rfft as rfft_scipy, next_fast_len as next_fast_length_fft
 from scipy.interpolate import interp1d
 
 from ._transfer_functions import (
     _spectral_deconvolve,
     _window_this_ir_tukey,
     _window_this_ir,
-    _min_phase_ir_from_real_cepstrum,
-    _get_minimum_phase_spectrum_from_real_cepstrum,
     _warp_time_series,
     _get_harmonic_times,
     _trim_ir,
 )
 from ..classes import Signal, Filter
 from ..classes._filter import _group_delay_filter
 from .._general_helpers import (
-    _remove_impulse_delay_from_phase,
+    _remove_ir_latency_from_phase,
+    _min_phase_ir_from_real_cepstrum,
+    _get_minimum_phase_spectrum_from_real_cepstrum,
     _find_frequencies_above_threshold,
     _fractional_octave_smoothing,
     _correct_for_real_phase_spectrum,
     _wrap_phase,
-    _get_fractional_impulse_peak_index,
 )
 from .._standard import (
     _welch,
     _minimum_phase,
     _group_delay_direct,
     _pad_trim,
 )
-from ..standard_functions import fractional_delay, merge_signals, normalize
+from ..standard_functions import (
+    fractional_delay,
+    merge_signals,
+    normalize,
+    latency,
+)
 from ..generators import dirac
 from ..filterbanks import linkwitz_riley_crossovers
 from ..room_acoustics._room_acoustics import _find_ir_start
 
 
 def spectral_deconvolve(
     num: Signal,
@@ -235,14 +239,17 @@
       parts of the window are set to 0 in order to make them visible.
 
     """
     assert signal.signal_type in (
         "rir",
         "ir",
     ), f"{signal.signal_type} is not a valid signal type. Use rir or ir."
+    assert (
+        constant_percentage < 1 and constant_percentage >= 0
+    ), "Constant percentage can not be larger than 1 or smaller than 0"
     assert offset_samples >= 0, "Offset must be positive"
     assert offset_samples <= constant_percentage * total_length_samples, (
         "Offset is too large for the constant part of the window and its "
         + "total length"
     )
     assert (
         left_to_right_flank_length_ratio >= 0
@@ -788,15 +795,15 @@
     return min_phase_sig
 
 
 def group_delay(
     signal: Signal,
     method="matlab",
     smoothing: int = 0,
-    remove_impulse_delay: bool = False,
+    remove_ir_latency: bool = False,
 ) -> tuple[np.ndarray, np.ndarray]:
     """Computes and returns group delay.
 
     Parameters
     ----------
     signal : `Signal`
         Signal for which to compute group delay.
@@ -804,15 +811,15 @@
         `'direct'` uses gradient with unwrapped phase. `'matlab'` uses
         this implementation:
         https://www.dsprelated.com/freebooks/filters/Phase_Group_Delay.html.
         Default: `'matlab'`.
     smoothing : int, optional
         Octave fraction by which to apply smoothing. `0` avoids any smoothing
         of the group delay. Default: `0`.
-    remove_impulse_delay : bool, optional
+    remove_ir_latency : bool, optional
         If the signal is of type `"ir"` or `"rir"`, the impulse delay can be
         removed. Default: `False`.
 
     Returns
     -------
     freqs : `np.ndarray`
         Frequency vector in Hz.
@@ -829,38 +836,38 @@
     if method == "direct":
         spec_parameters = signal._spectrum_parameters
         signal.set_spectrum_parameters("standard")
         f, sp = signal.get_spectrum()
         signal._spectrum_parameters = spec_parameters
         group_delays = np.zeros((sp.shape[0], sp.shape[1]))
 
-        if remove_impulse_delay:
+        if remove_ir_latency:
             assert signal.signal_type in (
                 "rir",
                 "ir",
             ), (
                 f"{signal.signal_type} is not a valid signal type. Use ir "
                 + "or rir"
             )
-            sp = _remove_impulse_delay_from_phase(
+            sp = _remove_ir_latency_from_phase(
                 f, np.angle(sp), signal.time_data, signal.sampling_rate_hz
             )
         for n in range(signal.number_of_channels):
             group_delays[:, n] = _group_delay_direct(sp[:, n], f[1] - f[0])
     else:
         group_delays = np.zeros(
             (signal.time_data.shape[0] // 2 + 1, signal.time_data.shape[1])
         )
         f = np.fft.rfftfreq(
             signal.time_data.shape[0], 1 / signal.sampling_rate_hz
         )
 
         for n in range(signal.number_of_channels):
             b = signal.time_data[:, n]
-            if remove_impulse_delay:
+            if remove_ir_latency:
                 b = b[max(int(np.argmax(np.abs(b))) - 1, 0) :]
             a = [1]
             _, group_delays[:, n] = _group_delay_filter(
                 [b, a], len(f), signal.sampling_rate_hz
             )
 
     if smoothing != 0:
@@ -984,29 +991,29 @@
     return f, min_gd
 
 
 def excess_group_delay(
     signal: Signal,
     method: str = "real cepstrum",
     smoothing: int = 0,
-    remove_impulse_delay: bool = False,
+    remove_ir_latency: bool = False,
 ) -> tuple[np.ndarray, np.ndarray]:
     """Computes excess group delay of an IR.
 
     Parameters
     ----------
     signal : `Signal`
         IR for which to compute minimal group delay.
     method : str, optional
         Select method for computing the minimum phase. It might be either
         `'real cepstrum'` or `'log hilbert'`. Default: `'real cepstrum'`.
     smoothing : int, optional
         Octave fraction by which to apply smoothing. `0` avoids any smoothing
         of the group delay. Default: `0`.
-    remove_impulse_delay : bool, optional
+    remove_ir_latency : bool, optional
         If the signal is of type `"ir"` or `"rir"`, the impulse delay can be
         removed. Default: `False`.
 
     Returns
     -------
     f : `np.ndarray`
         Frequency vector.
@@ -1020,15 +1027,15 @@
     """
     assert signal.signal_type in ("rir", "ir"), "Only valid for rir or ir"
     f, min_gd = minimum_group_delay(signal, method, smoothing=0)
     f, gd = group_delay(
         signal,
         smoothing=0,
         method="direct",
-        remove_impulse_delay=remove_impulse_delay,
+        remove_ir_latency=remove_ir_latency,
     )
     ex_gd = gd - min_gd
 
     if smoothing != 0:
         ex_gd = _fractional_octave_smoothing(ex_gd, smoothing)
 
     return f, ex_gd
@@ -1444,51 +1451,51 @@
 
     f_unwarped = ir.sampling_rate_hz / 2 / np.pi * np.arccos(warping_factor)
 
     return f_unwarped, warped_ir
 
 
 def find_ir_latency(ir: Signal) -> np.ndarray:
-    """Find the subsample maximum of each channel of the IR using the root of
-    the analytical function. This value can be associated with the latency
-    of the impulse response.
+    """Find the subsample maximum of each channel of the IR using the its
+    minimum phase equivalent.
 
     Parameters
     ----------
     ir : `Signal`
         Impulse response to find the maximum.
 
     Returns
     -------
     latency_samples : `np.ndarray`
         Array with the position of each channel's maximum in samples.
 
     """
     assert ir.signal_type in ("rir", "ir"), "Only valid for rir or ir"
-    return _get_fractional_impulse_peak_index(ir.time_data)
+    min_ir = min_phase_ir(ir)
+    return latency(ir, min_ir, 1)
 
 
 def harmonics_from_chirp_ir(
     ir: Signal,
     chirp_range_hz: list,
-    chirp_length_seconds: float,
+    chirp_length_s: float,
     n_harmonics: int = 5,
     offset_percentage: float = 0.05,
 ) -> list[Signal]:
     """Get the individual harmonics (distortion) IRs of an IR computed with
     an exponential chirp.
 
     Parameters
     ----------
     ir : `Signal`
         Impulse response obtained through deconvolution with an exponential
         chirp.
     chirp_range_hz : list of length 2
         The frequency range of the chirp.
-    chirp_length_seconds : float
+    chirp_length_s : float
         Length of chirp in seconds (without zero-padding).
     n_harmonics : int, optional
         Number of harmonics to analyze. Default: 5.
     offset_percentage : float, optional
         When this is larger than zero, each IR will also contain some samples
         prior to the impulse. Their amount corresponds to a percentage of the
         time length between that harmonic and their adjacent ones.
@@ -1521,17 +1528,15 @@
 
     # Get offsets
     td = ir.time_data
     offsets = -np.argmax(np.abs(td), axis=0) + 1
     td = np.roll(td, offsets, axis=0)
 
     # Get times of each harmonic
-    ts = _get_harmonic_times(
-        chirp_range_hz, chirp_length_seconds, n_harmonics + 1
-    )
+    ts = _get_harmonic_times(chirp_range_hz, chirp_length_s, n_harmonics + 1)
     time_harmonics_samples = len(td) + (ts * ir.sampling_rate_hz + 0.5).astype(
         int
     )
 
     time_harmonics_samples = np.insert(time_harmonics_samples, 0, len(td))
 
     # Dummy to obtain all metadata of the IR
@@ -1632,29 +1637,36 @@
 
         harm = ir
         n_harmonics = len(harm)
         if chirp_range_hz is None:
             chirp_range_hz = [0, ir2.sampling_rate_hz // 2]
 
         passed_harmonics = True
-
     elif type(ir) is Signal:
+        assert (
+            chirp_length_s is not None
+            and chirp_range_hz is not None
+            and n_harmonics is not None
+        ), "Chirp parameters and number of harmonics cannot be None"
+
         # Get different harmonics
         harm = harmonics_from_chirp_ir(
             ir, chirp_range_hz, chirp_length_s, n_harmonics, 0.01
         )
 
-        passed_harmonics = False
-
         # Trim and window IR
         ir2 = ir.copy()
-        start, stop, _ = _trim_ir(ir2.time_data, ir.sampling_rate_hz, 10e-3)
+        start, stop, _ = _trim_ir(
+            ir2.time_data[:, 0], ir.sampling_rate_hz, 10e-3
+        )
         ir2.time_data = ir2.time_data[start:stop]
         ir2 = window_ir(ir2, len(ir2), constant_percentage=0.9)[0]
         ir2._spectrum_parameters["smoothe"] = smoothing
+
+        passed_harmonics = False
     else:
         raise TypeError("Type for ir is not supported")
 
     # At least 5 Hz frequency resolution for base spectrum
     pad_length = max(ir2.sampling_rate_hz // 5, len(ir2)) - len(ir2)
     ir2.time_data = np.pad(ir2.time_data, ((0, pad_length), (0, 0)))
```

### Comparing `dsptoolbox-0.3.7/dsptoolbox/transforms/__init__.py` & `dsptoolbox-0.3.8/dsptoolbox/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/transforms/_transforms.py` & `dsptoolbox-0.3.8/dsptoolbox/transforms/_transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/dsptoolbox/transforms/transforms.py` & `dsptoolbox-0.3.8/dsptoolbox/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/audio_io_module.ipynb` & `dsptoolbox-0.3.8/examples/audio_io_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/beamforming_module.ipynb` & `dsptoolbox-0.3.8/examples/beamforming_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/distances_module.ipynb` & `dsptoolbox-0.3.8/examples/distances_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/filterbanks_module.ipynb` & `dsptoolbox-0.3.8/examples/filterbanks_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/general.ipynb` & `dsptoolbox-0.3.8/examples/general.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/generators_module.ipynb` & `dsptoolbox-0.3.8/examples/generators_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/room_acoustics_module.ipynb` & `dsptoolbox-0.3.8/examples/room_acoustics_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/standard_module.ipynb` & `dsptoolbox-0.3.8/examples/standard_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/transfer_function_module.ipynb` & `dsptoolbox-0.3.8/examples/transfer_function_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/transforms_module.ipynb` & `dsptoolbox-0.3.8/examples/transforms_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/array.xml` & `dsptoolbox-0.3.8/examples/data/array.xml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/chirp.wav` & `dsptoolbox-0.3.8/examples/data/chirp.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/chirp_mono.wav` & `dsptoolbox-0.3.8/examples/data/chirp_mono.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/chirp_stereo.wav` & `dsptoolbox-0.3.8/examples/data/chirp_stereo.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/fuer_elise.wav` & `dsptoolbox-0.3.8/examples/data/fuer_elise.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/rir.wav` & `dsptoolbox-0.3.8/examples/data/rir.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/examples/data/speech.flac` & `dsptoolbox-0.3.8/examples/data/speech.flac`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_beamforming.py` & `dsptoolbox-0.3.8/tests/test_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_classes.py` & `dsptoolbox-0.3.8/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_distances.py` & `dsptoolbox-0.3.8/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_filterbanks.py` & `dsptoolbox-0.3.8/tests/test_filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_fx.py` & `dsptoolbox-0.3.8/tests/test_fx.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_generators.py` & `dsptoolbox-0.3.8/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_room_acoustics.py` & `dsptoolbox-0.3.8/tests/test_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_standard.py` & `dsptoolbox-0.3.8/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/tests/test_transfer_functions.py` & `dsptoolbox-0.3.8/tests/test_transfer_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         # Check only that some result is produced, validity should be checked
         # somewhere else
         dsp.transfer_functions.group_delay(ir, method="matlab")
         dsp.transfer_functions.group_delay(ir, method="direct")
 
         dsp.transfer_functions.group_delay(ir, method="matlab", smoothing=4)
         dsp.transfer_functions.group_delay(
-            ir, method="direct", smoothing=4, remove_impulse_delay=True
+            ir, method="direct", smoothing=4, remove_ir_latency=True
         )
 
         # Single-channel plausibility check
         dsp.transfer_functions.group_delay(ir.get_channels(0))
 
     def test_minimum_phase(self):
         ir = dsp.transfer_functions.spectral_deconvolve(
@@ -425,15 +425,15 @@
             ir, 2**12, window_type="hann", at_start=True
         )
         # Check only that some result is produced, validity should be checked
         # somewhere else
         # Only works for some signal types
         dsp.transfer_functions.excess_group_delay(ir)
         dsp.transfer_functions.excess_group_delay(
-            ir, smoothing=3, remove_impulse_delay=True
+            ir, smoothing=3, remove_ir_latency=True
         )
         with pytest.raises(AssertionError):
             s1 = dsp.Signal(None, ir.time_data, ir.sampling_rate_hz)
             dsp.transfer_functions.excess_group_delay(s1)
         # Single-channel plausibility check
         dsp.transfer_functions.excess_group_delay(ir.get_channels(0))
 
@@ -460,14 +460,17 @@
         delay_seconds = 0.00133  # Some value to have a fractional delay
         delay_samples = self.fs * delay_seconds
         ir = dsp.fractional_delay(ir, delay_seconds)
         output = dsp.transfer_functions.find_ir_latency(ir).squeeze()
 
         assert np.isclose(delay_samples, output, atol=0.4)
 
+        ir = dsp.Signal(join("examples", "data", "rir.wav"), signal_type="rir")
+        assert dsp.transfer_functions.find_ir_latency(ir) > 0
+
     def test_window_frequency_dependent(self):
         s = dsp.Signal(join("examples", "data", "rir.wav"), signal_type="rir")
         f, sp = dsp.transfer_functions.window_frequency_dependent(
             s, 10, 0, [100, 1000]
         )
 
         fig, ax = s.plot_magnitude(normalize=None)
@@ -482,39 +485,39 @@
 
     def test_harmonics_from_chirp_ir(self):
         # Only functionality
         ir = dsp.Signal(join("examples", "data", "rir.wav"), signal_type="rir")
         dsp.transfer_functions.harmonics_from_chirp_ir(
             ir,
             chirp_range_hz=[20, 20e3],
-            chirp_length_seconds=2,
+            chirp_length_s=2,
             n_harmonics=2,
         )
 
     def test_harmonic_distortion_analysis(self):
         # Only functionality
         ir = dsp.Signal(join("examples", "data", "rir.wav"), signal_type="rir")
         dsp.transfer_functions.harmonic_distortion_analysis(
             ir,
             chirp_range_hz=[20, 20e3],
-            chirp_length_seconds=2,
+            chirp_length_s=2,
             n_harmonics=7,
         )
 
         harm = dsp.transfer_functions.harmonics_from_chirp_ir(
             ir,
             chirp_range_hz=[20, 20e3],
-            chirp_length_seconds=2,
+            chirp_length_s=2,
             n_harmonics=2,
         )
         harm.insert(0, dsp.transfer_functions.trim_ir(ir)[0])
         dsp.transfer_functions.harmonic_distortion_analysis(
             harm,
             chirp_range_hz=None,
-            chirp_length_seconds=None,
+            chirp_length_s=None,
             n_harmonics=None,
         )
 
     def test_trim_rir(self):
         # Only functionality
         ir = dsp.Signal(join("examples", "data", "rir.wav"), signal_type="rir")
         dsp.transfer_functions.trim_ir(ir)
```

### Comparing `dsptoolbox-0.3.7/tests/test_transforms.py` & `dsptoolbox-0.3.8/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/LICENSE` & `dsptoolbox-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/README.rst` & `dsptoolbox-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/pyproject.toml` & `dsptoolbox-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.7/PKG-INFO` & `dsptoolbox-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsptoolbox
-Version: 0.3.7
+Version: 0.3.8
 Summary: Collection of dsp algorithms to be used for analysis of audio signals
 Project-URL: Homepage, https://github.com/nico-franco-gomez/dsptoolbox
 Project-URL: Bug Tracker, https://github.com/nico-franco-gomez/dsptoolbox/issues
 Project-URL: Documentation, https://dsptoolbox.readthedocs.io/en/latest/
 Author: Nicolas Franco-Gomez
 License-Expression: MIT
 License-File: LICENSE
```

