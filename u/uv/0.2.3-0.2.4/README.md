# Comparing `tmp/uv-0.2.3.tar.gz` & `tmp/uv-0.2.4.tar.gz`

## Comparing `uv-0.2.3.tar` & `uv-0.2.4.tar`

### file list

```diff
@@ -1,393 +1,393 @@
--rw-r--r--   0     1001      127      752 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/Cargo.toml
--rw-r--r--   0     1001      127     9542 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/cache.rs
--rw-r--r--   0     1001      127    11219 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/credentials.rs
--rw-r--r--   0     1001      127     9340 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/keyring.rs
--rw-r--r--   0     1001      127      992 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/lib.rs
--rw-r--r--   0     1001      127    45581 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/middleware.rs
--rw-r--r--   0     1001      127     4661 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-auth/src/realm.rs
--rw-r--r--   0     1001      127      790 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/Cargo.toml
--rw-r--r--   0     1001      127      423 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/builds.rs
--rw-r--r--   0     1001      127      239 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/downloads.rs
--rw-r--r--   0     1001      127     6237 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/hash.rs
--rw-r--r--   0     1001      127      219 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/lib.rs
--rw-r--r--   0     1001      127     1478 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/requirements.rs
--rw-r--r--   0     1001      127     6944 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-types/src/traits.rs
--rw-r--r--   0     1001      127     1121 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/Cargo.toml
--rw-r--r--   0     1001      127     2527 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/annotation.rs
--rw-r--r--   0     1001      127     1048 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/any.rs
--rw-r--r--   0     1001      127     4667 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/buildable.rs
--rw-r--r--   0     1001      127     6720 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/cached.rs
--rw-r--r--   0     1001      127      280 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/diagnostic.rs
--rw-r--r--   0     1001      127     2474 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/editable.rs
--rw-r--r--   0     1001      127      985 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/error.rs
--rw-r--r--   0     1001      127     7205 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/file.rs
--rw-r--r--   0     1001      127     2831 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/hash.rs
--rw-r--r--   0     1001      127     3845 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/id.rs
--rw-r--r--   0     1001      127    14472 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/index_url.rs
--rw-r--r--   0     1001      127    12906 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/installed.rs
--rw-r--r--   0     1001      127    35900 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/lib.rs
--rw-r--r--   0     1001      127    20983 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/prioritized_distribution.rs
--rw-r--r--   0     1001      127     8297 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/requirement.rs
--rw-r--r--   0     1001      127     1228 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/requirements.rs
--rw-r--r--   0     1001      127     8062 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/resolution.rs
--rw-r--r--   0     1001      127     7176 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/resolved.rs
--rw-r--r--   0     1001      127     3015 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/specified_requirement.rs
--rw-r--r--   0     1001      127     8193 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-types/src/traits.rs
--rw-r--r--   0     1001      127      507 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/Cargo.toml
--rw-r--r--   0     1001      127     8335 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/cache_key.rs
--rw-r--r--   0     1001      127    12317 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/canonical_url.rs
--rw-r--r--   0     1001      127      620 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/digest.rs
--rw-r--r--   0     1001      127      191 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/lib.rs
--rw-r--r--   0     1001      127     1986 2024-05-24 18:20:15.000000 uv-0.2.3/crates/cache-key/src/stable_hash.rs
--rw-r--r--   0     1001      127     1004 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/License-BSD
--rw-r--r--   0     1001      127     2947 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/Readme.md
--rw-r--r--   0     1001      127     2105 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/python/Readme.md
--rw-r--r--   0     1001      127     2922 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/src/lib.rs
--rw-r--r--   0     1001      127   131052 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/src/version.rs
--rw-r--r--   0     1001      127    56892 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep440-rs/src/version_specifier.rs
--rw-r--r--   0     1001      127      918 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/Cargo.toml
--rw-r--r--   0     1001      127    63247 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/git.rs
--rw-r--r--   0     1001      127    37494 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/known_hosts.rs
--rw-r--r--   0     1001      127     3843 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/lib.rs
--rw-r--r--   0     1001      127      940 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/sha.rs
--rw-r--r--   0     1001      127     5058 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/source.rs
--rw-r--r--   0     1001      127     1362 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/util/errors.rs
--rw-r--r--   0     1001      127      733 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/util/mod.rs
--rw-r--r--   0     1001      127     7295 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-git/src/util/retry.rs
--rw-r--r--   0     1001      127      456 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-warnings/Cargo.toml
--rw-r--r--   0     1001      127     1701 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-warnings/src/lib.rs
--rw-r--r--   0     1001      127      911 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/Cargo.toml
--rw-r--r--   0     1001      127     1397 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/src/cachedir.rs
--rw-r--r--   0     1001      127    11137 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/src/lib.rs
--rw-r--r--   0     1001      127    12687 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-fs/src/path.rs
--rw-r--r--   0     1001      127     1002 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/Cargo.toml
--rw-r--r--   0     1001      127     7241 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/combine.rs
--rw-r--r--   0     1001      127      127 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/lib.rs
--rw-r--r--   0     1001      127     3296 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/settings.rs
--rw-r--r--   0     1001      127     5560 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-workspace/src/workspace.rs
--rw-r--r--   0     1001      127     1224 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/Cargo.toml
--rw-r--r--   0     1001      127    87285 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/lib.rs
--rw-r--r--   0     1001      127     2038 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/requirement.rs
--rw-r--r--   0     1001      127     6200 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
--rw-r--r--   0     1001      127     2683 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
--rw-r--r--   0     1001      127     2273 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
--rw-r--r--   0     1001      127      284 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
--rw-r--r--   0     1001      127     4140 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1816 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
--rw-r--r--   0     1001      127      828 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
--rw-r--r--   0     1001      127    11863 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     2257 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
--rw-r--r--   0     1001      127     3818 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
--rw-r--r--   0     1001      127     6200 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
--rw-r--r--   0     1001      127     2683 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
--rw-r--r--   0     1001      127     2273 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
--rw-r--r--   0     1001      127      284 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
--rw-r--r--   0     1001      127     4140 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1816 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
--rw-r--r--   0     1001      127      828 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
--rw-r--r--   0     1001      127    11863 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     2257 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
--rw-r--r--   0     1001      127     6684 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap
--rw-r--r--   0     1001      127     8155 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap
--rw-r--r--   0     1001      127     3818 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
--rw-r--r--   0     1001      127     6744 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap
--rw-r--r--   0     1001      127     8161 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap
--rw-r--r--   0     1001      127      113 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/bare-url.txt
--rw-r--r--   0     1001      127       90 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/basic.txt
--rw-r--r--   0     1001      127       45 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
--rw-r--r--   0     1001      127       27 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
--rw-r--r--   0     1001      127      491 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/editable.txt
--rw-r--r--   0     1001      127        0 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/empty.txt
--rw-r--r--   0     1001      127      101 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
--rw-r--r--   0     1001      127       43 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/include-a.txt
--rw-r--r--   0     1001      127        5 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/include-b.txt
--rw-r--r--   0     1001      127     1183 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
--rw-r--r--   0     1001      127       66 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/small.txt
--rw-r--r--   0     1001      127      183 2024-05-24 18:20:15.000000 uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
--rw-r--r--   0     1001      127      322 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-version/Cargo.toml
--rw-r--r--   0     1001      127      355 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-version/src/lib.rs
--rw-r--r--   0     1001      127     2085 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/License-BSD
--rw-r--r--   0     1001      127     3039 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/Readme.md
--rw-r--r--   0     1001      127     4301 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/cursor.rs
--rw-r--r--   0     1001      127    62060 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/lib.rs
--rw-r--r--   0     1001      127    94881 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/marker.rs
--rw-r--r--   0     1001      127      743 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/origin.rs
--rw-r--r--   0     1001      127    13353 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/unnamed.rs
--rw-r--r--   0     1001      127    18647 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pep508-rs/src/verbatim_url.rs
--rw-r--r--   0     1001      127     1528 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/Cargo.toml
--rw-r--r--   0     1001      127      684 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/archive.rs
--rw-r--r--   0     1001      127    34434 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/distribution_database.rs
--rw-r--r--   0     1001      127     2185 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/download.rs
--rw-r--r--   0     1001      127     6943 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/error.rs
--rw-r--r--   0     1001      127    10363 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/git.rs
--rw-r--r--   0     1001      127     7145 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/built_wheel_index.rs
--rw-r--r--   0     1001      127     3435 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/cached_wheel.rs
--rw-r--r--   0     1001      127      162 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/mod.rs
--rw-r--r--   0     1001      127     8729 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/index/registry_wheel_index.rs
--rw-r--r--   0     1001      127      965 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/lib.rs
--rw-r--r--   0     1001      127      600 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/locks.rs
--rw-r--r--   0     1001      127     1225 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/reporter.rs
--rw-r--r--   0     1001      127     2029 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/source/built_wheel_metadata.rs
--rw-r--r--   0     1001      127    60305 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/source/mod.rs
--rw-r--r--   0     1001      127     1998 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-distribution/src/source/revision.rs
--rw-r--r--   0     1001      127      897 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/Cargo.toml
--rw-r--r--   0     1001      127     1078 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/error.rs
--rw-r--r--   0     1001      127     4113 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/hash.rs
--rw-r--r--   0     1001      127      112 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/lib.rs
--rw-r--r--   0     1001      127     9419 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/stream.rs
--rw-r--r--   0     1001      127     3565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/sync.rs
--rw-r--r--   0     1001      127     1489 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/tar.rs
--rw-r--r--   0     1001      127     5685 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
--rw-r--r--   0     1001      127      112 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-extract/src/vendor/mod.rs
--rw-r--r--   0     1001      127      970 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-dispatch/Cargo.toml
--rw-r--r--   0     1001      127    10910 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-dispatch/src/lib.rs
--rw-r--r--   0     1001      127     1464 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/Cargo.toml
--rw-r--r--   0     1001      127    12444 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/compile.rs
--rw-r--r--   0     1001      127     9352 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/downloader.rs
--rw-r--r--   0     1001      127     4349 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/editable.rs
--rw-r--r--   0     1001      127     2833 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/installer.rs
--rw-r--r--   0     1001      127      533 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/pip_compileall.py
--rw-r--r--   0     1001      127    22428 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/plan.rs
--rw-r--r--   0     1001      127     7565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/satisfies.rs
--rw-r--r--   0     1001      127    22962 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/site_packages.rs
--rw-r--r--   0     1001      127      978 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-installer/src/uninstall.rs
--rw-r--r--   0     1001      127     1654 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/Cargo.toml
--rw-r--r--   0     1001      127     2206 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/confirm.rs
--rw-r--r--   0     1001      127      318 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/lib.rs
--rw-r--r--   0     1001      127     9898 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/lookahead.rs
--rw-r--r--   0     1001      127    31164 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/pyproject.rs
--rw-r--r--   0     1001      127     6930 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/source_tree.rs
--rw-r--r--   0     1001      127     7083 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/sources.rs
--rw-r--r--   0     1001      127    14943 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/specification.rs
--rw-r--r--   0     1001      127    12555 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/unnamed.rs
--rw-r--r--   0     1001      127     1677 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/upgrade.rs
--rw-r--r--   0     1001      127    25085 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-requirements/src/workspace.rs
--rw-r--r--   0     1001      127     1025 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/Cargo.toml
--rw-r--r--   0     1001      127      509 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/archive.rs
--rw-r--r--   0     1001      127      195 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/by_timestamp.rs
--rw-r--r--   0     1001      127     1768 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/cli.rs
--rw-r--r--   0     1001      127    35224 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/lib.rs
--rw-r--r--   0     1001      127     6138 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/removal.rs
--rw-r--r--   0     1001      127     1663 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/timestamp.rs
--rw-r--r--   0     1001      127     2538 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-cache/src/wheel.rs
--rw-r--r--   0     1001      127     1808 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/Cargo.toml
--rwxr-xr-x   0     1001      127     7922 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/fetch-version-metadata.py
--rw-r--r--   0     1001      127        0 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/__init__.py
--rw-r--r--   0     1001      127    21931 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/get_interpreter_info.py
--rw-r--r--   0     1001      127    10174 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.APACHE
--rw-r--r--   0     1001      127     1344 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.BSD
--rw-r--r--   0     1001      127      316 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/README.md
--rw-r--r--   0     1001      127      501 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/__init__.py
--rw-r--r--   0     1001      127     3282 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/_elffile.py
--rw-r--r--   0     1001      127     9588 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/_manylinux.py
--rw-r--r--   0     1001      127     2696 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python/packaging/_musllinux.py
--rw-r--r--   0     1001      127   182247 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/python-version-metadata.json
--rw-r--r--   0     1001      127    55660 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/discovery.rs
--rw-r--r--   0     1001      127     9015 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/environment.rs
--rw-r--r--   0     1001      127     1981 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/implementation.rs
--rw-r--r--   0     1001      127    28174 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/interpreter.rs
--rw-r--r--   0     1001      127    77357 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/lib.rs
--rw-r--r--   0     1001      127     8104 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/downloads.rs
--rw-r--r--   0     1001      127     5960 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/find.rs
--rw-r--r--   0     1001      127      253 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/mod.rs
--rw-r--r--   0     1001      127   224411 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc
--rw-r--r--   0     1001      127      691 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc.mustache
--rw-r--r--   0     1001      127     4389 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/platform.rs
--rw-r--r--   0     1001      127      430 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/pointer_size.rs
--rw-r--r--   0     1001      127     3234 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/py_launcher.rs
--rw-r--r--   0     1001      127     7736 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/python_version.rs
--rw-r--r--   0     1001      127      950 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/target.rs
--rw-r--r--   0     1001      127     5589 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/src/virtualenv.rs
--rw-r--r--   0     1001      127     2708 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-interpreter/template-version-metadata.py
--rw-r--r--   0     1001      127      411 2024-05-24 18:20:15.000000 uv-0.2.3/crates/once-map/Cargo.toml
--rw-r--r--   0     1001      127     3940 2024-05-24 18:20:15.000000 uv-0.2.3/crates/once-map/src/lib.rs
--rw-r--r--   0     1001      127      858 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/Cargo.toml
--rw-r--r--   0     1001      127     1014 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/authentication.rs
--rw-r--r--   0     1001      127    10763 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/build_options.rs
--rw-r--r--   0     1001      127     1054 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/concurrency.rs
--rw-r--r--   0     1001      127     9239 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/config_settings.rs
--rw-r--r--   0     1001      127     1698 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/constraints.rs
--rw-r--r--   0     1001      127      437 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/lib.rs
--rw-r--r--   0     1001      127     4059 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/name_specifiers.rs
--rw-r--r--   0     1001      127     1703 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/overrides.rs
--rw-r--r--   0     1001      127     2339 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/package_options.rs
--rw-r--r--   0     1001      127      782 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/preview.rs
--rw-r--r--   0     1001      127    11893 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-configuration/src/target_triple.rs
--rw-r--r--   0     1001      127     2046 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/Cargo.toml
--rw-r--r--   0     1001      127        1 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/bare.rs
--rw-r--r--   0     1001      127    17958 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/candidate_selector.rs
--rw-r--r--   0     1001      127      610 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/dependency_mode.rs
--rw-r--r--   0     1001      127     1140 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/dependency_provider.rs
--rw-r--r--   0     1001      127     1378 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/editables.rs
--rw-r--r--   0     1001      127    13502 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/error.rs
--rw-r--r--   0     1001      127     2743 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/exclude_newer.rs
--rw-r--r--   0     1001      127     1551 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/exclusions.rs
--rw-r--r--   0     1001      127     8107 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/flat_index.rs
--rw-r--r--   0     1001      127     1248 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/lib.rs
--rw-r--r--   0     1001      127    54353 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/lock.rs
--rw-r--r--   0     1001      127     8769 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/manifest.rs
--rw-r--r--   0     1001      127    12444 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/marker.rs
--rw-r--r--   0     1001      127     2149 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/options.rs
--rw-r--r--   0     1001      127     1122 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pins.rs
--rw-r--r--   0     1001      127     6069 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/preferences.rs
--rw-r--r--   0     1001      127     4046 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/prerelease_mode.rs
--rw-r--r--   0     1001      127    12211 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/dependencies.rs
--rw-r--r--   0     1001      127     1104 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/distribution.rs
--rw-r--r--   0     1001      127      541 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/mod.rs
--rw-r--r--   0     1001      127     7806 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/package.rs
--rw-r--r--   0     1001      127     5707 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/priority.rs
--rw-r--r--   0     1001      127    40255 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/report.rs
--rw-r--r--   0     1001      127     4890 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/pubgrub/specifier.rs
--rw-r--r--   0     1001      127     1163 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/python_requirement.rs
--rw-r--r--   0     1001      127     4963 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/redirect.rs
--rw-r--r--   0     1001      127    11323 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution/display.rs
--rw-r--r--   0     1001      127    24704 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution/graph.rs
--rw-r--r--   0     1001      127     4643 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution/mod.rs
--rw-r--r--   0     1001      127     1878 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolution_mode.rs
--rw-r--r--   0     1001      127     8210 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/batch_prefetch.rs
--rw-r--r--   0     1001      127     1172 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/index.rs
--rw-r--r--   0     1001      127    14028 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/locals.rs
--rw-r--r--   0     1001      127    66822 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/mod.rs
--rw-r--r--   0     1001      127     8756 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/provider.rs
--rw-r--r--   0     1001      127     1673 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/reporter.rs
--rw-r--r--   0     1001      127     8959 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/resolver/urls.rs
--rw-r--r--   0     1001      127     3325 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap
--rw-r--r--   0     1001      127      437 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_required_present.snap
--rw-r--r--   0     1001      127    23688 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/version_map.rs
--rw-r--r--   0     1001      127     1752 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/src/yanks.rs
--rw-r--r--   0     1001      127    22281 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-resolver/tests/resolver.rs
--rw-r--r--   0     1001      127      774 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/Cargo.toml
--rw-r--r--   0     1001      127      109 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/README.md
--rw-r--r--   0     1001      127     4375 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/_virtualenv.py
--rw-r--r--   0     1001      127       20 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/.gitattributes
--rw-r--r--   0     1001      127     3388 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate
--rw-r--r--   0     1001      127     2259 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.bat
--rw-r--r--   0     1001      127     2655 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.csh
--rw-r--r--   0     1001      127     4219 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.fish
--rw-r--r--   0     1001      127     3903 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.nu
--rw-r--r--   0     1001      127     2826 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate.ps1
--rw-r--r--   0     1001      127     2411 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/activate_this.py
--rw-r--r--   0     1001      127     1728 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/deactivate.bat
--rw-r--r--   0     1001      127     1215 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/activator/pydoc.bat
--rw-r--r--   0     1001      127    16565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/bare.rs
--rw-r--r--   0     1001      127     2090 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-virtualenv/src/lib.rs
--rw-r--r--   0     1001      127     1179 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-build/Cargo.toml
--rw-r--r--   0     1001      127       17 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-build/.gitignore
--rw-r--r--   0     1001      127    48369 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-build/src/lib.rs
--rw-r--r--   0     1001      127     1807 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/Cargo.toml
--rw-r--r--   0     1001      127      112 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/README.md
--rw-r--r--   0     1001      127     7109 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/base_client.rs
--rw-r--r--   0     1001      127    30512 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/cached_client.rs
--rw-r--r--   0     1001      127    10417 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/error.rs
--rw-r--r--   0     1001      127     9211 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/flat_index.rs
--rw-r--r--   0     1001      127    46032 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/html.rs
--rw-r--r--   0     1001      127    29250 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/httpcache/control.rs
--rw-r--r--   0     1001      127    60607 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/httpcache/mod.rs
--rw-r--r--   0     1001      127      648 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/lib.rs
--rw-r--r--   0     1001      127     5110 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/linehaul.rs
--rw-r--r--   0     1001      127     1228 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/middleware.rs
--rw-r--r--   0     1001      127    35668 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/registry_client.rs
--rw-r--r--   0     1001      127     4579 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/remote_metadata.rs
--rw-r--r--   0     1001      127    12019 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/src/rkyvutil.rs
--rw-r--r--   0     1001      127     1146 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/tests/remote_metadata.rs
--rw-r--r--   0     1001      127     8183 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-client/tests/user_agent_version.rs
--rw-r--r--   0     1001      127      608 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/Cargo.toml
--rw-r--r--   0     1001      127     1842 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/build_tag.rs
--rw-r--r--   0     1001      127     2352 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/lib.rs
--rw-r--r--   0     1001      127      532 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
--rw-r--r--   0     1001      127      564 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
--rw-r--r--   0     1001      127      423 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
--rw-r--r--   0     1001      127     7565 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/source_dist.rs
--rw-r--r--   0     1001      127    11807 2024-05-24 18:20:15.000000 uv-0.2.3/crates/distribution-filename/src/wheel.rs
--rw-r--r--   0     1001      127      472 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/Cargo.toml
--rw-r--r--   0     1001      127      161 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/src/lib.rs
--rw-r--r--   0     1001      127     3507 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/src/platform.rs
--rw-r--r--   0     1001      127    76059 2024-05-24 18:20:15.000000 uv-0.2.3/crates/platform-tags/src/tags.rs
--rw-r--r--   0     1001      127      284 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/src/extra_name.rs
--rw-r--r--   0     1001      127     5633 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/src/lib.rs
--rw-r--r--   0     1001      127     2847 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv-normalize/src/package_name.rs
--rw-r--r--   0     1001      127      910 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/Cargo.toml
--rw-r--r--   0     1001      127     1609 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/base_url.rs
--rw-r--r--   0     1001      127     4643 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/direct_url.rs
--rw-r--r--   0     1001      127    15762 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/lenient_requirement.rs
--rw-r--r--   0     1001      127      278 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/lib.rs
--rw-r--r--   0     1001      127    19633 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/metadata.rs
--rw-r--r--   0     1001      127    13865 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/parsed_url.rs
--rw-r--r--   0     1001      127      575 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/scheme.rs
--rw-r--r--   0     1001      127    12178 2024-05-24 18:20:15.000000 uv-0.2.3/crates/pypi-types/src/simple_json.rs
--rw-r--r--   0     1001      127     1504 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/Cargo.toml
--rw-r--r--   0     1001      127      515 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/Readme.md
--rw-r--r--   0     1001      127     4332 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/lib.rs
--rw-r--r--   0     1001      127    20181 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/linker.rs
--rw-r--r--   0     1001      127     7104 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/metadata.rs
--rw-r--r--   0     1001      127      474 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/record.rs
--rw-r--r--   0     1001      127     5550 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/script.rs
--rw-r--r--   0     1001      127    11211 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/uninstall.rs
--rw-r--r--   0     1001      127    34841 2024-05-24 18:20:15.000000 uv-0.2.3/crates/install-wheel-rs/src/wheel.rs
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 uv-0.2.3/crates/uv/Cargo.toml
--rw-r--r--   0     1001      127     3065 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/build.rs
--rw-r--r--   0     1001      127    79599 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/cli.rs
--rw-r--r--   0     1001      127     4158 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/cache_clean.rs
--rw-r--r--   0     1001      127      213 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/cache_dir.rs
--rw-r--r--   0     1001      127     1955 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/cache_prune.rs
--rw-r--r--   0     1001      127     4868 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/mod.rs
--rw-r--r--   0     1001      127     2362 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/check.rs
--rw-r--r--   0     1001      127    28326 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/compile.rs
--rw-r--r--   0     1001      127     2474 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/freeze.rs
--rw-r--r--   0     1001      127    15306 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/install.rs
--rw-r--r--   0     1001      127     6313 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/list.rs
--rw-r--r--   0     1001      127      209 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/mod.rs
--rw-r--r--   0     1001      127    25086 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/operations.rs
--rw-r--r--   0     1001      127     6615 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/show.rs
--rw-r--r--   0     1001      127    12804 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/sync.rs
--rw-r--r--   0     1001      127     7342 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/pip/uninstall.rs
--rw-r--r--   0     1001      127     5158 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/lock.rs
--rw-r--r--   0     1001      127     9046 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/mod.rs
--rw-r--r--   0     1001      127     5926 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/run.rs
--rw-r--r--   0     1001      127     4014 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/project/sync.rs
--rw-r--r--   0     1001      127    10251 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/reporters.rs
--rw-r--r--   0     1001      127     3965 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/self_update.rs
--rw-r--r--   0     1001      127       20 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/tool/mod.rs
--rw-r--r--   0     1001      127     4290 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/tool/run.rs
--rw-r--r--   0     1001      127    10247 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/venv.rs
--rw-r--r--   0     1001      127      570 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/commands/version.rs
--rw-r--r--   0     1001      127    11263 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/compat/mod.rs
--rw-r--r--   0     1001      127     7624 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/editables.rs
--rw-r--r--   0     1001      127     7604 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/logging.rs
--rw-r--r--   0     1001      127    24338 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/main.rs
--rw-r--r--   0     1001      127     2326 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/printer.rs
--rw-r--r--   0     1001      127    38621 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/settings.rs
--rw-r--r--   0     1001      127     2844 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/shell.rs
--rw-r--r--   0     1001      127     4816 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/src/version.rs
--rw-r--r--   0     1001      127     4437 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/cache_prune.rs
--rw-r--r--   0     1001      127    21781 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/common/mod.rs
--rw-r--r--   0     1001      127    27008 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/lock.rs
--rw-r--r--   0     1001      127     6060 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_check.rs
--rw-r--r--   0     1001      127   307159 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_compile.rs
--rw-r--r--   0     1001      127    19016 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_compile_scenarios.rs
--rw-r--r--   0     1001      127     8341 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_freeze.rs
--rw-r--r--   0     1001      127   151842 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_install.rs
--rw-r--r--   0     1001      127   159299 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_install_scenarios.rs
--rw-r--r--   0     1001      127    18430 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_list.rs
--rw-r--r--   0     1001      127    13190 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_show.rs
--rw-r--r--   0     1001      127   161999 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_sync.rs
--rw-r--r--   0     1001      127    14235 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/pip_uninstall.rs
--rw-r--r--   0     1001      127     1254 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/self_update.rs
--rw-r--r--   0     1001      127    18144 2024-05-24 18:20:15.000000 uv-0.2.3/crates/uv/tests/venv.rs
--rw-r--r--   0     1001      127   133939 2024-05-24 18:20:15.000000 uv-0.2.3/Cargo.lock
--rw-r--r--   0        0        0     8834 1970-01-01 00:00:00.000000 uv-0.2.3/Cargo.toml
--rw-r--r--   0     1001      127     2366 2024-05-24 18:20:15.000000 uv-0.2.3/pyproject.toml
--rw-r--r--   0     1001      127     1055 2024-05-24 18:20:15.000000 uv-0.2.3/python/uv/__main__.py
--rw-r--r--   0     1001      127      806 2024-05-24 18:20:15.000000 uv-0.2.3/python/uv/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-24 18:20:15.000000 uv-0.2.3/python/uv/py.typed
--rw-r--r--   0     1001      127    31568 2024-05-24 18:20:16.000000 uv-0.2.3/README.md
--rw-r--r--   0     1001      127       29 2024-05-24 18:20:15.000000 uv-0.2.3/rust-toolchain.toml
--rw-r--r--   0     1001      127    11356 2024-05-24 18:20:15.000000 uv-0.2.3/LICENSE-APACHE
--rw-r--r--   0     1001      127     1077 2024-05-24 18:20:15.000000 uv-0.2.3/LICENSE-MIT
--rw-r--r--   0        0        0    32935 1970-01-01 00:00:00.000000 uv-0.2.3/PKG-INFO
+-rw-r--r--   0     1001      127     1004 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/License-BSD
+-rw-r--r--   0     1001      127     2947 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/Readme.md
+-rw-r--r--   0     1001      127     2105 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/python/Readme.md
+-rw-r--r--   0     1001      127     2922 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/src/lib.rs
+-rw-r--r--   0     1001      127   131052 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/src/version.rs
+-rw-r--r--   0     1001      127    56892 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep440-rs/src/version_specifier.rs
+-rw-r--r--   0     1001      127      456 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-warnings/Cargo.toml
+-rw-r--r--   0     1001      127     1701 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-warnings/src/lib.rs
+-rw-r--r--   0     1001      127      608 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/Cargo.toml
+-rw-r--r--   0     1001      127     1842 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/build_tag.rs
+-rw-r--r--   0     1001      127     2352 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/lib.rs
+-rw-r--r--   0     1001      127      532 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
+-rw-r--r--   0     1001      127      564 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
+-rw-r--r--   0     1001      127      423 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
+-rw-r--r--   0     1001      127     7565 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/source_dist.rs
+-rw-r--r--   0     1001      127    11807 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-filename/src/wheel.rs
+-rw-r--r--   0     1001      127     1224 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/Cargo.toml
+-rw-r--r--   0     1001      127    87285 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/lib.rs
+-rw-r--r--   0     1001      127     2038 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/requirement.rs
+-rw-r--r--   0     1001      127     6200 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
+-rw-r--r--   0     1001      127     2683 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     2273 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      284 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
+-rw-r--r--   0     1001      127     4140 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1816 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
+-rw-r--r--   0     1001      127      828 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
+-rw-r--r--   0     1001      127    11863 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     2257 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
+-rw-r--r--   0     1001      127     3818 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
+-rw-r--r--   0     1001      127     6200 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
+-rw-r--r--   0     1001      127     2683 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     2273 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      284 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
+-rw-r--r--   0     1001      127     4140 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1816 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
+-rw-r--r--   0     1001      127      828 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
+-rw-r--r--   0     1001      127    11863 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     2257 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
+-rw-r--r--   0     1001      127     6684 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap
+-rw-r--r--   0     1001      127     8155 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap
+-rw-r--r--   0     1001      127     3818 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
+-rw-r--r--   0     1001      127     6744 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap
+-rw-r--r--   0     1001      127     8161 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap
+-rw-r--r--   0     1001      127      113 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/bare-url.txt
+-rw-r--r--   0     1001      127       90 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/basic.txt
+-rw-r--r--   0     1001      127       45 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
+-rw-r--r--   0     1001      127       27 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
+-rw-r--r--   0     1001      127      491 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/editable.txt
+-rw-r--r--   0     1001      127        0 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/empty.txt
+-rw-r--r--   0     1001      127      101 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
+-rw-r--r--   0     1001      127       43 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/include-a.txt
+-rw-r--r--   0     1001      127        5 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/include-b.txt
+-rw-r--r--   0     1001      127     1183 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
+-rw-r--r--   0     1001      127       66 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/small.txt
+-rw-r--r--   0     1001      127      183 2024-05-26 17:12:05.000000 uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
+-rw-r--r--   0     1001      127     1807 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/Cargo.toml
+-rw-r--r--   0     1001      127      112 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/README.md
+-rw-r--r--   0     1001      127     7109 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/base_client.rs
+-rw-r--r--   0     1001      127    30512 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/cached_client.rs
+-rw-r--r--   0     1001      127    10417 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/error.rs
+-rw-r--r--   0     1001      127     9211 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/flat_index.rs
+-rw-r--r--   0     1001      127    46032 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/html.rs
+-rw-r--r--   0     1001      127    29250 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/httpcache/control.rs
+-rw-r--r--   0     1001      127    60607 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/httpcache/mod.rs
+-rw-r--r--   0     1001      127      648 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/lib.rs
+-rw-r--r--   0     1001      127     5110 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/linehaul.rs
+-rw-r--r--   0     1001      127     1228 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/middleware.rs
+-rw-r--r--   0     1001      127    35668 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/registry_client.rs
+-rw-r--r--   0     1001      127     4579 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/remote_metadata.rs
+-rw-r--r--   0     1001      127    12019 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/src/rkyvutil.rs
+-rw-r--r--   0     1001      127     1146 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/tests/remote_metadata.rs
+-rw-r--r--   0     1001      127     8183 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-client/tests/user_agent_version.rs
+-rw-r--r--   0     1001      127     2085 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/License-BSD
+-rw-r--r--   0     1001      127     3039 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/Readme.md
+-rw-r--r--   0     1001      127     4301 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/src/cursor.rs
+-rw-r--r--   0     1001      127    62060 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/src/lib.rs
+-rw-r--r--   0     1001      127    94881 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/src/marker.rs
+-rw-r--r--   0     1001      127      743 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/src/origin.rs
+-rw-r--r--   0     1001      127    13353 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/src/unnamed.rs
+-rw-r--r--   0     1001      127    18647 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pep508-rs/src/verbatim_url.rs
+-rw-r--r--   0     1001      127      472 2024-05-26 17:12:05.000000 uv-0.2.4/crates/platform-tags/Cargo.toml
+-rw-r--r--   0     1001      127      161 2024-05-26 17:12:05.000000 uv-0.2.4/crates/platform-tags/src/lib.rs
+-rw-r--r--   0     1001      127     3507 2024-05-26 17:12:05.000000 uv-0.2.4/crates/platform-tags/src/platform.rs
+-rw-r--r--   0     1001      127    76059 2024-05-26 17:12:05.000000 uv-0.2.4/crates/platform-tags/src/tags.rs
+-rw-r--r--   0     1001      127      752 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/Cargo.toml
+-rw-r--r--   0     1001      127     9542 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/src/cache.rs
+-rw-r--r--   0     1001      127    11219 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/src/credentials.rs
+-rw-r--r--   0     1001      127     9340 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/src/keyring.rs
+-rw-r--r--   0     1001      127      992 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/src/lib.rs
+-rw-r--r--   0     1001      127    45581 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/src/middleware.rs
+-rw-r--r--   0     1001      127     4661 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-auth/src/realm.rs
+-rw-r--r--   0     1001      127     1504 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/Cargo.toml
+-rw-r--r--   0     1001      127      515 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/Readme.md
+-rw-r--r--   0     1001      127     4332 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/lib.rs
+-rw-r--r--   0     1001      127    20181 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/linker.rs
+-rw-r--r--   0     1001      127     7104 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/metadata.rs
+-rw-r--r--   0     1001      127      474 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/record.rs
+-rw-r--r--   0     1001      127     5550 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/script.rs
+-rw-r--r--   0     1001      127    11211 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/uninstall.rs
+-rw-r--r--   0     1001      127    34841 2024-05-26 17:12:05.000000 uv-0.2.4/crates/install-wheel-rs/src/wheel.rs
+-rw-r--r--   0     1001      127      411 2024-05-26 17:12:05.000000 uv-0.2.4/crates/once-map/Cargo.toml
+-rw-r--r--   0     1001      127     3940 2024-05-26 17:12:05.000000 uv-0.2.4/crates/once-map/src/lib.rs
+-rw-r--r--   0     1001      127     1179 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-build/Cargo.toml
+-rw-r--r--   0     1001      127       17 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-build/.gitignore
+-rw-r--r--   0     1001      127    48369 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-build/src/lib.rs
+-rw-r--r--   0     1001      127     1121 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/Cargo.toml
+-rw-r--r--   0     1001      127     2527 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/annotation.rs
+-rw-r--r--   0     1001      127     1048 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/any.rs
+-rw-r--r--   0     1001      127     4667 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/buildable.rs
+-rw-r--r--   0     1001      127     6720 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/cached.rs
+-rw-r--r--   0     1001      127      280 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/diagnostic.rs
+-rw-r--r--   0     1001      127     2474 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/editable.rs
+-rw-r--r--   0     1001      127      985 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/error.rs
+-rw-r--r--   0     1001      127     7205 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/file.rs
+-rw-r--r--   0     1001      127     2831 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/hash.rs
+-rw-r--r--   0     1001      127     3845 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/id.rs
+-rw-r--r--   0     1001      127    14472 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/index_url.rs
+-rw-r--r--   0     1001      127    12906 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/installed.rs
+-rw-r--r--   0     1001      127    35900 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/lib.rs
+-rw-r--r--   0     1001      127    20983 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/prioritized_distribution.rs
+-rw-r--r--   0     1001      127     8297 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/requirement.rs
+-rw-r--r--   0     1001      127     1228 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/requirements.rs
+-rw-r--r--   0     1001      127     8062 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/resolution.rs
+-rw-r--r--   0     1001      127     7176 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/resolved.rs
+-rw-r--r--   0     1001      127     3015 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/specified_requirement.rs
+-rw-r--r--   0     1001      127     8193 2024-05-26 17:12:05.000000 uv-0.2.4/crates/distribution-types/src/traits.rs
+-rw-r--r--   0     1001      127      774 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/Cargo.toml
+-rw-r--r--   0     1001      127      109 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/README.md
+-rw-r--r--   0     1001      127     4375 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/_virtualenv.py
+-rw-r--r--   0     1001      127       20 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/.gitattributes
+-rw-r--r--   0     1001      127     3388 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate
+-rw-r--r--   0     1001      127     2259 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate.bat
+-rw-r--r--   0     1001      127     2655 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate.csh
+-rw-r--r--   0     1001      127     4219 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate.fish
+-rw-r--r--   0     1001      127     3903 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate.nu
+-rw-r--r--   0     1001      127     2826 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate.ps1
+-rw-r--r--   0     1001      127     2411 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/activate_this.py
+-rw-r--r--   0     1001      127     1728 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/deactivate.bat
+-rw-r--r--   0     1001      127     1215 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/activator/pydoc.bat
+-rw-r--r--   0     1001      127    16565 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/bare.rs
+-rw-r--r--   0     1001      127     2090 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-virtualenv/src/lib.rs
+-rw-r--r--   0     1001      127      910 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/Cargo.toml
+-rw-r--r--   0     1001      127     1609 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/base_url.rs
+-rw-r--r--   0     1001      127     4643 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/direct_url.rs
+-rw-r--r--   0     1001      127    15762 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/lenient_requirement.rs
+-rw-r--r--   0     1001      127      278 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/lib.rs
+-rw-r--r--   0     1001      127    19633 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/metadata.rs
+-rw-r--r--   0     1001      127    13865 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/parsed_url.rs
+-rw-r--r--   0     1001      127      575 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/scheme.rs
+-rw-r--r--   0     1001      127    12178 2024-05-26 17:12:05.000000 uv-0.2.4/crates/pypi-types/src/simple_json.rs
+-rw-r--r--   0     1001      127     1002 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-workspace/Cargo.toml
+-rw-r--r--   0     1001      127     7241 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-workspace/src/combine.rs
+-rw-r--r--   0     1001      127      127 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-workspace/src/lib.rs
+-rw-r--r--   0     1001      127     3296 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-workspace/src/settings.rs
+-rw-r--r--   0     1001      127     5560 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-workspace/src/workspace.rs
+-rw-r--r--   0     1001      127     1654 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/Cargo.toml
+-rw-r--r--   0     1001      127     2206 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/confirm.rs
+-rw-r--r--   0     1001      127      318 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/lib.rs
+-rw-r--r--   0     1001      127     9898 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/lookahead.rs
+-rw-r--r--   0     1001      127    31164 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/pyproject.rs
+-rw-r--r--   0     1001      127     6930 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/source_tree.rs
+-rw-r--r--   0     1001      127     7083 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/sources.rs
+-rw-r--r--   0     1001      127    14943 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/specification.rs
+-rw-r--r--   0     1001      127    12555 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/unnamed.rs
+-rw-r--r--   0     1001      127     1677 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/upgrade.rs
+-rw-r--r--   0     1001      127    25085 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-requirements/src/workspace.rs
+-rw-r--r--   0     1001      127      284 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-normalize/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-normalize/src/extra_name.rs
+-rw-r--r--   0     1001      127     5633 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-normalize/src/lib.rs
+-rw-r--r--   0     1001      127     2847 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-normalize/src/package_name.rs
+-rw-r--r--   0     1001      127      790 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/Cargo.toml
+-rw-r--r--   0     1001      127      423 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/src/builds.rs
+-rw-r--r--   0     1001      127      239 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/src/downloads.rs
+-rw-r--r--   0     1001      127     6237 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/src/hash.rs
+-rw-r--r--   0     1001      127      219 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/src/lib.rs
+-rw-r--r--   0     1001      127     1478 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/src/requirements.rs
+-rw-r--r--   0     1001      127     6944 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-types/src/traits.rs
+-rw-r--r--   0     1001      127     1808 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/Cargo.toml
+-rwxr-xr-x   0     1001      127     7922 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/fetch-version-metadata.py
+-rw-r--r--   0     1001      127        0 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/__init__.py
+-rw-r--r--   0     1001      127    21931 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/get_interpreter_info.py
+-rw-r--r--   0     1001      127    10174 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/LICENSE.APACHE
+-rw-r--r--   0     1001      127     1344 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/LICENSE.BSD
+-rw-r--r--   0     1001      127      316 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/README.md
+-rw-r--r--   0     1001      127      501 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/__init__.py
+-rw-r--r--   0     1001      127     3282 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/_elffile.py
+-rw-r--r--   0     1001      127     9588 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/_manylinux.py
+-rw-r--r--   0     1001      127     2696 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python/packaging/_musllinux.py
+-rw-r--r--   0     1001      127   182247 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/python-version-metadata.json
+-rw-r--r--   0     1001      127    55660 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/discovery.rs
+-rw-r--r--   0     1001      127     9015 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/environment.rs
+-rw-r--r--   0     1001      127     1981 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/implementation.rs
+-rw-r--r--   0     1001      127    28174 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/interpreter.rs
+-rw-r--r--   0     1001      127    77357 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/lib.rs
+-rw-r--r--   0     1001      127     8103 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/managed/downloads.rs
+-rw-r--r--   0     1001      127     5959 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/managed/find.rs
+-rw-r--r--   0     1001      127      253 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/managed/mod.rs
+-rw-r--r--   0     1001      127   224411 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/managed/python_versions.inc
+-rw-r--r--   0     1001      127      691 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/managed/python_versions.inc.mustache
+-rw-r--r--   0     1001      127     4433 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/platform.rs
+-rw-r--r--   0     1001      127      430 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/pointer_size.rs
+-rw-r--r--   0     1001      127     3234 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/py_launcher.rs
+-rw-r--r--   0     1001      127     7736 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/python_version.rs
+-rw-r--r--   0     1001      127      950 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/target.rs
+-rw-r--r--   0     1001      127     5589 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/src/virtualenv.rs
+-rw-r--r--   0     1001      127     2708 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-interpreter/template-version-metadata.py
+-rw-r--r--   0     1001      127      322 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-version/Cargo.toml
+-rw-r--r--   0     1001      127      355 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-version/src/lib.rs
+-rw-r--r--   0     1001      127      918 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/Cargo.toml
+-rw-r--r--   0     1001      127    63247 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/git.rs
+-rw-r--r--   0     1001      127    37494 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/known_hosts.rs
+-rw-r--r--   0     1001      127     3843 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/lib.rs
+-rw-r--r--   0     1001      127      940 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/sha.rs
+-rw-r--r--   0     1001      127     5058 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/source.rs
+-rw-r--r--   0     1001      127     1362 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/util/errors.rs
+-rw-r--r--   0     1001      127      733 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/util/mod.rs
+-rw-r--r--   0     1001      127     7295 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-git/src/util/retry.rs
+-rw-r--r--   0     1001      127      911 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-fs/Cargo.toml
+-rw-r--r--   0     1001      127     1397 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-fs/src/cachedir.rs
+-rw-r--r--   0     1001      127    11137 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-fs/src/lib.rs
+-rw-r--r--   0     1001      127    12687 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-fs/src/path.rs
+-rw-r--r--   0     1001      127      858 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/Cargo.toml
+-rw-r--r--   0     1001      127     1014 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/authentication.rs
+-rw-r--r--   0     1001      127    10763 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/build_options.rs
+-rw-r--r--   0     1001      127     1054 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/concurrency.rs
+-rw-r--r--   0     1001      127     9239 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/config_settings.rs
+-rw-r--r--   0     1001      127     1698 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/constraints.rs
+-rw-r--r--   0     1001      127      437 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/lib.rs
+-rw-r--r--   0     1001      127     4059 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/name_specifiers.rs
+-rw-r--r--   0     1001      127     1703 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/overrides.rs
+-rw-r--r--   0     1001      127     2339 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/package_options.rs
+-rw-r--r--   0     1001      127      782 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/preview.rs
+-rw-r--r--   0     1001      127    11893 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-configuration/src/target_triple.rs
+-rw-r--r--   0     1001      127      507 2024-05-26 17:12:05.000000 uv-0.2.4/crates/cache-key/Cargo.toml
+-rw-r--r--   0     1001      127     8335 2024-05-26 17:12:05.000000 uv-0.2.4/crates/cache-key/src/cache_key.rs
+-rw-r--r--   0     1001      127    12317 2024-05-26 17:12:05.000000 uv-0.2.4/crates/cache-key/src/canonical_url.rs
+-rw-r--r--   0     1001      127      620 2024-05-26 17:12:05.000000 uv-0.2.4/crates/cache-key/src/digest.rs
+-rw-r--r--   0     1001      127      191 2024-05-26 17:12:05.000000 uv-0.2.4/crates/cache-key/src/lib.rs
+-rw-r--r--   0     1001      127     1986 2024-05-26 17:12:05.000000 uv-0.2.4/crates/cache-key/src/stable_hash.rs
+-rw-r--r--   0     1001      127     1025 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/Cargo.toml
+-rw-r--r--   0     1001      127      509 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/archive.rs
+-rw-r--r--   0     1001      127      195 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/by_timestamp.rs
+-rw-r--r--   0     1001      127     1768 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/cli.rs
+-rw-r--r--   0     1001      127    35224 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/lib.rs
+-rw-r--r--   0     1001      127     6138 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/removal.rs
+-rw-r--r--   0     1001      127     1663 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/timestamp.rs
+-rw-r--r--   0     1001      127     2538 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-cache/src/wheel.rs
+-rw-r--r--   0     1001      127     1464 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/Cargo.toml
+-rw-r--r--   0     1001      127    12444 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/compile.rs
+-rw-r--r--   0     1001      127     9352 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/downloader.rs
+-rw-r--r--   0     1001      127     4349 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/editable.rs
+-rw-r--r--   0     1001      127     2833 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/installer.rs
+-rw-r--r--   0     1001      127      533 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/pip_compileall.py
+-rw-r--r--   0     1001      127    22428 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/plan.rs
+-rw-r--r--   0     1001      127     7565 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/satisfies.rs
+-rw-r--r--   0     1001      127    22962 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/site_packages.rs
+-rw-r--r--   0     1001      127      978 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-installer/src/uninstall.rs
+-rw-r--r--   0     1001      127      897 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/Cargo.toml
+-rw-r--r--   0     1001      127     1078 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/error.rs
+-rw-r--r--   0     1001      127     4113 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/hash.rs
+-rw-r--r--   0     1001      127      112 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/lib.rs
+-rw-r--r--   0     1001      127     9419 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/stream.rs
+-rw-r--r--   0     1001      127     3565 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/sync.rs
+-rw-r--r--   0     1001      127     1489 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/tar.rs
+-rw-r--r--   0     1001      127     5685 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
+-rw-r--r--   0     1001      127      112 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-extract/src/vendor/mod.rs
+-rw-r--r--   0     1001      127     2046 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/Cargo.toml
+-rw-r--r--   0     1001      127        1 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/bare.rs
+-rw-r--r--   0     1001      127    17958 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/candidate_selector.rs
+-rw-r--r--   0     1001      127      610 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/dependency_mode.rs
+-rw-r--r--   0     1001      127     1140 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/dependency_provider.rs
+-rw-r--r--   0     1001      127     1378 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/editables.rs
+-rw-r--r--   0     1001      127    13502 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/error.rs
+-rw-r--r--   0     1001      127     2743 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/exclude_newer.rs
+-rw-r--r--   0     1001      127     1551 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/exclusions.rs
+-rw-r--r--   0     1001      127     8107 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/flat_index.rs
+-rw-r--r--   0     1001      127     1248 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/lib.rs
+-rw-r--r--   0     1001      127    54353 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/lock.rs
+-rw-r--r--   0     1001      127     8769 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/manifest.rs
+-rw-r--r--   0     1001      127    12444 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/marker.rs
+-rw-r--r--   0     1001      127     2149 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/options.rs
+-rw-r--r--   0     1001      127     1122 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pins.rs
+-rw-r--r--   0     1001      127     5920 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/preferences.rs
+-rw-r--r--   0     1001      127     4046 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/prerelease_mode.rs
+-rw-r--r--   0     1001      127    12211 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/dependencies.rs
+-rw-r--r--   0     1001      127     1104 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/distribution.rs
+-rw-r--r--   0     1001      127      541 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/mod.rs
+-rw-r--r--   0     1001      127     7806 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/package.rs
+-rw-r--r--   0     1001      127     5707 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/priority.rs
+-rw-r--r--   0     1001      127    40255 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/report.rs
+-rw-r--r--   0     1001      127     4890 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/pubgrub/specifier.rs
+-rw-r--r--   0     1001      127     1163 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/python_requirement.rs
+-rw-r--r--   0     1001      127     4963 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/redirect.rs
+-rw-r--r--   0     1001      127    11323 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolution/display.rs
+-rw-r--r--   0     1001      127    24704 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolution/graph.rs
+-rw-r--r--   0     1001      127     4643 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolution/mod.rs
+-rw-r--r--   0     1001      127     1878 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolution_mode.rs
+-rw-r--r--   0     1001      127     8210 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/batch_prefetch.rs
+-rw-r--r--   0     1001      127     1172 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/index.rs
+-rw-r--r--   0     1001      127    14028 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/locals.rs
+-rw-r--r--   0     1001      127    66822 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/mod.rs
+-rw-r--r--   0     1001      127     8756 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/provider.rs
+-rw-r--r--   0     1001      127     1673 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/reporter.rs
+-rw-r--r--   0     1001      127     8959 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/resolver/urls.rs
+-rw-r--r--   0     1001      127     3325 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap
+-rw-r--r--   0     1001      127      437 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_required_present.snap
+-rw-r--r--   0     1001      127    23688 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/version_map.rs
+-rw-r--r--   0     1001      127     2004 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/src/yanks.rs
+-rw-r--r--   0     1001      127    22324 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-resolver/tests/resolver.rs
+-rw-r--r--   0     1001      127      970 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-dispatch/Cargo.toml
+-rw-r--r--   0     1001      127    10910 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-dispatch/src/lib.rs
+-rw-r--r--   0     1001      127     1528 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/Cargo.toml
+-rw-r--r--   0     1001      127      684 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/archive.rs
+-rw-r--r--   0     1001      127    34434 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/distribution_database.rs
+-rw-r--r--   0     1001      127     2185 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/download.rs
+-rw-r--r--   0     1001      127     6943 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/error.rs
+-rw-r--r--   0     1001      127    10363 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/git.rs
+-rw-r--r--   0     1001      127     7145 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/index/built_wheel_index.rs
+-rw-r--r--   0     1001      127     3435 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/index/cached_wheel.rs
+-rw-r--r--   0     1001      127      162 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/index/mod.rs
+-rw-r--r--   0     1001      127     8729 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/index/registry_wheel_index.rs
+-rw-r--r--   0     1001      127      965 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/lib.rs
+-rw-r--r--   0     1001      127      600 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/locks.rs
+-rw-r--r--   0     1001      127     1225 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/reporter.rs
+-rw-r--r--   0     1001      127     2029 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/source/built_wheel_metadata.rs
+-rw-r--r--   0     1001      127    60305 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/source/mod.rs
+-rw-r--r--   0     1001      127     1998 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv-distribution/src/source/revision.rs
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 uv-0.2.4/crates/uv/Cargo.toml
+-rw-r--r--   0     1001      127     3065 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/build.rs
+-rw-r--r--   0     1001      127    78417 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/cli.rs
+-rw-r--r--   0     1001      127     4158 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/cache_clean.rs
+-rw-r--r--   0     1001      127      213 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/cache_dir.rs
+-rw-r--r--   0     1001      127     1955 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/cache_prune.rs
+-rw-r--r--   0     1001      127     4868 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/mod.rs
+-rw-r--r--   0     1001      127     2362 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/check.rs
+-rw-r--r--   0     1001      127    28326 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/compile.rs
+-rw-r--r--   0     1001      127     2474 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/freeze.rs
+-rw-r--r--   0     1001      127    15306 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/install.rs
+-rw-r--r--   0     1001      127     6313 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/list.rs
+-rw-r--r--   0     1001      127      209 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/mod.rs
+-rw-r--r--   0     1001      127    23750 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/operations.rs
+-rw-r--r--   0     1001      127     6615 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/show.rs
+-rw-r--r--   0     1001      127    12804 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/sync.rs
+-rw-r--r--   0     1001      127     7342 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/pip/uninstall.rs
+-rw-r--r--   0     1001      127     5158 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/project/lock.rs
+-rw-r--r--   0     1001      127     9046 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/project/mod.rs
+-rw-r--r--   0     1001      127     5926 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/project/run.rs
+-rw-r--r--   0     1001      127     4014 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/project/sync.rs
+-rw-r--r--   0     1001      127    10251 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/reporters.rs
+-rw-r--r--   0     1001      127     3965 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/self_update.rs
+-rw-r--r--   0     1001      127       20 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/tool/mod.rs
+-rw-r--r--   0     1001      127     4290 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/tool/run.rs
+-rw-r--r--   0     1001      127    10247 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/venv.rs
+-rw-r--r--   0     1001      127      570 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/commands/version.rs
+-rw-r--r--   0     1001      127    11263 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/compat/mod.rs
+-rw-r--r--   0     1001      127     7624 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/editables.rs
+-rw-r--r--   0     1001      127     7604 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/logging.rs
+-rw-r--r--   0     1001      127    24338 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/main.rs
+-rw-r--r--   0     1001      127     2326 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/printer.rs
+-rw-r--r--   0     1001      127    38621 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/settings.rs
+-rw-r--r--   0     1001      127     2844 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/shell.rs
+-rw-r--r--   0     1001      127     4816 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/src/version.rs
+-rw-r--r--   0     1001      127     4437 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/cache_prune.rs
+-rw-r--r--   0     1001      127    21781 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/common/mod.rs
+-rw-r--r--   0     1001      127    27008 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/lock.rs
+-rw-r--r--   0     1001      127     6060 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_check.rs
+-rw-r--r--   0     1001      127   307159 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_compile.rs
+-rw-r--r--   0     1001      127    19016 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_compile_scenarios.rs
+-rw-r--r--   0     1001      127     8341 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_freeze.rs
+-rw-r--r--   0     1001      127   151842 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_install.rs
+-rw-r--r--   0     1001      127   159299 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_install_scenarios.rs
+-rw-r--r--   0     1001      127    18430 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_list.rs
+-rw-r--r--   0     1001      127    13190 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_show.rs
+-rw-r--r--   0     1001      127   161999 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_sync.rs
+-rw-r--r--   0     1001      127    14235 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/pip_uninstall.rs
+-rw-r--r--   0     1001      127     1254 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/self_update.rs
+-rw-r--r--   0     1001      127    18144 2024-05-26 17:12:05.000000 uv-0.2.4/crates/uv/tests/venv.rs
+-rw-r--r--   0     1001      127   133925 2024-05-26 17:12:05.000000 uv-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0     8834 1970-01-01 00:00:00.000000 uv-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      127     2366 2024-05-26 17:12:05.000000 uv-0.2.4/pyproject.toml
+-rw-r--r--   0     1001      127     1055 2024-05-26 17:12:05.000000 uv-0.2.4/python/uv/__main__.py
+-rw-r--r--   0     1001      127      806 2024-05-26 17:12:05.000000 uv-0.2.4/python/uv/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-26 17:12:05.000000 uv-0.2.4/python/uv/py.typed
+-rw-r--r--   0     1001      127    31568 2024-05-26 17:12:05.000000 uv-0.2.4/README.md
+-rw-r--r--   0     1001      127       29 2024-05-26 17:12:05.000000 uv-0.2.4/rust-toolchain.toml
+-rw-r--r--   0     1001      127    11356 2024-05-26 17:12:05.000000 uv-0.2.4/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1077 2024-05-26 17:12:05.000000 uv-0.2.4/LICENSE-MIT
+-rw-r--r--   0        0        0    32935 1970-01-01 00:00:00.000000 uv-0.2.4/PKG-INFO
```

