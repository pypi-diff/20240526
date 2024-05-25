# Comparing `tmp/yt_dlp-2024.5.5.232701.dev0.tar.gz` & `tmp/yt_dlp-2024.5.8.232715.dev0.tar.gz`

## Comparing `yt_dlp-2024.5.5.232701.dev0.tar` & `yt_dlp-2024.5.8.232715.dev0.tar`

### file list

```diff
@@ -1,1183 +1,1183 @@
--rw-r--r--   0        0        0   428935 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/Changelog.md
--rw-r--r--   0        0        0   149757 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/README.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/setup.cfg
--rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/supportedsites.md
--rw-r--r--   0        0        0   146693 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt-dlp.1
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/completions/bash/yt-dlp
--rw-r--r--   0        0        0    50227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/completions/fish/yt-dlp.fish
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/completions/zsh/_yt-dlp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/bash-completion.in
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/bash-completion.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/changelog_override.json
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/changelog_override.schema.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/check-porn.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/cli_to_api.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/fish-completion.in
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/fish-completion.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/generate_aes_testdata.py
--rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/install_deps.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/lazy_load_template.py
--rw-r--r--   0        0        0    41043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/logo.ico
--rw-r--r--   0        0        0    18382 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/make_changelog.py
--rwxr-xr-x   0        0        0      763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/make_contributing.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/make_issue_template.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/make_lazy_extractors.py
--rwxr-xr-x   0        0        0     2892 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/make_readme.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/make_supportedsites.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/prepare_manpage.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/run_tests.bat
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/run_tests.py
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/run_tests.sh
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/set-variant.py
--rwxr-xr-x   0        0        0     4849 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/tomlparse.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/update-version.py
--rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/update_changelog.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/zsh-completion.in
--rwxr-xr-x   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/devscripts/zsh-completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/conftest.py
--rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/helper.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/parameters.json
--rw-r--r--   0        0        0   100697 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_InfoExtractor.py
--rw-r--r--   0        0        0    57080 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_YoutubeDL.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_YoutubeDLCookieJar.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_aes.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_age_restriction.py
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_all_urls.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_cache.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_compat.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_config.py
--rw-r--r--   0        0        0    13665 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_cookies.py
--rwxr-xr-x   0        0        0    12247 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_download.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_downloader_external.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_downloader_http.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_execution.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_iqiyi_sdk_interpreter.py
--rw-r--r--   0        0        0    18408 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_jsinterp.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_netrc.py
--rw-r--r--   0        0        0    87519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_networking.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_networking_utils.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_overwrites.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_plugins.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_post_hooks.py
--rw-r--r--   0        0        0    30542 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_postprocessors.py
--rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_socks.py
--rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_subtitles.py
--rw-r--r--   0        0        0    24268 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_traversal.py
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_update.py
--rw-r--r--   0        0        0    97858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_utils.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_verbose_output.py
--rw-r--r--   0        0        0    16532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_websockets.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_write_annotations.py.disabled
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_youtube_lists.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_youtube_misc.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/test_youtube_signature.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testcert.pem
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/ca.crt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/ca.key
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/ca.srl
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/client.crt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/client.csr
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/client.key
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/clientencrypted.key
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/clientwithencryptedkey.crt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/clientwithkey.crt
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/instructions.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/cookies/httponly_cookies.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/cookies/malformed_cookies.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/cookies/session_cookies.txt
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/f4m/custom_base_url.f4m
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/ism/ec-3_test.Manifest
--rw-r--r--   0        0        0    23179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/ism/sintel.Manifest
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/m3u8/bipbop_16x9.m3u8
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/float_duration.mpd
--rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/subtitles.mpd
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/unfragmented.mpd
--rw-r--r--   0        0        0    22374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/urls_only.mpd
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/xspf/foo_xspf.xspf
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/yt_dlp_plugins/extractor/_ignore.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/yt_dlp_plugins/extractor/ignore.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/yt_dlp_plugins/extractor/normal.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/yt_dlp_plugins/postprocessor/normal.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/zipped.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/zipped.py
--rw-r--r--   0        0        0   211705 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/YoutubeDL.py
--rw-r--r--   0        0        0    47722 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/__main__.py
--rw-r--r--   0        0        0    22402 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/aes.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/cache.py
--rw-r--r--   0        0        0    54844 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/cookies.py
--rw-r--r--   0        0        0    34646 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/jsinterp.py
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/minicurses.py
--rw-r--r--   0        0        0    96731 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/options.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/plugins.py
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/socks.py
--rw-r--r--   0        0        0    25165 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/update.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/version.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/webvtt.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/__pyinstaller/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/_deprecated.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/_legacy.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/compat_utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/functools.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/imghdr.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/shutil.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/types.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/urllib/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/urllib/request.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/dependencies/Cryptodome.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/dependencies/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/__init__.py
--rw-r--r--   0        0        0    19691 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/common.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/dash.py
--rw-r--r--   0        0        0    28090 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/external.py
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/f4m.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/fc2.py
--rw-r--r--   0        0        0    21795 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/fragment.py
--rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/hls.py
--rw-r--r--   0        0        0    16863 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/http.py
--rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/ism.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/mhtml.py
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/niconico.py
--rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/rtmp.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/rtsp.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/websocket.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/youtube_live_chat.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/__init__.py
--rw-r--r--   0        0        0    52880 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/_extractors.py
--rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abc.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abcnews.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abcotvs.py
--rw-r--r--   0        0        0    19939 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abematv.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/academicearth.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/acast.py
--rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/acfun.py
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adn.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adobeconnect.py
--rw-r--r--   0        0        0    52679 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adobepass.py
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adobetv.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adultswim.py
--rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aenetworks.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aeonco.py
--rw-r--r--   0        0        0    17843 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/afreecatv.py
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/agora.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/airtv.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aitube.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aliexpress.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aljazeera.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/allocine.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/allstar.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/alphaporno.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/alsace20tv.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/altcensored.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/alura.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amadeustv.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amara.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amazon.py
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amazonminitv.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amcnetworks.py
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/americastestkitchen.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amp.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/anchorfm.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/angel.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/antenna.py
--rw-r--r--   0        0        0    26757 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/anvato.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aol.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/apa.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aparat.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/appleconnect.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/applepodcasts.py
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/appletrailers.py
--rw-r--r--   0        0        0    46353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/archiveorg.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arcpublishing.py
--rw-r--r--   0        0        0    26748 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ard.py
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arkena.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arnes.py
--rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/art19.py
--rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arte.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/asobichannel.py
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/asobistage.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/atresplayer.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/atscaleconf.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/atvat.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audimedia.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audioboom.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audiodraft.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audiomack.py
--rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audius.py
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/awaan.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aws.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/axs.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/azmedien.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/baidu.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/banbye.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bandaichannel.py
--rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bandcamp.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bannedvideo.py
--rw-r--r--   0        0        0    72720 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bbc.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/beatbump.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/beatport.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/beeg.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/behindkink.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bellmedia.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/berufetv.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bet.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bfi.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bfmtv.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bibeltv.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bigflix.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bigo.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bild.py
--rw-r--r--   0        0        0    93818 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bilibili.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/biobiochiletv.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bitchute.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/blackboardcollaborate.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bleacherreport.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/blerp.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/blogger.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bloomberg.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bokecc.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bongacams.py
--rw-r--r--   0        0        0     8894 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/boosty.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bostonglobe.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/box.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/boxcast.py
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bpb.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/br.py
--rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/brainpop.py
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bravotv.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/breitbart.py
--rw-r--r--   0        0        0    42705 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/brightcove.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/brilliantpala.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bundesliga.py
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bundestag.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/businessinsider.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/buzzfeed.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/byutv.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/c56.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cableav.py
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/callin.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/caltrans.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cam4.py
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camdemy.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camfm.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cammodels.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camsoda.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camtasia.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canal1.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canalalpha.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canalc2.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canalplus.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/caracoltv.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cartoonnetwork.py
--rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbc.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbs.py
--rw-r--r--   0        0        0    19544 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbsnews.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbssports.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ccc.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ccma.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cctv.py
--rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cda.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cellebrite.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ceskatelevize.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cgtn.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/charlierose.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/chaturbate.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/chilloutzone.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/chzzk.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cinemax.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cinetecamilano.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cineverse.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ciscolive.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ciscowebex.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cjsw.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clipchamp.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clippit.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cliprs.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/closertotruth.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cloudflarestream.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cloudycdn.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clubic.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clyp.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cmt.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cnbc.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cnn.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/comedycentral.py
--rw-r--r--   0        0        0   192152 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/common.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/commonmistakes.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/commonprotocols.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/condenast.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/contv.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/corus.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/coub.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cozytv.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cpac.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cracked.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crackle.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/craftsy.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crooksandliars.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crowdbunker.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crtvg.py
--rw-r--r--   0        0        0    29342 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crunchyroll.py
--rw-r--r--   0        0        0    12105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cspan.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ctsnews.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ctv.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ctvnews.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cultureunplugged.py
--rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/curiositystream.py
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cwtv.py
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cybrary.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dacast.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dailymail.py
--rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dailymotion.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dailywire.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/damtomo.py
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/daum.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/daystar.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dbtv.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dctp.py
--rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/deezer.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/democracynow.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/detik.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/deuxm.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dfb.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dhm.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/digitalconcerthall.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/digiteka.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/discogs.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/discovery.py
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/discoverygo.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/disney.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dispeak.py
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dlf.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dlive.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/douyutv.py
--rw-r--r--   0        0        0    41198 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dplay.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drbonanza.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dreisat.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drooble.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dropbox.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dropout.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drtuber.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drtv.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dtube.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/duboku.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dumpert.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/duoplay.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dvtv.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dw.py
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eagleplatform.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ebaumsworld.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ebay.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/egghead.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eighttracks.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/einthusan.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eitb.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/elementorembed.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/elonet.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/elpais.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eltrecetv.py
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/embedly.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/epicon.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/epidemicsound.py
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eplus.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/epoch.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eporner.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/erocast.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eroprofile.py
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/err.py
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ertgr.py
--rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/espn.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ettutv.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/europa.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/europeantour.py
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eurosport.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/euscreen.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/expressen.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/extractors.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eyedotv.py
--rw-r--r--   0        0        0    48415 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/facebook.py
--rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fancode.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fathom.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/faz.py
--rw-r--r--   0        0        0    10584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fc2.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fczenit.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fifa.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/filmon.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/filmweb.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/firsttv.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fivetv.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/flextv.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/flickr.py
--rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/floatplane.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/folketinget.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/footyroom.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/formula1.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fourtube.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fox.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fox9.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/foxnews.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/foxsports.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fptplay.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/franceinter.py
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/francetv.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/freesound.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/freespeech.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/freetv.py
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/frontendmasters.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fujitv.py
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/funimation.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/funk.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/funker530.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fuyintv.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gab.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gaia.py
--rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gamejolt.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gamespot.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gamestar.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gaskrank.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gazeta.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gdcvault.py
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gedidigital.py
--rw-r--r--   0        0        0   119486 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/generic.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/genericembeds.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/genius.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/getcourseru.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gettr.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/giantbomb.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gigya.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/glide.py
--rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/globalplayer.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/globo.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/glomex.py
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gmanetwork.py
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/go.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/godtube.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gofile.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/golem.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/goodgame.py
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/googledrive.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/googlepodcasts.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/googlesearch.py
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/goplay.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gopro.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/goshgay.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gotostage.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gputechconf.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gronkh.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/groupon.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/harpodeon.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hbo.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hearthisat.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/heise.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hellporno.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hgtv.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hidive.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/historicfilms.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hitrecord.py
--rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hketv.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hollywoodreporter.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/holodex.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hotnewhiphop.py
--rw-r--r--   0        0        0    18185 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hotstar.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hrefli.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hrfensehen.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hrti.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hse.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/huajiao.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/huffpost.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hungama.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/huya.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hypem.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hypergryph.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hytale.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/icareus.py
--rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ichinanalive.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/idolplus.py
--rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ign.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iheart.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ilpost.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iltalehti.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/imdb.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/imggaming.py
--rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/imgur.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ina.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/inc.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/indavideo.py
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/infoq.py
--rw-r--r--   0        0        0    30961 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/instagram.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/internazionale.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/internetvideoarchive.py
--rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iprima.py
--rw-r--r--   0        0        0    31244 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iqiyi.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/islamchannel.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/israelnationalnews.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/itprotv.py
--rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/itv.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ivi.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ivideon.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iwara.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ixigua.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/izlesene.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jable.py
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jamendo.py
--rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/japandiet.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jeuxvideo.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jiosaavn.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jixie.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/joj.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/joqrag.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jove.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jstream.py
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jtbc.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jwplatform.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kakao.py
--rw-r--r--   0        0        0    24329 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kaltura.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kankanews.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/karaoketv.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kelbyone.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/khanacademy.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kick.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kicker.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kickstarter.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kinja.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kinopoisk.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kommunetv.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kompas.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/koo.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/krasview.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kth.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ku6.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kukululive.py
--rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kuwo.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/la7.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lastfm.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/laxarxames.py
--rw-r--r--   0        0        0   772452 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lazy_extractors.py
--rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lbry.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lci.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lcp.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lecture2go.py
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lecturio.py
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/leeco.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lefigaro.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lego.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lemonde.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lenta.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/libraryofcongress.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/libsyn.py
--rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lifenews.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/likee.py
--rw-r--r--   0        0        0    15006 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/limelight.py
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/linkedin.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/liputan6.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/listennotes.py
--rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/litv.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/livejournal.py
--rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/livestream.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/livestreamfails.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lnkgo.py
--rw-r--r--   0        0        0    18063 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/loom.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lovehomeporn.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lrt.py
--rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lsm.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lumni.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lynda.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/maariv.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/magellantv.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/magentamusik.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mailru.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mainstreaming.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mangomolo.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/manoto.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/manyvids.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/maoritv.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/markiza.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/massengeschmacktv.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/masters.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/matchtv.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mbn.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mdr.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/medaltv.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaite.py
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaklikk.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/medialaan.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaset.py
--rw-r--r--   0        0        0    16617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediasite.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediastream.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaworksnz.py
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/medici.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/megaphone.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/megatvcom.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/meipai.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/melonvod.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/metacritic.py
--rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mgtv.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/microsoftembed.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/microsoftstream.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/microsoftvirtualacademy.py
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mildom.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/minds.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/minoto.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mirrativ.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mirrorcouk.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mit.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mitele.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mixch.py
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mixcloud.py
--rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mlb.py
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mlssoccer.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mocha.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mojvideo.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/monstercat.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/motherless.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/motorsport.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/moviepilot.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/moview.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/moviezine.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/movingimage.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/msn.py
--rw-r--r--   0        0        0    25584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mtv.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/muenchentv.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/murrtube.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/museai.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/musescore.py
--rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/musicdex.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mx3.py
--rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mxplayer.py
--rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myspace.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myspass.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myvideoge.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myvidster.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mzaalo.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/n1.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nate.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nationalgeographic.py
--rw-r--r--   0        0        0    16447 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/naver.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nba.py
--rw-r--r--   0        0        0    35311 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nbc.py
--rw-r--r--   0        0        0    18232 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ndr.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ndtv.py
--rw-r--r--   0        0        0    20864 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nebula.py
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nekohacker.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nerdcubed.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/neteasemusic.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/netverse.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/netzkino.py
--rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/newgrounds.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/newspicks.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/newsy.py
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nextmedia.py
--rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nexx.py
--rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nfb.py
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nfhsnetwork.py
--rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nfl.py
--rw-r--r--   0        0        0    34642 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nhk.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nhl.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nick.py
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/niconico.py
--rw-r--r--   0        0        0    18094 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/niconicochannelplus.py
--rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninaprotocol.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninecninemedia.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninegag.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninenews.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninenow.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nintendo.py
--rw-r--r--   0        0        0    13650 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nitter.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nobelprize.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noice.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nonktube.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noodlemagazine.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noovo.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nosnl.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nova.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/novaplay.py
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nowness.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noz.py
--rw-r--r--   0        0        0    22320 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/npo.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/npr.py
--rw-r--r--   0        0        0    32207 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nrk.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nrl.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ntvcojp.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ntvde.py
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ntvru.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nubilesporn.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nuevo.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nuum.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nuvid.py
--rw-r--r--   0        0        0    17309 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nytimes.py
--rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nzherald.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nzonscreen.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nzz.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/odkmedia.py
--rw-r--r--   0        0        0    17342 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/odnoklassniki.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/oftv.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/oktoberfesttv.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/olympics.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/on24.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/once.py
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ondemandkorea.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onefootball.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onenewsnz.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/oneplace.py
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onet.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onionstudios.py
--rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/opencast.py
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/openload.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/openrec.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ora.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/orf.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/outsidetv.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/owncloud.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/packtpub.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/palcomp3.py
--rw-r--r--   0        0        0    25808 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/panopto.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/paramountplus.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/parler.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/parlview.py
--rw-r--r--   0        0        0    22805 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/patreon.py
--rw-r--r--   0        0        0    38530 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pbs.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pearvideo.py
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peekvids.py
--rw-r--r--   0        0        0    78541 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peertube.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peertv.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peloton.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/performgroup.py
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/periscope.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pgatour.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/philharmoniedeparis.py
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/phoenix.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/photobucket.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/piapro.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/piaulizaportal.py
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/picarto.py
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/piksel.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pinkbike.py
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pinterest.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pixivsketch.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pladform.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/planetmarathi.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/platzi.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playplustv.py
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playsuisse.py
--rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playtvak.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playwire.py
--rw-r--r--   0        0        0    18375 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pluralsight.py
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/plutotv.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/podbayfm.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/podchaser.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/podomatic.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pokemon.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pokergo.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/polsatgo.py
--rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/polskieradio.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/popcorntimes.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/popcorntv.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/porn91.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornbox.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornflip.py
--rw-r--r--   0        0        0    31546 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornhub.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornotube.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornovoisines.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornoxo.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pr0gramm.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/prankcast.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/premiershiprugby.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/presstv.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/projectveritas.py
--rw-r--r--   0        0        0    21515 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/prosiebensat1.py
--rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/prx.py
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/puhutv.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/puls4.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pyvideo.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/qdance.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/qingting.py
--rw-r--r--   0        0        0    13550 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/qqmusic.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/r7.py
--rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiko.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiocanada.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiocomercial.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiode.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiofrance.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiojavan.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiokapital.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiozet.py
--rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radlive.py
--rw-r--r--   0        0        0    34159 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rai.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/raywenderlich.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rbgtum.py
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rcs.py
--rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rcti.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rds.py
--rw-r--r--   0        0        0    14580 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redbee.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redbulltv.py
--rw-r--r--   0        0        0    14147 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/reddit.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redge.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redgifs.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redtube.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rentv.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/restudy.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/reuters.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/reverbnation.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rheinmaintv.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ridehome.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rinsefm.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rmcdecouverte.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rockstargames.py
--rw-r--r--   0        0        0    21043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rokfin.py
--rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/roosterteeth.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rottentomatoes.py
--rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rozhlas.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rte.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtl2.py
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtlnl.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtnews.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtp.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtrfm.py
--rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rts.py
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtvcplay.py
--rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtve.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtvs.py
--rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtvslo.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rudovideo.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rule34video.py
--rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rumble.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rutube.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rutv.py
--rw-r--r--   0        0        0    10968 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ruutu.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ruv.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/s4c.py
--rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/safari.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/saitosan.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/samplefocus.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sapo.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sbs.py
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sbscokr.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screen9.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screencast.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screencastify.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screencastomatic.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/scrippsnetworks.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/scrolller.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/scte.py
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sejmpl.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/senalcolombia.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/senategov.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sendtonews.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/servus.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sevenplus.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sexu.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/seznamzpravy.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/shahid.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sharepoint.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sharevideos.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/shemaroome.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/showroomlive.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sibnet.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/simplecast.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sina.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sixplay.py
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skeb.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sky.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skyit.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skylinewebcams.py
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skynewsarabia.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skynewsau.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/slideshare.py
--rw-r--r--   0        0        0    21906 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/slideslive.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/slutload.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/smotrim.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/snotr.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sohu.py
--rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sonyliv.py
--rw-r--r--   0        0        0    38941 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/soundcloud.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/soundgasm.py
--rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/southpark.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sovietscloset.py
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spankbang.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spiegel.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spike.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sport5.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sportbox.py
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sportdeutschland.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spotify.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spreaker.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/springboardplatform.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sprout.py
--rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/srgssr.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/srmediathek.py
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stacommu.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stageplus.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stanfordoc.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/startrek.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/startv.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/steam.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stitcher.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/storyfire.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/streamable.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/streamcz.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/streetvoice.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stretchinternet.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stripchat.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stv.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/substack.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sunporno.py
--rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sverigesradio.py
--rw-r--r--   0        0        0    17835 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/svt.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/swearnet.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/syfy.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/syvdk.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sztvhu.py
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tagesschau.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tass.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tbs.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tbsjp.py
--rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teachable.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teachertube.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teachingchannel.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teamcoco.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teamtreehouse.py
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ted.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tele13.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tele5.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telebruxelles.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telecaribe.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telecinco.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telegraaf.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telegram.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telemb.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telemundo.py
--rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telequebec.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teletask.py
--rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telewebion.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tempo.py
--rw-r--r--   0        0        0    19941 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tencent.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tennistv.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tenplay.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/testurl.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tf1.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tfo.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theguardian.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theholetv.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theintercept.py
--rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theplatform.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thestar.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thesun.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theweatherchannel.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thisamericanlife.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thisoldhouse.py
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thisvid.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/threeqsdn.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/threespeak.py
--rw-r--r--   0        0        0    60555 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tiktok.py
--rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tmz.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tnaflix.py
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toggle.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toggo.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tonline.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toongoggles.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toutv.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toypics.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/traileraddict.py
--rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/triller.py
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trovo.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trtcocuk.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trtworld.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trueid.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trunews.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/truth.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trutv.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tube8.py
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tubetugraz.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tubitv.py
--rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tumblr.py
--rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tunein.py
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/turner.py
--rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv2.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv24ua.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv2dk.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv2hu.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv4.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv5mondeplus.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv5unis.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tva.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvanouvelles.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvc.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tver.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvigle.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tviplayer.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvland.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvn24.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvnoe.py
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvopengr.py
--rw-r--r--   0        0        0    25539 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvp.py
--rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvplay.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvplayer.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tweakers.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twentymin.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twentythreevideo.py
--rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twitcasting.py
--rw-r--r--   0        0        0    42809 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twitch.py
--rw-r--r--   0        0        0    81104 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twitter.py
--rw-r--r--   0        0        0    17683 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/txxx.py
--rw-r--r--   0        0        0    19475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/udemy.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/udn.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ufctv.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ukcolumn.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/uktvplay.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/umg.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/unistra.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/unity.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/unsupported.py
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/uol.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/uplynk.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/urort.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/urplay.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/usanetwork.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/usatoday.py
--rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ustream.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ustudio.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/utreon.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/varzesh3.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vbox7.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/veo.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/veoh.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vesti.py
--rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vevo.py
--rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vgtv.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vh1.py
--rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vice.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viddler.py
--rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videa.py
--rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videocampus_sachsen.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videodetective.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videofyme.py
--rw-r--r--   0        0        0    13772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videoken.py
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videomore.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videopress.py
--rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vidio.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vidlii.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vidly.py
--rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viewlift.py
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viidea.py
--rw-r--r--   0        0        0    13492 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viki.py
--rw-r--r--   0        0        0    62548 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vimeo.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vimm.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vine.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viously.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viqeo.py
--rw-r--r--   0        0        0    21227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viu.py
--rw-r--r--   0        0        0    34047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vk.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vocaroo.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vodpl.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vodplatform.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/voicy.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/volejtv.py
--rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/voot.py
--rw-r--r--   0        0        0     9519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/voxmedia.py
--rw-r--r--   0        0        0    21514 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vrt.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vtm.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vuclip.py
--rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vvvvid.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/walla.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/washingtonpost.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wat.py
--rw-r--r--   0        0        0    15111 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wdr.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/webcamerapl.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/webcaster.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/webofstories.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weibo.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weiqitv.py
--rw-r--r--   0        0        0    25606 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weverse.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wevidi.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weyyak.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/whowatch.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/whyp.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wikimedia.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wimbledon.py
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wimtv.py
--rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wistia.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wordpress.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/worldstarhiphop.py
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wppilot.py
--rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wrestleuniverse.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wsj.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wwe.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wykop.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xanimu.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xboxclips.py
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xfileshare.py
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xhamster.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ximalaya.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xinpianchang.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xminus.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xnxx.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xstream.py
--rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xvideos.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xxxymovies.py
--rw-r--r--   0        0        0    17965 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yahoo.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yandexdisk.py
--rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yandexmusic.py
--rw-r--r--   0        0        0    17747 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yandexvideo.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yapfiles.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yappy.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yle_areena.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youjizz.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youku.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/younow.py
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youporn.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yourporn.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yourupload.py
--rw-r--r--   0        0        0   348531 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youtube.py
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zaiko.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zapiks.py
--rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zattoo.py
--rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zdf.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zee5.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zeenews.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zenporn.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zetland.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zhihu.py
--rw-r--r--   0        0        0    23571 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zingmp3.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zoom.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zype.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/__init__.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_curlcffi.py
--rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_helper.py
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_requests.py
--rw-r--r--   0        0        0    15738 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_urllib.py
--rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_websockets.py
--rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/common.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/exceptions.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/impersonate.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/websocket.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/__init__.py
--rw-r--r--   0        0        0     8359 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/common.py
--rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/embedthumbnail.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/exec.py
--rw-r--r--   0        0        0    49509 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/ffmpeg.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/metadataparser.py
--rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/modify_chapters.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/movefilesafterdownload.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/sponskrub.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/sponsorblock.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/xattrpp.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/_deprecated.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/_legacy.py
--rw-r--r--   0        0        0   184010 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/_utils.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/networking.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/progress.py
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/traversal.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/.gitignore
--rw-r--r--   0        0        0    17298 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/AUTHORS
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/LICENSE
--rw-r--r--   0        0        0   162031 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/README.md
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/pyproject.toml
--rw-r--r--   0        0        0   166156 2020-02-02 00:00:00.000000 yt_dlp-2024.5.5.232701.dev0/PKG-INFO
+-rw-r--r--   0        0        0   430539 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/Changelog.md
+-rw-r--r--   0        0        0   149757 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/README.txt
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/setup.cfg
+-rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/supportedsites.md
+-rw-r--r--   0        0        0   146693 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt-dlp.1
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/completions/bash/yt-dlp
+-rw-r--r--   0        0        0    50227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/completions/fish/yt-dlp.fish
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/completions/zsh/_yt-dlp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/__init__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/bash-completion.in
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/bash-completion.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/changelog_override.json
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/changelog_override.schema.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/check-porn.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/cli_to_api.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/fish-completion.in
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/fish-completion.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/generate_aes_testdata.py
+-rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/install_deps.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/lazy_load_template.py
+-rw-r--r--   0        0        0    41043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/logo.ico
+-rw-r--r--   0        0        0    18382 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/make_changelog.py
+-rwxr-xr-x   0        0        0      763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/make_contributing.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/make_issue_template.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/make_lazy_extractors.py
+-rwxr-xr-x   0        0        0     2892 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/make_readme.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/make_supportedsites.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/prepare_manpage.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/run_tests.bat
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/run_tests.py
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/run_tests.sh
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/set-variant.py
+-rwxr-xr-x   0        0        0     4849 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/tomlparse.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/update-version.py
+-rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/update_changelog.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/zsh-completion.in
+-rwxr-xr-x   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/devscripts/zsh-completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/conftest.py
+-rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/helper.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/parameters.json
+-rw-r--r--   0        0        0   100697 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_InfoExtractor.py
+-rw-r--r--   0        0        0    57080 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_YoutubeDL.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_YoutubeDLCookieJar.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_aes.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_age_restriction.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_all_urls.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_cache.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_compat.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_config.py
+-rw-r--r--   0        0        0    13665 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_cookies.py
+-rwxr-xr-x   0        0        0    12247 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_download.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_downloader_external.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_downloader_http.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_execution.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_iqiyi_sdk_interpreter.py
+-rw-r--r--   0        0        0    18408 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_jsinterp.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_netrc.py
+-rw-r--r--   0        0        0    87519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_networking.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_networking_utils.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_overwrites.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_plugins.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_post_hooks.py
+-rw-r--r--   0        0        0    30542 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_postprocessors.py
+-rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_socks.py
+-rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_subtitles.py
+-rw-r--r--   0        0        0    24268 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_traversal.py
+-rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_update.py
+-rw-r--r--   0        0        0    97858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_utils.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_verbose_output.py
+-rw-r--r--   0        0        0    16532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_websockets.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_write_annotations.py.disabled
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_youtube_lists.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_youtube_misc.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/test_youtube_signature.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testcert.pem
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/ca.crt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/ca.key
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/ca.srl
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/client.crt
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/client.csr
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/client.key
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/clientencrypted.key
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/clientwithencryptedkey.crt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/clientwithkey.crt
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/instructions.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/cookies/httponly_cookies.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/cookies/malformed_cookies.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/cookies/session_cookies.txt
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/f4m/custom_base_url.f4m
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/ism/ec-3_test.Manifest
+-rw-r--r--   0        0        0    23179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/ism/sintel.Manifest
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/m3u8/bipbop_16x9.m3u8
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/float_duration.mpd
+-rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/subtitles.mpd
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/unfragmented.mpd
+-rw-r--r--   0        0        0    22374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/urls_only.mpd
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/xspf/foo_xspf.xspf
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/yt_dlp_plugins/extractor/_ignore.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/yt_dlp_plugins/extractor/ignore.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/yt_dlp_plugins/extractor/normal.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/yt_dlp_plugins/postprocessor/normal.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/zipped.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/zipped.py
+-rw-r--r--   0        0        0   211705 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/YoutubeDL.py
+-rw-r--r--   0        0        0    47722 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/__main__.py
+-rw-r--r--   0        0        0    22402 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/aes.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/cache.py
+-rw-r--r--   0        0        0    54844 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/cookies.py
+-rw-r--r--   0        0        0    34646 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/jsinterp.py
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/minicurses.py
+-rw-r--r--   0        0        0    96731 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/options.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/plugins.py
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/socks.py
+-rw-r--r--   0        0        0    25165 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/update.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/version.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/webvtt.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/_deprecated.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/_legacy.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/compat_utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/functools.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/imghdr.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/shutil.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/types.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/urllib/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/urllib/request.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/dependencies/Cryptodome.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/dependencies/__init__.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/__init__.py
+-rw-r--r--   0        0        0    19691 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/common.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/dash.py
+-rw-r--r--   0        0        0    28090 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/external.py
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/f4m.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/fc2.py
+-rw-r--r--   0        0        0    21795 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/fragment.py
+-rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/hls.py
+-rw-r--r--   0        0        0    16863 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/http.py
+-rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/ism.py
+-rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/mhtml.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/niconico.py
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/rtmp.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/rtsp.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/websocket.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/youtube_live_chat.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/__init__.py
+-rw-r--r--   0        0        0    52880 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/_extractors.py
+-rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abc.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abcnews.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abcotvs.py
+-rw-r--r--   0        0        0    19939 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abematv.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/academicearth.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/acast.py
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/acfun.py
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adn.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adobeconnect.py
+-rw-r--r--   0        0        0    52679 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adobepass.py
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adobetv.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adultswim.py
+-rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aenetworks.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aeonco.py
+-rw-r--r--   0        0        0    17843 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/afreecatv.py
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/agora.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/airtv.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aitube.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aliexpress.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aljazeera.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/allocine.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/allstar.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/alphaporno.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/alsace20tv.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/altcensored.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/alura.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amadeustv.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amara.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amazon.py
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amazonminitv.py
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amcnetworks.py
+-rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/americastestkitchen.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amp.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/anchorfm.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/angel.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/antenna.py
+-rw-r--r--   0        0        0    26757 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/anvato.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aol.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/apa.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aparat.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/appleconnect.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/applepodcasts.py
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/appletrailers.py
+-rw-r--r--   0        0        0    46353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/archiveorg.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arcpublishing.py
+-rw-r--r--   0        0        0    26748 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ard.py
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arkena.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arnes.py
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/art19.py
+-rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arte.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/asobichannel.py
+-rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/asobistage.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/atresplayer.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/atscaleconf.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/atvat.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audimedia.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audioboom.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audiodraft.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audiomack.py
+-rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audius.py
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/awaan.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aws.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/axs.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/azmedien.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/baidu.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/banbye.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bandaichannel.py
+-rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bandcamp.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bannedvideo.py
+-rw-r--r--   0        0        0    72720 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bbc.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/beatbump.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/beatport.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/beeg.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/behindkink.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bellmedia.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/berufetv.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bet.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bfi.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bfmtv.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bibeltv.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bigflix.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bigo.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bild.py
+-rw-r--r--   0        0        0    94037 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bilibili.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/biobiochiletv.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bitchute.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/blackboardcollaborate.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bleacherreport.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/blerp.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/blogger.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bloomberg.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bokecc.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bongacams.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/boosty.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bostonglobe.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/box.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/boxcast.py
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bpb.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/br.py
+-rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/brainpop.py
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bravotv.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/breitbart.py
+-rw-r--r--   0        0        0    42705 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/brightcove.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/brilliantpala.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bundesliga.py
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bundestag.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/businessinsider.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/buzzfeed.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/byutv.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/c56.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cableav.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/callin.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/caltrans.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cam4.py
+-rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camdemy.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camfm.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cammodels.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camsoda.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camtasia.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canal1.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canalalpha.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canalc2.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canalplus.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/caracoltv.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cartoonnetwork.py
+-rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbc.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbs.py
+-rw-r--r--   0        0        0    19544 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbsnews.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbssports.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ccc.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ccma.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cctv.py
+-rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cda.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cellebrite.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ceskatelevize.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cgtn.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/charlierose.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/chaturbate.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/chilloutzone.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/chzzk.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cinemax.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cinetecamilano.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cineverse.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ciscolive.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ciscowebex.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cjsw.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clipchamp.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clippit.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cliprs.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/closertotruth.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cloudflarestream.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cloudycdn.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clubic.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clyp.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cmt.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cnbc.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cnn.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/comedycentral.py
+-rw-r--r--   0        0        0   192152 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/common.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/commonmistakes.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/commonprotocols.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/condenast.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/contv.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/corus.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/coub.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cozytv.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cpac.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cracked.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crackle.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/craftsy.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crooksandliars.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crowdbunker.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crtvg.py
+-rw-r--r--   0        0        0    29342 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crunchyroll.py
+-rw-r--r--   0        0        0    12105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cspan.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ctsnews.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ctv.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ctvnews.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cultureunplugged.py
+-rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/curiositystream.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cwtv.py
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cybrary.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dacast.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dailymail.py
+-rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dailymotion.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dailywire.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/damtomo.py
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/daum.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/daystar.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dbtv.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dctp.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/deezer.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/democracynow.py
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/detik.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/deuxm.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dfb.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dhm.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/digitalconcerthall.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/digiteka.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/discogs.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/discovery.py
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/discoverygo.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/disney.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dispeak.py
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dlf.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dlive.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/douyutv.py
+-rw-r--r--   0        0        0    41198 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dplay.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drbonanza.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dreisat.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drooble.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dropbox.py
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dropout.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drtuber.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drtv.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dtube.py
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/duboku.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dumpert.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/duoplay.py
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dvtv.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dw.py
+-rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eagleplatform.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ebaumsworld.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ebay.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/egghead.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eighttracks.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/einthusan.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eitb.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/elementorembed.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/elonet.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/elpais.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eltrecetv.py
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/embedly.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/epicon.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/epidemicsound.py
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eplus.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/epoch.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eporner.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/erocast.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eroprofile.py
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/err.py
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ertgr.py
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/espn.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ettutv.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/europa.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/europeantour.py
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eurosport.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/euscreen.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/expressen.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/extractors.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eyedotv.py
+-rw-r--r--   0        0        0    48415 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/facebook.py
+-rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fancode.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fathom.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/faz.py
+-rw-r--r--   0        0        0    10584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fc2.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fczenit.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fifa.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/filmon.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/filmweb.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/firsttv.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fivetv.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/flextv.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/flickr.py
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/floatplane.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/folketinget.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/footyroom.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/formula1.py
+-rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fourtube.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fox.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fox9.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/foxnews.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/foxsports.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fptplay.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/franceinter.py
+-rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/francetv.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/freesound.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/freespeech.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/freetv.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/frontendmasters.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fujitv.py
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/funimation.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/funk.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/funker530.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fuyintv.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gab.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gaia.py
+-rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gamejolt.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gamespot.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gamestar.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gaskrank.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gazeta.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gdcvault.py
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gedidigital.py
+-rw-r--r--   0        0        0   119486 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/generic.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/genericembeds.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/genius.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/getcourseru.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gettr.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/giantbomb.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gigya.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/glide.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/globalplayer.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/globo.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/glomex.py
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gmanetwork.py
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/go.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/godtube.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gofile.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/golem.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/goodgame.py
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/googledrive.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/googlepodcasts.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/googlesearch.py
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/goplay.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gopro.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/goshgay.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gotostage.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gputechconf.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gronkh.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/groupon.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/harpodeon.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hbo.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hearthisat.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/heise.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hellporno.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hgtv.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hidive.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/historicfilms.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hitrecord.py
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hketv.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hollywoodreporter.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/holodex.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hotnewhiphop.py
+-rw-r--r--   0        0        0    18185 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hotstar.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hrefli.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hrfensehen.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hrti.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hse.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/huajiao.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/huffpost.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hungama.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/huya.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hypem.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hypergryph.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hytale.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/icareus.py
+-rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ichinanalive.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/idolplus.py
+-rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ign.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iheart.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ilpost.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iltalehti.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/imdb.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/imggaming.py
+-rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/imgur.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ina.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/inc.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/indavideo.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/infoq.py
+-rw-r--r--   0        0        0    30961 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/instagram.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/internazionale.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/internetvideoarchive.py
+-rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iprima.py
+-rw-r--r--   0        0        0    31244 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iqiyi.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/islamchannel.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/israelnationalnews.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/itprotv.py
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/itv.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ivi.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ivideon.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iwara.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ixigua.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/izlesene.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jable.py
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jamendo.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/japandiet.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jeuxvideo.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jiosaavn.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jixie.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/joj.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/joqrag.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jove.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jstream.py
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jtbc.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jwplatform.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kakao.py
+-rw-r--r--   0        0        0    24329 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kaltura.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kankanews.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/karaoketv.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kelbyone.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/khanacademy.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kick.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kicker.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kickstarter.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kinja.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kinopoisk.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kommunetv.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kompas.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/koo.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/krasview.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kth.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ku6.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kukululive.py
+-rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kuwo.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/la7.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lastfm.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/laxarxames.py
+-rw-r--r--   0        0        0   772452 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lazy_extractors.py
+-rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lbry.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lci.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lcp.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lecture2go.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lecturio.py
+-rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/leeco.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lefigaro.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lego.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lemonde.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lenta.py
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/libraryofcongress.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/libsyn.py
+-rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lifenews.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/likee.py
+-rw-r--r--   0        0        0    15006 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/limelight.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/linkedin.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/liputan6.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/listennotes.py
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/litv.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/livejournal.py
+-rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/livestream.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/livestreamfails.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lnkgo.py
+-rw-r--r--   0        0        0    18063 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/loom.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lovehomeporn.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lrt.py
+-rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lsm.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lumni.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lynda.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/maariv.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/magellantv.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/magentamusik.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mailru.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mainstreaming.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mangomolo.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/manoto.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/manyvids.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/maoritv.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/markiza.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/massengeschmacktv.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/masters.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/matchtv.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mbn.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mdr.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/medaltv.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaite.py
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaklikk.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/medialaan.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaset.py
+-rw-r--r--   0        0        0    16617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediasite.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediastream.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaworksnz.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/medici.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/megaphone.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/megatvcom.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/meipai.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/melonvod.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/metacritic.py
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mgtv.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/microsoftembed.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/microsoftstream.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/microsoftvirtualacademy.py
+-rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mildom.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/minds.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/minoto.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mirrativ.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mirrorcouk.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mit.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mitele.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mixch.py
+-rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mixcloud.py
+-rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mlb.py
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mlssoccer.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mocha.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mojvideo.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/monstercat.py
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/motherless.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/motorsport.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/moviepilot.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/moview.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/moviezine.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/movingimage.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/msn.py
+-rw-r--r--   0        0        0    25584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mtv.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/muenchentv.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/murrtube.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/museai.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/musescore.py
+-rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/musicdex.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mx3.py
+-rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mxplayer.py
+-rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myspace.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myspass.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myvideoge.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myvidster.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mzaalo.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/n1.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nate.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nationalgeographic.py
+-rw-r--r--   0        0        0    16447 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/naver.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nba.py
+-rw-r--r--   0        0        0    35311 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nbc.py
+-rw-r--r--   0        0        0    18232 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ndr.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ndtv.py
+-rw-r--r--   0        0        0    20864 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nebula.py
+-rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nekohacker.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nerdcubed.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/neteasemusic.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/netverse.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/netzkino.py
+-rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/newgrounds.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/newspicks.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/newsy.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nextmedia.py
+-rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nexx.py
+-rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nfb.py
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nfhsnetwork.py
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nfl.py
+-rw-r--r--   0        0        0    34642 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nhk.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nhl.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nick.py
+-rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/niconico.py
+-rw-r--r--   0        0        0    18094 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/niconicochannelplus.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninaprotocol.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninecninemedia.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninegag.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninenews.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninenow.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nintendo.py
+-rw-r--r--   0        0        0    13650 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nitter.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nobelprize.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noice.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nonktube.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noodlemagazine.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noovo.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nosnl.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nova.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/novaplay.py
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nowness.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noz.py
+-rw-r--r--   0        0        0    22320 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/npo.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/npr.py
+-rw-r--r--   0        0        0    32207 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nrk.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nrl.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ntvcojp.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ntvde.py
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ntvru.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nubilesporn.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nuevo.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nuum.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nuvid.py
+-rw-r--r--   0        0        0    17309 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nytimes.py
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nzherald.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nzonscreen.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nzz.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/odkmedia.py
+-rw-r--r--   0        0        0    17342 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/odnoklassniki.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/oftv.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/oktoberfesttv.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/olympics.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/on24.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/once.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ondemandkorea.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onefootball.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onenewsnz.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/oneplace.py
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onet.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onionstudios.py
+-rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/opencast.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/openload.py
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/openrec.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ora.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/orf.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/outsidetv.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/owncloud.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/packtpub.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/palcomp3.py
+-rw-r--r--   0        0        0    25808 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/panopto.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/paramountplus.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/parler.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/parlview.py
+-rw-r--r--   0        0        0    22805 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/patreon.py
+-rw-r--r--   0        0        0    38530 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pbs.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pearvideo.py
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peekvids.py
+-rw-r--r--   0        0        0    78541 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peertube.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peertv.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peloton.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/performgroup.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/periscope.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pgatour.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/philharmoniedeparis.py
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/phoenix.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/photobucket.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/piapro.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/piaulizaportal.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/picarto.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/piksel.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pinkbike.py
+-rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pinterest.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pixivsketch.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pladform.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/planetmarathi.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/platzi.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playplustv.py
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playsuisse.py
+-rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playtvak.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playwire.py
+-rw-r--r--   0        0        0    18375 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pluralsight.py
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/plutotv.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/podbayfm.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/podchaser.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/podomatic.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pokemon.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pokergo.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/polsatgo.py
+-rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/polskieradio.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/popcorntimes.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/popcorntv.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/porn91.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornbox.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornflip.py
+-rw-r--r--   0        0        0    31546 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornhub.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornotube.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornovoisines.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornoxo.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pr0gramm.py
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/prankcast.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/premiershiprugby.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/presstv.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/projectveritas.py
+-rw-r--r--   0        0        0    21515 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/prosiebensat1.py
+-rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/prx.py
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/puhutv.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/puls4.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pyvideo.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/qdance.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/qingting.py
+-rw-r--r--   0        0        0    13550 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/qqmusic.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/r7.py
+-rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiko.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiocanada.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiocomercial.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiode.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiofrance.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiojavan.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiokapital.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiozet.py
+-rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radlive.py
+-rw-r--r--   0        0        0    34159 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rai.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/raywenderlich.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rbgtum.py
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rcs.py
+-rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rcti.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rds.py
+-rw-r--r--   0        0        0    14580 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redbee.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redbulltv.py
+-rw-r--r--   0        0        0    14147 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/reddit.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redge.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redgifs.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redtube.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rentv.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/restudy.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/reuters.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/reverbnation.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rheinmaintv.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ridehome.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rinsefm.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rmcdecouverte.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rockstargames.py
+-rw-r--r--   0        0        0    21043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rokfin.py
+-rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/roosterteeth.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rottentomatoes.py
+-rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rozhlas.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rte.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtl2.py
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtlnl.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtnews.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtp.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtrfm.py
+-rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rts.py
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtvcplay.py
+-rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtve.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtvs.py
+-rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtvslo.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rudovideo.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rule34video.py
+-rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rumble.py
+-rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rutube.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rutv.py
+-rw-r--r--   0        0        0    10968 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ruutu.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ruv.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/s4c.py
+-rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/safari.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/saitosan.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/samplefocus.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sapo.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sbs.py
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sbscokr.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screen9.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screencast.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screencastify.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screencastomatic.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/scrippsnetworks.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/scrolller.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/scte.py
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sejmpl.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/senalcolombia.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/senategov.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sendtonews.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/servus.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sevenplus.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sexu.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/seznamzpravy.py
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/shahid.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sharepoint.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sharevideos.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/shemaroome.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/showroomlive.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sibnet.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/simplecast.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sina.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sixplay.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skeb.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sky.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skyit.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skylinewebcams.py
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skynewsarabia.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skynewsau.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/slideshare.py
+-rw-r--r--   0        0        0    21906 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/slideslive.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/slutload.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/smotrim.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/snotr.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sohu.py
+-rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sonyliv.py
+-rw-r--r--   0        0        0    38941 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/soundcloud.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/soundgasm.py
+-rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/southpark.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sovietscloset.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spankbang.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spiegel.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spike.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sport5.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sportbox.py
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sportdeutschland.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spotify.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spreaker.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/springboardplatform.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sprout.py
+-rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/srgssr.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/srmediathek.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stacommu.py
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stageplus.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stanfordoc.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/startrek.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/startv.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/steam.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stitcher.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/storyfire.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/streamable.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/streamcz.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/streetvoice.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stretchinternet.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stripchat.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stv.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/substack.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sunporno.py
+-rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sverigesradio.py
+-rw-r--r--   0        0        0    17835 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/svt.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/swearnet.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/syfy.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/syvdk.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sztvhu.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tagesschau.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tass.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tbs.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tbsjp.py
+-rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teachable.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teachertube.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teachingchannel.py
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teamcoco.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teamtreehouse.py
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ted.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tele13.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tele5.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telebruxelles.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telecaribe.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telecinco.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telegraaf.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telegram.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telemb.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telemundo.py
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telequebec.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teletask.py
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telewebion.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tempo.py
+-rw-r--r--   0        0        0    19941 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tencent.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tennistv.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tenplay.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/testurl.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tf1.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tfo.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theguardian.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theholetv.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theintercept.py
+-rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theplatform.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thestar.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thesun.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theweatherchannel.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thisamericanlife.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thisoldhouse.py
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thisvid.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/threeqsdn.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/threespeak.py
+-rw-r--r--   0        0        0    60555 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tiktok.py
+-rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tmz.py
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tnaflix.py
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toggle.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toggo.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tonline.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toongoggles.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toutv.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toypics.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/traileraddict.py
+-rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/triller.py
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trovo.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trtcocuk.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trtworld.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trueid.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trunews.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/truth.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trutv.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tube8.py
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tubetugraz.py
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tubitv.py
+-rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tumblr.py
+-rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tunein.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/turner.py
+-rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv2.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv24ua.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv2dk.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv2hu.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv4.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv5mondeplus.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv5unis.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tva.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvanouvelles.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvc.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tver.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvigle.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tviplayer.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvland.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvn24.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvnoe.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvopengr.py
+-rw-r--r--   0        0        0    25539 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvp.py
+-rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvplay.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvplayer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tweakers.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twentymin.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twentythreevideo.py
+-rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twitcasting.py
+-rw-r--r--   0        0        0    42809 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twitch.py
+-rw-r--r--   0        0        0    81104 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twitter.py
+-rw-r--r--   0        0        0    17683 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/txxx.py
+-rw-r--r--   0        0        0    19475 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/udemy.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/udn.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ufctv.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ukcolumn.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/uktvplay.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/umg.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/unistra.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/unity.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/unsupported.py
+-rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/uol.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/uplynk.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/urort.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/urplay.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/usanetwork.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/usatoday.py
+-rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ustream.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ustudio.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/utreon.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/varzesh3.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vbox7.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/veo.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/veoh.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vesti.py
+-rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vevo.py
+-rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vgtv.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vh1.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vice.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viddler.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videa.py
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videocampus_sachsen.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videodetective.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videofyme.py
+-rw-r--r--   0        0        0    13772 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videoken.py
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videomore.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videopress.py
+-rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vidio.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vidlii.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vidly.py
+-rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viewlift.py
+-rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viidea.py
+-rw-r--r--   0        0        0    13492 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viki.py
+-rw-r--r--   0        0        0    62548 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vimeo.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vimm.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vine.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viously.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viqeo.py
+-rw-r--r--   0        0        0    21227 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viu.py
+-rw-r--r--   0        0        0    34579 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vk.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vocaroo.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vodpl.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vodplatform.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/voicy.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/volejtv.py
+-rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/voot.py
+-rw-r--r--   0        0        0     9519 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/voxmedia.py
+-rw-r--r--   0        0        0    21514 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vrt.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vtm.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vuclip.py
+-rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vvvvid.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/walla.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/washingtonpost.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wat.py
+-rw-r--r--   0        0        0    15111 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wdr.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/webcamerapl.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/webcaster.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/webofstories.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weibo.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weiqitv.py
+-rw-r--r--   0        0        0    25606 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weverse.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wevidi.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weyyak.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/whowatch.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/whyp.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wikimedia.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wimbledon.py
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wimtv.py
+-rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wistia.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wordpress.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/worldstarhiphop.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wppilot.py
+-rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wrestleuniverse.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wsj.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wwe.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wykop.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xanimu.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xboxclips.py
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xfileshare.py
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xhamster.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ximalaya.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xinpianchang.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xminus.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xnxx.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xstream.py
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xvideos.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xxxymovies.py
+-rw-r--r--   0        0        0    17965 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yahoo.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yandexdisk.py
+-rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yandexmusic.py
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yandexvideo.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yapfiles.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yappy.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yle_areena.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youjizz.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youku.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/younow.py
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youporn.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yourporn.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yourupload.py
+-rw-r--r--   0        0        0   348531 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youtube.py
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zaiko.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zapiks.py
+-rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zattoo.py
+-rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zdf.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zee5.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zeenews.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zenporn.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zetland.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zhihu.py
+-rw-r--r--   0        0        0    23571 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zingmp3.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zoom.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zype.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/__init__.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_curlcffi.py
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_helper.py
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_requests.py
+-rw-r--r--   0        0        0    15738 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_urllib.py
+-rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_websockets.py
+-rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/common.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/exceptions.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/impersonate.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/websocket.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/__init__.py
+-rw-r--r--   0        0        0     8359 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/common.py
+-rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/embedthumbnail.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/exec.py
+-rw-r--r--   0        0        0    49509 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/ffmpeg.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/metadataparser.py
+-rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/modify_chapters.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/movefilesafterdownload.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/sponskrub.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/sponsorblock.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/xattrpp.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/_deprecated.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/_legacy.py
+-rw-r--r--   0        0        0   184010 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/_utils.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/networking.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/progress.py
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/traversal.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/.gitignore
+-rw-r--r--   0        0        0    17312 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/AUTHORS
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/LICENSE
+-rw-r--r--   0        0        0   162031 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/README.md
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/pyproject.toml
+-rw-r--r--   0        0        0   166156 2020-02-02 00:00:00.000000 yt_dlp-2024.5.8.232715.dev0/PKG-INFO
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/Changelog.md` & `yt_dlp-2024.5.8.232715.dev0/Changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 # Changelog
 
 <!--
 # To create a release, dispatch the https://github.com/yt-dlp/yt-dlp/actions/workflows/release.yml workflow on master
 -->
 
-### 2024.05.05.232701
+### 2024.05.08.232715
 
 #### Core changes
 - [Warn if lack of ffmpeg alters format selection](https://github.com/yt-dlp/yt-dlp/commit/96da9525043f78aca4544d01761b13b2140e9ae6) ([#9805](https://github.com/yt-dlp/yt-dlp/issues/9805)) by [pukkandan](https://github.com/pukkandan), [seproDev](https://github.com/seproDev)
 - **windows**: [Improve shell quoting and tests](https://github.com/yt-dlp/yt-dlp/commit/64766459e37451b665c1464073c28361fbcf1c25) ([#9802](https://github.com/yt-dlp/yt-dlp/issues/9802)) by [Grub4K](https://github.com/Grub4K) (With fixes in [7e26bd5](https://github.com/yt-dlp/yt-dlp/commit/7e26bd53f9c5893518fde81dfd0079ec08dd841e))
 
 #### Extractor changes
 - [Make `_search_nextjs_data` non fatal](https://github.com/yt-dlp/yt-dlp/commit/3ee1194288981c4f2c4abd8315326de0c424d2ce) ([#8937](https://github.com/yt-dlp/yt-dlp/issues/8937)) by [Grub4K](https://github.com/Grub4K)
 - **afreecatv**: live: [Add `cdn` extractor-arg](https://github.com/yt-dlp/yt-dlp/commit/315b3544296bb83012e20ee3af9d3cbf5600dd1c) ([#9666](https://github.com/yt-dlp/yt-dlp/issues/9666)) by [bashonly](https://github.com/bashonly)
+- **bilibili**: [Fix `--geo-verification-proxy` support](https://github.com/yt-dlp/yt-dlp/commit/2338827072dacab0f15348b70aec8685feefc8d1) ([#9817](https://github.com/yt-dlp/yt-dlp/issues/9817)) by [fireattack](https://github.com/fireattack)
+- **bilibilispacevideo**: [Better error message](https://github.com/yt-dlp/yt-dlp/commit/06d52c87314e0bbc16c43c405090843885577b88) ([#9839](https://github.com/yt-dlp/yt-dlp/issues/9839)) by [fireattack](https://github.com/fireattack)
+- **boosty**: [Add cookies support](https://github.com/yt-dlp/yt-dlp/commit/145dc6f6563e80d2da1b3e9aea2ffa795b71622c) ([#9522](https://github.com/yt-dlp/yt-dlp/issues/9522)) by [RasmusAntons](https://github.com/RasmusAntons)
 - **cbc.ca**: player: [Improve `_VALID_URL`](https://github.com/yt-dlp/yt-dlp/commit/c8bf48f3a8fa29587e7c73ef5a7710385a5ea725) ([#9866](https://github.com/yt-dlp/yt-dlp/issues/9866)) by [carusocr](https://github.com/carusocr)
 - **crunchyroll**
     - [Always make metadata available](https://github.com/yt-dlp/yt-dlp/commit/cb2fb4a643949322adba561ca73bcba3221ec0c5) ([#9772](https://github.com/yt-dlp/yt-dlp/issues/9772)) by [bashonly](https://github.com/bashonly)
     - [Fix auth and remove cookies support](https://github.com/yt-dlp/yt-dlp/commit/ff38a011d57b763f3a69bebd25a5dc9044a717ce) ([#9749](https://github.com/yt-dlp/yt-dlp/issues/9749)) by [bashonly](https://github.com/bashonly)
     - [Support browser impersonation](https://github.com/yt-dlp/yt-dlp/commit/5904853ae5788509fdc4892cb7ecdfa9ae7f78e6) ([#9857](https://github.com/yt-dlp/yt-dlp/issues/9857)) by [bashonly](https://github.com/bashonly)
 - **facebook**: [Fix DASH formats extraction](https://github.com/yt-dlp/yt-dlp/commit/e3b42d8b1b8bcfff7ba146c19fc3f6f6ba843cea) ([#9734](https://github.com/yt-dlp/yt-dlp/issues/9734)) by [bashonly](https://github.com/bashonly)
 - **jiosaavn**: [Extract via API and fix playlists](https://github.com/yt-dlp/yt-dlp/commit/0c21c53885cf03f4040467ae8c44d7ff51016116) ([#9656](https://github.com/yt-dlp/yt-dlp/issues/9656)) by [bashonly](https://github.com/bashonly)
+- **mixch**: [Extract comments](https://github.com/yt-dlp/yt-dlp/commit/b38018b781b062d5169d104ab430489aef8e7f1e) ([#9860](https://github.com/yt-dlp/yt-dlp/issues/9860)) by [pzhlkj6612](https://github.com/pzhlkj6612)
 - **patreon**
     - [Extract multiple embeds](https://github.com/yt-dlp/yt-dlp/commit/036e0d92c6052465673d459678322ea03e61483d) ([#9850](https://github.com/yt-dlp/yt-dlp/issues/9850)) by [bashonly](https://github.com/bashonly)
     - [Fix Vimeo embed extraction](https://github.com/yt-dlp/yt-dlp/commit/c9ce57d9bf51541da2381d99bc096a9d0ddf1f27) ([#9712](https://github.com/yt-dlp/yt-dlp/issues/9712)) by [bashonly](https://github.com/bashonly)
+- **qub**: [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/6b54cccdcb892bca3e55993480d8b86f1c7e6da6) ([#7019](https://github.com/yt-dlp/yt-dlp/issues/7019)) by [alexhuot1](https://github.com/alexhuot1), [dirkf](https://github.com/dirkf)
 - **soundcloud**: [Extract `genres`](https://github.com/yt-dlp/yt-dlp/commit/231c2eacc41b06b65c63edf94c0d04768a5da607) ([#9821](https://github.com/yt-dlp/yt-dlp/issues/9821)) by [bashonly](https://github.com/bashonly)
 - **theatercomplextown**: [Fix extractors](https://github.com/yt-dlp/yt-dlp/commit/8056a3026ed6ec6a6d0ed56fdd7ebcd16e928341) ([#9754](https://github.com/yt-dlp/yt-dlp/issues/9754)) by [bashonly](https://github.com/bashonly)
+- **vk**: [Improve format extraction](https://github.com/yt-dlp/yt-dlp/commit/df5c9e733aaba703cf285c0372b6d61629330c82) ([#9885](https://github.com/yt-dlp/yt-dlp/issues/9885)) by [seproDev](https://github.com/seproDev)
 - **wrestleuniverse**: [Avoid partial stream formats](https://github.com/yt-dlp/yt-dlp/commit/c4853655cb9a793129280806af643de43c48f4d5) ([#9800](https://github.com/yt-dlp/yt-dlp/issues/9800)) by [bashonly](https://github.com/bashonly)
 - **youporn**: [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/351368cb9a6731b886a58f5a10fd6b302bbe47be) ([#8827](https://github.com/yt-dlp/yt-dlp/issues/8827)) by [The-MAGI](https://github.com/The-MAGI)
+- **zenyandex**: [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/c4b87dd885ee5391e5f481e7c8bd550a7c543623) ([#9813](https://github.com/yt-dlp/yt-dlp/issues/9813)) by [src-tinkerer](https://github.com/src-tinkerer)
 
 #### Networking changes
 - [Add `extensions` attribute to `Response`](https://github.com/yt-dlp/yt-dlp/commit/bec9a59e8ec82c18e3bf9268eaa436793dd52e35) ([#9756](https://github.com/yt-dlp/yt-dlp/issues/9756)) by [bashonly](https://github.com/bashonly)
 
 #### Misc. changes
 - **build**
     - [Migrate `linux_exe` to static musl builds](https://github.com/yt-dlp/yt-dlp/commit/ac817bc83efd939dca3e40c4b527d0ccfc77172b) ([#9811](https://github.com/yt-dlp/yt-dlp/issues/9811)) by [bashonly](https://github.com/bashonly), [Grub4K](https://github.com/Grub4K)
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/README.txt` & `yt_dlp-2024.5.8.232715.dev0/README.txt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/setup.cfg` & `yt_dlp-2024.5.8.232715.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/supportedsites.md` & `yt_dlp-2024.5.8.232715.dev0/supportedsites.md`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt-dlp.1` & `yt_dlp-2024.5.8.232715.dev0/yt-dlp.1`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/completions/bash/yt-dlp` & `yt_dlp-2024.5.8.232715.dev0/completions/bash/yt-dlp`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/completions/fish/yt-dlp.fish` & `yt_dlp-2024.5.8.232715.dev0/completions/fish/yt-dlp.fish`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/completions/zsh/_yt-dlp` & `yt_dlp-2024.5.8.232715.dev0/completions/zsh/_yt-dlp`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/bash-completion.in` & `yt_dlp-2024.5.8.232715.dev0/devscripts/bash-completion.in`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/bash-completion.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/bash-completion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/changelog_override.json` & `yt_dlp-2024.5.8.232715.dev0/devscripts/changelog_override.json`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/changelog_override.schema.json` & `yt_dlp-2024.5.8.232715.dev0/devscripts/changelog_override.schema.json`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/check-porn.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/check-porn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/cli_to_api.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/cli_to_api.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/fish-completion.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/fish-completion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/generate_aes_testdata.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/generate_aes_testdata.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/install_deps.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/install_deps.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/lazy_load_template.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/lazy_load_template.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/logo.ico` & `yt_dlp-2024.5.8.232715.dev0/devscripts/logo.ico`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/make_changelog.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/make_changelog.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/make_contributing.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/make_contributing.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/make_issue_template.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/make_issue_template.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/make_lazy_extractors.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/make_lazy_extractors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/make_readme.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/make_readme.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/prepare_manpage.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/prepare_manpage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/run_tests.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/set-variant.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/set-variant.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/tomlparse.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/tomlparse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/update-version.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/update-version.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/update_changelog.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/update_changelog.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/utils.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/zsh-completion.in` & `yt_dlp-2024.5.8.232715.dev0/devscripts/zsh-completion.in`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/devscripts/zsh-completion.py` & `yt_dlp-2024.5.8.232715.dev0/devscripts/zsh-completion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/conftest.py` & `yt_dlp-2024.5.8.232715.dev0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/helper.py` & `yt_dlp-2024.5.8.232715.dev0/test/helper.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/parameters.json` & `yt_dlp-2024.5.8.232715.dev0/test/parameters.json`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_InfoExtractor.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_InfoExtractor.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_YoutubeDL.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_YoutubeDL.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_YoutubeDLCookieJar.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_YoutubeDLCookieJar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_aes.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_aes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_age_restriction.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_age_restriction.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_all_urls.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_all_urls.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_cache.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_compat.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_compat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_config.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_cookies.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_cookies.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_download.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_download.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_downloader_external.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_downloader_external.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_downloader_http.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_downloader_http.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_execution.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_iqiyi_sdk_interpreter.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_iqiyi_sdk_interpreter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_jsinterp.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_jsinterp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_netrc.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_netrc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_networking.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_networking.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_networking_utils.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_networking_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_overwrites.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_overwrites.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_plugins.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_post_hooks.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_post_hooks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_postprocessors.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_postprocessors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_socks.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_socks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_subtitles.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_traversal.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_traversal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_update.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_update.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_utils.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_verbose_output.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_verbose_output.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_websockets.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_websockets.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_write_annotations.py.disabled` & `yt_dlp-2024.5.8.232715.dev0/test/test_write_annotations.py.disabled`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_youtube_lists.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_youtube_lists.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_youtube_misc.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_youtube_misc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/test_youtube_signature.py` & `yt_dlp-2024.5.8.232715.dev0/test/test_youtube_signature.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testcert.pem` & `yt_dlp-2024.5.8.232715.dev0/test/testcert.pem`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/ca.crt` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/ca.crt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/clientwithencryptedkey.crt` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/clientwithencryptedkey.crt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/clientwithkey.crt` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/clientwithkey.crt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/certificate/instructions.md` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/certificate/instructions.md`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/f4m/custom_base_url.f4m` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/f4m/custom_base_url.f4m`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/ism/ec-3_test.Manifest` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/ism/ec-3_test.Manifest`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/ism/sintel.Manifest` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/ism/sintel.Manifest`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/m3u8/bipbop_16x9.m3u8` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/m3u8/bipbop_16x9.m3u8`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/float_duration.mpd` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/float_duration.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/subtitles.mpd` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/subtitles.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/unfragmented.mpd` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/unfragmented.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/mpd/urls_only.mpd` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/mpd/urls_only.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/test/testdata/xspf/foo_xspf.xspf` & `yt_dlp-2024.5.8.232715.dev0/test/testdata/xspf/foo_xspf.xspf`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/YoutubeDL.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/YoutubeDL.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/aes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/aes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/cache.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/cache.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/cookies.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/cookies.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/jsinterp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/jsinterp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/minicurses.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/minicurses.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/options.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/options.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/plugins.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/plugins.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/socks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/socks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/update.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/update.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/webvtt.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/webvtt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/_deprecated.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/_deprecated.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/_legacy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/_legacy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/compat_utils.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/compat_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/imghdr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/imghdr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/shutil.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/shutil.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/compat/urllib/request.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/compat/urllib/request.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/dependencies/Cryptodome.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/dependencies/Cryptodome.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/dependencies/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/common.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/dash.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/dash.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/external.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/external.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/f4m.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/f4m.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/fc2.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/fc2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/fragment.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/fragment.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/hls.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/hls.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/http.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/http.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/ism.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/ism.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/mhtml.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/mhtml.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/niconico.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/niconico.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/rtmp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/rtmp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/rtsp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/rtsp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/websocket.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/websocket.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/downloader/youtube_live_chat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/downloader/youtube_live_chat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/_extractors.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/_extractors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abcnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abcnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abcotvs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abcotvs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/abematv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/abematv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/academicearth.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/academicearth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/acast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/acast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/acfun.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/acfun.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adobeconnect.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adobeconnect.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adobepass.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adobepass.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adobetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adobetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/adultswim.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/adultswim.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aenetworks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aenetworks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aeonco.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aeonco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/afreecatv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/afreecatv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/agora.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/agora.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/airtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/airtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aitube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aitube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aliexpress.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aliexpress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aljazeera.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aljazeera.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/allocine.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/allocine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/allstar.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/allstar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/alphaporno.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/alphaporno.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/alsace20tv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/alsace20tv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/altcensored.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/altcensored.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/alura.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/alura.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amadeustv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amadeustv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amara.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amara.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amazon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amazon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amazonminitv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amazonminitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amcnetworks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amcnetworks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/americastestkitchen.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/americastestkitchen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/amp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/amp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/anchorfm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/anchorfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/angel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/angel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/antenna.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/antenna.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/anvato.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/anvato.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aol.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aol.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/apa.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/apa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aparat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aparat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/appleconnect.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/appleconnect.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/applepodcasts.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/applepodcasts.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/appletrailers.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/appletrailers.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/archiveorg.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/archiveorg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arcpublishing.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arcpublishing.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ard.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ard.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arkena.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arkena.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arnes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arnes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/art19.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/art19.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/arte.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/arte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/asobichannel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/asobichannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/asobistage.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/asobistage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/atresplayer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/atresplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/atscaleconf.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/atscaleconf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/atvat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/atvat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audimedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audimedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audioboom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audioboom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audiodraft.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audiodraft.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audiomack.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audiomack.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/audius.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/audius.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/awaan.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/awaan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/aws.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/aws.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/axs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/axs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/azmedien.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/azmedien.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/baidu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/baidu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/banbye.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/banbye.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bandaichannel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bandaichannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bandcamp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bandcamp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bannedvideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bannedvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bbc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/beatbump.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/beatbump.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/beatport.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/beatport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/beeg.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/beeg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/behindkink.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/behindkink.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bellmedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bellmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/berufetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/berufetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bfi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bfi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bfmtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bfmtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bibeltv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bibeltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bigflix.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bigflix.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bigo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bigo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bild.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bild.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bilibili.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bilibili.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,19 @@
         missing_formats = format_names.keys() - set(traverse_obj(formats, (..., 'quality')))
         if missing_formats:
             self.to_screen(f'Format(s) {", ".join(format_names[i] for i in missing_formats)} are missing; '
                            f'you have to login or become premium member to download them. {self._login_hint()}')
 
         return formats
 
