# Comparing `tmp/luma-ml-0.8.1.tar.gz` & `tmp/luma-ml-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.8.1.tar", last modified: Fri May 17 14:28:21 2024, max compression
+gzip compressed data, was "luma-ml-0.8.2.tar", last modified: Sun May 26 19:19:09 2024, max compression
```

## Comparing `luma-ml-0.8.1.tar` & `luma-ml-0.8.2.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.912562 luma-ml-0.8.1/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.8.1/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-17 14:28:21.912167 luma-ml-0.8.1/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-05-17 14:25:43.000000 luma-ml-0.8.1/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.886076 luma-ml-0.8.1/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    11001 2024-05-17 14:03:21.000000 luma-ml-0.8.1/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.8.1/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.888825 luma-ml-0.8.1/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.8.1/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.8.1/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.8.1/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.8.1/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.8.1/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.8.1/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.891696 luma-ml-0.8.1/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.8.1/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.8.1/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.8.1/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.8.1/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.8.1/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.8.1/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.892645 luma-ml-0.8.1/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.8.1/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.8.1/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.8.1/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.894914 luma-ml-0.8.1/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.8.1/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.8.1/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.8.1/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.8.1/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.8.1/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.895674 luma-ml-0.8.1/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.8.1/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma-ml-0.8.1/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16195 2024-05-13 15:45:21.000000 luma-ml-0.8.1/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.896558 luma-ml-0.8.1/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.8.1/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.8.1/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.8.1/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.8.1/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.896944 luma-ml-0.8.1/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.8.1/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.898363 luma-ml-0.8.1/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.8.1/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.8.1/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.8.1/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.8.1/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.900096 luma-ml-0.8.1/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.901722 luma-ml-0.8.1/luma/neural/_layers/
--rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.8.1/luma/neural/_layers/_act.py
--rw-r--r--   0 chanlee    (501) staff       (20)    18113 2024-05-16 17:18:35.000000 luma-ml-0.8.1/luma/neural/_layers/_conv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-16 17:19:42.000000 luma-ml-0.8.1/luma/neural/_layers/_drop.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.8.1/luma/neural/_layers/_linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-16 17:20:47.000000 luma-ml-0.8.1/luma/neural/_layers/_norm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9441 2024-05-16 17:21:47.000000 luma-ml-0.8.1/luma/neural/_layers/_pool.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.902354 luma-ml-0.8.1/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    36463 2024-05-17 14:00:42.000000 luma-ml-0.8.1/luma/neural/_models/_imagenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12758 2024-05-17 07:23:08.000000 luma-ml-0.8.1/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-17 07:21:18.000000 luma-ml-0.8.1/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-13 17:00:56.000000 luma-ml-0.8.1/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16608 2024-05-17 13:11:54.000000 luma-ml-0.8.1/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.8.1/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25743 2024-05-16 14:22:33.000000 luma-ml-0.8.1/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.8.1/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    41603 2024-05-17 14:26:11.000000 luma-ml-0.8.1/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.8.1/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.8.1/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.902568 luma-ml-0.8.1/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.8.1/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.903866 luma-ml-0.8.1/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.8.1/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.8.1/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.8.1/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.8.1/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.905487 luma-ml-0.8.1/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    19132 2024-05-13 19:40:06.000000 luma-ml-0.8.1/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.8.1/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.8.1/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.908619 luma-ml-0.8.1/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.8.1/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.8.1/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.8.1/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.8.1/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.8.1/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.8.1/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.8.1/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.909233 luma-ml-0.8.1/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.8.1/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-14 16:39:15.000000 luma-ml-0.8.1/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.910557 luma-ml-0.8.1/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1948 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-17 14:28:21.000000 luma-ml-0.8.1/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-17 14:28:21.912633 luma-ml-0.8.1/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-17 14:28:15.000000 luma-ml-0.8.1/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-17 14:28:21.911467 luma-ml-0.8.1/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.8.1/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-17 14:02:51.000000 luma-ml-0.8.1/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.881916 luma-ml-0.8.2/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.8.2/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-26 19:19:09.881562 luma-ml-0.8.2/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-05-26 19:18:32.000000 luma-ml-0.8.2/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.865170 luma-ml-0.8.2/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    11481 2024-05-26 12:21:52.000000 luma-ml-0.8.2/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1502 2024-05-26 11:11:06.000000 luma-ml-0.8.2/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.866495 luma-ml-0.8.2/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.8.2/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.8.2/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-05-23 16:46:06.000000 luma-ml-0.8.2/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.8.2/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.8.2/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.8.2/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.868006 luma-ml-0.8.2/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.8.2/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.8.2/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.8.2/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.8.2/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.8.2/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.8.2/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.868744 luma-ml-0.8.2/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.8.2/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.8.2/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.8.2/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.870212 luma-ml-0.8.2/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.8.2/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.8.2/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.8.2/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.8.2/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.8.2/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.871143 luma-ml-0.8.2/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.8.2/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma-ml-0.8.2/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16195 2024-05-13 15:45:21.000000 luma-ml-0.8.2/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.871908 luma-ml-0.8.2/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.8.2/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.8.2/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.8.2/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.8.2/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.872079 luma-ml-0.8.2/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.8.2/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.872809 luma-ml-0.8.2/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.8.2/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.8.2/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.8.2/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.8.2/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.874312 luma-ml-0.8.2/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.875392 luma-ml-0.8.2/luma/neural/_layers/
+-rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.8.2/luma/neural/_layers/_act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19314 2024-05-26 11:53:00.000000 luma-ml-0.8.2/luma/neural/_layers/_conv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-23 16:58:05.000000 luma-ml-0.8.2/luma/neural/_layers/_drop.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.8.2/luma/neural/_layers/_linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-16 17:20:47.000000 luma-ml-0.8.2/luma/neural/_layers/_norm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    29777 2024-05-26 11:24:51.000000 luma-ml-0.8.2/luma/neural/_layers/_pool.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.876366 luma-ml-0.8.2/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    13100 2024-05-18 09:06:30.000000 luma-ml-0.8.2/luma/neural/_models/_alex.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6471 2024-05-26 12:18:12.000000 luma-ml-0.8.2/luma/neural/_models/_inception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12758 2024-05-17 07:23:08.000000 luma-ml-0.8.2/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-17 07:21:18.000000 luma-ml-0.8.2/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    23945 2024-05-24 18:22:17.000000 luma-ml-0.8.2/luma/neural/_models/_vgg.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-13 17:00:56.000000 luma-ml-0.8.2/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24180 2024-05-26 11:59:07.000000 luma-ml-0.8.2/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.8.2/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    33776 2024-05-26 11:55:46.000000 luma-ml-0.8.2/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.8.2/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    46067 2024-05-26 19:16:21.000000 luma-ml-0.8.2/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.8.2/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.8.2/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.876636 luma-ml-0.8.2/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.8.2/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.877357 luma-ml-0.8.2/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.8.2/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.8.2/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.8.2/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.8.2/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.878150 luma-ml-0.8.2/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19163 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.8.2/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.8.2/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.879488 luma-ml-0.8.2/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.8.2/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.8.2/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.8.2/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.8.2/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.8.2/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.8.2/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.8.2/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.879838 luma-ml-0.8.2/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.8.2/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-23 17:04:49.000000 luma-ml-0.8.2/luma/visual/eval.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.880727 luma-ml-0.8.2/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     2000 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-26 19:19:09.881987 luma-ml-0.8.2/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-26 19:18:56.000000 luma-ml-0.8.2/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.881083 luma-ml-0.8.2/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.8.2/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-18 16:19:55.000000 luma-ml-0.8.2/test/__test.py
```

### Comparing `luma-ml-0.8.1/LICENSE` & `luma-ml-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/PKG-INFO` & `luma-ml-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.71k-red">
+        <img src="https://img.shields.io/badge/total downloads-6.04k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.1</td>
+                    <td>0.8.2</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~23.8K</td>
+                    <td>~25.3K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.8.1 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.8.2 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.71k-red][GitHub code size in bytes][Code Style]
+6.04k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.1
-Lines of Code  ~23.8K
+Latest Version 0.8.2
+Lines of Code  ~25.3K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.1/README.md` & `luma-ml-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.71k-red">
+        <img src="https://img.shields.io/badge/total downloads-6.04k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.1</td>
+                    <td>0.8.2</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~23.8K</td>
+                    <td>~25.3K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.71k-red][GitHub code size in bytes][Code Style]
+6.04k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.1
-Lines of Code  ~23.8K
+Latest Version 0.8.2
+Lines of Code  ~25.3K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.1/luma/__import__.py` & `luma-ml-0.8.2/luma/__import__.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,16 +76,25 @@
 from luma.neural.layer import (
     Convolution1D,
     Convolution2D,
     Convolution3D,
     Pooling1D,
     Pooling2D,
     Pooling3D,
+    GlobalAvgPooling1D,
+    GlobalAvgPooling2D,
+    GlobalAvgPooling3D,
+    LpPooling1D,
+    LpPooling2D,
+    LpPooling3D,
     Dense,
     Dropout,
+    Dropout1D,
+    Dropout2D,
+    Dropout3D,
     Flatten,
     Activation,
     BatchNorm1D,
     BatchNorm2D,
     BatchNorm3D,
     LocalResponseNorm,
     LayerNorm,
@@ -100,25 +109,35 @@
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.loss import CrossEntropy, BinaryCrossEntropy, MSELoss
 from luma.neural.init import KaimingInit, XavierInit
-from luma.neural.block import ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock
+from luma.neural.block import (
+    ConvBlock1D,
+    ConvBlock2D,
+    ConvBlock3D,
+    DenseBlock,
+    InceptionBlock,
+)
 from luma.neural.network import SimpleMLP, SimpleCNN
 from luma.neural.network import (
     LeNet_1,
     LeNet_4,
+    LeNet_5,
     AlexNet,
     ZFNet,
     VGGNet_11,
     VGGNet_13,
     VGGNet_16,
     VGGNet_19,
+    Inception_V1,
+    Inception_V2,
+    Inception_V3,
 )
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
@@ -174,22 +193,22 @@
 
 from luma.visual.eda import (
     CorrelationBar,
     CorrelationHeatmap,
     JointPlot,
     MissingProportion,
 )
-from luma.visual.evaluation import (
+from luma.visual.eval import (
     DecisionRegion,
     ClusterPlot,
     ROCCurve,
     PrecisionRecallCurve,
 )
-from luma.visual.evaluation import ConfusionMatrix, ResidualPlot, LearningCurve
-from luma.visual.evaluation import ValidationCurve, InertiaPlot
+from luma.visual.eval import ConfusionMatrix, ResidualPlot, LearningCurve
+from luma.visual.eval import ValidationCurve, InertiaPlot
 
 from luma.migrate.port import ModelPorter
 
 
 if __name__ == "__main__":
 
     # ------------------- [ luma.core ] ------------------------
@@ -260,26 +279,32 @@
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
     Layer, Loss, Initializer, NeuralModel
 
     Convolution1D, Convolution2D, Convolution3D,
     Pooling1D, Pooling2D, Pooling3D,
+    GlobalAvgPooling1D, GlobalAvgPooling2D, GlobalAvgPooling3D,
+    LpPooling1D, LpPooling2D, LpPooling3D
+    Dropout, Dropout1D, Dropout2D, Dropout3D,
     BatchNorm1D, BatchNorm2D, BatchNorm3D,
     LocalResponseNorm, LayerNorm,
-    Dense, Dropout, Flatten, Activation, Sequential
+    Dense, Flatten, Activation,
+    Sequential
 
     CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
-    ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock
+    ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock,
+    InceptionBlock
 
-    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4, AlexNet, ZFNet,
-    VGGNet_11, VGGNet_13, VGGNet_16, VGGNet_19
+    SimpleMLP, SimpleCNN, LeNet_1, LeNet_4, LeNet_5, AlexNet,
+    ZFNet, VGGNet_11, VGGNet_13, VGGNet_16, VGGNet_19,
+    Inception_V1, Inception_V2, Inception_V3
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
```

### Comparing `luma-ml-0.8.1/luma/__init__.py` & `luma-ml-0.8.2/luma/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 `Luma`
 ======
 
 Lumerico's Universal Machine-learning Assistant
 -----------------------------------------------
-Luma is a comprehensive, user-friendly Python module designed for both beginners 
+Luma is a comprehensive, user-friendly Python library designed for both beginners 
 and advanced users in the field of machine learning and data science. It provides 
 a wide range of tools and functionalities to streamline the process of data analysis, 
 model building, evaluation, and deployment.
 
 Key Features
 ------------
 - Easy Data Handling: Simplify data preprocessing, transformation, and visualization.
```

### Comparing `luma-ml-0.8.1/luma/classifier/discriminant.py` & `luma-ml-0.8.2/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/classifier/logistic.py` & `luma-ml-0.8.2/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/classifier/naive_bayes.py` & `luma-ml-0.8.2/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/classifier/neighbors.py` & `luma-ml-0.8.2/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/classifier/svm.py` & `luma-ml-0.8.2/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/classifier/tree.py` & `luma-ml-0.8.2/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/clustering/affinity.py` & `luma-ml-0.8.2/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/clustering/density.py` & `luma-ml-0.8.2/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/clustering/hierarchy.py` & `luma-ml-0.8.2/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/clustering/kmeans.py` & `luma-ml-0.8.2/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/clustering/mixture.py` & `luma-ml-0.8.2/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/clustering/spectral.py` & `luma-ml-0.8.2/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/core/base.py` & `luma-ml-0.8.2/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/core/super.py` & `luma-ml-0.8.2/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/ensemble/bagging.py` & `luma-ml-0.8.2/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/ensemble/boost.py` & `luma-ml-0.8.2/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/ensemble/forest.py` & `luma-ml-0.8.2/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/ensemble/stack.py` & `luma-ml-0.8.2/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/ensemble/vote.py` & `luma-ml-0.8.2/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/interface/exception.py` & `luma-ml-0.8.2/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/interface/typing.py` & `luma-ml-0.8.2/luma/interface/typing.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/interface/util.py` & `luma-ml-0.8.2/luma/interface/util.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/metric/classification.py` & `luma-ml-0.8.2/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/metric/clustering.py` & `luma-ml-0.8.2/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/metric/distance.py` & `luma-ml-0.8.2/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/metric/regression.py` & `luma-ml-0.8.2/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/migrate/port.py` & `luma-ml-0.8.2/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/model_selection/cv.py` & `luma-ml-0.8.2/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/model_selection/fold.py` & `luma-ml-0.8.2/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/model_selection/search.py` & `luma-ml-0.8.2/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/model_selection/split.py` & `luma-ml-0.8.2/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/_layers/_act.py` & `luma-ml-0.8.2/luma/neural/_layers/_act.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/_layers/_conv.py` & `luma-ml-0.8.2/luma/neural/_layers/_conv.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,47 +12,50 @@
 
 
 class _Conv1D(Layer):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        filter_size: int,
+        filter_size: Tuple[int] | int,
         stride: int = 1,
-        padding: Literal["valid", "same"] = "same",
+        padding: Tuple[int] | int | Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
         optimizer: Optimizer | None = None,
         lambda_: float = 0.0,
         random_state: int | None = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
-        self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
         self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
         self.random_state = random_state
         self.rs_ = np.random.RandomState(self.random_state)
 
+        if isinstance(filter_size, int):
+            self.filter_size = (filter_size,)
+        else:
+            self.filter_size = filter_size
+
         self.init_params(
             w_shape=(
                 self.out_channels,
                 self.in_channels,
-                self.filter_size,
+                *self.filter_size,
             ),
             b_shape=(1, self.out_channels),
         )
         self.set_param_ranges(
             {
                 "in_channels": ("0<,+inf", int),
                 "out_channels": ("0<,+inf", int),
-                "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
     @Tensor.force_dim(3)
@@ -65,15 +68,15 @@
             raise ValueError(
                 f"channels of 'X' does not match with 'in_channels'! "
                 + f"({self.in_channels}!={channels})"
             )
 
         pad_w, padded_w = self._get_padding_dim(width)
 
-        out_width = ((padded_w - self.filter_size) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size[0]) // self.stride) + 1
         out: Tensor = np.zeros((batch_size, self.out_channels, out_width))
 
         X_padded = np.pad(X, ((0, 0), (0, 0), (pad_w, pad_w)), mode="constant")
         X_fft = np.fft.rfft(X_padded, n=padded_w, axis=2)
         filter_fft = np.fft.rfft(
             self.weights_,
             n=padded_w,
@@ -109,17 +112,18 @@
 
         for f in range(self.out_channels):
             for c in range(channels):
                 filter_d_out_fft = np.sum(
                     X_fft[:, c] * d_out_fft[:, f].conj(),
                     axis=0,
                 )
-                self.dW[f, c] = np.fft.irfft(filter_d_out_fft, n=padded_w)[
-                    : self.filter_size
-                ]
+                self.dW[f, c] = np.fft.irfftn(
+                    filter_d_out_fft,
+                    s=(padded_w,),
+                )[pad_w : pad_w + self.filter_size[0]]
 
         self.dW += 2 * self.lambda_ * self.weights_
 
         for i in range(batch_size):
             for c in range(channels):
                 temp = np.zeros(padded_w // 2 + 1, dtype=np.complex128)
                 for f in range(self.out_channels):
@@ -127,73 +131,80 @@
                     temp += filter_fft * d_out_fft[i, f]
                 dX_padded[i, c] = np.fft.irfft(temp, n=padded_w)
 
         self.dX = dX_padded[:, :, pad_w:-pad_w] if pad_w > 0 else dX_padded
         return self.dX
 
     def _get_padding_dim(self, width: int) -> Tuple[int, ...]:
-        if self.padding == "same":
-            pad_w = (self.filter_size - 1) // 2
-            padded_w = width + 2 * pad_w
-
+        if isinstance(self.padding, tuple):
+            if len(self.padding) != 1:
+                raise ValueError("Padding tuple must have exactly one value.")
+            pad_w = self.padding[0]
+
+        elif isinstance(self.padding, int):
+            pad_w = self.padding
+        elif self.padding == "same":
+            pad_w = (self.filter_size[0] - 1) // 2
         elif self.padding == "valid":
             pad_w = 0
-            padded_w = width
         else:
             raise UnsupportedParameterError(self.padding)
 
+        padded_w = width + 2 * pad_w
         return pad_w, padded_w
 
     def out_shape(self, in_shape: Tuple[int]) -> Tuple[int]:
         batch_size, _, width = in_shape
         _, padded_w = self._get_padding_dim(width)
-        out_width = ((padded_w - self.filter_size) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size[0]) // self.stride) + 1
 
         return (batch_size, self.out_channels, out_width)
 
 
 class _Conv2D(Layer):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        filter_size: int,
+        filter_size: Tuple[int, int] | int,
         stride: int = 1,
-        padding: Literal["valid", "same"] = "same",
+        padding: Tuple[int, int] | int | Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
         optimizer: Optimizer | None = None,
         lambda_: float = 0.0,
         random_state: int | None = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
-        self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
         self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
         self.random_state = random_state
         self.rs_ = np.random.RandomState(self.random_state)
 
+        if isinstance(filter_size, int):
+            self.filter_size = (filter_size, filter_size)
+        else:
+            self.filter_size = filter_size
+
         self.init_params(
             w_shape=(
                 self.out_channels,
                 self.in_channels,
-                self.filter_size,
-                self.filter_size,
+                *self.filter_size,
             ),
             b_shape=(1, self.out_channels),
         )
         self.set_param_ranges(
             {
                 "in_channels": ("0<,+inf", int),
                 "out_channels": ("0<,+inf", int),
-                "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
     @Tensor.force_dim(4)
@@ -206,16 +217,16 @@
             raise ValueError(
                 f"channels of 'X' does not match with 'in_channels'! "
                 + f"({self.in_channels}!={channels})"
             )
 
         pad_h, pad_w, padded_h, padded_w = self._get_padding_dim(height, width)
 
-        out_height = ((padded_h - self.filter_size) // self.stride) + 1
-        out_width = ((padded_w - self.filter_size) // self.stride) + 1
+        out_height = ((padded_h - self.filter_size[0]) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size[1]) // self.stride) + 1
         out: Tensor = np.zeros(
             (
                 batch_size,
                 self.out_channels,
                 out_height,
                 out_width,
             )
@@ -268,15 +279,18 @@
                 filter_d_out_fft = np.sum(
                     X_fft[:, c] * d_out_fft[:, f].conj(),
                     axis=0,
                 )
                 self.dW[f, c] = np.fft.irfftn(
                     filter_d_out_fft,
                     s=(padded_h, padded_w),
-                )[pad_h : pad_h + self.filter_size, pad_w : pad_w + self.filter_size]
+                )[
+                    pad_h : pad_h + self.filter_size[0],
+                    pad_w : pad_w + self.filter_size[1],
+                ]
 
         self.dW += 2 * self.lambda_ * self.weights_
 
         for i in range(batch_size):
             for c in range(channels):
                 temp = np.zeros((padded_h, padded_w // 2 + 1), dtype=np.complex128)
                 for f in range(self.out_channels):
@@ -290,78 +304,85 @@
             dX_padded[:, :, pad_h:-pad_h, pad_w:-pad_w]
             if pad_h > 0 or pad_w > 0
             else dX_padded
         )
         return self.dX
 
     def _get_padding_dim(self, height: int, width: int) -> Tuple[int, ...]:
-        if self.padding == "same":
-            pad_h = pad_w = (self.filter_size - 1) // 2
-            padded_h = height + 2 * pad_h
-            padded_w = width + 2 * pad_w
-
+        if isinstance(self.padding, tuple):
+            if len(self.padding) != 2:
+                raise ValueError("Padding tuple must have exactly two values.")
+            pad_h, pad_w = self.padding
+        elif isinstance(self.padding, int):
+            pad_h = pad_w = self.padding
+
+        elif self.padding == "same":
+            pad_h = (self.filter_size[0] - 1) // 2
+            pad_w = (self.filter_size[1] - 1) // 2
         elif self.padding == "valid":
             pad_h = pad_w = 0
-            padded_h = height
-            padded_w = width
         else:
             raise UnsupportedParameterError(self.padding)
 
+        padded_h = height + 2 * pad_h
+        padded_w = width + 2 * pad_w
+
         return pad_h, pad_w, padded_h, padded_w
 
     def out_shape(self, in_shape: Tuple[int]) -> Tuple[int]:
         batch_size, _, height, width = in_shape
         _, _, padded_h, padded_w = self._get_padding_dim(height, width)
 
-        out_height = ((padded_h - self.filter_size) // self.stride) + 1
-        out_width = ((padded_w - self.filter_size) // self.stride) + 1
+        out_height = ((padded_h - self.filter_size[0]) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size[1]) // self.stride) + 1
 
         return (batch_size, self.out_channels, out_height, out_width)
 
 
 class _Conv3D(Layer):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        filter_size: int,
+        filter_size: Tuple[int, int, int] | int,
         stride: int = 1,
-        padding: Literal["valid", "same"] = "same",
+        padding: Tuple[int, int, int] | int | Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
         optimizer: Optimizer | None = None,
         lambda_: float = 0.0,
         random_state: int | None = None,
     ) -> None:
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
-        self.filter_size = filter_size
         self.stride = stride
         self.padding = padding
         self.initializer = initializer
         self.optimizer = optimizer
         self.lambda_ = lambda_
         self.random_state = random_state
         self.rs_ = np.random.RandomState(self.random_state)
 
+        if isinstance(filter_size, int):
+            self.filter_size = (filter_size, filter_size, filter_size)
+        else:
+            self.filter_size = filter_size
+
         self.init_params(
             w_shape=(
                 self.out_channels,
                 self.in_channels,
-                self.filter_size,
-                self.filter_size,
-                self.filter_size,
+                *self.filter_size,
             ),
             b_shape=(1, self.out_channels),
         )
         self.set_param_ranges(
             {
                 "in_channels": ("0<,+inf", int),
                 "out_channels": ("0<,+inf", int),
-                "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
                 "lambda_": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
     @Tensor.force_dim(5)
@@ -375,17 +396,17 @@
                 f"channels of 'X' does not match with 'in_channels'! "
                 + f"({self.in_channels}!={channels})"
             )
 
         pad_d, pad_h, pad_w, padded_d, padded_h, padded_w = self._get_padding_dim(
             depth, height, width
         )
-        out_depth = ((padded_d - self.filter_size) // self.stride) + 1
-        out_height = ((padded_h - self.filter_size) // self.stride) + 1
-        out_width = ((padded_w - self.filter_size) // self.stride) + 1
+        out_depth = ((padded_d - self.filter_size[0]) // self.stride) + 1
+        out_height = ((padded_h - self.filter_size[1]) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size[2]) // self.stride) + 1
         out: Tensor = np.zeros(
             (batch_size, self.out_channels, out_depth, out_height, out_width)
         )
 
         X_padded = np.pad(
             X,
             ((0, 0), (0, 0), (pad_d, pad_d), (pad_h, pad_h), (pad_w, pad_w)),
@@ -454,17 +475,17 @@
                     X_fft[:, c] * d_out_fft[:, f].conj(),
                     axis=0,
                 )
                 self.dW[f, c] = np.fft.irfftn(
                     filter_d_out_fft,
                     s=(padded_d, padded_h, padded_w),
                 )[
-                    pad_d : pad_d + self.filter_size,
-                    pad_h : pad_h + self.filter_size,
-                    pad_w : pad_w + self.filter_size,
+                    pad_d : pad_d + self.filter_size[0],
+                    pad_h : pad_h + self.filter_size[1],
+                    pad_w : pad_w + self.filter_size[2],
                 ]
 
         self.dW += 2 * self.lambda_ * self.weights_
 
         for i in range(batch_size):
             for c in range(channels):
                 temp = np.zeros(
@@ -491,33 +512,39 @@
 
     def _get_padding_dim(
         self,
         depth: int,
         height: int,
         width: int,
     ) -> Tuple[int, ...]:
-        if self.padding == "same":
-            pad_d = pad_h = pad_w = (self.filter_size - 1) // 2
-            padded_d = depth + 2 * pad_d
-            padded_h = height + 2 * pad_h
-            padded_w = width + 2 * pad_w
-
+        if isinstance(self.padding, tuple):
+            if len(self.padding) != 3:
+                raise ValueError("Padding tuple must have exactly three values.")
+            pad_d, pad_h, pad_w = self.padding
+
+        elif isinstance(self.padding, int):
+            pad_d = pad_h = pad_w = self.padding
+        elif self.padding == "same":
+            pad_d = (self.filter_size[0] - 1) // 2
+            pad_h = (self.filter_size[1] - 1) // 2
+            pad_w = (self.filter_size[2] - 1) // 2
         elif self.padding == "valid":
             pad_d = pad_h = pad_w = 0
-            padded_d = depth
-            padded_h = height
-            padded_w = width
         else:
             raise UnsupportedParameterError(self.padding)
 
+        padded_d = depth + 2 * pad_d
+        padded_h = height + 2 * pad_h
+        padded_w = width + 2 * pad_w
+
         return pad_d, pad_h, pad_w, padded_d, padded_h, padded_w
 
     def out_shape(self, in_shape: Tuple[int]) -> Tuple[int]:
         batch_size, _, depth, height, width = in_shape
         _, _, _, padded_d, padded_h, padded_w = self._get_padding_dim(
             depth, height, width
         )
-        out_depth = ((padded_d - self.filter_size) // self.stride) + 1
-        out_height = ((padded_h - self.filter_size) // self.stride) + 1
-        out_width = ((padded_w - self.filter_size) // self.stride) + 1
+        out_depth = ((padded_d - self.filter_size[0]) // self.stride) + 1
+        out_height = ((padded_h - self.filter_size[1]) // self.stride) + 1
+        out_width = ((padded_w - self.filter_size[2]) // self.stride) + 1
 
         return (batch_size, self.out_channels, out_depth, out_height, out_width)
```

### Comparing `luma-ml-0.8.1/luma/neural/_layers/_drop.py` & `luma-ml-0.8.2/luma/neural/_layers/_drop.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/_layers/_linear.py` & `luma-ml-0.8.2/luma/neural/_layers/_linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/_layers/_norm.py` & `luma-ml-0.8.2/luma/neural/_layers/_norm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/_models/_imagenet.py` & `luma-ml-0.8.2/luma/neural/_models/_vgg.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,455 +9,26 @@
 from luma.neural.base import Loss, NeuralModel
 from luma.neural.loss import CrossEntropy
 from luma.neural.block import ConvBlock2D, DenseBlock, ConvBlockArgs, DenseBlockArgs
 from luma.neural.layer import (
     Activation,
     Dense,
     Flatten,
-    LocalResponseNorm,
     Sequential,
 )
 
 
 __all__ = (
-    "_AlexNet",
-    "_ZFNet",
     "_VGGNet_11",
     "_VGGNet_13",
     "_VGGNet_16",
     "_VGGNet_19",
 )
 
 
-class _AlexNet(Estimator, Supervised, NeuralModel):
-    def __init__(
-        self,
-        optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
-        initializer: InitUtil.InitStr = None,
-        out_features: int = 1000,
-        batch_size: int = 128,
-        n_epochs: int = 100,
-        learning_rate: float = 0.01,
-        valid_size: float = 0.1,
-        lambda_: float = 0.0,
-        dropout_rate: float = 0.5,
-        early_stopping: bool = False,
-        patience: int = 10,
-        shuffle: bool = True,
-        random_state: int = None,
-        deep_verbose: bool = False,
-    ) -> None:
-        self.activation = activation
-        self.optimizer = optimizer
-        self.loss = loss
-        self.initializer = initializer
-        self.out_features = out_features
-        self.lambda_ = lambda_
-        self.dropout_rate = dropout_rate
-        self.shuffle = shuffle
-        self.random_state = random_state
-        self._fitted = False
-
-        super().__init__(
-            batch_size,
-            n_epochs,
-            learning_rate,
-            valid_size,
-            early_stopping,
-            patience,
-            deep_verbose,
-        )
-        super().__init_model__()
-        self.model = Sequential()
-        self.optimizer.set_params(learning_rate=self.learning_rate)
-        self.model.set_optimizer(optimizer=self.optimizer)
-
-        self.feature_sizes_ = [
-            [3, 96, 256, 384, 384, 256],
-            [256 * 6 * 6, 4096, 4096, self.out_features],
-        ]
-        self.feature_shapes_ = [
-            self._get_feature_shapes(self.feature_sizes_[0]),
-            self._get_feature_shapes(self.feature_sizes_[1]),
-        ]
-
-        self.set_param_ranges(
-            {
-                "out_features": ("0<,+inf", int),
-                "batch_size": ("0<,+inf", int),
-                "n_epochs": ("0<,+inf", int),
-                "learning_rate": ("0<,+inf", None),
-                "valid_size": ("0<,<1", None),
-                "dropout_rate": ("0,1", None),
-                "lambda_": ("0,+inf", None),
-                "patience": (f"0<,+inf", int),
-            }
-        )
-        self.check_param_ranges()
-        self._build_model()
-
-    def _build_model(self) -> None:
-        conv_3x3_no_pool_arg = ConvBlockArgs(
-            filter_size=3,
-            stride=1,
-            activation=self.activation,
-            initializer=self.initializer,
-            padding="same",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            do_pooling=False,
-            random_state=self.random_state,
-        )
-        dense_args = DenseBlockArgs(
-            activation=self.activation,
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            dropout_rate=self.dropout_rate,
-            random_state=self.random_state,
-        )
-
-        self.model += (
-            "ConvBlock_1",
-            ConvBlock2D(
-                3,
-                96,
-                filter_size=11,
-                stride=4,
-                activation=self.activation,
-                initializer=self.initializer,
-                padding="valid",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_1",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_2",
-            ConvBlock2D(
-                96,
-                256,
-                filter_size=5,
-                stride=1,
-                activation=self.activation,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_2",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_3",
-            ConvBlock2D(256, 384, **asdict(conv_3x3_no_pool_arg)),
-        )
-        self.model += (
-            "LRN_3",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_4",
-            ConvBlock2D(384, 384, **asdict(conv_3x3_no_pool_arg)),
-        )
-        self.model += (
-            "LRN_4",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_5",
-            ConvBlock2D(
-                384,
-                256,
-                filter_size=3,
-                stride=1,
-                activation=self.activation,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_5",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += Flatten()
-        self.model += (
-            "DenseBlock_1",
-            DenseBlock(256 * 6 * 6, 4096, **asdict(dense_args)),
-        )
-        self.model += (
-            "DenseBlock_2",
-            DenseBlock(4096, 4096, **asdict(dense_args)),
-        )
-        self.model += Dense(
-            4096,
-            self.out_features,
-            lambda_=self.lambda_,
-            random_state=self.random_state,
-        )
-
-    @Tensor.force_dim(4)
-    def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_AlexNet, self).fit_nn(X, y)
-
-    @override
-    @Tensor.force_dim(4)
-    def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_AlexNet, self).predict_nn(X, argmax)
-
-    @override
-    @Tensor.force_dim(4)
-    def score(
-        self,
-        X: Tensor,
-        y: Matrix,
-        metric: Evaluator = Accuracy,
-        argmax: bool = True,
-    ) -> float:
-        return super(_AlexNet, self).score_nn(X, y, metric, argmax)
-
-
-class _ZFNet(Estimator, Supervised, NeuralModel):
-    def __init__(
-        self,
-        optimizer: Optimizer,
-        activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
-        initializer: InitUtil.InitStr = None,
-        out_features: int = 1000,
-        batch_size: int = 128,
-        n_epochs: int = 100,
-        learning_rate: float = 0.01,
-        valid_size: float = 0.1,
-        lambda_: float = 0.0,
-        dropout_rate: float = 0.5,
-        early_stopping: bool = False,
-        patience: int = 10,
-        shuffle: bool = True,
-        random_state: int = None,
-        deep_verbose: bool = False,
-    ) -> None:
-        self.activation = activation
-        self.optimizer = optimizer
-        self.loss = loss
-        self.initializer = initializer
-        self.out_features = out_features
-        self.lambda_ = lambda_
-        self.dropout_rate = dropout_rate
-        self.shuffle = shuffle
-        self.random_state = random_state
-        self._fitted = False
-
-        super().__init__(
-            batch_size,
-            n_epochs,
-            learning_rate,
-            valid_size,
-            early_stopping,
-            patience,
-            deep_verbose,
-        )
-        super().__init_model__()
-        self.model = Sequential()
-        self.optimizer.set_params(learning_rate=self.learning_rate)
-        self.model.set_optimizer(optimizer=self.optimizer)
-
-        self.feature_sizes_ = [
-            [3, 96, 256, 384, 384, 256],
-            [256 * 6 * 6, 4096, 4096, self.out_features],
-        ]
-        self.feature_shapes_ = [
-            self._get_feature_shapes(self.feature_sizes_[0]),
-            self._get_feature_shapes(self.feature_sizes_[1]),
-        ]
-
-        self.set_param_ranges(
-            {
-                "out_features": ("0<,+inf", int),
-                "batch_size": ("0<,+inf", int),
-                "n_epochs": ("0<,+inf", int),
-                "learning_rate": ("0<,+inf", None),
-                "valid_size": ("0<,<1", None),
-                "dropout_rate": ("0,1", None),
-                "lambda_": ("0,+inf", None),
-                "patience": (f"0<,+inf", int),
-            }
-        )
-        self.check_param_ranges()
-        self._build_model()
-
-    def _build_model(self) -> None:
-        conv_3x3_no_pool_arg = ConvBlockArgs(
-            filter_size=3,
-            stride=1,
-            activation=self.activation,
-            initializer=self.initializer,
-            padding="same",
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            do_pooling=False,
-            random_state=self.random_state,
-        )
-        dense_args = DenseBlockArgs(
-            activation=self.activation,
-            lambda_=self.lambda_,
-            do_batch_norm=False,
-            dropout_rate=self.dropout_rate,
-            random_state=self.random_state,
-        )
-
-        self.model += (
-            "ConvBlock_1",
-            ConvBlock2D(
-                3,
-                96,
-                filter_size=7,
-                stride=2,
-                activation=self.activation,
-                initializer=self.initializer,
-                padding="valid",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_1",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_2",
-            ConvBlock2D(
-                96,
-                256,
-                filter_size=5,
-                stride=2,
-                activation=self.activation,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_2",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_3",
-            ConvBlock2D(256, 384, **asdict(conv_3x3_no_pool_arg)),
-        )
-        self.model += (
-            "LRN_3",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_4",
-            ConvBlock2D(384, 384, **asdict(conv_3x3_no_pool_arg)),
-        )
-        self.model += (
-            "LRN_4",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += (
-            "ConvBlock_5",
-            ConvBlock2D(
-                384,
-                256,
-                filter_size=3,
-                stride=1,
-                activation=self.activation,
-                initializer=self.initializer,
-                padding="same",
-                lambda_=self.lambda_,
-                do_batch_norm=False,
-                pool_filter_size=3,
-                pool_stride=2,
-                pool_mode="max",
-                random_state=self.random_state,
-            ),
-        )
-        self.model += (
-            "LRN_5",
-            LocalResponseNorm(depth=5),
-        )
-
-        self.model += Flatten()
-        self.model += (
-            "DenseBlock_1",
-            DenseBlock(256 * 6 * 6, 4096, **asdict(dense_args)),
-        )
-        self.model += (
-            "DenseBlock_2",
-            DenseBlock(4096, 4096, **asdict(dense_args)),
-        )
-        self.model += Dense(
-            4096,
-            self.out_features,
-            lambda_=self.lambda_,
-            random_state=self.random_state,
-        )
-
-    @Tensor.force_dim(4)
-    def fit(self, X: Tensor, y: Matrix) -> Self:
-        return super(_ZFNet, self).fit_nn(X, y)
-
-    @override
-    @Tensor.force_dim(4)
-    def predict(self, X: Tensor, argmax: bool = True) -> Matrix | Vector:
-        return super(_ZFNet, self).predict_nn(X, argmax)
-
-    @override
-    @Tensor.force_dim(4)
-    def score(
-        self,
-        X: Tensor,
-        y: Matrix,
-        metric: Evaluator = Accuracy,
-        argmax: bool = True,
-    ) -> float:
-        return super(_ZFNet, self).score_nn(X, y, metric, argmax)
-
-
 class _VGGNet_11(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
         loss: Loss = CrossEntropy(),
         initializer: InitUtil.InitStr = None,
@@ -467,15 +38,15 @@
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
         self.out_features = out_features
@@ -639,15 +210,15 @@
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
         self.out_features = out_features
@@ -823,15 +394,15 @@
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
         self.out_features = out_features
@@ -1019,15 +590,15 @@
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
         dropout_rate: float = 0.5,
         early_stopping: bool = False,
         patience: int = 10,
         shuffle: bool = True,
-        random_state: int = None,
+        random_state: int | None = None,
         deep_verbose: bool = False,
     ) -> None:
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
         self.out_features = out_features
```

### Comparing `luma-ml-0.8.1/luma/neural/_models/_lenet.py` & `luma-ml-0.8.2/luma/neural/_models/_lenet.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/_models/_simple.py` & `luma-ml-0.8.2/luma/neural/_models/_simple.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/base.py` & `luma-ml-0.8.2/luma/neural/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/init.py` & `luma-ml-0.8.2/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/layer.py` & `luma-ml-0.8.2/luma/neural/layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, List, Literal, Self, Tuple, override
 
 from luma.core.super import Optimizer
 from luma.interface.typing import TensorLike
 from luma.interface.util import InitUtil, Clone
 from luma.neural.base import Layer
 
-from ._layers import (
+from luma.neural._layers import (
     _act,
     _conv,
     _drop,
     _linear,
     _norm,
     _pool,
 )
@@ -18,14 +18,20 @@
 __all__ = (
     "Convolution1D",
     "Convolution2D",
     "Convolution3D",
     "Pooling1D",
     "Pooling2D",
     "Pooling3D",
+    "GlobalAvgPooling1D",
+    "GlobalAvgPooling2D",
+    "GlobalAvgPooling3D",
+    "LpPooling1D",
+    "LpPooling2D",
+    "LpPooling3D",
     "Dense",
     "Dropout",
     "Dropout1D",
     "Dropout2D",
     "Dropout3D",
     "Flatten",
     "Activation",
@@ -50,19 +56,19 @@
 
     Parameters
     ----------
     `in_channels` : int
         Number of input channels
     `out_channels` : int
         Number of output channels(filters)
-    `filter_size`: int
-        Length of each filter
+    `filter_size`: tuple of int or int
+        Size of each filter
     `stride` : int, default=1
         Step size for filters during convolution
-    `padding` : {"valid", "same"}, default="same"
+    `padding` : tuple of int or int or {"valid", "same"}, default="same"
         Padding strategies ("valid" for no padding, "same" for zero-padding)
     `initializer` : InitStr, default=None
         Type of weight initializer
     `optimizer` : Optimizer, optional, default=None
         Optimizer for weight update
     `lambda_` : float, default=0.0
         L2-regularization strength
@@ -78,17 +84,17 @@
         ```
     """
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        filter_size: int,
+        filter_size: Tuple[int] | int,
         stride: int = 1,
-        padding: Literal["valid", "same"] = "same",
+        padding: Tuple[int] | int | Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
         optimizer: Optimizer | None = None,
         lambda_: float = 0,
         random_state: int | None = None,
     ) -> None:
         super().__init__(
             in_channels,
@@ -115,19 +121,19 @@
 
     Parameters
     ----------
     `in_channels` : int
         Number of input channels
     `out_channels` : int
         Number of output channels(filters)
-    `filter_size`: int
-        Length of each filter
+    `filter_size`: tuple of int or int
+        Size of each filter
     `stride` : int, default=1
         Step size for filters during convolution
-    `padding` : {"valid", "same"}, default="same"
+    `padding` : tuple of int or int or {"valid", "same"}, default="same"
         Padding strategies ("valid" for no padding, "same" for zero-padding)
     `initializer` : InitStr, default=None
         Type of weight initializer
     `optimizer` : Optimizer, optional, default=None
         Optimizer for weight update
     `lambda_` : float, default=0.0
         L2-regularization strength
@@ -143,17 +149,17 @@
         ```
     """
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        filter_size: int,
+        filter_size: Tuple[int, int] | int,
         stride: int = 1,
-        padding: Literal["valid", "same"] = "same",
+        padding: Tuple[int, int] | int | Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
         optimizer: Optimizer = None,
         lambda_: float = 0,
         random_state: int = None,
     ) -> None:
         super().__init__(
             in_channels,
@@ -180,19 +186,19 @@
 
     Parameters
     ----------
     `in_channels` : int
         Number of input channels
     `out_channels` : int
         Number of output channels(filters)
-    `filter_size`: int
-        Length of each filter
+    `filter_size`: tuple of int or int
+        Size of each filter
     `stride` : int, default=1
         Step size for filters during convolution
-    `padding` : {"valid", "same"}, default="same"
+    `padding` : tuple of int or int or {"valid", "same"}, default="same"
         Padding strategies ("valid" for no padding, "same" for zero-padding)
     `initializer` : InitStr, default=None
         Type of weight initializer
     `optimizer` : Optimizer, optional, default=None
         Optimizer for weight update
     `lambda_` : float, default=0.0
         L2-regularization strength
@@ -208,17 +214,17 @@
         ```
     """
 
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
-        filter_size: int,
+        filter_size: Tuple[int, int, int] | int,
         stride: int = 1,
-        padding: Literal["valid", "same"] = "same",
+        padding: Tuple[int, int, int] | int | Literal["valid", "same"] = "same",
         initializer: InitUtil.InitStr = None,
         optimizer: Optimizer = None,
         lambda_: float = 0,
         random_state: int = None,
     ) -> None:
         super().__init__(
             in_channels,
@@ -249,14 +255,16 @@
     ----------
     `filter_size` : int, default=2
         Size of the pooling filter
     `stride` : int, default=2
         Step size of the filter during pooling
     `mode` : {"max", "avg"}, default="max"
         Pooling strategy (i.e., 'max' or 'avg')
+    `padding` : tuple of int or int or {"valid", "same"}, default="valid"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
 
     Notes
     -----
     - The input `X` must have the form of 3D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, width)
@@ -264,16 +272,17 @@
     """
 
     def __init__(
         self,
         filter_size: int = 2,
         stride: int = 2,
         mode: Literal["max", "avg"] = "max",
+        padding: Tuple[int] | int | Literal["valid", "same"] = "valid",
     ) -> None:
-        super().__init__(filter_size, stride, mode)
+        super().__init__(filter_size, stride, mode, padding)
 
 
 class Pooling2D(_pool._Pool2D):
     """
     Pooling layer for 2-dimensional data.
 
     A pooling layer in a neural network reduces the spatial dimensions of
@@ -288,14 +297,16 @@
     ----------
     `filter_size` : int, default=2
         Size of the pooling filter
     `stride` : int, default=2
         Step size of the filter during pooling
     `mode` : {"max", "avg"}, default="max"
         Pooling strategy (i.e., 'max' or 'avg')
+    `padding` : tuple of int or int or {"valid", "same"}, default="valid"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
 
     Notes
     -----
     - The input `X` must have the form of 4D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, height, width)
@@ -303,16 +314,17 @@
     """
 
     def __init__(
         self,
         filter_size: int = 2,
         stride: int = 2,
         mode: Literal["max", "avg"] = "max",
+        padding: Tuple[int, int] | int | Literal["valid", "same"] = "valid",
     ) -> None:
-        super().__init__(filter_size, stride, mode)
+        super().__init__(filter_size, stride, mode, padding)
 
 
 class Pooling3D(_pool._Pool3D):
     """
     Pooling layer for 3-dimensional data.
 
     A pooling layer in a neural network reduces the spatial dimensions of
@@ -327,14 +339,16 @@
     ----------
     `filter_size` : int, default=2
         Size of the pooling filter
     `stride` : int, default=2
         Step size of the filter during pooling
     `mode` : {"max", "avg"}, default="max"
         Pooling strategy (i.e., 'max' or 'avg')
+    `padding` : tuple of int or int or {"valid", "same"}, default="valid"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
 
     Notes
     -----
     - The input `X` must have the form of 5D-array(`Tensor`).
 
         ```py
         X.shape = (batch_size, channels, depth, height, width)
@@ -342,16 +356,212 @@
     """
 
     def __init__(
         self,
         filter_size: int = 2,
         stride: int = 2,
         mode: Literal["max", "avg"] = "max",
+        padding: Tuple[int, int, int] | int | Literal["valid", "same"] = "valid",
+    ) -> None:
+        super().__init__(filter_size, stride, mode, padding)
+
+
+class GlobalAvgPooling1D(_pool._GlobalAvgPool1D):
+    """
+    Global average pooling layer for 1-dimensional data.
+
+    Global Average Pooling (GAP) is a downsampling technique in Convolutional
+    Neural Networks (CNNs) that reduces each feature map to a single value by
+    taking the average of all its elements. It effectively transforms a
+    multi-dimensional feature map into a one-dimensional vector, which helps in
+    reducing the number of parameters and avoiding overfitting.
+    GAP is commonly used in classification tasks, particularly in the final layer
+    before the output layer.
+
+    Notes
+    -----
+    - The input `X` must have the form of 3D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, width)
+        ```
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+
+class GlobalAvgPooling2D(_pool._GlobalAvgPool2D):
+    """
+    Global average pooling layer for 2-dimensional data.
+
+    Global Average Pooling (GAP) is a downsampling technique in Convolutional
+    Neural Networks (CNNs) that reduces each feature map to a single value by
+    taking the average of all its elements. It effectively transforms a
+    multi-dimensional feature map into a one-dimensional vector, which helps in
+    reducing the number of parameters and avoiding overfitting.
+    GAP is commonly used in classification tasks, particularly in the final layer
+    before the output layer.
+
+    Notes
+    -----
+    - The input `X` must have the form of 4D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, height, width)
+        ```
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+
+class GlobalAvgPooling3D(_pool._GlobalAvgPool3D):
+    """
+    Global average pooling layer for 3-dimensional data.
+
+    Global Average Pooling (GAP) is a downsampling technique in Convolutional
+    Neural Networks (CNNs) that reduces each feature map to a single value by
+    taking the average of all its elements. It effectively transforms a
+    multi-dimensional feature map into a one-dimensional vector, which helps in
+    reducing the number of parameters and avoiding overfitting.
+    GAP is commonly used in classification tasks, particularly in the final layer
+    before the output layer.
+
+    Notes
+    -----
+    - The input `X` must have the form of 5D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, depth, height, width)
+        ```
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+
+class LpPooling1D(_pool._LpPool1D):
+    """
+    Lp pooling layer for 1-dimensional data.
+
+    Lp Pooling is a generalized pooling method where the pooling operation is
+    based on the Lp norm. It computes the p-th power of the absolute values within
+    a pooling window, sums them up, and then takes the p-th root of this sum.
+    This approach provides a smooth transition between average pooling (p=1) and
+    max pooling (p approaching infinity).
+
+    Parameters
+    ----------
+    `filter_size` : int, default=2
+        Size of the pooling filter
+    `stride` : int, default=2
+        Step size of the filter during pooling
+    `p` : float, default=2.0
+        Powering factor for Lp norm.
+    `padding` : tuple of int or int or {"valid", "same"}, default="valid"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
+
+    Notes
+    -----
+    - The input `X` must have the form of 3D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, width)
+        ```
+    """
+
+    def __init__(
+        self,
+        filter_size: int = 2,
+        stride: int = 2,
+        p: float = 2,
+        padding: Tuple[int] | int | Literal["same", "valid"] = "valid",
+    ) -> None:
+        super().__init__(filter_size, stride, p, padding)
+
+
+class LpPooling2D(_pool._LpPool2D):
+    """
+    Lp pooling layer for 2-dimensional data.
+
+    Lp Pooling is a generalized pooling method where the pooling operation is
+    based on the Lp norm. It computes the p-th power of the absolute values within
+    a pooling window, sums them up, and then takes the p-th root of this sum.
+    This approach provides a smooth transition between average pooling (p=1) and
+    max pooling (p approaching infinity).
+
+    Parameters
+    ----------
+    `filter_size` : int, default=2
+        Size of the pooling filter
+    `stride` : int, default=2
+        Step size of the filter during pooling
+    `p` : float, default=2.0
+        Powering factor for Lp norm.
+    `padding` : tuple of int or int or {"valid", "same"}, default="valid"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
+
+    Notes
+    -----
+    - The input `X` must have the form of 4D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, height, width)
+        ```
+    """
+
+    def __init__(
+        self,
+        filter_size: int = 2,
+        stride: int = 2,
+        p: float = 2,
+        padding: Tuple[int, int] | int | Literal["same", "valid"] = "valid",
+    ) -> None:
+        super().__init__(filter_size, stride, p, padding)
+
+
+class LpPooling3D(_pool._LpPool3D):
+    """
+    Lp pooling layer for 3-dimensional data.
+
+    Lp Pooling is a generalized pooling method where the pooling operation is
+    based on the Lp norm. It computes the p-th power of the absolute values within
+    a pooling window, sums them up, and then takes the p-th root of this sum.
+    This approach provides a smooth transition between average pooling (p=1) and
+    max pooling (p approaching infinity).
+
+    Parameters
+    ----------
+    `filter_size` : int, default=2
+        Size of the pooling filter
+    `stride` : int, default=2
+        Step size of the filter during pooling
+    `p` : float, default=2.0
+        Powering factor for Lp norm.
+    `padding` : tuple of int or int or {"valid", "same"}, default="valid"
+        Padding strategies ("valid" for no padding, "same" for zero-padding)
+
+    Notes
+    -----
+    - The input `X` must have the form of 5D-array(`Tensor`).
+
+        ```py
+        X.shape = (batch_size, channels, depth, height, width)
+        ```
+    """
+
+    def __init__(
+        self,
+        filter_size: int = 2,
+        stride: int = 2,
+        p: float = 2,
+        padding: Tuple[int, int, int] | int | Literal["same", "valid"] = "valid",
     ) -> None:
-        super().__init__(filter_size, stride, mode)
+        super().__init__(filter_size, stride, p, padding)
 
 
 class Dense(_linear._Dense):
     """
     A dense layer, also known as a fully connected layer, connects each
     neuron in one layer to every neuron in the next layer. It performs a
     linear transformation followed by a nonlinear activation function,
@@ -732,15 +942,15 @@
     to the next in the order they are added. This organization simplifies the
     construction of neural networks, especially for straightforward architectures,
     by mirroring the logical flow of data from input through hidden layers to
     output.
 
     Parameters
     ----------
-    `*layers` : Layer or tuple[str, Layer]
+    `*layers` : Layer or tuple[str, Layer], optional
         Layers or layers with its name assigned
         (class name of the layer assigned by default)
 
     Methods
     -------
     For setting an optimizer of each layer:
     ```py
@@ -780,15 +990,15 @@
 
     out = model(X, is_train=True) # model.forward(X, is_train=True)
     model.backward(d_out) # assume d_out is the gradient w.r.t. loss
     model.update()
     ```
     """
 
-    def __init__(self, *layers: Layer | tuple[str, Layer]) -> None:
+    def __init__(self, *layers: Layer | tuple[str, Layer] | None) -> None:
         super().__init__()
         self.layers: List[tuple[str, Layer]] = list()
         for layer in layers:
             self.add(layer)
 
     def forward(self, X: TensorLike, is_train: bool = False) -> TensorLike:
         self.input_ = X
@@ -822,22 +1032,40 @@
     def _check_no_optimizer(self) -> None:
         if self.optimizer is None:
             raise RuntimeError(
                 f"'{self}' has no optimizer! "
                 + f"Call '{self}().set_optimizer' to assign an optimizer."
             )
 
-    def add(self, layer: Layer | tuple[str, Layer]) -> None:
+    def add(self, layer: Layer | tuple[str, Layer] | None) -> None:
+        if layer is None:
+            return
         if not isinstance(layer, tuple):
             layer = (str(layer), layer)
         self.layers.append(layer)
 
         if self.optimizer is not None:
             self.set_optimizer(self.optimizer)
 
+    def extend(
+        self,
+        *layers: Self | Layer | tuple[str, Layer] | None,
+        deep_add: bool = True,
+    ) -> None:
+        for layer in layers:
+            new_layer = layer
+            if isinstance(layer, tuple):
+                name, layer = layer
+                new_layer = (name, layer)
+            if hasattr(layer, "layers") and deep_add:
+                for sub_layer in layer.layers:
+                    self.add(sub_layer)
+                continue
+            self.add(new_layer)
+
     @override
     @property
     def param_size(self) -> Tuple[int, int]:
         w_size, b_size = 0, 0
         for _, layer in self.layers:
             w_, b_ = layer.param_size
             w_size += w_
@@ -846,15 +1074,15 @@
         return w_size, b_size
 
     def out_shape(self, in_shape: Tuple[int]) -> Tuple[int]:
         for _, layer in self.layers:
             in_shape = layer.out_shape(in_shape)
         return in_shape
 
-    def __add__(self, other: Layer | tuple[str, Layer]) -> Self:
+    def __add__(self, other: Layer | tuple[str, Layer] | None) -> Self:
         if isinstance(other, (Layer, tuple)):
             self.add(other)
         else:
             raise TypeError(
                 "Unsupported operand type(s) for +: '{}' and '{}'".format(
                     type(self).__name__, type(other).__name__
                 )
```

### Comparing `luma-ml-0.8.1/luma/neural/loss.py` & `luma-ml-0.8.2/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/network.py` & `luma-ml-0.8.2/luma/neural/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 from luma.core.super import Optimizer
 from luma.interface.util import InitUtil
 
 from luma.neural.base import Loss
 from luma.neural.layer import Activation
 from luma.neural.loss import CrossEntropy
 
-from ._models import _simple, _lenet, _imagenet
+from luma.neural._models import _simple, _lenet, _alex, _vgg, _inception
 
 
 __all__ = (
     "SimpleMLP",
     "SimpleCNN",
     "LeNet_1",
     "LeNet_4",
     "LeNet_5",
     "AlexNet",
     "ZFNet",
     "VGGNet_11",
     "VGGNet_13",
     "VGGNet_16",
     "VGGNet_19",
+    "Inception_V1",
+    "Inception_V2",
+    "Inception_V3",
 )
 
 
 class SimpleMLP(_simple._SimpleMLP):
     """
     An MLP (Multilayer Perceptron) is a type of artificial neural network
     composed of at least three layers: an input layer, one or more hidden
@@ -620,15 +623,15 @@
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
-class AlexNet(_imagenet._AlexNet):
+class AlexNet(_alex._AlexNet):
     """
     AlexNet is a deep convolutional neural network that is designed for
     challenging image recognition tasks and was the winning entry in ILSVRC 2012.
     This architecture uses deep layers of convolutions with ReLU activations,
     max pooling, dropout, and fully connected layers leading to a classification
     output.
 
@@ -734,15 +737,15 @@
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
-class ZFNet(_imagenet._ZFNet):
+class ZFNet(_alex._ZFNet):
     """
     ZFNet is a refinement of the AlexNet architecture that was specifically
     designed to improve model understanding and performance on image recognition
     tasks. This model was presented by Matthew Zeiler and Rob Fergus in their
     paper and was particularly notable for its improvements in layer configurations
     that enhanced visualization of intermediate activations, aiding in understanding
     the functioning of deep convolutional networks.
@@ -848,15 +851,15 @@
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
-class VGGNet_11(_imagenet._VGGNet_11):
+class VGGNet_11(_vgg._VGGNet_11):
     """
     VGG11 is a simplified variant of the VGG network architecture that was designed
     to enhance image recognition performance through deeper networks with smaller
     convolutional filters. This model was introduced by Karen Simonyan and Andrew
     Zisserman in their paper and is notable for its simplicity and effectiveness
     in image classification tasks.
 
@@ -964,15 +967,15 @@
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
-class VGGNet_13(_imagenet._VGGNet_13):
+class VGGNet_13(_vgg._VGGNet_13):
     """
     VGG13 is ont of the variants of the VGG network architecture that was designed
     to enhance image recognition performance through deeper networks with smaller
     convolutional filters. This model was introduced by Karen Simonyan and Andrew
     Zisserman in their paper and is notable for its simplicity and effectiveness
     in image classification tasks.
 
@@ -1083,15 +1086,15 @@
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
-class VGGNet_16(_imagenet._VGGNet_16):
+class VGGNet_16(_vgg._VGGNet_16):
     """
     VGG16 is ont of the variants of the VGG network architecture that was designed
     to enhance image recognition performance through deeper networks with smaller
     convolutional filters. This model was introduced by Karen Simonyan and Andrew
     Zisserman in their paper and is notable for its simplicity and effectiveness
     in image classification tasks.
 
@@ -1205,15 +1208,15 @@
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
-class VGGNet_19(_imagenet._VGGNet_19):
+class VGGNet_19(_vgg._VGGNet_19):
     """
     VGG19 is ont of the variants of the VGG network architecture that was designed
     to enhance image recognition performance through deeper networks with smaller
     convolutional filters. This model was introduced by Karen Simonyan and Andrew
     Zisserman in their paper and is notable for its simplicity and effectiveness
     in image classification tasks.
 
@@ -1328,7 +1331,141 @@
             dropout_rate,
             early_stopping,
             patience,
             shuffle,
             random_state,
             deep_verbose,
         )
+
+
+class Inception_V1(_inception._Inception_V1):
+    """
+    Inception v1, also known as GoogLeNet, is a deep convolutional neural network
+    architecture designed for image classification. It introduces an "Inception
+    module," which uses multiple convolutional filters of different sizes in
+    parallel to capture various features at different scales. This architecture
+    reduces computational costs by using 1x1 convolutions to decrease the number
+    of input channels. Inception v1 achieved state-of-the-art results on the
+    ImageNet Large Scale Visual Recognition Challenge (ILSVRC) 2014.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 224, 224]
+    ```
+    Introductory Convolutions:
+    ```py
+    ConvBlock2D(3, 64, filter_size=7, pool_mode="max") ->
+    ConvBlock2D(64, 64, filter_size=1, do_pooling=False) ->
+    ConvBlock2D(64, 192, filter_size=3, pool_mode="max") ->
+    ```
+    Inception Blocks:
+    ```py
+    InceptionBlock(192, 64, 96, 128, 16, 32, 32) ->  # Inception_3a
+    InceptionBlock(256, 128, 128, 192, 32, 96, 64) ->  # Inception_3b
+    Pooling2D(3, 2, mode="max")
+
+    InceptionBlock(480, 192, 96, 208, 16, 48, 64) ->  # Inception_4a
+    InceptionBlock(512, 160, 112, 224, 24, 64, 64) ->  # Inception_4b
+    InceptionBlock(512, 128, 128, 256, 24, 64, 64) ->  # Inception_4c
+    InceptionBlock(512, 112, 144, 288, 32, 64, 64) ->  # Inception_4d
+    InceptionBlock(528, 256, 160, 320, 32, 128, 128) ->  # Inception_4e
+    Pooling2D(3, 2, mode="max")
+
+    InceptionBlock(832, 256, 160, 320, 32, 128, 128) ->  # Inception_5a
+    InceptionBlock(832, 384, 192, 384, 48, 128, 128) ->  # Inception_5b
+    GlobalAvgPooling2D() ->
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten -> Dense(1024, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    6,990,272 weights, 8,280 biases -> 6,998,552 params
+    ```
+    Parameters
+    ----------
+    `activation` : FuncType, default=Activation.ReLU
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Szegedy, Christian, et al. “Going Deeper with Convolutions.” Proceedings
+    of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR),
+    2015, pp. 1-9.
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.ReLU,
+        loss: Loss = CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 128,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0.0,
+        dropout_rate: float = 0.4,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int | None = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
+
+
+class Inception_V2(_inception._Inception_V2):
+    NotImplemented
+
+
+class Inception_V3(_inception._Inception_V3):
+    NotImplemented
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `luma-ml-0.8.1/luma/neural/optimizer.py` & `luma-ml-0.8.2/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/neural/single.py` & `luma-ml-0.8.2/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/pipe/pipeline.py` & `luma-ml-0.8.2/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/preprocessing/encoder.py` & `luma-ml-0.8.2/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/preprocessing/imputer.py` & `luma-ml-0.8.2/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/preprocessing/outlier.py` & `luma-ml-0.8.2/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/preprocessing/scaler.py` & `luma-ml-0.8.2/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/reduction/linear.py` & `luma-ml-0.8.2/luma/reduction/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 from luma.interface.exception import (
     NotFittedError,
     NotConvergedError,
     UnsupportedParameterError,
 )
 
 
-__all__ = ("PCA", "LDA", "KDA", "CCA", "KernelPCA", "TruncatedSVD", "FactorAnalysis")
+__all__ = (
+    "PCA",
+    "LDA",
+    "KDA",
+    "CCA",
+    "KernelPCA",
+    "TruncatedSVD",
+    "FactorAnalysis",
+)
 
 
 class PCA(Transformer, Unsupervised):
     """
     PCA, or Principal Component Analysis, is a dimensionality
     reduction technique. It's primarily used to simplify complex
     data while retaining the most important information.
```

### Comparing `luma-ml-0.8.1/luma/reduction/manifold.py` & `luma-ml-0.8.2/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/reduction/selection.py` & `luma-ml-0.8.2/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/general.py` & `luma-ml-0.8.2/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/linear.py` & `luma-ml-0.8.2/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/neighbors.py` & `luma-ml-0.8.2/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/poly.py` & `luma-ml-0.8.2/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/robust.py` & `luma-ml-0.8.2/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/svm.py` & `luma-ml-0.8.2/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/regressor/tree.py` & `luma-ml-0.8.2/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/visual/eda.py` & `luma-ml-0.8.2/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma/visual/evaluation.py` & `luma-ml-0.8.2/luma/visual/eval.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.1/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.8.2/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.71k-red">
+        <img src="https://img.shields.io/badge/total downloads-6.04k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.1</td>
+                    <td>0.8.2</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~23.8K</td>
+                    <td>~25.3K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.8.1 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.8.2 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.71k-red][GitHub code size in bytes][Code Style]
+6.04k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.1
-Lines of Code  ~23.8K
+Latest Version 0.8.2
+Lines of Code  ~25.3K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.1/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.8.2/luma_ml.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -45,17 +45,19 @@
 luma/neural/single.py
 luma/neural/_layers/_act.py
 luma/neural/_layers/_conv.py
 luma/neural/_layers/_drop.py
 luma/neural/_layers/_linear.py
 luma/neural/_layers/_norm.py
 luma/neural/_layers/_pool.py
-luma/neural/_models/_imagenet.py
+luma/neural/_models/_alex.py
+luma/neural/_models/_inception.py
 luma/neural/_models/_lenet.py
 luma/neural/_models/_simple.py
+luma/neural/_models/_vgg.py
 luma/pipe/pipeline.py
 luma/preprocessing/encoder.py
 luma/preprocessing/imputer.py
 luma/preprocessing/outlier.py
 luma/preprocessing/scaler.py
 luma/reduction/linear.py
 luma/reduction/manifold.py
@@ -64,15 +66,15 @@
 luma/regressor/linear.py
 luma/regressor/neighbors.py
 luma/regressor/poly.py
 luma/regressor/robust.py
 luma/regressor/svm.py
 luma/regressor/tree.py
 luma/visual/eda.py
-luma/visual/evaluation.py
+luma/visual/eval.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
 test/__act.py
 test/__test.py
```

### Comparing `luma-ml-0.8.1/setup.py` & `luma-ml-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.8.1",
+    version="0.8.2",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.8.1/test/__act.py` & `luma-ml-0.8.2/test/__act.py`

 * *Files identical despite different names*