### Comparing `uv-0.2.3/crates/uv-auth/Cargo.toml` & `uv-0.2.4/crates/uv-auth/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-auth/src/cache.rs` & `uv-0.2.4/crates/uv-auth/src/cache.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-auth/src/credentials.rs` & `uv-0.2.4/crates/uv-auth/src/credentials.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-auth/src/keyring.rs` & `uv-0.2.4/crates/uv-auth/src/keyring.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-auth/src/lib.rs` & `uv-0.2.4/crates/uv-auth/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-auth/src/middleware.rs` & `uv-0.2.4/crates/uv-auth/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-auth/src/realm.rs` & `uv-0.2.4/crates/uv-auth/src/realm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-types/Cargo.toml` & `uv-0.2.4/crates/uv-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-types/src/hash.rs` & `uv-0.2.4/crates/uv-types/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-types/src/requirements.rs` & `uv-0.2.4/crates/uv-types/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-types/src/traits.rs` & `uv-0.2.4/crates/uv-types/src/traits.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/Cargo.toml` & `uv-0.2.4/crates/distribution-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/annotation.rs` & `uv-0.2.4/crates/distribution-types/src/annotation.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/any.rs` & `uv-0.2.4/crates/distribution-types/src/any.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/buildable.rs` & `uv-0.2.4/crates/distribution-types/src/buildable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/cached.rs` & `uv-0.2.4/crates/distribution-types/src/cached.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/editable.rs` & `uv-0.2.4/crates/distribution-types/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/error.rs` & `uv-0.2.4/crates/distribution-types/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/file.rs` & `uv-0.2.4/crates/distribution-types/src/file.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/hash.rs` & `uv-0.2.4/crates/distribution-types/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/id.rs` & `uv-0.2.4/crates/distribution-types/src/id.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/index_url.rs` & `uv-0.2.4/crates/distribution-types/src/index_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/installed.rs` & `uv-0.2.4/crates/distribution-types/src/installed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/lib.rs` & `uv-0.2.4/crates/distribution-types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/prioritized_distribution.rs` & `uv-0.2.4/crates/distribution-types/src/prioritized_distribution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/requirement.rs` & `uv-0.2.4/crates/distribution-types/src/requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/requirements.rs` & `uv-0.2.4/crates/distribution-types/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/resolution.rs` & `uv-0.2.4/crates/distribution-types/src/resolution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/resolved.rs` & `uv-0.2.4/crates/distribution-types/src/resolved.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/specified_requirement.rs` & `uv-0.2.4/crates/distribution-types/src/specified_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-types/src/traits.rs` & `uv-0.2.4/crates/distribution-types/src/traits.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/cache-key/src/cache_key.rs` & `uv-0.2.4/crates/cache-key/src/cache_key.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/cache-key/src/canonical_url.rs` & `uv-0.2.4/crates/cache-key/src/canonical_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/cache-key/src/digest.rs` & `uv-0.2.4/crates/cache-key/src/digest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/cache-key/src/stable_hash.rs` & `uv-0.2.4/crates/cache-key/src/stable_hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/Cargo.toml` & `uv-0.2.4/crates/pep440-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/License-Apache` & `uv-0.2.4/crates/pep440-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/License-BSD` & `uv-0.2.4/crates/pep440-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/Readme.md` & `uv-0.2.4/crates/pep440-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/python/Readme.md` & `uv-0.2.4/crates/pep440-rs/python/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/src/lib.rs` & `uv-0.2.4/crates/pep440-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/src/version.rs` & `uv-0.2.4/crates/pep440-rs/src/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep440-rs/src/version_specifier.rs` & `uv-0.2.4/crates/pep440-rs/src/version_specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/Cargo.toml` & `uv-0.2.4/crates/uv-git/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/git.rs` & `uv-0.2.4/crates/uv-git/src/git.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/known_hosts.rs` & `uv-0.2.4/crates/uv-git/src/known_hosts.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/lib.rs` & `uv-0.2.4/crates/uv-git/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/sha.rs` & `uv-0.2.4/crates/uv-git/src/sha.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/source.rs` & `uv-0.2.4/crates/uv-git/src/source.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/util/errors.rs` & `uv-0.2.4/crates/uv-git/src/util/errors.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/util/mod.rs` & `uv-0.2.4/crates/uv-git/src/util/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-git/src/util/retry.rs` & `uv-0.2.4/crates/uv-git/src/util/retry.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-warnings/src/lib.rs` & `uv-0.2.4/crates/uv-warnings/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-fs/Cargo.toml` & `uv-0.2.4/crates/uv-fs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-fs/src/cachedir.rs` & `uv-0.2.4/crates/uv-fs/src/cachedir.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-fs/src/lib.rs` & `uv-0.2.4/crates/uv-fs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-fs/src/path.rs` & `uv-0.2.4/crates/uv-fs/src/path.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-workspace/Cargo.toml` & `uv-0.2.4/crates/uv-workspace/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-workspace/src/combine.rs` & `uv-0.2.4/crates/uv-workspace/src/combine.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-workspace/src/settings.rs` & `uv-0.2.4/crates/uv-workspace/src/settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-workspace/src/workspace.rs` & `uv-0.2.4/crates/uv-workspace/src/workspace.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/Cargo.toml` & `uv-0.2.4/crates/requirements-txt/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/lib.rs` & `uv-0.2.4/crates/requirements-txt/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/requirement.rs` & `uv-0.2.4/crates/requirements-txt/src/requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap` & `uv-0.2.4/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt` & `uv-0.2.4/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/Cargo.toml` & `uv-0.2.4/crates/pep508-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/License-Apache` & `uv-0.2.4/crates/pep508-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/License-BSD` & `uv-0.2.4/crates/pep508-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/Readme.md` & `uv-0.2.4/crates/pep508-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/src/cursor.rs` & `uv-0.2.4/crates/pep508-rs/src/cursor.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/src/lib.rs` & `uv-0.2.4/crates/pep508-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/src/marker.rs` & `uv-0.2.4/crates/pep508-rs/src/marker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/src/origin.rs` & `uv-0.2.4/crates/pep508-rs/src/origin.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/src/unnamed.rs` & `uv-0.2.4/crates/pep508-rs/src/unnamed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pep508-rs/src/verbatim_url.rs` & `uv-0.2.4/crates/pep508-rs/src/verbatim_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/Cargo.toml` & `uv-0.2.4/crates/uv-distribution/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/archive.rs` & `uv-0.2.4/crates/uv-distribution/src/archive.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/distribution_database.rs` & `uv-0.2.4/crates/uv-distribution/src/distribution_database.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/download.rs` & `uv-0.2.4/crates/uv-distribution/src/download.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/error.rs` & `uv-0.2.4/crates/uv-distribution/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/git.rs` & `uv-0.2.4/crates/uv-distribution/src/git.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/index/built_wheel_index.rs` & `uv-0.2.4/crates/uv-distribution/src/index/built_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/index/cached_wheel.rs` & `uv-0.2.4/crates/uv-distribution/src/index/cached_wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/index/registry_wheel_index.rs` & `uv-0.2.4/crates/uv-distribution/src/index/registry_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/lib.rs` & `uv-0.2.4/crates/uv-distribution/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/locks.rs` & `uv-0.2.4/crates/uv-distribution/src/locks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/reporter.rs` & `uv-0.2.4/crates/uv-distribution/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/source/built_wheel_metadata.rs` & `uv-0.2.4/crates/uv-distribution/src/source/built_wheel_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/source/mod.rs` & `uv-0.2.4/crates/uv-distribution/src/source/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-distribution/src/source/revision.rs` & `uv-0.2.4/crates/uv-distribution/src/source/revision.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/Cargo.toml` & `uv-0.2.4/crates/uv-extract/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/src/error.rs` & `uv-0.2.4/crates/uv-extract/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/src/hash.rs` & `uv-0.2.4/crates/uv-extract/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/src/stream.rs` & `uv-0.2.4/crates/uv-extract/src/stream.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/src/sync.rs` & `uv-0.2.4/crates/uv-extract/src/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/src/tar.rs` & `uv-0.2.4/crates/uv-extract/src/tar.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs` & `uv-0.2.4/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-dispatch/Cargo.toml` & `uv-0.2.4/crates/uv-dispatch/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-dispatch/src/lib.rs` & `uv-0.2.4/crates/uv-dispatch/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/Cargo.toml` & `uv-0.2.4/crates/uv-installer/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/compile.rs` & `uv-0.2.4/crates/uv-installer/src/compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/downloader.rs` & `uv-0.2.4/crates/uv-installer/src/downloader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/editable.rs` & `uv-0.2.4/crates/uv-installer/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/installer.rs` & `uv-0.2.4/crates/uv-installer/src/installer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/lib.rs` & `uv-0.2.4/crates/uv-installer/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/pip_compileall.py` & `uv-0.2.4/crates/uv-installer/src/pip_compileall.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/plan.rs` & `uv-0.2.4/crates/uv-installer/src/plan.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/satisfies.rs` & `uv-0.2.4/crates/uv-installer/src/satisfies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/site_packages.rs` & `uv-0.2.4/crates/uv-installer/src/site_packages.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-installer/src/uninstall.rs` & `uv-0.2.4/crates/uv-installer/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/Cargo.toml` & `uv-0.2.4/crates/uv-requirements/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/confirm.rs` & `uv-0.2.4/crates/uv-requirements/src/confirm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/lookahead.rs` & `uv-0.2.4/crates/uv-requirements/src/lookahead.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/pyproject.rs` & `uv-0.2.4/crates/uv-requirements/src/pyproject.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/source_tree.rs` & `uv-0.2.4/crates/uv-requirements/src/source_tree.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/sources.rs` & `uv-0.2.4/crates/uv-requirements/src/sources.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/specification.rs` & `uv-0.2.4/crates/uv-requirements/src/specification.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/unnamed.rs` & `uv-0.2.4/crates/uv-requirements/src/unnamed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/upgrade.rs` & `uv-0.2.4/crates/uv-requirements/src/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-requirements/src/workspace.rs` & `uv-0.2.4/crates/uv-requirements/src/workspace.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-cache/Cargo.toml` & `uv-0.2.4/crates/uv-cache/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-cache/src/cli.rs` & `uv-0.2.4/crates/uv-cache/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-cache/src/lib.rs` & `uv-0.2.4/crates/uv-cache/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-cache/src/removal.rs` & `uv-0.2.4/crates/uv-cache/src/removal.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-cache/src/timestamp.rs` & `uv-0.2.4/crates/uv-cache/src/timestamp.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-cache/src/wheel.rs` & `uv-0.2.4/crates/uv-cache/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/Cargo.toml` & `uv-0.2.4/crates/uv-interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/fetch-version-metadata.py` & `uv-0.2.4/crates/uv-interpreter/fetch-version-metadata.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python/get_interpreter_info.py` & `uv-0.2.4/crates/uv-interpreter/python/get_interpreter_info.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.APACHE` & `uv-0.2.4/crates/uv-interpreter/python/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python/packaging/LICENSE.BSD` & `uv-0.2.4/crates/uv-interpreter/python/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python/packaging/_elffile.py` & `uv-0.2.4/crates/uv-interpreter/python/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python/packaging/_manylinux.py` & `uv-0.2.4/crates/uv-interpreter/python/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python/packaging/_musllinux.py` & `uv-0.2.4/crates/uv-interpreter/python/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/python-version-metadata.json` & `uv-0.2.4/crates/uv-interpreter/python-version-metadata.json`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/discovery.rs` & `uv-0.2.4/crates/uv-interpreter/src/discovery.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/environment.rs` & `uv-0.2.4/crates/uv-interpreter/src/environment.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/implementation.rs` & `uv-0.2.4/crates/uv-interpreter/src/implementation.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/interpreter.rs` & `uv-0.2.4/crates/uv-interpreter/src/interpreter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/lib.rs` & `uv-0.2.4/crates/uv-interpreter/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/managed/downloads.rs` & `uv-0.2.4/crates/uv-interpreter/src/managed/downloads.rs`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         if self.arch.is_none() {
             self.arch = Some(Arch::from_env()?);
         }
         if self.os.is_none() {
             self.os = Some(Os::from_env()?);
         }
         if self.libc.is_none() {
-            self.libc = Some(Libc::from_env()?);
+            self.libc = Some(Libc::from_env());
         }
         Ok(self)
     }
 }
 
 impl FromStr for PythonDownloadRequest {
     type Err = Error;
```

### Comparing `uv-0.2.3/crates/uv-interpreter/src/managed/find.rs` & `uv-0.2.4/crates/uv-interpreter/src/managed/find.rs`

 * *Files 0% similar despite different names*

```diff
@@ -165,10 +165,10 @@
         .collect::<Vec<_>>())
 }
 
 /// Generate a platform portion of a key from the environment.
 fn platform_key_from_env() -> Result<String, Error> {
     let os = Os::from_env()?;
     let arch = Arch::from_env()?;
-    let libc = Libc::from_env()?;
+    let libc = Libc::from_env();
     Ok(format!("{os}-{arch}-{libc}").to_lowercase())
 }
