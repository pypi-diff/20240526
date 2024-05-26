# Comparing `tmp/mimllearning-0.5.8.tar.gz` & `tmp/mimllearning-0.5.9.tar.gz`

## Comparing `mimllearning-0.5.8.tar` & `mimllearning-0.5.9.tar`

### file list

```diff
@@ -1,758 +1,758 @@
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.8/readme.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mimllearning-0.5.8/todo.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/Makefile
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/make.bat
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mi.all_positive_apr_classifier.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mi.apr_classifier.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mi.miles_classifier.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mi.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.miml_classifier.rst
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.classifier.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.data.bag.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.data.instance.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.data.miml_dataset.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.data.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.datasets.dataset_utils.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.datasets.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.report.report.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.report.rst
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOmi.label_powerset_transformation.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOml.arithmetic.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOml.geometric.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOml.minmax.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/api/miml.transformation.rst
--rw-r--r--   0        0        0   910561 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.doctree
--rw-r--r--   0        0        0    22467 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree
--rw-r--r--   0        0        0    22307 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.doctree
--rw-r--r--   0        0        0    22996 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.doctree
--rw-r--r--   0        0        0    19833 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree
--rw-r--r--   0        0        0    30229 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree
--rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOml.doctree
--rw-r--r--   0        0        0    30791 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree
--rw-r--r--   0        0        0    33278 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.classifier.miml_classifier.doctree
--rw-r--r--   0        0        0    75621 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.data.bag.doctree
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.data.doctree
--rw-r--r--   0        0        0    53060 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.data.instance.doctree
--rw-r--r--   0        0        0   134179 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.data.miml_dataset.doctree
--rw-r--r--   0        0        0    30437 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.datasets.dataset_utils.doctree
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.datasets.doctree
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.doctree
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.report.doctree
--rw-r--r--   0        0        0    21980 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.report.report.doctree
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.doctree
--rw-r--r--   0        0        0    14881 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOmi.doctree
--rw-r--r--   0        0        0    14826 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree
--rw-r--r--   0        0        0    13807 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.doctree
--rw-r--r--   0        0        0    14715 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree
--rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/doctrees/modules.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    55911 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/genindex.html
--rw-r--r--   0        0        0    31650 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.html
--rw-r--r--   0        0        0    26504 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html
--rw-r--r--   0        0        0    26478 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mi.apr_classifier.html
--rw-r--r--   0        0        0    22883 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mi.html
--rw-r--r--   0        0        0    26371 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mi.miles_classifier.html
--rw-r--r--   0        0        0    23859 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.html
--rw-r--r--   0        0        0    25934 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html
--rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html
--rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOml.html
--rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html
--rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.classifier.miml_classifier.html
--rw-r--r--   0        0        0    49079 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.data.bag.html
--rw-r--r--   0        0        0    36223 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.data.html
--rw-r--r--   0        0        0    41275 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.data.instance.html
--rw-r--r--   0        0        0    73862 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.data.miml_dataset.html
--rw-r--r--   0        0        0    30869 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.datasets.dataset_utils.html
--rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.datasets.html
--rw-r--r--   0        0        0    26183 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.html
--rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.report.html
--rw-r--r--   0        0        0    27344 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.report.report.html
--rw-r--r--   0        0        0    25587 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.html
--rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html
--rw-r--r--   0        0        0    21740 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOmi.html
--rw-r--r--   0        0        0    24417 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html
--rw-r--r--   0        0        0    24106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.arithmetic.html
--rw-r--r--   0        0        0    24493 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.geometric.html
--rw-r--r--   0        0        0    23219 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.html
--rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html
--rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.minmax.html
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/modules.html
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/objects.inv
--rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/search.html
--rw-r--r--   0        0        0    24269 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst.txt
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mi.rst.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOmi.rst.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.mimlTOml.rst.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.miml_classifier.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.miml_classifier.rst.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.rst
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.classifier.rst.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.bag.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.bag.rst.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.instance.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.instance.rst.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.miml_dataset.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.miml_dataset.rst.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.data.rst.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.datasets.dataset_utils.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.datasets.dataset_utils.rst.txt
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.datasets.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.datasets.rst.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.report.report.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.report.report.rst.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.report.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.report.rst.txt
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.rst
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.rst.txt
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst.txt
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOmi.rst.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst.txt
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.mimlTOml.rst.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/miml.transformation.rst.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0    12755 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    81602 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   332914 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    44317 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/styles/bootstrap.css.map
--rw-r--r--   0        0        0    72327 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0   294060 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
--rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
--rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
--rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/base.rst
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/conf.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mi.all_positive_apr_classifier.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mi.apr_classifier.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mi.miles_classifier.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mi.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.miml_classifier.rst
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.classifier.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.data.bag.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.data.instance.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.data.miml_dataset.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.data.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.datasets.dataset_utils.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.datasets.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.report.report.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.report.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOmi.label_powerset_transformation.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOml.arithmetic.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOml.geometric.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOml.minmax.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/docs/source/miml.transformation.rst
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.8/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/__init__.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/Makefile
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/make.bat
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mi.all_positive_apr_classifier.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mi.apr_classifier.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mi.miles_classifier.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mi.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.miml_classifier.rst
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.classifier.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.data.bag.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.data.instance.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.data.miml_dataset.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.data.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.datasets.dataset_utils.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.datasets.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.report.report.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.report.rst
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOmi.label_powerset_transformation.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOml.arithmetic.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOml.geometric.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOml.minmax.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api/miml.transformation.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.classifier.mi.rst
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.classifier.rst
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.data.rst
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.datasets.rst
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.report.rst
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.rst
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/miml.transformation.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/api2/modules.rst
--rw-r--r--   0        0        0   910561 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/environment.pickle
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.doctree
--rw-r--r--   0        0        0    22467 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree
--rw-r--r--   0        0        0    22307 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.doctree
--rw-r--r--   0        0        0    22996 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.doctree
--rw-r--r--   0        0        0    19833 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree
--rw-r--r--   0        0        0    30229 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree
--rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOml.doctree
--rw-r--r--   0        0        0    30791 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree
--rw-r--r--   0        0        0    33278 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.miml_classifier.doctree
--rw-r--r--   0        0        0    75621 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.data.bag.doctree
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.data.doctree
--rw-r--r--   0        0        0    53060 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.data.instance.doctree
--rw-r--r--   0        0        0   134179 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.data.miml_dataset.doctree
--rw-r--r--   0        0        0    30437 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.datasets.dataset_utils.doctree
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.datasets.doctree
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.doctree
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.report.doctree
--rw-r--r--   0        0        0    21980 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.report.report.doctree
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.doctree
--rw-r--r--   0        0        0    14881 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOmi.doctree
--rw-r--r--   0        0        0    14826 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree
--rw-r--r--   0        0        0    13807 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.doctree
--rw-r--r--   0        0        0    14715 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree
--rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/doctrees/modules.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/.buildinfo
--rw-r--r--   0        0        0    55911 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/genindex.html
--rw-r--r--   0        0        0    31650 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.html
--rw-r--r--   0        0        0    26504 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html
--rw-r--r--   0        0        0    26478 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.apr_classifier.html
--rw-r--r--   0        0        0    22883 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.html
--rw-r--r--   0        0        0    26371 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.miles_classifier.html
--rw-r--r--   0        0        0    23859 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.html
--rw-r--r--   0        0        0    25934 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html
--rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html
--rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOml.html
--rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html
--rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.classifier.miml_classifier.html
--rw-r--r--   0        0        0    49079 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.data.bag.html
--rw-r--r--   0        0        0    36223 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.data.html
--rw-r--r--   0        0        0    41275 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.data.instance.html
--rw-r--r--   0        0        0    73862 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.data.miml_dataset.html
--rw-r--r--   0        0        0    30869 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.datasets.dataset_utils.html
--rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.datasets.html
--rw-r--r--   0        0        0    26183 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.html
--rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.report.html
--rw-r--r--   0        0        0    27344 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.report.report.html
--rw-r--r--   0        0        0    25587 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.html
--rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html
--rw-r--r--   0        0        0    21740 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOmi.html
--rw-r--r--   0        0        0    24417 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html
--rw-r--r--   0        0        0    24106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.arithmetic.html
--rw-r--r--   0        0        0    24493 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.geometric.html
--rw-r--r--   0        0        0    23219 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.html
--rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html
--rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.minmax.html
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/modules.html
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/objects.inv
--rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/search.html
--rw-r--r--   0        0        0    24269 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/searchindex.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst.txt
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mi.rst.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst.txt
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOmi.rst.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.mimlTOml.rst.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.miml_classifier.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.miml_classifier.rst.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.rst
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.classifier.rst.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.bag.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.bag.rst.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.instance.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.instance.rst.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.miml_dataset.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.miml_dataset.rst.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.rst
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.data.rst.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.datasets.dataset_utils.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.datasets.dataset_utils.rst.txt
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.datasets.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.datasets.rst.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.report.report.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.report.report.rst.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.report.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.report.rst.txt
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.rst
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.rst.txt
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst.txt
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOmi.rst.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst.txt
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.mimlTOml.rst.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/miml.transformation.rst.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0    12755 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/sbt-webpack-macros.html
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0        0        0    81602 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0        0        0   332914 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0        0        0    44317 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/styles/bootstrap.css.map
--rw-r--r--   0        0        0    72327 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0        0        0   294060 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/styles/theme.css
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
--rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
--rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
--rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/conf.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mi.all_positive_apr_classifier.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mi.apr_classifier.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mi.miles_classifier.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mi.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mimlTOmi.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.mimlTOml.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.miml_classifier.rst
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.classifier.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.data.bag.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.data.instance.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.data.miml_dataset.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.data.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.datasets.dataset_utils.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.datasets.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.report.report.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.report.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOmi.label_powerset_transformation.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOmi.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOml.arithmetic.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOml.geometric.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOml.minmax.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.mimlTOml.rst
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/docs/source/miml.transformation.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mi/mi_wrapper_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/data/bag.py
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/data/dataset_utils.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/data/instance.py
--rw-r--r--   0        0        0    26874 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/report/__init__.py
--rw-r--r--   0        0        0     8970 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/report/report.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/tutorial/classifiers_mimltomi.ipynb
--rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/tutorial/classifiers_mimltoml.ipynb
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/tutorial/data_miml.ipynb
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/tutorial/train_test_experiment_miml.ipynb
--rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 mimllearning-0.5.8/src/miml/tutorial/transformations_miml.ipynb
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.8/LICENSE.txt
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.8/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.9/readme.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mimllearning-0.5.9/todo.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/Makefile
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/make.bat
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mi.all_positive_apr_classifier.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mi.apr_classifier.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mi.miles_classifier.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.miml_classifier.rst
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.classifier.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.data.bag.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.data.instance.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.data.miml_dataset.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.data.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.datasets.dataset_utils.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.datasets.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.report.report.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.report.rst
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOmi.label_powerset_transformation.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOml.arithmetic.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOml.geometric.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOml.minmax.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/api/miml.transformation.rst
+-rw-r--r--   0        0        0   910561 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.doctree
+-rw-r--r--   0        0        0    22467 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree
+-rw-r--r--   0        0        0    22307 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.doctree
+-rw-r--r--   0        0        0    22996 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.doctree
+-rw-r--r--   0        0        0    19833 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree
+-rw-r--r--   0        0        0    30229 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree
+-rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOml.doctree
+-rw-r--r--   0        0        0    30791 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree
+-rw-r--r--   0        0        0    33278 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.classifier.miml_classifier.doctree
+-rw-r--r--   0        0        0    75621 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.data.bag.doctree
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.data.doctree
+-rw-r--r--   0        0        0    53060 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.data.instance.doctree
+-rw-r--r--   0        0        0   134179 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.data.miml_dataset.doctree
+-rw-r--r--   0        0        0    30437 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.datasets.dataset_utils.doctree
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.datasets.doctree
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.doctree
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.report.doctree
+-rw-r--r--   0        0        0    21980 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.report.report.doctree
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.doctree
+-rw-r--r--   0        0        0    14881 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOmi.doctree
+-rw-r--r--   0        0        0    14826 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree
+-rw-r--r--   0        0        0    13807 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.doctree
+-rw-r--r--   0        0        0    14715 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree
+-rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    55911 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    31650 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.html
+-rw-r--r--   0        0        0    26504 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html
+-rw-r--r--   0        0        0    26478 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mi.apr_classifier.html
+-rw-r--r--   0        0        0    22883 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mi.html
+-rw-r--r--   0        0        0    26371 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mi.miles_classifier.html
+-rw-r--r--   0        0        0    23859 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.html
+-rw-r--r--   0        0        0    25934 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html
+-rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html
+-rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOml.html
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html
+-rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.classifier.miml_classifier.html
+-rw-r--r--   0        0        0    49079 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.data.bag.html
+-rw-r--r--   0        0        0    36223 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.data.html
+-rw-r--r--   0        0        0    41275 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.data.instance.html
+-rw-r--r--   0        0        0    73862 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.data.miml_dataset.html
+-rw-r--r--   0        0        0    30869 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.datasets.dataset_utils.html
+-rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.datasets.html
+-rw-r--r--   0        0        0    26183 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.html
+-rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.report.html
+-rw-r--r--   0        0        0    27344 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.report.report.html
+-rw-r--r--   0        0        0    25587 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.html
+-rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html
+-rw-r--r--   0        0        0    21740 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOmi.html
+-rw-r--r--   0        0        0    24417 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html
+-rw-r--r--   0        0        0    24106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.arithmetic.html
+-rw-r--r--   0        0        0    24493 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.geometric.html
+-rw-r--r--   0        0        0    23219 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.html
+-rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html
+-rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.minmax.html
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/objects.inv
+-rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/search.html
+-rw-r--r--   0        0        0    24269 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst.txt
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mi.rst.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOmi.rst.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.mimlTOml.rst.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.miml_classifier.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.miml_classifier.rst.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.rst
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.classifier.rst.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.bag.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.bag.rst.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.instance.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.instance.rst.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.miml_dataset.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.miml_dataset.rst.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.data.rst.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.datasets.dataset_utils.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.datasets.dataset_utils.rst.txt
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.datasets.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.datasets.rst.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.report.report.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.report.report.rst.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.report.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.report.rst.txt
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.rst
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.rst.txt
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst.txt
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOmi.rst.txt
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst.txt
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.mimlTOml.rst.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/miml.transformation.rst.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0    12755 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/sbt-webpack-macros.html
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0    81602 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   332914 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    44317 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/styles/bootstrap.css.map
+-rw-r--r--   0        0        0    72327 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0   294060 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
+-rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
+-rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
+-rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/base.rst
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/conf.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mi.all_positive_apr_classifier.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mi.apr_classifier.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mi.miles_classifier.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.miml_classifier.rst
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.classifier.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.data.bag.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.data.instance.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.data.miml_dataset.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.data.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.datasets.dataset_utils.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.datasets.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.report.report.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.report.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOmi.label_powerset_transformation.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOml.arithmetic.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOml.geometric.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOml.minmax.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/docs/source/miml.transformation.rst
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.5.9/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/__init__.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/Makefile
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/make.bat
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mi.all_positive_apr_classifier.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mi.apr_classifier.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mi.miles_classifier.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.miml_classifier.rst
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.classifier.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.data.bag.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.data.instance.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.data.miml_dataset.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.data.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.datasets.dataset_utils.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.datasets.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.report.report.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.report.rst
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOmi.label_powerset_transformation.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOml.arithmetic.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOml.geometric.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOml.minmax.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api/miml.transformation.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.classifier.rst
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.data.rst
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.datasets.rst
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.report.rst
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.rst
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/miml.transformation.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/api2/modules.rst
+-rw-r--r--   0        0        0   910561 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.doctree
+-rw-r--r--   0        0        0    22467 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree
+-rw-r--r--   0        0        0    22307 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.doctree
+-rw-r--r--   0        0        0    22996 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.doctree
+-rw-r--r--   0        0        0    19833 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree
+-rw-r--r--   0        0        0    30229 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree
+-rw-r--r--   0        0        0    19493 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOml.doctree
+-rw-r--r--   0        0        0    30791 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree
+-rw-r--r--   0        0        0    33278 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.miml_classifier.doctree
+-rw-r--r--   0        0        0    75621 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.data.bag.doctree
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.data.doctree
+-rw-r--r--   0        0        0    53060 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.data.instance.doctree
+-rw-r--r--   0        0        0   134179 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.data.miml_dataset.doctree
+-rw-r--r--   0        0        0    30437 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.datasets.dataset_utils.doctree
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.datasets.doctree
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.doctree
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.report.doctree
+-rw-r--r--   0        0        0    21980 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.report.report.doctree
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.doctree
+-rw-r--r--   0        0        0    14881 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOmi.doctree
+-rw-r--r--   0        0        0    14826 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree
+-rw-r--r--   0        0        0    13807 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.doctree
+-rw-r--r--   0        0        0    14715 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree
+-rw-r--r--   0        0        0    14395 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    55911 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    31650 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.html
+-rw-r--r--   0        0        0    26504 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html
+-rw-r--r--   0        0        0    26478 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.apr_classifier.html
+-rw-r--r--   0        0        0    22883 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.html
+-rw-r--r--   0        0        0    26371 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.miles_classifier.html
+-rw-r--r--   0        0        0    23859 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.html
+-rw-r--r--   0        0        0    25934 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html
+-rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html
+-rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOml.html
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html
+-rw-r--r--   0        0        0    31231 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.classifier.miml_classifier.html
+-rw-r--r--   0        0        0    49079 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.data.bag.html
+-rw-r--r--   0        0        0    36223 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.data.html
+-rw-r--r--   0        0        0    41275 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.data.instance.html
+-rw-r--r--   0        0        0    73862 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.data.miml_dataset.html
+-rw-r--r--   0        0        0    30869 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.datasets.dataset_utils.html
+-rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.datasets.html
+-rw-r--r--   0        0        0    26183 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.html
+-rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.report.html
+-rw-r--r--   0        0        0    27344 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.report.report.html
+-rw-r--r--   0        0        0    25587 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.html
+-rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html
+-rw-r--r--   0        0        0    21740 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOmi.html
+-rw-r--r--   0        0        0    24417 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html
+-rw-r--r--   0        0        0    24106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.arithmetic.html
+-rw-r--r--   0        0        0    24493 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.geometric.html
+-rw-r--r--   0        0        0    23219 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.html
+-rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html
+-rw-r--r--   0        0        0    23536 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.minmax.html
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/objects.inv
+-rw-r--r--   0        0        0    24486 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/search.html
+-rw-r--r--   0        0        0    24269 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.all_positive_apr_classifier.rst.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.apr_classifier.rst.txt
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.miles_classifier.rst.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mi.rst.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOmi.rst.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOml.miml_to_ml_classifier.rst.txt
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.mimlTOml.rst.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.miml_classifier.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.miml_classifier.rst.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.rst
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.classifier.rst.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.bag.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.bag.rst.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.instance.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.instance.rst.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.miml_dataset.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.miml_dataset.rst.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.data.rst.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.datasets.dataset_utils.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.datasets.dataset_utils.rst.txt
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.datasets.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.datasets.rst.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.report.report.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.report.report.rst.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.report.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.report.rst.txt
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.rst
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.rst.txt
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOmi.binary_relevance_transformation.rst.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOmi.label_powerset_transformation.rst.txt
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOmi.rst.txt
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.arithmetic.rst.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.geometric.rst.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.miml_to_ml_transformation.rst.txt
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.minmax.rst.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.mimlTOml.rst.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/miml.transformation.rst.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0    12755 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/sbt-webpack-macros.html
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135314 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0        0        0    81602 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0        0        0   332914 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0        0        0    44317 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0        0        0   208854 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0        0        0   555088 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/styles/bootstrap.css.map
+-rw-r--r--   0        0        0    72327 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0        0        0   294060 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/styles/pydata-sphinx-theme.css.map
+-rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt
+-rw-r--r--   0        0        0   102621 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css
+-rw-r--r--   0        0        0  1485766 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   207972 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    68004 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25452 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   419720 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156496 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/conf.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mi.all_positive_apr_classifier.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mi.apr_classifier.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mi.miles_classifier.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mi.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mimlTOmi.miml_to_mi_classifier.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mimlTOmi.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mimlTOml.miml_to_ml_classifier.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.mimlTOml.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.miml_classifier.rst
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.classifier.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.data.bag.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.data.instance.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.data.miml_dataset.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.data.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.datasets.dataset_utils.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.datasets.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.report.report.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.report.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOmi.binary_relevance_transformation.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOmi.label_powerset_transformation.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOmi.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOml.arithmetic.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOml.geometric.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOml.miml_to_ml_transformation.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOml.minmax.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.mimlTOml.rst
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/docs/source/miml.transformation.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mi/mi_wrapper_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/data/dataset_utils.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/data/instance.py
+-rw-r--r--   0        0        0    26874 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/report/report.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/tutorial/classifiers_mimltomi.ipynb
+-rw-r--r--   0        0        0    15720 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/tutorial/classifiers_mimltoml.ipynb
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/tutorial/data_miml.ipynb
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/tutorial/train_test_experiment_miml.ipynb
+-rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 mimllearning-0.5.9/src/miml/tutorial/transformations_miml.ipynb
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 mimllearning-0.5.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mimllearning-0.5.9/LICENSE.txt
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 mimllearning-0.5.9/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 mimllearning-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 mimllearning-0.5.9/PKG-INFO
```

