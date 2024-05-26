# Comparing `tmp/swanlab-0.3.3.tar.gz` & `tmp/swanlab-0.3.4.tar.gz`

## Comparing `swanlab-0.3.3.tar` & `swanlab-0.3.4.tar`

### file list

```diff
@@ -1,835 +1,854 @@
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.3/.eslintrc-auto-import.json
--rw-r--r--   0        0        0    28402 2020-02-02 00:00:00.000000 swanlab-0.3.3/README.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.3/jsconfig.json
--rw-r--r--   0        0        0   236829 2020-02-02 00:00:00.000000 swanlab-0.3.3/package-lock.json
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 swanlab-0.3.3/package.json
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.3/.config/copy_frontend.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.3/.vscode/extensions.json
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 swanlab-0.3.3/.vscode/launch.json
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.3/.vscode/settings.json
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.3/.vscode/tailwind.json
--rw-r--r--   0        0        0   218965 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/.package-lock.json
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@alloc/quick-lru/package.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antfu/utils/package.json
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/adjust/package.json
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/adjust/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/attr/package.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/color-util/package.json
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/component/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/component/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/coord/package.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/dom-util/package.json
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/event-emitter/package.json
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-base/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-canvas/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-math/package.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g-svg/package.json
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g2/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/g2plot/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/scale/package.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@antv/util/package.json
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@babel/parser/package.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@esbuild/linux-x64/package.json
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@eslint/eslintrc/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@eslint/js/package.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@eslint-community/eslint-utils/package.json
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@eslint-community/regexpp/package.json
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@headlessui/vue/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@humanwhocodes/config-array/package.json
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@humanwhocodes/module-importer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@humanwhocodes/object-schema/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@intlify/core-base/package.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@intlify/message-compiler/package.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@intlify/shared/package.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@isaacs/cliui/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jest/schemas/package.json
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jridgewell/gen-mapping/package.json
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jridgewell/resolve-uri/package.json
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jridgewell/set-array/package.json
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jridgewell/source-map/package.json
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jridgewell/sourcemap-codec/package.json
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@jridgewell/trace-mapping/package.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@ljharb/resumer/package.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@ljharb/through/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@ljharb/through/tsconfig.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@nodelib/fs.scandir/package.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@nodelib/fs.stat/package.json
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@nodelib/fs.walk/package.json
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@pkgjs/parseargs/package.json
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@rollup/pluginutils/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@rollup/pluginutils/dist/es/package.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@rollup/rollup-linux-x64-gnu/package.json
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@rollup/rollup-linux-x64-musl/package.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@sinclair/typebox/package.json
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@tanstack/virtual-core/package.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@tanstack/vue-virtual/package.json
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@types/d3-timer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@types/estree/package.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@ungap/structured-clone/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@ungap/structured-clone/cjs/package.json
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitejs/plugin-vue/package.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/expect/package.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/runner/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/runner/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/snapshot/package.json
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/spy/package.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/utils/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vitest/utils/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/compiler-core/package.json
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/compiler-dom/package.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/compiler-sfc/package.json
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/compiler-ssr/package.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/devtools-api/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/reactivity/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/runtime-core/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/runtime-dom/package.json
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/server-renderer/package.json
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/@vue/shared/package.json
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/acorn/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/acorn-jsx/package.json
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/acorn-walk/package.json
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ajv/package.json
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ajv/lib/refs/data.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-draft-04.json
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-draft-06.json
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-draft-07.json
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-secure.json
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/align-text/package.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/amdefine/package.json
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/any-promise/package.json
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/anymatch/package.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/arg/package.json
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/argparse/package.json
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/array-buffer-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/array-buffer-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/arraybuffer.prototype.slice/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/assertion-error/package.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/asynckit/package.json
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/autoprefixer/package.json
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/available-typed-arrays/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/available-typed-arrays/tsconfig.json
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/axios/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/balanced-match/package.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/base64-arraybuffer/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/binary-extensions/binary-extensions.json
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/binary-extensions/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/boolbase/package.json
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/braces/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/browserslist/package.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/buffer-from/package.json
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/cac/package.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/call-bind/package.json
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/callsites/package.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/camelcase/package.json
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/camelcase-css/package.json
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/caniuse-lite/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/center-align/package.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/chai/bower.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/chai/package.json
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/chalk/package.json
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/check-error/package.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/chokidar/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/chokidar/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/cliui/package.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/color-convert/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/color-name/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/combined-stream/package.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/commander/package-support.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/commander/package.json
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/concat-map/package.json
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/confbox/package.json
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/contour_plot/package.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/cross-spawn/package.json
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/css-line-break/package.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/cssesc/package.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/csstype/package.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/d3-color/package.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/d3-ease/package.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/d3-hierarchy/package.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/d3-interpolate/package.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/d3-regression/package.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/d3-timer/package.json
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/data-view-buffer/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/data-view-buffer/tsconfig.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/data-view-byte-length/package.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/data-view-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/data-view-byte-offset/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/data-view-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/debug/package.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/decamelize/package.json
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/deep-eql/package.json
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/deep-equal/package.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/deep-is/package.json
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/define-data-property/package.json
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/define-data-property/tsconfig.json
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/define-properties/package.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/defined/package.json
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/delayed-stream/package.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/detect-browser/package.json
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/didyoumean/package.json
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/diff-sequences/package.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/dlv/package.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/doctrine/package.json
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/dotignore/package.json
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eastasianwidth/package.json
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/electron-to-chromium/chromium-versions.json
--rw-r--r--   0        0        0    50337 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/electron-to-chromium/full-chromium-versions.json
--rw-r--r--   0        0        0    78704 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/electron-to-chromium/full-versions.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/electron-to-chromium/package.json
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/electron-to-chromium/versions.json
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/entities/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/entities/lib/esm/package.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-abstract/package.json
--rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-abstract/helpers/caseFolding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-abstract/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-abstract/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-define-property/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-define-property/tsconfig.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-errors/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-errors/tsconfig.json
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-object-atoms/package.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-object-atoms/tsconfig.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-set-tostringtag/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-set-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/es-to-primitive/package.json
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/esbuild/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/escalade/package.json
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint/conf/replacements.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint/conf/rule-type-list.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-config-prettier/package.json
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-prettier/package.json
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/package.json
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
--rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/math-elements.json
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-scope/package.json
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/eslint-visitor-keys/package.json
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/espree/package.json
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/esquery/package.json
--rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/esrecurse/package.json
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/estraverse/package.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/estree-walker/dist/esm/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/estree-walker/src/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/esutils/package.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/execa/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-deep-equal/package.json
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-diff/package.json
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-glob/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-glob/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-json-stable-stringify/package.json
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-json-stable-stringify/benchmark/test.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fast-levenshtein/package.json
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fastq/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fastq/test/tsconfig.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fecha/package.json
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/file-entry-cache/package.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fill-range/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/find-up/package.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/flat-cache/package.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/flatted/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/flatted/cjs/package.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fmin/.eslintrc.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fmin/package.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/follow-redirects/package.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/for-each/package.json
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/foreground-child/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/foreground-child/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/foreground-child/dist/mjs/package.json
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/form-data/package.json
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fraction.js/package.json
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/fs.realpath/package.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/function-bind/package.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/function.prototype.name/package.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/functions-have-names/package.json
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/get-func-name/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/get-intrinsic/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/get-stream/package.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/get-symbol-description/package.json
--rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/mat2/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/mat2d/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/mat3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/mat4/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/quat/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/quat2/package.json
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/types.d.ts/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/vec2/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/vec3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gl-matrix/vec4/package.json
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/glob/package.json
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/globals/globals.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/globals/package.json
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/globalthis/package.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/gopd/package.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/graphemer/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has/package.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-ansi/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-bigints/package.json
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-flag/package.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-property-descriptors/package.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-proto/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-proto/tsconfig.json
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-symbols/package.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-tostringtag/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/has-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/hasown/package.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/hasown/tsconfig.json
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/html2canvas/package.json
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/html2canvas/tsconfig.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/human-signals/package.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/husky/package.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ignore/package.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/immutable/package.json
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/import-fresh/package.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/imurmurhash/package.json
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/inflight/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/inherits/package.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/internal-slot/package.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-arguments/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-bigint/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-binary-path/package.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-boolean-object/package.json
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-buffer/package.json
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-callable/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-core-module/core.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-core-module/package.json
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-data-view/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-data-view/tsconfig.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-date-object/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-extglob/package.json
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-fullwidth-code-point/package.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-glob/package.json
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-negative-zero/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-negative-zero/tsconfig.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-number/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-number-object/package.json
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-path-inside/package.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-regex/package.json
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-shared-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-shared-array-buffer/tsconfig.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-stream/package.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-string/package.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-symbol/package.json
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-typed-array/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-typed-array/tsconfig.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/is-weakref/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/isarray/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/isexe/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/jackspeak/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/jackspeak/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/jackspeak/dist/esm/package.json
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/jiti/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/js-tokens/package.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/js-yaml/package.json
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/json-buffer/package.json
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/json-schema-traverse/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/json-stable-stringify-without-jsonify/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/json2module/package.json
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/json5/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/keyv/package.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/kind-of/package.json
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lazy-cache/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/levn/package.json
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lines-and-columns/package.json
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/locate-path/package.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lodash/package.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lodash-es/package.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lodash.merge/package.json
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/longest/package.json
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/loupe/package.json
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lru-cache/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/lru-cache/dist/esm/package.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/magic-string/package.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/merge-stream/package.json
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/merge2/package.json
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/micromatch/package.json
--rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mime-db/db.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mime-db/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mime-types/package.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mimic-fn/package.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/minimatch/package.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/minimist/package.json
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/minipass/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/minipass/dist/commonjs/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/minipass/dist/esm/package.json
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mlly/package.json
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mock-property/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mockjs/bower.json
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mockjs/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mockjs/test/bower.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mockjs/test/package.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/moment/package.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ms/package.json
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/mz/package.json
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/nanoid/package.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/nanoid/async/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/nanoid/non-secure/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/nanoid/url-alphabet/package.json
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/natural-compare/package.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/node-releases/package.json
--rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/node-releases/data/processed/envs.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/node-releases/data/release-schedule/release-schedule.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/normalize-path/package.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/normalize-range/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/npm-run-path/package.json
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/npm-run-path/node_modules/path-key/package.json
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/nth-check/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/nth-check/lib/esm/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object-assign/package.json
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object-hash/package.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object-is/package.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object-keys/package.json
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/object.assign/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/once/package.json
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/onetime/package.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/optionator/package.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/p-locate/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/parent-module/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-exists/package.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-is-absolute/package.json
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-key/package.json
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-parse/package.json
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-scurry/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-scurry/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/path-scurry/dist/esm/package.json
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pathe/package.json
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pathval/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pdfast/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/picocolors/package.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/picomatch/package.json
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pify/package.json
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pinia/package.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pinia/node_modules/vue-demi/package.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pirates/package.json
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pkg-types/package.json
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/possible-typed-array-names/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/possible-typed-array-names/tsconfig.json
--rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-import/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-js/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-load-config/package.json
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-load-config/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-nested/package.json
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-selector-parser/package.json
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/postcss-value-parser/package.json
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/prelude-ls/package.json
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/prettier/package.json
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/prettier-linter-helpers/package.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/prettier-linter-helpers/.vscode/settings.json
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pretty-format/package.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/pretty-format/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/proxy-from-env/package.json
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/punycode/package.json
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/queue-microtask/package.json
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/react-is/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/read-cache/package.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/readdirp/package.json
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/regexp.prototype.flags/package.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/repeat-string/package.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/lib/core.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/baz/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/browser_field/package.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/dot_main/package.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/dot_slash_main/package.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/false_main/package.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/incorrect_main/package.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/invalid_main/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/multirepo/lerna.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/multirepo/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve/test/resolver/symlinked/package/package.json
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/resolve-from/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/reusify/package.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/right-align/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rimraf/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/node_modules/chalk/package.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rollup/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/run-parallel/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/rw/package.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/safe-array-concat/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/safe-array-concat/tsconfig.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/safe-regex-test/package.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sass/package.json
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/scule/package.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/semver/package.json
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/set-function-length/package.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/set-function-length/tsconfig.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/set-function-name/package.json
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/set-function-name/tsconfig.json
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/shebang-command/package.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/shebang-regex/package.json
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/side-channel/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/side-channel/tsconfig.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/side-channel/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/side-channel/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/siginfo/package.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/signal-exit/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/signal-exit/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/signal-exit/dist/mjs/package.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/size-sensor/package.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/source-map/package.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/source-map-js/package.json
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/stackback/package.json
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/std-env/package.json
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string-width/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string-width/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string-width/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string-width-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string.prototype.trim/package.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string.prototype.trimend/package.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/string.prototype.trimstart/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/strip-ansi-cjs/package.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/strip-final-newline/package.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/strip-json-comments/package.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/strip-literal/package.json
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/commander/package.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/glob/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/glob/dist/esm/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/supports-preserve-symlinks-flag/package.json
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tailwindcss/package.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tailwindcss/stubs/.prettierrc.json
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tape/package.json
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/terser/package.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/terser/bin/package.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/terser/dist/package.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/terser/node_modules/commander/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/terser/node_modules/source-map/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/terser/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/text-segmentation/package.json
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/text-table/package.json
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/thenify/package.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/thenify-all/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tinybench/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tinypool/package.json
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tinyspy/package.json
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tippy.js/package.json
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tippy.js/headless/package.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/to-regex-range/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ts-interface-checker/package.json
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/type-check/package.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/type-detect/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/type-fest/package.json
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-buffer/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-byte-offset/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-length/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/typed-array-length/tsconfig.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/ufo/package.json
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/uglify-js/package.json
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/uglify-js/node_modules/source-map/package.json
--rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/uglify-js/tools/domprops.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/uglify-to-browserify/package.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unbox-primitive/package.json
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unimport/package.json
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unimport/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unimport/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unimport/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin/package.json
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-auto-import/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-vue-components/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/update-browserslist-db/.devcontainer.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/update-browserslist-db/package.json
--rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/uri-js/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/util-deprecate/package.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/utrie/package.json
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vite/package.json
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vite/node_modules/rollup/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vite/node_modules/rollup/dist/es/package.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vite/types/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vite-node/package.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vite-plugin-json5/package.json
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vitest/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vitest/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vitest/node_modules/strip-literal/package.json
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue/compiler-sfc/package.json
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue/jsx-runtime/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue/server-renderer/package.json
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-eslint-parser/package.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-i18n/package.json
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-i18n/vetur/attributes.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-i18n/vetur/tags.json
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-router/package.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-router/vetur/attributes.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-router/vetur/tags.json
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-tippy/package.json
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-tippy/tsconfig.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-tippy/vetur/attributes.json
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/vue-tippy/vetur/tags.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/webpack-sources/package.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/webpack-virtual-modules/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/which/package.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/which-boxed-primitive/package.json
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/which-typed-array/package.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/which-typed-array/tsconfig.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/why-is-node-running/package.json
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/window-size/package.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/word-wrap/package.json
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wordwrap/package.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/wrappy/package.json
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/xml-name-validator/package.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/yaml/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/yaml/browser/package.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/yargs/package.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.3/node_modules/yocto-queue/package.json
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/__init__.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/env.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/error.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/package.json
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/package.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/cos.py
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/http.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/info.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/auth/__init__.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/auth/login.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/upload/__init__.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/api/upload/model.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cli/__init__.py
--rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cli/main.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cli/utils.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/__init__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/_log_collector.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/start_thread.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/task_types.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/utils.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/dog/README.md
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/dog/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/dog/log_sniffer.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/dog/metadata_handle.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/cloud/dog/sniffer_queue.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/compat/README.md
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/compat/server/controller/experiment.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/converter/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/converter/tfb/__init__.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/converter/tfb/_utils.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/converter/tfb/tfb_converter.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/converter/wb/__init__.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/converter/wb/wb_converter.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/__init__.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/callback_cloud.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/callback_local.py
--rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/config.py
--rw-r--r--   0        0        0    13459 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/sdk.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/settings.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/_utils.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/audio.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/base.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/chart.py
--rw-r--r--   0        0        0    13848 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/image.py
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/object_3d.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/text.py
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/video.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/utils_modules/__init__.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/utils_modules/bounding_boxes.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/modules/utils_modules/image_mask.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/run/__init__.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/run/callback.py
--rw-r--r--   0        0        0    18197 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/run/exp.py
--rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/run/main.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/system/__init__.py
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/system/info.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/system/monitor.py
--rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/data/system/bin/apple_gpu_stats
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/__init__.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/db_connect.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/error.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/model.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/table_config.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/docs/Errors.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/docs/README.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/migrate/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/migrate/chart.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/migrate/experiment.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/migrate/namespace.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/migrate/project.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/migrate/tag.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/__init__.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/charts.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/displays.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/experiments.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/namespaces.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/projects.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/sources.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/models/tags.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/utils/__init__.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/db/utils/chart.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/fastai.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/huggingface.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/mmengine.py
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/pytorch_lightning.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/ultralytics.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/integration_utils/autologging.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/integration_utils/get_modules.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/integration_utils/timer.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/openai/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/openai/openai.py
--rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/openai/resolver.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/zhipuai/__init__.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/zhipuai/resolver.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/integration/zhipuai/zhipuai.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/log/__init__.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/log/console.py
--rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/log/log.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/app.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/settings.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/chart.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/db.py
--rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/experiment.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/namespace.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/project.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/utils/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/utils/charts.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/controller/utils/tag.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/middleware/common.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/module/__init__.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/module/resp.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/router/chart.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/router/experiment.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/router/media.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/router/namespace.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/server/router/project.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/index.html
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/ChartPage-C2Rj7xI3.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/ChartPage-DgOOkrVh.css
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/ChartsView-DpI6U3QH.js
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvHardware-4H7mp2Bs.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvIndex-B5_l1b65.js
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvItems-B4PwmQT4.js
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvItems-BfjcRO-X.css
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/ExperimentView-BTbu21ka.js
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/ExperimentView-CCDMXo4h.css
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/FuncBar-Ct_nBdvU.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/FuncBar-DgVTuZfd.css
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/HelpView-C4wSXY1I.js
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/HomeView-BS7FyMAt.css
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/HomeView-BqTu9_fG.js
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/IndexPage-C5dvtib2.css
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/IndexPage-CrqN4Ekl.js
--rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/LogPage-B-fC6sB7.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/LogPage-DBzoauOW.css
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/NotFound-DijsQ96i.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/SLLoading-6DfF2aH0.js
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js
--rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/chart-DB312WPs.css
--rw-r--r--   0        0        0  1098521 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/chart-eW1meEc1.js
--rw-r--r--   0        0        0   393892 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/index-B5SDzoY4.js
--rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/index-B7Izi8NT.css
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/template/assets/logo-ChHf2ozk.ico
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/utils/__init__.py
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/utils/file.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/utils/font.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/utils/judgment.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/utils/key.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.3/swanlab/utils/time.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/create_error_chart.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/create_experiment.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/start_server.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/use_swanlog.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/config/config.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/config/load.yaml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/conftest.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/pytest_example.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/auth/pytest_login.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/data/pytest_sdk.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/data/run/pytest_main.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/log/pytest_log.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/server/controller/utils/utils.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/utils/pytest_file.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/utils/pytest_key.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.3/test/unit/utils/pytest_package.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 swanlab-0.3.3/.gitignore
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.3/LICENSE
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    30539 2020-02-02 00:00:00.000000 swanlab-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.4/.eslintrc-auto-import.json
+-rw-r--r--   0        0        0    28875 2020-02-02 00:00:00.000000 swanlab-0.3.4/README.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.4/jsconfig.json
+-rw-r--r--   0        0        0   236753 2020-02-02 00:00:00.000000 swanlab-0.3.4/package-lock.json
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 swanlab-0.3.4/package.json
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.4/.config/copy_frontend.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/extensions.json
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/launch.json
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/settings.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.4/.vscode/tailwind.json
+-rw-r--r--   0        0        0   218889 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/.package-lock.json
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@alloc/quick-lru/package.json
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antfu/utils/package.json
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/package.json
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/attr/package.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/color-util/package.json
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/component/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/coord/package.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/dom-util/package.json
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/event-emitter/package.json
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-base/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-canvas/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-math/package.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g-svg/package.json
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/g2plot/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/scale/package.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@antv/util/package.json
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@babel/parser/package.json
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@esbuild/linux-x64/package.json
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint/eslintrc/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint/js/package.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint-community/eslint-utils/package.json
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@eslint-community/regexpp/package.json
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@headlessui/vue/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@humanwhocodes/config-array/package.json
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@humanwhocodes/module-importer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@humanwhocodes/object-schema/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@intlify/core-base/package.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@intlify/message-compiler/package.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@intlify/shared/package.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@isaacs/cliui/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jest/schemas/package.json
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/gen-mapping/package.json
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/resolve-uri/package.json
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/set-array/package.json
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/source-map/package.json
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/sourcemap-codec/package.json
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@jridgewell/trace-mapping/package.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ljharb/resumer/package.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ljharb/through/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ljharb/through/tsconfig.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@nodelib/fs.scandir/package.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@nodelib/fs.stat/package.json
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@nodelib/fs.walk/package.json
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@pkgjs/parseargs/package.json
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@popperjs/core/package.json
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/pluginutils/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/pluginutils/dist/es/package.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/rollup-linux-x64-gnu/package.json
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@rollup/rollup-linux-x64-musl/package.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@sinclair/typebox/package.json
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@tanstack/virtual-core/package.json
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@tanstack/vue-virtual/package.json
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@types/d3-timer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@types/estree/package.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ungap/structured-clone/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@ungap/structured-clone/cjs/package.json
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitejs/plugin-vue/package.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/expect/package.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/runner/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/runner/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/snapshot/package.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/spy/package.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/utils/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vitest/utils/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-core/package.json
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-dom/package.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/compiler-ssr/package.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/devtools-api/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/reactivity/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/runtime-core/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/runtime-dom/package.json
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/server-renderer/package.json
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/@vue/shared/package.json
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/acorn/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/acorn-jsx/package.json
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/acorn-walk/package.json
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/package.json
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/data.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-04.json
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-06.json
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-07.json
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-secure.json
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/align-text/package.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/amdefine/package.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/any-promise/package.json
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/anymatch/package.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/arg/package.json
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/argparse/package.json
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/array-buffer-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/array-buffer-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/arraybuffer.prototype.slice/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/assertion-error/package.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/asynckit/package.json
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/autoprefixer/package.json
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/available-typed-arrays/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/available-typed-arrays/tsconfig.json
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/axios/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/balanced-match/package.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/base64-arraybuffer/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/binary-extensions/binary-extensions.json
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/binary-extensions/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/boolbase/package.json
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/braces/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/browserslist/package.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/buffer-from/package.json
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cac/package.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/call-bind/package.json
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/callsites/package.json
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/camelcase/package.json
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/camelcase-css/package.json
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/caniuse-lite/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/center-align/package.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chai/bower.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chai/package.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chalk/package.json
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/check-error/package.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chokidar/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/chokidar/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cliui/package.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/color-convert/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/color-name/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/combined-stream/package.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/commander/package-support.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/commander/package.json
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/concat-map/package.json
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/confbox/package.json
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/contour_plot/package.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cross-spawn/package.json
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/css-line-break/package.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/cssesc/package.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/csstype/package.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-color/package.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-ease/package.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-hierarchy/package.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-interpolate/package.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-regression/package.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/d3-timer/package.json
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-buffer/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-length/package.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-offset/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/data-view-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/debug/package.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/decamelize/package.json
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/deep-eql/package.json
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/deep-equal/package.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/deep-is/package.json
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/define-data-property/package.json
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/define-data-property/tsconfig.json
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/define-properties/package.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/defined/package.json
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/delayed-stream/package.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/detect-browser/package.json
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/didyoumean/package.json
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/diff-sequences/package.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/dlv/package.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/doctrine/package.json
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/dotignore/package.json
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eastasianwidth/package.json
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/chromium-versions.json
+-rw-r--r--   0        0        0    50514 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/full-chromium-versions.json
+-rw-r--r--   0        0        0    78988 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/full-versions.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/package.json
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/electron-to-chromium/versions.json
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/entities/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/entities/lib/esm/package.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/package.json
+-rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/helpers/caseFolding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-abstract/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-define-property/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-define-property/tsconfig.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-errors/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-errors/tsconfig.json
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-object-atoms/package.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-object-atoms/tsconfig.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-set-tostringtag/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-set-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/es-to-primitive/package.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esbuild/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/escalade/package.json
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/conf/replacements.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/conf/rule-type-list.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-config-prettier/package.json
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-prettier/package.json
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/package.json
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
+-rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/math-elements.json
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-scope/package.json
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/eslint-visitor-keys/package.json
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/espree/package.json
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esquery/package.json
+-rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esrecurse/package.json
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estraverse/package.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estree-walker/dist/esm/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/estree-walker/src/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/esutils/package.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/execa/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-deep-equal/package.json
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-diff/package.json
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-glob/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-glob/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-json-stable-stringify/package.json
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-json-stable-stringify/benchmark/test.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fast-levenshtein/package.json
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fastq/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fastq/test/tsconfig.json
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fecha/package.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/file-entry-cache/package.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fill-range/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/find-up/package.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/flat-cache/package.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/flatted/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/flatted/cjs/package.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fmin/.eslintrc.json
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fmin/package.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/follow-redirects/package.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/for-each/package.json
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/foreground-child/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/foreground-child/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/foreground-child/dist/mjs/package.json
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/form-data/package.json
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fraction.js/package.json
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/fs.realpath/package.json
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/function.prototype.name/package.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/functions-have-names/package.json
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-func-name/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-stream/package.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/get-symbol-description/package.json
+-rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat2/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat2d/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/mat4/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/quat/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/quat2/package.json
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/types.d.ts/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/vec2/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/vec3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gl-matrix/vec4/package.json
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/glob/package.json
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/globals/globals.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/globals/package.json
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/globalthis/package.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/gopd/package.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/graphemer/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has/package.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-ansi/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-bigints/package.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-flag/package.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-proto/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-proto/tsconfig.json
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-tostringtag/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/has-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/hasown/package.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/hasown/tsconfig.json
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/html2canvas/package.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/html2canvas/tsconfig.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/human-signals/package.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/husky/package.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ignore/package.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/immutable/package.json
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/import-fresh/package.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/imurmurhash/package.json
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/inflight/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/inherits/package.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/internal-slot/package.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-arguments/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-bigint/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-binary-path/package.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-boolean-object/package.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-buffer/package.json
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-callable/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-core-module/core.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-core-module/package.json
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-data-view/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-data-view/tsconfig.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-date-object/package.json
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-extglob/package.json
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-fullwidth-code-point/package.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-glob/package.json
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-negative-zero/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-negative-zero/tsconfig.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-number/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-number-object/package.json
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-path-inside/package.json
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-regex/package.json
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-shared-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-shared-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-stream/package.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-string/package.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-symbol/package.json
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-typed-array/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-typed-array/tsconfig.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/is-weakref/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/isarray/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/isexe/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jackspeak/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jackspeak/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jackspeak/dist/esm/package.json
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/jiti/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/js-tokens/package.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/js-yaml/package.json
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json-buffer/package.json
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json-schema-traverse/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json-stable-stringify-without-jsonify/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json2module/package.json
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/json5/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/keyv/package.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/kind-of/package.json
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lazy-cache/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/levn/package.json
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lines-and-columns/package.json
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/locate-path/package.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lodash/package.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lodash-es/package.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lodash.merge/package.json
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/longest/package.json
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/loupe/package.json
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lru-cache/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/lru-cache/dist/esm/package.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/magic-string/package.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/merge-stream/package.json
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/merge2/package.json
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/micromatch/package.json
+-rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mime-db/db.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mime-db/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mime-types/package.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mimic-fn/package.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minimist/package.json
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minipass/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minipass/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/minipass/dist/esm/package.json
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mlly/package.json
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mock-property/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/bower.json
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/test/bower.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mockjs/test/package.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/moment/package.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ms/package.json
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/mz/package.json
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/package.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/async/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/non-secure/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nanoid/url-alphabet/package.json
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/natural-compare/package.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/node-releases/package.json
+-rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/node-releases/data/processed/envs.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/node-releases/data/release-schedule/release-schedule.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/normalize-path/package.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/normalize-range/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/npm-run-path/package.json
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/npm-run-path/node_modules/path-key/package.json
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nth-check/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/nth-check/lib/esm/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-assign/package.json
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-hash/package.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-is/package.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object-keys/package.json
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/object.assign/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/once/package.json
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/onetime/package.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/optionator/package.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/p-locate/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/parent-module/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-exists/package.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-is-absolute/package.json
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-key/package.json
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-parse/package.json
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-scurry/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-scurry/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/path-scurry/dist/esm/package.json
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pathe/package.json
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pathval/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pdfast/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/picocolors/package.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/picomatch/package.json
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pify/package.json
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pinia/package.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pinia/node_modules/vue-demi/package.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pirates/package.json
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pkg-types/package.json
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/possible-typed-array-names/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/possible-typed-array-names/tsconfig.json
+-rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-import/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-js/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-load-config/package.json
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-load-config/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-nested/package.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-selector-parser/package.json
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/postcss-value-parser/package.json
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prelude-ls/package.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prettier/package.json
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prettier-linter-helpers/package.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/prettier-linter-helpers/.vscode/settings.json
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pretty-format/package.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/pretty-format/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/proxy-from-env/package.json
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/punycode/package.json
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/queue-microtask/package.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/react-is/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/read-cache/package.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/readdirp/package.json
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/regexp.prototype.flags/package.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/repeat-string/package.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/lib/core.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/baz/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/browser_field/package.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/dot_main/package.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/dot_slash_main/package.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/false_main/package.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/incorrect_main/package.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/invalid_main/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/lerna.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve/test/resolver/symlinked/package/package.json
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/resolve-from/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/reusify/package.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/right-align/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rimraf/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/chalk/package.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rollup/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/run-parallel/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/rw/package.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/safe-array-concat/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/safe-array-concat/tsconfig.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/safe-regex-test/package.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sass/package.json
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/scule/package.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/semver/package.json
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-length/package.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-length/tsconfig.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-name/package.json
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/set-function-name/tsconfig.json
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/shebang-command/package.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/shebang-regex/package.json
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/tsconfig.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/side-channel/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/siginfo/package.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/signal-exit/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/signal-exit/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/signal-exit/dist/mjs/package.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/size-sensor/package.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/source-map/package.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/source-map-js/package.json
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/stackback/package.json
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/std-env/package.json
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string.prototype.trim/package.json
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string.prototype.trimend/package.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/string.prototype.trimstart/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-ansi-cjs/package.json
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-final-newline/package.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-json-comments/package.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/strip-literal/package.json
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/glob/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/glob/dist/esm/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/supports-preserve-symlinks-flag/package.json
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tailwindcss/package.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tailwindcss/stubs/.prettierrc.json
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tape/package.json
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/package.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/bin/package.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/dist/package.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/node_modules/source-map/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/terser/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/text-segmentation/package.json
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/text-table/package.json
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/thenify/package.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/thenify-all/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tinybench/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tinypool/package.json
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tinyspy/package.json
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tippy.js/package.json
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tippy.js/headless/package.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/to-regex-range/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ts-interface-checker/package.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/type-check/package.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/type-detect/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/type-fest/package.json
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-buffer/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-offset/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-length/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/typed-array-length/tsconfig.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/ufo/package.json
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-js/package.json
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-js/node_modules/source-map/package.json
+-rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-js/tools/domprops.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uglify-to-browserify/package.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unbox-primitive/package.json
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/package.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unimport/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin/package.json
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/update-browserslist-db/.devcontainer.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/update-browserslist-db/package.json
+-rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/uri-js/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/util-deprecate/package.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/utrie/package.json
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/package.json
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/node_modules/rollup/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/node_modules/rollup/dist/es/package.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite/types/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite-node/package.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vite-plugin-json5/package.json
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vitest/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vitest/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/jsx-runtime/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue/server-renderer/package.json
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-eslint-parser/package.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-i18n/package.json
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-i18n/vetur/attributes.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-i18n/vetur/tags.json
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-router/package.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-router/vetur/attributes.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-router/vetur/tags.json
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/package.json
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/tsconfig.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/vetur/attributes.json
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/vue-tippy/vetur/tags.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/webpack-sources/package.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/webpack-virtual-modules/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which/package.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which-boxed-primitive/package.json
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which-typed-array/package.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/which-typed-array/tsconfig.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/why-is-node-running/package.json
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/window-size/package.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/word-wrap/package.json
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wordwrap/package.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/wrappy/package.json
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/xml-name-validator/package.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yaml/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yaml/browser/package.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yargs/package.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.4/node_modules/yocto-queue/package.json
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/__init__.py
+-rw-r--r--   0        0        0     9852 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/env.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/error.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/package.json
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/package.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/cos.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/http.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/info.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/auth/__init__.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/auth/login.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/upload/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/api/upload/model.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cli/__init__.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cli/main.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cli/utils.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/__init__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/_log_collector.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/start_thread.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/task_types.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/utils.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/README.md
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/log_sniffer.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/metadata_handle.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/cloud/dog/sniffer_queue.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/compat/README.md
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/compat/server/controller/experiment.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/tfb/__init__.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/tfb/_utils.py
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/tfb/tfb_converter.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/wb/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/converter/wb/wb_converter.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/__init__.py
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/callback_cloud.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/callback_local.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/config.py
+-rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/sdk.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/settings.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/_utils.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/audio.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/base.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/chart.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/image.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/object_3d.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/text.py
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/video.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/utils_modules/__init__.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/utils_modules/bounding_boxes.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/modules/utils_modules/image_mask.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/__init__.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/callback.py
+-rw-r--r--   0        0        0    16930 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/exp.py
+-rw-r--r--   0        0        0    13553 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/main.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/run/operator.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/__init__.py
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/info.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/monitor.py
+-rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/data/system/bin/apple_gpu_stats
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/__init__.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/callback.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/db_connect.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/error.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/model.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/table_config.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/docs/Errors.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/docs/README.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/chart.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/experiment.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/namespace.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/project.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/migrate/tag.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/__init__.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/charts.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/displays.py
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/experiments.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/namespaces.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/projects.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/sources.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/models/tags.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/utils/__init__.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/db/utils/chart.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/fastai.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/huggingface.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/mmengine.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/pytorch_lightning.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/sb3.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/ultralytics.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/integration_utils/autologging.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/integration_utils/get_modules.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/integration_utils/timer.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/openai/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/openai/openai.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/openai/resolver.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/zhipuai/__init__.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/zhipuai/resolver.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/integration/zhipuai/zhipuai.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/log/__init__.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/log/console.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/log/log.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/app.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/settings.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/chart.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/db.py
+-rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/experiment.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/namespace.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/project.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/utils/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/utils/charts.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/controller/utils/tag.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/middleware/common.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/module/__init__.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/module/resp.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/chart.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/experiment.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/media.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/namespace.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/server/router/project.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/index.html
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ChartPage-C2Rj7xI3.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ChartPage-DgOOkrVh.css
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ChartsView-DpI6U3QH.js
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvHardware-4H7mp2Bs.js
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvIndex-B5_l1b65.js
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvItems-B4PwmQT4.js
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvItems-BfjcRO-X.css
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ExperimentView-BTbu21ka.js
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/ExperimentView-CCDMXo4h.css
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/FuncBar-Ct_nBdvU.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/FuncBar-DgVTuZfd.css
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/HelpView-C4wSXY1I.js
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/HomeView-BS7FyMAt.css
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/HomeView-BqTu9_fG.js
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/IndexPage-C5dvtib2.css
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/IndexPage-CrqN4Ekl.js
+-rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/LogPage-B-fC6sB7.js
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/LogPage-DBzoauOW.css
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/NotFound-DijsQ96i.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SLLoading-6DfF2aH0.js
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js
+-rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
+-rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/chart-DB312WPs.css
+-rw-r--r--   0        0        0  1098521 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/chart-eW1meEc1.js
+-rw-r--r--   0        0        0   393892 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/index-B5SDzoY4.js
+-rw-r--r--   0        0        0    37013 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/index-B7Izi8NT.css
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/template/assets/logo-ChHf2ozk.ico
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/__init__.py
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/file.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/font.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/judgment.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/key.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.4/swanlab/utils/time.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/create_error_chart.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/create_experiment.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/start_server.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/use_swanlog.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/config/config.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/config/load.yaml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/.gitignore
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/fastai/fastai_train.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/fastai/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/huggingface/requirements.txt
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/huggingface/transformers_bert_train.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/lightning/lightning_base.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/lightning/lightning_train.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/lightning/requirements.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/sb3/requirements.txt
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/sb3/sb3_PPO.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/requirements.txt
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_classifer.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_detection.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_pose.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/integration/ultralytics/ultralytics_segmentation.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/pytest_env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/pytest_example.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/auth/pytest_login.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/data/pytest_sdk.py
+-rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/data/run/pytest_main.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/log/pytest_log.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/server/controller/utils/utils.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/utils/pytest_file.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/utils/pytest_key.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.4/test/unit/utils/pytest_package.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swanlab-0.3.4/.gitignore
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.4/LICENSE
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    31012 2020-02-02 00:00:00.000000 swanlab-0.3.4/PKG-INFO
```