-    def _download_playinfo(self, video_id, cid):
+    def _download_playinfo(self, video_id, cid, headers=None):
         return self._download_json(
             'https://api.bilibili.com/x/player/playurl', video_id,
             query={'bvid': video_id, 'cid': cid, 'fnval': 4048},
-            note=f'Downloading video formats for cid {cid}')['data']
+            note=f'Downloading video formats for cid {cid}', headers=headers)['data']
 
     def json2srt(self, json_data):
         srt_data = ''
         for idx, line in enumerate(json_data.get('body') or []):
             srt_data += (f'{idx + 1}\n'
                          f'{srt_subtitles_timecode(line["from"])} --> {srt_subtitles_timecode(line["to"])}\n'
                          f'{line["content"]}\n\n')
@@ -489,15 +489,16 @@
             'ext': 'mp4',
         },
         'skip': 'geo-restricted',
     }]
 
     def _real_extract(self, url):
         video_id = self._match_id(url)
-        webpage, urlh = self._download_webpage_handle(url, video_id)
+        headers = self.geo_verification_headers()
+        webpage, urlh = self._download_webpage_handle(url, video_id, headers=headers)
         if not self._match_valid_url(urlh.url):
             return self.url_result(urlh.url)
 
         initial_state = self._search_json(r'window\.__INITIAL_STATE__\s*=', webpage, 'initial state', video_id)
 
         is_festival = 'videoData' not in initial_state
         if is_festival:
@@ -527,15 +528,15 @@
         video_id, title = video_data['bvid'], video_data.get('title')
 
         # Bilibili anthologies are similar to playlists but all videos share the same video ID as the anthology itself.
         page_list_json = not is_festival and traverse_obj(
             self._download_json(
                 'https://api.bilibili.com/x/player/pagelist', video_id,
                 fatal=False, query={'bvid': video_id, 'jsonp': 'jsonp'},
-                note='Extracting videos in anthology'),
+                note='Extracting videos in anthology', headers=headers),
             'data', expected_type=list) or []
         is_anthology = len(page_list_json) > 1
 
         part_id = int_or_none(parse_qs(url).get('p', [None])[-1])
         if is_anthology and not part_id and self._yes_playlist(video_id, video_id):
             return self.playlist_from_matches(
                 page_list_json, video_id, title, ie=BiliBiliIE,
@@ -548,15 +549,15 @@
         aid = video_data.get('aid')
         old_video_id = format_field(aid, None, f'%s_part{part_id or 1}')
 
         cid = traverse_obj(video_data, ('pages', part_id - 1, 'cid')) if part_id else video_data.get('cid')
 
         festival_info = {}
         if is_festival:
-            play_info = self._download_playinfo(video_id, cid)
+            play_info = self._download_playinfo(video_id, cid, headers=headers)
 
             festival_info = traverse_obj(initial_state, {
                 'uploader': ('videoInfo', 'upName'),
                 'uploader_id': ('videoInfo', 'upMid', {str_or_none}),
                 'like_count': ('videoStatus', 'like', {int_or_none}),
                 'thumbnail': ('sectionEpisodes', lambda _, v: v['bvid'] == video_id, 'cover'),
             }, get_all=False)
@@ -662,22 +663,23 @@
             'upload_date': '20201016',
             'thumbnail': r're:^https?://.*\.(jpg|jpeg|png)$'
         },
     }]
 
     def _real_extract(self, url):
         episode_id = self._match_id(url)