### Comparing `mimllearning-0.5.8/readme.md` & `mimllearning-0.5.9/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/todo.md` & `mimllearning-0.5.9/todo.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/Makefile` & `mimllearning-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/make.bat` & `mimllearning-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/environment.pickle` & `mimllearning-0.5.9/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOml.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.classifier.miml_classifier.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.classifier.miml_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.data.bag.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.data.bag.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.data.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.data.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.data.instance.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.data.instance.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.data.miml_dataset.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.data.miml_dataset.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.datasets.dataset_utils.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.datasets.dataset_utils.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.datasets.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.datasets.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.report.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.report.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.report.report.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.report.report.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOmi.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOmi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree` & `mimllearning-0.5.9/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/doctrees/modules.doctree` & `mimllearning-0.5.9/docs/build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/genindex.html` & `mimllearning-0.5.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mi.apr_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mi.apr_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mi.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mi.miles_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mi.miles_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOml.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.classifier.miml_classifier.html` & `mimllearning-0.5.9/docs/build/html/miml.classifier.miml_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.data.bag.html` & `mimllearning-0.5.9/docs/build/html/miml.data.bag.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.data.html` & `mimllearning-0.5.9/docs/build/html/miml.data.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.data.instance.html` & `mimllearning-0.5.9/docs/build/html/miml.data.instance.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.data.miml_dataset.html` & `mimllearning-0.5.9/docs/build/html/miml.data.miml_dataset.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.datasets.dataset_utils.html` & `mimllearning-0.5.9/docs/build/html/miml.datasets.dataset_utils.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.datasets.html` & `mimllearning-0.5.9/docs/build/html/miml.datasets.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.html` & `mimllearning-0.5.9/docs/build/html/miml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.report.html` & `mimllearning-0.5.9/docs/build/html/miml.report.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.report.report.html` & `mimllearning-0.5.9/docs/build/html/miml.report.report.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOmi.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOmi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.arithmetic.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.arithmetic.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.geometric.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.geometric.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/miml.transformation.mimlTOml.minmax.html` & `mimllearning-0.5.9/docs/build/html/miml.transformation.mimlTOml.minmax.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/modules.html` & `mimllearning-0.5.9/docs/build/html/modules.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/objects.inv` & `mimllearning-0.5.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/py-modindex.html` & `mimllearning-0.5.9/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/search.html` & `mimllearning-0.5.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/searchindex.js` & `mimllearning-0.5.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mimllearning-0.5.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/basic.css` & `mimllearning-0.5.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/doctools.js` & `mimllearning-0.5.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/jquery.js` & `mimllearning-0.5.9/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/language_data.js` & `mimllearning-0.5.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/pygments.css` & `mimllearning-0.5.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/searchtools.js` & `mimllearning-0.5.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/sphinx_highlight.js` & `mimllearning-0.5.9/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/webpack-macros.html` & `mimllearning-0.5.9/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/badge_only.css` & `mimllearning-0.5.9/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/theme.css` & `mimllearning-0.5.9/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-bold.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal.woff` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/css/fonts/lato-normal.woff2` & `mimllearning-0.5.9/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/images/logo_binder.svg` & `mimllearning-0.5.9/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/images/logo_colab.png` & `mimllearning-0.5.9/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/images/logo_deepnote.svg` & `mimllearning-0.5.9/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/images/logo_jupyterhub.svg` & `mimllearning-0.5.9/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/js/badge_only.js` & `mimllearning-0.5.9/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `mimllearning-0.5.9/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/js/html5shiv.min.js` & `mimllearning-0.5.9/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/js/theme.js` & `mimllearning-0.5.9/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/scripts/bootstrap.js` & `mimllearning-0.5.9/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/scripts/bootstrap.js.map` & `mimllearning-0.5.9/docs/build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `mimllearning-0.5.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map` & `mimllearning-0.5.9/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/scripts/sphinx-book-theme.js` & `mimllearning-0.5.9/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `mimllearning-0.5.9/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/styles/bootstrap.css` & `mimllearning-0.5.9/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/styles/bootstrap.css.map` & `mimllearning-0.5.9/docs/build/html/_static/styles/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `mimllearning-0.5.9/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/styles/pydata-sphinx-theme.css.map` & `mimllearning-0.5.9/docs/build/html/_static/styles/pydata-sphinx-theme.css.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/styles/sphinx-book-theme.css` & `mimllearning-0.5.9/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2` & `mimllearning-0.5.9/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/source/base.rst` & `mimllearning-0.5.9/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/docs/source/conf.py` & `mimllearning-0.5.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.5.9/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/Makefile` & `mimllearning-0.5.9/src/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/make.bat` & `mimllearning-0.5.9/src/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/api2/miml.classifier.mi.rst` & `mimllearning-0.5.9/src/docs/api2/miml.classifier.mi.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/api2/miml.classifier.mimlTOmi.rst` & `mimllearning-0.5.9/src/docs/api2/miml.classifier.mimlTOmi.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/api2/miml.data.rst` & `mimllearning-0.5.9/src/docs/api2/miml.data.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/api2/miml.transformation.mimlTOmi.rst` & `mimllearning-0.5.9/src/docs/api2/miml.transformation.mimlTOmi.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/api2/miml.transformation.mimlTOml.rst` & `mimllearning-0.5.9/src/docs/api2/miml.transformation.mimlTOml.rst`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/environment.pickle` & `mimllearning-0.5.9/src/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.all_positive_apr_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.apr_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mi.miles_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOml.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.mimlTOml.miml_to_ml_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.classifier.miml_classifier.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.classifier.miml_classifier.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.data.bag.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.data.bag.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.data.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.data.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.data.instance.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.data.instance.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.data.miml_dataset.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.data.miml_dataset.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.datasets.dataset_utils.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.datasets.dataset_utils.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.datasets.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.datasets.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.report.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.report.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.report.report.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.report.report.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOmi.binary_relevance_transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOmi.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOmi.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOmi.label_powerset_transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.arithmetic.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.geometric.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.miml_to_ml_transformation.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/miml.transformation.mimlTOml.minmax.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/doctrees/modules.doctree` & `mimllearning-0.5.9/src/docs/build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/genindex.html` & `mimllearning-0.5.9/src/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.all_positive_apr_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.apr_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.apr_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mi.miles_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mi.miles_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_br_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOmi.miml_to_mi_lp_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOml.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.mimlTOml.miml_to_ml_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.classifier.miml_classifier.html` & `mimllearning-0.5.9/src/docs/build/html/miml.classifier.miml_classifier.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.data.bag.html` & `mimllearning-0.5.9/src/docs/build/html/miml.data.bag.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.data.html` & `mimllearning-0.5.9/src/docs/build/html/miml.data.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.data.instance.html` & `mimllearning-0.5.9/src/docs/build/html/miml.data.instance.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.data.miml_dataset.html` & `mimllearning-0.5.9/src/docs/build/html/miml.data.miml_dataset.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.datasets.dataset_utils.html` & `mimllearning-0.5.9/src/docs/build/html/miml.datasets.dataset_utils.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.datasets.html` & `mimllearning-0.5.9/src/docs/build/html/miml.datasets.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.html` & `mimllearning-0.5.9/src/docs/build/html/miml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.report.html` & `mimllearning-0.5.9/src/docs/build/html/miml.report.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.report.report.html` & `mimllearning-0.5.9/src/docs/build/html/miml.report.report.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOmi.binary_relevance_transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOmi.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOmi.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOmi.label_powerset_transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.arithmetic.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.arithmetic.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.geometric.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.geometric.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.miml_to_ml_transformation.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/miml.transformation.mimlTOml.minmax.html` & `mimllearning-0.5.9/src/docs/build/html/miml.transformation.mimlTOml.minmax.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/modules.html` & `mimllearning-0.5.9/src/docs/build/html/modules.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/objects.inv` & `mimllearning-0.5.9/src/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/py-modindex.html` & `mimllearning-0.5.9/src/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/search.html` & `mimllearning-0.5.9/src/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/searchindex.js` & `mimllearning-0.5.9/src/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `mimllearning-0.5.9/src/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/basic.css` & `mimllearning-0.5.9/src/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/doctools.js` & `mimllearning-0.5.9/src/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/jquery.js` & `mimllearning-0.5.9/src/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/language_data.js` & `mimllearning-0.5.9/src/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/pygments.css` & `mimllearning-0.5.9/src/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/searchtools.js` & `mimllearning-0.5.9/src/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/sphinx_highlight.js` & `mimllearning-0.5.9/src/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/webpack-macros.html` & `mimllearning-0.5.9/src/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/badge_only.css` & `mimllearning-0.5.9/src/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/theme.css` & `mimllearning-0.5.9/src/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-bold.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal.woff` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/css/fonts/lato-normal.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/images/logo_binder.svg` & `mimllearning-0.5.9/src/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/images/logo_colab.png` & `mimllearning-0.5.9/src/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/images/logo_deepnote.svg` & `mimllearning-0.5.9/src/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/images/logo_jupyterhub.svg` & `mimllearning-0.5.9/src/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/js/badge_only.js` & `mimllearning-0.5.9/src/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `mimllearning-0.5.9/src/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/js/html5shiv.min.js` & `mimllearning-0.5.9/src/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/js/theme.js` & `mimllearning-0.5.9/src/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.mo`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `mimllearning-0.5.9/src/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/scripts/bootstrap.js` & `mimllearning-0.5.9/src/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/scripts/bootstrap.js.map` & `mimllearning-0.5.9/src/docs/build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `mimllearning-0.5.9/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map` & `mimllearning-0.5.9/src/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/scripts/sphinx-book-theme.js` & `mimllearning-0.5.9/src/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `mimllearning-0.5.9/src/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/styles/bootstrap.css` & `mimllearning-0.5.9/src/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/styles/bootstrap.css.map` & `mimllearning-0.5.9/src/docs/build/html/_static/styles/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `mimllearning-0.5.9/src/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/styles/pydata-sphinx-theme.css.map` & `mimllearning-0.5.9/src/docs/build/html/_static/styles/pydata-sphinx-theme.css.map`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/styles/sphinx-book-theme.css` & `mimllearning-0.5.9/src/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/css/all.min.css`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/js/all.min.js`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2` & `mimllearning-0.5.9/src/docs/build/html/_static/vendor/fontawesome/6.5.1/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/docs/source/conf.py` & `mimllearning-0.5.9/src/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/miml_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/mi/mi_wrapper_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/mi/mi_wrapper_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.5.9/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/data/bag.py` & `mimllearning-0.5.9/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/data/dataset_utils.py` & `mimllearning-0.5.9/src/miml/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/data/instance.py` & `mimllearning-0.5.9/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/data/miml_dataset.py` & `mimllearning-0.5.9/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/datasets/miml_birds.arff` & `mimllearning-0.5.9/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/datasets/miml_birds.csv` & `mimllearning-0.5.9/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.5.9/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.5.9/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/report/report.py` & `mimllearning-0.5.9/src/miml/report/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import warnings
+from copy import deepcopy
+
 import numpy as np
 from sklearn.metrics import hamming_loss, accuracy_score, fbeta_score, jaccard_score, log_loss, \
     roc_auc_score, f1_score, precision_score, recall_score, average_precision_score
 from ..data import MIMLDataset
 
 
 class Report:
@@ -114,15 +116,15 @@
         path : str, default=None
             Path to csv where the data would be stored
 
         """
         self.calculate_metrics()
         header = ""
         if self.header:
-            metrics=self.metrics_name
+            metrics = deepcopy(self.metrics_name)
 
             for metric in range(len(metrics)):
                 if metrics[metric][0:5] == "fbeta":
                     metrics[metric] += " beta value = " + str(self.beta)
             header = ",".join(str(metric) for metric in metrics)
         values = ",".join(str(self.metrics_value[metric]) for metric in self.metrics_name)
         if path is None:
```

### Comparing `mimllearning-0.5.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.5.9/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.5.9/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.5.9/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.5.9/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.5.9/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/tutorial/classifiers_mimltomi.ipynb` & `mimllearning-0.5.9/src/miml/tutorial/classifiers_mimltomi.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/tutorial/classifiers_mimltoml.ipynb` & `mimllearning-0.5.9/src/miml/tutorial/classifiers_mimltoml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/tutorial/data_miml.ipynb` & `mimllearning-0.5.9/src/miml/tutorial/data_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/tutorial/train_test_experiment_miml.ipynb` & `mimllearning-0.5.9/src/miml/tutorial/train_test_experiment_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/src/miml/tutorial/transformations_miml.ipynb` & `mimllearning-0.5.9/src/miml/tutorial/transformations_miml.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/LICENSE.txt` & `mimllearning-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/README.md` & `mimllearning-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.5.8/pyproject.toml` & `mimllearning-0.5.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.5.8"
+version = "0.5.9"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.5.8"
+version = "0.5.9"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 license = "GPL-3.0"
 keywords = ["machine-learning", "python", "data-science", "miml", "multilabel", "multi-instance"]
 readme = "README.md"
```

### Comparing `mimllearning-0.5.8/PKG-INFO` & `mimllearning-0.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.5.8
+Version: 0.5.9
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE.txt
 Keywords: data-science,machine-learning,miml,multi-instance,multilabel,python
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