```

### Comparing `uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc` & `uv-0.2.4/crates/uv-interpreter/src/managed/python_versions.inc`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/managed/python_versions.inc.mustache` & `uv-0.2.4/crates/uv-interpreter/src/managed/python_versions.inc.mustache`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/platform.rs` & `uv-0.2.4/crates/uv-interpreter/src/platform.rs`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     pub fn new(os: Os, arch: Arch, libc: Libc) -> Self {
         Self { os, arch, libc }
     }
     pub fn from_env() -> Result<Self, Error> {
         Ok(Self::new(
             Os::from_env()?,
             Arch::from_env()?,
-            Libc::from_env()?,
+            Libc::from_env(),
         ))
     }
 }
 
 impl fmt::Display for Os {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         match *self {
@@ -145,20 +145,22 @@
 impl Arch {
     pub(crate) fn from_env() -> Result<Self, Error> {
         Self::from_str(std::env::consts::ARCH)
     }
 }
 
 impl Libc {
-    pub(crate) fn from_env() -> Result<Self, Error> {
+    pub(crate) fn from_env() -> Self {
         // TODO(zanieb): Perform this lookup
         match std::env::consts::OS {
-            "linux" => Ok(Libc::Gnu),
-            "windows" | "macos" => Ok(Libc::None),
-            _ => Err(Error::LibcNotDetected()),
+            // Supported platforms.
+            "linux" => Libc::Gnu,
+            "windows" | "macos" => Libc::None,
+            // Platforms without explicit support.
+            _ => Libc::None,
         }
     }
 }
 
 impl fmt::Display for Libc {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
```