### Comparing `swanlab-0.3.3/.eslintrc-auto-import.json` & `swanlab-0.3.4/.eslintrc-auto-import.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/README.md` & `swanlab-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,15 @@
 
 - Flexible recording of hyperparameters and experiment configurations.
 - **Supported metadata types**: scalar metrics, images, audio, text, etc.
 - **Supported chart types**: line graphs, media charts (images, audio, text), etc.
 - **Automatic logging**: console logging, GPU hardware, Git information, Python interpreter, list of Python libraries,
   code directory.
 
-**2. ⚡️ Comprehensive Framework Integration**: PyTorch, TensorFlow, PyTorch Lightning, 🤗HuggingFace Transformers, Tensorboard, 
-MMEngine, OpenAI, ZhipuAI, Hydra, etc.
+**2. ⚡️ Comprehensive Framework Integration**: PyTorch、Tensorflow、PyTorch Lightning、🤗HuggingFace、Transformers、MMEngine、Ultralytics、fastai、Tensorboard、OpenAI、ZhipuAI、Hydra、...
 
 **3. 📦 Organizing Experiments**: Centralized dashboard for efficiently managing multiple projects and experiments,
 providing an overview of training at a glance.
 
 **4. 🆚 Comparing Results**: Use online tables and paired charts to compare the hyperparameters and outcomes of different
 experiments, developing iterative inspiration.
 
@@ -689,14 +688,15 @@
 
 </details>
 
 <details>
 <summary>
   <strong> MMEngine(MMDetection etc.)</strong>
 </summary>
+<br>
 
 Integrate `SwanlabVisBackend` into MMEngine to enable automatic logging of training metrics by SwanLab.
 
 Add the following code snippet to your MM config file to start training:
 
 ```python
 custom_imports = dict(imports=["swanlab.integration.mmengine"], allow_failed_imports=False)
@@ -714,14 +714,40 @@
 visualizer = dict(
     type="Visualizer",
     vis_backends=vis_backends,
 )
 ```
 </details>
 
+<details>
+<summary>
+  <strong> Ultralytics</strong>
+</summary>
+<br>
+
+Integrating SwanLab into Ultralytics is very simple; you can use the `add_swanlab_callback` function:
+
+```python
+from ultralytics import YOLO
+from swanlab.integration.ultralytics import add_swanlab_callback
+
+model = YOLO("yolov8n.yaml")
+model.load()
+
+add_swanlab_callback(model)
+
+model.train(
+    data="./coco.yaml",
+    epochs=50, 
+    imgsz=320,
+)
+```
+
+</details>
+
 
 
 <br>
 
 ## 🆚 Comparison with familiar tools
 
 ### Tensorboard vs SwanLab