-        webpage = self._download_webpage(url, episode_id)
+        headers = self.geo_verification_headers()
+        webpage = self._download_webpage(url, episode_id, headers=headers)
 
         if '您所在的地区无法观看本片' in webpage:
             raise GeoRestrictedError('This video is restricted')
         elif '正在观看预览，大会员免费看全片' in webpage:
             self.raise_login_required('This video is for premium members only')
 
-        headers = {'Referer': url, **self.geo_verification_headers()}
+        headers['Referer'] = url
         play_info = self._download_json(
             'https://api.bilibili.com/pgc/player/web/v2/playurl', episode_id,
             'Extracting episode', query={'fnval': '4048', 'ep_id': episode_id},
             headers=headers)
         premium_only = play_info.get('code') == -10403
         play_info = traverse_obj(play_info, ('result', 'video_info', {dict})) or {}
 
@@ -720,15 +722,15 @@
             'episode_id': episode_id,
             'season': str_or_none(season_title),
             'season_id': str_or_none(season_id),
             'season_number': season_number,
             'duration': float_or_none(play_info.get('timelength'), scale=1000),
             'subtitles': self.extract_subtitles(episode_id, episode_info.get('cid'), aid=aid),
             '__post_extractor': self.extract_comments(aid),
-            'http_headers': headers,
+            'http_headers': {'Referer': url},
         }
 
 
 class BiliBiliBangumiMediaIE(BilibiliBaseIE):
     _VALID_URL = r'https?://(?:www\.)?bilibili\.com/bangumi/media/md(?P<id>\d+)'
     _TESTS = [{
         'url': 'https://www.bilibili.com/bangumi/media/md24097891',
@@ -1045,17 +1047,18 @@
                 response = self._download_json('https://api.bilibili.com/x/space/wbi/arc/search',
                                                playlist_id, note=f'Downloading page {page_idx}', query=query)
             except ExtractorError as e:
                 if isinstance(e.cause, HTTPError) and e.cause.status == 412:
                     raise ExtractorError(
                         'Request is blocked by server (412), please add cookies, wait and try later.', expected=True)
                 raise
-            if response['code'] == -401:
+            if response['code'] in (-352, -401):
                 raise ExtractorError(
-                    'Request is blocked by server (401), please add cookies, wait and try later.', expected=True)
+                    f'Request is blocked by server ({-response["code"]}), '
+                    'please add cookies, wait and try later.', expected=True)
             return response['data']
 
         def get_metadata(page_data):
             page_size = page_data['page']['ps']
             entry_count = page_data['page']['count']
             return {
                 'page_count': math.ceil(entry_count / page_size),
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/biobiochiletv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/biobiochiletv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bitchute.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bitchute.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/blackboardcollaborate.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/blackboardcollaborate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bleacherreport.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bleacherreport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/blerp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/blerp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/blogger.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/blogger.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bloomberg.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bloomberg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bokecc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bokecc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bongacams.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bongacams.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/boosty.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/boosty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import json
+import urllib.parse
+
 from .common import InfoExtractor
 from .youtube import YoutubeIE
 from ..utils import (
     ExtractorError,
+    bug_reports_message,
     int_or_none,
     qualities,
     str_or_none,
     url_or_none,
 )
 from ..utils.traversal import traverse_obj
 
@@ -158,17 +162,27 @@
                 })
             else:
                 self.report_warning(f'Unknown format type: {format_type!r}')
         return formats
 
     def _real_extract(self, url):
         user, post_id = self._match_valid_url(url).group('user', 'post_id')
+
+        auth_headers = {}
+        auth_cookie = self._get_cookies('https://boosty.to/').get('auth')
+        if auth_cookie is not None:
+            try:
+                auth_data = json.loads(urllib.parse.unquote(auth_cookie.value))
+                auth_headers['Authorization'] = f'Bearer {auth_data["accessToken"]}'
+            except (json.JSONDecodeError, KeyError):
+                self.report_warning(f'Failed to extract token from auth cookie{bug_reports_message()}')
+
         post = self._download_json(
             f'https://api.boosty.to/v1/blog/{user}/post/{post_id}', post_id,
-            note='Downloading post data', errnote='Unable to download post data')
+            note='Downloading post data', errnote='Unable to download post data', headers=auth_headers)
 
         post_title = post.get('title')
         if not post_title:
             self.report_warning('Unable to extract post title. Falling back to parsing html page')
             webpage = self._download_webpage(url, video_id=post_id)
             post_title = self._og_search_title(webpage, default=None) or self._html_extract_title(webpage)
 
@@ -198,12 +212,14 @@
                     **traverse_obj(item, {
                         'title': ('title', {str}),
                         'duration': ('duration', {int_or_none}),
                         'view_count': ('viewsCounter', {int_or_none}),
                         'thumbnail': (('previewUrl', 'defaultPreview'), {url_or_none}),
                     }, get_all=False)})
 