### Comparing `uv-0.2.3/crates/uv-interpreter/src/py_launcher.rs` & `uv-0.2.4/crates/uv-interpreter/src/py_launcher.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/python_version.rs` & `uv-0.2.4/crates/uv-interpreter/src/python_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/target.rs` & `uv-0.2.4/crates/uv-interpreter/src/target.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/src/virtualenv.rs` & `uv-0.2.4/crates/uv-interpreter/src/virtualenv.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-interpreter/template-version-metadata.py` & `uv-0.2.4/crates/uv-interpreter/template-version-metadata.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/once-map/src/lib.rs` & `uv-0.2.4/crates/once-map/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/Cargo.toml` & `uv-0.2.4/crates/uv-configuration/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/authentication.rs` & `uv-0.2.4/crates/uv-configuration/src/authentication.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/build_options.rs` & `uv-0.2.4/crates/uv-configuration/src/build_options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/concurrency.rs` & `uv-0.2.4/crates/uv-configuration/src/concurrency.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/config_settings.rs` & `uv-0.2.4/crates/uv-configuration/src/config_settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/constraints.rs` & `uv-0.2.4/crates/uv-configuration/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/name_specifiers.rs` & `uv-0.2.4/crates/uv-configuration/src/name_specifiers.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/overrides.rs` & `uv-0.2.4/crates/uv-configuration/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/package_options.rs` & `uv-0.2.4/crates/uv-configuration/src/package_options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/preview.rs` & `uv-0.2.4/crates/uv-configuration/src/preview.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-configuration/src/target_triple.rs` & `uv-0.2.4/crates/uv-configuration/src/target_triple.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/Cargo.toml` & `uv-0.2.4/crates/uv-resolver/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/candidate_selector.rs` & `uv-0.2.4/crates/uv-resolver/src/candidate_selector.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/dependency_mode.rs` & `uv-0.2.4/crates/uv-resolver/src/dependency_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/dependency_provider.rs` & `uv-0.2.4/crates/uv-resolver/src/dependency_provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/editables.rs` & `uv-0.2.4/crates/uv-resolver/src/editables.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/error.rs` & `uv-0.2.4/crates/uv-resolver/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/exclude_newer.rs` & `uv-0.2.4/crates/uv-resolver/src/exclude_newer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/exclusions.rs` & `uv-0.2.4/crates/uv-resolver/src/exclusions.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/flat_index.rs` & `uv-0.2.4/crates/uv-resolver/src/flat_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/lib.rs` & `uv-0.2.4/crates/uv-resolver/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/lock.rs` & `uv-0.2.4/crates/uv-resolver/src/lock.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/manifest.rs` & `uv-0.2.4/crates/uv-resolver/src/manifest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/marker.rs` & `uv-0.2.4/crates/uv-resolver/src/marker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/options.rs` & `uv-0.2.4/crates/uv-resolver/src/options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pins.rs` & `uv-0.2.4/crates/uv-resolver/src/pins.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/prerelease_mode.rs` & `uv-0.2.4/crates/uv-resolver/src/prerelease_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/dependencies.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/dependencies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/distribution.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/distribution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/mod.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/package.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/package.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/priority.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/priority.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/report.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/report.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/pubgrub/specifier.rs` & `uv-0.2.4/crates/uv-resolver/src/pubgrub/specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/python_requirement.rs` & `uv-0.2.4/crates/uv-resolver/src/python_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/redirect.rs` & `uv-0.2.4/crates/uv-resolver/src/redirect.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolution/display.rs` & `uv-0.2.4/crates/uv-resolver/src/resolution/display.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolution/graph.rs` & `uv-0.2.4/crates/uv-resolver/src/resolution/graph.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolution/mod.rs` & `uv-0.2.4/crates/uv-resolver/src/resolution/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolution_mode.rs` & `uv-0.2.4/crates/uv-resolver/src/resolution_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/batch_prefetch.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/batch_prefetch.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/index.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/locals.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/locals.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/mod.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/provider.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/reporter.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/resolver/urls.rs` & `uv-0.2.4/crates/uv-resolver/src/resolver/urls.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap` & `uv-0.2.4/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/version_map.rs` & `uv-0.2.4/crates/uv-resolver/src/version_map.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-resolver/src/yanks.rs` & `uv-0.2.4/crates/uv-resolver/src/yanks.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 use distribution_types::RequirementSource;
 use rustc_hash::{FxHashMap, FxHashSet};
 
 use pep440_rs::Version;
 use pep508_rs::MarkerEnvironment;
 use uv_normalize::PackageName;
 