```

### Comparing `swanlab-0.3.3/package-lock.json` & `swanlab-0.3.4/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995711269072405%*

 * *Differences: {"'packages'": "{'node_modules/@babel/parser': {'version': '7.24.6', 'resolved': "*

 * *               "'https://registry.npmjs.org/@babel/parser/-/parser-7.24.6.tgz', 'integrity': "*

 * *               "'sha512-eNZXdfU35nJC2h24RznROuOpO94h6x8sg9ju0tT9biNtLZ2vuP8SduLqqV+/8+cebSLV9SJEAN5Z3zQbJG/M+Q=='}, "*

 * *               "'node_modules/electron-to-chromium': {'version': '1.4.783', 'resolved': "*

 * *               "'https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.783.tgz', "*

 * *               "'integ […]*

```diff
@@ -351,17 +351,17 @@
         "node_modules/@babel/parser": {
             "bin": {
                 "parser": "bin/babel-parser.js"
             },
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg==",
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.5.tgz",
-            "version": "7.24.5"
+            "integrity": "sha512-eNZXdfU35nJC2h24RznROuOpO94h6x8sg9ju0tT9biNtLZ2vuP8SduLqqV+/8+cebSLV9SJEAN5Z3zQbJG/M+Q==",
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.6.tgz",
+            "version": "7.24.6"
         },
         "node_modules/@esbuild/aix-ppc64": {
             "cpu": [
                 "ppc64"
             ],
             "dev": true,
             "engines": {
@@ -2381,17 +2381,17 @@
             "dev": true,
             "integrity": "sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==",
             "resolved": "https://registry.npmjs.org/eastasianwidth/-/eastasianwidth-0.2.0.tgz",
             "version": "0.2.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-n02NCwLJ3wexLfK/yQeqfywCblZqLcXphzmid5e8yVPdtEcida7li0A5WQKghHNG0FeOMCzeFOzEbtAh5riXFw==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.777.tgz",
-            "version": "1.4.777"
+            "integrity": "sha512-bT0jEz/Xz1fahQpbZ1D7LgmPYZ3iHVY39NcWWro1+hA2IvjiPeaXtfSqrQ+nXjApMvQRE2ASt1itSLRrebHMRQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.783.tgz",
+            "version": "1.4.783"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-9.2.2.tgz",
             "version": "9.2.2"
         },
@@ -3138,14 +3138,15 @@
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
                 "minimatch": "^3.1.1",
                 "once": "^1.3.0",
                 "path-is-absolute": "^1.0.0"
             },
+            "deprecated": "Glob versions prior to v9 are no longer supported",
             "engines": {
                 "node": "*"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==",
@@ -3389,14 +3390,15 @@
             "version": "0.1.4"
         },
         "node_modules/inflight": {
             "dependencies": {
                 "once": "^1.3.0",
                 "wrappy": "1"
             },
+            "deprecated": "This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.",
             "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
             "resolved": "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz",
             "version": "1.0.6"
         },
         "node_modules/inherits": {
             "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
             "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
@@ -4011,17 +4013,17 @@
             "version": "1.2.8"
         },
         "node_modules/minipass": {
             "dev": true,
             "engines": {
                 "node": ">=16 || 14 >=14.17"
             },
-            "integrity": "sha512-UZ7eQ+h8ywIRAW1hIEl2AqdwzJucU/Kp59+8kkZeSvafXhZjul247BvIJjEVFVeON6d7lM46XX1HXCduKAS8VA==",
-            "resolved": "https://registry.npmjs.org/minipass/-/minipass-7.1.1.tgz",
-            "version": "7.1.1"
+            "integrity": "sha512-qOOzS1cBTWYF4BH8fVePDBOO9iptMnGUEZwNc/cMWnTV2nVLZ7VoNWEPHkYczZA0pdoA7dl6e7FL659nX9S2aw==",
+            "resolved": "https://registry.npmjs.org/minipass/-/minipass-7.1.2.tgz",
+            "version": "7.1.2"
         },
         "node_modules/mlly": {
             "dependencies": {
                 "acorn": "^8.11.3",
                 "pathe": "^1.1.2",
                 "pkg-types": "^1.1.0",
                 "ufo": "^1.5.3"
@@ -4624,17 +4626,17 @@
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-A0RVJrX+IUkVZbW3ClroRWurercFhieevHB38sr2+l9eUClMqome3LmEmnhlNy+5Mr2EYN6B2Kaw9wYdd+VHiw==",
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.16.tgz",
-            "version": "6.0.16"
+            "integrity": "sha512-UMz42UD0UY0EApS0ZL9o1XnLhSTtvvvLe5Dc2H2O56fvRZi+KulDyf5ctDhhtYJBGKStV2FL1fy6253cmLgqVQ==",
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.1.0.tgz",
+            "version": "6.1.0"
         },
         "node_modules/postcss-value-parser": {
             "dev": true,
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
@@ -4834,14 +4836,15 @@
         "node_modules/rimraf": {
             "bin": {
                 "rimraf": "bin.js"
             },
             "dependencies": {
                 "glob": "^7.1.3"
             },
+            "deprecated": "Rimraf versions prior to v4 are no longer supported",
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==",
             "resolved": "https://registry.npmjs.org/rimraf/-/rimraf-3.0.2.tgz",
             "version": "3.0.2"
@@ -5308,23 +5311,23 @@
             },
             "integrity": "sha512-6fPc+R4ihwqP6N/aIv2f1gMH8lOVtWQHoqC4yK6oSDVVocumAsfCqjkXnqiYMhmMwS/mEHLp7Vehlt3ql6lEig==",
             "resolved": "https://registry.npmjs.org/strip-json-comments/-/strip-json-comments-3.1.1.tgz",
             "version": "3.1.1"
         },
         "node_modules/strip-literal": {
             "dependencies": {
-                "acorn": "^8.10.0"
+                "js-tokens": "^9.0.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/antfu"
             },
-            "integrity": "sha512-PugKzOsyXpArk0yWmUwqOZecSO0GH0bPoctLcqNDH9J04pVW3lflYE0ujElBGTloevcxF5MofAOZ7C5l2b+wLg==",
-            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-1.3.0.tgz",
-            "version": "1.3.0"
+            "integrity": "sha512-Op+UycaUt/8FbN/Z2TWPBLge3jWrP3xj10f3fnYxf052bKuS3EKs1ZQcVGjnEMdsNVAM+plXRdmjrZ/KgG3Skw==",
+            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-2.1.0.tgz",
+            "version": "2.1.0"
         },
         "node_modules/sucrase": {
             "bin": {
                 "sucrase": "bin/sucrase",
                 "sucrase-node": "bin/sucrase-node"
             },
             "dependencies": {
@@ -5365,28 +5368,28 @@
         "node_modules/sucrase/node_modules/glob": {
             "bin": {
                 "glob": "dist/esm/bin.mjs"
             },
             "dependencies": {
                 "foreground-child": "^3.1.0",
                 "jackspeak": "^3.1.2",
-                "minimatch": "^9.0.1",
-                "minipass": "^7.0.4",
-                "path-scurry": "^1.11.0"
+                "minimatch": "^9.0.4",
+                "minipass": "^7.1.2",
+                "path-scurry": "^1.11.1"
             },
             "dev": true,
             "engines": {
                 "node": ">=16 || 14 >=14.18"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
-            "integrity": "sha512-JDKXl1DiuuHJ6fVS2FXjownaavciiHNUU4mOvV/B793RLh05vZL1rcPnCSaOgv1hDT6RDlY7AB7ZUvFYAtPgAw==",
-            "resolved": "https://registry.npmjs.org/glob/-/glob-10.3.16.tgz",
-            "version": "10.3.16"
+            "integrity": "sha512-2jelhlq3E4ho74ZyVLN03oKdAZVUa6UDZzFLVH1H7dnoax+y9qyaq8zBkfDIggjniU19z0wU18y16jMB2eyVIw==",
+            "resolved": "https://registry.npmjs.org/glob/-/glob-10.4.1.tgz",
+            "version": "10.4.1"
         },
         "node_modules/sucrase/node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -5769,31 +5772,31 @@
             "integrity": "sha512-61pPlCD9h51VoreyJ0BReideM3MDKMKnh6+V9L08331ipq6Q8OFXZYiqP6n/tbHx4s5I9uRhcye6BrbkizkBDw==",
             "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/unimport": {
             "dependencies": {
                 "@rollup/pluginutils": "^5.1.0",
-                "acorn": "^8.11.2",
+                "acorn": "^8.11.3",
                 "escape-string-regexp": "^5.0.0",
                 "estree-walker": "^3.0.3",
                 "fast-glob": "^3.3.2",
                 "local-pkg": "^0.5.0",
-                "magic-string": "^0.30.5",
-                "mlly": "^1.4.2",
-                "pathe": "^1.1.1",
-                "pkg-types": "^1.0.3",
-                "scule": "^1.1.1",
-                "strip-literal": "^1.3.0",
-                "unplugin": "^1.5.1"
+                "magic-string": "^0.30.10",
+                "mlly": "^1.7.0",
+                "pathe": "^1.1.2",
+                "pkg-types": "^1.1.1",
+                "scule": "^1.3.0",
+                "strip-literal": "^2.1.0",
+                "unplugin": "^1.10.1"
             },
             "dev": true,
-            "integrity": "sha512-V9HpXYfsZye5bPPYUgs0Otn3ODS1mDUciaBlXljI4C2fTwfFpvFZRywmlOu943puN9sncxROMZhsZCjNXEpzEQ==",
-            "resolved": "https://registry.npmjs.org/unimport/-/unimport-3.7.1.tgz",
-            "version": "3.7.1"
+            "integrity": "sha512-91mxcZTadgXyj3lFWmrGT8GyoRHWuE5fqPOjg5RVtF6vj+OfM5G6WCzXjuYtSgELE5ggB34RY4oiCSEP8I3AHw==",
+            "resolved": "https://registry.npmjs.org/unimport/-/unimport-3.7.2.tgz",
+            "version": "3.7.2"
         },
         "node_modules/unimport/node_modules/escape-string-regexp": {
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "funding": {
@@ -6216,26 +6219,14 @@
             "funding": {
                 "url": "https://github.com/sponsors/antfu"
             },
             "integrity": "sha512-ok6z3qlYyCDS4ZEU27HaU6x/xZa9Whf8jD4ptH5UZTQYZVYeb9bnZ3ojVhiJNLiXK1Hfc0GNbLXcmZ5plLDDBg==",
             "resolved": "https://registry.npmjs.org/local-pkg/-/local-pkg-0.5.0.tgz",
             "version": "0.5.0"
         },
-        "node_modules/vitest/node_modules/strip-literal": {
-            "dependencies": {
-                "js-tokens": "^9.0.0"
-            },
-            "dev": true,
-            "funding": {
-                "url": "https://github.com/sponsors/antfu"
-            },
-            "integrity": "sha512-Op+UycaUt/8FbN/Z2TWPBLge3jWrP3xj10f3fnYxf052bKuS3EKs1ZQcVGjnEMdsNVAM+plXRdmjrZ/KgG3Skw==",
-            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-2.1.0.tgz",
-            "version": "2.1.0"
-        },
         "node_modules/vue": {
             "dependencies": {
                 "@vue/compiler-dom": "3.4.27",
                 "@vue/compiler-sfc": "3.4.27",
                 "@vue/runtime-dom": "3.4.27",
                 "@vue/server-renderer": "3.4.27",
                 "@vue/shared": "3.4.27"
```

### Comparing `swanlab-0.3.3/package.json` & `swanlab-0.3.4/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/.vscode/extensions.json` & `swanlab-0.3.4/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/.vscode/launch.json` & `swanlab-0.3.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/.vscode/settings.json` & `swanlab-0.3.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/.vscode/tailwind.json` & `swanlab-0.3.4/.vscode/tailwind.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/.package-lock.json` & `swanlab-0.3.4/node_modules/.package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999538136669336%*

 * *Differences: {"'packages'": "{'node_modules/@babel/parser': {'version': '7.24.6', 'resolved': "*

 * *               "'https://registry.npmjs.org/@babel/parser/-/parser-7.24.6.tgz', 'integrity': "*

 * *               "'sha512-eNZXdfU35nJC2h24RznROuOpO94h6x8sg9ju0tT9biNtLZ2vuP8SduLqqV+/8+cebSLV9SJEAN5Z3zQbJG/M+Q=='}, "*

 * *               "'node_modules/electron-to-chromium': {'version': '1.4.783', 'resolved': "*

 * *               "'https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.783.tgz', "*

 * *               "'integ […]*

```diff
@@ -314,17 +314,17 @@
         "node_modules/@babel/parser": {
             "bin": {
                 "parser": "bin/babel-parser.js"
             },
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg==",
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.5.tgz",
-            "version": "7.24.5"
+            "integrity": "sha512-eNZXdfU35nJC2h24RznROuOpO94h6x8sg9ju0tT9biNtLZ2vuP8SduLqqV+/8+cebSLV9SJEAN5Z3zQbJG/M+Q==",
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.6.tgz",
+            "version": "7.24.6"
         },
         "node_modules/@esbuild/linux-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
@@ -1810,17 +1810,17 @@
             "dev": true,
             "integrity": "sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==",
             "resolved": "https://registry.npmjs.org/eastasianwidth/-/eastasianwidth-0.2.0.tgz",
             "version": "0.2.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-n02NCwLJ3wexLfK/yQeqfywCblZqLcXphzmid5e8yVPdtEcida7li0A5WQKghHNG0FeOMCzeFOzEbtAh5riXFw==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.777.tgz",
-            "version": "1.4.777"
+            "integrity": "sha512-bT0jEz/Xz1fahQpbZ1D7LgmPYZ3iHVY39NcWWro1+hA2IvjiPeaXtfSqrQ+nXjApMvQRE2ASt1itSLRrebHMRQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.783.tgz",
+            "version": "1.4.783"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-9.2.2.tgz",
             "version": "9.2.2"
         },
@@ -2554,14 +2554,15 @@
                 "fs.realpath": "^1.0.0",
                 "inflight": "^1.0.4",
                 "inherits": "2",
                 "minimatch": "^3.1.1",
                 "once": "^1.3.0",
                 "path-is-absolute": "^1.0.0"
             },
+            "deprecated": "Glob versions prior to v9 are no longer supported",
             "engines": {
                 "node": "*"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==",
@@ -2805,14 +2806,15 @@
             "version": "0.1.4"
         },
         "node_modules/inflight": {
             "dependencies": {
                 "once": "^1.3.0",
                 "wrappy": "1"
             },
+            "deprecated": "This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.",
             "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
             "resolved": "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz",
             "version": "1.0.6"
         },
         "node_modules/inherits": {
             "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
             "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
@@ -3427,17 +3429,17 @@
             "version": "1.2.8"
         },
         "node_modules/minipass": {
             "dev": true,
             "engines": {
                 "node": ">=16 || 14 >=14.17"
             },
-            "integrity": "sha512-UZ7eQ+h8ywIRAW1hIEl2AqdwzJucU/Kp59+8kkZeSvafXhZjul247BvIJjEVFVeON6d7lM46XX1HXCduKAS8VA==",
-            "resolved": "https://registry.npmjs.org/minipass/-/minipass-7.1.1.tgz",
-            "version": "7.1.1"
+            "integrity": "sha512-qOOzS1cBTWYF4BH8fVePDBOO9iptMnGUEZwNc/cMWnTV2nVLZ7VoNWEPHkYczZA0pdoA7dl6e7FL659nX9S2aw==",
+            "resolved": "https://registry.npmjs.org/minipass/-/minipass-7.1.2.tgz",
+            "version": "7.1.2"
         },
         "node_modules/mlly": {
             "dependencies": {
                 "acorn": "^8.11.3",
                 "pathe": "^1.1.2",
                 "pkg-types": "^1.1.0",
                 "ufo": "^1.5.3"
@@ -4040,17 +4042,17 @@
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-A0RVJrX+IUkVZbW3ClroRWurercFhieevHB38sr2+l9eUClMqome3LmEmnhlNy+5Mr2EYN6B2Kaw9wYdd+VHiw==",
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.16.tgz",
-            "version": "6.0.16"
+            "integrity": "sha512-UMz42UD0UY0EApS0ZL9o1XnLhSTtvvvLe5Dc2H2O56fvRZi+KulDyf5ctDhhtYJBGKStV2FL1fy6253cmLgqVQ==",
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.1.0.tgz",
+            "version": "6.1.0"
         },
         "node_modules/postcss-value-parser": {
             "dev": true,
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
@@ -4250,14 +4252,15 @@
         "node_modules/rimraf": {
             "bin": {
                 "rimraf": "bin.js"
             },
             "dependencies": {
                 "glob": "^7.1.3"
             },
+            "deprecated": "Rimraf versions prior to v4 are no longer supported",
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
             "integrity": "sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==",
             "resolved": "https://registry.npmjs.org/rimraf/-/rimraf-3.0.2.tgz",
             "version": "3.0.2"
@@ -4724,23 +4727,23 @@
             },
             "integrity": "sha512-6fPc+R4ihwqP6N/aIv2f1gMH8lOVtWQHoqC4yK6oSDVVocumAsfCqjkXnqiYMhmMwS/mEHLp7Vehlt3ql6lEig==",
             "resolved": "https://registry.npmjs.org/strip-json-comments/-/strip-json-comments-3.1.1.tgz",
             "version": "3.1.1"
         },
         "node_modules/strip-literal": {
             "dependencies": {
-                "acorn": "^8.10.0"
+                "js-tokens": "^9.0.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://github.com/sponsors/antfu"
             },
-            "integrity": "sha512-PugKzOsyXpArk0yWmUwqOZecSO0GH0bPoctLcqNDH9J04pVW3lflYE0ujElBGTloevcxF5MofAOZ7C5l2b+wLg==",
-            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-1.3.0.tgz",
-            "version": "1.3.0"
+            "integrity": "sha512-Op+UycaUt/8FbN/Z2TWPBLge3jWrP3xj10f3fnYxf052bKuS3EKs1ZQcVGjnEMdsNVAM+plXRdmjrZ/KgG3Skw==",
+            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-2.1.0.tgz",
+            "version": "2.1.0"
         },
         "node_modules/sucrase": {
             "bin": {
                 "sucrase": "bin/sucrase",
                 "sucrase-node": "bin/sucrase-node"
             },
             "dependencies": {
@@ -4781,28 +4784,28 @@
         "node_modules/sucrase/node_modules/glob": {
             "bin": {
                 "glob": "dist/esm/bin.mjs"
             },
             "dependencies": {
                 "foreground-child": "^3.1.0",
                 "jackspeak": "^3.1.2",
-                "minimatch": "^9.0.1",
-                "minipass": "^7.0.4",
-                "path-scurry": "^1.11.0"
+                "minimatch": "^9.0.4",
+                "minipass": "^7.1.2",
+                "path-scurry": "^1.11.1"
             },
             "dev": true,
             "engines": {
                 "node": ">=16 || 14 >=14.18"
             },
             "funding": {
                 "url": "https://github.com/sponsors/isaacs"
             },
-            "integrity": "sha512-JDKXl1DiuuHJ6fVS2FXjownaavciiHNUU4mOvV/B793RLh05vZL1rcPnCSaOgv1hDT6RDlY7AB7ZUvFYAtPgAw==",
-            "resolved": "https://registry.npmjs.org/glob/-/glob-10.3.16.tgz",
-            "version": "10.3.16"
+            "integrity": "sha512-2jelhlq3E4ho74ZyVLN03oKdAZVUa6UDZzFLVH1H7dnoax+y9qyaq8zBkfDIggjniU19z0wU18y16jMB2eyVIw==",
+            "resolved": "https://registry.npmjs.org/glob/-/glob-10.4.1.tgz",
+            "version": "10.4.1"
         },
         "node_modules/sucrase/node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^2.0.1"
             },
             "dev": true,
             "engines": {
@@ -5185,31 +5188,31 @@
             "integrity": "sha512-61pPlCD9h51VoreyJ0BReideM3MDKMKnh6+V9L08331ipq6Q8OFXZYiqP6n/tbHx4s5I9uRhcye6BrbkizkBDw==",
             "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.0.2.tgz",
             "version": "1.0.2"
         },
         "node_modules/unimport": {
             "dependencies": {
                 "@rollup/pluginutils": "^5.1.0",
-                "acorn": "^8.11.2",
+                "acorn": "^8.11.3",
                 "escape-string-regexp": "^5.0.0",
                 "estree-walker": "^3.0.3",
                 "fast-glob": "^3.3.2",
                 "local-pkg": "^0.5.0",
-                "magic-string": "^0.30.5",
-                "mlly": "^1.4.2",
-                "pathe": "^1.1.1",
-                "pkg-types": "^1.0.3",
-                "scule": "^1.1.1",
-                "strip-literal": "^1.3.0",
-                "unplugin": "^1.5.1"
+                "magic-string": "^0.30.10",
+                "mlly": "^1.7.0",
+                "pathe": "^1.1.2",
+                "pkg-types": "^1.1.1",
+                "scule": "^1.3.0",
+                "strip-literal": "^2.1.0",
+                "unplugin": "^1.10.1"
             },
             "dev": true,
-            "integrity": "sha512-V9HpXYfsZye5bPPYUgs0Otn3ODS1mDUciaBlXljI4C2fTwfFpvFZRywmlOu943puN9sncxROMZhsZCjNXEpzEQ==",
-            "resolved": "https://registry.npmjs.org/unimport/-/unimport-3.7.1.tgz",
-            "version": "3.7.1"
+            "integrity": "sha512-91mxcZTadgXyj3lFWmrGT8GyoRHWuE5fqPOjg5RVtF6vj+OfM5G6WCzXjuYtSgELE5ggB34RY4oiCSEP8I3AHw==",
+            "resolved": "https://registry.npmjs.org/unimport/-/unimport-3.7.2.tgz",
+            "version": "3.7.2"
         },
         "node_modules/unimport/node_modules/escape-string-regexp": {
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "funding": {
@@ -5632,26 +5635,14 @@
             "funding": {
                 "url": "https://github.com/sponsors/antfu"
             },
             "integrity": "sha512-ok6z3qlYyCDS4ZEU27HaU6x/xZa9Whf8jD4ptH5UZTQYZVYeb9bnZ3ojVhiJNLiXK1Hfc0GNbLXcmZ5plLDDBg==",
             "resolved": "https://registry.npmjs.org/local-pkg/-/local-pkg-0.5.0.tgz",
             "version": "0.5.0"
         },
-        "node_modules/vitest/node_modules/strip-literal": {
-            "dependencies": {
-                "js-tokens": "^9.0.0"
-            },
-            "dev": true,
-            "funding": {
-                "url": "https://github.com/sponsors/antfu"
-            },
-            "integrity": "sha512-Op+UycaUt/8FbN/Z2TWPBLge3jWrP3xj10f3fnYxf052bKuS3EKs1ZQcVGjnEMdsNVAM+plXRdmjrZ/KgG3Skw==",
-            "resolved": "https://registry.npmjs.org/strip-literal/-/strip-literal-2.1.0.tgz",
-            "version": "2.1.0"
-        },
         "node_modules/vue": {
             "dependencies": {
                 "@vue/compiler-dom": "3.4.27",
                 "@vue/compiler-sfc": "3.4.27",
                 "@vue/runtime-dom": "3.4.27",
                 "@vue/server-renderer": "3.4.27",
                 "@vue/shared": "3.4.27"
```

### Comparing `swanlab-0.3.3/node_modules/@alloc/quick-lru/package.json` & `swanlab-0.3.4/node_modules/@alloc/quick-lru/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antfu/utils/package.json` & `swanlab-0.3.4/node_modules/@antfu/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/adjust/package.json` & `swanlab-0.3.4/node_modules/@antv/adjust/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/adjust/node_modules/tslib/package.json` & `swanlab-0.3.4/node_modules/@antv/adjust/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/attr/package.json` & `swanlab-0.3.4/node_modules/@antv/attr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/color-util/package.json` & `swanlab-0.3.4/node_modules/@antv/color-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/component/package.json` & `swanlab-0.3.4/node_modules/@antv/component/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/component/node_modules/@antv/path-util/package.json` & `swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.4/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/coord/package.json` & `swanlab-0.3.4/node_modules/@antv/coord/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/dom-util/package.json` & `swanlab-0.3.4/node_modules/@antv/dom-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/event-emitter/package.json` & `swanlab-0.3.4/node_modules/@antv/event-emitter/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-base/package.json` & `swanlab-0.3.4/node_modules/@antv/g-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json` & `swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.4/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-canvas/package.json` & `swanlab-0.3.4/node_modules/@antv/g-canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json` & `swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.4/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-math/package.json` & `swanlab-0.3.4/node_modules/@antv/g-math/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g-svg/package.json` & `swanlab-0.3.4/node_modules/@antv/g-svg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g2/package.json` & `swanlab-0.3.4/node_modules/@antv/g2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g2/node_modules/@antv/path-util/package.json` & `swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.4/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/g2plot/package.json` & `swanlab-0.3.4/node_modules/@antv/g2plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.4/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/path-util/package.json` & `swanlab-0.3.4/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/scale/package.json` & `swanlab-0.3.4/node_modules/@antv/scale/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@antv/util/package.json` & `swanlab-0.3.4/node_modules/@antv/util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@babel/parser/package.json` & `swanlab-0.3.4/node_modules/@babel/parser/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9558823529411765%*

 * *Differences: {"'devDependencies'": "{'@babel/code-frame': '^7.24.6', '@babel/helper-check-duplicate-nodes': "*

 * *                      "'^7.24.6', '@babel/helper-fixtures': '^7.24.6', "*

 * *                      "'@babel/helper-string-parser': '^7.24.6', "*

 * *                      "'@babel/helper-validator-identifier': '^7.24.6', '@babel/types': '^7.24.6'}",*

 * * "'version'": "'7.24.6'"}*

```diff
@@ -1,18 +1,19 @@
 {
     "author": "The Babel Team (https://babel.dev/team)",
     "bin": "./bin/babel-parser.js",
     "bugs": "https://github.com/babel/babel/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22pkg%3A+parser+%28babylon%29%22+is%3Aopen",
     "description": "A JavaScript parser",
     "devDependencies": {
-        "@babel/code-frame": "^7.24.2",
-        "@babel/helper-check-duplicate-nodes": "^7.22.5",
-        "@babel/helper-fixtures": "^7.24.4",
-        "@babel/helper-string-parser": "^7.24.1",
-        "@babel/helper-validator-identifier": "^7.24.5",
+        "@babel/code-frame": "^7.24.6",
+        "@babel/helper-check-duplicate-nodes": "^7.24.6",
+        "@babel/helper-fixtures": "^7.24.6",
+        "@babel/helper-string-parser": "^7.24.6",
+        "@babel/helper-validator-identifier": "^7.24.6",
+        "@babel/types": "^7.24.6",
         "charcodes": "^0.2.0"
     },
     "engines": {
         "node": ">=6.0.0"
     },
     "files": [
         "bin",
@@ -38,9 +39,9 @@
     "repository": {
         "directory": "packages/babel-parser",
         "type": "git",
         "url": "https://github.com/babel/babel.git"
     },
     "type": "commonjs",
     "types": "./typings/babel-parser.d.ts",
-    "version": "7.24.5"
+    "version": "7.24.6"
 }
```

### Comparing `swanlab-0.3.3/node_modules/@eslint/eslintrc/package.json` & `swanlab-0.3.4/node_modules/@eslint/eslintrc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@eslint/js/package.json` & `swanlab-0.3.4/node_modules/@eslint/js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@eslint-community/eslint-utils/package.json` & `swanlab-0.3.4/node_modules/@eslint-community/eslint-utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@eslint-community/regexpp/package.json` & `swanlab-0.3.4/node_modules/@eslint-community/regexpp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@headlessui/vue/package.json` & `swanlab-0.3.4/node_modules/@headlessui/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@humanwhocodes/config-array/package.json` & `swanlab-0.3.4/node_modules/@humanwhocodes/config-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@humanwhocodes/module-importer/package.json` & `swanlab-0.3.4/node_modules/@humanwhocodes/module-importer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@humanwhocodes/object-schema/package.json` & `swanlab-0.3.4/node_modules/@humanwhocodes/object-schema/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@intlify/core-base/package.json` & `swanlab-0.3.4/node_modules/@intlify/core-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@intlify/message-compiler/package.json` & `swanlab-0.3.4/node_modules/@intlify/message-compiler/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@intlify/shared/package.json` & `swanlab-0.3.4/node_modules/@intlify/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@isaacs/cliui/package.json` & `swanlab-0.3.4/node_modules/@isaacs/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json` & `swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json` & `swanlab-0.3.4/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jest/schemas/package.json` & `swanlab-0.3.4/node_modules/@jest/schemas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jridgewell/gen-mapping/package.json` & `swanlab-0.3.4/node_modules/@jridgewell/gen-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jridgewell/resolve-uri/package.json` & `swanlab-0.3.4/node_modules/@jridgewell/resolve-uri/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jridgewell/set-array/package.json` & `swanlab-0.3.4/node_modules/@jridgewell/set-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jridgewell/source-map/package.json` & `swanlab-0.3.4/node_modules/@jridgewell/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jridgewell/sourcemap-codec/package.json` & `swanlab-0.3.4/node_modules/@jridgewell/sourcemap-codec/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@jridgewell/trace-mapping/package.json` & `swanlab-0.3.4/node_modules/@jridgewell/trace-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@ljharb/resumer/package.json` & `swanlab-0.3.4/node_modules/@ljharb/resumer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@ljharb/through/package.json` & `swanlab-0.3.4/node_modules/@ljharb/through/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@nodelib/fs.scandir/package.json` & `swanlab-0.3.4/node_modules/@nodelib/fs.scandir/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@nodelib/fs.stat/package.json` & `swanlab-0.3.4/node_modules/@nodelib/fs.stat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@nodelib/fs.walk/package.json` & `swanlab-0.3.4/node_modules/@nodelib/fs.walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@pkgjs/parseargs/package.json` & `swanlab-0.3.4/node_modules/@pkgjs/parseargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@popperjs/core/package.json` & `swanlab-0.3.4/node_modules/@popperjs/core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@rollup/pluginutils/package.json` & `swanlab-0.3.4/node_modules/@rollup/pluginutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@sinclair/typebox/package.json` & `swanlab-0.3.4/node_modules/@sinclair/typebox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@tanstack/virtual-core/package.json` & `swanlab-0.3.4/node_modules/@tanstack/virtual-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@tanstack/vue-virtual/package.json` & `swanlab-0.3.4/node_modules/@tanstack/vue-virtual/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@types/d3-timer/package.json` & `swanlab-0.3.4/node_modules/@types/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@types/estree/package.json` & `swanlab-0.3.4/node_modules/@types/estree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@ungap/structured-clone/package.json` & `swanlab-0.3.4/node_modules/@ungap/structured-clone/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitejs/plugin-vue/package.json` & `swanlab-0.3.4/node_modules/@vitejs/plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/expect/package.json` & `swanlab-0.3.4/node_modules/@vitest/expect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/runner/package.json` & `swanlab-0.3.4/node_modules/@vitest/runner/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/runner/node_modules/p-limit/package.json` & `swanlab-0.3.4/node_modules/@vitest/runner/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/runner/node_modules/yocto-queue/package.json` & `swanlab-0.3.4/node_modules/@vitest/runner/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/snapshot/package.json` & `swanlab-0.3.4/node_modules/@vitest/snapshot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/spy/package.json` & `swanlab-0.3.4/node_modules/@vitest/spy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/utils/package.json` & `swanlab-0.3.4/node_modules/@vitest/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vitest/utils/node_modules/estree-walker/package.json` & `swanlab-0.3.4/node_modules/@vitest/utils/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/compiler-core/package.json` & `swanlab-0.3.4/node_modules/@vue/compiler-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/compiler-dom/package.json` & `swanlab-0.3.4/node_modules/@vue/compiler-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/compiler-sfc/package.json` & `swanlab-0.3.4/node_modules/@vue/compiler-sfc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/compiler-ssr/package.json` & `swanlab-0.3.4/node_modules/@vue/compiler-ssr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/devtools-api/package.json` & `swanlab-0.3.4/node_modules/@vue/devtools-api/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/reactivity/package.json` & `swanlab-0.3.4/node_modules/@vue/reactivity/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/runtime-core/package.json` & `swanlab-0.3.4/node_modules/@vue/runtime-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/runtime-dom/package.json` & `swanlab-0.3.4/node_modules/@vue/runtime-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/server-renderer/package.json` & `swanlab-0.3.4/node_modules/@vue/server-renderer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/@vue/shared/package.json` & `swanlab-0.3.4/node_modules/@vue/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/acorn/package.json` & `swanlab-0.3.4/node_modules/acorn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/acorn-jsx/package.json` & `swanlab-0.3.4/node_modules/acorn-jsx/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/acorn-walk/package.json` & `swanlab-0.3.4/node_modules/acorn-walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ajv/package.json` & `swanlab-0.3.4/node_modules/ajv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ajv/lib/refs/data.json` & `swanlab-0.3.4/node_modules/ajv/lib/refs/data.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-draft-04.json` & `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-04.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-draft-06.json` & `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-06.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-draft-07.json` & `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-draft-07.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ajv/lib/refs/json-schema-secure.json` & `swanlab-0.3.4/node_modules/ajv/lib/refs/json-schema-secure.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/align-text/package.json` & `swanlab-0.3.4/node_modules/align-text/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ansi-regex/package.json` & `swanlab-0.3.4/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ansi-styles/package.json` & `swanlab-0.3.4/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/any-promise/package.json` & `swanlab-0.3.4/node_modules/any-promise/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/anymatch/package.json` & `swanlab-0.3.4/node_modules/anymatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/arg/package.json` & `swanlab-0.3.4/node_modules/arg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/argparse/package.json` & `swanlab-0.3.4/node_modules/argparse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/array-buffer-byte-length/package.json` & `swanlab-0.3.4/node_modules/array-buffer-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/array-buffer-byte-length/tsconfig.json` & `swanlab-0.3.4/node_modules/array-buffer-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/arraybuffer.prototype.slice/package.json` & `swanlab-0.3.4/node_modules/arraybuffer.prototype.slice/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/assertion-error/package.json` & `swanlab-0.3.4/node_modules/assertion-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/asynckit/package.json` & `swanlab-0.3.4/node_modules/asynckit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/autoprefixer/package.json` & `swanlab-0.3.4/node_modules/autoprefixer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/available-typed-arrays/package.json` & `swanlab-0.3.4/node_modules/available-typed-arrays/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/available-typed-arrays/tsconfig.json` & `swanlab-0.3.4/node_modules/available-typed-arrays/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/axios/package.json` & `swanlab-0.3.4/node_modules/axios/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/balanced-match/package.json` & `swanlab-0.3.4/node_modules/balanced-match/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/base64-arraybuffer/package.json` & `swanlab-0.3.4/node_modules/base64-arraybuffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/binary-extensions/binary-extensions.json` & `swanlab-0.3.4/node_modules/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/binary-extensions/package.json` & `swanlab-0.3.4/node_modules/binary-extensions/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/boolbase/package.json` & `swanlab-0.3.4/node_modules/boolbase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/brace-expansion/package.json` & `swanlab-0.3.4/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/braces/package.json` & `swanlab-0.3.4/node_modules/braces/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/browserslist/package.json` & `swanlab-0.3.4/node_modules/browserslist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/cac/package.json` & `swanlab-0.3.4/node_modules/cac/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/call-bind/package.json` & `swanlab-0.3.4/node_modules/call-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/callsites/package.json` & `swanlab-0.3.4/node_modules/callsites/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/camelcase/package.json` & `swanlab-0.3.4/node_modules/camelcase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/camelcase-css/package.json` & `swanlab-0.3.4/node_modules/camelcase-css/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/caniuse-lite/package.json` & `swanlab-0.3.4/node_modules/caniuse-lite/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/center-align/package.json` & `swanlab-0.3.4/node_modules/center-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/chai/package.json` & `swanlab-0.3.4/node_modules/chai/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/chalk/package.json` & `swanlab-0.3.4/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/check-error/package.json` & `swanlab-0.3.4/node_modules/check-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/chokidar/package.json` & `swanlab-0.3.4/node_modules/chokidar/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/chokidar/node_modules/glob-parent/package.json` & `swanlab-0.3.4/node_modules/chokidar/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/cliui/package.json` & `swanlab-0.3.4/node_modules/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/color-convert/package.json` & `swanlab-0.3.4/node_modules/color-convert/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/color-name/package.json` & `swanlab-0.3.4/node_modules/color-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/combined-stream/package.json` & `swanlab-0.3.4/node_modules/combined-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/commander/package.json` & `swanlab-0.3.4/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/concat-map/package.json` & `swanlab-0.3.4/node_modules/concat-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/confbox/package.json` & `swanlab-0.3.4/node_modules/confbox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/contour_plot/package.json` & `swanlab-0.3.4/node_modules/contour_plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/cross-spawn/package.json` & `swanlab-0.3.4/node_modules/cross-spawn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/css-line-break/package.json` & `swanlab-0.3.4/node_modules/css-line-break/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/cssesc/package.json` & `swanlab-0.3.4/node_modules/cssesc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/csstype/package.json` & `swanlab-0.3.4/node_modules/csstype/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/d3-color/package.json` & `swanlab-0.3.4/node_modules/d3-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/d3-ease/package.json` & `swanlab-0.3.4/node_modules/d3-ease/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/d3-hierarchy/package.json` & `swanlab-0.3.4/node_modules/d3-hierarchy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/d3-interpolate/package.json` & `swanlab-0.3.4/node_modules/d3-interpolate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/d3-regression/package.json` & `swanlab-0.3.4/node_modules/d3-regression/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/d3-timer/package.json` & `swanlab-0.3.4/node_modules/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/data-view-buffer/package.json` & `swanlab-0.3.4/node_modules/data-view-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/data-view-buffer/tsconfig.json` & `swanlab-0.3.4/node_modules/data-view-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/data-view-byte-length/package.json` & `swanlab-0.3.4/node_modules/data-view-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/data-view-byte-offset/package.json` & `swanlab-0.3.4/node_modules/data-view-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/data-view-byte-offset/tsconfig.json` & `swanlab-0.3.4/node_modules/data-view-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/debug/package.json` & `swanlab-0.3.4/node_modules/debug/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/decamelize/package.json` & `swanlab-0.3.4/node_modules/decamelize/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/deep-eql/package.json` & `swanlab-0.3.4/node_modules/deep-eql/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/deep-equal/package.json` & `swanlab-0.3.4/node_modules/deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/deep-is/package.json` & `swanlab-0.3.4/node_modules/deep-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/define-data-property/package.json` & `swanlab-0.3.4/node_modules/define-data-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/define-data-property/tsconfig.json` & `swanlab-0.3.4/node_modules/define-data-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/define-properties/package.json` & `swanlab-0.3.4/node_modules/define-properties/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/defined/package.json` & `swanlab-0.3.4/node_modules/defined/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/delayed-stream/package.json` & `swanlab-0.3.4/node_modules/delayed-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/detect-browser/package.json` & `swanlab-0.3.4/node_modules/detect-browser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/didyoumean/package.json` & `swanlab-0.3.4/node_modules/didyoumean/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/diff-sequences/package.json` & `swanlab-0.3.4/node_modules/diff-sequences/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/dlv/package.json` & `swanlab-0.3.4/node_modules/dlv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/doctrine/package.json` & `swanlab-0.3.4/node_modules/doctrine/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/dotignore/package.json` & `swanlab-0.3.4/node_modules/dotignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/electron-to-chromium/chromium-versions.json` & `swanlab-0.3.4/node_modules/electron-to-chromium/chromium-versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/electron-to-chromium/full-chromium-versions.json` & `swanlab-0.3.4/node_modules/electron-to-chromium/full-chromium-versions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949170274170275%*

 * *Differences: {"'120.0.6099.291'": "{insert: [(9, '28.3.2'), (10, '28.3.3')]}",*

 * * "'122.0.6261.156'": "{insert: [(6, '29.4.1')]}",*

 * * "'124.0.6367.221'": "['30.0.7']",*

 * * "'124.0.6367.230'": "['30.0.8']",*

 * * "'126.0.6445.0'": "{insert: [(5, '31.0.0-beta.6'), (13, '32.0.0-nightly.20240522'), (14, "*

 * *                   "'32.0.0-nightly.20240523'), (15, '32.0.0-nightly.20240524')]}"}*

```diff
@@ -1128,15 +1128,17 @@
         "28.2.5",
         "28.2.6",
         "28.2.7",
         "28.2.8",
         "28.2.9",
         "28.2.10",
         "28.3.0",
-        "28.3.1"
+        "28.3.1",
+        "28.3.2",
+        "28.3.3"
     ],
     "120.0.6099.35": [
         "28.0.0-beta.11"
     ],
     "120.0.6099.5": [
         "28.0.0-beta.3",
         "28.0.0-beta.4"
@@ -1242,15 +1244,16 @@
     ],
     "122.0.6261.156": [
         "29.2.0",
         "29.3.0",
         "29.3.1",
         "29.3.2",
         "29.3.3",
-        "29.4.0"
+        "29.4.0",
+        "29.4.1"
     ],
     "122.0.6261.18": [
         "29.0.0-beta.5",
         "29.0.0-beta.6",
         "29.0.0-beta.7",
         "29.0.0-beta.8",
         "29.0.0-beta.9",
@@ -1362,14 +1365,20 @@
     "124.0.6367.201": [
         "30.0.4"
     ],
     "124.0.6367.207": [
         "30.0.5",
         "30.0.6"
     ],
+    "124.0.6367.221": [
+        "30.0.7"
+    ],
+    "124.0.6367.230": [
+        "30.0.8"
+    ],
     "124.0.6367.29": [
         "30.0.0-beta.7",
         "30.0.0-beta.8"
     ],
     "124.0.6367.49": [
         "30.0.0"
     ],
@@ -1409,21 +1418,25 @@
     ],
     "126.0.6445.0": [
         "31.0.0-beta.1",
         "31.0.0-beta.2",
         "31.0.0-beta.3",
         "31.0.0-beta.4",
         "31.0.0-beta.5",
+        "31.0.0-beta.6",
         "32.0.0-nightly.20240513",
         "32.0.0-nightly.20240514",
         "32.0.0-nightly.20240515",
         "32.0.0-nightly.20240516",
         "32.0.0-nightly.20240517",
         "32.0.0-nightly.20240520",
-        "32.0.0-nightly.20240521"
+        "32.0.0-nightly.20240521",
+        "32.0.0-nightly.20240522",
+        "32.0.0-nightly.20240523",
+        "32.0.0-nightly.20240524"
     ],
     "39.0.2171.65": [
         "0.20.0",
         "0.20.1",
         "0.20.2",
         "0.20.3",
         "0.20.4",
```

### Comparing `swanlab-0.3.3/node_modules/electron-to-chromium/full-versions.json` & `swanlab-0.3.4/node_modules/electron-to-chromium/full-versions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962358845671268%*

 * *Differences: {"'28.3.2'": "'120.0.6099.291'",*

 * * "'28.3.3'": "'120.0.6099.291'",*

 * * "'29.4.1'": "'122.0.6261.156'",*

 * * "'30.0.7'": "'124.0.6367.221'",*

 * * "'30.0.8'": "'124.0.6367.230'",*

 * * "'31.0.0-beta.6'": "'126.0.6445.0'",*

 * * "'32.0.0-nightly.20240522'": "'126.0.6445.0'",*

 * * "'32.0.0-nightly.20240523'": "'126.0.6445.0'",*

 * * "'32.0.0-nightly.20240524'": "'126.0.6445.0'"}*

```diff
@@ -1748,14 +1748,16 @@
     "28.2.5": "120.0.6099.291",
     "28.2.6": "120.0.6099.291",
     "28.2.7": "120.0.6099.291",
     "28.2.8": "120.0.6099.291",
     "28.2.9": "120.0.6099.291",
     "28.3.0": "120.0.6099.291",
     "28.3.1": "120.0.6099.291",
+    "28.3.2": "120.0.6099.291",
+    "28.3.3": "120.0.6099.291",
     "29.0.0": "122.0.6261.39",
     "29.0.0-alpha.1": "121.0.6147.0",
     "29.0.0-alpha.10": "122.0.6236.2",
     "29.0.0-alpha.11": "122.0.6236.2",
     "29.0.0-alpha.2": "121.0.6147.0",
     "29.0.0-alpha.3": "121.0.6147.0",
     "29.0.0-alpha.4": "121.0.6159.0",
@@ -1826,14 +1828,15 @@
     "29.1.6": "122.0.6261.139",
     "29.2.0": "122.0.6261.156",
     "29.3.0": "122.0.6261.156",
     "29.3.1": "122.0.6261.156",
     "29.3.2": "122.0.6261.156",
     "29.3.3": "122.0.6261.156",
     "29.4.0": "122.0.6261.156",
+    "29.4.1": "122.0.6261.156",
     "3.0.0": "66.0.3359.181",
     "3.0.0-beta.1": "66.0.3359.181",
     "3.0.0-beta.10": "66.0.3359.181",
     "3.0.0-beta.11": "66.0.3359.181",
     "3.0.0-beta.12": "66.0.3359.181",
     "3.0.0-beta.13": "66.0.3359.181",
     "3.0.0-beta.2": "66.0.3359.181",
@@ -1946,24 +1949,27 @@
     "30.0.0-nightly.20240221": "123.0.6296.0",
     "30.0.1": "124.0.6367.60",
     "30.0.2": "124.0.6367.91",
     "30.0.3": "124.0.6367.119",
     "30.0.4": "124.0.6367.201",
     "30.0.5": "124.0.6367.207",
     "30.0.6": "124.0.6367.207",
+    "30.0.7": "124.0.6367.221",
+    "30.0.8": "124.0.6367.230",
     "31.0.0-alpha.1": "125.0.6412.0",
     "31.0.0-alpha.2": "125.0.6412.0",
     "31.0.0-alpha.3": "125.0.6412.0",
     "31.0.0-alpha.4": "125.0.6412.0",
     "31.0.0-alpha.5": "125.0.6412.0",
     "31.0.0-beta.1": "126.0.6445.0",
     "31.0.0-beta.2": "126.0.6445.0",
     "31.0.0-beta.3": "126.0.6445.0",
     "31.0.0-beta.4": "126.0.6445.0",
     "31.0.0-beta.5": "126.0.6445.0",
+    "31.0.0-beta.6": "126.0.6445.0",
     "31.0.0-nightly.20240222": "123.0.6312.5",
     "31.0.0-nightly.20240223": "123.0.6312.5",
     "31.0.0-nightly.20240226": "123.0.6312.5",
     "31.0.0-nightly.20240227": "123.0.6312.5",
     "31.0.0-nightly.20240228": "123.0.6312.5",
     "31.0.0-nightly.20240229": "124.0.6323.0",
     "31.0.0-nightly.20240301": "124.0.6323.0",
@@ -2013,14 +2019,17 @@
     "32.0.0-nightly.20240513": "126.0.6445.0",
     "32.0.0-nightly.20240514": "126.0.6445.0",
     "32.0.0-nightly.20240515": "126.0.6445.0",
     "32.0.0-nightly.20240516": "126.0.6445.0",
     "32.0.0-nightly.20240517": "126.0.6445.0",
     "32.0.0-nightly.20240520": "126.0.6445.0",
     "32.0.0-nightly.20240521": "126.0.6445.0",
+    "32.0.0-nightly.20240522": "126.0.6445.0",
+    "32.0.0-nightly.20240523": "126.0.6445.0",
+    "32.0.0-nightly.20240524": "126.0.6445.0",
     "4.0.0": "69.0.3497.106",
     "4.0.0-beta.1": "69.0.3497.106",
     "4.0.0-beta.10": "69.0.3497.106",
     "4.0.0-beta.11": "69.0.3497.106",
     "4.0.0-beta.2": "69.0.3497.106",
     "4.0.0-beta.3": "69.0.3497.106",
     "4.0.0-beta.4": "69.0.3497.106",
```

### Comparing `swanlab-0.3.3/node_modules/electron-to-chromium/package.json` & `swanlab-0.3.4/node_modules/electron-to-chromium/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.4.783'"}*

```diff
@@ -36,9 +36,9 @@
     },
     "scripts": {
         "build": "node build.mjs",
         "report": "nyc report --reporter=text-lcov > coverage.lcov && codecov",
         "test": "nyc ava --verbose",
         "update": "node automated-update.js"
     },
-    "version": "1.4.777"
+    "version": "1.4.783"
 }
```

### Comparing `swanlab-0.3.3/node_modules/electron-to-chromium/versions.json` & `swanlab-0.3.4/node_modules/electron-to-chromium/versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/emoji-regex/package.json` & `swanlab-0.3.4/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/entities/package.json` & `swanlab-0.3.4/node_modules/entities/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-abstract/package.json` & `swanlab-0.3.4/node_modules/es-abstract/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-abstract/helpers/caseFolding.json` & `swanlab-0.3.4/node_modules/es-abstract/helpers/caseFolding.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-abstract/node_modules/object-inspect/package.json` & `swanlab-0.3.4/node_modules/es-abstract/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-define-property/package.json` & `swanlab-0.3.4/node_modules/es-define-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-define-property/tsconfig.json` & `swanlab-0.3.4/node_modules/es-define-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-errors/package.json` & `swanlab-0.3.4/node_modules/es-errors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-errors/tsconfig.json` & `swanlab-0.3.4/node_modules/es-errors/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-object-atoms/package.json` & `swanlab-0.3.4/node_modules/es-object-atoms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-set-tostringtag/package.json` & `swanlab-0.3.4/node_modules/es-set-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-set-tostringtag/tsconfig.json` & `swanlab-0.3.4/node_modules/es-set-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/es-to-primitive/package.json` & `swanlab-0.3.4/node_modules/es-to-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/esbuild/package.json` & `swanlab-0.3.4/node_modules/esbuild/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/escalade/package.json` & `swanlab-0.3.4/node_modules/escalade/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.4/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint/package.json` & `swanlab-0.3.4/node_modules/eslint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint/conf/replacements.json` & `swanlab-0.3.4/node_modules/eslint/conf/replacements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint/conf/rule-type-list.json` & `swanlab-0.3.4/node_modules/eslint/conf/rule-type-list.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json` & `swanlab-0.3.4/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-prettier/package.json` & `swanlab-0.3.4/node_modules/eslint-plugin-prettier/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/package.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/html-elements.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/html-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json` & `swanlab-0.3.4/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-scope/package.json` & `swanlab-0.3.4/node_modules/eslint-scope/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/eslint-visitor-keys/package.json` & `swanlab-0.3.4/node_modules/eslint-visitor-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/espree/package.json` & `swanlab-0.3.4/node_modules/espree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/esquery/package.json` & `swanlab-0.3.4/node_modules/esquery/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/esrecurse/package.json` & `swanlab-0.3.4/node_modules/esrecurse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/estraverse/package.json` & `swanlab-0.3.4/node_modules/estraverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/estree-walker/package.json` & `swanlab-0.3.4/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/esutils/package.json` & `swanlab-0.3.4/node_modules/esutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/execa/package.json` & `swanlab-0.3.4/node_modules/execa/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-deep-equal/package.json` & `swanlab-0.3.4/node_modules/fast-deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-diff/package.json` & `swanlab-0.3.4/node_modules/fast-diff/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-glob/package.json` & `swanlab-0.3.4/node_modules/fast-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-glob/node_modules/glob-parent/package.json` & `swanlab-0.3.4/node_modules/fast-glob/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-json-stable-stringify/package.json` & `swanlab-0.3.4/node_modules/fast-json-stable-stringify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-json-stable-stringify/benchmark/test.json` & `swanlab-0.3.4/node_modules/fast-json-stable-stringify/benchmark/test.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fast-levenshtein/package.json` & `swanlab-0.3.4/node_modules/fast-levenshtein/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fastq/package.json` & `swanlab-0.3.4/node_modules/fastq/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fecha/package.json` & `swanlab-0.3.4/node_modules/fecha/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/file-entry-cache/package.json` & `swanlab-0.3.4/node_modules/file-entry-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fill-range/package.json` & `swanlab-0.3.4/node_modules/fill-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/find-up/package.json` & `swanlab-0.3.4/node_modules/find-up/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/flat-cache/package.json` & `swanlab-0.3.4/node_modules/flat-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/flatted/package.json` & `swanlab-0.3.4/node_modules/flatted/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fmin/package.json` & `swanlab-0.3.4/node_modules/fmin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/follow-redirects/package.json` & `swanlab-0.3.4/node_modules/follow-redirects/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/for-each/package.json` & `swanlab-0.3.4/node_modules/for-each/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/foreground-child/package.json` & `swanlab-0.3.4/node_modules/foreground-child/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/form-data/package.json` & `swanlab-0.3.4/node_modules/form-data/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fraction.js/package.json` & `swanlab-0.3.4/node_modules/fraction.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/fs.realpath/package.json` & `swanlab-0.3.4/node_modules/fs.realpath/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/function-bind/package.json` & `swanlab-0.3.4/node_modules/function-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/function.prototype.name/package.json` & `swanlab-0.3.4/node_modules/function.prototype.name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/functions-have-names/package.json` & `swanlab-0.3.4/node_modules/functions-have-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/get-func-name/package.json` & `swanlab-0.3.4/node_modules/get-func-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/get-intrinsic/package.json` & `swanlab-0.3.4/node_modules/get-intrinsic/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/get-stream/package.json` & `swanlab-0.3.4/node_modules/get-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/get-symbol-description/package.json` & `swanlab-0.3.4/node_modules/get-symbol-description/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/gl-matrix/package.json` & `swanlab-0.3.4/node_modules/gl-matrix/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/glob/package.json` & `swanlab-0.3.4/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/glob-parent/package.json` & `swanlab-0.3.4/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/globals/globals.json` & `swanlab-0.3.4/node_modules/globals/globals.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/globals/package.json` & `swanlab-0.3.4/node_modules/globals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/globalthis/package.json` & `swanlab-0.3.4/node_modules/globalthis/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/gopd/package.json` & `swanlab-0.3.4/node_modules/gopd/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/graphemer/package.json` & `swanlab-0.3.4/node_modules/graphemer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has/package.json` & `swanlab-0.3.4/node_modules/has/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-ansi/package.json` & `swanlab-0.3.4/node_modules/has-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.4/node_modules/has-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-bigints/package.json` & `swanlab-0.3.4/node_modules/has-bigints/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-flag/package.json` & `swanlab-0.3.4/node_modules/has-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-property-descriptors/package.json` & `swanlab-0.3.4/node_modules/has-property-descriptors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-proto/package.json` & `swanlab-0.3.4/node_modules/has-proto/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-proto/tsconfig.json` & `swanlab-0.3.4/node_modules/has-proto/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-symbols/package.json` & `swanlab-0.3.4/node_modules/has-symbols/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-tostringtag/package.json` & `swanlab-0.3.4/node_modules/has-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/has-tostringtag/tsconfig.json` & `swanlab-0.3.4/node_modules/has-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/hasown/package.json` & `swanlab-0.3.4/node_modules/hasown/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/html2canvas/package.json` & `swanlab-0.3.4/node_modules/html2canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/html2canvas/tsconfig.json` & `swanlab-0.3.4/node_modules/html2canvas/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/human-signals/package.json` & `swanlab-0.3.4/node_modules/human-signals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/husky/package.json` & `swanlab-0.3.4/node_modules/husky/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ignore/package.json` & `swanlab-0.3.4/node_modules/ignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/immutable/package.json` & `swanlab-0.3.4/node_modules/immutable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/import-fresh/package.json` & `swanlab-0.3.4/node_modules/import-fresh/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/imurmurhash/package.json` & `swanlab-0.3.4/node_modules/imurmurhash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/inflight/package.json` & `swanlab-0.3.4/node_modules/inflight/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/inherits/package.json` & `swanlab-0.3.4/node_modules/inherits/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/internal-slot/package.json` & `swanlab-0.3.4/node_modules/internal-slot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-arguments/package.json` & `swanlab-0.3.4/node_modules/is-arguments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-array-buffer/package.json` & `swanlab-0.3.4/node_modules/is-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-array-buffer/tsconfig.json` & `swanlab-0.3.4/node_modules/is-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-bigint/package.json` & `swanlab-0.3.4/node_modules/is-bigint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-binary-path/package.json` & `swanlab-0.3.4/node_modules/is-binary-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-boolean-object/package.json` & `swanlab-0.3.4/node_modules/is-boolean-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-buffer/package.json` & `swanlab-0.3.4/node_modules/is-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-callable/package.json` & `swanlab-0.3.4/node_modules/is-callable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-core-module/core.json` & `swanlab-0.3.4/node_modules/is-core-module/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-core-module/package.json` & `swanlab-0.3.4/node_modules/is-core-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-data-view/package.json` & `swanlab-0.3.4/node_modules/is-data-view/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-data-view/tsconfig.json` & `swanlab-0.3.4/node_modules/is-data-view/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-date-object/package.json` & `swanlab-0.3.4/node_modules/is-date-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-extglob/package.json` & `swanlab-0.3.4/node_modules/is-extglob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-fullwidth-code-point/package.json` & `swanlab-0.3.4/node_modules/is-fullwidth-code-point/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-glob/package.json` & `swanlab-0.3.4/node_modules/is-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-negative-zero/package.json` & `swanlab-0.3.4/node_modules/is-negative-zero/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-negative-zero/tsconfig.json` & `swanlab-0.3.4/node_modules/is-negative-zero/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-number/package.json` & `swanlab-0.3.4/node_modules/is-number/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-number-object/package.json` & `swanlab-0.3.4/node_modules/is-number-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-path-inside/package.json` & `swanlab-0.3.4/node_modules/is-path-inside/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-regex/package.json` & `swanlab-0.3.4/node_modules/is-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-shared-array-buffer/package.json` & `swanlab-0.3.4/node_modules/is-shared-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-shared-array-buffer/tsconfig.json` & `swanlab-0.3.4/node_modules/is-shared-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-stream/package.json` & `swanlab-0.3.4/node_modules/is-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-string/package.json` & `swanlab-0.3.4/node_modules/is-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-symbol/package.json` & `swanlab-0.3.4/node_modules/is-symbol/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-typed-array/package.json` & `swanlab-0.3.4/node_modules/is-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-typed-array/tsconfig.json` & `swanlab-0.3.4/node_modules/is-typed-array/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/is-weakref/package.json` & `swanlab-0.3.4/node_modules/is-weakref/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/isarray/package.json` & `swanlab-0.3.4/node_modules/isarray/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/isexe/package.json` & `swanlab-0.3.4/node_modules/isexe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/jackspeak/package.json` & `swanlab-0.3.4/node_modules/jackspeak/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/jiti/package.json` & `swanlab-0.3.4/node_modules/jiti/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/js-yaml/package.json` & `swanlab-0.3.4/node_modules/js-yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/json-buffer/package.json` & `swanlab-0.3.4/node_modules/json-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/json-schema-traverse/package.json` & `swanlab-0.3.4/node_modules/json-schema-traverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/json-stable-stringify-without-jsonify/package.json` & `swanlab-0.3.4/node_modules/json-stable-stringify-without-jsonify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/json2module/package.json` & `swanlab-0.3.4/node_modules/json2module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/json5/package.json` & `swanlab-0.3.4/node_modules/json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/keyv/package.json` & `swanlab-0.3.4/node_modules/keyv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/kind-of/package.json` & `swanlab-0.3.4/node_modules/kind-of/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lazy-cache/package.json` & `swanlab-0.3.4/node_modules/lazy-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/levn/package.json` & `swanlab-0.3.4/node_modules/levn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lilconfig/package.json` & `swanlab-0.3.4/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lines-and-columns/package.json` & `swanlab-0.3.4/node_modules/lines-and-columns/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/local-pkg/package.json` & `swanlab-0.3.4/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/locate-path/package.json` & `swanlab-0.3.4/node_modules/locate-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lodash/package.json` & `swanlab-0.3.4/node_modules/lodash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lodash-es/package.json` & `swanlab-0.3.4/node_modules/lodash-es/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lodash.merge/package.json` & `swanlab-0.3.4/node_modules/lodash.merge/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/longest/package.json` & `swanlab-0.3.4/node_modules/longest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/loupe/package.json` & `swanlab-0.3.4/node_modules/loupe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/lru-cache/package.json` & `swanlab-0.3.4/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/magic-string/package.json` & `swanlab-0.3.4/node_modules/magic-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/merge2/package.json` & `swanlab-0.3.4/node_modules/merge2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/micromatch/package.json` & `swanlab-0.3.4/node_modules/micromatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mime-db/db.json` & `swanlab-0.3.4/node_modules/mime-db/db.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mime-db/package.json` & `swanlab-0.3.4/node_modules/mime-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mime-types/package.json` & `swanlab-0.3.4/node_modules/mime-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mimic-fn/package.json` & `swanlab-0.3.4/node_modules/mimic-fn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/minimatch/package.json` & `swanlab-0.3.4/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/minimist/package.json` & `swanlab-0.3.4/node_modules/minimist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/minipass/package.json` & `swanlab-0.3.4/node_modules/minipass/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9574074074074075%*

 * *Differences: {"'devDependencies'": "{'tap': '^19.0.0', 'tshy': '^1.14.0', delete: ['typescript']}",*

 * * "'tshy'": "{'selfLink': False}",*

 * * "'version'": "'7.1.2'"}*

```diff
@@ -3,19 +3,18 @@
     "description": "minimal implementation of a PassThrough stream",
     "devDependencies": {
         "@types/end-of-stream": "^1.4.2",
         "@types/node": "^20.1.2",
         "end-of-stream": "^1.4.0",
         "node-abort-controller": "^3.1.1",
         "prettier": "^2.6.2",
-        "tap": "^18.3.0",
+        "tap": "^19.0.0",
         "through2": "^2.0.3",
-        "tshy": "^1.2.2",
-        "typedoc": "^0.25.1",
-        "typescript": "^5.2.2"
+        "tshy": "^1.14.0",
+        "typedoc": "^0.25.1"
     },
     "engines": {
         "node": ">=16 || 14 >=14.17"
     },
     "exports": {
         ".": {
             "import": {
@@ -70,13 +69,14 @@
         "typecheck": true
     },
     "tshy": {
         "exports": {
             ".": "./src/index.ts",
             "./package.json": "./package.json"
         },
-        "main": true
+        "main": true,
+        "selfLink": false
     },
     "type": "module",
     "types": "./dist/commonjs/index.d.ts",
-    "version": "7.1.1"
+    "version": "7.1.2"
 }
```

### Comparing `swanlab-0.3.3/node_modules/mlly/package.json` & `swanlab-0.3.4/node_modules/mlly/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mock-property/package.json` & `swanlab-0.3.4/node_modules/mock-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mockjs/package.json` & `swanlab-0.3.4/node_modules/mockjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/moment/package.json` & `swanlab-0.3.4/node_modules/moment/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ms/package.json` & `swanlab-0.3.4/node_modules/ms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/mz/package.json` & `swanlab-0.3.4/node_modules/mz/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/nanoid/package.json` & `swanlab-0.3.4/node_modules/nanoid/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/natural-compare/package.json` & `swanlab-0.3.4/node_modules/natural-compare/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/node-releases/data/processed/envs.json` & `swanlab-0.3.4/node_modules/node-releases/data/processed/envs.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/node-releases/data/release-schedule/release-schedule.json` & `swanlab-0.3.4/node_modules/node-releases/data/release-schedule/release-schedule.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/normalize-path/package.json` & `swanlab-0.3.4/node_modules/normalize-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/normalize-range/package.json` & `swanlab-0.3.4/node_modules/normalize-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/npm-run-path/package.json` & `swanlab-0.3.4/node_modules/npm-run-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/npm-run-path/node_modules/path-key/package.json` & `swanlab-0.3.4/node_modules/npm-run-path/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/nth-check/package.json` & `swanlab-0.3.4/node_modules/nth-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/object-assign/package.json` & `swanlab-0.3.4/node_modules/object-assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/object-hash/package.json` & `swanlab-0.3.4/node_modules/object-hash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/object-inspect/package.json` & `swanlab-0.3.4/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/object-is/package.json` & `swanlab-0.3.4/node_modules/object-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/object-keys/package.json` & `swanlab-0.3.4/node_modules/object-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/object.assign/package.json` & `swanlab-0.3.4/node_modules/object.assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/once/package.json` & `swanlab-0.3.4/node_modules/once/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/onetime/package.json` & `swanlab-0.3.4/node_modules/onetime/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/optionator/package.json` & `swanlab-0.3.4/node_modules/optionator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/p-limit/package.json` & `swanlab-0.3.4/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/p-locate/package.json` & `swanlab-0.3.4/node_modules/p-locate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/parent-module/package.json` & `swanlab-0.3.4/node_modules/parent-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/path-exists/package.json` & `swanlab-0.3.4/node_modules/path-exists/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/path-is-absolute/package.json` & `swanlab-0.3.4/node_modules/path-is-absolute/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/path-key/package.json` & `swanlab-0.3.4/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/path-parse/package.json` & `swanlab-0.3.4/node_modules/path-parse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/path-scurry/package.json` & `swanlab-0.3.4/node_modules/path-scurry/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pathe/package.json` & `swanlab-0.3.4/node_modules/pathe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pathval/package.json` & `swanlab-0.3.4/node_modules/pathval/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pdfast/package.json` & `swanlab-0.3.4/node_modules/pdfast/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/picocolors/package.json` & `swanlab-0.3.4/node_modules/picocolors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/picomatch/package.json` & `swanlab-0.3.4/node_modules/picomatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pify/package.json` & `swanlab-0.3.4/node_modules/pify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pinia/package.json` & `swanlab-0.3.4/node_modules/pinia/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pinia/node_modules/vue-demi/package.json` & `swanlab-0.3.4/node_modules/pinia/node_modules/vue-demi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pirates/package.json` & `swanlab-0.3.4/node_modules/pirates/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pkg-types/package.json` & `swanlab-0.3.4/node_modules/pkg-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/possible-typed-array-names/package.json` & `swanlab-0.3.4/node_modules/possible-typed-array-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/possible-typed-array-names/tsconfig.json` & `swanlab-0.3.4/node_modules/possible-typed-array-names/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss/package.json` & `swanlab-0.3.4/node_modules/postcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss-import/package.json` & `swanlab-0.3.4/node_modules/postcss-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss-js/package.json` & `swanlab-0.3.4/node_modules/postcss-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss-load-config/package.json` & `swanlab-0.3.4/node_modules/postcss-load-config/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss-load-config/node_modules/lilconfig/package.json` & `swanlab-0.3.4/node_modules/postcss-load-config/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss-nested/package.json` & `swanlab-0.3.4/node_modules/postcss-nested/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/postcss-selector-parser/package.json` & `swanlab-0.3.4/node_modules/postcss-selector-parser/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'6.1.0'"}*

```diff
@@ -72,9 +72,9 @@
         "pretest": "eslint src && npm run typecheck",
         "report": "nyc report --reporter=html",
         "test": "nyc ava src/__tests__/*.mjs",
         "testone": "ava",
         "typecheck": "tsc --noEmit --strict postcss-selector-parser.d.ts postcss-selector-parser.test.ts"
     },
     "types": "postcss-selector-parser.d.ts",
-    "version": "6.0.16"
+    "version": "6.1.0"
 }
```

### Comparing `swanlab-0.3.3/node_modules/postcss-value-parser/package.json` & `swanlab-0.3.4/node_modules/postcss-value-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/prelude-ls/package.json` & `swanlab-0.3.4/node_modules/prelude-ls/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/prettier-linter-helpers/package.json` & `swanlab-0.3.4/node_modules/prettier-linter-helpers/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pretty-format/package.json` & `swanlab-0.3.4/node_modules/pretty-format/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/pretty-format/node_modules/ansi-styles/package.json` & `swanlab-0.3.4/node_modules/pretty-format/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/proxy-from-env/package.json` & `swanlab-0.3.4/node_modules/proxy-from-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/punycode/package.json` & `swanlab-0.3.4/node_modules/punycode/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/queue-microtask/package.json` & `swanlab-0.3.4/node_modules/queue-microtask/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/read-cache/package.json` & `swanlab-0.3.4/node_modules/read-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/readdirp/package.json` & `swanlab-0.3.4/node_modules/readdirp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/regexp.prototype.flags/package.json` & `swanlab-0.3.4/node_modules/regexp.prototype.flags/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/repeat-string/package.json` & `swanlab-0.3.4/node_modules/repeat-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/resolve/package.json` & `swanlab-0.3.4/node_modules/resolve/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/resolve/lib/core.json` & `swanlab-0.3.4/node_modules/resolve/lib/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/resolve-from/package.json` & `swanlab-0.3.4/node_modules/resolve-from/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/reusify/package.json` & `swanlab-0.3.4/node_modules/reusify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/right-align/package.json` & `swanlab-0.3.4/node_modules/right-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rimraf/package.json` & `swanlab-0.3.4/node_modules/rimraf/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/package.json` & `swanlab-0.3.4/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/node_modules/ansi-regex/package.json` & `swanlab-0.3.4/node_modules/rollup/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/node_modules/ansi-styles/package.json` & `swanlab-0.3.4/node_modules/rollup/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/node_modules/chalk/package.json` & `swanlab-0.3.4/node_modules/rollup/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.4/node_modules/rollup/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/node_modules/strip-ansi/package.json` & `swanlab-0.3.4/node_modules/rollup/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rollup/node_modules/supports-color/package.json` & `swanlab-0.3.4/node_modules/rollup/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/run-parallel/package.json` & `swanlab-0.3.4/node_modules/run-parallel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/rw/package.json` & `swanlab-0.3.4/node_modules/rw/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/safe-array-concat/package.json` & `swanlab-0.3.4/node_modules/safe-array-concat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/safe-regex-test/package.json` & `swanlab-0.3.4/node_modules/safe-regex-test/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/sass/package.json` & `swanlab-0.3.4/node_modules/sass/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/scule/package.json` & `swanlab-0.3.4/node_modules/scule/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/semver/package.json` & `swanlab-0.3.4/node_modules/semver/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/set-function-length/package.json` & `swanlab-0.3.4/node_modules/set-function-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/set-function-name/package.json` & `swanlab-0.3.4/node_modules/set-function-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/set-function-name/tsconfig.json` & `swanlab-0.3.4/node_modules/set-function-name/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/shebang-command/package.json` & `swanlab-0.3.4/node_modules/shebang-command/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/shebang-regex/package.json` & `swanlab-0.3.4/node_modules/shebang-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/side-channel/package.json` & `swanlab-0.3.4/node_modules/side-channel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/side-channel/tsconfig.json` & `swanlab-0.3.4/node_modules/side-channel/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/side-channel/node_modules/object-inspect/package.json` & `swanlab-0.3.4/node_modules/side-channel/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/siginfo/package.json` & `swanlab-0.3.4/node_modules/siginfo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/signal-exit/package.json` & `swanlab-0.3.4/node_modules/signal-exit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/size-sensor/package.json` & `swanlab-0.3.4/node_modules/size-sensor/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/source-map/package.json` & `swanlab-0.3.4/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/source-map-js/package.json` & `swanlab-0.3.4/node_modules/source-map-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/source-map-support/package.json` & `swanlab-0.3.4/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/std-env/package.json` & `swanlab-0.3.4/node_modules/std-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string-width/package.json` & `swanlab-0.3.4/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string-width/node_modules/ansi-regex/package.json` & `swanlab-0.3.4/node_modules/string-width/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string-width/node_modules/strip-ansi/package.json` & `swanlab-0.3.4/node_modules/string-width/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string-width-cjs/package.json` & `swanlab-0.3.4/node_modules/string-width-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string-width-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.4/node_modules/string-width-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string.prototype.trim/package.json` & `swanlab-0.3.4/node_modules/string.prototype.trim/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string.prototype.trimend/package.json` & `swanlab-0.3.4/node_modules/string.prototype.trimend/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/string.prototype.trimstart/package.json` & `swanlab-0.3.4/node_modules/string.prototype.trimstart/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/strip-ansi/package.json` & `swanlab-0.3.4/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/strip-ansi-cjs/package.json` & `swanlab-0.3.4/node_modules/strip-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/strip-final-newline/package.json` & `swanlab-0.3.4/node_modules/strip-final-newline/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/strip-json-comments/package.json` & `swanlab-0.3.4/node_modules/strip-json-comments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/strip-literal/package.json` & `swanlab-0.3.4/node_modules/strip-literal/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9125%*

 * *Differences: {"'dependencies'": "{replace: OrderedDict([('js-tokens', '^9.0.0')])}",*

 * * "'devDependencies'": "{'@antfu/eslint-config': '^2.11.4', '@antfu/ni': '^0.21.12', '@types/node': "*

 * *                      "'^20.11.30', 'bumpp': '^9.4.0', 'eslint': '^8.57.0', 'esmo': '^4.7.0', "*

 * *                      "'pnpm': '^8.15.5', 'rimraf': '^5.0.5', 'three': '^0.163.0', 'typescript': "*

 * *                      "'^5.4.3', 'unbuild': '^2.0.0', 'vite': '^5.2.7', 'vitest': '^1.4.0', 'vue': "*

 * *                      "'^3.4.21'}",*

 * * "'pack […]*

```diff
@@ -1,31 +1,31 @@
 {
     "author": "Anthony Fu <anthonyfu117@hotmail.com>",
     "bugs": {
         "url": "https://github.com/antfu/strip-literal/issues"
     },
     "dependencies": {
-        "acorn": "^8.10.0"
+        "js-tokens": "^9.0.0"
     },
     "description": "Strip comments and string literals from JavaScript code",
     "devDependencies": {
-        "@antfu/eslint-config": "^0.40.0",
-        "@antfu/ni": "^0.21.5",
-        "@types/node": "^20.4.5",
-        "bumpp": "^9.1.1",
-        "eslint": "^8.46.0",
-        "esmo": "^0.17.0",
-        "pnpm": "^8.6.11",
-        "rimraf": "^5.0.1",
-        "three": "^0.155.0",
-        "typescript": "^5.1.6",
-        "unbuild": "^1.2.1",
-        "vite": "^4.4.8",
-        "vitest": "^0.34.1",
-        "vue": "^3.3.4"
+        "@antfu/eslint-config": "^2.11.4",
+        "@antfu/ni": "^0.21.12",
+        "@types/node": "^20.11.30",
+        "bumpp": "^9.4.0",
+        "eslint": "^8.57.0",
+        "esmo": "^4.7.0",
+        "pnpm": "^8.15.5",
+        "rimraf": "^5.0.5",
+        "three": "^0.163.0",
+        "typescript": "^5.4.3",
+        "unbuild": "^2.0.0",
+        "vite": "^5.2.7",
+        "vitest": "^1.4.0",
+        "vue": "^3.4.21"
     },
     "exports": {
         ".": {
             "import": "./dist/index.mjs",
             "require": "./dist/index.cjs",
             "types": "./dist/index.d.ts"
         }
@@ -36,15 +36,15 @@
     "funding": "https://github.com/sponsors/antfu",
     "homepage": "https://github.com/antfu/strip-literal#readme",
     "keywords": [],
     "license": "MIT",
     "main": "./dist/index.cjs",
     "module": "./dist/index.mjs",
     "name": "strip-literal",
-    "packageManager": "pnpm@8.6.11",
+    "packageManager": "pnpm@8.15.5",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/antfu/strip-literal.git"
     },
     "scripts": {
         "bench": "vitest bench",
         "build": "unbuild",
@@ -54,9 +54,9 @@
         "release": "bumpp --commit --push --tag && npm publish",
         "start": "esmo src/index.ts",
         "test": "vitest",
         "typecheck": "tsc --noEmit"
     },
     "sideEffects": false,
     "types": "./dist/index.d.ts",
-    "version": "1.3.0"
+    "version": "2.1.0"
 }
```

### Comparing `swanlab-0.3.3/node_modules/sucrase/package.json` & `swanlab-0.3.4/node_modules/sucrase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/sucrase/node_modules/brace-expansion/package.json` & `swanlab-0.3.4/node_modules/sucrase/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/sucrase/node_modules/commander/package.json` & `swanlab-0.3.4/node_modules/sucrase/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/sucrase/node_modules/glob/package.json` & `swanlab-0.3.4/node_modules/sucrase/node_modules/glob/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9552146464646464%*

 * *Differences: {"'dependencies'": "{'minimatch': '^9.0.4', 'minipass': '^7.1.2', 'path-scurry': '^1.11.1'}",*

 * * "'devDependencies'": "{'prettier': '^3.2.5', 'rimraf': '^5.0.7', 'tap': '^19.0.0', 'tshy': "*

 * *                      "'^1.14.0', delete: ['ts-node', 'typescript']}",*

 * * "'prettier'": "{'experimentalTernaries': True}",*

 * * "'scripts'": "{'format': 'prettier --write . --log-level warn'}",*

 * * "'version'": "'10.4.1'"}*

```diff
@@ -1,30 +1,28 @@
 {
     "author": "Isaac Z. Schlueter <i@izs.me> (https://blog.izs.me/)",
     "bin": "./dist/esm/bin.mjs",
     "dependencies": {
         "foreground-child": "^3.1.0",
         "jackspeak": "^3.1.2",
-        "minimatch": "^9.0.1",
-        "minipass": "^7.0.4",
-        "path-scurry": "^1.11.0"
+        "minimatch": "^9.0.4",
+        "minipass": "^7.1.2",
+        "path-scurry": "^1.11.1"
     },
     "description": "the most correct and second fastest glob implementation in JavaScript",
     "devDependencies": {
         "@types/node": "^20.11.30",
         "memfs": "^3.4.13",
         "mkdirp": "^3.0.1",
-        "prettier": "^2.8.3",
-        "rimraf": "^5.0.1",
+        "prettier": "^3.2.5",
+        "rimraf": "^5.0.7",
         "sync-content": "^1.0.2",
-        "tap": "^18.7.2",
-        "ts-node": "^10.9.2",
-        "tshy": "^1.12.0",
-        "typedoc": "^0.25.12",
-        "typescript": "^5.2.2"
+        "tap": "^19.0.0",
+        "tshy": "^1.14.0",
+        "typedoc": "^0.25.12"
     },
     "engines": {
         "node": ">=16 || 14 >=14.18"
     },
     "exports": {
         ".": {
             "import": {
@@ -47,29 +45,30 @@
     "license": "ISC",
     "main": "./dist/commonjs/index.js",
     "name": "glob",
     "prettier": {
         "arrowParens": "avoid",
         "bracketSameLine": true,
         "endOfLine": "lf",
+        "experimentalTernaries": true,
         "jsxSingleQuote": false,
         "printWidth": 75,
         "semi": false,
         "singleQuote": true,
         "tabWidth": 2,
         "useTabs": false
     },
     "repository": {
         "type": "git",
         "url": "git://github.com/isaacs/node-glob.git"
     },
     "scripts": {
         "bench": "bash benchmark.sh",
         "benchclean": "node benchclean.cjs",
-        "format": "prettier --write . --loglevel warn",
+        "format": "prettier --write . --log-level warn",
         "postversion": "npm publish",
         "prebench": "npm run prepare",
         "prepare": "tshy",
         "preprof": "npm run prepare",
         "prepublish": "npm run benchclean",
         "prepublishOnly": "git push origin --follow-tags",
         "presnap": "npm run prepare",
@@ -90,9 +89,9 @@
             ".": "./src/index.ts",
             "./package.json": "./package.json"
         },
         "main": true
     },
     "type": "module",
     "types": "./dist/commonjs/index.d.ts",
-    "version": "10.3.16"
+    "version": "10.4.1"
 }
```

### Comparing `swanlab-0.3.3/node_modules/sucrase/node_modules/minimatch/package.json` & `swanlab-0.3.4/node_modules/sucrase/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/supports-color/package.json` & `swanlab-0.3.4/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/supports-preserve-symlinks-flag/package.json` & `swanlab-0.3.4/node_modules/supports-preserve-symlinks-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tailwindcss/package.json` & `swanlab-0.3.4/node_modules/tailwindcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tape/package.json` & `swanlab-0.3.4/node_modules/tape/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/terser/package.json` & `swanlab-0.3.4/node_modules/terser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/terser/node_modules/commander/package.json` & `swanlab-0.3.4/node_modules/terser/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/terser/node_modules/source-map/package.json` & `swanlab-0.3.4/node_modules/terser/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/terser/node_modules/source-map-support/package.json` & `swanlab-0.3.4/node_modules/terser/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/text-segmentation/package.json` & `swanlab-0.3.4/node_modules/text-segmentation/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/text-table/package.json` & `swanlab-0.3.4/node_modules/text-table/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/thenify/package.json` & `swanlab-0.3.4/node_modules/thenify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/thenify-all/package.json` & `swanlab-0.3.4/node_modules/thenify-all/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tinybench/package.json` & `swanlab-0.3.4/node_modules/tinybench/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tinypool/package.json` & `swanlab-0.3.4/node_modules/tinypool/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tinyspy/package.json` & `swanlab-0.3.4/node_modules/tinyspy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tippy.js/package.json` & `swanlab-0.3.4/node_modules/tippy.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/to-regex-range/package.json` & `swanlab-0.3.4/node_modules/to-regex-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ts-interface-checker/package.json` & `swanlab-0.3.4/node_modules/ts-interface-checker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/tslib/package.json` & `swanlab-0.3.4/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/type-check/package.json` & `swanlab-0.3.4/node_modules/type-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/type-detect/package.json` & `swanlab-0.3.4/node_modules/type-detect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/type-fest/package.json` & `swanlab-0.3.4/node_modules/type-fest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-buffer/package.json` & `swanlab-0.3.4/node_modules/typed-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-buffer/tsconfig.json` & `swanlab-0.3.4/node_modules/typed-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-byte-length/package.json` & `swanlab-0.3.4/node_modules/typed-array-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-byte-length/tsconfig.json` & `swanlab-0.3.4/node_modules/typed-array-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-byte-offset/package.json` & `swanlab-0.3.4/node_modules/typed-array-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-byte-offset/tsconfig.json` & `swanlab-0.3.4/node_modules/typed-array-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/typed-array-length/package.json` & `swanlab-0.3.4/node_modules/typed-array-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/ufo/package.json` & `swanlab-0.3.4/node_modules/ufo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/uglify-js/package.json` & `swanlab-0.3.4/node_modules/uglify-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/uglify-js/node_modules/source-map/package.json` & `swanlab-0.3.4/node_modules/uglify-js/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/uglify-js/tools/domprops.json` & `swanlab-0.3.4/node_modules/uglify-js/tools/domprops.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unbox-primitive/package.json` & `swanlab-0.3.4/node_modules/unbox-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unimport/package.json` & `swanlab-0.3.4/node_modules/unimport/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9156078296703297%*

 * *Differences: {"'dependencies'": "{'acorn': '^8.11.3', 'magic-string': '^0.30.10', 'mlly': '^1.7.0', 'pathe': "*

 * *                   "'^1.1.2', 'pkg-types': '^1.1.1', 'scule': '^1.3.0', 'strip-literal': '^2.1.0', "*

 * *                   "'unplugin': '^1.10.1'}",*

 * * "'devDependencies'": "{'@antfu/eslint-config': '^2.18.1', '@types/node': '^20.12.12', "*

 * *                      "'@vitest/coverage-v8': '^1.6.0', 'bumpp': '^9.4.1', "*

 * *                      "'conventional-changelog-cli': '^5.0.0', 'eslint': '^9.3.0', 'h3': "*

 * *            […]*

```diff
@@ -1,39 +1,39 @@
 {
     "dependencies": {
         "@rollup/pluginutils": "^5.1.0",
-        "acorn": "^8.11.2",
+        "acorn": "^8.11.3",
         "escape-string-regexp": "^5.0.0",
         "estree-walker": "^3.0.3",
         "fast-glob": "^3.3.2",
         "local-pkg": "^0.5.0",
-        "magic-string": "^0.30.5",
-        "mlly": "^1.4.2",
-        "pathe": "^1.1.1",
-        "pkg-types": "^1.0.3",
-        "scule": "^1.1.1",
-        "strip-literal": "^1.3.0",
-        "unplugin": "^1.5.1"
+        "magic-string": "^0.30.10",
+        "mlly": "^1.7.0",
+        "pathe": "^1.1.2",
+        "pkg-types": "^1.1.1",
+        "scule": "^1.3.0",
+        "strip-literal": "^2.1.0",
+        "unplugin": "^1.10.1"
     },
     "description": "Unified utils for auto importing APIs in modules",
     "devDependencies": {
-        "@antfu/eslint-config": "^2.4.6",
+        "@antfu/eslint-config": "^2.18.1",
         "@types/estree": "^1.0.5",
-        "@types/node": "^20.10.5",
-        "@vitest/coverage-v8": "^1.1.0",
-        "bumpp": "^9.2.1",
-        "conventional-changelog-cli": "^4.1.0",
-        "eslint": "8.56.0",
-        "h3": "^1.9.0",
+        "@types/node": "^20.12.12",
+        "@vitest/coverage-v8": "^1.6.0",
+        "bumpp": "^9.4.1",
+        "conventional-changelog-cli": "^5.0.0",
+        "eslint": "^9.3.0",
+        "h3": "^1.11.1",
         "jquery": "^3.7.1",
-        "lit": "^3.1.0",
-        "typescript": "^5.3.3",
+        "lit": "^3.1.3",
+        "typescript": "^5.4.5",
         "unbuild": "^2.0.0",
-        "vitest": "^1.1.0",
-        "vue-tsc": "^1.8.26"
+        "vitest": "^1.6.0",
+        "vue-tsc": "^2.0.19"
     },
     "exports": {
         ".": {
             "import": "./dist/index.mjs",
             "require": "./dist/index.cjs",
             "types": "./dist/index.d.ts"
         },
@@ -53,15 +53,15 @@
         "*.d.ts",
         "dist"
     ],
     "license": "MIT",
     "main": "./dist/index.cjs",
     "module": "./dist/index.mjs",
     "name": "unimport",
-    "packageManager": "pnpm@8.12.1",
+    "packageManager": "pnpm@9.1.2",
     "repository": "unjs/unimport",
     "scripts": {
         "build": "unbuild",
         "changelog": "conventional-changelog -p angular -i CHANGELOG.md -s",
         "dev": "vitest dev",
         "lint": "eslint .",
         "play": "pnpm -C playground run dev",
@@ -70,9 +70,9 @@
         "release": "pnpm run test --run && bumpp -x \"pnpm run changelog\" --all && npm publish",
         "test": "vitest --coverage",
         "typecheck": "vue-tsc --noEmit"
     },
     "sideEffects": false,
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "3.7.1"
+    "version": "3.7.2"
 }
```

### Comparing `swanlab-0.3.3/node_modules/unimport/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.4/node_modules/unimport/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unimport/node_modules/estree-walker/package.json` & `swanlab-0.3.4/node_modules/unimport/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unimport/node_modules/local-pkg/package.json` & `swanlab-0.3.4/node_modules/unimport/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin/package.json` & `swanlab-0.3.4/node_modules/unplugin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin-auto-import/package.json` & `swanlab-0.3.4/node_modules/unplugin-auto-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json` & `swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin-auto-import/node_modules/minimatch/package.json` & `swanlab-0.3.4/node_modules/unplugin-auto-import/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin-vue-components/package.json` & `swanlab-0.3.4/node_modules/unplugin-vue-components/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json` & `swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/unplugin-vue-components/node_modules/minimatch/package.json` & `swanlab-0.3.4/node_modules/unplugin-vue-components/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/update-browserslist-db/.devcontainer.json` & `swanlab-0.3.4/node_modules/update-browserslist-db/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/update-browserslist-db/package.json` & `swanlab-0.3.4/node_modules/update-browserslist-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/uri-js/package.json` & `swanlab-0.3.4/node_modules/uri-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/util-deprecate/package.json` & `swanlab-0.3.4/node_modules/util-deprecate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/utrie/package.json` & `swanlab-0.3.4/node_modules/utrie/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vite/package.json` & `swanlab-0.3.4/node_modules/vite/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vite/node_modules/rollup/package.json` & `swanlab-0.3.4/node_modules/vite/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vite-node/package.json` & `swanlab-0.3.4/node_modules/vite-node/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vite-plugin-json5/package.json` & `swanlab-0.3.4/node_modules/vite-plugin-json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vitest/package.json` & `swanlab-0.3.4/node_modules/vitest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vitest/node_modules/local-pkg/package.json` & `swanlab-0.3.4/node_modules/vitest/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vitest/node_modules/strip-literal/package.json` & `swanlab-0.3.4/node_modules/webpack-sources/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.34909408773045136%*

 * *Differences: {"'author'": "'Tobias Koppers @sokra'",*

 * * "'bugs'": "{'url': 'https://github.com/webpack/webpack-sources/issues'}",*

 * * "'description'": "'Source code handling classes for webpack'",*

 * * "'devDependencies'": "{'eslint': '^7.7.0', 'coveralls': '^3.0.2', 'eslint-config-prettier': "*

 * *                      "'^6.11.0', 'eslint-plugin-jest': '^23.20.0', 'eslint-plugin-mocha': "*

 * *                      "'^8.0.0', 'eslint-plugin-node': '^11.1.0', 'eslint-plugin-nodeca': "*

 * *                      "'^1.0.3', 'eslint-plugin-prett […]*

```diff
@@ -1,62 +1,58 @@
 {
-    "author": "Anthony Fu <anthonyfu117@hotmail.com>",
+    "author": "Tobias Koppers @sokra",
     "bugs": {
-        "url": "https://github.com/antfu/strip-literal/issues"
+        "url": "https://github.com/webpack/webpack-sources/issues"
     },
-    "dependencies": {
-        "js-tokens": "^9.0.0"
-    },
-    "description": "Strip comments and string literals from JavaScript code",
+    "description": "Source code handling classes for webpack",
     "devDependencies": {
-        "@antfu/eslint-config": "^2.11.4",
-        "@antfu/ni": "^0.21.12",
-        "@types/node": "^20.11.30",
-        "bumpp": "^9.4.0",
-        "eslint": "^8.57.0",
-        "esmo": "^4.7.0",
-        "pnpm": "^8.15.5",
-        "rimraf": "^5.0.5",
-        "three": "^0.163.0",
-        "typescript": "^5.4.3",
-        "unbuild": "^2.0.0",
-        "vite": "^5.2.7",
-        "vitest": "^1.4.0",
-        "vue": "^3.4.21"
-    },
-    "exports": {
-        ".": {
-            "import": "./dist/index.mjs",
-            "require": "./dist/index.cjs",
-            "types": "./dist/index.d.ts"
-        }
+        "coveralls": "^3.0.2",
+        "eslint": "^7.7.0",
+        "eslint-config-prettier": "^6.11.0",
+        "eslint-plugin-jest": "^23.20.0",
+        "eslint-plugin-mocha": "^8.0.0",
+        "eslint-plugin-node": "^11.1.0",
+        "eslint-plugin-nodeca": "^1.0.3",
+        "eslint-plugin-prettier": "^3.0.1",
+        "istanbul": "^0.4.1",
+        "jest": "^26.4.0",
+        "prettier": "^2.0.5",
+        "source-map": "^0.7.3",
+        "sourcemap-validator": "^2.1.0"
+    },
+    "engines": {
+        "node": ">=10.13.0"
     },
     "files": [
-        "dist"
+        "lib/",
+        "!lib/helpers/__mocks__"
+    ],
+    "homepage": "https://github.com/webpack/webpack-sources#readme",
+    "jest": {
+        "forceExit": true,
+        "testEnvironment": "node",
+        "testMatch": [
+            "<rootDir>/test/*.js"
+        ],
+        "transformIgnorePatterns": [
+            "<rootDir>"
+        ]
+    },
+    "keywords": [
+        "webpack",
+        "source-map"
     ],
-    "funding": "https://github.com/sponsors/antfu",
-    "homepage": "https://github.com/antfu/strip-literal#readme",
-    "keywords": [],
     "license": "MIT",
-    "main": "./dist/index.cjs",
-    "module": "./dist/index.mjs",
-    "name": "strip-literal",
-    "packageManager": "pnpm@8.15.5",
+    "main": "./lib/index.js",
+    "name": "webpack-sources",
     "repository": {
         "type": "git",
-        "url": "git+https://github.com/antfu/strip-literal.git"
+        "url": "git+https://github.com/webpack/webpack-sources.git"
     },
     "scripts": {
-        "bench": "vitest bench",
-        "build": "unbuild",
-        "dev": "unbuild --stub",
-        "lint": "eslint .",
-        "prepublishOnly": "nr build",
-        "release": "bumpp --commit --push --tag && npm publish",
-        "start": "esmo src/index.ts",
-        "test": "vitest",
-        "typecheck": "tsc --noEmit"
-    },
-    "sideEffects": false,
-    "types": "./dist/index.d.ts",
-    "version": "2.1.0"
+        "cover": "jest --coverage",
+        "lint": "eslint --cache lib test/*.js",
+        "pretest": "yarn lint",
+        "test": "jest"
+    },
+    "version": "3.2.3"
 }
```

### Comparing `swanlab-0.3.3/node_modules/vue/package.json` & `swanlab-0.3.4/node_modules/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-eslint-parser/package.json` & `swanlab-0.3.4/node_modules/vue-eslint-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-i18n/package.json` & `swanlab-0.3.4/node_modules/vue-i18n/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-i18n/vetur/attributes.json` & `swanlab-0.3.4/node_modules/vue-i18n/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-i18n/vetur/tags.json` & `swanlab-0.3.4/node_modules/vue-i18n/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-router/package.json` & `swanlab-0.3.4/node_modules/vue-router/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-router/vetur/attributes.json` & `swanlab-0.3.4/node_modules/vue-router/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-router/vetur/tags.json` & `swanlab-0.3.4/node_modules/vue-router/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-tippy/package.json` & `swanlab-0.3.4/node_modules/vue-tippy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-tippy/tsconfig.json` & `swanlab-0.3.4/node_modules/vue-tippy/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-tippy/vetur/attributes.json` & `swanlab-0.3.4/node_modules/vue-tippy/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/vue-tippy/vetur/tags.json` & `swanlab-0.3.4/node_modules/vue-tippy/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/webpack-sources/package.json` & `swanlab-0.3.4/node_modules/yargs/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.33888888888888885%*

 * *Differences: {"'author'": "{replace: OrderedDict([('name', 'Alex Ford'), ('email', 'Alex.Ford@CodeTunnel.com'), "*

 * *             "('url', 'http://CodeTunnel.com')])}",*

 * * "'contributors'": "[OrderedDict([('name', 'Benjamin Coe'), ('email', 'ben@npmjs.com'), ('url', "*

 * *                   "'https://github.com/bcoe')]), OrderedDict([('name', 'Chris Needham'), "*

 * *                   "('email', 'chris@chrisneedham.com'), ('url', 'http://chrisneedham.com')]), "*

 * *                   "OrderedDict([('name', 'James Nylen'), ('email', 'jny […]*

```diff
@@ -1,58 +1,85 @@
 {
-    "author": "Tobias Koppers @sokra",
-    "bugs": {
-        "url": "https://github.com/webpack/webpack-sources/issues"
+    "author": {
+        "email": "Alex.Ford@CodeTunnel.com",
+        "name": "Alex Ford",
+        "url": "http://CodeTunnel.com"
+    },
+    "contributors": [
+        {
+            "email": "ben@npmjs.com",
+            "name": "Benjamin Coe",
+            "url": "https://github.com/bcoe"
+        },
+        {
+            "email": "chris@chrisneedham.com",
+            "name": "Chris Needham",
+            "url": "http://chrisneedham.com"
+        },
+        {
+            "email": "jnylen@gmail.com",
+            "name": "James Nylen",
+            "url": "https://github.com/nylen"
+        },
+        {
+            "name": "Benjamin Horsleben",
+            "url": "https://github.com/fizker"
+        },
+        {
+            "name": "Lin Clark",
+            "url": "https://github.com/linclark"
+        }
+    ],
+    "dependencies": {
+        "camelcase": "^1.0.2",
+        "cliui": "^2.1.0",
+        "decamelize": "^1.0.0",
+        "window-size": "0.1.0"
     },
-    "description": "Source code handling classes for webpack",
+    "description": "Light-weight option parsing with an argv hash. No optstrings attached.",
     "devDependencies": {
-        "coveralls": "^3.0.2",
-        "eslint": "^7.7.0",
-        "eslint-config-prettier": "^6.11.0",
-        "eslint-plugin-jest": "^23.20.0",
-        "eslint-plugin-mocha": "^8.0.0",
-        "eslint-plugin-node": "^11.1.0",
-        "eslint-plugin-nodeca": "^1.0.3",
-        "eslint-plugin-prettier": "^3.0.1",
-        "istanbul": "^0.4.1",
-        "jest": "^26.4.0",
-        "prettier": "^2.0.5",
-        "source-map": "^0.7.3",
-        "sourcemap-validator": "^2.1.0"
+        "chai": "^2.2.0",
+        "coveralls": "^2.11.2",
+        "hashish": "0.0.4",
+        "mocha": "^2.2.1",
+        "nyc": "^2.2.1",
+        "standard": "^3.11.1"
     },
-    "engines": {
-        "node": ">=10.13.0"
+    "engine": {
+        "node": ">=0.4"
     },
     "files": [
-        "lib/",
-        "!lib/helpers/__mocks__"
+        "index.js",
+        "lib",
+        "completion.sh.hbs",
+        "LICENSE"
     ],
-    "homepage": "https://github.com/webpack/webpack-sources#readme",
-    "jest": {
-        "forceExit": true,
-        "testEnvironment": "node",
-        "testMatch": [
-            "<rootDir>/test/*.js"
-        ],
-        "transformIgnorePatterns": [
-            "<rootDir>"
-        ]
-    },
     "keywords": [
-        "webpack",
-        "source-map"
+        "argument",
+        "args",
+        "option",
+        "parser",
+        "parsing",
+        "cli",
+        "command"
     ],
     "license": "MIT",
-    "main": "./lib/index.js",
-    "name": "webpack-sources",
+    "main": "./index.js",
+    "name": "yargs",
     "repository": {
         "type": "git",
-        "url": "git+https://github.com/webpack/webpack-sources.git"
+        "url": "http://github.com/bcoe/yargs.git"
     },
     "scripts": {
-        "cover": "jest --coverage",
-        "lint": "eslint --cache lib test/*.js",
-        "pretest": "yarn lint",
-        "test": "jest"
+        "coverage": "nyc report --reporter=text-lcov | coveralls",
+        "test": "standard && nyc mocha --check-leaks && nyc report"
+    },
+    "standard": {
+        "globals": [
+            "it"
+        ],
+        "ignore": [
+            "**/example/**"
+        ]
     },
-    "version": "3.2.3"
+    "version": "3.10.0"
 }
```

### Comparing `swanlab-0.3.3/node_modules/webpack-virtual-modules/package.json` & `swanlab-0.3.4/node_modules/webpack-virtual-modules/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/which/package.json` & `swanlab-0.3.4/node_modules/which/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/which-boxed-primitive/package.json` & `swanlab-0.3.4/node_modules/which-boxed-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/which-typed-array/package.json` & `swanlab-0.3.4/node_modules/which-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/why-is-node-running/package.json` & `swanlab-0.3.4/node_modules/why-is-node-running/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/window-size/package.json` & `swanlab-0.3.4/node_modules/window-size/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/word-wrap/package.json` & `swanlab-0.3.4/node_modules/word-wrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wordwrap/package.json` & `swanlab-0.3.4/node_modules/wordwrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi/node_modules/ansi-styles/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi/node_modules/strip-ansi/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi-cjs/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json` & `swanlab-0.3.4/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/wrappy/package.json` & `swanlab-0.3.4/node_modules/wrappy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/xml-name-validator/package.json` & `swanlab-0.3.4/node_modules/xml-name-validator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/yaml/package.json` & `swanlab-0.3.4/node_modules/yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/node_modules/yocto-queue/package.json` & `swanlab-0.3.4/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/error.py` & `swanlab-0.3.4/swanlab/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/package.py` & `swanlab-0.3.4/swanlab/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @File: swanlab/utils/package.py
 @IDE: vscode
 @Description:
     用于管理swanlab的包管理器的模块，做一些封装
 """
 import json
 import os
-from .env import is_dev, get_swanlab_folder
+from .env import is_dev, get_swanlab_folder, is_strict_mode
 from .utils.key import get_key
 from .error import KeyFileError
 
 package_path = None
 if is_dev():
     # 当前运行时的位置
     package_path = os.environ['SWANLAB_PACKAGE_PATH']
@@ -145,14 +145,16 @@
         主要是显示不同的错误信息
 
     Raises
     ------
     ValueError
         如果版本号低于v0.1.5则抛出异常
     """
+    if not is_strict_mode():
+        return
     # 判断文件夹内是否存在runs.swanlog文件
     if os.path.exists(os.path.join(path, "runs.swanlog")):
         return
     # 不存在则进一步判断，如果存在project.json文件，且可以被json读取，并且存在version字段，则说明版本号小于v0.1.5
     if os.path.exists(os.path.join(path, "project.json")):
         with open(os.path.join(path, "project.json"), "r") as f:
             project = json.load(f)
```

### Comparing `swanlab-0.3.3/swanlab/api/cos.py` & `swanlab-0.3.4/swanlab/api/cos.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/api/http.py` & `swanlab-0.3.4/swanlab/api/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,16 +248,15 @@
 
 
 def create_http(login_info: LoginInfo) -> HTTP:
     """
     创建http请求对象
     """
     global http
-    if http is None:
-        http = HTTP(login_info)
+    http = HTTP(login_info)
     return http
 
 
 def get_http() -> HTTP:
     """
     创建http请求对象
     :return: http请求对象
```

### Comparing `swanlab-0.3.3/swanlab/api/info.py` & `swanlab-0.3.4/swanlab/api/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             return None
         return self.__api_key
 
     def __str__(self) -> str:
         """错误时会返回错误信息"""
         if self.__resp.reason == "OK":
             return "Login success"
-        if self.__resp.reason == "Unauthorized":
+        if self.__resp.reason == "Unauthorized" or self.__resp.reason == "Authorization Required":
             return "Error api key"
         if self.__resp.reason == "Forbidden":
             return "You need to be verified first"
         return self.__resp.reason
 
     def save(self):
         """
```

### Comparing `swanlab-0.3.3/swanlab/api/auth/login.py` & `swanlab-0.3.4/swanlab/api/auth/login.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/api/upload/__init__.py` & `swanlab-0.3.4/swanlab/api/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/api/upload/model.py` & `swanlab-0.3.4/swanlab/api/upload/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cli/main.py` & `swanlab-0.3.4/swanlab/cli/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cli/utils.py` & `swanlab-0.3.4/swanlab/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/_log_collector.py` & `swanlab-0.3.4/swanlab/cloud/_log_collector.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/start_thread.py` & `swanlab-0.3.4/swanlab/cloud/start_thread.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/task_types.py` & `swanlab-0.3.4/swanlab/cloud/task_types.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/utils.py` & `swanlab-0.3.4/swanlab/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/dog/log_sniffer.py` & `swanlab-0.3.4/swanlab/cloud/dog/log_sniffer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/dog/metadata_handle.py` & `swanlab-0.3.4/swanlab/cloud/dog/metadata_handle.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/cloud/dog/sniffer_queue.py` & `swanlab-0.3.4/swanlab/cloud/dog/sniffer_queue.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/compat/server/controller/experiment.py` & `swanlab-0.3.4/swanlab/compat/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/converter/tfb/_utils.py` & `swanlab-0.3.4/swanlab/converter/tfb/_utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/converter/tfb/tfb_converter.py` & `swanlab-0.3.4/swanlab/converter/tfb/tfb_converter.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/converter/wb/wb_converter.py` & `swanlab-0.3.4/swanlab/converter/wb/wb_converter.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/__init__.py` & `swanlab-0.3.4/swanlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/callback_cloud.py` & `swanlab-0.3.4/swanlab/data/callback_cloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 r"""
 @DATE: 2024/5/5 20:22
 @File: callback_cloud.py
 @IDE: pycharm
 @Description:
     云端回调
 """
-from .run.callback import NewKeyInfo
+from .run.callback import MetricInfo, ColumnInfo
 from swanlab.cloud import UploadType
-from typing import Optional, Dict
 from swanlab.error import ApiError
 from swanlab.api.upload.model import ColumnModel
 from urllib.parse import quote
 from swanlab.api import LoginInfo, create_http, terminal_login
 from swanlab.api.upload import upload_logs
 from swanlab.log import swanlog
 from swanlab.utils.font import FONT
@@ -41,20 +40,37 @@
         super(CloudRunCallback, self).__init__()
         self.pool = ThreadPool()
         self.exiting = False
         """
         标记是否正在退出云端环境
         """
 
-    def before_init_project(self, project: str, workspace: str, *args, **kwargs) -> int:
-        if self.login_info is None:
-            swanlog.debug("Login info is None, get login info.")
-            self.login_info = self.get_login_info()
-        http = create_http(self.login_info)
-        return http.mount_project(project, workspace).history_exp_count
+    @classmethod
+    def get_login_info(cls):
+        """
+        发起登录，获取登录信息，执行此方法会覆盖原有的login_info
+        """
+        key = None
+        try:
+            key = get_key(os.path.join(get_swanlab_folder(), ".netrc"), get_host_api())[2]
+        except KeyFileError:
+            fd = sys.stdin.fileno()
+            # 不是标准终端，且非jupyter环境，无法控制其回显
+            if not os.isatty(fd) and not in_jupyter():
+                raise KeyFileError("The key file is not found, call `swanlab.login()` or use `swanlab login` ")
+        return terminal_login(key)
+
+    def _view_web_print(self):
+        self._watch_tip_print()
+        http = get_http()
+        project_url = get_host_web() + f"/@{http.groupname}/{http.projname}"
+        experiment_url = project_url + f"/runs/{http.exp_id}"
+        swanlog.info("🏠 View project at " + FONT.blue(FONT.underline(project_url)))
+        swanlog.info("🚀 View run at " + FONT.blue(FONT.underline(experiment_url)))
+        return experiment_url
 
     def _clean_handler(self):
         run = get_run()
         if run is None:
             return swanlog.debug("SwanLab Runtime has been cleaned manually.")
         if self.exiting:
             return swanlog.debug("SwanLab is exiting, please wait.")
@@ -70,24 +86,26 @@
             sys.exit(1)
         self._error_print(tp)
         # 结束运行
         get_run().finish(SwanLabRunState.CRASHED, error=self._traceback_error(tb))
         if tp != KeyboardInterrupt:
             raise tp(val)
 
-    def _view_web_print(self):
-        self._watch_tip_print()
-        http = get_http()
-        project_url = get_host_web() + f"/@{http.groupname}/{http.projname}"
-        experiment_url = project_url + f"/runs/{http.exp_id}"
-        swanlog.info("🏠 View project at " + FONT.blue(FONT.underline(project_url)))
-        swanlog.info("🚀 View run at " + FONT.blue(FONT.underline(experiment_url)))
-        return experiment_url
+    def __str__(self):
+        return "SwanLabCloudRunCallback"
 
-    def on_train_begin(self):
+    def on_init(self, project: str, workspace: str, logdir: str = None) -> int:
+        super(CloudRunCallback, self).on_init(project, workspace, logdir)
+        if self.login_info is None:
+            swanlog.debug("Login info is None, get login info.")
+            self.login_info = self.get_login_info()
+        http = create_http(self.login_info)
+        return http.mount_project(project, workspace).history_exp_count
+
+    def on_run(self):
         # 注册实验信息
         try:
             get_http().mount_exp(
                 exp_name=self.settings.exp_name,
                 colors=self.settings.exp_colors,
                 description=self.settings.description,
             )
@@ -116,15 +134,35 @@
         swanlog.info("Syncing run " + FONT.yellow(self.settings.exp_name) + " to the cloud")
         experiment_url = self._view_web_print()
 
         # 在Jupyter Notebook环境下，显示按钮
         if in_jupyter():
             show_button_html(experiment_url)
 
-    def on_train_end(self, error: str = None):
+    def on_column_create(self, column_info: ColumnInfo):
+        self.pool.queue.put((
+            UploadType.COLUMN,
+            [ColumnModel(column_info.key, column_info.data_type.upper(), column_info.error)]
+        ))
+
+    def on_metric_create(self, metric_info: MetricInfo):
+        super(CloudRunCallback, self).on_metric_create(metric_info)
+        if metric_info.error:
+            return
+        new_data = metric_info.metric
+        new_data['key'] = metric_info.key
+        new_data['index'] = metric_info.step
+        new_data['epoch'] = metric_info.epoch
+        if metric_info.data_type == "default":
+            return self.pool.queue.put((UploadType.SCALAR_METRIC, [new_data]))
+        key = quote(metric_info.key, safe="")
+        data = (new_data, key, metric_info.data_type, metric_info.static_dir)
+        self.pool.queue.put((UploadType.MEDIA_METRIC, [data]))
+
+    def on_stop(self, error: str = None):
         # 打印信息
         self._view_web_print()
         run = get_run()
         # 如果正在退出或者run对象为None或者不在云端环境下
         if self.exiting or run is None:
             return swanlog.debug("SwanLab is exiting or run is None, ignore it.")
         state = run.state
@@ -141,44 +179,7 @@
                 upload_logs(msg, level="ERROR")
 
         FONT.loading("Waiting for uploading complete", _)
         get_http().update_state(state == SwanLabRunState.SUCCESS)
         # 取消注册系统回调
         self._unregister_sys_callback()
         self.exiting = False
-
-    def on_metric_create(self, key: str, key_info: NewKeyInfo, static_dir: str):
-        """
-        指标创建回调函数,新增指标信息时调用
-        :param key: 指标key名称
-        :param key_info: 指标信息
-        :param static_dir: 媒体文件目录
-        """
-        if key_info is None:
-            return
-        new_data, data_type, step, epoch = key_info
-        new_data['key'] = key
-        new_data['index'] = step
-        new_data['epoch'] = epoch
-        if data_type == "default":
-            return self.pool.queue.put((UploadType.SCALAR_METRIC, [new_data]))
-        key = quote(key, safe="")
-        data = (new_data, key, data_type, static_dir)
-        self.pool.queue.put((UploadType.MEDIA_METRIC, [data]))
-
-    def on_column_create(self, key, data_type: str, error: Optional[Dict] = None):
-        self.pool.queue.put((UploadType.COLUMN, [ColumnModel(key, data_type.upper(), error)]))
-
-    @classmethod
-    def get_login_info(cls):
-        """
-        发起登录，获取登录信息，执行此方法会覆盖原有的login_info
-        """
-        key = None
-        try:
-            key = get_key(os.path.join(get_swanlab_folder(), ".netrc"), get_host_api())[2]
-        except KeyFileError:
-            fd = sys.stdin.fileno()
-            # 不是标准终端，且非jupyter环境，无法控制其回显
-            if not os.isatty(fd) and not in_jupyter():
-                raise KeyFileError("The key file is not found, call `swanlab.login()` or use `swanlab login` ")
-        return terminal_login(key)
```

### Comparing `swanlab-0.3.3/swanlab/data/config.py` & `swanlab-0.3.4/swanlab/data/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 def need_inited(func):
     """装饰器，用于检查是否已经初始化"""
 
     def wrapper(self, *args, **kwargs):
         if not self._inited:
-            raise RuntimeError("You must call swanlab.init() before using swanlab.log")
+            raise RuntimeError("You must call swanlab.init() before using swanlab.config")
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
 class SwanLabConfig(Mapping):
     """
@@ -80,17 +80,22 @@
         Parameters
         ----------
         settings : SwanDataSettings, optional
             运行时设置
         """
         self.__config.update(self.__check_config(config))
         self.__settings["save_path"] = settings.config_path if settings is not None else None
+        self.__settings["should_save"] = settings.should_save if settings is not None else False
         if self._inited:
             self.__save()
 
+    @property
+    def should_shave(self):
+        return self.__settings.get("should_save")
+
     @staticmethod
     def __check_config(config: dict) -> dict:
         """
         检查配置是否合法，确保它可以被 JSON/YAML 序列化。
         如果传入的是 argparse.Namespace 类型，会先转换为字典。
         """
         if config is None:
@@ -316,14 +321,16 @@
         except KeyError:
             return False
 
     def __save(self):
         """
         保存config为json，不必校验config的YAML格式，将在写入时完成校验
         """
+        if not self.should_shave:
+            return
         swanlog.debug("Save config to {}".format(self.__settings.get("save_path")))
         with open(self.__settings.get("save_path"), "w") as f:
             # 将config的每个key的value转换为desc和value两部分，value就是原来的value，desc是None
             # 这样做的目的是为了在web界面中显示config的内容,desc是用于描述value的
             config = {
                 key: {
                     "desc": None,
```

### Comparing `swanlab-0.3.3/swanlab/data/sdk.py` & `swanlab-0.3.4/swanlab/data/sdk.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 @DATE: 2024-01-01 18:00:04
 @File: swanlab/data/sdk.py
 @IDE: vscode
 @Description:
     在此处封装swanlab在日志记录模式下的各种接口
 """
 import os
-from typing import Optional, Union, Dict
+from typing import Optional, Union, Dict, Tuple
 from .modules import DataType
 from .run import (
     SwanLabRunState,
     SwanLabRun,
     register,
     get_run,
 )
 from .callback_cloud import CloudRunCallback
 from .callback_local import LocalRunCallback
+from .run.operator import SwanLabRunOperator
 from .config import SwanLabConfig
-from ..db import Project, connect
-from ..env import init_env, ROOT
-from ..log import swanlog
-from ..utils import check_load_json_yaml, check_proj_name_format
+from swanlab.env import init_env, get_swanlog_dir, SwanLabMode, MODE
+from swanlab.log import swanlog
+from swanlab.utils import check_load_json_yaml, check_proj_name_format
 from swanlab.api import code_login
+from swanlab.db import GlomCallback
 from swanlab.package import version_limit
 
 _config: Optional["SwanLabConfig"] = SwanLabConfig(None)
 """
 Allows users to record experiment configurations through swanlab.config.
 Before calling the init() function, config cannot be read or written, even if it is a SwanLabConfig object.
 After calling the init() function, swanlab.config is equivalent to run.config.
@@ -86,15 +87,15 @@
     project: str = None,
     workspace: str = None,
     experiment_name: str = None,
     description: str = None,
     config: Union[dict, str] = None,
     logdir: str = None,
     suffix: Union[str, None, bool] = "default",
-    cloud: bool = True,
+    mode: str = None,
     load: str = None,
     **kwargs,
 ) -> SwanLabRun:
     """
     Start a new run to track and log. Once you have called this function, you can use 'swanlab.log' to log data to
     the current run. Meanwhile, you can use 'swanlab.finish' to finish the current run and close the current
     experiment. After calling this function, SwanLab will begin to record the console output of the current process,
@@ -135,76 +136,71 @@
         The suffix of the experiment name, the default is 'default'.
         If this parameter is 'default', suffix will be '%b%d-%h-%m-%s'(example:'Feb03_14-45-37'),
         which represents the current time.
         example: experiment_name = 'example', suffix = 'default' -> 'example_Feb03_14-45-37';
         If this parameter is None or False, no suffix will be added.
         If this parameter is a string, the suffix will be the string you provided.
         Attention: experiment_name + suffix must be unique, otherwise the experiment will not be created.
-    cloud : bool, optional
-        Whether to use the cloud mode, the default is True.
-        If you use the cloud mode, the log file will be stored in the cloud, which will still be saved locally.
-        If you are not using cloud mode, the `workspace` fields are invalid.
+    mode : str, optional
+        Allowed values are 'cloud', 'cloud-only', 'local', 'disabled'.
+        If the value is 'cloud', the data will be uploaded to the cloud and the local log will be saved.
+        If the value is 'cloud-only', the data will only be uploaded to the cloud and the local log will not be saved.
+        If the value is 'local', the data will only be saved locally and will not be uploaded to the cloud.
+        If the value is 'disabled', the data will not be saved or uploaded, just parsing the data.
     load : str, optional
         If you pass this parameter,SwanLab will search for the configuration file you specified
         (which must be in JSON or YAML format)
         and automatically fill in some explicit parameters of this function for you
         (excluding parameters in `**kwargs` and the parameters if they are None).
         In terms of priority, if the parameters passed to init are `None`,
         SwanLab will attempt to replace them from the configuration file you provided;
         otherwise, it will use the parameters you passed as the definitive ones.
     """
-    # 如果已经初始化过了，直接返回run
     run = get_run()
     if run is not None:
         swanlog.warning("You have already initialized a run, the init function will be ignored")
         return run
     # ---------------------------------- 一些变量、格式检查 ----------------------------------
-    # 如果传入了load，则加载load文件，如果load文件不存在，报错
+    if "cloud" in kwargs:
+        swanlog.warning(
+            "The `cloud` parameter in swanlab.init is deprecated and will be removed in the future"
+            "please use `mode='cloud'` instead."
+        )
+        mode = "cloud" if kwargs["cloud"] else mode
     if load:
         load_data = check_load_json_yaml(load, load)
-        # 尝试更改传入的参数为None的情况，如果传入的参数不是None，不做任何操作
         experiment_name = _load_data(load_data, "experiment_name", experiment_name)
         description = _load_data(load_data, "description", description)
         config = _load_data(load_data, "config", config)
         logdir = _load_data(load_data, "logdir", logdir)
         suffix = _load_data(load_data, "suffix", suffix)
-        cloud = _load_data(load_data, "cloud", cloud)
+        mode = _load_data(load_data, "mode", mode)
         project = _load_data(load_data, "project", project)
         workspace = _load_data(load_data, "workspace", workspace)
-    if not cloud and workspace is not None:
-        swanlog.warning("The `workspace` field is invalid in local mode")
-    # 默认实验名称为当前目录名
-    project = _check_proj_name(project if project else os.path.basename(os.getcwd()))
-    # 初始化logdir参数，接下来logdir被设置为绝对路径且当前程序有写权限
-    logdir = _init_logdir(logdir)
+    operator, c = _create_operator(mode)
+    project = _check_proj_name(project if project else os.path.basename(os.getcwd()))  # 默认实验名称为当前目录名
+    exp_num = SwanLabRunOperator.parse_return(
+        operator.on_init(project, workspace, logdir=logdir), key=c.__str__() if c else None
+    )
     # 初始化confi参数
     config = _init_config(config)
-    # 检查logdir内文件的版本，如果<=0.1.4则报错
-    version_limit(logdir, mode="init")
-    # 初始化环境变量
     init_env()
-    # 定义回调函数
-    callbacks = CloudRunCallback() if cloud else LocalRunCallback()
-    # ---------------------------------- 初始化项目 ----------------------------------
-    # 获取云端历史总数
-    exp_num = callbacks.before_init_project(project, workspace)
-    # 连接本地数据库，要求路径必须存在，但是如果数据库文件不存在，会自动创建
-    connect(autocreate=True)
-    # 初始化项目数据库
-    Project.init(project)
+    # 检查logdir内文件的版本，如果<=0.1.4则报错
+    version_limit(get_swanlog_dir(), mode="init")
     # ---------------------------------- 实例化实验 ----------------------------------
     # 注册实验
     run = register(
+        project_name=project,
         experiment_name=experiment_name,
         description=description,
         config=config,
         log_level=kwargs.get("log_level", "info"),
         suffix=suffix,
         exp_num=exp_num,
-        callbacks=callbacks,
+        operator=operator,
     )
     return run
 
 
 def log(data: Dict[str, DataType], step: int = None):
     """
     Log a row of data to the current run.
@@ -239,67 +235,66 @@
     if not get_run():
         raise RuntimeError("You must call swanlab.data.init() before using finish()")
     if not run.is_running:
         return swanlog.error("After experiment is finished, you can't call finish() again.")
     run.finish(state, error)
 
 
-def _init_logdir(logdir: str) -> str:
+def _init_mode(mode: str = None):
     """
-    处理通过init传入的logdir存在的一些情况
-    """
-    # 如果传入了logdir，则将logdir设置为环境变量，代表日志文件存放的路径
-    if logdir is not None:
-        try:
-            if not isinstance(logdir, str):
-                raise ValueError("path must be a string")
-            if not os.path.isabs(logdir):
-                logdir = os.path.abspath(logdir)
-            # 如果创建失败，也是抛出IOError
-            try:
-                os.makedirs(logdir, exist_ok=True)
-            except Exception as e:
-                raise IOError(f"create path: {logdir} failed, error: {e}")
-            if not os.access(logdir, os.W_OK):
-                raise IOError(f"no write permission for path: {logdir}")
-        except ValueError:
-            raise ValueError("logdir must be a str.")
-        except IOError:
-            raise IOError("logdir must be a path and have Write permission.")
-        os.environ[ROOT] = logdir
-    # 如果没有传入logdir，则使用默认的logdir, 即当前工作目录下的swanlog文件夹，但是需要保证目录存在
-    else:
-        logdir = os.environ.get(ROOT) or os.path.join(os.getcwd(), "swanlog")
-        logdir = os.path.abspath(logdir)
-        try:
-            os.makedirs(logdir, exist_ok=True)
-            if not os.access(logdir, os.W_OK):
-                raise IOError
-        except IOError:
-            raise IOError("logdir must have Write permission.")
-    # 如果logdir是空的，创建.gitignore文件，写入*
-    if not os.listdir(logdir):
-        with open(os.path.join(logdir, ".gitignore"), "w") as f:
-            f.write("*")
-    return logdir
+    初始化mode参数
+    从环境变量中提取默认的mode参数，如果传入的mode参数不为None，则使用环境变量中的mode参数，否则使用传入的mode参数
+    传入的mode必须为SwanLabMode枚举中的一个值，否则报错ValueError
+    如果环境变量和传入的mode参数都为None，则默认为cloud
+
+    :param mode: str, optional
+        传入的mode参数
+    :return: str mode
+    :raise ValueError: mode参数不合法
+    """
+    allowed = [m.value for m in SwanLabMode]
+    m = os.environ.get(MODE)
+    if m is not None and mode is not None:
+        swanlog.warning(f"The environment variable {MODE} will be overwritten by the parameter mode")
+    mode = m if mode is None else mode
+    if mode is not None and mode not in allowed:
+        raise ValueError(f"`mode` must be one of {allowed}, but got {mode}")
+    mode = "cloud" if mode is None else mode
+    os.environ[MODE] = mode
+    return mode
 
 
 def _init_config(config: Union[dict, str]):
     """初始化传入的config参数"""
     if isinstance(config, str):
         swanlog.info("The parameter config is loaded from the configuration file: {}".format(config))
         return check_load_json_yaml(config, "config")
 
     return config
 
 
 def _load_data(load_data: dict, key: str, value):
-    """从load_data中加载数据，如果value不是None"""
+    """
+    从load_data中加载数据，如果value不是None，则直接返回value，如果为None，则返回load_data中的key
+    """
     if value is not None:
-        # tip = "The parameter {} is loaded from the configuration file: {}".format(FONT.bold(key), value)
-        # print(FONT.swanlab(tip))
         return value
     d = load_data.get(key, None)
-    # if d is not None:
-    #     tip = "The parameter {} is loaded from the configuration file: {}".format(FONT.bold(key), d)
-    #     print(FONT.swanlab(tip))
     return d
+
+
+def _create_operator(mode) -> Tuple[SwanLabRunOperator, Optional[CloudRunCallback]]:
+    """
+    创建SwanLabRunOperator实例
+    如果mode为disabled，则返回一个空的SwanLabRunOperator实例和None
+
+    :param mode: str
+        运行模式
+    :return: SwanLabRunOperator, CloudRunCallback
+    """
+    mode = _init_mode(mode)
+    if mode == SwanLabMode.DISABLED.value:
+        swanlog.warning("SwanLab run disabled, the data will not be saved or uploaded.")
+        return SwanLabRunOperator(), None
+    c = CloudRunCallback() if mode == SwanLabMode.CLOUD.value else LocalRunCallback()
+    callbacks = [c, GlomCallback()]
+    return SwanLabRunOperator(callbacks), c
```

### Comparing `swanlab-0.3.3/swanlab/data/settings.py` & `swanlab-0.3.4/swanlab/data/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 from ..env import get_swanlog_dir
 from typing import Tuple
 from swanlab.package import get_package_version
 
 
 class SwanDataSettings:
-    def __init__(self, run_id: str) -> None:
+    def __init__(self, run_id: str, should_save: bool) -> None:
         """实验名称
 
         Parameters
         ----------
         exp_name : str
             实验名称，实验名称应该唯一，由0-9，a-z，A-Z，" ","_","-","/"组成
             但此处不做限制
@@ -31,14 +31,27 @@
         # 日志存放目录
         self.__swanlog_dir: str = get_swanlog_dir()
         # 日志存放目录的上一级目录，默认情况下这应该是项目根目录
         self.__root_dir: str = os.path.dirname(self.__swanlog_dir)
         # 实验运行id
         self.__run_id: str = run_id
         self.__version = get_package_version()
+        self.__should_save = should_save
+
+    @property
+    def should_save(self):
+        """
+        是否应该保存实验信息
+        """
+        return self.__should_save
+
+    def mkdir(self, path: str) -> None:
+        """创建目录"""
+        if not os.path.exists(path) and self.should_save:
+            os.makedirs(path, exist_ok=True)
 
     @property
     def version(self) -> str:
         return self.__version
 
     @property
     def exp_name(self) -> str:
@@ -113,24 +126,23 @@
         """记录终端日志路径"""
         return os.path.join(self.run_dir, "console")
 
     @property
     def static_dir(self) -> str:
         """静态资源路径"""
         path = os.path.join(self.run_dir, "media")
-        if not os.path.exists(path):
-            os.mkdir(path)
+        self.mkdir(path)
         return path
 
     @property
     def files_dir(self) -> str:
         """实验配置信息路径"""
         path = os.path.join(self.run_dir, "files")
-        os.makedirs(path, exist_ok=True)
-        return os.path.join(self.run_dir, "files")
+        self.mkdir(path)
+        return path
 
     @property
     def requirements_path(self) -> str:
         """实验依赖的存储文件"""
         return os.path.join(self.files_dir, "requirements.txt")
 
     @property
```

### Comparing `swanlab-0.3.3/swanlab/data/modules/_utils.py` & `swanlab-0.3.4/swanlab/data/modules/_utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/modules/audio.py` & `swanlab-0.3.4/swanlab/data/modules/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         self.caption = self.__convert_caption(caption)
 
     def get_data(self):
         # 如果传入的是Audio类列表
         if isinstance(self.value, list):
             return self.get_data_list()
         self.__preprocess(self.value)
+        # 判断是否要保存(mode='disabled'时不保存)
+        if not self.settings.should_save:
+            return
         hash_name = (
             get_file_hash_numpy_array(self.audio_data)[:16]
             if isinstance(self.audio_data, np.ndarray)
             else get_file_hash_path(self.audio_data)[:16]
         )
         save_dir = os.path.join(self.settings.static_dir, self.tag)
         save_name = f"audio-step{self.step}-{hash_name}.wav"
```

### Comparing `swanlab-0.3.3/swanlab/data/modules/base.py` & `swanlab-0.3.4/swanlab/data/modules/base.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/modules/chart.py` & `swanlab-0.3.4/swanlab/data/modules/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/modules/image.py` & `swanlab-0.3.4/swanlab/data/modules/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,19 @@
         super().__init__(data_or_path)
         self.image_data = None
         self.mode = mode
         self.caption = self.__convert_caption(caption)
         self.format = self.__convert_file_type(file_type)
         self.size = self.__convert_size(size)
 
+        # 提前预处理maplotlib类型
+        if hasattr(self.value, "savefig"):
+            # 如果输入为matplotlib图像
+            self.value = self.__convert_plt_to_image(self.value)
+
         # TODO: 等前端支持Boxes和Masks后再开启
 
         # self.boxes = None
         # self.boxes_total_classes = None
         # self.masks = None
         # self.masks_total_classes = None
         # if boxes:
@@ -76,14 +81,17 @@
 
     def get_data(self):
         # 如果传入的是Image类列表
         if isinstance(self.value, list):
             return self.get_data_list()
         # 图像预处理
         self.__preprocess(self.value)
+        # 判断是否要保存(mode='disabled'时不保存)
+        if not self.settings.should_save:
+            return
         # 获取图像的hash值
         hash_name = get_file_hash_pil(self.image_data)[:16]
         # 设置保存路径, 保存文件名
         save_dir = os.path.join(self.settings.static_dir, self.tag)
         save_name = f"image-step{self.step}-{hash_name}.{self.format}"
         # 如果不存在目录则创建
         if os.path.exists(save_dir) is False:
@@ -194,17 +202,14 @@
             image = self.__load_image_from_path(data)
         elif isinstance(data, np.ndarray):
             # 如果输入为numpy array
             image = self.__convert_numpy_array_to_image(data)
         elif isinstance(data, PILImage.Image):
             # 如果输入为PIL.Image
             image = data.convert(self.mode)
-        elif hasattr(self.value, "savefig"):
-            # 如果输入为matplotlib图像
-            image = self.__convert_plt_to_image(data)
         elif is_pytorch_tensor_typename(get_full_typename(data)):
             # 如果输入为pytorch tensor
             try:
                 import torchvision
             except ImportError as e:
                 raise TypeError(
                     "swanlab.Image requires `torchvision` when process torch.tensor data. Install with 'pip install torchvision'."
```

### Comparing `swanlab-0.3.3/swanlab/data/modules/object_3d.py` & `swanlab-0.3.4/swanlab/data/modules/object_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     def get_data(self):
         # 如果传入的是Object3D类列表
         if isinstance(self.value, list):
             return self.get_data_list()
 
         self.object3d_data = self.__preprocess(self.value)
 
+        # 判断是否要保存(mode='disabled'时不保存)
+        if not self.settings.should_save:
+            return
+
         # 根据不同的输入类型进行不同的哈希校验
         hash_name = (
             get_file_hash_numpy_array(self.object3d_data)[:16]
             if isinstance(self.object3d_data, np.ndarray)
             else get_file_hash_path(self.object3d_data)[:16]
         )
```

### Comparing `swanlab-0.3.3/swanlab/data/modules/text.py` & `swanlab-0.3.4/swanlab/data/modules/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         # 如果传入的是Text类列表
         if isinstance(self.value, list):
             return self.get_data_list()
 
         # 预处理文本数据
         self.__preprocess(self.value)
 
+        # 判断是否要保存(mode='disabled'时不保存)
+        if not self.settings.should_save:
+            return
+
         return self.text_data
 
     def expect_types(self, *args, **kwargs) -> list:
         return ["str", "int", "float"]
 
     def __preprocess(self, data):
         """
```

### Comparing `swanlab-0.3.3/swanlab/data/modules/video.py` & `swanlab-0.3.4/swanlab/data/modules/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
 
     def get_data(self, *args, **kwargs):
         # 如果传入的是Video类列表
         if isinstance(self.value, list):
             return self.get_data_list()
         # 视频预处理
         self.video_data = self.__preprocess(self.value)
+
+        # 判断是否要保存(mode='disabled'时不保存)
+        if not self.settings.should_save:
+            return
+
         # 获取视频hash值
         hash_name = (
             get_file_hash_numpy_array(self.video_data)[:16]
             if isinstance(self.video_data, np.ndarray)
             else get_file_hash_path(self.video_data)[:16]
         )
         # 设置视频保存路径, 保存文件名
```

### Comparing `swanlab-0.3.3/swanlab/data/modules/utils_modules/bounding_boxes.py` & `swanlab-0.3.4/swanlab/data/modules/utils_modules/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/modules/utils_modules/image_mask.py` & `swanlab-0.3.4/swanlab/data/modules/utils_modules/image_mask.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/run/exp.py` & `swanlab-0.3.4/swanlab/data/run/exp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 import json
 from swanlab.data.settings import SwanDataSettings
 from swanlab.data.modules import BaseType, DataType
 from swanlab.log import swanlog
-from typing import Dict, Tuple, Union, Optional
+from typing import Dict, Union, Optional
 from swanlab.utils import create_time
 from swanlab.utils.file import check_tag_format
+from .callback import MetricInfo, ColumnInfo
+from .operator import SwanLabRunOperator
 from urllib.parse import quote
-import ujson
 import os
 import math
-from swanlab.db import Tag, Namespace, Chart, Source, Experiment, Display, ExistedError, ChartTypeError, add_multi_chart
-from .callback import SwanLabRunCallback, NewKeyInfo
 
 
 class SwanLabExp:
     """
     Class for running experiments
     save keys when running experiments
     """
 
-    def __init__(self, settings: SwanDataSettings, expid: int, exp: Experiment, callbacks: SwanLabRunCallback) -> None:
+    def __init__(self, settings: SwanDataSettings, operator: SwanLabRunOperator) -> None:
         """初始化实验
 
         Parameters
         ----------
         settings : SwanDataSettings
             全局运行时配置
-        expid : int
-            实验id
-        exp : Experiment
-            数据库实例，代表当前实验行
+        operator : SwanLabRunOperator
+            操作员
         """
         self.settings = settings
-        if not os.path.exists(self.settings.log_dir):
-            os.mkdir(self.settings.log_dir)
         # 当前实验的所有tag数据字段
         self.tags: Dict[str, SwanLabTag] = {}
-        self.id = expid
-        """此实验对应的id，实际上就是db.id"""
-        self.db: Experiment = exp
-        """此实验对应的数据库实例"""
-        self.__callbacks = callbacks
+        self.__operator = operator
         """回调函数"""
 
-    def add(self, key: str, data: DataType, step: int = None):
+    def add(self, key: str, data: DataType, step: int = None) -> MetricInfo:
         """记录一条新的tag数据
 
         Parameters
         ----------
         key : str
             tag名称，需要检查数据类型
         data : Union[int, float, BaseType]
@@ -71,235 +62,267 @@
         tag_obj: SwanLabTag = self.tags.get(tag, None)
         """
         数据库创建字段将在chart创建完成后进行
         无论格式是否正确，都会创建chart，但是如果格式不正确，不会写入日志
         """
         if tag_obj is None:
             # 将此tag对象添加到实验列表中
-            tag_obj = SwanLabTag(self.id, tag, self.settings.log_dir)
+            tag_obj = SwanLabTag(tag, self.settings.log_dir)
             self.tags[tag] = tag_obj
             """
             由于添加图表的同时会尝试转换data的类型，但这在注入step之前
             所以此处需要手动注入依赖
             关于step，如果step格式不正确，会在tag_obj.add的时候被拦截，此处如果格式不正确直接设置为0即可
             """
             if isinstance(data, BaseType):
                 data.step = 0 if step is None or not isinstance(step, int) else step
                 data.tag = tag_obj.tag
-            result = tag_obj.create_chart(tag, data)
+            column_info = tag_obj.create_chart(tag, data)
+            self.warn_type_error(tag)
             # 创建新列，生成回调
-            self.__callbacks.on_column_create(*result)
+            self.__operator.on_column_create(column_info)
 
         # 检查tag创建时图表是否创建成功，如果失败则也没有写入数据的必要了，直接退出
         if not tag_obj.is_chart_valid:
-            return swanlog.warning(
-                f"swanlab: Chart '{tag}' creation failed. Reason: The expected value type for the chart '{tag}' is int ,float or BaseType, but the input type is {type(data)}. "
-            )
-
-        # 添加tag信息
+            self.warn_chart_error(tag)
+            return MetricInfo(key, tag_obj.column_info)
         key_info = tag_obj.add(data, step)
-        # 调用回调函数
-        self.__callbacks.on_metric_create(tag_obj.tag, key_info, self.settings.static_dir)
+        key_info.static_dir = self.settings.static_dir
+        return key_info
+
+    def warn_type_error(self, tag: str):
+        """警告类型错误
+        执行此方法时需保证tag已经存在
+        """
+        tag_obj = self.tags[tag]
+        class_name = tag_obj.now_data_type
+        excepted = tag_obj.expect_data_types
+        if tag_obj.is_chart_valid:
+            return
+        if class_name == "list":
+            swanlog.error(f"Data type error, tag: {tag}, there is element of invalid data type in the list.")
+        else:
+            swanlog.error(f"Data type error, tag: {tag}, data type: {class_name}, excepted: {excepted}")
+
+    def warn_chart_error(self, tag: str):
+        """
+        警告图表创建错误
+        执行此方法时需保证tag已经存在
+        """
+        tag_obj = self.tags[tag]
+        if tag_obj.is_chart_valid:
+            return
+        class_name = tag_obj.now_data_type
+        if class_name == "list":
+            swanlog.warning(
+                f"Chart '{tag}' creation failed. "
+                f"Reason: The data type in list of the tag '{tag}' is not as expected, please check the data type."
+            )
+        else:
+            swanlog.warning(
+                f"Chart '{tag}' creation failed. "
+                f"Reason: The expected value type for the chart '{tag}' is one of int,"
+                f"float or BaseType, but the input type is {class_name}."
+            )
 
 
 class SwanLabTag:
     """
     运行时每个tag的配置，用于记录一些信息
     包括每个tag专属的图表配置
     """
 
     # 每__slice_size个tag数据保存为一个文件
     __slice_size = 1000
 
-    def __init__(self, experiment_id, tag: str, log_dir: str) -> None:
+    def __init__(self, tag: str, log_dir: str) -> None:
         """
         初始化tag对象
 
         Parameters
         ----------
-        experiment_id : int
-            实验id
         tag : str
             tag名称
         log_dir : str
             log文件夹路径
         """
-        self.experiment_id = experiment_id
         self.tag = tag
         self.__steps = set()
-        """此tag已经包含的steps步骤
         """
-        self.__chart = None
-        """当前tag的图表配置"""
+        此tag已经包含的steps步骤
+        """
         self.__log_dir = log_dir
         """存储文件夹路径"""
         self.data_types = [float, int]
         """默认数据类型，如果tag数据为BaseType的子类，则使用其规定的数据类型"""
         self._summary = {}
         """数据概要总结"""
         self.__data = self.__new_tags()
         """当前tag的数据"""
-        self.__namespace = None
-        """当前tag自动生成图表的命名空间"""
         self.__error = None
         """此tag在自动生成chart的时候的错误信息"""
         self.data_type = None
         """当前tag的数据类型，如果是BaseType类型，则为BaseType的小写类名，否则为default"""
+        self.__column_info = None
+
+    @property
+    def now_data_type(self) -> Optional[str]:
+        """
+        当is_chart_valid为False时，返回当前数据的类型
+        这指的是用户传入的数据类型，而不是转换后的数据类型
+        """
+        if self.__error is not None:
+            return self.__error.get("data_class")
+        return None
+
+    @property
+    def expect_data_types(self) -> Optional[list]:
+        """
+        当is_chart_valid为False时，返回期望的数据类型
+        如果为True，则返回None
+        """
+        if self.__error is not None:
+            return self.__error.get("excepted")
+        return None
 
     @property
     def sum(self):
         """当前tag的数据总数"""
         return len(self.__steps)
 
     @property
+    def column_info(self):
+        """获取当前tag对应的ColumnInfo"""
+        return self.__column_info
+
+    @property
+    def chart_created(self):
+        """判断当前tag是否已经创建了图表"""
+        return self.__column_info is not None
+
+    @property
     def is_chart_valid(self) -> bool:
         """判断当前tag对应的自动创建图表是否成功
         成功则返回False，失败则返回True
         为True则一切正常
         为False则tag对应的路径不存在
         """
         return self.__error is None
 
     @staticmethod
     def __is_nan(data):
         """判断data是否为nan"""
         return isinstance(data, (int, float)) and math.isnan(data)
 
-    def add(self, data: DataType, step: int = None) -> NewKeyInfo:
+    def add(self, data: DataType, step: int = None) -> MetricInfo:
         """添加一个数据，在内部完成数据类型转换
         如果转换失败，打印警告并退出
         并且添加数据，当前的数据保存是直接保存，后面会改成缓存形式
 
         Parameters
         ----------
         data : DataType
             待添加的数据
         step : int, optional
             步数，如果不传则默认当前步数为'已添加数据数量+1'
+
+        Returns
+        -------
+        metric_info
+            添加数据的信息，如果ok为False，则返回None
+        ok
+            是否添加成功，如果当前step已经存在，或者类型转换失败，返回False
         """
-        # 如果step不是None也不是int，设置为None且打印警告
         if step is not None and not isinstance(step, int):
             swanlog.warning(f"Step {step} is not int, SwanLab will set it automatically.")
             step = None
-        # 转换step，如果step为None，则改为合适的长度，目前step从0开始
         if step is None:
             step = len(self.__steps)
-        # 如果step已经存在，打印警告并退出
         if step in self.__steps:
-            return swanlog.warning(f"Step {step} on tag {self.tag} already exists, ignored.")
-        # 添加数据，首先比较数据，如果数据比之前的数据大，则更新最大值，否则不更新
-        """
-        python环境下data可能是列表、字符串、整型、浮点型等
-        因此下面的summary还需要在未来做好兼容
-        对于整型和浮点型，还存在极大和极小值的问题
-        目前的策略是让python解释器自己处理，在前端完成数据的格式化展示
-        """
+            swanlog.warning(f"Step {step} on tag {self.tag} already exists, ignored.")
+            return MetricInfo(self.tag, self.__column_info)
         more = None if not isinstance(data, BaseType) else data.get_more()
         try:
             data = self.try_convert_after_add_chart(data, step)
         except ValueError:
-            return swanlog.warning(
-                f"Log failed. Reason: Data {data} on tag '{self.tag}' (step {step}) cannot be converted .It should be an int, float, or a DataType, but it is {type(data)}, please check the data type. "
+            swanlog.warning(
+                f"Log failed. Reason: Data {data} on tag '{self.tag}' (step {step}) cannot be converted .It should be "
+                f"an int, float, or a DataType, but it is {type(data)}, please check the data type."
             )
+            return MetricInfo(self.tag, self.__column_info)
         is_nan = self.__is_nan(data)
+        # 更新数据概要
         if not is_nan:
-            # 如果数据比之前的数据小，则更新最小值，否则不更新
             if self._summary.get("max") is None or data > self._summary["max"]:
                 self._summary["max"] = data
                 self._summary["max_step"] = step
             if self._summary.get("min") is None or data < self._summary["min"]:
                 self._summary["min"] = data
                 self._summary["min_step"] = step
         self._summary["num"] = self._summary.get("num", 0) + 1
         self.__steps.add(step)
         swanlog.debug(f"Add data, tag: {self.tag}, step: {step}, data: {data}")
-        # ---------------------------------- 保存数据 ----------------------------------
-        """添加数据到data中"""
         if len(self.__data["data"]) >= self.__slice_size:
-            # 如果当前数据已经达到了__slice_size，重新创建一个新的data
             self.__data = self.__new_tags()
-        # 添加数据
         data = data if not is_nan else "NaN"
         new_data = self.__new_tag(step, data, more=more)
         self.__data["data"].append(new_data)
-        # 优化文件分片，每__slice_size个tag数据保存为一个文件，通过sum来判断
         epoch = len(self.__steps)
         mu = math.ceil(epoch / self.__slice_size)
-        # 存储路径
         file_path = os.path.join(self.save_path, str(mu * self.__slice_size) + ".log")
-        # 更新实验信息总结
-        with open(os.path.join(self.save_path, "_summary.json"), "w+") as f:
-            ujson.dump(self._summary, f, ensure_ascii=False)
-        # 保存数据
-        with open(file_path, "a") as f:
-            f.write(ujson.dumps(new_data, ensure_ascii=False) + "\n")
-        # 深度拷贝，防止数据被修改
-        return json.loads(json.dumps(new_data)), self.data_type, step, epoch
+        return MetricInfo(
+            self.tag,
+            self.__column_info,
+            json.loads(json.dumps(new_data)),
+            json.loads(json.dumps(self._summary)),
+            self.data_type,
+            step,
+            epoch,
+            metric_path=file_path,
+            summary_path=os.path.join(self.save_path, "_summary.json"),
+            error=False,
+        )
 
     @property
     def save_path(self):
         """获取当前tag的保存路径
 
         Returns
         -------
         str
             保存路径
         """
         path = os.path.join(self.__log_dir, quote(self.tag, safe=""))
-        if not os.path.exists(path):
-            os.mkdir(path)
         return path
 
-    def create_chart(self, tag: str, data: DataType) -> Tuple[str, str, Optional[Dict]]:
+    def create_chart(self, tag: str, data: DataType) -> ColumnInfo:
         """在第一次添加tag的时候，自动创建图表和namespaces，同时写入tag和数据库信息，将创建的信息保存到数据库中
         此方法只能执行一次
         具体步骤是：
         1. 创建tag字段
         2. 如果不是baseType类型，
-
-
         :returns tag, chart_type, error
-        [WARNING] 返回位置需与回调函数入参位置一致
+
+        WARNING 返回位置需与回调函数入参位置一致
         """
-        if self.__namespace is not None or self.__chart is not None:
+        if self.chart_created:
             raise ValueError(f"Chart {tag} has been created, cannot create again.")
-
         # 如果是非BaseType类型，写入默认命名空间，否则写入BaseType指定的命名空间
+        sort = 0
         if not isinstance(data, BaseType):
-            # data_type不变
             namespace, chart_type, reference, config = "default", "default", "step", None
-            sort = 0
             data_type = "default"
         else:
-            # 解构数据
             namespace, types, reference, config = data.__next__()
             chart_type, self.data_types = types
-            sort = None
             data_type = data.__class__.__name__.lower()
-        # 创建chart
-        self.__chart: Chart = Chart.create(
-            tag,
-            experiment_id=self.experiment_id,
-            type=chart_type,
-            reference=reference,
-            config=config,
-        )
-        # 创建命名空间，如果命名空间已经存在，会抛出ExistedError异常，捕获不处理即可
-        # 需要指定sort，default命名空间的sort为0，其他命名空间的sort为None，表示默认添加到最后
-        try:
-            # 对于namespace，如果tag的名称存在斜杠，则使用斜杠前的部分作为namespace的名称
-            if len(tag.split("/")) > 1:
-                namespace = tag.split("/")[0]
-            self.__namespace = Namespace.create(name=namespace, experiment_id=self.experiment_id, sort=sort)
-            swanlog.debug(f"Namespace {namespace} created, id: {self.__namespace.id}")
-        except ExistedError:
-            self.__namespace: Namespace = Namespace.get(name=namespace, experiment_id=self.experiment_id)
-            swanlog.debug(f"Namespace {namespace} exists, id: {self.__namespace.id}")
-        # 创建display，这个必然是成功的，因为display是唯一的，直接添加到最后一条即可
-        Display.create(chart_id=self.__chart.id, namespace_id=self.__namespace.id)
+        # 对于namespace，如果tag的名称存在斜杠，则使用斜杠前的部分作为namespace的名称
+        if "/" in tag and tag[0] != "/":
+            namespace = tag.split("/")[0]
+            sort = None
         """
         接下来判断tag格式的正确性，判断完毕后往source中添加一条tag记录
         在此函数中，只判断tag的格式是否正确，不记录数据
         在逻辑上只有第一次会检查tag的正确性，也就是说前端的error错误只有在第一次添加tag的时候才有可能出现
         如果第一次添加成功，后续出现错误，只会在添加的时候warning一下然后丢弃这个错误
         如果第一次添加失败，后续都不会再添加此数据，因此不会出现错误
         """
@@ -313,35 +336,22 @@
                 # 此时代表数据异常，拿到data的__class__.__name__，生成error并保存
                 if isinstance(data, BaseType):
                     class_name = data.value.__class__.__name__
                     excepted = data.expect_types()
                 else:
                     class_name = data.__class__.__name__
                     excepted = [i.__name__ for i in self.data_types]
-                swanlog.error(f"Data type error, tag: {tag}, data type: {class_name}, excepted: {excepted}")
                 error = {"data_class": class_name, "excepted": excepted}
         if self.__is_nan(data):
-            """如果data是nan，生成error并保存"""
             error = {"data_class": "NaN", "excepted": [i.__name__ for i in self.data_types]}
-        tag: Tag = Tag.create(
-            experiment_id=self.experiment_id,
-            name=tag,
-            # 如果data是BaseType类型，使用data的小写类名，否则使用default
-            type=data_type,
-        )
-        self.data_type = data_type
-        # 添加一条source记录
-        Source.create(tag_id=tag.id, chart_id=self.__chart.id, error=error)
+        column_info = ColumnInfo(tag, namespace, data_type, chart_type, sort, error, reference, config)
         self.__error = error
-        # 新建多实验对比图表数据
-        try:
-            add_multi_chart(tag_id=tag.id, chart_id=self.__chart.id)
-        except ChartTypeError:
-            swanlog.warning("In the multi-experiment chart, the current type of tag is not as expected.")
-        return tag.name, chart_type, error
+        self.data_type = data_type
+        self.__column_info = column_info
+        return column_info
 
     @staticmethod
     def __new_tag(index, data, more: dict = None) -> dict:
         """创建一个新的data数据，实际上是一个字典，包含一些默认信息
 
         Parameters
         ----------
```

### Comparing `swanlab-0.3.3/swanlab/data/run/main.py` & `swanlab-0.3.4/swanlab/data/run/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,31 +4,24 @@
 @DATE: 2024-01-01 15:58:58
 @File: swanlab/data/run/main.py
 @IDE: vscode
 @Description:
     在此处定义SwanLabRun类并导出
 """
 from ..settings import SwanDataSettings
-from ..system import get_system_info, get_requirements
 from swanlab.log import swanlog
-from swanlab.utils.file import (
-    check_exp_name_format,
-    check_desc_format,
-)
-from swanlab.db import Experiment, ExistedError, NotExistedError
 from swanlab.data.modules import BaseType
 from swanlab.data.config import SwanLabConfig
-import time
 import random
-import ujson
 from enum import Enum
 from .exp import SwanLabExp
 from datetime import datetime
-from typing import Tuple, Callable, Optional, Dict
-from .callback import SwanLabRunCallback, EmptyCallback
+from typing import Callable, Optional, Dict
+from .operator import SwanLabRunOperator
+from swanlab.env import get_mode, SwanLabMode
 
 
 class SwanLabRunState(Enum):
     """SwanLabRunState is an enumeration class that represents the state of the experiment.
     We Recommend that you use this enumeration class to represent the state of the experiment.
     """
     NOT_STARTED = -2
@@ -41,27 +34,30 @@
     """
     The SwanLabRun class is used for logging during a single experiment.
     There should be only one instance of the SwanLabRun class for each experiment.
     """
 
     def __init__(
         self,
+        project_name: str = None,
         experiment_name: str = None,
         description: str = None,
         config: dict = None,
         log_level: str = None,
         suffix: str = None,
         exp_num: int = None,
-        callbacks: SwanLabRunCallback = None
+        operator: SwanLabRunOperator = SwanLabRunOperator(),
     ):
         """
         Initializing the SwanLabRun class involves configuring the settings and initiating other logging processes.
 
         Parameters
         ----------
+        project_name : str, optional
+            项目名称，目前单纯做一个记录
         experiment_name : str, optional
             实验名称，实验名称应该唯一，由0-9，a-z，A-Z，" ","_","-","/"组成
             如果不提供此参数(为None)，SwanLab将自动生成一个实验名称
         description : str, optional
             实验描述，用于对当前实验进行更详细的介绍或标注
             如果不提供此参数(为None)，可以在web界面中进行修改,这意味着必须在此改为空字符串""
         config : dict, optional
@@ -72,65 +68,70 @@
             不区分大小写，如果不提供此参数(为None)，则默认为 'info'
             如果提供的日志等级不在上述范围内，默认改为info
         suffix : str, optional
             实验名称后缀，用于区分同名实验，格式为yyyy-mm-dd_HH-MM-SS
             如果不提供此参数(为None)，不会添加后缀
         exp_num : int, optional
             历史实验总数，用于云端颜色与本地颜色的对应
-        callbacks : Dict[str, Callable]
-            回调函数字典，key为回调函数名，value为回调函数
+        operator : SwanLabRunOperator, optional
+            实验操作员，用于批量处理回调函数的调用，如果不提供此参数(为None)，则会自动生成一个实例
         """
         global run
         if run is not None:
             raise RuntimeError("SwanLabRun has been initialized")
         # ---------------------------------- 初始化类内参数 ----------------------------------
+        self.__project_name = project_name
         # 生成一个唯一的id，随机生成一个8位的16进制字符串，小写
         _id = hex(random.randint(0, 2 ** 32 - 1))[2:].zfill(8)
         timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
         self.__run_id = "run-{}-{}".format(timestamp, _id)
-        # 初始化配置
-        self.__settings = SwanDataSettings(run_id=self.__run_id)
-        # 初始化回调
-        self.__callbacks: SwanLabRunCallback = callbacks if callbacks is not None else EmptyCallback()
-        # 注入依赖
-        self.__callbacks.inject(self.__settings)
+        # 操作员初始化
+        self.__operator = SwanLabRunOperator() if operator is None else operator
+        self.__settings = SwanDataSettings(run_id=self.__run_id, should_save=not self.__operator.disabled)
+        self.__operator.inject(self.__settings)
         # ---------------------------------- 初始化日志记录器 ----------------------------------
         # output、console_dir等内容不依赖于实验名称的设置
-        swanlog.install(self.__settings.console_dir, self.__check_log_level(log_level))
+        swanlog.set_level(self.__check_log_level(log_level))
         # ---------------------------------- 初始化配置 ----------------------------------
         # 给外部1个config
         self.__config = SwanLabConfig(config, self.__settings)
         # ---------------------------------- 注册实验 ----------------------------------
-        # 校验描述格式
-        description = self.__check_description(description)
         self.__exp: SwanLabExp = self.__register_exp(experiment_name, description, suffix, num=exp_num)
         # 实验状态标记，如果status不为0，则无法再次调用log方法
         self.__state = SwanLabRunState.RUNNING
 
         # 动态定义一个方法，用于修改实验状态
         def _(state: SwanLabRunState):
             self.__state = state
 
         global _change_run_state
         _change_run_state = _
         run = self
 
         # ---------------------------------- 初始化完成 ----------------------------------
-        self.__callbacks.on_train_begin()
+        self.__operator.on_run()
 
     @property
-    def callbacks(self) -> SwanLabRunCallback:
-        return self.__callbacks
+    def operator(self) -> SwanLabRunOperator:
+        return self.__operator
+
+    @property
+    def project_name(self) -> str:
+        return self.__project_name
+
+    @property
+    def mode(self) -> str:
+        return get_mode()
 
     @property
     def state(self) -> SwanLabRunState:
         return self.__state
 
-    @staticmethod
-    def get_state() -> SwanLabRunState:
+    @classmethod
+    def get_state(cls) -> SwanLabRunState:
         """
         获取当前实验状态
         """
         global run
         return run.state if run is not None else SwanLabRunState.NOT_STARTED
 
     @property
@@ -164,24 +165,22 @@
         # 3. 清空run对象，run改为局部变量_run
         # 4. 返回_run
         if run is None:
             raise RuntimeError("The run object is None, please call `swanlab.init` first.")
         if state == SwanLabRunState.CRASHED and error is None:
             raise ValueError("When the state is 'CRASHED', the error message cannot be None.")
         _set_run_state(state)
-        # 写入错误信息
-        if state == SwanLabRunState.CRASHED:
-            with open(run.settings.error_path, "a") as fError:
-                print(datetime.now(), file=fError)
-                print(error, file=fError)
-        else:
-            error = None
+        error = error if state == SwanLabRunState.CRASHED else None
         # 退出回调
-        run.callbacks.on_train_end(error)
-        swanlog.uninstall()
+        run.operator.on_stop(error)
+        try:
+            swanlog.uninstall()
+        except RuntimeError:
+            # disabled 模式下没有install，所以会报错
+            pass
         _run, run = run, None
         return _run
 
     @property
     def settings(self) -> SwanDataSettings:
         """
         This property allows you to access the 'settings' content passed through `init`,
@@ -220,186 +219,91 @@
             The value must be a `float`, `float convertible object`, `int` or `swanlab.data.BaseType`.
         step : int, optional
             The step number of the current data, if not provided, it will be automatically incremented.
             If step is duplicated, the data will be ignored.
         """
         if self.__state != SwanLabRunState.RUNNING:
             raise RuntimeError("After experiment finished, you can no longer log data to the current experiment")
-        # 每一次log的时候检查一下数据库中的实验状态
-        # 如果实验状态不为0，说明实验已经结束，不允许再次调用log方法
-        # 这意味着每次log都会进行查询，比较消耗性能，后续考虑采用多进程共享内存的方式进行优化
-        swanlog.debug(f"Check experiment and state...")
-        try:
-            exp = Experiment.get(self.__exp.id)
-        except NotExistedError:
-            raise KeyboardInterrupt("The experiment has been deleted by the user")
-        # 此时self.__state == 0，说明是前端主动停止的
-        if exp.status != 0:
-            raise KeyboardInterrupt("The experiment has been stopped by the user")
+        self.__operator.on_log()
 
         if not isinstance(data, dict):
             return swanlog.error(
                 "log data must be a dict, but got {}, SwanLab will ignore records it.".format(type(data))
             )
         # 检查step的类型
         if step is not None and (not isinstance(step, int) or step < 0):
             swanlog.error(
                 "'step' must be an integer not less than zero, but got {}, SwanLab will automatically set step".format(
                     step
                 )
             )
             step = None
+
+        log_return = {}
         # 遍历data，记录data
         for key in data:
             # 遍历字典的key，记录到本地文件中
             d = data[key]
             # 如果d的数据类型是list，且里面的数据全部为Image类型，则需要转换一下
             if isinstance(d, list) and all([isinstance(i, BaseType) for i in d]) and len(d) > 0:
                 # 将d作为输入，构造一个与d相同类型的实例
                 d = d[0].__class__(d)
             # 数据类型的检查将在创建chart配置的时候完成，因为数据类型错误并不会影响实验进行
-            self.__exp.add(key=key, data=d, step=step)
+            metric_info = self.__exp.add(key=key, data=d, step=step)
+            self.__operator.on_metric_create(metric_info)
+            log_return[metric_info.key] = metric_info
+
+        return log_return
 
     def __str__(self) -> str:
         """此类的字符串表示"""
         return self.__run_id
 
-    @staticmethod
-    def __get_exp_name(experiment_name: str = None, suffix: str = None) -> Tuple[str, str]:
-        """
-        预处理实验名称，如果实验名称过长，截断
-
-        Parameters
-        ----------
-        experiment_name : str
-            实验名称
-        suffix : str
-            实验名称后缀添加方式，可以为None、"default"或自由后缀，前者代表不添加后缀，后者代表添加时间戳后缀
-
-        Returns
-        ----------
-        experiment_name : str
-            校验后的实验名称
-        exp_name : str
-            最终的实验名称
-        """
-        # ---------------------------------- 校验实验名称 ----------------------------------
-        experiment_name = "exp" if experiment_name is None else experiment_name
-        # 校验实验名称
-        experiment_name_checked = check_exp_name_format(experiment_name)
-        # 如果实验名称太长的tip
-        tip = "The experiment name you provided is too long, it has been truncated automatically."
-
-        # 如果前后长度不一样，说明实验名称被截断了，提醒
-        if len(experiment_name_checked) != len(experiment_name) and suffix is None:
-            swanlog.warning(tip)
-
-        # 如果suffix为None, 则不添加后缀，直接返回
-        if suffix is None or suffix is False:
-            return experiment_name_checked, experiment_name
-
-        # 如果suffix为True, 则添加默认后缀
-        if suffix is True:
-            suffix = "default"
-
-        # suffix必须是字符串
-        if not isinstance(suffix, str):
-            raise TypeError("The suffix must be a string, but got {}".format(type(suffix)))
-
-        # 如果suffix_checked为default，则设置为默认后缀
-        if suffix.lower().strip() == "default":
-            # 添加默认后缀
-            default_suffix = "{}".format(datetime.now().strftime("%b%d_%H-%M-%S"))
-            exp_name = "{}_{}".format(experiment_name_checked, default_suffix)
-        else:
-            exp_name = "{}_{}".format(experiment_name_checked, suffix)
-
-        # 校验实验名称，如果实验名称过长，截断
-        experiment_name_checked = check_exp_name_format(exp_name)
-        if len(experiment_name_checked) != len(exp_name):
-            swanlog.warning(tip)
-
-        return experiment_name_checked, exp_name
-
     def __register_exp(
         self,
         experiment_name: str,
         description: str = None,
         suffix: str = None,
         num: int = None,
     ) -> SwanLabExp:
         """
         注册实验，将实验配置写入数据库中，完成实验配置的初始化
         """
-        # 这个循环的目的是如果创建失败则等零点五秒重新生成后缀重新创建，直到创建成功
-        # 但是由于需要考虑suffix为none不生成后缀的情况，所以需要在except中判断一下
-        old = experiment_name
-        exp = None
-        while True:
-            experiment_name, exp_name = self.__get_exp_name(old, suffix)
-            try:
-                # 获得数据库实例
-                exp = Experiment.create(name=exp_name, run_id=self.__run_id, description=description, num=num)
-                break
-            except ExistedError:
-                # 如果suffix名为default，说明是自动生成的后缀，需要重新生成后缀
-                if isinstance(suffix, str) and suffix.lower().strip() == "default":
-                    swanlog.debug(f"Experiment {exp_name} has existed, try another name...")
-                    time.sleep(0.5)
-                    continue
-                # 其他情况下，说明是用户自定义的后缀，需要报错
-                else:
-                    Experiment.purely_delete(run_id=self.__run_id)
-                    raise ExistedError(f"Experiment {exp_name} has existed in local, please try another name.")
-
-        # 实验创建成功，设置实验相关信息
-        self.__settings.exp_name = exp_name
-        self.settings.exp_colors = (exp.light, exp.dark)
-        self.settings.description = description
-        # 执行一些记录操作
-        self.__record_exp_config()  # 记录实验配置
-        return SwanLabExp(self.__settings, exp.id, exp=exp, callbacks=self.__callbacks)
+
+        # ---------------------------------- 初始化实验 ----------------------------------
+
+        def setter(exp_name: str, light_color: str, dark_color: str, desc: str):
+            """
+            设置实验相关信息
+            :param exp_name: 实验名称
+            :param light_color: 亮色
+            :param dark_color: 暗色
+            :param desc: 实验描述
+            :return:
+            """
+            # 实验创建成功，设置实验相关信息
+            self.__settings.exp_name = exp_name
+            self.settings.exp_colors = (light_color, dark_color)
+            self.settings.description = desc
+
+        self.__operator.before_init_experiment(self.__run_id, experiment_name, description, num, suffix, setter)
+        return SwanLabExp(self.__settings, operator=self.__operator)
 
     @staticmethod
     def __check_log_level(log_level: str) -> str:
         """检查日志等级是否合法"""
         valid = ["debug", "info", "warning", "error", "critical"]
         if log_level is None:
             return "info"
         elif log_level.lower() in valid:
             return log_level.lower()
         else:
             swanlog.warning(f"The log level you provided is not valid, it has been set to {log_level}.")
             return "info"
 
-    @staticmethod
-    def __check_description(description: str) -> str:
-        """检查实验描述是否合法"""
-        if description is None:
-            return ""
-        desc = check_desc_format(description)
-        if desc != description:
-            swanlog.warning("The description has been truncated automatically.")
-        return desc
-
-    def __record_exp_config(self):
-        """创建实验配置目录 files
-        - 创建 files 目录
-        - 将实验环境写入 files/swanlab-metadata.json 中
-        - 将实验依赖写入 files/requirements.txt 中
-        """
-        requirements_path = self.__settings.requirements_path
-        metadata_path = self.__settings.metadata_path
-        # 将实验依赖存入 requirements.txt
-        with open(requirements_path, "w") as f:
-            f.write(get_requirements())
-        # 将实验环境(硬件信息、git信息等等)存入 swanlab-metadata.json
-        with open(metadata_path, "w") as f:
-            ujson.dump(get_system_info(self.__settings), f)
-
 
 run: Optional["SwanLabRun"] = None
 """Global runtime instance. After the user calls finish(), run will be set to None."""
 _change_run_state: Optional["Callable"] = None
 """
 修改实验状态的函数，用于在实验状态改变时调用
 """
@@ -414,16 +318,14 @@
 
     if state not in SwanLabRunState or state in [SwanLabRunState.NOT_STARTED, SwanLabRunState.RUNNING]:
         swanlog.warning("Invalid state when set, state must be in SwanLabRunState and not be RUNNING or NOT_STARTED")
         swanlog.warning("SwanLab will set state to `CRASHED`")
         state = SwanLabRunState.CRASHED
     # 设置state
     _change_run_state(state)
-    # 更新数据库中的实验状态
-    run.exp.db.update_status(state.value)
 
 
 def get_run() -> Optional["SwanLabRun"]:
     """
     Get the current run object. If the experiment has not been initialized, return None.
     """
     global run
```

### Comparing `swanlab-0.3.3/swanlab/data/system/info.py` & `swanlab-0.3.4/swanlab/data/system/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/system/monitor.py` & `swanlab-0.3.4/swanlab/data/system/monitor.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/data/system/bin/apple_gpu_stats` & `swanlab-0.3.4/swanlab/data/system/bin/apple_gpu_stats`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/__init__.py` & `swanlab-0.3.4/swanlab/db/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,7 +26,8 @@
     ForeignChartNotExistedError,
     ForeignNameNotExistedError,
     ChartTypeError,
 )
 from .table_config import tables
 from .db_connect import connect
 from .utils import add_multi_chart
+from .callback import GlomCallback
```

### Comparing `swanlab-0.3.3/swanlab/db/db_connect.py` & `swanlab-0.3.4/swanlab/db/db_connect.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/error.py` & `swanlab-0.3.4/swanlab/db/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/model.py` & `swanlab-0.3.4/swanlab/db/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/docs/Errors.md` & `swanlab-0.3.4/swanlab/db/docs/Errors.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/docs/README.md` & `swanlab-0.3.4/swanlab/db/docs/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/migrate/chart.py` & `swanlab-0.3.4/swanlab/db/migrate/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/migrate/experiment.py` & `swanlab-0.3.4/swanlab/db/migrate/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/migrate/namespace.py` & `swanlab-0.3.4/swanlab/db/migrate/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/migrate/project.py` & `swanlab-0.3.4/swanlab/db/migrate/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/models/charts.py` & `swanlab-0.3.4/swanlab/db/models/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/models/displays.py` & `swanlab-0.3.4/swanlab/db/models/displays.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/models/experiments.py` & `swanlab-0.3.4/swanlab/db/models/experiments.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,31 +164,14 @@
                 dark=dark,
             )
         except IntegrityError:
             raise ExistedError("实验已经存在")
 
     @classmethod
     def get(cls, *args, **kwargs) -> "Experiment":
-        """覆写继承的get方法，通过id获取实验实例
-
-        Parameters
-        ----------
-        id : int
-            实验id
-
-        Returns
-        -------
-        Experiment
-            实验实例
-
-        Raises
-        -------
-        NotExistedError
-            实验不存在
-        """
         try:
             return super().get(*args, **kwargs)
         except:
             raise NotExistedError("Experiment does not exist: {}".format(kwargs))
 
     def update_status(self, status: int):
         """更新实验状态
@@ -199,29 +182,27 @@
             实验状态
         """
         self.status = status
         self.finish_time = create_time()
         self.save()
 
     @classmethod
-    def purely_delete(cls, **kwargs):
+    def purely_delete(cls, run_id: str):
         """
         删除某一个实验，顺便删除实验的文件夹
 
         Parameters
         ----------
-        id : int
-            实验id
+        run_id : int
+            实验run_id
         """
         # 获取实验实例
         try:
-            exp = cls.get(**kwargs)
+            exp = cls.get(run_id=run_id)
             # 删除实验
             exp.delete_instance()
             # 更新项目的实验数量
             Project.decrease_sum()
             # 删除实验文件夹
             shutil.rmtree(os.path.join(get_swanlog_dir(), exp.run_id.__str__()))
         except NotExistedError:
-            # 删除实验文件夹
-            if "run_id" in kwargs:
-                shutil.rmtree(os.path.join(get_swanlog_dir(), kwargs["run_id"]))
+            shutil.rmtree(os.path.join(get_swanlog_dir(), run_id))
```

### Comparing `swanlab-0.3.3/swanlab/db/models/namespaces.py` & `swanlab-0.3.4/swanlab/db/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/models/projects.py` & `swanlab-0.3.4/swanlab/db/models/projects.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/models/sources.py` & `swanlab-0.3.4/swanlab/db/models/sources.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/models/tags.py` & `swanlab-0.3.4/swanlab/db/models/tags.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/db/utils/chart.py` & `swanlab-0.3.4/swanlab/db/utils/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/fastai.py` & `swanlab-0.3.4/swanlab/integration/fastai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Docs: https://docs.swanlab.cn/zh/guide_cloud/integration/integration-fastai.html
+"""
+
 try:
     from fastai.learner import Callback
     from fastcore.basics import store_attr, detuplify, ignore_exceptions
     from fastai.callback.hook import total_params
 except ImportError:
     raise RuntimeError(
         "This module requires `fastai` to be installed. " "Please install it with command: \n pip install fastai"
```

### Comparing `swanlab-0.3.3/swanlab/integration/huggingface.py` & `swanlab-0.3.4/swanlab/integration/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Docs: https://docs.swanlab.cn/zh/guide_cloud/integration/integration-huggingface-transformers.html
+"""
+
 from typing import Optional, List, Dict, Union, Any
 import swanlab
 
 try:
     from transformers.trainer_callback import TrainerCallback
 except ImportError:
     raise RuntimeError(
```

### Comparing `swanlab-0.3.3/swanlab/integration/mmengine.py` & `swanlab-0.3.4/swanlab/integration/mmengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+Docs: https://docs.swanlab.cn/zh/guide_cloud/integration/integration-mmengine.html
+
 For adaptation to the mmengine framework, this adaptation also applies to frameworks such as mmdetection, xtuner, etc.
 , which use mmengine as the engine. By setting 'vis_backends' to 'swanlab' in the config file, experiment logs can be
 uploaded to SwanLab or viewed using the local version of SwanLab. Detailed configuration file changes are as follows:
 ------config.py in mmengine------
 ...
 custom_imports = dict(
     imports=["swanlab.integration.mmengine"], allow_failed_imports=False
@@ -105,14 +107,15 @@
     @force_init_env
     def add_config(self, config: Config, **kwargs) -> None:
         """Record the config to swanlab.
 
         Args:
             config (Config): The Config object
         """
+
         def repack_dict(a, prefix=""):
             """
             Unpack Nested Dictionary func
             """
             new_dict = dict()
             for key, value in a.items():
                 key = str(key)
```

### Comparing `swanlab-0.3.3/swanlab/integration/pytorch_lightning.py` & `swanlab-0.3.4/swanlab/integration/pytorch_lightning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Docs:https://docs.swanlab.cn/zh/guide_cloud/integration/integration-pytorch-lightning.html
+"""
+
 import os
 import importlib.util
 from typing import Any, Dict, Optional, Union, Mapping, List
 from argparse import Namespace
 import packaging.version
 from pathlib import Path
```

### Comparing `swanlab-0.3.3/swanlab/integration/integration_utils/autologging.py` & `swanlab-0.3.4/swanlab/integration/integration_utils/autologging.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/integration_utils/get_modules.py` & `swanlab-0.3.4/swanlab/integration/integration_utils/get_modules.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/integration_utils/timer.py` & `swanlab-0.3.4/swanlab/integration/integration_utils/timer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/openai/openai.py` & `swanlab-0.3.4/swanlab/integration/openai/openai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/openai/resolver.py` & `swanlab-0.3.4/swanlab/integration/openai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/zhipuai/resolver.py` & `swanlab-0.3.4/swanlab/integration/zhipuai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/integration/zhipuai/zhipuai.py` & `swanlab-0.3.4/swanlab/integration/zhipuai/zhipuai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/log/console.py` & `swanlab-0.3.4/swanlab/log/console.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/log/log.py` & `swanlab-0.3.4/swanlab/log/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,32 +120,37 @@
     }
 
     def __init__(self, name=__name__.lower(), level="info"):
         super().__init__()
         self.prefix = name + ':'
         self.__logger = logging.getLogger(name)
         self.__original_level = self._get_level(level)
-        self.__now_level = None
-        # 设置日志等级
+        self.__installed = False
         self.__logger.setLevel(self.__original_level)
         # 初始化控制台日志处理器
         self.__handler = logging.StreamHandler(sys.stdout)
         # 添加颜色格式化，并在此处设置格式化后的输出流是否可以被其他处理器处理
         colored_formatter = ColoredFormatter("%(name)s: %(message)s")
         self.__handler.setFormatter(colored_formatter)
-        self.__logger.addHandler(self.__handler)
+        self.enable_log()
         # 控制台监控记录器
         self.__consoler = SwanConsoler()
 
+    def disable_log(self):
+        self.__logger.removeHandler(self.__handler)
+
+    def enable_log(self):
+        self.__logger.addHandler(self.__handler)
+
     @property
     def installed(self):
         """
         判断是否已经install
         """
-        return self.__now_level is not None
+        return self.__installed
 
     def install(self, console_dir: str = None, log_level: str = None) -> "SwanLog":
         """
         初始化安装日志系统，同一实例在没有执行uninstall的情况下，不可重复安装
         功能是开启标准输出流拦截功能，并设置日志等级
         :param console_dir: 控制台日志文件路径文件夹，如果提供，则会将控制台日志记录到对应文件夹，否则不记录，需要保证文件夹存在
         :param log_level: 日志等级，可以是 "debug", "info", "warning", "error", 或 "critical"，默认为info
@@ -155,35 +160,35 @@
         :raises: RuntimeError: 已经安装过日志系统
         :raises: KeyError: 无效的日志级别
         :raises: FileNotFoundError: 控制台日志文件夹不存在
         """
         if self.installed:
             raise RuntimeError("SwanLog has been installed")
         # 设置日志等级
-        log_level = log_level if log_level else "info"
-        self.__now_level = self._get_level(log_level)
-        self.__logger.setLevel(self.__now_level)
+        if log_level is not None:
+            self.set_level(log_level)
         # 初始化控制台记录器
         if console_dir:
             self.debug("Init consoler to record console log")
             self.__consoler.install(console_dir)
+        self.__installed = True
         return self
 
     def uninstall(self):
         """
         卸载日志系统，卸载后需要重新安装
         在设计上我们并不希望外界乱用这个函数，所以我们不提供外部调用（不在最外层的__all__中）
         此时将卸载标准输出流拦截功能，并重置日志等级为初始化时的等级
         """
         if not self.installed:
             raise RuntimeError("SwanLog has not been installed")
         self.debug("uninstall swanlog, reset consoler")
         self.__logger.setLevel(self.__original_level)
-        self.__now_level = None
         self.__consoler.uninstall()
+        self.__installed = False
 
     @property
     def write_callback(self):
         return self.__consoler.write_callback
 
     def set_write_callback(self, func):
         self.__consoler.set_write_callback(func)
```

### Comparing `swanlab-0.3.3/swanlab/server/app.py` & `swanlab-0.3.4/swanlab/server/app.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/settings.py` & `swanlab-0.3.4/swanlab/server/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/chart.py` & `swanlab-0.3.4/swanlab/server/controller/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/experiment.py` & `swanlab-0.3.4/swanlab/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/namespace.py` & `swanlab-0.3.4/swanlab/server/controller/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/project.py` & `swanlab-0.3.4/swanlab/server/controller/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/utils/__init__.py` & `swanlab-0.3.4/swanlab/server/controller/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/utils/charts.py` & `swanlab-0.3.4/swanlab/server/controller/utils/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/controller/utils/tag.py` & `swanlab-0.3.4/swanlab/server/controller/utils/tag.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/middleware/common.py` & `swanlab-0.3.4/swanlab/server/middleware/common.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/module/resp.py` & `swanlab-0.3.4/swanlab/server/module/resp.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/router/chart.py` & `swanlab-0.3.4/swanlab/server/router/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/router/experiment.py` & `swanlab-0.3.4/swanlab/server/router/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/router/media.py` & `swanlab-0.3.4/swanlab/server/router/media.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/router/namespace.py` & `swanlab-0.3.4/swanlab/server/router/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/server/router/project.py` & `swanlab-0.3.4/swanlab/server/router/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/ChartPage-C2Rj7xI3.js` & `swanlab-0.3.4/swanlab/template/assets/ChartPage-C2Rj7xI3.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/ChartsView-DpI6U3QH.js` & `swanlab-0.3.4/swanlab/template/assets/ChartsView-DpI6U3QH.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/EnvHardware-4H7mp2Bs.js` & `swanlab-0.3.4/swanlab/template/assets/EnvHardware-4H7mp2Bs.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/EnvIndex-B5_l1b65.js` & `swanlab-0.3.4/swanlab/template/assets/EnvIndex-B5_l1b65.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/EnvItems-B4PwmQT4.js` & `swanlab-0.3.4/swanlab/template/assets/EnvItems-B4PwmQT4.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/EnvItems-BfjcRO-X.css` & `swanlab-0.3.4/swanlab/template/assets/EnvItems-BfjcRO-X.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js` & `swanlab-0.3.4/swanlab/template/assets/EnvRequirements-Cpn2Fk1D.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js` & `swanlab-0.3.4/swanlab/template/assets/EnvironmentPage-Bb8ousXq.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/ExperimentView-BTbu21ka.js` & `swanlab-0.3.4/swanlab/template/assets/ExperimentView-BTbu21ka.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/ExperimentView-CCDMXo4h.css` & `swanlab-0.3.4/swanlab/template/assets/ExperimentView-CCDMXo4h.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/FuncBar-Ct_nBdvU.js` & `swanlab-0.3.4/swanlab/template/assets/FuncBar-Ct_nBdvU.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/HomeView-BS7FyMAt.css` & `swanlab-0.3.4/swanlab/template/assets/HomeView-BS7FyMAt.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/HomeView-BqTu9_fG.js` & `swanlab-0.3.4/swanlab/template/assets/HomeView-BqTu9_fG.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/IndexPage-C5dvtib2.css` & `swanlab-0.3.4/swanlab/template/assets/IndexPage-C5dvtib2.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/IndexPage-CrqN4Ekl.js` & `swanlab-0.3.4/swanlab/template/assets/IndexPage-CrqN4Ekl.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf` & `swanlab-0.3.4/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/LogPage-B-fC6sB7.js` & `swanlab-0.3.4/swanlab/template/assets/LogPage-B-fC6sB7.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/LogPage-DBzoauOW.css` & `swanlab-0.3.4/swanlab/template/assets/LogPage-DBzoauOW.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/NotFound-DijsQ96i.js` & `swanlab-0.3.4/swanlab/template/assets/NotFound-DijsQ96i.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/SLLoading-6DfF2aH0.js` & `swanlab-0.3.4/swanlab/template/assets/SLLoading-6DfF2aH0.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/SLStatusLabel-BRacn5XK.css` & `swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-BRacn5XK.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js` & `swanlab-0.3.4/swanlab/template/assets/SLStatusLabel-DvEKZN8v.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf` & `swanlab-0.3.4/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/chart-DB312WPs.css` & `swanlab-0.3.4/swanlab/template/assets/chart-DB312WPs.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/chart-eW1meEc1.js` & `swanlab-0.3.4/swanlab/template/assets/chart-eW1meEc1.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/index-B5SDzoY4.js` & `swanlab-0.3.4/swanlab/template/assets/index-B5SDzoY4.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/index-B7Izi8NT.css` & `swanlab-0.3.4/swanlab/template/assets/index-B7Izi8NT.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/template/assets/logo-ChHf2ozk.ico` & `swanlab-0.3.4/swanlab/template/assets/logo-ChHf2ozk.ico`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/utils/file.py` & `swanlab-0.3.4/swanlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/utils/font.py` & `swanlab-0.3.4/swanlab/utils/font.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/utils/judgment.py` & `swanlab-0.3.4/swanlab/utils/judgment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/swanlab/utils/key.py` & `swanlab-0.3.4/swanlab/utils/key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/create_experiment.py` & `swanlab-0.3.4/test/create_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 offset = random.random() / 5
 # 初始化
 swanlab.init(
     description="这是一个测试实验",
     log_level="debug",
     config="test/config/config.json",
     load="test/config/load.yaml",
-    cloud=True,
+    mode="cloud",
 )
 swanlab.config.epoches = epochs
 swanlab.config.learning_rate = lr
 swanlab.config.debug = "这是一串" + "很长" * 100 + "的字符串"
 # 模拟训练
 for epoch in range(2, swanlab.config.epoches):
     acc = 1 - 2 ** -epoch - random.random() / epoch - offset
```

### Comparing `swanlab-0.3.3/test/start_server.py` & `swanlab-0.3.4/test/start_server.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/use_swanlog.py` & `swanlab-0.3.4/test/use_swanlog.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/pytest_example.py` & `swanlab-0.3.4/test/unit/pytest_example.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/auth/pytest_login.py` & `swanlab-0.3.4/test/unit/auth/pytest_login.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/log/pytest_log.py` & `swanlab-0.3.4/test/unit/log/pytest_log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/server/controller/utils/utils.py` & `swanlab-0.3.4/test/unit/server/controller/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/utils/pytest_file.py` & `swanlab-0.3.4/test/unit/utils/pytest_file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/utils/pytest_key.py` & `swanlab-0.3.4/test/unit/utils/pytest_key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/test/unit/utils/pytest_package.py` & `swanlab-0.3.4/test/unit/utils/pytest_package.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/LICENSE` & `swanlab-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/pyproject.toml` & `swanlab-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.3/PKG-INFO` & `swanlab-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: swanlab
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python library for streamlined tracking and management of AI training processes.
 Project-URL: Homepage, https://swanhub.co
 Project-URL: Source, https://github.com/SwanHubX/SwanLab
 Project-URL: Bug Reports, https://github.com/SwanHubX/SwanLab/issues
 Project-URL: Documentation, https://geektechstudio.feishu.cn/wiki/space/7310593325374013444?ccm_open_type=lark_wiki_spaceLink&open_tab_from=wiki_home
 Author-email: Cunyue <team@swanhub.co>, Feudalman <team@swanhub.co>, ZeYi Lin <team@swanhub.co>, KashiwaByte <team@swanhub.co>
 License-Expression: Apache-2.0
@@ -127,16 +127,15 @@
 
 - Flexible recording of hyperparameters and experiment configurations.
 - **Supported metadata types**: scalar metrics, images, audio, text, etc.
 - **Supported chart types**: line graphs, media charts (images, audio, text), etc.
 - **Automatic logging**: console logging, GPU hardware, Git information, Python interpreter, list of Python libraries,
   code directory.
 
-**2. ⚡️ Comprehensive Framework Integration**: PyTorch, TensorFlow, PyTorch Lightning, 🤗HuggingFace Transformers, Tensorboard, 
-MMEngine, OpenAI, ZhipuAI, Hydra, etc.
+**2. ⚡️ Comprehensive Framework Integration**: PyTorch、Tensorflow、PyTorch Lightning、🤗HuggingFace、Transformers、MMEngine、Ultralytics、fastai、Tensorboard、OpenAI、ZhipuAI、Hydra、...
 
 **3. 📦 Organizing Experiments**: Centralized dashboard for efficiently managing multiple projects and experiments,
 providing an overview of training at a glance.
 
 **4. 🆚 Comparing Results**: Use online tables and paired charts to compare the hyperparameters and outcomes of different
 experiments, developing iterative inspiration.
 
@@ -732,14 +731,15 @@
 
 </details>
 
 <details>
 <summary>
   <strong> MMEngine(MMDetection etc.)</strong>
 </summary>
+<br>
 
 Integrate `SwanlabVisBackend` into MMEngine to enable automatic logging of training metrics by SwanLab.
 
 Add the following code snippet to your MM config file to start training:
 
 ```python
 custom_imports = dict(imports=["swanlab.integration.mmengine"], allow_failed_imports=False)
@@ -757,14 +757,40 @@
 visualizer = dict(
     type="Visualizer",
     vis_backends=vis_backends,
 )
 ```
 </details>
 
+<details>
+<summary>
+  <strong> Ultralytics</strong>
+</summary>
+<br>
+
+Integrating SwanLab into Ultralytics is very simple; you can use the `add_swanlab_callback` function:
+
+```python
+from ultralytics import YOLO
+from swanlab.integration.ultralytics import add_swanlab_callback
+
+model = YOLO("yolov8n.yaml")
+model.load()
+
+add_swanlab_callback(model)
+
+model.train(
+    data="./coco.yaml",
+    epochs=50, 
+    imgsz=320,
+)
+```
+
+</details>
+
 
 
 <br>
 
 ## 🆚 Comparison with familiar tools
 
 ### Tensorboard vs SwanLab
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: swanlab Version: 0.3.3 Summary: Python library for
+Metadata-Version: 2.3 Name: swanlab Version: 0.3.4 Summary: Python library for
 streamlined tracking and management of AI training processes. Project-URL:
 Homepage, https://swanhub.co Project-URL: Source, https://github.com/SwanHubX/
 SwanLab Project-URL: Bug Reports, https://github.com/SwanHubX/SwanLab/issues
 Project-URL: Documentation, https://geektechstudio.feishu.cn/wiki/space/
 7310593325374013444?ccm_open_type=lark_wiki_spaceLink&open_tab_from=wiki_home
 Author-email: Cunyue
 swanhub.co>, Feudalman
@@ -63,31 +63,31 @@
 Metrics and Tracking Hyperparameter**: Embed your machine learning pipeline
 with minimalistic code and track key training metrics. - Flexible recording of
 hyperparameters and experiment configurations. - **Supported metadata types**:
 scalar metrics, images, audio, text, etc. - **Supported chart types**: line
 graphs, media charts (images, audio, text), etc. - **Automatic logging**:
 console logging, GPU hardware, Git information, Python interpreter, list of
 Python libraries, code directory. **2. â¡ï¸ Comprehensive Framework
-Integration**: PyTorch, TensorFlow, PyTorch Lightning, ð¤HuggingFace
-Transformers, Tensorboard, MMEngine, OpenAI, ZhipuAI, Hydra, etc. **3. ð¦
-Organizing Experiments**: Centralized dashboard for efficiently managing
-multiple projects and experiments, providing an overview of training at a
-glance. **4. ð Comparing Results**: Use online tables and paired charts to
-compare the hyperparameters and outcomes of different experiments, developing
-iterative inspiration. **5. ð¥ Online Collaboration**: Collaborate with your
-team on training projects, supporting real-time synchronization of experiments
-under the same project, allowing you to synchronize training records of the
-team online and share insights and suggestions based on results. **6. âï¸
-Sharing Results**: Copy and send persistent URLs to share each experiment,
-efficiently send them to colleagues, or embed them in online notes. **7. ð»
-Self-hosting Support**: Supports offline mode with a self-hosted community
-version that also allows for dashboard viewing and experiment management. > \
-[!IMPORTANT] > > **Star Us**, You will receive all release notifications from
-GitHub without any delay ~ â­ï¸ ![star-us](https://raw.githubusercontent.com/
-SwanHubX/swanlab/main/readme_files/star-us.png)
+Integration**: PyTorchãTensorflowãPyTorch
+Lightningãð¤HuggingFaceãTransformersãMMEngineãUltralyticsãfastaiãTensorboardãOpenAIãZhipuAIãHydraã...
+**3. ð¦ Organizing Experiments**: Centralized dashboard for efficiently
+managing multiple projects and experiments, providing an overview of training
+at a glance. **4. ð Comparing Results**: Use online tables and paired charts
+to compare the hyperparameters and outcomes of different experiments,
+developing iterative inspiration. **5. ð¥ Online Collaboration**: Collaborate
+with your team on training projects, supporting real-time synchronization of
+experiments under the same project, allowing you to synchronize training
+records of the team online and share insights and suggestions based on results.
+**6. âï¸ Sharing Results**: Copy and send persistent URLs to share each
+experiment, efficiently send them to colleagues, or embed them in online notes.
+**7. ð» Self-hosting Support**: Supports offline mode with a self-hosted
+community version that also allows for dashboard viewing and experiment
+management. > \[!IMPORTANT] > > **Star Us**, You will receive all release
+notifications from GitHub without any delay ~ â­ï¸ ![star-us](https://
+raw.githubusercontent.com/SwanHubX/swanlab/main/readme_files/star-us.png)
 ## ð Quick Start ### 1.Installation ```bash pip install swanlab ``` ###
 2.Log in and get the API Key 1. **Free [Sign Up](https://swanlab.cn)** 2. **Log
 in to your account**, go to User Settings > [API Key](https://swanlab.cn/
 settings) and copy your API Key. 3. **Open your terminal and enter**: ```bash
 swanlab login ``` When prompted, enter your API Key and press Enter to complete
 the login. ### 3. Integrate SwanLab with Your Code ```python import swanlab #
 Create a new SwanLab experiment swanlab.init( project="my-first-ml", config=
@@ -274,22 +274,27 @@
 (1000)) metric = evaluate.load("accuracy") model =
 AutoModelForSequenceClassification.from_pretrained("bert-base-cased",
 num_labels=5) training_args = TrainingArguments( output_dir="test_trainer",
 report_to="none", num_train_epochs=3, logging_steps=50, ) swanlab_callback =
 SwanLabCallback(experiment_name="TransformersTest", cloud=False) trainer =
 Trainer( model=model, args=training_args, train_dataset=small_train_dataset,
 eval_dataset=small_eval_dataset, compute_metrics=compute_metrics, callbacks=
-[swanlab_callback], ) trainer.train() ``` MMMMEEnnggiinnee((MMMMDDeetteeccttiioonn eettcc..)) Integrate
-`SwanlabVisBackend` into MMEngine to enable automatic logging of training
-metrics by SwanLab. Add the following code snippet to your MM config file to
-start training: ```python custom_imports = dict(imports=
+[swanlab_callback], ) trainer.train() ``` MMMMEEnnggiinnee((MMMMDDeetteeccttiioonn eettcc..))
+Integrate `SwanlabVisBackend` into MMEngine to enable automatic logging of
+training metrics by SwanLab. Add the following code snippet to your MM config
+file to start training: ```python custom_imports = dict(imports=
 ["swanlab.integration.mmengine"], allow_failed_imports=False) vis_backends =
 [ dict( type="SwanlabVisBackend", save_dir="runs/swanlab", init_kwargs=
 { "project": "swanlab-mmengine", }, ), ] visualizer = dict( type="Visualizer",
-vis_backends=vis_backends, ) ```
+vis_backends=vis_backends, ) ``` UUllttrraallyyttiiccss
+Integrating SwanLab into Ultralytics is very simple; you can use the
+`add_swanlab_callback` function: ```python from ultralytics import YOLO from
+swanlab.integration.ultralytics import add_swanlab_callback model = YOLO
+("yolov8n.yaml") model.load() add_swanlab_callback(model) model.train( data="./
+coco.yaml", epochs=50, imgsz=320, ) ```
 ## ð Comparison with familiar tools ### Tensorboard vs SwanLab - **âï¸
 Online Usage Support**: With SwanLab, training experiments can be conveniently
 synchronized and saved in the cloud, allowing for remote monitoring of training
 progress, managing historical projects, sharing experiment links, sending real-
 time notification messages, and viewing experiments across multiple devices. In
 contrast, TensorBoard is an offline experiment tracking tool. - **ð¥
 Collaborative Multi-user Environment**: SwanLab facilitates easy management of
```