-        if not entries:
+        if not entries and not post.get('hasAccess'):
+            self.raise_login_required('This post requires a subscription', metadata_available=True)
+        elif not entries:
             raise ExtractorError('No videos found', expected=True)
         if len(entries) == 1:
             return entries[0]
         return self.playlist_result(entries, post_id, post_title, **common_metadata)
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bostonglobe.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bostonglobe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/box.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/box.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/boxcast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/boxcast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bpb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bpb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/br.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/br.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/brainpop.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/brainpop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bravotv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bravotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/breitbart.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/breitbart.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/brightcove.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/brightcove.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/brilliantpala.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/brilliantpala.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bundesliga.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bundesliga.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/bundestag.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/bundestag.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/businessinsider.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/businessinsider.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/buzzfeed.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/buzzfeed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/byutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/byutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/c56.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/c56.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cableav.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cableav.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/callin.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/callin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/caltrans.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/caltrans.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cam4.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cam4.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camdemy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camdemy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camfm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cammodels.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cammodels.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camsoda.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camsoda.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/camtasia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/camtasia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canal1.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canal1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canalalpha.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canalalpha.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canalc2.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canalc2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/canalplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/canalplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/caracoltv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/caracoltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cartoonnetwork.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cartoonnetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbsnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbsnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cbssports.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cbssports.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ccc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ccc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ccma.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ccma.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cctv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cctv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cda.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cda.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cellebrite.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cellebrite.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ceskatelevize.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cgtn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cgtn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/charlierose.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/charlierose.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/chaturbate.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/chaturbate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/chilloutzone.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/chilloutzone.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/chzzk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/chzzk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cinemax.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cinemax.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cinetecamilano.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cinetecamilano.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cineverse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cineverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ciscolive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ciscolive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ciscowebex.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ciscowebex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cjsw.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cjsw.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clipchamp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clipchamp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clippit.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clippit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cliprs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cliprs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/closertotruth.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/closertotruth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cloudflarestream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cloudflarestream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cloudycdn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cloudycdn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clubic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clubic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/clyp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/clyp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cmt.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cmt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cnbc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cnbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cnn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cnn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/comedycentral.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/comedycentral.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/common.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/commonmistakes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/commonmistakes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/commonprotocols.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/commonprotocols.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/condenast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/condenast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/contv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/contv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/corus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/corus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/coub.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/coub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cozytv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cozytv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cpac.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cpac.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cracked.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cracked.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crackle.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crackle.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/craftsy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/craftsy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crooksandliars.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crooksandliars.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crowdbunker.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crowdbunker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crtvg.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crtvg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/crunchyroll.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cspan.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cspan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ctsnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ctsnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ctv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ctv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ctvnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ctvnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cultureunplugged.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cultureunplugged.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/curiositystream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/curiositystream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cwtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cwtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/cybrary.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/cybrary.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dacast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dacast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dailymail.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dailymail.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dailymotion.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dailymotion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dailywire.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dailywire.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/damtomo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/damtomo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/daum.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/daum.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/daystar.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/daystar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dbtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dbtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dctp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dctp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/deezer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/deezer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/democracynow.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/democracynow.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/detik.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/detik.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/deuxm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/deuxm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dfb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dfb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dhm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dhm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/digitalconcerthall.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/digitalconcerthall.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/digiteka.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/digiteka.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/discogs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/discogs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/discovery.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/discovery.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/discoverygo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/discoverygo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/disney.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/disney.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dispeak.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dispeak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dlf.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dlf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dlive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dlive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/douyutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/douyutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drbonanza.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drbonanza.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dreisat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dreisat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drooble.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drooble.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dropbox.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dropbox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dropout.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dropout.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drtuber.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drtuber.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/drtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/drtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dtube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/duboku.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/duboku.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dumpert.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dumpert.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/duoplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/duoplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dvtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dvtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/dw.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/dw.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eagleplatform.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eagleplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ebaumsworld.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ebaumsworld.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ebay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ebay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/egghead.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/egghead.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eighttracks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eighttracks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/einthusan.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/einthusan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eitb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eitb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/elementorembed.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/elementorembed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/elonet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/elonet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/elpais.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/elpais.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eltrecetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eltrecetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/embedly.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/embedly.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/epicon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/epicon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/epidemicsound.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/epidemicsound.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/epoch.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/epoch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eporner.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eporner.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/erocast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/erocast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eroprofile.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eroprofile.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/err.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/err.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ertgr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ertgr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/espn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/espn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ettutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ettutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/europa.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/europa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/europeantour.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/europeantour.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eurosport.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eurosport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/euscreen.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/euscreen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/expressen.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/expressen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/extractors.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/extractors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/eyedotv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/eyedotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/facebook.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/facebook.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fancode.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fancode.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fathom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fathom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/faz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/faz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fc2.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fc2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fczenit.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fczenit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fifa.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fifa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/filmon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/filmon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/filmweb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/filmweb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/firsttv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/firsttv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fivetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fivetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/flextv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/flextv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/flickr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/flickr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/floatplane.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/floatplane.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/folketinget.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/folketinget.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/footyroom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/footyroom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/formula1.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/formula1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fourtube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fourtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fox.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fox9.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fox9.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/foxnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/foxnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/foxsports.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/foxsports.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fptplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fptplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/franceinter.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/franceinter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/francetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/francetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/freesound.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/freesound.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/freespeech.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/freespeech.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/freetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/freetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/frontendmasters.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/frontendmasters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fujitv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fujitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/funimation.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/funimation.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/funk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/funk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/funker530.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/funker530.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/fuyintv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/fuyintv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gab.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gab.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gaia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gaia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gamejolt.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gamejolt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gamespot.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gamespot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gamestar.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gamestar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gaskrank.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gaskrank.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gazeta.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gazeta.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gdcvault.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gdcvault.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gedidigital.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gedidigital.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/generic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/generic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/genericembeds.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/genericembeds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/genius.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/genius.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/getcourseru.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/getcourseru.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gettr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gettr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/giantbomb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/giantbomb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gigya.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gigya.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/glide.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/glide.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/globalplayer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/globalplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/globo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/globo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/glomex.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/glomex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gmanetwork.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gmanetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/go.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/go.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/godtube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/godtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gofile.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gofile.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/golem.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/golem.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/goodgame.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/goodgame.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/googledrive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/googledrive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/googlepodcasts.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/googlepodcasts.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/googlesearch.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/googlesearch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/goplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/goplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gopro.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gopro.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/goshgay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/goshgay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gotostage.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gotostage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gputechconf.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gputechconf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/gronkh.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/gronkh.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/groupon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/groupon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/harpodeon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/harpodeon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hbo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hbo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hearthisat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hearthisat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/heise.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/heise.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hellporno.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hellporno.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hgtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hgtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hidive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hidive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/historicfilms.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/historicfilms.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hitrecord.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hitrecord.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hketv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hketv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hollywoodreporter.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hollywoodreporter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/holodex.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/holodex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hotnewhiphop.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hotnewhiphop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hotstar.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hotstar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hrefli.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hrefli.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hrfensehen.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hrfensehen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hrti.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hrti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/huajiao.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/huajiao.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/huffpost.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/huffpost.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hungama.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hungama.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/huya.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/huya.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hypem.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hypem.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hypergryph.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hypergryph.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/hytale.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/hytale.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/icareus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/icareus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ichinanalive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ichinanalive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/idolplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/idolplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ign.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ign.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iheart.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iheart.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ilpost.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ilpost.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iltalehti.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iltalehti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/imdb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/imdb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/imggaming.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/imggaming.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/imgur.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/imgur.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ina.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ina.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/inc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/inc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/indavideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/indavideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/infoq.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/infoq.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/instagram.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/instagram.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/internazionale.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/internazionale.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/internetvideoarchive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/internetvideoarchive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iprima.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iprima.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iqiyi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iqiyi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/islamchannel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/islamchannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/israelnationalnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/israelnationalnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/itprotv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/itprotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/itv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/itv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ivi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ivi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ivideon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ivideon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/iwara.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/iwara.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ixigua.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ixigua.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/izlesene.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/izlesene.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jable.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jable.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jamendo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jamendo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/japandiet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/japandiet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jeuxvideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jeuxvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jiosaavn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jiosaavn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jixie.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jixie.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/joj.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/joj.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/joqrag.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/joqrag.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jove.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jove.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jstream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jstream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jtbc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jtbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/jwplatform.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/jwplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kakao.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kakao.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kaltura.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kaltura.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kankanews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kankanews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/karaoketv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/karaoketv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kelbyone.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kelbyone.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/khanacademy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/khanacademy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kick.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kick.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kicker.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kicker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kickstarter.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kickstarter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kinja.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kinja.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kinopoisk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kinopoisk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kommunetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kommunetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kompas.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kompas.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/koo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/koo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/krasview.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/krasview.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kth.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ku6.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ku6.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kukululive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kukululive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/kuwo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/kuwo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/la7.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/la7.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lastfm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lastfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/laxarxames.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/laxarxames.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lazy_extractors.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lazy_extractors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lbry.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lbry.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lci.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lci.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lcp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lcp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lecture2go.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lecture2go.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lecturio.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lecturio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/leeco.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/leeco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lefigaro.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lefigaro.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lego.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lego.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lemonde.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lemonde.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lenta.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lenta.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/libraryofcongress.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/libraryofcongress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/libsyn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/libsyn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lifenews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lifenews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/likee.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/likee.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/limelight.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/limelight.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/linkedin.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/linkedin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/liputan6.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/liputan6.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/listennotes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/listennotes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/litv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/litv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/livejournal.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/livejournal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/livestream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/livestream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/livestreamfails.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/livestreamfails.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lnkgo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lnkgo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/loom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/loom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lovehomeporn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lovehomeporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lrt.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lrt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lsm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lsm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lumni.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lumni.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/lynda.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/lynda.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/maariv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/maariv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/magellantv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/magellantv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/magentamusik.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/magentamusik.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mailru.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mailru.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mainstreaming.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mainstreaming.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mangomolo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mangomolo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/manoto.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/manoto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/manyvids.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/manyvids.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/maoritv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/maoritv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/markiza.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/markiza.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/massengeschmacktv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/massengeschmacktv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/masters.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/masters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/matchtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/matchtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mbn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mbn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mdr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mdr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/medaltv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/medaltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaite.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaite.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaklikk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/medialaan.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/medialaan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaset.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaset.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediasite.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediasite.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediastream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediastream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mediaworksnz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mediaworksnz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/medici.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/medici.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/megaphone.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/megaphone.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/megatvcom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/megatvcom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/meipai.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/meipai.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/melonvod.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/melonvod.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/metacritic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/metacritic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mgtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mgtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/microsoftembed.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/microsoftembed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/microsoftstream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/microsoftstream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/microsoftvirtualacademy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/microsoftvirtualacademy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mildom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mildom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/minds.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/minds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/minoto.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/minoto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mirrativ.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mirrativ.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mirrorcouk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mirrorcouk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mit.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mitele.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mitele.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mixch.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/scrolller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,102 @@
-from .common import InfoExtractor
-from ..networking.exceptions import HTTPError
-from ..utils import ExtractorError, UserNotLive, int_or_none, url_or_none
-from ..utils.traversal import traverse_obj
+import json
 
+from .common import InfoExtractor
+from ..utils import determine_ext, int_or_none
 
-class MixchIE(InfoExtractor):
-    IE_NAME = 'mixch'
-    _VALID_URL = r'https?://(?:www\.)?mixch\.tv/u/(?P<id>\d+)'
 