-use crate::{DependencyMode, Manifest, Preference};
+use crate::{DependencyMode, Manifest};
 
 /// A set of package versions that are permitted, even if they're marked as yanked by the
 /// relevant index.
 #[derive(Debug, Default, Clone)]
 pub struct AllowedYanks(FxHashMap<PackageName, FxHashSet<Version>>);
 
 impl AllowedYanks {
     pub fn from_manifest(
         manifest: &Manifest,
         markers: Option<&MarkerEnvironment>,
         dependencies: DependencyMode,
     ) -> Self {
         let mut allowed_yanks = FxHashMap::<PackageName, FxHashSet<Version>>::default();
 
-        for requirement in manifest
-            .requirements(markers, dependencies)
-            .chain(manifest.preferences.iter().map(Preference::requirement))
-        {
+        // Allow yanks for any pinned input requirements.
+        for requirement in manifest.requirements(markers, dependencies) {
             let RequirementSource::Registry { specifier, .. } = &requirement.source else {
                 continue;
             };
             let [specifier] = specifier.as_ref() else {
                 continue;
             };
             if matches!(
@@ -36,14 +34,23 @@
             ) {
                 allowed_yanks
                     .entry(requirement.name.clone())
                     .or_default()
                     .insert(specifier.version().clone());
             }
         }
+
+        // Allow yanks for any packages that are already pinned in the lockfile.
+        for preference in &manifest.preferences {
+            allowed_yanks
+                .entry(preference.name().clone())
+                .or_default()
+                .insert(preference.version().clone());
+        }
+
         Self(allowed_yanks)
     }
 
     /// Returns versions for the given package which are allowed even if marked as yanked by the
     /// relevant index.
     pub fn allowed_versions(&self, package_name: &PackageName) -> Option<&FxHashSet<Version>> {
         self.0.get(package_name)
```

### Comparing `uv-0.2.3/crates/uv-resolver/tests/resolver.rs` & `uv-0.2.4/crates/uv-resolver/tests/resolver.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 use std::str::FromStr;
 
 use anyhow::Result;
 use chrono::{DateTime, Utc};
 use once_cell::sync::Lazy;
 
 use distribution_types::{CachedDist, IndexLocations, Requirement, Resolution, SourceDist};
+use pep440_rs::Version;
 use pep508_rs::{MarkerEnvironment, MarkerEnvironmentBuilder};
 use platform_tags::{Arch, Os, Platform, Tags};
 use uv_cache::Cache;
 use uv_client::RegistryClientBuilder;
 use uv_configuration::{
     BuildKind, Concurrency, Constraints, NoBinary, NoBuild, Overrides, SetupPyStrategy,
 };
 use uv_distribution::DistributionDatabase;
 use uv_interpreter::{find_default_interpreter, Interpreter, PythonEnvironment};
+use uv_normalize::PackageName;
 use uv_resolver::{
     DisplayResolutionGraph, ExcludeNewer, Exclusions, FlatIndex, InMemoryIndex, Manifest, Options,
     OptionsBuilder, PreReleaseMode, Preference, PythonRequirement, ResolutionGraph, ResolutionMode,
     Resolver,
 };
 use uv_types::{
     BuildContext, BuildIsolation, EmptyInstalledPackages, HashStrategy, SourceBuildTrait,
@@ -469,17 +471,18 @@
 async fn black_respect_preference() -> Result<()> {
     let manifest = Manifest::new(
         vec![Requirement::from(pep508_rs::Requirement::from_str(
             "black<=23.9.1",
         )?)],
         Constraints::default(),
         Overrides::default(),
-        vec![Preference::from_requirement(Requirement::from(
-            pep508_rs::Requirement::from_str("black==23.9.0")?,
-        ))],
+        vec![Preference::simple(
+            PackageName::from_str("black")?,
+            Version::from_str("23.9.0")?,
+        )],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
 
     let options = OptionsBuilder::new()
@@ -509,17 +512,18 @@
 async fn black_ignore_preference() -> Result<()> {
     let manifest = Manifest::new(
         vec![Requirement::from(pep508_rs::Requirement::from_str(
             "black<=23.9.1",
         )?)],
         Constraints::default(),
         Overrides::default(),
-        vec![Preference::from_requirement(Requirement::from(
-            pep508_rs::Requirement::from_str("black==23.9.2")?,
-        ))],
+        vec![Preference::simple(
+            PackageName::from_str("black")?,
+            Version::from_str("23.9.2")?,
+        )],
         None,
         vec![],
         Exclusions::default(),
         vec![],
     );
     let options = OptionsBuilder::new()
         .exclude_newer(Some(*EXCLUDE_NEWER))
```

### Comparing `uv-0.2.3/crates/uv-virtualenv/Cargo.toml` & `uv-0.2.4/crates/uv-virtualenv/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/_virtualenv.py` & `uv-0.2.4/crates/uv-virtualenv/src/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.bat` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.csh` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate.csh`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.fish` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate.fish`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.nu` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate.nu`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate.ps1` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate.ps1`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/activate_this.py` & `uv-0.2.4/crates/uv-virtualenv/src/activator/activate_this.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/deactivate.bat` & `uv-0.2.4/crates/uv-virtualenv/src/activator/deactivate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/activator/pydoc.bat` & `uv-0.2.4/crates/uv-virtualenv/src/activator/pydoc.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/bare.rs` & `uv-0.2.4/crates/uv-virtualenv/src/bare.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-virtualenv/src/lib.rs` & `uv-0.2.4/crates/uv-virtualenv/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-build/Cargo.toml` & `uv-0.2.4/crates/uv-build/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-build/src/lib.rs` & `uv-0.2.4/crates/uv-build/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/Cargo.toml` & `uv-0.2.4/crates/uv-client/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/base_client.rs` & `uv-0.2.4/crates/uv-client/src/base_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/cached_client.rs` & `uv-0.2.4/crates/uv-client/src/cached_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/error.rs` & `uv-0.2.4/crates/uv-client/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/flat_index.rs` & `uv-0.2.4/crates/uv-client/src/flat_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/html.rs` & `uv-0.2.4/crates/uv-client/src/html.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/httpcache/control.rs` & `uv-0.2.4/crates/uv-client/src/httpcache/control.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/httpcache/mod.rs` & `uv-0.2.4/crates/uv-client/src/httpcache/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/lib.rs` & `uv-0.2.4/crates/uv-client/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/linehaul.rs` & `uv-0.2.4/crates/uv-client/src/linehaul.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/middleware.rs` & `uv-0.2.4/crates/uv-client/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/registry_client.rs` & `uv-0.2.4/crates/uv-client/src/registry_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/remote_metadata.rs` & `uv-0.2.4/crates/uv-client/src/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/src/rkyvutil.rs` & `uv-0.2.4/crates/uv-client/src/rkyvutil.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/tests/remote_metadata.rs` & `uv-0.2.4/crates/uv-client/tests/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-client/tests/user_agent_version.rs` & `uv-0.2.4/crates/uv-client/tests/user_agent_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/Cargo.toml` & `uv-0.2.4/crates/distribution-filename/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/src/build_tag.rs` & `uv-0.2.4/crates/distribution-filename/src/build_tag.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/src/lib.rs` & `uv-0.2.4/crates/distribution-filename/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap` & `uv-0.2.4/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap` & `uv-0.2.4/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/src/source_dist.rs` & `uv-0.2.4/crates/distribution-filename/src/source_dist.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/distribution-filename/src/wheel.rs` & `uv-0.2.4/crates/distribution-filename/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/platform-tags/src/platform.rs` & `uv-0.2.4/crates/platform-tags/src/platform.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/platform-tags/src/tags.rs` & `uv-0.2.4/crates/platform-tags/src/tags.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-normalize/src/extra_name.rs` & `uv-0.2.4/crates/uv-normalize/src/extra_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-normalize/src/lib.rs` & `uv-0.2.4/crates/uv-normalize/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv-normalize/src/package_name.rs` & `uv-0.2.4/crates/uv-normalize/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/Cargo.toml` & `uv-0.2.4/crates/pypi-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/base_url.rs` & `uv-0.2.4/crates/pypi-types/src/base_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/direct_url.rs` & `uv-0.2.4/crates/pypi-types/src/direct_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/lenient_requirement.rs` & `uv-0.2.4/crates/pypi-types/src/lenient_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/metadata.rs` & `uv-0.2.4/crates/pypi-types/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/parsed_url.rs` & `uv-0.2.4/crates/pypi-types/src/parsed_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/scheme.rs` & `uv-0.2.4/crates/pypi-types/src/scheme.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/pypi-types/src/simple_json.rs` & `uv-0.2.4/crates/pypi-types/src/simple_json.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/Cargo.toml` & `uv-0.2.4/crates/install-wheel-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/Readme.md` & `uv-0.2.4/crates/install-wheel-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/src/lib.rs` & `uv-0.2.4/crates/install-wheel-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/src/linker.rs` & `uv-0.2.4/crates/install-wheel-rs/src/linker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/src/metadata.rs` & `uv-0.2.4/crates/install-wheel-rs/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/src/script.rs` & `uv-0.2.4/crates/install-wheel-rs/src/script.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/src/uninstall.rs` & `uv-0.2.4/crates/install-wheel-rs/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/install-wheel-rs/src/wheel.rs` & `uv-0.2.4/crates/install-wheel-rs/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/Cargo.toml` & `uv-0.2.4/crates/uv/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uv"
-version = "0.2.3"
+version = "0.2.4"
 edition = { workspace = true }
 rust-version = { workspace = true }
 homepage = { workspace = true }
 documentation = { workspace = true }
 repository = { workspace = true }
 authors = { workspace = true }
 license = { workspace = true }
@@ -12,15 +12,14 @@
 
 [lints]
 workspace = true
 
 [dependencies]
 distribution-types = { workspace = true }
 install-wheel-rs = { workspace = true, features = ["clap"], default-features = false }
-pep440_rs = { workspace = true }
 pep508_rs = { workspace = true }
 platform-tags = { workspace = true }
 pypi-types = { workspace = true }
 requirements-txt = { workspace = true, features = ["http"] }
 uv-auth = { workspace = true }
 uv-cache = { workspace = true, features = ["clap"] }
 uv-client = { workspace = true }
```

### Comparing `uv-0.2.3/crates/uv/build.rs` & `uv-0.2.4/crates/uv/build.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/cli.rs` & `uv-0.2.4/crates/uv/src/cli.rs`

 * *Files 1% similar despite different names*

```diff
@@ -461,28 +461,27 @@
     /// option allows you to specify a different interpreter.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(long, verbatim_doc_comment, group = "discovery")]
+    #[arg(long, verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// Install packages into the system Python.
     ///
     /// By default, `uv` uses the virtual environment in the current working directory or any parent
     /// directory, falling back to searching for a Python executable in `PATH`. The `--system`
     /// option instructs `uv` to avoid using a virtual environment Python and restrict its search to
     /// the system path.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 
@@ -764,36 +763,29 @@
     /// workflows.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// Install packages into the system Python.
     ///
     /// By default, `uv` installs into the virtual environment in the current working directory or
     /// any parent directory. The `--system` option instructs `uv` to instead use the first Python
     /// found in the system `PATH`.
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution, as it can modify the system Python installation.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 
@@ -803,15 +795,14 @@
     /// environments, when installing into Python installations that are managed by an external
     /// package manager, like `apt`. It should be used with caution, as such Python installations
     /// explicitly recommend against modifications by other package managers (like `uv` or `pip`).
     #[arg(
         long,
         env = "UV_BREAK_SYSTEM_PACKAGES",
         value_parser = clap::builder::BoolishValueParser::new(),
-        requires = "discovery",
         overrides_with("no_break_system_packages")
     )]
     pub(crate) break_system_packages: bool,
 
     #[arg(long, overrides_with("break_system_packages"))]
     pub(crate) no_break_system_packages: bool,
 
@@ -1159,36 +1150,29 @@
     /// workflows.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// Install packages into the system Python.
     ///
     /// By default, `uv` installs into the virtual environment in the current working directory or
     /// any parent directory. The `--system` option instructs `uv` to instead use the first Python
     /// found in the system `PATH`.
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution, as it can modify the system Python installation.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 
@@ -1198,15 +1182,14 @@
     /// environments, when installing into Python installations that are managed by an external
     /// package manager, like `apt`. It should be used with caution, as such Python installations
     /// explicitly recommend against modifications by other package managers (like `uv` or `pip`).
     #[arg(
         long,
         env = "UV_BREAK_SYSTEM_PACKAGES",
         value_parser = clap::builder::BoolishValueParser::new(),
-        requires = "discovery",
         overrides_with("no_break_system_packages")
     )]
     pub(crate) break_system_packages: bool,
 
     #[arg(long, overrides_with("break_system_packages"))]
     pub(crate) no_break_system_packages: bool,
 
@@ -1375,21 +1358,15 @@
     /// workflows.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// Attempt to use `keyring` for authentication for remote requirements files.
     ///
     /// Due to not having Python imports, only `--keyring-provider subprocess` argument is currently
     /// implemented `uv` will try to use `keyring` via CLI when this flag is used.
     ///
@@ -1405,15 +1382,14 @@
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution, as it can modify the system Python installation.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 
@@ -1423,15 +1399,14 @@
     /// environments, when installing into Python installations that are managed by an external
     /// package manager, like `apt`. It should be used with caution, as such Python installations
     /// explicitly recommend against modifications by other package managers (like `uv` or `pip`).
     #[arg(
         long,
         env = "UV_BREAK_SYSTEM_PACKAGES",
         value_parser = clap::builder::BoolishValueParser::new(),
-        requires = "discovery",
         overrides_with("no_break_system_packages")
     )]
     pub(crate) break_system_packages: bool,
 
     #[arg(long, overrides_with("break_system_packages"))]
     pub(crate) no_break_system_packages: bool,
 
@@ -1463,21 +1438,15 @@
     /// falling back to the system Python if no virtual environment is found.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// List packages for the system Python.
     ///
     /// By default, `uv` lists packages in the currently activated virtual environment, or a virtual
     /// environment (`.venv`) located in the current working directory or any parent directory,
     /// falling back to the system Python if no virtual environment is found. The `--system` option
@@ -1485,15 +1454,14 @@
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 }
@@ -1532,21 +1500,15 @@
     /// falling back to the system Python if no virtual environment is found.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// List packages for the system Python.
     ///
     /// By default, `uv` lists packages in the currently activated virtual environment, or a virtual
     /// environment (`.venv`) located in the current working directory or any parent directory,
     /// falling back to the system Python if no virtual environment is found. The `--system` option
@@ -1554,15 +1516,14 @@
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 
@@ -1580,21 +1541,15 @@
     /// falling back to the system Python if no virtual environment is found.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// List packages for the system Python.
     ///
     /// By default, `uv` lists packages in the currently activated virtual environment, or a virtual
     /// environment (`.venv`) located in the current working directory or any parent directory,
     /// falling back to the system Python if no virtual environment is found. The `--system` option
@@ -1602,15 +1557,14 @@
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 }
@@ -1636,21 +1590,15 @@
     /// falling back to the system Python if no virtual environment is found.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// List packages for the system Python.
     ///
     /// By default, `uv` lists packages in the currently activated virtual environment, or a virtual
     /// environment (`.venv`) located in the current working directory or any parent directory,
     /// falling back to the system Python if no virtual environment is found. The `--system` option
@@ -1658,15 +1606,14 @@
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 }
@@ -1680,36 +1627,29 @@
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
     ///
     /// Note that this is different from `--python-version` in `pip compile`, which takes `3.10` or `3.10.13` and
     /// doesn't look for a Python interpreter on disk.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 
     /// Use the system Python to uninstall packages.
     ///
     /// By default, `uv` uninstalls from the virtual environment in the current working directory or
     /// any parent directory. The `--system` option instructs `uv` to use the first Python found in
     /// the system `PATH`.
     ///
     /// WARNING: `--system` is intended for use in continuous integration (CI) environments and
     /// should be used with caution, as it can modify the system Python installation.
     #[arg(
         long,
         env = "UV_SYSTEM_PYTHON",
         value_parser = clap::builder::BoolishValueParser::new(),
-        group = "discovery",
         overrides_with("no_system")
     )]
     pub(crate) system: bool,
 
     #[arg(long, overrides_with("system"))]
     pub(crate) no_system: bool,
 
@@ -1842,21 +1782,15 @@
     /// option allows you to specify a different interpreter.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 }
 
 #[derive(Args)]
 #[allow(clippy::struct_excessive_bools)]
 pub(crate) struct SyncArgs {
     /// The Python interpreter to use to build the run environment.
@@ -1866,21 +1800,15 @@
     /// option allows you to specify a different interpreter.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 }
 
 #[derive(Args)]
 #[allow(clippy::struct_excessive_bools)]
 pub(crate) struct LockArgs {
     /// The Python interpreter to use to build the run environment.
@@ -1890,21 +1818,15 @@
     /// option allows you to specify a different interpreter.
     ///
     /// Supported formats:
     /// - `3.10` looks for an installed Python 3.10 using `py --list-paths` on Windows, or
     ///   `python3.10` on Linux and macOS.
     /// - `python3.10` or `python.exe` looks for a binary with the given name in `PATH`.
     /// - `/home/ferris/.local/bin/python3.10` uses the exact Python at the given path.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 }
 
 #[derive(Args)]
 #[allow(clippy::struct_excessive_bools)]
 struct AddArgs {
     /// The name of the package to add (e.g., `Django==4.2.6`).
@@ -1947,16 +1869,10 @@
     pub(crate) from: Option<String>,
 
     /// Include the following extra requirements.
     #[arg(long)]
     pub(crate) with: Vec<String>,
 
     /// The Python interpreter to use to build the run environment.
-    #[arg(
-        long,
-        short,
-        env = "UV_PYTHON",
-        verbatim_doc_comment,
-        group = "discovery"
-    )]
+    #[arg(long, short, env = "UV_PYTHON", verbatim_doc_comment)]
     pub(crate) python: Option<String>,
 }
```

### Comparing `uv-0.2.3/crates/uv/src/commands/cache_clean.rs` & `uv-0.2.4/crates/uv/src/commands/cache_clean.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/cache_prune.rs` & `uv-0.2.4/crates/uv/src/commands/cache_prune.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/mod.rs` & `uv-0.2.4/crates/uv/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/check.rs` & `uv-0.2.4/crates/uv/src/commands/pip/check.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/compile.rs` & `uv-0.2.4/crates/uv/src/commands/pip/compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/freeze.rs` & `uv-0.2.4/crates/uv/src/commands/pip/freeze.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/install.rs` & `uv-0.2.4/crates/uv/src/commands/pip/install.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/list.rs` & `uv-0.2.4/crates/uv/src/commands/pip/list.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/operations.rs` & `uv-0.2.4/crates/uv/src/commands/pip/operations.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 //! Common operations shared across the `pip` API and subcommands.
 
-use pypi_types::{ParsedUrl, ParsedUrlError};
 use std::fmt::Write;
 use std::path::PathBuf;
 
 use anyhow::{anyhow, Context};
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use tracing::debug;
 
 use distribution_types::{
     CachedDist, Diagnostic, InstalledDist, Requirement, ResolutionDiagnostic,
     UnresolvedRequirementSpecification,
 };
 use distribution_types::{
-    DistributionMetadata, IndexLocations, InstalledMetadata, InstalledVersion, LocalDist, Name,
-    RequirementSource, Resolution,
+    DistributionMetadata, IndexLocations, InstalledMetadata, LocalDist, Name, Resolution,
 };
 use install_wheel_rs::linker::LinkMode;
-use pep440_rs::{VersionSpecifier, VersionSpecifiers};
-use pep508_rs::{MarkerEnvironment, VerbatimUrl};
+use pep508_rs::MarkerEnvironment;
 use platform_tags::Tags;
 use uv_cache::Cache;
 use uv_client::{BaseClientBuilder, RegistryClient};
 use uv_configuration::{
     Concurrency, Constraints, NoBinary, Overrides, PreviewMode, Reinstall, Upgrade,
 };
 use uv_dispatch::BuildDispatch;
@@ -198,46 +195,20 @@
         }
         DependencyMode::Direct => Vec::new(),
     };
 
     // TODO(zanieb): Consider consuming these instead of cloning
     let exclusions = Exclusions::new(reinstall.clone(), upgrade.clone());
 
-    // Prefer current site packages; filter out packages that are marked for reinstall or upgrade
+    // Prefer current site packages; filter out packages that are marked for reinstall or upgrade.
     let preferences = installed_packages
         .iter()
         .filter(|dist| !exclusions.contains(dist.name()))
-        .map(|dist| {
-            let source = match dist.installed_version() {
-                InstalledVersion::Version(version) => RequirementSource::Registry {
-                    specifier: VersionSpecifiers::from(VersionSpecifier::equals_version(
-                        version.clone(),
-                    )),
-                    // TODO(konstin): track index
-                    index: None,
-                },
-                InstalledVersion::Url(url, _version) => {
-                    let parsed_url = ParsedUrl::try_from(url.clone())?;
-                    RequirementSource::from_parsed_url(
-                        parsed_url,
-                        VerbatimUrl::from_url(url.clone()),
-                    )
-                }
-            };
-            let requirement = Requirement {
-                name: dist.name().clone(),
-                extras: vec![],
-                marker: None,
-                source,
-                origin: None,
-            };
-            Ok(Preference::from_requirement(requirement))
-        })
-        .collect::<Result<_, _>>()
-        .map_err(Error::UnsupportedInstalledDist)?;
+        .map(Preference::from_installed)
+        .collect::<Vec<_>>();
 
     // Create a manifest of the requirements.
     let manifest = Manifest::new(
         requirements,
         constraints,
         overrides,
         preferences,
@@ -768,11 +739,8 @@
     Fmt(#[from] std::fmt::Error),
 
     #[error(transparent)]
     Lookahead(#[from] uv_requirements::LookaheadError),
 
     #[error(transparent)]
     Anyhow(#[from] anyhow::Error),
-
-    #[error("Installed distribution has unsupported type")]
-    UnsupportedInstalledDist(#[source] Box<ParsedUrlError>),
 }
```

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/show.rs` & `uv-0.2.4/crates/uv/src/commands/pip/show.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/sync.rs` & `uv-0.2.4/crates/uv/src/commands/pip/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/pip/uninstall.rs` & `uv-0.2.4/crates/uv/src/commands/pip/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/project/lock.rs` & `uv-0.2.4/crates/uv/src/commands/project/lock.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/project/mod.rs` & `uv-0.2.4/crates/uv/src/commands/project/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/project/run.rs` & `uv-0.2.4/crates/uv/src/commands/project/run.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/project/sync.rs` & `uv-0.2.4/crates/uv/src/commands/project/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/reporters.rs` & `uv-0.2.4/crates/uv/src/commands/reporters.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/self_update.rs` & `uv-0.2.4/crates/uv/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/tool/run.rs` & `uv-0.2.4/crates/uv/src/commands/tool/run.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/venv.rs` & `uv-0.2.4/crates/uv/src/commands/venv.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/commands/version.rs` & `uv-0.2.4/crates/uv/src/commands/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/compat/mod.rs` & `uv-0.2.4/crates/uv/src/compat/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/editables.rs` & `uv-0.2.4/crates/uv/src/editables.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/logging.rs` & `uv-0.2.4/crates/uv/src/logging.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/main.rs` & `uv-0.2.4/crates/uv/src/main.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/printer.rs` & `uv-0.2.4/crates/uv/src/printer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/settings.rs` & `uv-0.2.4/crates/uv/src/settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/shell.rs` & `uv-0.2.4/crates/uv/src/shell.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/src/version.rs` & `uv-0.2.4/crates/uv/src/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/cache_prune.rs` & `uv-0.2.4/crates/uv/tests/cache_prune.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/common/mod.rs` & `uv-0.2.4/crates/uv/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/lock.rs` & `uv-0.2.4/crates/uv/tests/lock.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_check.rs` & `uv-0.2.4/crates/uv/tests/pip_check.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_compile.rs` & `uv-0.2.4/crates/uv/tests/pip_compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_compile_scenarios.rs` & `uv-0.2.4/crates/uv/tests/pip_compile_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_freeze.rs` & `uv-0.2.4/crates/uv/tests/pip_freeze.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_install.rs` & `uv-0.2.4/crates/uv/tests/pip_install.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_install_scenarios.rs` & `uv-0.2.4/crates/uv/tests/pip_install_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_list.rs` & `uv-0.2.4/crates/uv/tests/pip_list.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_show.rs` & `uv-0.2.4/crates/uv/tests/pip_show.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_sync.rs` & `uv-0.2.4/crates/uv/tests/pip_sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/pip_uninstall.rs` & `uv-0.2.4/crates/uv/tests/pip_uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/self_update.rs` & `uv-0.2.4/crates/uv/tests/self_update.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/crates/uv/tests/venv.rs` & `uv-0.2.4/crates/uv/tests/venv.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/Cargo.lock` & `uv-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -4467,15 +4467,15 @@
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "uv"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "anstream",
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "axoupdater",
  "base64 0.22.1",
@@ -4492,15 +4492,14 @@
  "indoc",
  "insta",
  "install-wheel-rs",
  "itertools 0.13.0",
  "miette",
  "mimalloc",
  "owo-colors",
- "pep440_rs",
  "pep508_rs",
  "platform-tags",
  "predicates",
  "pypi-types",
  "rayon",
  "regex",
  "requirements-txt",
@@ -5053,15 +5052,15 @@
  "uv-configuration",
  "uv-interpreter",
  "uv-normalize",
 ]
 
 [[package]]
 name = "uv-version"
-version = "0.2.3"
+version = "0.2.4"
 
 [[package]]
 name = "uv-virtualenv"
 version = "0.0.4"
 dependencies = [
  "fs-err",
  "itertools 0.13.0",
```

### Comparing `uv-0.2.3/Cargo.toml` & `uv-0.2.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/pyproject.toml` & `uv-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "uv"
-version = "0.2.3"
+version = "0.2.4"
 description = "An extremely fast Python package installer and resolver, written in Rust."
 authors = [{ name = "Astral Software Inc.", email = "hey@astral.sh" }]
 requires-python = ">=3.8"
 keywords = [
   "uv", "requirements", "packaging"
 ]
 classifiers = [
```

### Comparing `uv-0.2.3/python/uv/__main__.py` & `uv-0.2.4/python/uv/__main__.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/python/uv/__init__.py` & `uv-0.2.4/python/uv/__init__.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/README.md` & `uv-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/LICENSE-APACHE` & `uv-0.2.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/LICENSE-MIT` & `uv-0.2.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `uv-0.2.3/PKG-INFO` & `uv-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uv
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