+class ScrolllerIE(InfoExtractor):
+    _VALID_URL = r'https?://(?:www\.)?scrolller\.com/(?P<id>[\w-]+)'
     _TESTS = [{
-        'url': 'https://mixch.tv/u/16236849/live',
-        'skip': 'don\'t know if this live persists',
+        'url': 'https://scrolller.com/a-helping-hand-1k9pxikxkw',
         'info_dict': {
-            'id': '16236849',
-            'title': '24配信シェア⭕️投票🙏💦',
-            'comment_count': 13145,
-            'view_count': 28348,
-            'timestamp': 1636189377,
-            'uploader': '🦥伊咲👶🏻#フレアワ',
-            'uploader_id': '16236849',
+            'id': 'a-helping-hand-1k9pxikxkw',
+            'ext': 'mp4',
+            'thumbnail': 'https://zepto.scrolller.com/a-helping-hand-3ty9q8x094-540x960.jpg',
+            'title': 'A helping hand',
+            'age_limit': 0,
         }
     }, {
-        'url': 'https://mixch.tv/u/16137876/live',
-        'only_matching': True,
-    }]
-
-    def _real_extract(self, url):
-        video_id = self._match_id(url)
-        data = self._download_json(f'https://mixch.tv/api-web/users/{video_id}/live', video_id)
-        if not traverse_obj(data, ('liveInfo', {dict})):
-            raise UserNotLive(video_id=video_id)
-
-        return {
-            'id': video_id,
-            'uploader_id': video_id,
-            **traverse_obj(data, {
-                'title': ('liveInfo', 'title', {str}),
-                'comment_count': ('liveInfo', 'comments', {int_or_none}),
-                'view_count': ('liveInfo', 'visitor', {int_or_none}),
-                'timestamp': ('liveInfo', 'created', {int_or_none}),
-                'uploader': ('broadcasterInfo', 'name', {str}),
-            }),
-            'formats': [{
-                'format_id': 'hls',
-                'url': data['liveInfo']['hls'],
-                'ext': 'mp4',
-                'protocol': 'm3u8',
-            }],
-            'is_live': True,
+        'url': 'https://scrolller.com/tigers-chasing-a-drone-c5d1f2so6j',
+        'info_dict': {
+            'id': 'tigers-chasing-a-drone-c5d1f2so6j',
+            'ext': 'mp4',
+            'thumbnail': 'https://zepto.scrolller.com/tigers-chasing-a-drone-az9pkpguwe-540x303.jpg',
+            'title': 'Tigers chasing a drone',
+            'age_limit': 0,
         }
-
-
-class MixchArchiveIE(InfoExtractor):
-    IE_NAME = 'mixch:archive'
-    _VALID_URL = r'https?://(?:www\.)?mixch\.tv/archive/(?P<id>\d+)'
-
-    _TESTS = [{
-        'url': 'https://mixch.tv/archive/421',
-        'skip': 'paid video, no DRM. expires at Jan 23',
+    }, {
+        'url': 'https://scrolller.com/baby-rhino-smells-something-9chhugsv9p',
         'info_dict': {
-            'id': '421',
+            'id': 'baby-rhino-smells-something-9chhugsv9p',
             'ext': 'mp4',
-            'title': '96NEKO SHOW TIME',
+            'thumbnail': 'https://atto.scrolller.com/hmm-whats-that-smell-bh54mf2c52-300x224.jpg',
+            'title': 'Baby rhino smells something',
+            'age_limit': 0,
         }
     }, {
-        'url': 'https://mixch.tv/archive/1213',
-        'skip': 'paid video, no DRM. expires at Dec 31, 2023',
+        'url': 'https://scrolller.com/its-all-fun-and-games-cco8jjmoh7',
         'info_dict': {
-            'id': '1213',
+            'id': 'its-all-fun-and-games-cco8jjmoh7',
             'ext': 'mp4',
-            'title': '【特別トーク番組アーカイブス】Merm4id×燐舞曲 2nd LIVE「VERSUS」',
-            'release_date': '20231201',
-            'thumbnail': str,
+            'thumbnail': 'https://atto.scrolller.com/its-all-fun-and-games-3amk9vg7m3-540x649.jpg',
+            'title': 'It\'s all fun and games...',
+            'age_limit': 0,
         }
     }, {
-        'url': 'https://mixch.tv/archive/1214',
-        'only_matching': True,
+        'url': 'https://scrolller.com/may-the-force-be-with-you-octokuro-yeytg1fs7a',
+        'info_dict': {
+            'id': 'may-the-force-be-with-you-octokuro-yeytg1fs7a',
+            'ext': 'mp4',
+            'thumbnail': 'https://thumbs2.redgifs.com/DarkStarchyNautilus-poster.jpg',
+            'title': 'May the force be with you (Octokuro)',
+            'age_limit': 18,
+        }
     }]
 
     def _real_extract(self, url):
         video_id = self._match_id(url)
 
-        try:
-            info_json = self._download_json(
-                f'https://mixch.tv/api-web/archive/{video_id}', video_id)['archive']
-        except ExtractorError as e:
-            if isinstance(e.cause, HTTPError) and e.cause.status == 401:
-                self.raise_login_required()
-            raise
+        query = {
+            'query': '''{
+                getSubredditPost(url:"/%s"){
+                    id
+                    title
+                    isNsfw
+                    mediaSources{
+                        url
+                        width
+                        height
+                    }
+                }
+            }''' % video_id
+        }
+
+        video_data = self._download_json(
+            'https://api.scrolller.com/api/v2/graphql', video_id, data=json.dumps(query).encode(),
+            headers={'Content-Type': 'application/json'})['data']['getSubredditPost']
+
+        formats, thumbnails = [], []
+        for source in video_data['mediaSources']:
+            if determine_ext(source.get('url')) in ('jpg', 'png'):
+                thumbnails.append({
+                    'url': source['url'],
+                    'width': int_or_none(source.get('width')),
+                    'height': int_or_none(source.get('height')),
+                })
+            elif source.get('url'):
+                formats.append({
+                    'url': source['url'],
+                    'width': int_or_none(source.get('width')),
+                    'height': int_or_none(source.get('height')),
+                })
+
+        if not formats:
+            self.raise_no_formats('There is no video.', expected=True, video_id=video_id)
 
         return {
             'id': video_id,
-            'title': traverse_obj(info_json, ('title', {str})),
-            'formats': self._extract_m3u8_formats(info_json['archiveURL'], video_id),
-            'thumbnail': traverse_obj(info_json, ('thumbnailURL', {url_or_none})),
+            'title': video_data.get('title'),
+            'thumbnails': thumbnails,
+            'formats': formats,
+            'age_limit': 18 if video_data.get('isNsfw') else 0
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mixcloud.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mixcloud.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mlb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mlb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mlssoccer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mlssoccer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mocha.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mocha.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mojvideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mojvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/monstercat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/monstercat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/motherless.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/motherless.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/motorsport.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/motorsport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/moviepilot.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/moviepilot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/moview.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/moview.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/moviezine.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/moviezine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/movingimage.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/movingimage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/msn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/msn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/muenchentv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/muenchentv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/murrtube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/murrtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/museai.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/museai.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/musescore.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/musescore.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/musicdex.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/musicdex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mx3.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mx3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mxplayer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mxplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myspace.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myspace.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myspass.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myspass.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myvideoge.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myvideoge.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/myvidster.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/myvidster.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/mzaalo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/mzaalo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/n1.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/n1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nate.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nationalgeographic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nationalgeographic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/naver.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/naver.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nba.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nba.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nbc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ndr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ndr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ndtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ndtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nebula.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nebula.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nekohacker.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nekohacker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nerdcubed.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nerdcubed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/neteasemusic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/neteasemusic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/netverse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/netverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/netzkino.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/netzkino.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/newgrounds.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/newgrounds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/newspicks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/newspicks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/newsy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/newsy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nextmedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nextmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nexx.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nexx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nfb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nfb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nfhsnetwork.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nfhsnetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nfl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nfl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nhk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nhk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nhl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nhl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nick.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nick.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/niconico.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/niconico.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/niconicochannelplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/niconicochannelplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninaprotocol.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninaprotocol.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninecninemedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninecninemedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninegag.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninegag.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninenews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninenews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ninenow.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ninenow.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nintendo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nintendo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nitter.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nitter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nobelprize.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nobelprize.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noice.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noice.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nonktube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nonktube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noodlemagazine.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noodlemagazine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noovo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noovo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nosnl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nosnl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nova.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nova.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/novaplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/novaplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nowness.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nowness.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/noz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/noz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/npo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/npo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/npr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/npr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nrk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nrk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nrl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nrl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ntvcojp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ntvcojp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ntvde.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ntvde.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ntvru.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ntvru.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nubilesporn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nubilesporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nuevo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nuevo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nuum.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nuum.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nuvid.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nuvid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nytimes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nytimes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nzherald.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nzherald.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nzonscreen.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nzonscreen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/nzz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/nzz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/odkmedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/odkmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/odnoklassniki.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/odnoklassniki.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/oftv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/oftv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/oktoberfesttv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/oktoberfesttv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/olympics.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/olympics.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/on24.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/on24.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/once.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/once.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ondemandkorea.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ondemandkorea.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onefootball.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onefootball.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onenewsnz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onenewsnz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/oneplace.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/oneplace.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/onionstudios.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/onionstudios.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/opencast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/opencast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/openload.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/openload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/openrec.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/openrec.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ora.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ora.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/orf.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/orf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/outsidetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/outsidetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/owncloud.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/owncloud.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/packtpub.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/packtpub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/palcomp3.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/palcomp3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/panopto.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/panopto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/paramountplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/paramountplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/parler.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/parler.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/parlview.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/parlview.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/patreon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/patreon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pbs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pearvideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pearvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peekvids.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peekvids.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peertube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peertube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peertv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peertv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/peloton.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/peloton.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/performgroup.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/performgroup.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/periscope.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/periscope.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pgatour.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pgatour.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/philharmoniedeparis.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/philharmoniedeparis.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/phoenix.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/phoenix.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/photobucket.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/photobucket.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/piapro.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/piapro.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/piaulizaportal.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/piaulizaportal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/picarto.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/picarto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/piksel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/piksel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pinkbike.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pinkbike.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pinterest.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pinterest.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pixivsketch.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pixivsketch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pladform.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pladform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/planetmarathi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/planetmarathi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/platzi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/platzi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playplustv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playplustv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playsuisse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playsuisse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playtvak.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playtvak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/playwire.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/playwire.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pluralsight.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pluralsight.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/plutotv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/plutotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/podbayfm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/podbayfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/podchaser.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/podchaser.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/podomatic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/podomatic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pokemon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pokemon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pokergo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pokergo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/polsatgo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/polsatgo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/polskieradio.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/polskieradio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/popcorntimes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/popcorntimes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/popcorntv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/popcorntv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/porn91.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/porn91.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornbox.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornbox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornflip.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornflip.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornhub.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornhub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornotube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornotube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornovoisines.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornovoisines.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pornoxo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pornoxo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pr0gramm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pr0gramm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/prankcast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/prankcast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/premiershiprugby.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/premiershiprugby.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/presstv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/presstv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/projectveritas.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/projectveritas.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/prosiebensat1.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/prosiebensat1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/prx.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/prx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/puhutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/puhutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/puls4.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/puls4.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/pyvideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/pyvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/qdance.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/qdance.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/qingting.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/qingting.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/qqmusic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/qqmusic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/r7.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/r7.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiko.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiko.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiocanada.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiocanada.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiocomercial.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiocomercial.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiode.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiode.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiofrance.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiofrance.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiojavan.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiojavan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiokapital.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiokapital.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radiozet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radiozet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/radlive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/radlive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rai.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rai.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/raywenderlich.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/raywenderlich.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rbgtum.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rbgtum.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rcs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rcs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rcti.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rcti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rds.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redbee.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redbee.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redbulltv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redbulltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/reddit.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/reddit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redge.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redge.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redgifs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redgifs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/redtube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/redtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rentv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rentv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/restudy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/restudy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/reuters.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/reuters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/reverbnation.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/reverbnation.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rheinmaintv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rheinmaintv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ridehome.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ridehome.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rinsefm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rinsefm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rmcdecouverte.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rmcdecouverte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rockstargames.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rockstargames.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rokfin.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rokfin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/roosterteeth.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/roosterteeth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rottentomatoes.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rozhlas.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rozhlas.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rte.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtl2.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtl2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtlnl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtlnl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtnews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtrfm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtrfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rts.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rts.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtvcplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtvcplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtve.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtve.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtvs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtvs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rtvslo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rtvslo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rudovideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rudovideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rule34video.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rule34video.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rumble.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rumble.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rutube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rutube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/rutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/rutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ruutu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ruutu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ruv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ruv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/s4c.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/s4c.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/safari.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/safari.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/saitosan.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/saitosan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/samplefocus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/samplefocus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sapo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sapo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sbs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sbscokr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sbscokr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screen9.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screen9.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screencast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screencast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screencastify.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screencastify.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/screencastomatic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/screencastomatic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/scrippsnetworks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/scrippsnetworks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/scrolller.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/utreon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,98 @@
-import json
-
 from .common import InfoExtractor
-from ..utils import determine_ext, int_or_none
+from ..utils import (
+    dict_get,
+    int_or_none,
+    str_or_none,
+    try_get,
+    unified_strdate,
+    url_or_none,
+)
 
 
-class ScrolllerIE(InfoExtractor):
-    _VALID_URL = r'https?://(?:www\.)?scrolller\.com/(?P<id>[\w-]+)'
+class UtreonIE(InfoExtractor):
+    IE_NAME = 'playeur'
+    _VALID_URL = r'https?://(?:www\.)?(?:utreon|playeur)\.com/v/(?P<id>[\w-]+)'
     _TESTS = [{
-        'url': 'https://scrolller.com/a-helping-hand-1k9pxikxkw',
+        'url': 'https://utreon.com/v/z_I7ikQbuDw',
         'info_dict': {
-            'id': 'a-helping-hand-1k9pxikxkw',
+            'id': 'z_I7ikQbuDw',
             'ext': 'mp4',
-            'thumbnail': 'https://zepto.scrolller.com/a-helping-hand-3ty9q8x094-540x960.jpg',
-            'title': 'A helping hand',
-            'age_limit': 0,
+            'title': 'Freedom Friday meditation - Rising in the wind',
+            'description': 'md5:a9bf15a42434a062fe313b938343ad1b',
+            'uploader': 'Heather Dawn Elemental Health',
+            'thumbnail': r're:^https?://.+\.jpg',
+            'release_date': '20210723',
+            'duration': 586,
         }
     }, {
-        'url': 'https://scrolller.com/tigers-chasing-a-drone-c5d1f2so6j',
+        'url': 'https://utreon.com/v/jerJw5EOOVU',
         'info_dict': {
-            'id': 'tigers-chasing-a-drone-c5d1f2so6j',
+            'id': 'jerJw5EOOVU',
             'ext': 'mp4',
-            'thumbnail': 'https://zepto.scrolller.com/tigers-chasing-a-drone-az9pkpguwe-540x303.jpg',
-            'title': 'Tigers chasing a drone',
-            'age_limit': 0,
+            'title': 'When I\'m alone, I love to reflect in peace, to make my dreams come true... [Quotes and Poems]',
+            'description': 'md5:4026aa3a2c10169c3649926ac8ef62b6',
+            'uploader': 'Frases e Poemas Quotes and Poems',
+            'thumbnail': r're:^https?://.+\.jpg',
+            'release_date': '20210723',
+            'duration': 60,
         }
     }, {
-        'url': 'https://scrolller.com/baby-rhino-smells-something-9chhugsv9p',
+        'url': 'https://utreon.com/v/C4ZxXhYBBmE',
         'info_dict': {
-            'id': 'baby-rhino-smells-something-9chhugsv9p',
+            'id': 'C4ZxXhYBBmE',
             'ext': 'mp4',
-            'thumbnail': 'https://atto.scrolller.com/hmm-whats-that-smell-bh54mf2c52-300x224.jpg',
-            'title': 'Baby rhino smells something',
-            'age_limit': 0,
+            'title': 'Biden’s Capital Gains Tax Rate to Test World’s Highest',
+            'description': 'md5:995aa9ad0733c0e5863ebdeff954f40e',
+            'uploader': 'Nomad Capitalist',
+            'thumbnail': r're:^https?://.+\.jpg',
+            'release_date': '20210723',
+            'duration': 884,
         }
     }, {
-        'url': 'https://scrolller.com/its-all-fun-and-games-cco8jjmoh7',
+        'url': 'https://utreon.com/v/Y-stEH-FBm8',
         'info_dict': {
-            'id': 'its-all-fun-and-games-cco8jjmoh7',
+            'id': 'Y-stEH-FBm8',
             'ext': 'mp4',
-            'thumbnail': 'https://atto.scrolller.com/its-all-fun-and-games-3amk9vg7m3-540x649.jpg',
-            'title': 'It\'s all fun and games...',
-            'age_limit': 0,
+            'title': 'Creeper-Chan Pranks Steve! 💚 [MINECRAFT ANIME]',
+            'description': 'md5:7a48450b0d761b96dec194be0c5ecb5f',
+            'uploader': 'Merryweather Comics',
+            'thumbnail': r're:^https?://.+\.jpg',
+            'release_date': '20210718',
+            'duration': 151,
         }
     }, {
-        'url': 'https://scrolller.com/may-the-force-be-with-you-octokuro-yeytg1fs7a',
+        'url': 'https://playeur.com/v/Wzqp-UrxSeu',
         'info_dict': {
-            'id': 'may-the-force-be-with-you-octokuro-yeytg1fs7a',
+            'id': 'Wzqp-UrxSeu',
             'ext': 'mp4',
-            'thumbnail': 'https://thumbs2.redgifs.com/DarkStarchyNautilus-poster.jpg',
-            'title': 'May the force be with you (Octokuro)',
-            'age_limit': 18,
+            'title': 'Update: Clockwork Basilisk Books on the Way!',
+            'description': 'md5:d9756b0b1884c904655b0e170d17cea5',
+            'uploader': 'Forgotten Weapons',
+            'release_date': '20240208',
+            'thumbnail': r're:^https?://.+\.jpg',
+            'duration': 262,
         }
     }]
 
     def _real_extract(self, url):
         video_id = self._match_id(url)
-
-        query = {
-            'query': '''{
-                getSubredditPost(url:"/%s"){
-                    id
-                    title
-                    isNsfw
-                    mediaSources{
-                        url
-                        width
-                        height
-                    }
-                }
-            }''' % video_id
-        }
-
-        video_data = self._download_json(
-            'https://api.scrolller.com/api/v2/graphql', video_id, data=json.dumps(query).encode(),
-            headers={'Content-Type': 'application/json'})['data']['getSubredditPost']
-
-        formats, thumbnails = [], []
-        for source in video_data['mediaSources']:
-            if determine_ext(source.get('url')) in ('jpg', 'png'):
-                thumbnails.append({
-                    'url': source['url'],
-                    'width': int_or_none(source.get('width')),
-                    'height': int_or_none(source.get('height')),
-                })
-            elif source.get('url'):
-                formats.append({
-                    'url': source['url'],
-                    'width': int_or_none(source.get('width')),
-                    'height': int_or_none(source.get('height')),
-                })
-
-        if not formats:
-            self.raise_no_formats('There is no video.', expected=True, video_id=video_id)
-
+        json_data = self._download_json(
+            'https://api.playeur.com/v1/videos/' + video_id,
+            video_id)
+        videos_json = json_data['videos']
+        formats = [{
+            'url': format_url,
+            'format_id': format_key.split('_')[1],
+            'height': int(format_key.split('_')[1][:-1]),
+        } for format_key, format_url in videos_json.items() if url_or_none(format_url)]
+        thumbnail = url_or_none(dict_get(json_data, ('cover_image_url', 'preview_image_url')))
         return {
             'id': video_id,
-            'title': video_data.get('title'),
-            'thumbnails': thumbnails,
+            'title': json_data['title'],
             'formats': formats,
-            'age_limit': 18 if video_data.get('isNsfw') else 0
+            'description': str_or_none(json_data.get('description')),
+            'duration': int_or_none(json_data.get('duration')),
+            'uploader': str_or_none(try_get(json_data, lambda x: x['channel']['title'])),
+            'thumbnail': thumbnail,
+            'release_date': unified_strdate(json_data.get('published_datetime')),
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/scte.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/scte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sejmpl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sejmpl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/senalcolombia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/senalcolombia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/senategov.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/senategov.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sendtonews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sendtonews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/servus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/servus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sevenplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sevenplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sexu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sexu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/seznamzpravy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/seznamzpravy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/shahid.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/shahid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sharepoint.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sharepoint.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/shemaroome.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/shemaroome.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/showroomlive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/showroomlive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sibnet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sibnet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/simplecast.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/simplecast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sina.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sina.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sixplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sixplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skeb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skeb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sky.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sky.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skyit.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skyit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skylinewebcams.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skylinewebcams.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skynewsarabia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skynewsarabia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/skynewsau.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/skynewsau.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/slideshare.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/slideshare.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/slideslive.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/slideslive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/slutload.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/slutload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/smotrim.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/smotrim.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/snotr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/snotr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sohu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sohu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sonyliv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sonyliv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/soundcloud.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/soundcloud.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/soundgasm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/soundgasm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/southpark.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/southpark.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sovietscloset.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sovietscloset.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spankbang.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spankbang.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spiegel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spiegel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spike.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spike.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sport5.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sport5.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sportbox.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sportbox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sportdeutschland.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sportdeutschland.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spotify.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spotify.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/spreaker.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/spreaker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/springboardplatform.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/springboardplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sprout.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sprout.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/srgssr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/srgssr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/srmediathek.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/srmediathek.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stacommu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stacommu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stageplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stageplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stanfordoc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stanfordoc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/startrek.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/startrek.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/startv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/startv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/steam.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/steam.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stitcher.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stitcher.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/storyfire.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/storyfire.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/streamable.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/streamable.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/streamcz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/streamcz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/streetvoice.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/streetvoice.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stretchinternet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stretchinternet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stripchat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stripchat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/stv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/stv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/substack.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/substack.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sunporno.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sunporno.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sverigesradio.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sverigesradio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/svt.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/svt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/swearnet.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/swearnet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/syfy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/syfy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/syvdk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/syvdk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/sztvhu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/sztvhu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tagesschau.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tagesschau.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tass.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tass.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tbs.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tbsjp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tbsjp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teachable.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teachable.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teachertube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teachertube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teachingchannel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teachingchannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teamcoco.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teamcoco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teamtreehouse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teamtreehouse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ted.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ted.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tele13.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tele13.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tele5.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tele5.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telebruxelles.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telebruxelles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telecaribe.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telecaribe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telecinco.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telecinco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telegraaf.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telegraaf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telegram.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telegram.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telemb.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telemb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telemundo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telemundo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telequebec.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telequebec.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/teletask.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/teletask.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/telewebion.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/telewebion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tempo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tempo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tencent.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tencent.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tennistv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tennistv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tenplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tenplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/testurl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/testurl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tf1.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tf1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tfo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tfo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theguardian.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theguardian.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theholetv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theholetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theintercept.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theintercept.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theplatform.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thestar.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thestar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thesun.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thesun.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/theweatherchannel.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/theweatherchannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thisamericanlife.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thisamericanlife.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thisoldhouse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thisoldhouse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/thisvid.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/thisvid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/threeqsdn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/threeqsdn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/threespeak.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/threespeak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tiktok.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tiktok.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tmz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tmz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tnaflix.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tnaflix.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toggle.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toggle.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toggo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toggo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tonline.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tonline.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toongoggles.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toongoggles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/toypics.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/toypics.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/traileraddict.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/traileraddict.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/triller.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/triller.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trovo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trovo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trtcocuk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trtcocuk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trtworld.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trtworld.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trueid.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trueid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trunews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trunews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/truth.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/truth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/trutv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/trutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tube8.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tube8.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tubetugraz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tubetugraz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tubitv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tubitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tumblr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tumblr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tunein.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tunein.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/turner.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/turner.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv2.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv24ua.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv24ua.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv2dk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv2dk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv2hu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv2hu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv4.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv4.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv5mondeplus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv5mondeplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tv5unis.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tv5unis.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tva.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/unistra.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,64 @@
-from .common import InfoExtractor
-from ..utils import (
-    float_or_none,
-    int_or_none,
-    smuggle_url,
-    strip_or_none,
-)
-
-
-class TVAIE(InfoExtractor):
-    _VALID_URL = r'https?://videos?\.tva\.ca/details/_(?P<id>\d+)'
-    _TESTS = [{
-        'url': 'https://videos.tva.ca/details/_5596811470001',
-        'info_dict': {
-            'id': '5596811470001',
-            'ext': 'mp4',
-            'title': 'Un extrait de l\'épisode du dimanche 8 octobre 2017 !',
-            'uploader_id': '5481942443001',
-            'upload_date': '20171003',
-            'timestamp': 1507064617,
-        },
-        'params': {
-            # m3u8 download
-            'skip_download': True,
-        },
-        'skip': 'HTTP Error 404: Not Found',
-    }, {
-        'url': 'https://video.tva.ca/details/_5596811470001',
-        'only_matching': True,
-    }]
-    BRIGHTCOVE_URL_TEMPLATE = 'http://players.brightcove.net/5481942443001/default_default/index.html?videoId=%s'
+import re
 
-    def _real_extract(self, url):
-        video_id = self._match_id(url)
+from .common import InfoExtractor
+from ..utils import qualities
 
-        return {
-            '_type': 'url_transparent',
-            'id': video_id,
-            'url': smuggle_url(self.BRIGHTCOVE_URL_TEMPLATE % video_id, {'geo_countries': ['CA']}),
-            'ie_key': 'BrightcoveNew',
-        }
 
+class UnistraIE(InfoExtractor):
+    _VALID_URL = r'https?://utv\.unistra\.fr/(?:index|video)\.php\?id_video\=(?P<id>\d+)'
 
-class QubIE(InfoExtractor):
-    _VALID_URL = r'https?://(?:www\.)?qub\.ca/(?:[^/]+/)*[0-9a-z-]+-(?P<id>\d+)'
-    _TESTS = [{
-        'url': 'https://www.qub.ca/tvaplus/tva/alerte-amber/saison-1/episode-01-1000036619',
-        'md5': '949490fd0e7aee11d0543777611fbd53',
-        'info_dict': {
-            'id': '6084352463001',
-            'ext': 'mp4',
-            'title': 'Épisode 01',
-            'uploader_id': '5481942443001',
-            'upload_date': '20190907',
-            'timestamp': 1567899756,
-            'description': 'md5:9c0d7fbb90939420c651fd977df90145',
+    _TESTS = [
+        {
+            'url': 'http://utv.unistra.fr/video.php?id_video=154',
+            'md5': '736f605cfdc96724d55bb543ab3ced24',
+            'info_dict': {
+                'id': '154',
+                'ext': 'mp4',
+                'title': 'M!ss Yella',
+                'description': 'md5:104892c71bd48e55d70b902736b81bbf',
+            },
         },
-    }, {
-        'url': 'https://www.qub.ca/tele/video/lcn-ca-vous-regarde-rev-30s-ap369664-1009357943',
-        'only_matching': True,
-    }]
-    # reference_id also works with old account_id(5481942443001)
-    # BRIGHTCOVE_URL_TEMPLATE = 'http://players.brightcove.net/5813221784001/default_default/index.html?videoId=ref:%s'
+        {
+            'url': 'http://utv.unistra.fr/index.php?id_video=437',
+            'md5': '1ddddd6cccaae76f622ce29b8779636d',
+            'info_dict': {
+                'id': '437',
+                'ext': 'mp4',
+                'title': 'Prix Louise Weiss 2014',
+                'description': 'md5:cc3a8735f079f4fb6b0b570fc10c135a',
+            },
+        }
+    ]
 
     def _real_extract(self, url):
-        entity_id = self._match_id(url)
-        entity = self._download_json(
-            'https://www.qub.ca/proxy/pfu/content-delivery-service/v1/entities',
-            entity_id, query={'id': entity_id})
-        video_id = entity['videoId']
-        episode = strip_or_none(entity.get('name'))
+        mobj = self._match_valid_url(url)
+        video_id = mobj.group('id')
+
+        webpage = self._download_webpage(url, video_id)
+
+        files = set(re.findall(r'file\s*:\s*"(/[^"]+)"', webpage))
+
+        quality = qualities(['SD', 'HD'])
+        formats = []
+        for file_path in files:
+            format_id = 'HD' if file_path.endswith('-HD.mp4') else 'SD'
+            formats.append({
+                'url': 'http://vod-flash.u-strasbg.fr:8080%s' % file_path,
+                'format_id': format_id,
+                'quality': quality(format_id)
+            })
+
+        title = self._html_search_regex(
+            r'<title>UTV - (.*?)</', webpage, 'title')
+        description = self._html_search_regex(
+            r'<meta name="Description" content="(.*?)"', webpage, 'description', flags=re.DOTALL)
+        thumbnail = self._search_regex(
+            r'image: "(.*?)"', webpage, 'thumbnail')
 
         return {
-            '_type': 'url_transparent',
             'id': video_id,
-            'title': episode,
-            # 'url': self.BRIGHTCOVE_URL_TEMPLATE % entity['referenceId'],
-            'url': 'https://videos.tva.ca/details/_' + video_id,
-            'description': entity.get('longDescription'),
-            'duration': float_or_none(entity.get('durationMillis'), 1000),
-            'episode': episode,
-            'episode_number': int_or_none(entity.get('episodeNumber')),
-            # 'ie_key': 'BrightcoveNew',
-            'ie_key': TVAIE.ie_key(),
+            'title': title,
+            'description': description,
+            'thumbnail': thumbnail,
+            'formats': formats
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvanouvelles.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvanouvelles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvc.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tver.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tver.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvigle.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvigle.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tviplayer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tviplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvland.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvland.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvn24.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvn24.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvnoe.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvnoe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvopengr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvopengr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tvplayer.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tvplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/tweakers.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tweakers.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twentymin.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twentymin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twentythreevideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twentythreevideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twitcasting.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twitcasting.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twitch.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twitch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/twitter.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/twitter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/txxx.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/txxx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/udemy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/udemy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/udn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/udn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ukcolumn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ukcolumn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/uktvplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/uktvplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/umg.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/umg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/unistra.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xboxclips.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 import re
 
 from .common import InfoExtractor
-from ..utils import qualities
-
-
-class UnistraIE(InfoExtractor):
-    _VALID_URL = r'https?://utv\.unistra\.fr/(?:index|video)\.php\?id_video\=(?P<id>\d+)'
-
-    _TESTS = [
-        {
-            'url': 'http://utv.unistra.fr/video.php?id_video=154',
-            'md5': '736f605cfdc96724d55bb543ab3ced24',
-            'info_dict': {
-                'id': '154',
-                'ext': 'mp4',
-                'title': 'M!ss Yella',
-                'description': 'md5:104892c71bd48e55d70b902736b81bbf',
-            },
-        },
-        {
-            'url': 'http://utv.unistra.fr/index.php?id_video=437',
-            'md5': '1ddddd6cccaae76f622ce29b8779636d',
-            'info_dict': {
-                'id': '437',
-                'ext': 'mp4',
-                'title': 'Prix Louise Weiss 2014',
-                'description': 'md5:cc3a8735f079f4fb6b0b570fc10c135a',
-            },
+from ..utils import (
+    int_or_none,
+    month_by_abbreviation,
+    parse_filesize,
+    parse_qs,
+)
+
+
+class XboxClipsIE(InfoExtractor):
+    _VALID_URL = r'https?://(?:www\.)?(?:xboxclips\.com|gameclips\.io)/(?:video\.php\?.*vid=|[^/]+/)(?P<id>[\da-f]{8}-(?:[\da-f]{4}-){3}[\da-f]{12})'
+    _TESTS = [{
+        'url': 'http://xboxclips.com/video.php?uid=2533274823424419&gamertag=Iabdulelah&vid=074a69a9-5faf-46aa-b93b-9909c1720325',
+        'md5': 'fbe1ec805e920aeb8eced3c3e657df5d',
+        'info_dict': {
+            'id': '074a69a9-5faf-46aa-b93b-9909c1720325',
+            'ext': 'mp4',
+            'title': 'iAbdulElah playing Titanfall',
+            'filesize_approx': 26800000,
+            'upload_date': '20140807',
+            'duration': 56,
         }
-    ]
+    }, {
+        'url': 'https://gameclips.io/iAbdulElah/074a69a9-5faf-46aa-b93b-9909c1720325',
+        'only_matching': True,
+    }]
 
     def _real_extract(self, url):
-        mobj = self._match_valid_url(url)
-        video_id = mobj.group('id')
+        video_id = self._match_id(url)
 
-        webpage = self._download_webpage(url, video_id)
+        if '/video.php' in url:
+            qs = parse_qs(url)
+            url = 'https://gameclips.io/%s/%s' % (qs['gamertag'][0], qs['vid'][0])
 
-        files = set(re.findall(r'file\s*:\s*"(/[^"]+)"', webpage))
+        webpage = self._download_webpage(url, video_id)
+        info = self._parse_html5_media_entries(url, webpage, video_id)[0]
 
-        quality = qualities(['SD', 'HD'])
-        formats = []
-        for file_path in files:
-            format_id = 'HD' if file_path.endswith('-HD.mp4') else 'SD'
-            formats.append({
-                'url': 'http://vod-flash.u-strasbg.fr:8080%s' % file_path,
-                'format_id': format_id,
-                'quality': quality(format_id)
-            })
-
-        title = self._html_search_regex(
-            r'<title>UTV - (.*?)</', webpage, 'title')
-        description = self._html_search_regex(
-            r'<meta name="Description" content="(.*?)"', webpage, 'description', flags=re.DOTALL)
-        thumbnail = self._search_regex(
-            r'image: "(.*?)"', webpage, 'thumbnail')
+        title = self._html_search_meta(['og:title', 'twitter:title'], webpage)
+        upload_date = None
+        mobj = re.search(
+            r'>Recorded: (\d{2})-(Jan|Feb|Mar|Apr|May|Ju[nl]|Aug|Sep|Oct|Nov|Dec)-(\d{4})',
+            webpage)
+        if mobj:
+            upload_date = '%s%.2d%s' % (mobj.group(3), month_by_abbreviation(mobj.group(2)), mobj.group(1))
+        filesize = parse_filesize(self._html_search_regex(
+            r'>Size: ([^<]+)<', webpage, 'file size', fatal=False))
+        duration = int_or_none(self._html_search_regex(
+            r'>Duration: (\d+) Seconds<', webpage, 'duration', fatal=False))
+        view_count = int_or_none(self._html_search_regex(
+            r'>Views: (\d+)<', webpage, 'view count', fatal=False))
 
-        return {
+        info.update({
             'id': video_id,
             'title': title,
-            'description': description,
-            'thumbnail': thumbnail,
-            'formats': formats
-        }
+            'upload_date': upload_date,
+            'filesize_approx': filesize,
+            'duration': duration,
+            'view_count': view_count,
+        })
+        return info
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/unity.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/unity.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/unsupported.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/unsupported.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/uol.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/uol.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/uplynk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/uplynk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/urort.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/urort.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/urplay.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/urplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/usanetwork.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/usanetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/usatoday.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/usatoday.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ustream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ustream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ustudio.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ustudio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/utreon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wevidi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,108 @@
 from .common import InfoExtractor
-from ..utils import (
-    dict_get,
-    int_or_none,
-    str_or_none,
-    try_get,
-    unified_strdate,
-    url_or_none,
-)
+from ..utils import clean_html, float_or_none, get_element_by_class, js_to_json, traverse_obj
 
 
-class UtreonIE(InfoExtractor):
-    IE_NAME = 'playeur'
-    _VALID_URL = r'https?://(?:www\.)?(?:utreon|playeur)\.com/v/(?P<id>[\w-]+)'
+class WeVidiIE(InfoExtractor):
+    _VALID_URL = r'https?://(?:www\.)?wevidi\.net/watch/(?P<id>[\w-]{11})'
     _TESTS = [{
-        'url': 'https://utreon.com/v/z_I7ikQbuDw',
+        'url': 'https://wevidi.net/watch/2th7UO5F4KV',
+        'md5': 'b913d1ff5bbad499e2c7ef4aa6d829d7',
         'info_dict': {
-            'id': 'z_I7ikQbuDw',
+            'id': '2th7UO5F4KV',
             'ext': 'mp4',
-            'title': 'Freedom Friday meditation - Rising in the wind',
-            'description': 'md5:a9bf15a42434a062fe313b938343ad1b',
-            'uploader': 'Heather Dawn Elemental Health',
-            'thumbnail': r're:^https?://.+\.jpg',
-            'release_date': '20210723',
-            'duration': 586,
+            'title': 'YouTube Alternative: WeVidi - customizable channels & more',
+            'thumbnail': r're:^https?://.*\.jpg$',
+            'description': 'md5:73a27d0a87d49fbcc5584566326ebeed',
+            'uploader': 'eclecRC',
+            'duration': 932.098,
         }
     }, {
-        'url': 'https://utreon.com/v/jerJw5EOOVU',
+        'url': 'https://wevidi.net/watch/ievRuuQHbPS',
+        'md5': 'ce8a94989a959bff9003fa27ee572935',
         'info_dict': {
-            'id': 'jerJw5EOOVU',
+            'id': 'ievRuuQHbPS',
             'ext': 'mp4',
-            'title': 'When I\'m alone, I love to reflect in peace, to make my dreams come true... [Quotes and Poems]',
-            'description': 'md5:4026aa3a2c10169c3649926ac8ef62b6',
-            'uploader': 'Frases e Poemas Quotes and Poems',
-            'thumbnail': r're:^https?://.+\.jpg',
-            'release_date': '20210723',
-            'duration': 60,
+            'title': 'WeVidi Playlists',
+            'thumbnail': r're:^https?://.*\.jpg$',
+            'description': 'md5:32cdfca272687390d9bd9b0c9c6153ee',
+            'uploader': 'WeVidi',
+            'duration': 36.1999,
         }
     }, {
-        'url': 'https://utreon.com/v/C4ZxXhYBBmE',
+        'url': 'https://wevidi.net/watch/PcMzDWaQSWb',
+        'md5': '55ee0d3434be5d9e5cc76b83f2bb57ec',
         'info_dict': {
-            'id': 'C4ZxXhYBBmE',
+            'id': 'PcMzDWaQSWb',
             'ext': 'mp4',
-            'title': 'Biden’s Capital Gains Tax Rate to Test World’s Highest',
-            'description': 'md5:995aa9ad0733c0e5863ebdeff954f40e',
-            'uploader': 'Nomad Capitalist',
-            'thumbnail': r're:^https?://.+\.jpg',
-            'release_date': '20210723',
-            'duration': 884,
+            'title': 'Cat blep',
+            'thumbnail': r're:^https?://.*\.jpg$',
+            'description': 'md5:e2c9e2b54b8bb424cc64937c8fdc068f',
+            'uploader': 'WeVidi',
+            'duration': 41.972,
         }
     }, {
-        'url': 'https://utreon.com/v/Y-stEH-FBm8',
+        'url': 'https://wevidi.net/watch/wJnRqDHNe_u',
+        'md5': 'c8f263dd47e66cc17546b3abf47b5a77',
         'info_dict': {
-            'id': 'Y-stEH-FBm8',
+            'id': 'wJnRqDHNe_u',
             'ext': 'mp4',
-            'title': 'Creeper-Chan Pranks Steve! 💚 [MINECRAFT ANIME]',
-            'description': 'md5:7a48450b0d761b96dec194be0c5ecb5f',
-            'uploader': 'Merryweather Comics',
-            'thumbnail': r're:^https?://.+\.jpg',
-            'release_date': '20210718',
-            'duration': 151,
+            'title': 'Gissy Talks: YouTube Alternatives',
+            'thumbnail': r're:^https?://.*\.jpg$',
+            'description': 'md5:e65036f0d4af80e0af191bd11af5195e',
+            'uploader': 'GissyEva',
+            'duration': 630.451,
         }
     }, {
-        'url': 'https://playeur.com/v/Wzqp-UrxSeu',
+        'url': 'https://wevidi.net/watch/4m1c4yJR_yc',
+        'md5': 'c63ce5ca6990dce86855fc02ca5bc1ed',
         'info_dict': {
-            'id': 'Wzqp-UrxSeu',
+            'id': '4m1c4yJR_yc',
             'ext': 'mp4',
-            'title': 'Update: Clockwork Basilisk Books on the Way!',
-            'description': 'md5:d9756b0b1884c904655b0e170d17cea5',
-            'uploader': 'Forgotten Weapons',
-            'release_date': '20240208',
-            'thumbnail': r're:^https?://.+\.jpg',
-            'duration': 262,
+            'title': 'Enough of that! - Awesome Exilez Podcast',
+            'thumbnail': r're:^https?://.*\.jpg$',
+            'description': 'md5:96af99dd63468b2dfab3020560e3e9b2',
+            'uploader': 'eclecRC',
+            'duration': 6.804,
         }
     }]
 
+    def _extract_formats(self, wvplayer_props):
+        # Taken from WeVidi player JS: https://wevidi.net/layouts/default/static/player.min.js
+        resolution_map = {
+            1: 144,
+            2: 240,
+            3: 360,
+            4: 480,
+            5: 720,
+            6: 1080
+        }
+
+        src_path = f'{wvplayer_props["srcVID"]}/{wvplayer_props["srcUID"]}/{wvplayer_props["srcNAME"]}'
+        for res in traverse_obj(wvplayer_props, ('resolutions', ..., {int}, {lambda x: x or None})):
+            format_id = str(-(res // -2) - 1)
+            yield {
+                'acodec': 'mp4a.40.2',
+                'ext': 'mp4',
+                'format_id': format_id,
+                'height': resolution_map.get(res),
+                'url': f'https://www.wevidi.net/videoplayback/{src_path}/{format_id}',
+                'vcodec': 'avc1.42E01E',
+            }
+
     def _real_extract(self, url):
         video_id = self._match_id(url)
-        json_data = self._download_json(
-            'https://api.playeur.com/v1/videos/' + video_id,
-            video_id)
-        videos_json = json_data['videos']
-        formats = [{
-            'url': format_url,
-            'format_id': format_key.split('_')[1],
-            'height': int(format_key.split('_')[1][:-1]),
-        } for format_key, format_url in videos_json.items() if url_or_none(format_url)]
-        thumbnail = url_or_none(dict_get(json_data, ('cover_image_url', 'preview_image_url')))
+        webpage = self._download_webpage(url, video_id)
+
+        wvplayer_props = self._search_json(
+            r'WVPlayer\(', webpage, 'player', video_id,
+            transform_source=lambda x: js_to_json(x.replace('||', '}')))
+
         return {
             'id': video_id,
-            'title': json_data['title'],
-            'formats': formats,
-            'description': str_or_none(json_data.get('description')),
-            'duration': int_or_none(json_data.get('duration')),
-            'uploader': str_or_none(try_get(json_data, lambda x: x['channel']['title'])),
-            'thumbnail': thumbnail,
-            'release_date': unified_strdate(json_data.get('published_datetime')),
+            'title': clean_html(get_element_by_class('video_title', webpage)),
+            'description': clean_html(get_element_by_class('descr_long', webpage)),
+            'uploader': clean_html(get_element_by_class('username', webpage)),
+            'formats': list(self._extract_formats(wvplayer_props)),
+            'thumbnail': self._og_search_thumbnail(webpage),
+            'duration': float_or_none(wvplayer_props.get('duration')),
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/varzesh3.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/varzesh3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vbox7.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vbox7.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/veo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/veo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/veoh.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/veoh.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vesti.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vesti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vevo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vevo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vgtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vgtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vh1.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vh1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vice.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vice.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viddler.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viddler.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videa.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videocampus_sachsen.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videocampus_sachsen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videodetective.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videodetective.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videofyme.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videofyme.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videoken.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videoken.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videomore.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videomore.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/videopress.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/videopress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vidio.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vidio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vidlii.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vidlii.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vidly.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vidly.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viewlift.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viewlift.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viidea.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viidea.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viki.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viki.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vimeo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vimeo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vimm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vimm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vine.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viously.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viously.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viqeo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viqeo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/viu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/viu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vk.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,39 +447,48 @@
             'upload date', default=None)) or int_or_none(data.get('date'))
 
         view_count = str_to_int(self._search_regex(
             r'class=["\']mv_views_count[^>]+>\s*([\d,.]+)',
             info_page, 'view count', default=None))
 
         formats = []
+        subtitles = {}
         for format_id, format_url in data.items():
             format_url = url_or_none(format_url)
             if not format_url or not format_url.startswith(('http', '//', 'rtmp')):
                 continue
             if (format_id.startswith(('url', 'cache'))
                     or format_id in ('extra_data', 'live_mp4', 'postlive_mp4')):
                 height = int_or_none(self._search_regex(
                     r'^(?:url|cache)(\d+)', format_id, 'height', default=None))
                 formats.append({
                     'format_id': format_id,
                     'url': format_url,
+                    'ext': 'mp4',
+                    'source_preference': 1,
                     'height': height,
                 })
             elif format_id == 'hls':
-                formats.extend(self._extract_m3u8_formats(
+                fmts, subs = self._extract_m3u8_formats_and_subtitles(
                     format_url, video_id, 'mp4', 'm3u8_native',
-                    m3u8_id=format_id, fatal=False, live=is_live))
+                    m3u8_id=format_id, fatal=False, live=is_live)
+                formats.extend(fmts)
+                self._merge_subtitles(subs, target=subtitles)
+            elif format_id.startswith('dash_'):
+                fmts, subs = self._extract_mpd_formats_and_subtitles(
+                    format_url, video_id, mpd_id=format_id, fatal=False)
+                formats.extend(fmts)
+                self._merge_subtitles(subs, target=subtitles)
             elif format_id == 'rtmp':
                 formats.append({
                     'format_id': format_id,
                     'url': format_url,
                     'ext': 'flv',
                 })
 
-        subtitles = {}
         for sub in data.get('subs') or {}:
             subtitles.setdefault(sub.get('lang', 'en'), []).append({
                 'ext': sub.get('title', '.srt').split('.')[-1],
                 'url': url_or_none(sub.get('url')),
             })
 
         return {
@@ -492,14 +501,15 @@
             'duration': int_or_none(data.get('duration') or mv_data.get('duration')),
             'timestamp': timestamp,
             'view_count': view_count,
             'like_count': int_or_none(mv_data.get('likes')),
             'comment_count': int_or_none(mv_data.get('commcount')),
             'is_live': is_live,
             'subtitles': subtitles,
+            '_format_sort_fields': ('res', 'source'),
         }
 
 
 class VKUserVideosIE(VKBaseIE):
     IE_NAME = 'vk:uservideos'
     IE_DESC = "VK - User's Videos"
     _VALID_URL = r'https?://(?:(?:m|new)\.)?vk\.com/video/(?:playlist/)?(?P<id>[^?$#/&]+)(?!\?.*\bz=video)(?:[/?#&](?:.*?\bsection=(?P<section>\w+))?|$)'
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vocaroo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vocaroo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vodpl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vodpl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vodplatform.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vodplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/voicy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/voicy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/volejtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/volejtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/voot.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/voot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/voxmedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/voxmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vrt.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vrt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vtm.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vtm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vuclip.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vuclip.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/vvvvid.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/vvvvid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/walla.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/walla.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/washingtonpost.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wat.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wdr.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wdr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/webcamerapl.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/webcamerapl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/webcaster.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/webcaster.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/webofstories.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/webofstories.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weibo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weibo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weiqitv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weiqitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weverse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wevidi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/tva.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,95 @@
+import functools
+import re
+
 from .common import InfoExtractor
-from ..utils import clean_html, float_or_none, get_element_by_class, js_to_json, traverse_obj
+from ..utils import float_or_none, int_or_none, smuggle_url, strip_or_none
+from ..utils.traversal import traverse_obj
 
 
-class WeVidiIE(InfoExtractor):
-    _VALID_URL = r'https?://(?:www\.)?wevidi\.net/watch/(?P<id>[\w-]{11})'
+class TVAIE(InfoExtractor):
+    _VALID_URL = r'https?://videos?\.tva\.ca/details/_(?P<id>\d+)'
     _TESTS = [{
-        'url': 'https://wevidi.net/watch/2th7UO5F4KV',
-        'md5': 'b913d1ff5bbad499e2c7ef4aa6d829d7',
+        'url': 'https://videos.tva.ca/details/_5596811470001',
         'info_dict': {
-            'id': '2th7UO5F4KV',
+            'id': '5596811470001',
             'ext': 'mp4',
-            'title': 'YouTube Alternative: WeVidi - customizable channels & more',
-            'thumbnail': r're:^https?://.*\.jpg$',
-            'description': 'md5:73a27d0a87d49fbcc5584566326ebeed',
-            'uploader': 'eclecRC',
-            'duration': 932.098,
-        }
+            'title': 'Un extrait de l\'épisode du dimanche 8 octobre 2017 !',
+            'uploader_id': '5481942443001',
+            'upload_date': '20171003',
+            'timestamp': 1507064617,
+        },
+        'params': {
+            # m3u8 download
+            'skip_download': True,
+        },
+        'skip': 'HTTP Error 404: Not Found',
     }, {
-        'url': 'https://wevidi.net/watch/ievRuuQHbPS',
-        'md5': 'ce8a94989a959bff9003fa27ee572935',
-        'info_dict': {
-            'id': 'ievRuuQHbPS',
-            'ext': 'mp4',
-            'title': 'WeVidi Playlists',
-            'thumbnail': r're:^https?://.*\.jpg$',
-            'description': 'md5:32cdfca272687390d9bd9b0c9c6153ee',
-            'uploader': 'WeVidi',
-            'duration': 36.1999,
-        }
-    }, {
-        'url': 'https://wevidi.net/watch/PcMzDWaQSWb',
-        'md5': '55ee0d3434be5d9e5cc76b83f2bb57ec',
-        'info_dict': {
-            'id': 'PcMzDWaQSWb',
-            'ext': 'mp4',
-            'title': 'Cat blep',
-            'thumbnail': r're:^https?://.*\.jpg$',
-            'description': 'md5:e2c9e2b54b8bb424cc64937c8fdc068f',
-            'uploader': 'WeVidi',
-            'duration': 41.972,
+        'url': 'https://video.tva.ca/details/_5596811470001',
+        'only_matching': True,
+    }]
+    BRIGHTCOVE_URL_TEMPLATE = 'http://players.brightcove.net/5481942443001/default_default/index.html?videoId=%s'
+
+    def _real_extract(self, url):
+        video_id = self._match_id(url)
+
+        return {
+            '_type': 'url_transparent',
+            'id': video_id,
+            'url': smuggle_url(self.BRIGHTCOVE_URL_TEMPLATE % video_id, {'geo_countries': ['CA']}),
+            'ie_key': 'BrightcoveNew',
         }
-    }, {
-        'url': 'https://wevidi.net/watch/wJnRqDHNe_u',
-        'md5': 'c8f263dd47e66cc17546b3abf47b5a77',
+
+
+class QubIE(InfoExtractor):
+    _VALID_URL = r'https?://(?:www\.)?qub\.ca/(?:[^/]+/)*[0-9a-z-]+-(?P<id>\d+)'
+    _TESTS = [{
+        'url': 'https://www.qub.ca/tvaplus/tva/alerte-amber/saison-1/episode-01-1000036619',
+        'md5': '949490fd0e7aee11d0543777611fbd53',
         'info_dict': {
-            'id': 'wJnRqDHNe_u',
+            'id': '6084352463001',
             'ext': 'mp4',
-            'title': 'Gissy Talks: YouTube Alternatives',
-            'thumbnail': r're:^https?://.*\.jpg$',
-            'description': 'md5:e65036f0d4af80e0af191bd11af5195e',
-            'uploader': 'GissyEva',
-            'duration': 630.451,
-        }
+            'title': 'Ép 01. Mon dernier jour',
+            'uploader_id': '5481942443001',
+            'upload_date': '20190907',
+            'timestamp': 1567899756,
+            'description': 'md5:9c0d7fbb90939420c651fd977df90145',
+            'thumbnail': r're:https://.+\.jpg',
+            'episode': 'Ép 01. Mon dernier jour',
+            'episode_number': 1,
+            'tags': ['alerte amber', 'alerte amber saison 1', 'surdemande'],
+            'duration': 2625.963,
+            'season': 'Season 1',
+            'season_number': 1,
+            'series': 'Alerte Amber',
+            'channel': 'TVA',
+        },
     }, {
-        'url': 'https://wevidi.net/watch/4m1c4yJR_yc',
-        'md5': 'c63ce5ca6990dce86855fc02ca5bc1ed',
-        'info_dict': {
-            'id': '4m1c4yJR_yc',
-            'ext': 'mp4',
-            'title': 'Enough of that! - Awesome Exilez Podcast',
-            'thumbnail': r're:^https?://.*\.jpg$',
-            'description': 'md5:96af99dd63468b2dfab3020560e3e9b2',
-            'uploader': 'eclecRC',
-            'duration': 6.804,
-        }
+        'url': 'https://www.qub.ca/tele/video/lcn-ca-vous-regarde-rev-30s-ap369664-1009357943',
+        'only_matching': True,
     }]
-
-    def _extract_formats(self, wvplayer_props):
-        # Taken from WeVidi player JS: https://wevidi.net/layouts/default/static/player.min.js
-        resolution_map = {
-            1: 144,
-            2: 240,
-            3: 360,
-            4: 480,
-            5: 720,
-            6: 1080
-        }
-
-        src_path = f'{wvplayer_props["srcVID"]}/{wvplayer_props["srcUID"]}/{wvplayer_props["srcNAME"]}'
-        for res in traverse_obj(wvplayer_props, ('resolutions', ..., {int}, {lambda x: x or None})):
-            format_id = str(-(res // -2) - 1)
-            yield {
-                'acodec': 'mp4a.40.2',
-                'ext': 'mp4',
-                'format_id': format_id,
-                'height': resolution_map.get(res),
-                'url': f'https://www.wevidi.net/videoplayback/{src_path}/{format_id}',
-                'vcodec': 'avc1.42E01E',
-            }
+    # reference_id also works with old account_id(5481942443001)
+    # BRIGHTCOVE_URL_TEMPLATE = 'http://players.brightcove.net/5813221784001/default_default/index.html?videoId=ref:%s'
 
     def _real_extract(self, url):
-        video_id = self._match_id(url)
-        webpage = self._download_webpage(url, video_id)
-
-        wvplayer_props = self._search_json(
-            r'WVPlayer\(', webpage, 'player', video_id,
-            transform_source=lambda x: js_to_json(x.replace('||', '}')))
+        entity_id = self._match_id(url)
+        webpage = self._download_webpage(url, entity_id)
+        entity = self._search_nextjs_data(webpage, entity_id)['props']['initialProps']['pageProps']['fallbackData']
+        video_id = entity['videoId']
+        episode = strip_or_none(entity.get('name'))
 
         return {
+            '_type': 'url_transparent',
+            'url': f'https://videos.tva.ca/details/_{video_id}',
+            'ie_key': TVAIE.ie_key(),
             'id': video_id,
-            'title': clean_html(get_element_by_class('video_title', webpage)),
-            'description': clean_html(get_element_by_class('descr_long', webpage)),
-            'uploader': clean_html(get_element_by_class('username', webpage)),
-            'formats': list(self._extract_formats(wvplayer_props)),
-            'thumbnail': self._og_search_thumbnail(webpage),
-            'duration': float_or_none(wvplayer_props.get('duration')),
+            'title': episode,
+            'episode': episode,
+            **traverse_obj(entity, {
+                'description': ('longDescription', {str}),
+                'duration': ('durationMillis', {functools.partial(float_or_none, scale=1000)}),
+                'channel': ('knownEntities', 'channel', 'name', {str}),
+                'series': ('knownEntities', 'videoShow', 'name', {str}),
+                'season_number': ('slug', {lambda x: re.search(r'/s(?:ai|ea)son-(\d+)/', x)}, 1, {int_or_none}),
+                'episode_number': ('episodeNumber', {int_or_none}),
+            }),
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/weyyak.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/weyyak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/whowatch.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/whowatch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/whyp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/whyp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wikimedia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wikimedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wimbledon.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wimbledon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wimtv.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wimtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wistia.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wistia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wordpress.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wordpress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/worldstarhiphop.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/worldstarhiphop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wppilot.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wppilot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wrestleuniverse.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wrestleuniverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wsj.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wsj.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wwe.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wwe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/wykop.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/wykop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xanimu.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xanimu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xboxclips.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youjizz.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,90 @@
-import re
-
 from .common import InfoExtractor
 from ..utils import (
+    determine_ext,
     int_or_none,
-    month_by_abbreviation,
-    parse_filesize,
-    parse_qs,
+    parse_duration,
+    url_or_none,
 )
 
 
-class XboxClipsIE(InfoExtractor):
-    _VALID_URL = r'https?://(?:www\.)?(?:xboxclips\.com|gameclips\.io)/(?:video\.php\?.*vid=|[^/]+/)(?P<id>[\da-f]{8}-(?:[\da-f]{4}-){3}[\da-f]{12})'
+class YouJizzIE(InfoExtractor):
+    _VALID_URL = r'https?://(?:\w+\.)?youjizz\.com/videos/(?:[^/#?]*-(?P<id>\d+)\.html|embed/(?P<embed_id>\d+))'
     _TESTS = [{
-        'url': 'http://xboxclips.com/video.php?uid=2533274823424419&gamertag=Iabdulelah&vid=074a69a9-5faf-46aa-b93b-9909c1720325',
-        'md5': 'fbe1ec805e920aeb8eced3c3e657df5d',
+        'url': 'http://www.youjizz.com/videos/zeichentrick-1-2189178.html',
+        'md5': 'b1e1dfaa8bb9537d8b84eeda9cf4acf4',
         'info_dict': {
-            'id': '074a69a9-5faf-46aa-b93b-9909c1720325',
+            'id': '2189178',
             'ext': 'mp4',
-            'title': 'iAbdulElah playing Titanfall',
-            'filesize_approx': 26800000,
-            'upload_date': '20140807',
-            'duration': 56,
+            'title': 'Zeichentrick 1',
+            'age_limit': 18,
+            'duration': 2874,
         }
     }, {
-        'url': 'https://gameclips.io/iAbdulElah/074a69a9-5faf-46aa-b93b-9909c1720325',
+        'url': 'http://www.youjizz.com/videos/-2189178.html',
+        'only_matching': True,
+    }, {
+        'url': 'https://www.youjizz.com/videos/embed/31991001',
         'only_matching': True,
     }]
 
     def _real_extract(self, url):
-        video_id = self._match_id(url)
-
-        if '/video.php' in url:
-            qs = parse_qs(url)
-            url = 'https://gameclips.io/%s/%s' % (qs['gamertag'][0], qs['vid'][0])
+        mobj = self._match_valid_url(url)
+        video_id = mobj.group('id') or mobj.group('embed_id')
 
         webpage = self._download_webpage(url, video_id)
-        info = self._parse_html5_media_entries(url, webpage, video_id)[0]
 
-        title = self._html_search_meta(['og:title', 'twitter:title'], webpage)
-        upload_date = None
-        mobj = re.search(
-            r'>Recorded: (\d{2})-(Jan|Feb|Mar|Apr|May|Ju[nl]|Aug|Sep|Oct|Nov|Dec)-(\d{4})',
-            webpage)
-        if mobj:
-            upload_date = '%s%.2d%s' % (mobj.group(3), month_by_abbreviation(mobj.group(2)), mobj.group(1))
-        filesize = parse_filesize(self._html_search_regex(
-            r'>Size: ([^<]+)<', webpage, 'file size', fatal=False))
-        duration = int_or_none(self._html_search_regex(
-            r'>Duration: (\d+) Seconds<', webpage, 'duration', fatal=False))
-        view_count = int_or_none(self._html_search_regex(
-            r'>Views: (\d+)<', webpage, 'view count', fatal=False))
+        title = self._html_extract_title(webpage)
 
-        info.update({
+        formats = []
+
+        encodings = self._parse_json(
+            self._search_regex(
+                r'[Ee]ncodings\s*=\s*(\[.+?\]);\n', webpage, 'encodings',
+                default='[]'),
+            video_id, fatal=False)
+        for encoding in encodings:
+            if not isinstance(encoding, dict):
+                continue
+            format_url = url_or_none(encoding.get('filename'))
+            if not format_url:
+                continue
+            if determine_ext(format_url) == 'm3u8':
+                formats.extend(self._extract_m3u8_formats(
+                    format_url, video_id, 'mp4', entry_protocol='m3u8_native',
+                    m3u8_id='hls', fatal=False))
+            else:
+                format_id = encoding.get('name') or encoding.get('quality')
+                height = int_or_none(self._search_regex(
+                    r'^(\d+)[pP]', format_id, 'height', default=None))
+                formats.append({
+                    'url': format_url,
+                    'format_id': format_id,
+                    'height': height,
+                })
+
+        if formats:
+            info_dict = {
+                'formats': formats,
+            }
+        else:
+            # YouJizz's HTML5 player has invalid HTML
+            webpage = webpage.replace('"controls', '" controls')
+            info_dict = self._parse_html5_media_entries(
+                url, webpage, video_id)[0]
+
+        duration = parse_duration(self._search_regex(
+            r'<strong>Runtime:</strong>([^<]+)', webpage, 'duration',
+            default=None))
+        uploader = self._search_regex(
+            r'<strong>Uploaded By:.*?<a[^>]*>([^<]+)', webpage, 'uploader',
+            default=None)
+
+        info_dict.update({
             'id': video_id,
             'title': title,
-            'upload_date': upload_date,
-            'filesize_approx': filesize,
+            'age_limit': self._rta_search(webpage),
             'duration': duration,
-            'view_count': view_count,
+            'uploader': uploader,
         })
-        return info
+
+        return info_dict
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xfileshare.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xfileshare.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xhamster.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xhamster.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/ximalaya.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/ximalaya.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xinpianchang.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xinpianchang.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xminus.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xminus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xnxx.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xnxx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xstream.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xstream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xvideos.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xvideos.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/xxxymovies.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/xxxymovies.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yahoo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yahoo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yandexdisk.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yandexdisk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yandexmusic.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yandexmusic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yandexvideo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yandexvideo.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,23 +255,23 @@
         webpage = self._download_webpage(url, video_id)
         redirect = self._search_json(r'var it\s*=', webpage, 'redirect', id, default={}).get('retpath')
         if redirect:
             video_id = self._match_id(redirect)
             webpage = self._download_webpage(redirect, video_id, note='Redirecting')
         data_json = self._search_json(
             r'("data"\s*:|data\s*=)', webpage, 'metadata', video_id, contains_pattern=r'{["\']_*serverState_*video.+}')
-        serverstate = self._search_regex(r'(_+serverState_+video-site_[^_]+_+)',
-                                         webpage, 'server state').replace('State', 'Settings')
+        serverstate = self._search_regex(r'(_+serverState_+video-site_[^_]+_+)', webpage, 'server state')
         uploader = self._search_regex(r'(<a\s*class=["\']card-channel-link[^"\']+["\'][^>]+>)',
                                       webpage, 'uploader', default='<a>')
         uploader_name = extract_attributes(uploader).get('aria-label')
-        video_json = try_get(data_json, lambda x: x[serverstate]['exportData']['video'], dict)
-        stream_urls = try_get(video_json, lambda x: x['video']['streams'])
+        item_id = traverse_obj(data_json, (serverstate, 'videoViewer', 'openedItemId', {str}))
+        video_json = traverse_obj(data_json, (serverstate, 'videoViewer', 'items', item_id, {dict})) or {}
+
         formats, subtitles = [], {}
-        for s_url in stream_urls:
+        for s_url in traverse_obj(video_json, ('video', 'streams', ..., {url_or_none})):
             ext = determine_ext(s_url)
             if ext == 'mpd':
                 fmts, subs = self._extract_mpd_formats_and_subtitles(s_url, video_id, mpd_id='dash')
             elif ext == 'm3u8':
                 fmts, subs = self._extract_m3u8_formats_and_subtitles(s_url, video_id, 'mp4')
             formats.extend(fmts)
             subtitles = self._merge_subtitles(subtitles, subs)
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yapfiles.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yapfiles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yappy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yappy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yle_areena.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yle_areena.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youjizz.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zhihu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,65 @@
 from .common import InfoExtractor
-from ..utils import (
-    determine_ext,
-    int_or_none,
-    parse_duration,
-    url_or_none,
-)
+from ..utils import format_field, float_or_none, int_or_none
 
 
-class YouJizzIE(InfoExtractor):
-    _VALID_URL = r'https?://(?:\w+\.)?youjizz\.com/videos/(?:[^/#?]*-(?P<id>\d+)\.html|embed/(?P<embed_id>\d+))'
-    _TESTS = [{
-        'url': 'http://www.youjizz.com/videos/zeichentrick-1-2189178.html',
-        'md5': 'b1e1dfaa8bb9537d8b84eeda9cf4acf4',
+class ZhihuIE(InfoExtractor):
+    _VALID_URL = r'https?://(?:www\.)?zhihu\.com/zvideo/(?P<id>[0-9]+)'
+    _TEST = {
+        'url': 'https://www.zhihu.com/zvideo/1342930761977176064',
+        'md5': 'c8d4c9cd72dd58e6f9bc9c2c84266464',
         'info_dict': {
-            'id': '2189178',
+            'id': '1342930761977176064',
             'ext': 'mp4',
-            'title': 'Zeichentrick 1',
-            'age_limit': 18,
-            'duration': 2874,
+            'title': '写春联也太难了吧！',
+            'thumbnail': r're:^https?://.*\.jpg',
+            'uploader': '桥半舫',
+            'timestamp': 1612959715,
+            'upload_date': '20210210',
+            'uploader_id': '244ecb13b0fd7daf92235288c8ca3365',
+            'duration': 146.333,
+            'view_count': int,
+            'like_count': int,
+            'comment_count': int,
         }
-    }, {
-        'url': 'http://www.youjizz.com/videos/-2189178.html',
-        'only_matching': True,
-    }, {
-        'url': 'https://www.youjizz.com/videos/embed/31991001',
-        'only_matching': True,
-    }]
+    }
 
     def _real_extract(self, url):
-        mobj = self._match_valid_url(url)
-        video_id = mobj.group('id') or mobj.group('embed_id')
-
-        webpage = self._download_webpage(url, video_id)
-
-        title = self._html_extract_title(webpage)
+        video_id = self._match_id(url)
+        zvideo = self._download_json(
+            'https://www.zhihu.com/api/v4/zvideos/' + video_id, video_id)
+        title = zvideo['title']
+        video = zvideo.get('video') or {}
 
         formats = []
-
-        encodings = self._parse_json(
-            self._search_regex(
-                r'[Ee]ncodings\s*=\s*(\[.+?\]);\n', webpage, 'encodings',
-                default='[]'),
-            video_id, fatal=False)
-        for encoding in encodings:
-            if not isinstance(encoding, dict):
-                continue
-            format_url = url_or_none(encoding.get('filename'))
-            if not format_url:
+        for format_id, q in (video.get('playlist') or {}).items():
+            play_url = q.get('url') or q.get('play_url')
+            if not play_url:
                 continue
-            if determine_ext(format_url) == 'm3u8':
-                formats.extend(self._extract_m3u8_formats(
-                    format_url, video_id, 'mp4', entry_protocol='m3u8_native',
-                    m3u8_id='hls', fatal=False))
-            else:
-                format_id = encoding.get('name') or encoding.get('quality')
-                height = int_or_none(self._search_regex(
-                    r'^(\d+)[pP]', format_id, 'height', default=None))
-                formats.append({
-                    'url': format_url,
-                    'format_id': format_id,
-                    'height': height,
-                })
-
-        if formats:
-            info_dict = {
-                'formats': formats,
-            }
-        else:
-            # YouJizz's HTML5 player has invalid HTML
-            webpage = webpage.replace('"controls', '" controls')
-            info_dict = self._parse_html5_media_entries(
-                url, webpage, video_id)[0]
-
-        duration = parse_duration(self._search_regex(
-            r'<strong>Runtime:</strong>([^<]+)', webpage, 'duration',
-            default=None))
-        uploader = self._search_regex(
-            r'<strong>Uploaded By:.*?<a[^>]*>([^<]+)', webpage, 'uploader',
-            default=None)
+            formats.append({
+                'asr': int_or_none(q.get('sample_rate')),
+                'filesize': int_or_none(q.get('size')),
+                'format_id': format_id,
+                'fps': int_or_none(q.get('fps')),
+                'height': int_or_none(q.get('height')),
+                'tbr': float_or_none(q.get('bitrate')),
+                'url': play_url,
+                'width': int_or_none(q.get('width')),
+            })
 
-        info_dict.update({
+        author = zvideo.get('author') or {}
+        url_token = author.get('url_token')
+
+        return {
             'id': video_id,
             'title': title,
-            'age_limit': self._rta_search(webpage),
-            'duration': duration,
-            'uploader': uploader,
-        })
-
-        return info_dict
+            'formats': formats,
+            'thumbnail': video.get('thumbnail') or zvideo.get('image_url'),
+            'uploader': author.get('name'),
+            'timestamp': int_or_none(zvideo.get('published_at')),
+            'uploader_id': author.get('id'),
+            'uploader_url': format_field(url_token, None, 'https://www.zhihu.com/people/%s'),
+            'duration': float_or_none(video.get('duration')),
+            'view_count': int_or_none(zvideo.get('play_count')),
+            'like_count': int_or_none(zvideo.get('liked_count')),
+            'comment_count': int_or_none(zvideo.get('comment_count')),
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youku.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youku.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/younow.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/younow.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youporn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yourporn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yourporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/yourupload.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/yourupload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/youtube.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/youtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zaiko.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zaiko.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zapiks.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zapiks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zattoo.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zattoo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zdf.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zdf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zee5.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zee5.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zeenews.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zeenews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zenporn.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zenporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zetland.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zetland.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zingmp3.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zingmp3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zoom.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zoom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/extractor/zype.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/extractor/zype.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_curlcffi.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_curlcffi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_helper.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_helper.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_requests.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_requests.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_urllib.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_urllib.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/_websockets.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/_websockets.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/common.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/exceptions.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/exceptions.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/networking/impersonate.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/networking/impersonate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/__init__.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/common.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/embedthumbnail.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/embedthumbnail.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/exec.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/exec.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/ffmpeg.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/metadataparser.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/metadataparser.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/modify_chapters.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/modify_chapters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/movefilesafterdownload.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/movefilesafterdownload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/sponskrub.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/sponskrub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/sponsorblock.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/sponsorblock.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/postprocessor/xattrpp.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/postprocessor/xattrpp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/_deprecated.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/_legacy.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/_utils.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/networking.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/networking.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/progress.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/progress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/yt_dlp/utils/traversal.py` & `yt_dlp-2024.5.8.232715.dev0/yt_dlp/utils/traversal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/.gitignore` & `yt_dlp-2024.5.8.232715.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/AUTHORS` & `yt_dlp-2024.5.8.232715.dev0/AUTHORS`

 * *Files 0% similar despite different names*

```diff
@@ -767,14 +767,15 @@
 Rafal Borczuch
 Rajeshwaran
 Ralf Haring
 Ralph Drake
 Random User
 Raphael Michel
 Raphaël Droz
+Rasmus Antons
 Rasmus Rendal
 Rastislav Barlik
 Ray Douglass
 RedDeffender
 Reino17
 Remita Amine
 Reto Kromer
```

### Comparing `yt_dlp-2024.5.5.232701.dev0/LICENSE` & `yt_dlp-2024.5.8.232715.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/README.md` & `yt_dlp-2024.5.8.232715.dev0/README.md`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/pyproject.toml` & `yt_dlp-2024.5.8.232715.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.5.5.232701.dev0/PKG-INFO` & `yt_dlp-2024.5.8.232715.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 7974 2d64  : 2.3.Name: yt-d
 00000020: 6c70 0a56 6572 7369 6f6e 3a20 3230 3234  lp.Version: 2024
-00000030: 2e35 2e35 2e32 3332 3730 312e 6465 7630  .5.5.232701.dev0
+00000030: 2e35 2e38 2e32 3332 3731 352e 6465 7630  .5.8.232715.dev0
 00000040: 0a53 756d 6d61 7279 3a20 4120 6665 6174  .Summary: A feat
 00000050: 7572 652d 7269 6368 2063 6f6d 6d61 6e64  ure-rich command
 00000060: 2d6c 696e 6520 6175 6469 6f2f 7669 6465  -line audio/vide
 00000070: 6f20 646f 776e 6c6f 6164 6572 0a50 726f  o downloader.Pro
 00000080: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
 00000090: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
 000000a0: 2f67 6974 6875 622e 636f 6d2f 7974 2d64  /github.com/yt-d
```

